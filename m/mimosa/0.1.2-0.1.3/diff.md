# Comparing `tmp/mimosa-0.1.2.tar.gz` & `tmp/mimosa-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mimosa-0.1.2.tar", last modified: Fri Jul 21 09:05:07 2023, max compression
+gzip compressed data, was "mimosa-0.1.3.tar", last modified: Fri Jul 21 11:20:16 2023, max compression
```

## Comparing `mimosa-0.1.2.tar` & `mimosa-0.1.3.tar`

### file list

```diff
@@ -1,188 +1,188 @@
-drwxrwxrwx   0        0        0        0 2023-07-21 09:05:07.465590 mimosa-0.1.2/
--rw-rw-rw-   0        0        0       66 2020-05-27 06:46:03.000000 mimosa-0.1.2/.gitattributes
--rw-rw-rw-   0        0        0     2098 2021-05-12 09:46:36.000000 mimosa-0.1.2/.gitignore
--rw-rw-rw-   0        0        0    35822 2020-05-18 11:44:25.000000 mimosa-0.1.2/LICENSE
--rw-rw-rw-   0        0        0       26 2023-07-21 06:53:35.000000 mimosa-0.1.2/MANIFEST.in
--rw-rw-rw-   0        0        0     5763 2023-07-21 09:05:07.463590 mimosa-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     5477 2023-07-21 06:53:35.000000 mimosa-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-21 09:05:06.937629 mimosa-0.1.2/mimosa/
--rw-rw-rw-   0        0        0      108 2023-07-21 07:52:23.000000 mimosa-0.1.2/mimosa/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 09:05:06.977151 mimosa-0.1.2/mimosa/__pycache__/
--rw-rw-rw-   0        0        0      275 2023-07-21 07:54:49.000000 mimosa-0.1.2/mimosa/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0     3648 2023-07-21 07:42:48.000000 mimosa-0.1.2/mimosa/__pycache__/abstract_model.cpython-310.pyc
--rw-rw-rw-   0        0        0     6915 2023-07-21 07:41:57.000000 mimosa-0.1.2/mimosa/__pycache__/mimosa.cpython-310.pyc
--rw-rw-rw-   0        0        0     5160 2023-07-21 07:41:41.000000 mimosa-0.1.2/mimosa/abstract_model.py
-drwxrwxrwx   0        0        0        0 2023-07-21 09:05:06.987131 mimosa-0.1.2/mimosa/common/
--rw-rw-rw-   0        0        0     1206 2023-07-21 06:54:00.000000 mimosa-0.1.2/mimosa/common/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 09:05:07.006446 mimosa-0.1.2/mimosa/common/__pycache__/
--rw-rw-rw-   0        0        0     1361 2023-07-21 07:41:57.000000 mimosa-0.1.2/mimosa/common/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0     1405 2023-07-21 07:42:48.000000 mimosa-0.1.2/mimosa/common/__pycache__/economics.cpython-310.pyc
--rw-rw-rw-   0        0        0     9297 2023-07-21 07:41:59.000000 mimosa-0.1.2/mimosa/common/__pycache__/pyomo_utils.cpython-310.pyc
--rw-rw-rw-   0        0        0     3475 2023-07-21 07:42:42.000000 mimosa-0.1.2/mimosa/common/__pycache__/units.cpython-310.pyc
--rw-rw-rw-   0        0        0     1705 2023-07-21 07:42:41.000000 mimosa-0.1.2/mimosa/common/__pycache__/utils.cpython-310.pyc
-drwxrwxrwx   0        0        0        0 2023-07-21 09:05:07.008453 mimosa-0.1.2/mimosa/common/config/
--rw-rw-rw-   0        0        0        0 2023-07-21 06:54:00.000000 mimosa-0.1.2/mimosa/common/config/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 09:05:07.017439 mimosa-0.1.2/mimosa/common/config/__pycache__/
--rw-rw-rw-   0        0        0      191 2023-07-21 07:42:48.000000 mimosa-0.1.2/mimosa/common/config/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0     2230 2023-07-21 07:54:51.000000 mimosa-0.1.2/mimosa/common/config/__pycache__/parseconfig.cpython-310.pyc
--rw-rw-rw-   0        0        0     2429 2023-07-21 07:54:34.000000 mimosa-0.1.2/mimosa/common/config/parseconfig.py
-drwxrwxrwx   0        0        0        0 2023-07-21 09:05:07.026478 mimosa-0.1.2/mimosa/common/config/utils/
--rw-rw-rw-   0        0        0      112 2023-07-21 06:54:00.000000 mimosa-0.1.2/mimosa/common/config/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 09:05:07.037148 mimosa-0.1.2/mimosa/common/config/utils/__pycache__/
--rw-rw-rw-   0        0        0      352 2023-07-21 07:42:48.000000 mimosa-0.1.2/mimosa/common/config/utils/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0     1190 2023-07-21 07:42:48.000000 mimosa-0.1.2/mimosa/common/config/utils/__pycache__/nested_dict.cpython-310.pyc
--rw-rw-rw-   0        0        0     9387 2023-07-21 07:42:48.000000 mimosa-0.1.2/mimosa/common/config/utils/__pycache__/parsers.cpython-310.pyc
--rw-rw-rw-   0        0        0      969 2023-07-21 06:54:00.000000 mimosa-0.1.2/mimosa/common/config/utils/nested_dict.py
--rw-rw-rw-   0        0        0     8454 2023-07-21 07:41:43.000000 mimosa-0.1.2/mimosa/common/config/utils/parsers.py
-drwxrwxrwx   0        0        0        0 2023-07-21 09:05:07.048032 mimosa-0.1.2/mimosa/common/data/
--rw-rw-rw-   0        0        0       36 2023-07-21 06:54:00.000000 mimosa-0.1.2/mimosa/common/data/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 09:05:07.066745 mimosa-0.1.2/mimosa/common/data/__pycache__/
--rw-rw-rw-   0        0        0      232 2023-07-21 07:42:44.000000 mimosa-0.1.2/mimosa/common/data/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0     6111 2023-07-21 07:42:44.000000 mimosa-0.1.2/mimosa/common/data/__pycache__/datastore.cpython-310.pyc
--rw-rw-rw-   0        0        0     1235 2023-07-21 07:42:48.000000 mimosa-0.1.2/mimosa/common/data/__pycache__/utils.cpython-310.pyc
--rw-rw-rw-   0        0        0     6574 2023-07-21 07:42:30.000000 mimosa-0.1.2/mimosa/common/data/datastore.py
--rw-rw-rw-   0        0        0     1463 2023-07-21 06:54:00.000000 mimosa-0.1.2/mimosa/common/data/utils.py
--rw-rw-rw-   0        0        0     1419 2023-07-21 07:41:43.000000 mimosa-0.1.2/mimosa/common/economics.py
--rw-rw-rw-   0        0        0     8234 2023-07-21 07:41:43.000000 mimosa-0.1.2/mimosa/common/pyomo_utils.py
-drwxrwxrwx   0        0        0        0 2023-07-21 09:05:07.083709 mimosa-0.1.2/mimosa/common/regional_params/
--rw-rw-rw-   0        0        0       38 2023-07-21 06:54:00.000000 mimosa-0.1.2/mimosa/common/regional_params/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 09:05:07.098017 mimosa-0.1.2/mimosa/common/regional_params/__pycache__/
--rw-rw-rw-   0        0        0      247 2023-07-21 07:42:48.000000 mimosa-0.1.2/mimosa/common/regional_params/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0     2765 2023-07-21 07:42:48.000000 mimosa-0.1.2/mimosa/common/regional_params/__pycache__/main.cpython-310.pyc
--rw-rw-rw-   0        0        0     2404 2023-07-21 07:42:48.000000 mimosa-0.1.2/mimosa/common/regional_params/__pycache__/region_mappers.cpython-310.pyc
--rw-rw-rw-   0        0        0     1334 2023-07-21 07:42:48.000000 mimosa-0.1.2/mimosa/common/regional_params/__pycache__/regional_param_container.cpython-310.pyc
--rw-rw-rw-   0        0        0     2754 2023-07-21 06:54:00.000000 mimosa-0.1.2/mimosa/common/regional_params/main.py
--rw-rw-rw-   0        0        0     2772 2023-07-21 07:42:30.000000 mimosa-0.1.2/mimosa/common/regional_params/region_mappers.py
--rw-rw-rw-   0        0        0     1340 2023-07-21 07:42:30.000000 mimosa-0.1.2/mimosa/common/regional_params/regional_param_container.py
--rw-rw-rw-   0        0        0     3579 2023-07-21 07:42:29.000000 mimosa-0.1.2/mimosa/common/units.py
--rw-rw-rw-   0        0        0     1220 2023-07-21 07:42:29.000000 mimosa-0.1.2/mimosa/common/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-21 09:05:07.117414 mimosa-0.1.2/mimosa/components/
--rw-rw-rw-   0        0        0        0 2023-07-21 06:54:00.000000 mimosa-0.1.2/mimosa/components/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 09:05:07.146226 mimosa-0.1.2/mimosa/components/__pycache__/
--rw-rw-rw-   0        0        0      188 2023-07-21 07:42:48.000000 mimosa-0.1.2/mimosa/components/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0     4889 2023-07-21 07:42:48.000000 mimosa-0.1.2/mimosa/components/__pycache__/abatement.cpython-310.pyc
--rw-rw-rw-   0        0        0     3844 2023-07-21 07:42:48.000000 mimosa-0.1.2/mimosa/components/__pycache__/burdensharing.cpython-310.pyc
--rw-rw-rw-   0        0        0     3333 2023-07-21 07:42:48.000000 mimosa-0.1.2/mimosa/components/__pycache__/cobbdouglas.cpython-310.pyc
--rw-rw-rw-   0        0        0     6923 2023-07-21 07:42:48.000000 mimosa-0.1.2/mimosa/components/__pycache__/emissions.cpython-310.pyc
--rw-rw-rw-   0        0        0     3700 2023-07-21 07:42:48.000000 mimosa-0.1.2/mimosa/components/__pycache__/sealevelrise.cpython-310.pyc
--rw-rw-rw-   0        0        0     5469 2023-07-21 07:41:44.000000 mimosa-0.1.2/mimosa/components/abatement.py
--rw-rw-rw-   0        0        0     4025 2023-07-21 07:41:44.000000 mimosa-0.1.2/mimosa/components/burdensharing.py
--rw-rw-rw-   0        0        0     3697 2023-07-21 07:41:44.000000 mimosa-0.1.2/mimosa/components/cobbdouglas.py
-drwxrwxrwx   0        0        0        0 2023-07-21 09:05:07.156242 mimosa-0.1.2/mimosa/components/damages/
--rw-rw-rw-   0        0        0      116 2023-07-21 06:54:00.000000 mimosa-0.1.2/mimosa/components/damages/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 09:05:07.185413 mimosa-0.1.2/mimosa/components/damages/__pycache__/
--rw-rw-rw-   0        0        0      364 2023-07-21 07:42:48.000000 mimosa-0.1.2/mimosa/components/damages/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0     4552 2023-07-21 07:42:48.000000 mimosa-0.1.2/mimosa/components/damages/__pycache__/ad_rice2010.cpython-310.pyc
--rw-rw-rw-   0        0        0     4166 2023-07-21 07:42:48.000000 mimosa-0.1.2/mimosa/components/damages/__pycache__/ad_rice2012.cpython-310.pyc
--rw-rw-rw-   0        0        0     4299 2023-07-21 07:42:48.000000 mimosa-0.1.2/mimosa/components/damages/__pycache__/ad_witch.cpython-310.pyc
--rw-rw-rw-   0        0        0     3277 2023-07-21 07:42:48.000000 mimosa-0.1.2/mimosa/components/damages/__pycache__/coacch.cpython-310.pyc
--rw-rw-rw-   0        0        0     1274 2023-07-21 07:42:48.000000 mimosa-0.1.2/mimosa/components/damages/__pycache__/nodamage.cpython-310.pyc
--rw-rw-rw-   0        0        0     5331 2023-07-21 07:41:45.000000 mimosa-0.1.2/mimosa/components/damages/ad_rice2010.py
--rw-rw-rw-   0        0        0     4874 2023-07-21 07:41:45.000000 mimosa-0.1.2/mimosa/components/damages/ad_rice2012.py
--rw-rw-rw-   0        0        0     6688 2023-07-21 07:41:46.000000 mimosa-0.1.2/mimosa/components/damages/ad_witch.py
--rw-rw-rw-   0        0        0     4260 2023-07-21 07:41:45.000000 mimosa-0.1.2/mimosa/components/damages/coacch.py
--rw-rw-rw-   0        0        0      971 2023-07-21 07:41:45.000000 mimosa-0.1.2/mimosa/components/damages/nodamage.py
--rw-rw-rw-   0        0        0    10151 2023-07-21 07:41:44.000000 mimosa-0.1.2/mimosa/components/emissions.py
-drwxrwxrwx   0        0        0        0 2023-07-21 09:05:07.197697 mimosa-0.1.2/mimosa/components/emissiontrade/
--rw-rw-rw-   0        0        0      112 2023-07-21 06:54:00.000000 mimosa-0.1.2/mimosa/components/emissiontrade/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 09:05:07.216142 mimosa-0.1.2/mimosa/components/emissiontrade/__pycache__/
--rw-rw-rw-   0        0        0      348 2023-07-21 07:42:48.000000 mimosa-0.1.2/mimosa/components/emissiontrade/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0     3898 2023-07-21 07:42:48.000000 mimosa-0.1.2/mimosa/components/emissiontrade/__pycache__/emissiontrade.cpython-310.pyc
--rw-rw-rw-   0        0        0     2968 2023-07-21 07:42:48.000000 mimosa-0.1.2/mimosa/components/emissiontrade/__pycache__/globalcostpool.cpython-310.pyc
--rw-rw-rw-   0        0        0     1414 2023-07-21 07:42:48.000000 mimosa-0.1.2/mimosa/components/emissiontrade/__pycache__/notrade.cpython-310.pyc
--rw-rw-rw-   0        0        0     5274 2023-07-21 07:41:45.000000 mimosa-0.1.2/mimosa/components/emissiontrade/emissiontrade.py
--rw-rw-rw-   0        0        0     3276 2023-07-21 07:41:44.000000 mimosa-0.1.2/mimosa/components/emissiontrade/globalcostpool.py
--rw-rw-rw-   0        0        0     1131 2023-07-21 07:41:44.000000 mimosa-0.1.2/mimosa/components/emissiontrade/notrade.py
-drwxrwxrwx   0        0        0        0 2023-07-21 09:05:07.226704 mimosa-0.1.2/mimosa/components/financialtransfer/
--rw-rw-rw-   0        0        0      105 2023-07-21 06:54:00.000000 mimosa-0.1.2/mimosa/components/financialtransfer/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 09:05:07.236238 mimosa-0.1.2/mimosa/components/financialtransfer/__pycache__/
--rw-rw-rw-   0        0        0      336 2023-07-21 07:42:48.000000 mimosa-0.1.2/mimosa/components/financialtransfer/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0     2230 2023-07-21 07:42:48.000000 mimosa-0.1.2/mimosa/components/financialtransfer/__pycache__/globaldamagepool.cpython-310.pyc
--rw-rw-rw-   0        0        0     1093 2023-07-21 07:42:48.000000 mimosa-0.1.2/mimosa/components/financialtransfer/__pycache__/notransfer.cpython-310.pyc
--rw-rw-rw-   0        0        0     1968 2023-07-21 07:41:44.000000 mimosa-0.1.2/mimosa/components/financialtransfer/globaldamagepool.py
--rw-rw-rw-   0        0        0      939 2023-07-21 07:41:44.000000 mimosa-0.1.2/mimosa/components/financialtransfer/notransfer.py
-drwxrwxrwx   0        0        0        0 2023-07-21 09:05:07.246457 mimosa-0.1.2/mimosa/components/objective/
--rw-rw-rw-   0        0        0      101 2023-07-21 06:54:00.000000 mimosa-0.1.2/mimosa/components/objective/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 09:05:07.257606 mimosa-0.1.2/mimosa/components/objective/__pycache__/
--rw-rw-rw-   0        0        0      322 2023-07-21 07:42:48.000000 mimosa-0.1.2/mimosa/components/objective/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0     2118 2023-07-21 07:42:48.000000 mimosa-0.1.2/mimosa/components/objective/__pycache__/globalcosts.cpython-310.pyc
--rw-rw-rw-   0        0        0     1736 2023-07-21 07:42:48.000000 mimosa-0.1.2/mimosa/components/objective/__pycache__/utility.cpython-310.pyc
--rw-rw-rw-   0        0        0     1558 2023-07-21 07:41:44.000000 mimosa-0.1.2/mimosa/components/objective/globalcosts.py
--rw-rw-rw-   0        0        0     1713 2023-07-21 07:41:44.000000 mimosa-0.1.2/mimosa/components/objective/utility.py
--rw-rw-rw-   0        0        0     4213 2023-07-21 07:41:44.000000 mimosa-0.1.2/mimosa/components/sealevelrise.py
-drwxrwxrwx   0        0        0        0 2023-07-21 09:05:07.267020 mimosa-0.1.2/mimosa/components/welfare/
--rw-rw-rw-   0        0        0      165 2023-07-21 06:54:00.000000 mimosa-0.1.2/mimosa/components/welfare/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 09:05:07.277630 mimosa-0.1.2/mimosa/components/welfare/__pycache__/
--rw-rw-rw-   0        0        0      391 2023-07-21 07:42:48.000000 mimosa-0.1.2/mimosa/components/welfare/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0     1882 2023-07-21 07:42:48.000000 mimosa-0.1.2/mimosa/components/welfare/__pycache__/inequal_aversion_elasmu.cpython-310.pyc
--rw-rw-rw-   0        0        0     2368 2023-07-21 07:42:48.000000 mimosa-0.1.2/mimosa/components/welfare/__pycache__/inequal_aversion_general.cpython-310.pyc
--rw-rw-rw-   0        0        0     2133 2023-07-21 07:42:48.000000 mimosa-0.1.2/mimosa/components/welfare/__pycache__/inequal_aversion_zero.cpython-310.pyc
--rw-rw-rw-   0        0        0     1456 2023-07-21 07:41:44.000000 mimosa-0.1.2/mimosa/components/welfare/inequal_aversion_elasmu.py
--rw-rw-rw-   0        0        0     2048 2023-07-21 07:41:44.000000 mimosa-0.1.2/mimosa/components/welfare/inequal_aversion_general.py
--rw-rw-rw-   0        0        0     1663 2023-07-21 07:41:44.000000 mimosa-0.1.2/mimosa/components/welfare/inequal_aversion_zero.py
-drwxrwxrwx   0        0        0        0 2023-07-21 09:05:07.286169 mimosa-0.1.2/mimosa/concrete_model/
--rw-rw-rw-   0        0        0        0 2023-07-21 06:54:00.000000 mimosa-0.1.2/mimosa/concrete_model/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 09:05:07.286169 mimosa-0.1.2/mimosa/concrete_model/__pycache__/
--rw-rw-rw-   0        0        0      192 2023-07-21 07:42:48.000000 mimosa-0.1.2/mimosa/concrete_model/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0     8590 2023-07-21 07:42:48.000000 mimosa-0.1.2/mimosa/concrete_model/__pycache__/instantiate_params.cpython-310.pyc
--rw-rw-rw-   0        0        0    15078 2023-07-21 07:41:42.000000 mimosa-0.1.2/mimosa/concrete_model/instantiate_params.py
-drwxrwxrwx   0        0        0        0 2023-07-21 09:05:07.308512 mimosa-0.1.2/mimosa/concrete_model/simulation_mode/
--rw-rw-rw-   0        0        0       39 2023-07-21 06:54:00.000000 mimosa-0.1.2/mimosa/concrete_model/simulation_mode/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 09:05:07.336619 mimosa-0.1.2/mimosa/concrete_model/simulation_mode/__pycache__/
--rw-rw-rw-   0        0        0      256 2023-07-21 07:42:48.000000 mimosa-0.1.2/mimosa/concrete_model/simulation_mode/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0      677 2023-07-21 07:42:48.000000 mimosa-0.1.2/mimosa/concrete_model/simulation_mode/__pycache__/deactivate_constraints.cpython-310.pyc
--rw-rw-rw-   0        0        0     1046 2023-07-21 07:42:48.000000 mimosa-0.1.2/mimosa/concrete_model/simulation_mode/__pycache__/main.cpython-310.pyc
--rw-rw-rw-   0        0        0     2504 2023-07-21 07:42:48.000000 mimosa-0.1.2/mimosa/concrete_model/simulation_mode/__pycache__/set_constraints.cpython-310.pyc
--rw-rw-rw-   0        0        0     2101 2023-07-21 07:42:48.000000 mimosa-0.1.2/mimosa/concrete_model/simulation_mode/__pycache__/utils.cpython-310.pyc
--rw-rw-rw-   0        0        0      493 2023-07-21 06:54:00.000000 mimosa-0.1.2/mimosa/concrete_model/simulation_mode/deactivate_constraints.py
--rw-rw-rw-   0        0        0      907 2023-07-21 07:41:42.000000 mimosa-0.1.2/mimosa/concrete_model/simulation_mode/main.py
--rw-rw-rw-   0        0        0     3369 2023-07-21 07:41:42.000000 mimosa-0.1.2/mimosa/concrete_model/simulation_mode/set_constraints.py
--rw-rw-rw-   0        0        0     1557 2023-07-21 07:41:42.000000 mimosa-0.1.2/mimosa/concrete_model/simulation_mode/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-21 09:05:07.346131 mimosa-0.1.2/mimosa/export/
--rw-rw-rw-   0        0        0      202 2023-07-21 06:54:00.000000 mimosa-0.1.2/mimosa/export/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 09:05:07.357872 mimosa-0.1.2/mimosa/export/__pycache__/
--rw-rw-rw-   0        0        0      418 2023-07-21 07:42:48.000000 mimosa-0.1.2/mimosa/export/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0     3355 2023-07-21 07:42:48.000000 mimosa-0.1.2/mimosa/export/__pycache__/plot.cpython-310.pyc
--rw-rw-rw-   0        0        0     2567 2023-07-21 07:42:48.000000 mimosa-0.1.2/mimosa/export/__pycache__/save.cpython-310.pyc
--rw-rw-rw-   0        0        0     5349 2023-07-21 07:42:48.000000 mimosa-0.1.2/mimosa/export/__pycache__/utils.cpython-310.pyc
--rw-rw-rw-   0        0        0     5262 2023-07-21 07:41:42.000000 mimosa-0.1.2/mimosa/export/plot.py
--rw-rw-rw-   0        0        0     3110 2023-07-21 07:41:42.000000 mimosa-0.1.2/mimosa/export/save.py
--rw-rw-rw-   0        0        0     5836 2023-07-21 09:03:34.000000 mimosa-0.1.2/mimosa/export/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-21 09:05:06.908449 mimosa-0.1.2/mimosa/inputdata/
-drwxrwxrwx   0        0        0        0 2023-07-21 09:05:07.380423 mimosa-0.1.2/mimosa/inputdata/config/
--rw-rw-rw-   0        0        0       13 2023-07-21 06:54:00.000000 mimosa-0.1.2/mimosa/inputdata/config/config.yaml
--rw-rw-rw-   0        0        0     2296 2023-07-21 07:42:29.000000 mimosa-0.1.2/mimosa/inputdata/config/config_R5.yaml
--rw-rw-rw-   0        0        0    13790 2023-07-21 07:42:30.000000 mimosa-0.1.2/mimosa/inputdata/config/config_default.yaml
--rw-rw-rw-   0        0        0      154 2023-07-21 06:54:00.000000 mimosa-0.1.2/mimosa/inputdata/config/default_units.yaml
--rw-rw-rw-   0        0        0      456 2023-07-21 06:54:00.000000 mimosa-0.1.2/mimosa/inputdata/config/extra_units.txt
-drwxrwxrwx   0        0        0        0 2023-07-21 09:05:07.387433 mimosa-0.1.2/mimosa/inputdata/data/
--rw-rw-rw-   0        0        0    89096 2023-07-21 06:54:00.000000 mimosa-0.1.2/mimosa/inputdata/data/data_IMAGE_SSP.csv
--rw-rw-rw-   0        0        0    89101 2023-07-21 06:54:00.000000 mimosa-0.1.2/mimosa/inputdata/data/data_IMAGE_SSP_harmonised_2020.csv
-drwxrwxrwx   0        0        0        0 2023-07-21 09:05:07.420747 mimosa-0.1.2/mimosa/inputdata/params/
--rw-rw-rw-   0        0        0      491 2023-07-21 06:54:00.000000 mimosa-0.1.2/mimosa/inputdata/params/ADRICE2010.csv
--rw-rw-rw-   0        0        0      593 2023-07-21 06:54:00.000000 mimosa-0.1.2/mimosa/inputdata/params/ADRICE2012.csv
--rw-rw-rw-   0        0        0    34077 2023-07-21 06:54:00.000000 mimosa-0.1.2/mimosa/inputdata/params/COACCH.csv
--rw-rw-rw-   0        0        0      321 2023-07-21 06:54:00.000000 mimosa-0.1.2/mimosa/inputdata/params/economics.csv
--rw-rw-rw-   0        0        0     7044 2023-07-21 06:54:00.000000 mimosa-0.1.2/mimosa/inputdata/params/mac.csv
-drwxrwxrwx   0        0        0        0 2023-07-21 09:05:07.451592 mimosa-0.1.2/mimosa/inputdata/regions/
--rw-rw-rw-   0        0        0      286 2023-07-21 06:54:00.000000 mimosa-0.1.2/mimosa/inputdata/regions/IMAGE26_ADRICE2010.csv
--rw-rw-rw-   0        0        0      280 2023-07-21 06:54:00.000000 mimosa-0.1.2/mimosa/inputdata/regions/IMAGE26_ADRICE2012.csv
--rw-rw-rw-   0        0        0      337 2023-07-21 06:54:00.000000 mimosa-0.1.2/mimosa/inputdata/regions/IMAGE26_COACCH.csv
--rw-rw-rw-   0        0        0   167460 2023-07-21 06:54:00.000000 mimosa-0.1.2/mimosa/inputdata/regions/IMAGE26_regions.json
--rw-rw-rw-   0        0        0   123689 2023-07-21 06:54:00.000000 mimosa-0.1.2/mimosa/inputdata/regions/R5_regions.json
--rw-rw-rw-   0        0        0    21007 2023-07-21 06:54:00.000000 mimosa-0.1.2/mimosa/inputdata/regions/country_ISO_codes.csv
--rw-rw-rw-   0        0        0     8217 2023-07-21 07:41:41.000000 mimosa-0.1.2/mimosa/mimosa.py
-drwxrwxrwx   0        0        0        0 2023-07-21 09:05:07.457590 mimosa-0.1.2/mimosa/socialcostofcarbon/
--rw-rw-rw-   0        0        0        0 2023-07-21 06:54:00.000000 mimosa-0.1.2/mimosa/socialcostofcarbon/__init__.py
--rw-rw-rw-   0        0        0     5546 2023-07-21 07:41:42.000000 mimosa-0.1.2/mimosa/socialcostofcarbon/scc.py
-drwxrwxrwx   0        0        0        0 2023-07-21 09:05:06.967702 mimosa-0.1.2/mimosa.egg-info/
--rw-rw-rw-   0        0        0     5763 2023-07-21 09:05:06.000000 mimosa-0.1.2/mimosa.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     6851 2023-07-21 09:05:06.000000 mimosa-0.1.2/mimosa.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-21 09:05:06.000000 mimosa-0.1.2/mimosa.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2023-07-21 09:05:06.000000 mimosa-0.1.2/mimosa.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-21 09:05:06.000000 mimosa-0.1.2/mimosa.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-07-21 08:04:00.000000 mimosa-0.1.2/pyproject.toml
--rw-rw-rw-   0        0        0       61 2023-07-21 06:53:35.000000 mimosa-0.1.2/requirements.txt
--rw-rw-rw-   0        0        0      217 2023-07-21 07:56:33.000000 mimosa-0.1.2/run.py
--rw-rw-rw-   0        0        0       42 2023-07-21 09:05:07.466593 mimosa-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      621 2023-07-21 09:04:46.000000 mimosa-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-21 11:20:16.101244 mimosa-0.1.3/
+-rw-rw-rw-   0        0        0       66 2020-05-27 06:46:03.000000 mimosa-0.1.3/.gitattributes
+-rw-rw-rw-   0        0        0     2098 2021-05-12 09:46:36.000000 mimosa-0.1.3/.gitignore
+-rw-rw-rw-   0        0        0    35822 2020-05-18 11:44:25.000000 mimosa-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0       26 2023-07-21 06:53:35.000000 mimosa-0.1.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     5603 2023-07-21 11:20:16.101244 mimosa-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     5308 2023-07-21 11:18:29.000000 mimosa-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-21 11:20:15.684654 mimosa-0.1.3/mimosa/
+-rw-rw-rw-   0        0        0      108 2023-07-21 11:19:18.000000 mimosa-0.1.3/mimosa/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 11:20:15.738051 mimosa-0.1.3/mimosa/__pycache__/
+-rw-rw-rw-   0        0        0      275 2023-07-21 07:54:49.000000 mimosa-0.1.3/mimosa/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0     3648 2023-07-21 07:42:48.000000 mimosa-0.1.3/mimosa/__pycache__/abstract_model.cpython-310.pyc
+-rw-rw-rw-   0        0        0     6915 2023-07-21 07:41:57.000000 mimosa-0.1.3/mimosa/__pycache__/mimosa.cpython-310.pyc
+-rw-rw-rw-   0        0        0     5160 2023-07-21 11:19:18.000000 mimosa-0.1.3/mimosa/abstract_model.py
+drwxrwxrwx   0        0        0        0 2023-07-21 11:20:15.758571 mimosa-0.1.3/mimosa/common/
+-rw-rw-rw-   0        0        0     1206 2023-07-21 11:19:18.000000 mimosa-0.1.3/mimosa/common/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 11:20:15.774197 mimosa-0.1.3/mimosa/common/__pycache__/
+-rw-rw-rw-   0        0        0     1361 2023-07-21 07:41:57.000000 mimosa-0.1.3/mimosa/common/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1405 2023-07-21 07:42:48.000000 mimosa-0.1.3/mimosa/common/__pycache__/economics.cpython-310.pyc
+-rw-rw-rw-   0        0        0     9297 2023-07-21 07:41:59.000000 mimosa-0.1.3/mimosa/common/__pycache__/pyomo_utils.cpython-310.pyc
+-rw-rw-rw-   0        0        0     3475 2023-07-21 07:42:42.000000 mimosa-0.1.3/mimosa/common/__pycache__/units.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1705 2023-07-21 07:42:41.000000 mimosa-0.1.3/mimosa/common/__pycache__/utils.cpython-310.pyc
+drwxrwxrwx   0        0        0        0 2023-07-21 11:20:15.774197 mimosa-0.1.3/mimosa/common/config/
+-rw-rw-rw-   0        0        0        0 2023-07-21 11:19:18.000000 mimosa-0.1.3/mimosa/common/config/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 11:20:15.774197 mimosa-0.1.3/mimosa/common/config/__pycache__/
+-rw-rw-rw-   0        0        0      191 2023-07-21 07:42:48.000000 mimosa-0.1.3/mimosa/common/config/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2230 2023-07-21 07:54:51.000000 mimosa-0.1.3/mimosa/common/config/__pycache__/parseconfig.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2429 2023-07-21 11:19:18.000000 mimosa-0.1.3/mimosa/common/config/parseconfig.py
+drwxrwxrwx   0        0        0        0 2023-07-21 11:20:15.789824 mimosa-0.1.3/mimosa/common/config/utils/
+-rw-rw-rw-   0        0        0      112 2023-07-21 11:19:18.000000 mimosa-0.1.3/mimosa/common/config/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 11:20:15.789824 mimosa-0.1.3/mimosa/common/config/utils/__pycache__/
+-rw-rw-rw-   0        0        0      352 2023-07-21 07:42:48.000000 mimosa-0.1.3/mimosa/common/config/utils/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1190 2023-07-21 07:42:48.000000 mimosa-0.1.3/mimosa/common/config/utils/__pycache__/nested_dict.cpython-310.pyc
+-rw-rw-rw-   0        0        0     9387 2023-07-21 07:42:48.000000 mimosa-0.1.3/mimosa/common/config/utils/__pycache__/parsers.cpython-310.pyc
+-rw-rw-rw-   0        0        0      969 2023-07-21 11:19:18.000000 mimosa-0.1.3/mimosa/common/config/utils/nested_dict.py
+-rw-rw-rw-   0        0        0     8454 2023-07-21 11:19:18.000000 mimosa-0.1.3/mimosa/common/config/utils/parsers.py
+drwxrwxrwx   0        0        0        0 2023-07-21 11:20:15.805445 mimosa-0.1.3/mimosa/common/data/
+-rw-rw-rw-   0        0        0       36 2023-07-21 11:19:18.000000 mimosa-0.1.3/mimosa/common/data/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 11:20:15.813051 mimosa-0.1.3/mimosa/common/data/__pycache__/
+-rw-rw-rw-   0        0        0      232 2023-07-21 07:42:44.000000 mimosa-0.1.3/mimosa/common/data/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0     6111 2023-07-21 07:42:44.000000 mimosa-0.1.3/mimosa/common/data/__pycache__/datastore.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1235 2023-07-21 07:42:48.000000 mimosa-0.1.3/mimosa/common/data/__pycache__/utils.cpython-310.pyc
+-rw-rw-rw-   0        0        0     6574 2023-07-21 11:19:18.000000 mimosa-0.1.3/mimosa/common/data/datastore.py
+-rw-rw-rw-   0        0        0     1463 2023-07-21 11:19:18.000000 mimosa-0.1.3/mimosa/common/data/utils.py
+-rw-rw-rw-   0        0        0     1419 2023-07-21 11:19:18.000000 mimosa-0.1.3/mimosa/common/economics.py
+-rw-rw-rw-   0        0        0     8234 2023-07-21 11:19:18.000000 mimosa-0.1.3/mimosa/common/pyomo_utils.py
+drwxrwxrwx   0        0        0        0 2023-07-21 11:20:15.822557 mimosa-0.1.3/mimosa/common/regional_params/
+-rw-rw-rw-   0        0        0       38 2023-07-21 11:19:18.000000 mimosa-0.1.3/mimosa/common/regional_params/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 11:20:15.838186 mimosa-0.1.3/mimosa/common/regional_params/__pycache__/
+-rw-rw-rw-   0        0        0      247 2023-07-21 07:42:48.000000 mimosa-0.1.3/mimosa/common/regional_params/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2765 2023-07-21 07:42:48.000000 mimosa-0.1.3/mimosa/common/regional_params/__pycache__/main.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2404 2023-07-21 07:42:48.000000 mimosa-0.1.3/mimosa/common/regional_params/__pycache__/region_mappers.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1334 2023-07-21 07:42:48.000000 mimosa-0.1.3/mimosa/common/regional_params/__pycache__/regional_param_container.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2754 2023-07-21 11:19:18.000000 mimosa-0.1.3/mimosa/common/regional_params/main.py
+-rw-rw-rw-   0        0        0     2772 2023-07-21 11:19:18.000000 mimosa-0.1.3/mimosa/common/regional_params/region_mappers.py
+-rw-rw-rw-   0        0        0     1340 2023-07-21 11:19:18.000000 mimosa-0.1.3/mimosa/common/regional_params/regional_param_container.py
+-rw-rw-rw-   0        0        0     3579 2023-07-21 11:19:18.000000 mimosa-0.1.3/mimosa/common/units.py
+-rw-rw-rw-   0        0        0     1220 2023-07-21 11:19:18.000000 mimosa-0.1.3/mimosa/common/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-21 11:20:15.838186 mimosa-0.1.3/mimosa/components/
+-rw-rw-rw-   0        0        0        0 2023-07-21 11:19:18.000000 mimosa-0.1.3/mimosa/components/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 11:20:15.869432 mimosa-0.1.3/mimosa/components/__pycache__/
+-rw-rw-rw-   0        0        0      188 2023-07-21 07:42:48.000000 mimosa-0.1.3/mimosa/components/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0     4889 2023-07-21 07:42:48.000000 mimosa-0.1.3/mimosa/components/__pycache__/abatement.cpython-310.pyc
+-rw-rw-rw-   0        0        0     3844 2023-07-21 07:42:48.000000 mimosa-0.1.3/mimosa/components/__pycache__/burdensharing.cpython-310.pyc
+-rw-rw-rw-   0        0        0     3333 2023-07-21 07:42:48.000000 mimosa-0.1.3/mimosa/components/__pycache__/cobbdouglas.cpython-310.pyc
+-rw-rw-rw-   0        0        0     6923 2023-07-21 07:42:48.000000 mimosa-0.1.3/mimosa/components/__pycache__/emissions.cpython-310.pyc
+-rw-rw-rw-   0        0        0     3700 2023-07-21 07:42:48.000000 mimosa-0.1.3/mimosa/components/__pycache__/sealevelrise.cpython-310.pyc
+-rw-rw-rw-   0        0        0     5469 2023-07-21 11:19:18.000000 mimosa-0.1.3/mimosa/components/abatement.py
+-rw-rw-rw-   0        0        0     4025 2023-07-21 11:19:18.000000 mimosa-0.1.3/mimosa/components/burdensharing.py
+-rw-rw-rw-   0        0        0     3697 2023-07-21 11:19:18.000000 mimosa-0.1.3/mimosa/components/cobbdouglas.py
+drwxrwxrwx   0        0        0        0 2023-07-21 11:20:15.869432 mimosa-0.1.3/mimosa/components/damages/
+-rw-rw-rw-   0        0        0      116 2023-07-21 11:19:18.000000 mimosa-0.1.3/mimosa/components/damages/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 11:20:15.900679 mimosa-0.1.3/mimosa/components/damages/__pycache__/
+-rw-rw-rw-   0        0        0      364 2023-07-21 07:42:48.000000 mimosa-0.1.3/mimosa/components/damages/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0     4552 2023-07-21 07:42:48.000000 mimosa-0.1.3/mimosa/components/damages/__pycache__/ad_rice2010.cpython-310.pyc
+-rw-rw-rw-   0        0        0     4166 2023-07-21 07:42:48.000000 mimosa-0.1.3/mimosa/components/damages/__pycache__/ad_rice2012.cpython-310.pyc
+-rw-rw-rw-   0        0        0     4299 2023-07-21 07:42:48.000000 mimosa-0.1.3/mimosa/components/damages/__pycache__/ad_witch.cpython-310.pyc
+-rw-rw-rw-   0        0        0     3277 2023-07-21 07:42:48.000000 mimosa-0.1.3/mimosa/components/damages/__pycache__/coacch.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1274 2023-07-21 07:42:48.000000 mimosa-0.1.3/mimosa/components/damages/__pycache__/nodamage.cpython-310.pyc
+-rw-rw-rw-   0        0        0     5331 2023-07-21 11:19:18.000000 mimosa-0.1.3/mimosa/components/damages/ad_rice2010.py
+-rw-rw-rw-   0        0        0     4874 2023-07-21 11:19:18.000000 mimosa-0.1.3/mimosa/components/damages/ad_rice2012.py
+-rw-rw-rw-   0        0        0     6688 2023-07-21 11:19:18.000000 mimosa-0.1.3/mimosa/components/damages/ad_witch.py
+-rw-rw-rw-   0        0        0     4260 2023-07-21 11:19:18.000000 mimosa-0.1.3/mimosa/components/damages/coacch.py
+-rw-rw-rw-   0        0        0      971 2023-07-21 11:19:18.000000 mimosa-0.1.3/mimosa/components/damages/nodamage.py
+-rw-rw-rw-   0        0        0    10151 2023-07-21 11:19:18.000000 mimosa-0.1.3/mimosa/components/emissions.py
+drwxrwxrwx   0        0        0        0 2023-07-21 11:20:15.900679 mimosa-0.1.3/mimosa/components/emissiontrade/
+-rw-rw-rw-   0        0        0      112 2023-07-21 11:19:18.000000 mimosa-0.1.3/mimosa/components/emissiontrade/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 11:20:15.922815 mimosa-0.1.3/mimosa/components/emissiontrade/__pycache__/
+-rw-rw-rw-   0        0        0      348 2023-07-21 07:42:48.000000 mimosa-0.1.3/mimosa/components/emissiontrade/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0     3898 2023-07-21 07:42:48.000000 mimosa-0.1.3/mimosa/components/emissiontrade/__pycache__/emissiontrade.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2968 2023-07-21 07:42:48.000000 mimosa-0.1.3/mimosa/components/emissiontrade/__pycache__/globalcostpool.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1414 2023-07-21 07:42:48.000000 mimosa-0.1.3/mimosa/components/emissiontrade/__pycache__/notrade.cpython-310.pyc
+-rw-rw-rw-   0        0        0     5274 2023-07-21 11:19:18.000000 mimosa-0.1.3/mimosa/components/emissiontrade/emissiontrade.py
+-rw-rw-rw-   0        0        0     3276 2023-07-21 11:19:18.000000 mimosa-0.1.3/mimosa/components/emissiontrade/globalcostpool.py
+-rw-rw-rw-   0        0        0     1131 2023-07-21 11:19:18.000000 mimosa-0.1.3/mimosa/components/emissiontrade/notrade.py
+drwxrwxrwx   0        0        0        0 2023-07-21 11:20:15.922815 mimosa-0.1.3/mimosa/components/financialtransfer/
+-rw-rw-rw-   0        0        0      105 2023-07-21 11:19:18.000000 mimosa-0.1.3/mimosa/components/financialtransfer/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 11:20:15.938444 mimosa-0.1.3/mimosa/components/financialtransfer/__pycache__/
+-rw-rw-rw-   0        0        0      336 2023-07-21 07:42:48.000000 mimosa-0.1.3/mimosa/components/financialtransfer/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2230 2023-07-21 07:42:48.000000 mimosa-0.1.3/mimosa/components/financialtransfer/__pycache__/globaldamagepool.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1093 2023-07-21 07:42:48.000000 mimosa-0.1.3/mimosa/components/financialtransfer/__pycache__/notransfer.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1968 2023-07-21 11:19:18.000000 mimosa-0.1.3/mimosa/components/financialtransfer/globaldamagepool.py
+-rw-rw-rw-   0        0        0      939 2023-07-21 11:19:18.000000 mimosa-0.1.3/mimosa/components/financialtransfer/notransfer.py
+drwxrwxrwx   0        0        0        0 2023-07-21 11:20:15.938444 mimosa-0.1.3/mimosa/components/objective/
+-rw-rw-rw-   0        0        0      101 2023-07-21 11:19:18.000000 mimosa-0.1.3/mimosa/components/objective/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 11:20:15.954082 mimosa-0.1.3/mimosa/components/objective/__pycache__/
+-rw-rw-rw-   0        0        0      322 2023-07-21 07:42:48.000000 mimosa-0.1.3/mimosa/components/objective/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2118 2023-07-21 07:42:48.000000 mimosa-0.1.3/mimosa/components/objective/__pycache__/globalcosts.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1736 2023-07-21 07:42:48.000000 mimosa-0.1.3/mimosa/components/objective/__pycache__/utility.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1558 2023-07-21 11:19:19.000000 mimosa-0.1.3/mimosa/components/objective/globalcosts.py
+-rw-rw-rw-   0        0        0     1713 2023-07-21 11:19:19.000000 mimosa-0.1.3/mimosa/components/objective/utility.py
+-rw-rw-rw-   0        0        0     4213 2023-07-21 11:19:19.000000 mimosa-0.1.3/mimosa/components/sealevelrise.py
+drwxrwxrwx   0        0        0        0 2023-07-21 11:20:15.954082 mimosa-0.1.3/mimosa/components/welfare/
+-rw-rw-rw-   0        0        0      165 2023-07-21 11:19:19.000000 mimosa-0.1.3/mimosa/components/welfare/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 11:20:15.969690 mimosa-0.1.3/mimosa/components/welfare/__pycache__/
+-rw-rw-rw-   0        0        0      391 2023-07-21 07:42:48.000000 mimosa-0.1.3/mimosa/components/welfare/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1882 2023-07-21 07:42:48.000000 mimosa-0.1.3/mimosa/components/welfare/__pycache__/inequal_aversion_elasmu.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2368 2023-07-21 07:42:48.000000 mimosa-0.1.3/mimosa/components/welfare/__pycache__/inequal_aversion_general.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2133 2023-07-21 07:42:48.000000 mimosa-0.1.3/mimosa/components/welfare/__pycache__/inequal_aversion_zero.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1456 2023-07-21 11:19:19.000000 mimosa-0.1.3/mimosa/components/welfare/inequal_aversion_elasmu.py
+-rw-rw-rw-   0        0        0     2048 2023-07-21 11:19:19.000000 mimosa-0.1.3/mimosa/components/welfare/inequal_aversion_general.py
+-rw-rw-rw-   0        0        0     1663 2023-07-21 11:19:19.000000 mimosa-0.1.3/mimosa/components/welfare/inequal_aversion_zero.py
+drwxrwxrwx   0        0        0        0 2023-07-21 11:20:15.985317 mimosa-0.1.3/mimosa/concrete_model/
+-rw-rw-rw-   0        0        0        0 2023-07-21 11:19:19.000000 mimosa-0.1.3/mimosa/concrete_model/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 11:20:15.985317 mimosa-0.1.3/mimosa/concrete_model/__pycache__/
+-rw-rw-rw-   0        0        0      192 2023-07-21 07:42:48.000000 mimosa-0.1.3/mimosa/concrete_model/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0     8590 2023-07-21 07:42:48.000000 mimosa-0.1.3/mimosa/concrete_model/__pycache__/instantiate_params.cpython-310.pyc
+-rw-rw-rw-   0        0        0    15078 2023-07-21 11:19:19.000000 mimosa-0.1.3/mimosa/concrete_model/instantiate_params.py
+drwxrwxrwx   0        0        0        0 2023-07-21 11:20:16.000937 mimosa-0.1.3/mimosa/concrete_model/simulation_mode/
+-rw-rw-rw-   0        0        0       39 2023-07-21 11:19:19.000000 mimosa-0.1.3/mimosa/concrete_model/simulation_mode/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 11:20:16.023093 mimosa-0.1.3/mimosa/concrete_model/simulation_mode/__pycache__/
+-rw-rw-rw-   0        0        0      256 2023-07-21 07:42:48.000000 mimosa-0.1.3/mimosa/concrete_model/simulation_mode/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0      677 2023-07-21 07:42:48.000000 mimosa-0.1.3/mimosa/concrete_model/simulation_mode/__pycache__/deactivate_constraints.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1046 2023-07-21 07:42:48.000000 mimosa-0.1.3/mimosa/concrete_model/simulation_mode/__pycache__/main.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2504 2023-07-21 07:42:48.000000 mimosa-0.1.3/mimosa/concrete_model/simulation_mode/__pycache__/set_constraints.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2101 2023-07-21 07:42:48.000000 mimosa-0.1.3/mimosa/concrete_model/simulation_mode/__pycache__/utils.cpython-310.pyc
+-rw-rw-rw-   0        0        0      493 2023-07-21 11:19:19.000000 mimosa-0.1.3/mimosa/concrete_model/simulation_mode/deactivate_constraints.py
+-rw-rw-rw-   0        0        0      907 2023-07-21 11:19:19.000000 mimosa-0.1.3/mimosa/concrete_model/simulation_mode/main.py
+-rw-rw-rw-   0        0        0     3369 2023-07-21 11:19:19.000000 mimosa-0.1.3/mimosa/concrete_model/simulation_mode/set_constraints.py
+-rw-rw-rw-   0        0        0     1557 2023-07-21 11:19:19.000000 mimosa-0.1.3/mimosa/concrete_model/simulation_mode/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-21 11:20:16.023093 mimosa-0.1.3/mimosa/export/
+-rw-rw-rw-   0        0        0      202 2023-07-21 11:19:19.000000 mimosa-0.1.3/mimosa/export/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 11:20:16.038745 mimosa-0.1.3/mimosa/export/__pycache__/
+-rw-rw-rw-   0        0        0      418 2023-07-21 07:42:48.000000 mimosa-0.1.3/mimosa/export/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0     3355 2023-07-21 07:42:48.000000 mimosa-0.1.3/mimosa/export/__pycache__/plot.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2567 2023-07-21 07:42:48.000000 mimosa-0.1.3/mimosa/export/__pycache__/save.cpython-310.pyc
+-rw-rw-rw-   0        0        0     5349 2023-07-21 07:42:48.000000 mimosa-0.1.3/mimosa/export/__pycache__/utils.cpython-310.pyc
+-rw-rw-rw-   0        0        0     5262 2023-07-21 11:19:19.000000 mimosa-0.1.3/mimosa/export/plot.py
+-rw-rw-rw-   0        0        0     3110 2023-07-21 11:19:19.000000 mimosa-0.1.3/mimosa/export/save.py
+-rw-rw-rw-   0        0        0     5836 2023-07-21 11:19:19.000000 mimosa-0.1.3/mimosa/export/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-21 11:20:15.653412 mimosa-0.1.3/mimosa/inputdata/
+drwxrwxrwx   0        0        0        0 2023-07-21 11:20:16.054368 mimosa-0.1.3/mimosa/inputdata/config/
+-rw-rw-rw-   0        0        0       13 2023-07-21 11:19:19.000000 mimosa-0.1.3/mimosa/inputdata/config/config.yaml
+-rw-rw-rw-   0        0        0     2296 2023-07-21 11:19:19.000000 mimosa-0.1.3/mimosa/inputdata/config/config_R5.yaml
+-rw-rw-rw-   0        0        0    13790 2023-07-21 11:19:19.000000 mimosa-0.1.3/mimosa/inputdata/config/config_default.yaml
+-rw-rw-rw-   0        0        0      154 2023-07-21 11:19:19.000000 mimosa-0.1.3/mimosa/inputdata/config/default_units.yaml
+-rw-rw-rw-   0        0        0      456 2023-07-21 11:19:19.000000 mimosa-0.1.3/mimosa/inputdata/config/extra_units.txt
+drwxrwxrwx   0        0        0        0 2023-07-21 11:20:16.054368 mimosa-0.1.3/mimosa/inputdata/data/
+-rw-rw-rw-   0        0        0    89096 2023-07-21 11:19:19.000000 mimosa-0.1.3/mimosa/inputdata/data/data_IMAGE_SSP.csv
+-rw-rw-rw-   0        0        0    89101 2023-07-21 11:19:19.000000 mimosa-0.1.3/mimosa/inputdata/data/data_IMAGE_SSP_harmonised_2020.csv
+drwxrwxrwx   0        0        0        0 2023-07-21 11:20:16.069998 mimosa-0.1.3/mimosa/inputdata/params/
+-rw-rw-rw-   0        0        0      491 2023-07-21 11:19:19.000000 mimosa-0.1.3/mimosa/inputdata/params/ADRICE2010.csv
+-rw-rw-rw-   0        0        0      593 2023-07-21 11:19:19.000000 mimosa-0.1.3/mimosa/inputdata/params/ADRICE2012.csv
+-rw-rw-rw-   0        0        0    34077 2023-07-21 11:19:19.000000 mimosa-0.1.3/mimosa/inputdata/params/COACCH.csv
+-rw-rw-rw-   0        0        0      321 2023-07-21 11:19:19.000000 mimosa-0.1.3/mimosa/inputdata/params/economics.csv
+-rw-rw-rw-   0        0        0     7044 2023-07-21 11:19:19.000000 mimosa-0.1.3/mimosa/inputdata/params/mac.csv
+drwxrwxrwx   0        0        0        0 2023-07-21 11:20:16.101244 mimosa-0.1.3/mimosa/inputdata/regions/
+-rw-rw-rw-   0        0        0      286 2023-07-21 11:19:19.000000 mimosa-0.1.3/mimosa/inputdata/regions/IMAGE26_ADRICE2010.csv
+-rw-rw-rw-   0        0        0      280 2023-07-21 11:19:19.000000 mimosa-0.1.3/mimosa/inputdata/regions/IMAGE26_ADRICE2012.csv
+-rw-rw-rw-   0        0        0      337 2023-07-21 11:19:19.000000 mimosa-0.1.3/mimosa/inputdata/regions/IMAGE26_COACCH.csv
+-rw-rw-rw-   0        0        0   167460 2023-07-21 11:19:19.000000 mimosa-0.1.3/mimosa/inputdata/regions/IMAGE26_regions.json
+-rw-rw-rw-   0        0        0   123689 2023-07-21 11:19:19.000000 mimosa-0.1.3/mimosa/inputdata/regions/R5_regions.json
+-rw-rw-rw-   0        0        0    21007 2023-07-21 11:19:19.000000 mimosa-0.1.3/mimosa/inputdata/regions/country_ISO_codes.csv
+-rw-rw-rw-   0        0        0     8217 2023-07-21 11:19:19.000000 mimosa-0.1.3/mimosa/mimosa.py
+drwxrwxrwx   0        0        0        0 2023-07-21 11:20:16.101244 mimosa-0.1.3/mimosa/socialcostofcarbon/
+-rw-rw-rw-   0        0        0        0 2023-07-21 11:19:19.000000 mimosa-0.1.3/mimosa/socialcostofcarbon/__init__.py
+-rw-rw-rw-   0        0        0     5546 2023-07-21 11:19:19.000000 mimosa-0.1.3/mimosa/socialcostofcarbon/scc.py
+drwxrwxrwx   0        0        0        0 2023-07-21 11:20:15.738051 mimosa-0.1.3/mimosa.egg-info/
+-rw-rw-rw-   0        0        0     5603 2023-07-21 11:20:15.000000 mimosa-0.1.3/mimosa.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     6851 2023-07-21 11:20:15.000000 mimosa-0.1.3/mimosa.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-21 11:20:15.000000 mimosa-0.1.3/mimosa.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2023-07-21 11:20:15.000000 mimosa-0.1.3/mimosa.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-21 11:20:15.000000 mimosa-0.1.3/mimosa.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-07-21 11:19:19.000000 mimosa-0.1.3/pyproject.toml
+-rw-rw-rw-   0        0        0       61 2023-07-21 06:53:35.000000 mimosa-0.1.3/requirements.txt
+-rw-rw-rw-   0        0        0      217 2023-07-21 11:19:19.000000 mimosa-0.1.3/run.py
+-rw-rw-rw-   0        0        0       42 2023-07-21 11:20:16.101244 mimosa-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      621 2023-07-21 11:19:41.000000 mimosa-0.1.3/setup.py
```

### Comparing `mimosa-0.1.2/.gitignore` & `mimosa-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.2/LICENSE` & `mimosa-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.2/PKG-INFO` & `mimosa-0.1.3/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,7 @@
-Metadata-Version: 2.1
-Name: mimosa
-Version: 0.1.2
-Summary: MIMOSA: Integrated Assessment Model for Cost-Benefit Analysis
-Author: Kaj-Ivar van der Wijst
-Author-email: k.i.vanderwijst@gmail.com
-License: LICENSE.txt
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # MIMOSA: Mathematical Integrated Model for Optimal and Stylised Assessment
 
 MIMOSA is a recent simple IAM based on FAIR, with 26 regions covering the whole world. It is a relatively simple Cost-Benefit IAM but still covers the relevant technological and socio-economic dynamics. Temperature is a linear function of cumulative CO2 emissions. MIMOSA uses the DICE sea-level rise module. The mitigation costs, population, initial capital stock and baseline GDP and CO2 emissions are regional. The direct regional mitigation costs are calculated as area under the Marginal Abatement Cost (MAC) curve, and have been calibrated to the IPCC AR6 WGIII database.
 
 ### General
 
 The model is written in the Python optimisation package [Pyomo](https://www.pyomo.org/). It is mainly an `AbstractModel`
@@ -37,67 +27,67 @@
     * [Maximise utility](mimosa/model/components/objective/utility.py)
     * [Minimise global costs](mimosa/model/components/objective/globalcosts.py)
   * Welfare function module
     * [Global cost-minimising](mimosa/model/components/welfare/inequal_aversion_zero.py)
     * [Regional welfare loss-minimising](mimosa/model/components/welfare/inequal_aversion_elasmu.py)
 * [Concrete model](mimosa/model/concrete_model/instantiate_params.py)
   * [Simulation mode](mimosa/model/concrete_model/simulation_mode/main.py) (when emission/temperature paths are imposed exogenously)
-    
-### Data
-
-The parameter values are defined in the [`config.yaml`](mimosa/inputdata/config/config.yaml) file in the `input` directory, and for region- and component-specific parameters in:
-* Initial capital factor: [`economics.csv`](mimosa/inputdata/params/economics.csv)
-* MAC factors: [`mac.csv`](mimosa/inputdata/params/mac.csv)
-* Regional damages and adaptation coefficients: [`COACCH.csv`](mimosa/inputdata/params/COACCH.csv)
-
-The baseline emissions, baseline GDP (for calculation of Total Factor Productivity) and population data is read in IIASA
-database format. By default, the IMAGE data of [`inputdata/data/data_IMAGE_SSP.csv`](mimosa/inputdata/data/data_IMAGE_SSP.csv) is used.
 
-The config parameter values and the input data are combined with the `AbstractModel` to create the `ConcreteModel` in
-[`model/concrete_model/instantiate_params.py`](mimosa/model/concrete_model/instantiate_params.py).
+<br>
+<br>
 
-The main file of the model, where concrete model is created and the model is solved, is [`model/mimosa.py`](mimosa/model/mimosa.py).
+![](https://media.springernature.com/full/springer-static/image/art%3A10.1038%2Fs41467-021-22826-5/MediaObjects/41467_2021_22826_Fig1_HTML.png)
+*Schematic overview of the MIMOSA model. From [[1]](#1).*
+  
+## Installing and running MIMOSA
+
+MIMOSA can be installed using `pip`:
+```bash
+pip install mimosa
+```
 
-### Running the model
+Since MIMOSA is an optimisation model, an optimisation engine needs to be specified. This can be installed locally (see [With IPOPT installed locally](#ipopt-local)), but an easier way is to use a free cloud-based optimisation service called NEOS.
 
-The simplest way to run the model is shown in [`run.py`](run.py). You can change parameter values by either editing the 
-`config.yaml` file, or by updating the `params` variable (which is simply a Python dictionary containing the `config.yaml`
-data).
+<h4>Using the NEOS server</h4>
+The MIMOSA runs can easily be sent to the NEOS server (https://neos-server.org) for remote optimisation. First, on their website, sign up for a free account. You can then run MIMOSA with NEOS enabled by providing it with the email address you used to sign up for NEOS:
 
 ```python
-from mimosa.model.mimosa import MIMOSA
-
-from mimosa.model.common.config import parseconfig
+from mimosa import MIMOSA, load_params
 
-params = parseconfig.load_params()
-params["emissions"]["carbonbudget"] = False
+params = load_params()
 
 model1 = MIMOSA(params)
-model1.solve()
+model1.solve(use_neos=True, neos_email="your.email@email.com")
 model1.save("run1")
 ```
 
-#### With IPOPT installed locally
+Depending on the MIMOSA parameters chosen and on how busy the NEOS server is, running the model might take a while (typically a couple of minutes).
+
+<h4 id='ipopt-local'>With IPOPT installed locally</h4>
 
-By default, this requires the optimisation package `ipopt` to be installed. The easiest way is to install it using
+A faster way to run MIMOSA, and which doesn't require an internet connection, is to install the open-source optimisation engine IPOPT locally:
 ```
 conda install -c conda-forge ipopt
 ```
 However, this sometimes fails on Windows. To fix it, go to https://www.coin-or.org/download/binary/Ipopt/ and download the latest win64-version. Unzip the files. A subfolder `bin` should contain the file `ipopt.exe`. The next step is to add this folder to your PATH environment:
 Windows > Edit the system environment variables > Environment variables... > Select "Path" and click Edit... > Click New and browse to the folder you just unzipped. Make sure to select the `bin` subfolder as this folder contains the file `ipopt.exe`.
 
-#### Using the NEOS server
-Even easier than installing IPOPT is by using the NEOS server: https://neos-server.org. The MIMOSA runs are then optimised on a remote server from the US optimisation community NEOS. On their website, sign up for a free account. You can then run MIMOSA with NEOS enabled by providing it with the email address you used to sign up for NEOS:
+Once IPOPT is installed, MIMOSA can be ran without NEOS:
 ```python
-from mimosa.model.mimosa import MIMOSA
-
-from mimosa.model.common.config import parseconfig
+from mimosa import MIMOSA, load_params
 
-params = parseconfig.load_params()
-params["emissions"]["carbonbudget"] = False
+params = load_params()
 
 model1 = MIMOSA(params)
-model1.solve(use_neos=True, neos_email="your.email@email.com")
+model1.solve()  # No NEOS required
 model1.save("run1")
 ```
 
+## How to cite
+When using MIMOSA, please cite [[1]](#1) (global version) and [[2]](#2) (regional version).
+
+## References
+<a id="1">[1]</a> 
+van der Wijst, KI., Hof, A.F. & van Vuuren, D.P. On the optimality of 2°C targets and a decomposition of uncertainty. *Nature Communications* **12**, 2575 (2021). https://doi.org/10.1038/s41467-021-22826-5
 
+<a id="2">[2]</a> 
+van der Wijst, KI., Bosello, F., Dasgupta, S. *et al*. New damage curves and multimodel analysis suggest lower optimal temperature. *Nature Climate Change* **13**, 434–441 (2023). https://doi.org/10.1038/s41558-023-01636-1
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `mimosa-0.1.2/README.md` & `mimosa-0.1.3/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+Metadata-Version: 2.1
+Name: mimosa
+Version: 0.1.3
+Summary: MIMOSA: Integrated Assessment Model for Cost-Benefit Analysis
+Author: Kaj-Ivar van der Wijst
+Author-email: k.i.vanderwijst@gmail.com
+License: LICENSE.txt
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # MIMOSA: Mathematical Integrated Model for Optimal and Stylised Assessment
 
 MIMOSA is a recent simple IAM based on FAIR, with 26 regions covering the whole world. It is a relatively simple Cost-Benefit IAM but still covers the relevant technological and socio-economic dynamics. Temperature is a linear function of cumulative CO2 emissions. MIMOSA uses the DICE sea-level rise module. The mitigation costs, population, initial capital stock and baseline GDP and CO2 emissions are regional. The direct regional mitigation costs are calculated as area under the Marginal Abatement Cost (MAC) curve, and have been calibrated to the IPCC AR6 WGIII database.
 
 ### General
 
 The model is written in the Python optimisation package [Pyomo](https://www.pyomo.org/). It is mainly an `AbstractModel`
@@ -27,67 +37,67 @@
     * [Maximise utility](mimosa/model/components/objective/utility.py)
     * [Minimise global costs](mimosa/model/components/objective/globalcosts.py)
   * Welfare function module
     * [Global cost-minimising](mimosa/model/components/welfare/inequal_aversion_zero.py)
     * [Regional welfare loss-minimising](mimosa/model/components/welfare/inequal_aversion_elasmu.py)
 * [Concrete model](mimosa/model/concrete_model/instantiate_params.py)
   * [Simulation mode](mimosa/model/concrete_model/simulation_mode/main.py) (when emission/temperature paths are imposed exogenously)
-    
-### Data
-
-The parameter values are defined in the [`config.yaml`](mimosa/inputdata/config/config.yaml) file in the `input` directory, and for region- and component-specific parameters in:
-* Initial capital factor: [`economics.csv`](mimosa/inputdata/params/economics.csv)
-* MAC factors: [`mac.csv`](mimosa/inputdata/params/mac.csv)
-* Regional damages and adaptation coefficients: [`COACCH.csv`](mimosa/inputdata/params/COACCH.csv)
-
-The baseline emissions, baseline GDP (for calculation of Total Factor Productivity) and population data is read in IIASA
-database format. By default, the IMAGE data of [`inputdata/data/data_IMAGE_SSP.csv`](mimosa/inputdata/data/data_IMAGE_SSP.csv) is used.
 
-The config parameter values and the input data are combined with the `AbstractModel` to create the `ConcreteModel` in
-[`model/concrete_model/instantiate_params.py`](mimosa/model/concrete_model/instantiate_params.py).
+<br>
+<br>
 
-The main file of the model, where concrete model is created and the model is solved, is [`model/mimosa.py`](mimosa/model/mimosa.py).
+![](https://media.springernature.com/full/springer-static/image/art%3A10.1038%2Fs41467-021-22826-5/MediaObjects/41467_2021_22826_Fig1_HTML.png)
+*Schematic overview of the MIMOSA model. From [[1]](#1).*
+  
+## Installing and running MIMOSA
+
+MIMOSA can be installed using `pip`:
+```bash
+pip install mimosa
+```
 
-### Running the model
+Since MIMOSA is an optimisation model, an optimisation engine needs to be specified. This can be installed locally (see [With IPOPT installed locally](#ipopt-local)), but an easier way is to use a free cloud-based optimisation service called NEOS.
 
-The simplest way to run the model is shown in [`run.py`](run.py). You can change parameter values by either editing the 
-`config.yaml` file, or by updating the `params` variable (which is simply a Python dictionary containing the `config.yaml`
-data).
+<h4>Using the NEOS server</h4>
+The MIMOSA runs can easily be sent to the NEOS server (https://neos-server.org) for remote optimisation. First, on their website, sign up for a free account. You can then run MIMOSA with NEOS enabled by providing it with the email address you used to sign up for NEOS:
 
 ```python
-from mimosa.model.mimosa import MIMOSA
-
-from mimosa.model.common.config import parseconfig
+from mimosa import MIMOSA, load_params
 
-params = parseconfig.load_params()
-params["emissions"]["carbonbudget"] = False
+params = load_params()
 
 model1 = MIMOSA(params)
-model1.solve()
+model1.solve(use_neos=True, neos_email="your.email@email.com")
 model1.save("run1")
 ```
 
-#### With IPOPT installed locally
+Depending on the MIMOSA parameters chosen and on how busy the NEOS server is, running the model might take a while (typically a couple of minutes).
+
+<h4 id='ipopt-local'>With IPOPT installed locally</h4>
 
-By default, this requires the optimisation package `ipopt` to be installed. The easiest way is to install it using
+A faster way to run MIMOSA, and which doesn't require an internet connection, is to install the open-source optimisation engine IPOPT locally:
 ```
 conda install -c conda-forge ipopt
 ```
 However, this sometimes fails on Windows. To fix it, go to https://www.coin-or.org/download/binary/Ipopt/ and download the latest win64-version. Unzip the files. A subfolder `bin` should contain the file `ipopt.exe`. The next step is to add this folder to your PATH environment:
 Windows > Edit the system environment variables > Environment variables... > Select "Path" and click Edit... > Click New and browse to the folder you just unzipped. Make sure to select the `bin` subfolder as this folder contains the file `ipopt.exe`.
 
-#### Using the NEOS server
-Even easier than installing IPOPT is by using the NEOS server: https://neos-server.org. The MIMOSA runs are then optimised on a remote server from the US optimisation community NEOS. On their website, sign up for a free account. You can then run MIMOSA with NEOS enabled by providing it with the email address you used to sign up for NEOS:
+Once IPOPT is installed, MIMOSA can be ran without NEOS:
 ```python
-from mimosa.model.mimosa import MIMOSA
-
-from mimosa.model.common.config import parseconfig
+from mimosa import MIMOSA, load_params
 
-params = parseconfig.load_params()
-params["emissions"]["carbonbudget"] = False
+params = load_params()
 
 model1 = MIMOSA(params)
-model1.solve(use_neos=True, neos_email="your.email@email.com")
+model1.solve()  # No NEOS required
 model1.save("run1")
 ```
 
+## How to cite
+When using MIMOSA, please cite [[1]](#1) (global version) and [[2]](#2) (regional version).
+
+## References
+<a id="1">[1]</a> 
+van der Wijst, KI., Hof, A.F. & van Vuuren, D.P. On the optimality of 2Â°C targets and a decomposition of uncertainty. *Nature Communications* **12**, 2575 (2021). https://doi.org/10.1038/s41467-021-22826-5
 
+<a id="2">[2]</a> 
+van der Wijst, KI., Bosello, F., Dasgupta, S. *et al*. New damage curves and multimodel analysis suggest lower optimal temperature. *Nature Climate Change* **13**, 434â€“441 (2023). https://doi.org/10.1038/s41558-023-01636-1
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `mimosa-0.1.2/mimosa/__pycache__/abstract_model.cpython-310.pyc` & `mimosa-0.1.3/mimosa/__pycache__/abstract_model.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.2/mimosa/__pycache__/mimosa.cpython-310.pyc` & `mimosa-0.1.3/mimosa/__pycache__/mimosa.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.2/mimosa/abstract_model.py` & `mimosa-0.1.3/mimosa/abstract_model.py`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.2/mimosa/common/__init__.py` & `mimosa-0.1.3/mimosa/common/__init__.py`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.2/mimosa/common/__pycache__/__init__.cpython-310.pyc` & `mimosa-0.1.3/mimosa/common/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.2/mimosa/common/__pycache__/economics.cpython-310.pyc` & `mimosa-0.1.3/mimosa/common/__pycache__/economics.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.2/mimosa/common/__pycache__/pyomo_utils.cpython-310.pyc` & `mimosa-0.1.3/mimosa/common/__pycache__/pyomo_utils.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.2/mimosa/common/__pycache__/units.cpython-310.pyc` & `mimosa-0.1.3/mimosa/common/__pycache__/units.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.2/mimosa/common/__pycache__/utils.cpython-310.pyc` & `mimosa-0.1.3/mimosa/common/__pycache__/utils.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.2/mimosa/common/config/__pycache__/parseconfig.cpython-310.pyc` & `mimosa-0.1.3/mimosa/common/config/__pycache__/parseconfig.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.2/mimosa/common/config/parseconfig.py` & `mimosa-0.1.3/mimosa/common/config/parseconfig.py`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.2/mimosa/common/config/utils/__pycache__/nested_dict.cpython-310.pyc` & `mimosa-0.1.3/mimosa/common/config/utils/__pycache__/nested_dict.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.2/mimosa/common/config/utils/__pycache__/parsers.cpython-310.pyc` & `mimosa-0.1.3/mimosa/common/config/utils/__pycache__/parsers.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.2/mimosa/common/config/utils/nested_dict.py` & `mimosa-0.1.3/mimosa/common/config/utils/nested_dict.py`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.2/mimosa/common/config/utils/parsers.py` & `mimosa-0.1.3/mimosa/common/config/utils/parsers.py`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.2/mimosa/common/data/__pycache__/datastore.cpython-310.pyc` & `mimosa-0.1.3/mimosa/common/data/__pycache__/datastore.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.2/mimosa/common/data/__pycache__/utils.cpython-310.pyc` & `mimosa-0.1.3/mimosa/common/data/__pycache__/utils.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.2/mimosa/common/data/datastore.py` & `mimosa-0.1.3/mimosa/common/data/datastore.py`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.2/mimosa/common/data/utils.py` & `mimosa-0.1.3/mimosa/common/data/utils.py`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.2/mimosa/common/economics.py` & `mimosa-0.1.3/mimosa/common/economics.py`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.2/mimosa/common/pyomo_utils.py` & `mimosa-0.1.3/mimosa/common/pyomo_utils.py`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.2/mimosa/common/regional_params/__pycache__/main.cpython-310.pyc` & `mimosa-0.1.3/mimosa/common/regional_params/__pycache__/main.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.2/mimosa/common/regional_params/__pycache__/region_mappers.cpython-310.pyc` & `mimosa-0.1.3/mimosa/common/regional_params/__pycache__/region_mappers.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.2/mimosa/common/regional_params/__pycache__/regional_param_container.cpython-310.pyc` & `mimosa-0.1.3/mimosa/common/regional_params/__pycache__/regional_param_container.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.2/mimosa/common/regional_params/main.py` & `mimosa-0.1.3/mimosa/common/regional_params/main.py`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.2/mimosa/common/regional_params/region_mappers.py` & `mimosa-0.1.3/mimosa/common/regional_params/region_mappers.py`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.2/mimosa/common/regional_params/regional_param_container.py` & `mimosa-0.1.3/mimosa/common/regional_params/regional_param_container.py`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.2/mimosa/common/units.py` & `mimosa-0.1.3/mimosa/common/units.py`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.2/mimosa/common/utils.py` & `mimosa-0.1.3/mimosa/common/utils.py`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.2/mimosa/components/__pycache__/abatement.cpython-310.pyc` & `mimosa-0.1.3/mimosa/components/__pycache__/abatement.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.2/mimosa/components/__pycache__/burdensharing.cpython-310.pyc` & `mimosa-0.1.3/mimosa/components/__pycache__/burdensharing.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.2/mimosa/components/__pycache__/cobbdouglas.cpython-310.pyc` & `mimosa-0.1.3/mimosa/components/__pycache__/cobbdouglas.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.2/mimosa/components/__pycache__/emissions.cpython-310.pyc` & `mimosa-0.1.3/mimosa/components/__pycache__/emissions.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.2/mimosa/components/__pycache__/sealevelrise.cpython-310.pyc` & `mimosa-0.1.3/mimosa/components/__pycache__/sealevelrise.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.2/mimosa/components/abatement.py` & `mimosa-0.1.3/mimosa/components/abatement.py`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.2/mimosa/components/burdensharing.py` & `mimosa-0.1.3/mimosa/components/burdensharing.py`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.2/mimosa/components/cobbdouglas.py` & `mimosa-0.1.3/mimosa/components/cobbdouglas.py`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.2/mimosa/components/damages/__pycache__/ad_rice2010.cpython-310.pyc` & `mimosa-0.1.3/mimosa/components/damages/__pycache__/ad_rice2010.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.2/mimosa/components/damages/__pycache__/ad_rice2012.cpython-310.pyc` & `mimosa-0.1.3/mimosa/components/damages/__pycache__/ad_rice2012.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.2/mimosa/components/damages/__pycache__/ad_witch.cpython-310.pyc` & `mimosa-0.1.3/mimosa/components/damages/__pycache__/ad_witch.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.2/mimosa/components/damages/__pycache__/coacch.cpython-310.pyc` & `mimosa-0.1.3/mimosa/components/damages/__pycache__/coacch.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.2/mimosa/components/damages/__pycache__/nodamage.cpython-310.pyc` & `mimosa-0.1.3/mimosa/components/damages/__pycache__/nodamage.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.2/mimosa/components/damages/ad_rice2010.py` & `mimosa-0.1.3/mimosa/components/damages/ad_rice2010.py`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.2/mimosa/components/damages/ad_rice2012.py` & `mimosa-0.1.3/mimosa/components/damages/ad_rice2012.py`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.2/mimosa/components/damages/ad_witch.py` & `mimosa-0.1.3/mimosa/components/damages/ad_witch.py`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.2/mimosa/components/damages/coacch.py` & `mimosa-0.1.3/mimosa/components/damages/coacch.py`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.2/mimosa/components/damages/nodamage.py` & `mimosa-0.1.3/mimosa/components/damages/nodamage.py`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.2/mimosa/components/emissions.py` & `mimosa-0.1.3/mimosa/components/emissions.py`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.2/mimosa/components/emissiontrade/__pycache__/emissiontrade.cpython-310.pyc` & `mimosa-0.1.3/mimosa/components/emissiontrade/__pycache__/emissiontrade.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.2/mimosa/components/emissiontrade/__pycache__/globalcostpool.cpython-310.pyc` & `mimosa-0.1.3/mimosa/components/emissiontrade/__pycache__/globalcostpool.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.2/mimosa/components/emissiontrade/__pycache__/notrade.cpython-310.pyc` & `mimosa-0.1.3/mimosa/components/emissiontrade/__pycache__/notrade.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.2/mimosa/components/emissiontrade/emissiontrade.py` & `mimosa-0.1.3/mimosa/components/emissiontrade/emissiontrade.py`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.2/mimosa/components/emissiontrade/globalcostpool.py` & `mimosa-0.1.3/mimosa/components/emissiontrade/globalcostpool.py`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.2/mimosa/components/emissiontrade/notrade.py` & `mimosa-0.1.3/mimosa/components/emissiontrade/notrade.py`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.2/mimosa/components/financialtransfer/__pycache__/globaldamagepool.cpython-310.pyc` & `mimosa-0.1.3/mimosa/components/financialtransfer/__pycache__/globaldamagepool.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.2/mimosa/components/financialtransfer/__pycache__/notransfer.cpython-310.pyc` & `mimosa-0.1.3/mimosa/components/financialtransfer/__pycache__/notransfer.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.2/mimosa/components/financialtransfer/globaldamagepool.py` & `mimosa-0.1.3/mimosa/components/financialtransfer/globaldamagepool.py`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.2/mimosa/components/financialtransfer/notransfer.py` & `mimosa-0.1.3/mimosa/components/financialtransfer/notransfer.py`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.2/mimosa/components/objective/__pycache__/globalcosts.cpython-310.pyc` & `mimosa-0.1.3/mimosa/components/objective/__pycache__/globalcosts.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.2/mimosa/components/objective/__pycache__/utility.cpython-310.pyc` & `mimosa-0.1.3/mimosa/components/objective/__pycache__/utility.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.2/mimosa/components/objective/globalcosts.py` & `mimosa-0.1.3/mimosa/components/objective/globalcosts.py`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.2/mimosa/components/objective/utility.py` & `mimosa-0.1.3/mimosa/components/objective/utility.py`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.2/mimosa/components/sealevelrise.py` & `mimosa-0.1.3/mimosa/components/sealevelrise.py`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.2/mimosa/components/welfare/__pycache__/inequal_aversion_elasmu.cpython-310.pyc` & `mimosa-0.1.3/mimosa/components/welfare/__pycache__/inequal_aversion_elasmu.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.2/mimosa/components/welfare/__pycache__/inequal_aversion_general.cpython-310.pyc` & `mimosa-0.1.3/mimosa/components/welfare/__pycache__/inequal_aversion_general.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.2/mimosa/components/welfare/__pycache__/inequal_aversion_zero.cpython-310.pyc` & `mimosa-0.1.3/mimosa/components/welfare/__pycache__/inequal_aversion_zero.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.2/mimosa/components/welfare/inequal_aversion_elasmu.py` & `mimosa-0.1.3/mimosa/components/welfare/inequal_aversion_elasmu.py`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.2/mimosa/components/welfare/inequal_aversion_general.py` & `mimosa-0.1.3/mimosa/components/welfare/inequal_aversion_general.py`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.2/mimosa/components/welfare/inequal_aversion_zero.py` & `mimosa-0.1.3/mimosa/components/welfare/inequal_aversion_zero.py`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.2/mimosa/concrete_model/__pycache__/instantiate_params.cpython-310.pyc` & `mimosa-0.1.3/mimosa/concrete_model/__pycache__/instantiate_params.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.2/mimosa/concrete_model/instantiate_params.py` & `mimosa-0.1.3/mimosa/concrete_model/instantiate_params.py`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.2/mimosa/concrete_model/simulation_mode/__pycache__/deactivate_constraints.cpython-310.pyc` & `mimosa-0.1.3/mimosa/concrete_model/simulation_mode/__pycache__/deactivate_constraints.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.2/mimosa/concrete_model/simulation_mode/__pycache__/main.cpython-310.pyc` & `mimosa-0.1.3/mimosa/concrete_model/simulation_mode/__pycache__/main.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.2/mimosa/concrete_model/simulation_mode/__pycache__/set_constraints.cpython-310.pyc` & `mimosa-0.1.3/mimosa/concrete_model/simulation_mode/__pycache__/set_constraints.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.2/mimosa/concrete_model/simulation_mode/__pycache__/utils.cpython-310.pyc` & `mimosa-0.1.3/mimosa/concrete_model/simulation_mode/__pycache__/utils.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.2/mimosa/concrete_model/simulation_mode/main.py` & `mimosa-0.1.3/mimosa/concrete_model/simulation_mode/main.py`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.2/mimosa/concrete_model/simulation_mode/set_constraints.py` & `mimosa-0.1.3/mimosa/concrete_model/simulation_mode/set_constraints.py`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.2/mimosa/concrete_model/simulation_mode/utils.py` & `mimosa-0.1.3/mimosa/concrete_model/simulation_mode/utils.py`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.2/mimosa/export/__pycache__/plot.cpython-310.pyc` & `mimosa-0.1.3/mimosa/export/__pycache__/plot.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.2/mimosa/export/__pycache__/save.cpython-310.pyc` & `mimosa-0.1.3/mimosa/export/__pycache__/save.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.2/mimosa/export/__pycache__/utils.cpython-310.pyc` & `mimosa-0.1.3/mimosa/export/__pycache__/utils.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.2/mimosa/export/plot.py` & `mimosa-0.1.3/mimosa/export/plot.py`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.2/mimosa/export/save.py` & `mimosa-0.1.3/mimosa/export/save.py`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.2/mimosa/export/utils.py` & `mimosa-0.1.3/mimosa/export/utils.py`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.2/mimosa/inputdata/config/config_R5.yaml` & `mimosa-0.1.3/mimosa/inputdata/config/config_R5.yaml`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.2/mimosa/inputdata/config/config_default.yaml` & `mimosa-0.1.3/mimosa/inputdata/config/config_default.yaml`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.2/mimosa/inputdata/data/data_IMAGE_SSP.csv` & `mimosa-0.1.3/mimosa/inputdata/data/data_IMAGE_SSP.csv`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.2/mimosa/inputdata/data/data_IMAGE_SSP_harmonised_2020.csv` & `mimosa-0.1.3/mimosa/inputdata/data/data_IMAGE_SSP_harmonised_2020.csv`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.2/mimosa/inputdata/params/ADRICE2012.csv` & `mimosa-0.1.3/mimosa/inputdata/params/ADRICE2012.csv`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.2/mimosa/inputdata/params/COACCH.csv` & `mimosa-0.1.3/mimosa/inputdata/params/COACCH.csv`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.2/mimosa/inputdata/params/mac.csv` & `mimosa-0.1.3/mimosa/inputdata/params/mac.csv`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.2/mimosa/inputdata/regions/IMAGE26_regions.json` & `mimosa-0.1.3/mimosa/inputdata/regions/IMAGE26_regions.json`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.2/mimosa/inputdata/regions/R5_regions.json` & `mimosa-0.1.3/mimosa/inputdata/regions/R5_regions.json`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.2/mimosa/inputdata/regions/country_ISO_codes.csv` & `mimosa-0.1.3/mimosa/inputdata/regions/country_ISO_codes.csv`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.2/mimosa/mimosa.py` & `mimosa-0.1.3/mimosa/mimosa.py`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.2/mimosa/socialcostofcarbon/scc.py` & `mimosa-0.1.3/mimosa/socialcostofcarbon/scc.py`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.2/mimosa.egg-info/SOURCES.txt` & `mimosa-0.1.3/mimosa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mimosa-0.1.2/setup.py` & `mimosa-0.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md") as fh:
     description = fh.read()
 
 setup(
     name="mimosa",
-    version="0.1.2",
+    version="0.1.3",
     author="Kaj-Ivar van der Wijst",
     author_email="k.i.vanderwijst@gmail.com",
     packages=["mimosa"],
     # url="http://pypi.python.org/pypi/PackageName/",
     license="LICENSE.txt",
     description="MIMOSA: Integrated Assessment Model for Cost-Benefit Analysis",
     long_description=description,
```

