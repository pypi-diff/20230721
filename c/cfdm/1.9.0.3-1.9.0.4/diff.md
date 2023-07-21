# Comparing `tmp/cfdm-1.9.0.3.tar.gz` & `tmp/cfdm-1.9.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cfdm-1.9.0.3.tar", last modified: Thu Mar 10 18:35:36 2022, max compression
+gzip compressed data, was "cfdm-1.9.0.4.tar", last modified: Mon Jul 18 14:23:03 2022, max compression
```

## Comparing `cfdm-1.9.0.3.tar` & `cfdm-1.9.0.4.tar`

### file list

```diff
@@ -1,182 +1,182 @@
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-03-10 18:35:36.970495 cfdm-1.9.0.3/
--rw-rw-r--   0 david     (1000) david     (1000)     2661 2020-10-05 07:32:03.000000 cfdm-1.9.0.3/CODE_OF_CONDUCT.md
--rw-rw-r--   0 david     (1000) david     (1000)     1179 2020-10-05 07:32:03.000000 cfdm-1.9.0.3/CONTRIBUTING.md
--rw-rw-r--   0 david     (1000) david     (1000)    16350 2022-03-10 18:16:47.000000 cfdm-1.9.0.3/Changelog.rst
--rw-rw-r--   0 david     (1000) david     (1000)     1065 2020-03-20 18:57:35.000000 cfdm-1.9.0.3/LICENSE
--rw-rw-r--   0 david     (1000) david     (1000)      132 2020-10-09 10:28:32.000000 cfdm-1.9.0.3/MANIFEST.in
--rw-rw-r--   0 david     (1000) david     (1000)     4319 2022-03-10 18:35:36.970495 cfdm-1.9.0.3/PKG-INFO
--rw-rw-r--   0 david     (1000) david     (1000)     6390 2021-09-07 06:51:03.000000 cfdm-1.9.0.3/README.md
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-03-10 18:35:36.946495 cfdm-1.9.0.3/cfdm/
--rw-rw-r--   0 david     (1000) david     (1000)     5834 2022-03-10 18:16:30.000000 cfdm-1.9.0.3/cfdm/__init__.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-03-10 18:35:36.946495 cfdm-1.9.0.3/cfdm/abstract/
--rw-rw-r--   0 david     (1000) david     (1000)       76 2020-10-05 07:32:03.000000 cfdm-1.9.0.3/cfdm/abstract/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)      186 2021-09-07 06:51:03.000000 cfdm-1.9.0.3/cfdm/abstract/container.py
--rw-rw-r--   0 david     (1000) david     (1000)     3438 2021-09-07 06:51:03.000000 cfdm-1.9.0.3/cfdm/abstract/implementation.py
--rw-rw-r--   0 david     (1000) david     (1000)     3941 2021-09-07 06:51:03.000000 cfdm-1.9.0.3/cfdm/auxiliarycoordinate.py
--rw-rw-r--   0 david     (1000) david     (1000)     8289 2021-09-07 06:51:03.000000 cfdm-1.9.0.3/cfdm/bounds.py
--rw-rw-r--   0 david     (1000) david     (1000)    12863 2022-01-31 11:09:58.000000 cfdm-1.9.0.3/cfdm/cellmeasure.py
--rw-rw-r--   0 david     (1000) david     (1000)    16210 2021-09-07 06:51:03.000000 cfdm-1.9.0.3/cfdm/cellmethod.py
--rw-rw-r--   0 david     (1000) david     (1000)    72755 2021-09-07 06:51:03.000000 cfdm-1.9.0.3/cfdm/cfdmimplementation.py
--rw-rw-r--   0 david     (1000) david     (1000)     1501 2021-09-07 06:51:03.000000 cfdm-1.9.0.3/cfdm/constants.py
--rw-rw-r--   0 david     (1000) david     (1000)   113901 2022-01-31 11:09:58.000000 cfdm-1.9.0.3/cfdm/constructs.py
--rw-rw-r--   0 david     (1000) david     (1000)      970 2021-09-07 06:51:03.000000 cfdm-1.9.0.3/cfdm/coordinateconversion.py
--rw-rw-r--   0 david     (1000) david     (1000)    19224 2021-09-07 06:51:03.000000 cfdm-1.9.0.3/cfdm/coordinatereference.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-03-10 18:35:36.950495 cfdm-1.9.0.3/cfdm/core/
--rw-rw-r--   0 david     (1000) david     (1000)     2122 2022-03-10 18:09:22.000000 cfdm-1.9.0.3/cfdm/core/__init__.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-03-10 18:35:36.950495 cfdm-1.9.0.3/cfdm/core/abstract/
--rw-rw-r--   0 david     (1000) david     (1000)      307 2021-01-22 18:34:02.000000 cfdm-1.9.0.3/cfdm/core/abstract/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)     9520 2021-09-07 06:51:03.000000 cfdm-1.9.0.3/cfdm/core/abstract/container.py
--rw-rw-r--   0 david     (1000) david     (1000)     5174 2021-09-07 06:51:03.000000 cfdm-1.9.0.3/cfdm/core/abstract/coordinate.py
--rw-rw-r--   0 david     (1000) david     (1000)     9571 2021-09-07 06:51:03.000000 cfdm-1.9.0.3/cfdm/core/abstract/parameters.py
--rw-rw-r--   0 david     (1000) david     (1000)    11097 2021-05-10 16:58:27.000000 cfdm-1.9.0.3/cfdm/core/abstract/parametersdomainancillaries.py
--rw-rw-r--   0 david     (1000) david     (1000)    10685 2021-09-07 06:51:03.000000 cfdm-1.9.0.3/cfdm/core/abstract/properties.py
--rw-rw-r--   0 david     (1000) david     (1000)    11427 2021-09-07 06:51:03.000000 cfdm-1.9.0.3/cfdm/core/abstract/propertiesdata.py
--rw-rw-r--   0 david     (1000) david     (1000)    19349 2021-09-07 06:51:03.000000 cfdm-1.9.0.3/cfdm/core/abstract/propertiesdatabounds.py
--rw-rw-r--   0 david     (1000) david     (1000)     1987 2021-03-22 16:15:42.000000 cfdm-1.9.0.3/cfdm/core/auxiliarycoordinate.py
--rw-rw-r--   0 david     (1000) david     (1000)     1517 2021-05-10 16:58:27.000000 cfdm-1.9.0.3/cfdm/core/bounds.py
--rw-rw-r--   0 david     (1000) david     (1000)     6281 2022-01-31 11:09:58.000000 cfdm-1.9.0.3/cfdm/core/cellmeasure.py
--rw-rw-r--   0 david     (1000) david     (1000)    17016 2021-05-10 16:58:27.000000 cfdm-1.9.0.3/cfdm/core/cellmethod.py
--rw-rw-r--   0 david     (1000) david     (1000)    45405 2021-09-07 06:51:03.000000 cfdm-1.9.0.3/cfdm/core/constructs.py
--rw-rw-r--   0 david     (1000) david     (1000)      949 2021-03-22 16:15:42.000000 cfdm-1.9.0.3/cfdm/core/coordinateconversion.py
--rw-rw-r--   0 david     (1000) david     (1000)    21103 2021-09-07 06:51:03.000000 cfdm-1.9.0.3/cfdm/core/coordinatereference.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-03-10 18:35:36.954495 cfdm-1.9.0.3/cfdm/core/data/
--rw-rw-r--   0 david     (1000) david     (1000)       86 2020-10-05 07:32:03.000000 cfdm-1.9.0.3/cfdm/core/data/__init__.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-03-10 18:35:36.954495 cfdm-1.9.0.3/cfdm/core/data/abstract/
--rw-rw-r--   0 david     (1000) david     (1000)       25 2020-03-20 18:57:35.000000 cfdm-1.9.0.3/cfdm/core/data/abstract/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)     4952 2021-05-10 16:58:27.000000 cfdm-1.9.0.3/cfdm/core/data/abstract/array.py
--rw-rw-r--   0 david     (1000) david     (1000)    21952 2021-09-07 06:51:03.000000 cfdm-1.9.0.3/cfdm/core/data/data.py
--rw-rw-r--   0 david     (1000) david     (1000)     3575 2021-05-10 16:58:27.000000 cfdm-1.9.0.3/cfdm/core/data/numpyarray.py
--rw-rw-r--   0 david     (1000) david     (1000)      771 2021-03-22 16:15:42.000000 cfdm-1.9.0.3/cfdm/core/datum.py
--rw-rw-r--   0 david     (1000) david     (1000)     3736 2021-03-22 16:15:42.000000 cfdm-1.9.0.3/cfdm/core/dimensioncoordinate.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-03-10 18:35:36.954495 cfdm-1.9.0.3/cfdm/core/docstring/
--rw-rw-r--   0 david     (1000) david     (1000)       59 2020-10-05 07:32:03.000000 cfdm-1.9.0.3/cfdm/core/docstring/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)     5320 2021-05-10 16:58:27.000000 cfdm-1.9.0.3/cfdm/core/docstring/docstring.py
--rw-rw-r--   0 david     (1000) david     (1000)     7868 2021-09-07 06:51:03.000000 cfdm-1.9.0.3/cfdm/core/domain.py
--rw-rw-r--   0 david     (1000) david     (1000)     1305 2021-05-12 12:32:47.000000 cfdm-1.9.0.3/cfdm/core/domainancillary.py
--rw-rw-r--   0 david     (1000) david     (1000)     4864 2021-05-10 16:58:27.000000 cfdm-1.9.0.3/cfdm/core/domainaxis.py
--rw-rw-r--   0 david     (1000) david     (1000)    19000 2021-09-07 06:51:03.000000 cfdm-1.9.0.3/cfdm/core/field.py
--rw-rw-r--   0 david     (1000) david     (1000)     1637 2021-03-22 16:15:42.000000 cfdm-1.9.0.3/cfdm/core/fieldancillary.py
--rw-rw-r--   0 david     (1000) david     (1000)     3028 2021-09-07 06:51:03.000000 cfdm-1.9.0.3/cfdm/core/functions.py
--rw-rw-r--   0 david     (1000) david     (1000)     1009 2021-03-22 16:15:42.000000 cfdm-1.9.0.3/cfdm/core/interiorring.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-03-10 18:35:36.954495 cfdm-1.9.0.3/cfdm/core/meta/
--rw-rw-r--   0 david     (1000) david     (1000)       51 2020-10-05 07:32:03.000000 cfdm-1.9.0.3/cfdm/core/meta/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)    24252 2021-09-07 06:51:03.000000 cfdm-1.9.0.3/cfdm/core/meta/docstringrewrite.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-03-10 18:35:36.954495 cfdm-1.9.0.3/cfdm/core/mixin/
--rw-rw-r--   0 david     (1000) david     (1000)       37 2021-05-10 16:58:27.000000 cfdm-1.9.0.3/cfdm/core/mixin/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)    11933 2021-09-07 06:51:03.000000 cfdm-1.9.0.3/cfdm/core/mixin/fielddomain.py
--rw-rw-r--   0 david     (1000) david     (1000)     3257 2021-09-07 06:51:03.000000 cfdm-1.9.0.3/cfdm/count.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-03-10 18:35:36.958495 cfdm-1.9.0.3/cfdm/data/
--rw-rw-r--   0 david     (1000) david     (1000)      362 2021-01-22 18:34:02.000000 cfdm-1.9.0.3/cfdm/data/__init__.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-03-10 18:35:36.958495 cfdm-1.9.0.3/cfdm/data/abstract/
--rw-rw-r--   0 david     (1000) david     (1000)       70 2020-10-05 07:32:03.000000 cfdm-1.9.0.3/cfdm/data/abstract/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)      289 2021-05-10 16:58:27.000000 cfdm-1.9.0.3/cfdm/data/abstract/array.py
--rw-rw-r--   0 david     (1000) david     (1000)     7848 2021-05-10 16:58:27.000000 cfdm-1.9.0.3/cfdm/data/abstract/compressedarray.py
--rw-rw-r--   0 david     (1000) david     (1000)    77327 2022-01-31 11:22:47.000000 cfdm-1.9.0.3/cfdm/data/data.py
--rw-rw-r--   0 david     (1000) david     (1000)     5605 2021-05-10 16:58:27.000000 cfdm-1.9.0.3/cfdm/data/gatheredarray.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-03-10 18:35:36.958495 cfdm-1.9.0.3/cfdm/data/mixin/
--rw-rw-r--   0 david     (1000) david     (1000)      123 2020-10-05 07:32:03.000000 cfdm-1.9.0.3/cfdm/data/mixin/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)     6506 2021-05-10 16:58:27.000000 cfdm-1.9.0.3/cfdm/data/mixin/arraymixin.py
--rw-rw-r--   0 david     (1000) david     (1000)      839 2021-05-10 16:58:27.000000 cfdm-1.9.0.3/cfdm/data/mixin/raggedcontiguous.py
--rw-rw-r--   0 david     (1000) david     (1000)      789 2021-05-10 16:58:27.000000 cfdm-1.9.0.3/cfdm/data/mixin/raggedindexed.py
--rw-rw-r--   0 david     (1000) david     (1000)    13938 2021-09-07 06:51:03.000000 cfdm-1.9.0.3/cfdm/data/netcdfarray.py
--rw-rw-r--   0 david     (1000) david     (1000)     1521 2021-09-07 06:51:03.000000 cfdm-1.9.0.3/cfdm/data/numpyarray.py
--rw-rw-r--   0 david     (1000) david     (1000)     4288 2021-09-07 06:51:03.000000 cfdm-1.9.0.3/cfdm/data/raggedcontiguousarray.py
--rw-rw-r--   0 david     (1000) david     (1000)     4081 2021-09-07 06:51:03.000000 cfdm-1.9.0.3/cfdm/data/raggedindexedarray.py
--rw-rw-r--   0 david     (1000) david     (1000)     5403 2021-09-07 06:51:03.000000 cfdm-1.9.0.3/cfdm/data/raggedindexedcontiguousarray.py
--rw-rw-r--   0 david     (1000) david     (1000)     1712 2021-09-07 06:51:03.000000 cfdm-1.9.0.3/cfdm/datum.py
--rw-rw-r--   0 david     (1000) david     (1000)     9661 2021-09-07 06:51:03.000000 cfdm-1.9.0.3/cfdm/decorators.py
--rw-rw-r--   0 david     (1000) david     (1000)     4088 2021-09-07 06:51:03.000000 cfdm-1.9.0.3/cfdm/dimensioncoordinate.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-03-10 18:35:36.958495 cfdm-1.9.0.3/cfdm/docstring/
--rw-rw-r--   0 david     (1000) david     (1000)       59 2020-10-05 07:32:03.000000 cfdm-1.9.0.3/cfdm/docstring/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)    14606 2021-09-07 06:51:03.000000 cfdm-1.9.0.3/cfdm/docstring/docstring.py
--rw-rw-r--   0 david     (1000) david     (1000)    30492 2022-03-01 11:07:55.000000 cfdm-1.9.0.3/cfdm/domain.py
--rw-rw-r--   0 david     (1000) david     (1000)     3547 2021-09-07 06:51:03.000000 cfdm-1.9.0.3/cfdm/domainancillary.py
--rw-rw-r--   0 david     (1000) david     (1000)     8547 2021-09-07 06:51:03.000000 cfdm-1.9.0.3/cfdm/domainaxis.py
--rw-rw-r--   0 david     (1000) david     (1000)   207829 2021-09-07 06:51:03.000000 cfdm-1.9.0.3/cfdm/examplefield.py
--rw-rw-r--   0 david     (1000) david     (1000)    78173 2021-10-08 10:44:13.000000 cfdm-1.9.0.3/cfdm/field.py
--rw-rw-r--   0 david     (1000) david     (1000)     3217 2021-09-07 06:51:03.000000 cfdm-1.9.0.3/cfdm/fieldancillary.py
--rw-rw-r--   0 david     (1000) david     (1000)    42703 2021-09-07 12:16:42.000000 cfdm-1.9.0.3/cfdm/functions.py
--rw-rw-r--   0 david     (1000) david     (1000)     3744 2021-09-07 06:51:03.000000 cfdm-1.9.0.3/cfdm/index.py
--rw-rw-r--   0 david     (1000) david     (1000)     3423 2021-09-07 06:51:03.000000 cfdm-1.9.0.3/cfdm/interiorring.py
--rw-rw-r--   0 david     (1000) david     (1000)     2597 2021-09-07 06:51:03.000000 cfdm-1.9.0.3/cfdm/list.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-03-10 18:35:36.962494 cfdm-1.9.0.3/cfdm/mixin/
--rw-rw-r--   0 david     (1000) david     (1000)      624 2021-05-10 16:58:27.000000 cfdm-1.9.0.3/cfdm/mixin/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)     8137 2021-11-24 14:25:03.000000 cfdm-1.9.0.3/cfdm/mixin/container.py
--rw-rw-r--   0 david     (1000) david     (1000)     2756 2021-09-07 06:51:03.000000 cfdm-1.9.0.3/cfdm/mixin/coordinate.py
--rw-rw-r--   0 david     (1000) david     (1000)    42621 2021-09-07 06:51:03.000000 cfdm-1.9.0.3/cfdm/mixin/fielddomain.py
--rw-rw-r--   0 david     (1000) david     (1000)   107060 2021-09-07 06:51:03.000000 cfdm-1.9.0.3/cfdm/mixin/netcdf.py
--rw-rw-r--   0 david     (1000) david     (1000)     3593 2021-09-07 06:51:03.000000 cfdm-1.9.0.3/cfdm/mixin/parameters.py
--rw-rw-r--   0 david     (1000) david     (1000)     3478 2021-09-07 06:51:03.000000 cfdm-1.9.0.3/cfdm/mixin/parametersdomainancillaries.py
--rw-rw-r--   0 david     (1000) david     (1000)    13658 2021-09-07 06:51:03.000000 cfdm-1.9.0.3/cfdm/mixin/properties.py
--rw-rw-r--   0 david     (1000) david     (1000)    26475 2021-09-07 06:51:03.000000 cfdm-1.9.0.3/cfdm/mixin/propertiesdata.py
--rw-rw-r--   0 david     (1000) david     (1000)    54538 2021-09-07 06:51:03.000000 cfdm-1.9.0.3/cfdm/mixin/propertiesdatabounds.py
--rw-rw-r--   0 david     (1000) david     (1000)     1812 2021-09-07 06:51:03.000000 cfdm-1.9.0.3/cfdm/nodecountproperties.py
--rw-rw-r--   0 david     (1000) david     (1000)     2084 2021-09-07 06:51:03.000000 cfdm-1.9.0.3/cfdm/partnodecountproperties.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-03-10 18:35:36.966495 cfdm-1.9.0.3/cfdm/read_write/
--rw-rw-r--   0 david     (1000) david     (1000)       90 2021-01-22 18:34:02.000000 cfdm-1.9.0.3/cfdm/read_write/__init__.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-03-10 18:35:36.966495 cfdm-1.9.0.3/cfdm/read_write/abstract/
--rw-rw-r--   0 david     (1000) david     (1000)       44 2021-01-22 18:34:02.000000 cfdm-1.9.0.3/cfdm/read_write/abstract/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)     1235 2021-05-10 16:58:27.000000 cfdm-1.9.0.3/cfdm/read_write/abstract/abstractio.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-03-10 18:35:36.966495 cfdm-1.9.0.3/cfdm/read_write/netcdf/
--rw-rw-r--   0 david     (1000) david     (1000)       72 2020-07-03 10:25:19.000000 cfdm-1.9.0.3/cfdm/read_write/netcdf/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)     1607 2021-01-22 18:34:02.000000 cfdm-1.9.0.3/cfdm/read_write/netcdf/constants.py
--rw-rw-r--   0 david     (1000) david     (1000)   232163 2022-03-10 18:06:42.000000 cfdm-1.9.0.3/cfdm/read_write/netcdf/netcdfread.py
--rw-rw-r--   0 david     (1000) david     (1000)   177558 2022-03-10 18:06:42.000000 cfdm-1.9.0.3/cfdm/read_write/netcdf/netcdfwrite.py
--rw-rw-r--   0 david     (1000) david     (1000)    14818 2021-09-07 06:51:03.000000 cfdm-1.9.0.3/cfdm/read_write/read.py
--rw-rw-r--   0 david     (1000) david     (1000)    22283 2021-09-07 06:51:03.000000 cfdm-1.9.0.3/cfdm/read_write/write.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-03-10 18:35:36.970495 cfdm-1.9.0.3/cfdm/test/
--rw-rw-r--   0 david     (1000) david     (1000)        0 2020-03-20 18:57:35.000000 cfdm-1.9.0.3/cfdm/test/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)    44392 2021-09-07 06:51:03.000000 cfdm-1.9.0.3/cfdm/test/create_test_files.py
--rw-rw-r--   0 david     (1000) david     (1000)     5199 2021-09-07 06:51:03.000000 cfdm-1.9.0.3/cfdm/test/run_tests.py
--rw-rw-r--   0 david     (1000) david     (1000)     9100 2021-09-07 06:51:03.000000 cfdm-1.9.0.3/cfdm/test/setup_create_field.py
--rw-rw-r--   0 david     (1000) david     (1000)     9175 2021-09-07 06:51:03.000000 cfdm-1.9.0.3/cfdm/test/setup_create_field_2.py
--rw-rw-r--   0 david     (1000) david     (1000)     9597 2021-09-07 06:51:03.000000 cfdm-1.9.0.3/cfdm/test/setup_create_field_3.py
--rw-rw-r--   0 david     (1000) david     (1000)     5881 2021-09-07 06:51:03.000000 cfdm-1.9.0.3/cfdm/test/test_AuxiliaryCoordinate.py
--rw-rw-r--   0 david     (1000) david     (1000)     1693 2021-09-07 06:51:03.000000 cfdm-1.9.0.3/cfdm/test/test_CFDMImplementation.py
--rw-rw-r--   0 david     (1000) david     (1000)     2209 2021-09-07 06:51:03.000000 cfdm-1.9.0.3/cfdm/test/test_CellMeasure.py
--rw-rw-r--   0 david     (1000) david     (1000)     4837 2021-09-07 06:51:03.000000 cfdm-1.9.0.3/cfdm/test/test_CellMethod.py
--rw-rw-r--   0 david     (1000) david     (1000)    17748 2021-09-07 06:51:03.000000 cfdm-1.9.0.3/cfdm/test/test_Constructs.py
--rw-rw-r--   0 david     (1000) david     (1000)     8643 2022-01-31 11:09:58.000000 cfdm-1.9.0.3/cfdm/test/test_CoordinateReference.py
--rw-rw-r--   0 david     (1000) david     (1000)     1219 2021-09-07 06:51:03.000000 cfdm-1.9.0.3/cfdm/test/test_Count.py
--rw-rw-r--   0 david     (1000) david     (1000)    20770 2021-09-07 06:51:03.000000 cfdm-1.9.0.3/cfdm/test/test_Data.py
--rw-rw-r--   0 david     (1000) david     (1000)     3482 2021-09-07 06:51:03.000000 cfdm-1.9.0.3/cfdm/test/test_DimensionCoordinate.py
--rw-rw-r--   0 david     (1000) david     (1000)     5617 2022-03-10 18:06:42.000000 cfdm-1.9.0.3/cfdm/test/test_Domain.py
--rw-rw-r--   0 david     (1000) david     (1000)     4659 2021-09-07 06:51:03.000000 cfdm-1.9.0.3/cfdm/test/test_DomainAncillary.py
--rw-rw-r--   0 david     (1000) david     (1000)     2615 2021-09-07 06:51:03.000000 cfdm-1.9.0.3/cfdm/test/test_DomainAxis.py
--rw-rw-r--   0 david     (1000) david     (1000)    22053 2022-03-10 18:06:42.000000 cfdm-1.9.0.3/cfdm/test/test_Field.py
--rw-rw-r--   0 david     (1000) david     (1000)     3536 2021-09-07 06:51:03.000000 cfdm-1.9.0.3/cfdm/test/test_FieldAncillary.py
--rw-rw-r--   0 david     (1000) david     (1000)     1210 2021-09-07 06:51:03.000000 cfdm-1.9.0.3/cfdm/test/test_Index.py
--rw-rw-r--   0 david     (1000) david     (1000)     1620 2021-09-07 06:51:03.000000 cfdm-1.9.0.3/cfdm/test/test_InteriorRing.py
--rw-rw-r--   0 david     (1000) david     (1000)     1193 2021-09-07 06:51:03.000000 cfdm-1.9.0.3/cfdm/test/test_List.py
--rw-rw-r--   0 david     (1000) david     (1000)     1642 2021-09-07 06:51:03.000000 cfdm-1.9.0.3/cfdm/test/test_NodeCountProperties.py
--rw-rw-r--   0 david     (1000) david     (1000)     1449 2021-09-07 06:51:03.000000 cfdm-1.9.0.3/cfdm/test/test_NumpyArray.py
--rw-rw-r--   0 david     (1000) david     (1000)     1668 2021-09-07 06:51:03.000000 cfdm-1.9.0.3/cfdm/test/test_PartNodeCountProperties.py
--rw-rw-r--   0 david     (1000) david     (1000)     1620 2021-09-07 06:51:03.000000 cfdm-1.9.0.3/cfdm/test/test_RaggedContiguousArray.py
--rw-rw-r--   0 david     (1000) david     (1000)     1602 2021-09-07 06:51:03.000000 cfdm-1.9.0.3/cfdm/test/test_RaggedIndexedArray.py
--rw-rw-r--   0 david     (1000) david     (1000)     1690 2021-09-07 06:51:03.000000 cfdm-1.9.0.3/cfdm/test/test_RaggedIndexedContiguousArray.py
--rw-rw-r--   0 david     (1000) david     (1000)     8342 2021-09-07 06:51:03.000000 cfdm-1.9.0.3/cfdm/test/test_core_1.py
--rw-rw-r--   0 david     (1000) david     (1000)     1235 2021-09-07 06:51:03.000000 cfdm-1.9.0.3/cfdm/test/test_core_2.py
--rw-rw-r--   0 david     (1000) david     (1000)    11106 2021-09-07 06:51:03.000000 cfdm-1.9.0.3/cfdm/test/test_decorators.py
--rw-rw-r--   0 david     (1000) david     (1000)     9485 2021-09-07 06:51:03.000000 cfdm-1.9.0.3/cfdm/test/test_docstring.py
--rw-rw-r--   0 david     (1000) david     (1000)    14747 2021-09-07 06:51:03.000000 cfdm-1.9.0.3/cfdm/test/test_dsg.py
--rw-rw-r--   0 david     (1000) david     (1000)     5612 2021-09-07 06:51:03.000000 cfdm-1.9.0.3/cfdm/test/test_external.py
--rw-rw-r--   0 david     (1000) david     (1000)    19903 2022-01-31 11:09:58.000000 cfdm-1.9.0.3/cfdm/test/test_functions.py
--rw-rw-r--   0 david     (1000) david     (1000)    12115 2021-09-07 06:51:03.000000 cfdm-1.9.0.3/cfdm/test/test_gathering.py
--rw-rw-r--   0 david     (1000) david     (1000)    10868 2021-09-07 06:51:03.000000 cfdm-1.9.0.3/cfdm/test/test_geometry.py
--rw-rw-r--   0 david     (1000) david     (1000)    19010 2022-03-10 18:06:42.000000 cfdm-1.9.0.3/cfdm/test/test_groups.py
--rw-rw-r--   0 david     (1000) david     (1000)    24265 2021-09-07 06:51:03.000000 cfdm-1.9.0.3/cfdm/test/test_netCDF.py
--rw-rw-r--   0 david     (1000) david     (1000)    31958 2022-01-31 11:09:58.000000 cfdm-1.9.0.3/cfdm/test/test_read_write.py
--rw-rw-r--   0 david     (1000) david     (1000)     4011 2021-09-07 06:51:03.000000 cfdm-1.9.0.3/cfdm/test/test_string.py
--rw-rw-r--   0 david     (1000) david     (1000)     3164 2021-09-07 06:51:03.000000 cfdm-1.9.0.3/cfdm/test/test_style.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-03-10 18:35:36.946495 cfdm-1.9.0.3/cfdm.egg-info/
--rw-rw-r--   0 david     (1000) david     (1000)     4319 2022-03-10 18:35:36.000000 cfdm-1.9.0.3/cfdm.egg-info/PKG-INFO
--rw-rw-r--   0 david     (1000) david     (1000)     4320 2022-03-10 18:35:36.000000 cfdm-1.9.0.3/cfdm.egg-info/SOURCES.txt
--rw-rw-r--   0 david     (1000) david     (1000)        1 2022-03-10 18:35:36.000000 cfdm-1.9.0.3/cfdm.egg-info/dependency_links.txt
--rw-rw-r--   0 david     (1000) david     (1000)      241 2022-03-10 18:35:36.000000 cfdm-1.9.0.3/cfdm.egg-info/requires.txt
--rw-rw-r--   0 david     (1000) david     (1000)        5 2022-03-10 18:35:36.000000 cfdm-1.9.0.3/cfdm.egg-info/top_level.txt
--rw-rw-r--   0 david     (1000) david     (1000)      872 2021-09-07 06:51:03.000000 cfdm-1.9.0.3/pyproject.toml
--rw-rw-r--   0 david     (1000) david     (1000)       81 2022-03-10 18:16:14.000000 cfdm-1.9.0.3/requirements.txt
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-03-10 18:35:36.970495 cfdm-1.9.0.3/scripts/
--rwxrwxr-x   0 david     (1000) david     (1000)     4671 2021-09-07 06:51:03.000000 cfdm-1.9.0.3/scripts/cfdump
--rw-rw-r--   0 david     (1000) david     (1000)       38 2022-03-10 18:35:36.970495 cfdm-1.9.0.3/setup.cfg
--rwxrwxr-x   0 david     (1000) david     (1000)     5907 2021-09-21 13:39:06.000000 cfdm-1.9.0.3/setup.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-07-18 14:23:03.268627 cfdm-1.9.0.4/
+-rw-rw-r--   0 david     (1000) david     (1000)     2661 2020-10-05 07:32:03.000000 cfdm-1.9.0.4/CODE_OF_CONDUCT.md
+-rw-rw-r--   0 david     (1000) david     (1000)     1179 2020-10-05 07:32:03.000000 cfdm-1.9.0.4/CONTRIBUTING.md
+-rw-rw-r--   0 david     (1000) david     (1000)    16786 2022-07-18 13:59:39.000000 cfdm-1.9.0.4/Changelog.rst
+-rw-rw-r--   0 david     (1000) david     (1000)     1065 2020-03-20 18:57:35.000000 cfdm-1.9.0.4/LICENSE
+-rw-rw-r--   0 david     (1000) david     (1000)      132 2020-10-09 10:28:32.000000 cfdm-1.9.0.4/MANIFEST.in
+-rw-rw-r--   0 david     (1000) david     (1000)     4319 2022-07-18 14:23:03.268627 cfdm-1.9.0.4/PKG-INFO
+-rw-rw-r--   0 david     (1000) david     (1000)     6390 2022-07-18 08:28:33.000000 cfdm-1.9.0.4/README.md
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-07-18 14:23:03.228628 cfdm-1.9.0.4/cfdm/
+-rw-rw-r--   0 david     (1000) david     (1000)     5834 2022-07-18 08:28:33.000000 cfdm-1.9.0.4/cfdm/__init__.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-07-18 14:23:03.232627 cfdm-1.9.0.4/cfdm/abstract/
+-rw-rw-r--   0 david     (1000) david     (1000)       76 2020-10-05 07:32:03.000000 cfdm-1.9.0.4/cfdm/abstract/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)      186 2021-09-07 06:51:03.000000 cfdm-1.9.0.4/cfdm/abstract/container.py
+-rw-rw-r--   0 david     (1000) david     (1000)     3438 2022-07-18 08:28:33.000000 cfdm-1.9.0.4/cfdm/abstract/implementation.py
+-rw-rw-r--   0 david     (1000) david     (1000)     3941 2021-09-07 06:51:03.000000 cfdm-1.9.0.4/cfdm/auxiliarycoordinate.py
+-rw-rw-r--   0 david     (1000) david     (1000)     8289 2022-07-18 08:28:33.000000 cfdm-1.9.0.4/cfdm/bounds.py
+-rw-rw-r--   0 david     (1000) david     (1000)    12863 2022-07-18 08:28:33.000000 cfdm-1.9.0.4/cfdm/cellmeasure.py
+-rw-rw-r--   0 david     (1000) david     (1000)    16210 2022-07-18 08:28:33.000000 cfdm-1.9.0.4/cfdm/cellmethod.py
+-rw-rw-r--   0 david     (1000) david     (1000)    72755 2022-07-18 08:28:33.000000 cfdm-1.9.0.4/cfdm/cfdmimplementation.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1501 2021-09-07 06:51:03.000000 cfdm-1.9.0.4/cfdm/constants.py
+-rw-rw-r--   0 david     (1000) david     (1000)   113901 2022-07-18 08:28:33.000000 cfdm-1.9.0.4/cfdm/constructs.py
+-rw-rw-r--   0 david     (1000) david     (1000)      970 2021-09-07 06:51:03.000000 cfdm-1.9.0.4/cfdm/coordinateconversion.py
+-rw-rw-r--   0 david     (1000) david     (1000)    19224 2022-07-18 08:28:33.000000 cfdm-1.9.0.4/cfdm/coordinatereference.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-07-18 14:23:03.232627 cfdm-1.9.0.4/cfdm/core/
+-rw-rw-r--   0 david     (1000) david     (1000)     2122 2022-07-18 14:00:00.000000 cfdm-1.9.0.4/cfdm/core/__init__.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-07-18 14:23:03.236627 cfdm-1.9.0.4/cfdm/core/abstract/
+-rw-rw-r--   0 david     (1000) david     (1000)      307 2021-01-22 18:34:02.000000 cfdm-1.9.0.4/cfdm/core/abstract/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)     9520 2022-07-18 08:28:33.000000 cfdm-1.9.0.4/cfdm/core/abstract/container.py
+-rw-rw-r--   0 david     (1000) david     (1000)     5174 2022-07-18 08:28:33.000000 cfdm-1.9.0.4/cfdm/core/abstract/coordinate.py
+-rw-rw-r--   0 david     (1000) david     (1000)     9571 2022-07-18 08:28:33.000000 cfdm-1.9.0.4/cfdm/core/abstract/parameters.py
+-rw-rw-r--   0 david     (1000) david     (1000)    11097 2022-07-18 08:28:33.000000 cfdm-1.9.0.4/cfdm/core/abstract/parametersdomainancillaries.py
+-rw-rw-r--   0 david     (1000) david     (1000)    10685 2022-07-18 08:28:33.000000 cfdm-1.9.0.4/cfdm/core/abstract/properties.py
+-rw-rw-r--   0 david     (1000) david     (1000)    11427 2022-07-18 08:28:33.000000 cfdm-1.9.0.4/cfdm/core/abstract/propertiesdata.py
+-rw-rw-r--   0 david     (1000) david     (1000)    19349 2022-07-18 08:28:33.000000 cfdm-1.9.0.4/cfdm/core/abstract/propertiesdatabounds.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1987 2022-07-18 08:28:33.000000 cfdm-1.9.0.4/cfdm/core/auxiliarycoordinate.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1517 2021-05-10 16:58:27.000000 cfdm-1.9.0.4/cfdm/core/bounds.py
+-rw-rw-r--   0 david     (1000) david     (1000)     6281 2022-07-18 08:28:33.000000 cfdm-1.9.0.4/cfdm/core/cellmeasure.py
+-rw-rw-r--   0 david     (1000) david     (1000)    17016 2022-07-18 08:28:33.000000 cfdm-1.9.0.4/cfdm/core/cellmethod.py
+-rw-rw-r--   0 david     (1000) david     (1000)    45405 2022-07-18 08:28:33.000000 cfdm-1.9.0.4/cfdm/core/constructs.py
+-rw-rw-r--   0 david     (1000) david     (1000)      949 2021-03-22 16:15:42.000000 cfdm-1.9.0.4/cfdm/core/coordinateconversion.py
+-rw-rw-r--   0 david     (1000) david     (1000)    21103 2022-07-18 08:28:33.000000 cfdm-1.9.0.4/cfdm/core/coordinatereference.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-07-18 14:23:03.236627 cfdm-1.9.0.4/cfdm/core/data/
+-rw-rw-r--   0 david     (1000) david     (1000)       86 2020-10-05 07:32:03.000000 cfdm-1.9.0.4/cfdm/core/data/__init__.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-07-18 14:23:03.236627 cfdm-1.9.0.4/cfdm/core/data/abstract/
+-rw-rw-r--   0 david     (1000) david     (1000)       25 2020-03-20 18:57:35.000000 cfdm-1.9.0.4/cfdm/core/data/abstract/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)     4952 2022-07-18 08:28:33.000000 cfdm-1.9.0.4/cfdm/core/data/abstract/array.py
+-rw-rw-r--   0 david     (1000) david     (1000)    21952 2022-07-18 08:28:33.000000 cfdm-1.9.0.4/cfdm/core/data/data.py
+-rw-rw-r--   0 david     (1000) david     (1000)     3575 2022-07-18 08:28:33.000000 cfdm-1.9.0.4/cfdm/core/data/numpyarray.py
+-rw-rw-r--   0 david     (1000) david     (1000)      771 2021-03-22 16:15:42.000000 cfdm-1.9.0.4/cfdm/core/datum.py
+-rw-rw-r--   0 david     (1000) david     (1000)     3736 2022-07-18 08:28:33.000000 cfdm-1.9.0.4/cfdm/core/dimensioncoordinate.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-07-18 14:23:03.236627 cfdm-1.9.0.4/cfdm/core/docstring/
+-rw-rw-r--   0 david     (1000) david     (1000)       59 2020-10-05 07:32:03.000000 cfdm-1.9.0.4/cfdm/core/docstring/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)     5320 2022-07-18 08:28:33.000000 cfdm-1.9.0.4/cfdm/core/docstring/docstring.py
+-rw-rw-r--   0 david     (1000) david     (1000)     7868 2022-07-18 08:28:33.000000 cfdm-1.9.0.4/cfdm/core/domain.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1305 2022-07-18 08:28:33.000000 cfdm-1.9.0.4/cfdm/core/domainancillary.py
+-rw-rw-r--   0 david     (1000) david     (1000)     4864 2022-07-18 08:28:33.000000 cfdm-1.9.0.4/cfdm/core/domainaxis.py
+-rw-rw-r--   0 david     (1000) david     (1000)    19000 2022-07-18 08:28:33.000000 cfdm-1.9.0.4/cfdm/core/field.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1637 2022-07-18 08:28:33.000000 cfdm-1.9.0.4/cfdm/core/fieldancillary.py
+-rw-rw-r--   0 david     (1000) david     (1000)     3028 2022-07-18 08:28:33.000000 cfdm-1.9.0.4/cfdm/core/functions.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1009 2021-03-22 16:15:42.000000 cfdm-1.9.0.4/cfdm/core/interiorring.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-07-18 14:23:03.236627 cfdm-1.9.0.4/cfdm/core/meta/
+-rw-rw-r--   0 david     (1000) david     (1000)       51 2020-10-05 07:32:03.000000 cfdm-1.9.0.4/cfdm/core/meta/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)    24256 2022-07-18 08:28:41.000000 cfdm-1.9.0.4/cfdm/core/meta/docstringrewrite.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-07-18 14:23:03.240628 cfdm-1.9.0.4/cfdm/core/mixin/
+-rw-rw-r--   0 david     (1000) david     (1000)       37 2021-05-10 16:58:27.000000 cfdm-1.9.0.4/cfdm/core/mixin/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)    11933 2022-07-18 08:28:33.000000 cfdm-1.9.0.4/cfdm/core/mixin/fielddomain.py
+-rw-rw-r--   0 david     (1000) david     (1000)     3257 2021-09-07 06:51:03.000000 cfdm-1.9.0.4/cfdm/count.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-07-18 14:23:03.240628 cfdm-1.9.0.4/cfdm/data/
+-rw-rw-r--   0 david     (1000) david     (1000)      362 2022-07-18 08:28:33.000000 cfdm-1.9.0.4/cfdm/data/__init__.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-07-18 14:23:03.240628 cfdm-1.9.0.4/cfdm/data/abstract/
+-rw-rw-r--   0 david     (1000) david     (1000)       70 2022-07-18 08:28:33.000000 cfdm-1.9.0.4/cfdm/data/abstract/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)      289 2022-07-18 08:28:33.000000 cfdm-1.9.0.4/cfdm/data/abstract/array.py
+-rw-rw-r--   0 david     (1000) david     (1000)     7848 2022-07-18 08:28:33.000000 cfdm-1.9.0.4/cfdm/data/abstract/compressedarray.py
+-rw-rw-r--   0 david     (1000) david     (1000)    77327 2022-07-18 08:28:33.000000 cfdm-1.9.0.4/cfdm/data/data.py
+-rw-rw-r--   0 david     (1000) david     (1000)     5605 2022-07-18 08:28:33.000000 cfdm-1.9.0.4/cfdm/data/gatheredarray.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-07-18 14:23:03.240628 cfdm-1.9.0.4/cfdm/data/mixin/
+-rw-rw-r--   0 david     (1000) david     (1000)      123 2022-07-18 08:28:33.000000 cfdm-1.9.0.4/cfdm/data/mixin/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)     6506 2022-07-18 08:28:33.000000 cfdm-1.9.0.4/cfdm/data/mixin/arraymixin.py
+-rw-rw-r--   0 david     (1000) david     (1000)      839 2022-07-18 08:28:33.000000 cfdm-1.9.0.4/cfdm/data/mixin/raggedcontiguous.py
+-rw-rw-r--   0 david     (1000) david     (1000)      789 2022-07-18 08:28:33.000000 cfdm-1.9.0.4/cfdm/data/mixin/raggedindexed.py
+-rw-rw-r--   0 david     (1000) david     (1000)    13938 2022-07-18 08:28:33.000000 cfdm-1.9.0.4/cfdm/data/netcdfarray.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1521 2022-07-18 08:28:33.000000 cfdm-1.9.0.4/cfdm/data/numpyarray.py
+-rw-rw-r--   0 david     (1000) david     (1000)     4288 2022-07-18 08:28:33.000000 cfdm-1.9.0.4/cfdm/data/raggedcontiguousarray.py
+-rw-rw-r--   0 david     (1000) david     (1000)     4081 2022-07-18 08:28:33.000000 cfdm-1.9.0.4/cfdm/data/raggedindexedarray.py
+-rw-rw-r--   0 david     (1000) david     (1000)     5403 2022-07-18 08:28:33.000000 cfdm-1.9.0.4/cfdm/data/raggedindexedcontiguousarray.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1712 2021-09-07 06:51:03.000000 cfdm-1.9.0.4/cfdm/datum.py
+-rw-rw-r--   0 david     (1000) david     (1000)     9661 2021-09-07 06:51:03.000000 cfdm-1.9.0.4/cfdm/decorators.py
+-rw-rw-r--   0 david     (1000) david     (1000)     4088 2021-09-07 06:51:03.000000 cfdm-1.9.0.4/cfdm/dimensioncoordinate.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-07-18 14:23:03.244628 cfdm-1.9.0.4/cfdm/docstring/
+-rw-rw-r--   0 david     (1000) david     (1000)       59 2020-10-05 07:32:03.000000 cfdm-1.9.0.4/cfdm/docstring/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)    14606 2022-07-18 08:28:33.000000 cfdm-1.9.0.4/cfdm/docstring/docstring.py
+-rw-rw-r--   0 david     (1000) david     (1000)    30492 2022-07-18 08:28:33.000000 cfdm-1.9.0.4/cfdm/domain.py
+-rw-rw-r--   0 david     (1000) david     (1000)     3547 2021-09-07 06:51:03.000000 cfdm-1.9.0.4/cfdm/domainancillary.py
+-rw-rw-r--   0 david     (1000) david     (1000)     8547 2022-07-18 08:28:33.000000 cfdm-1.9.0.4/cfdm/domainaxis.py
+-rw-rw-r--   0 david     (1000) david     (1000)   207829 2022-07-18 08:28:33.000000 cfdm-1.9.0.4/cfdm/examplefield.py
+-rw-rw-r--   0 david     (1000) david     (1000)    78173 2022-07-18 08:28:33.000000 cfdm-1.9.0.4/cfdm/field.py
+-rw-rw-r--   0 david     (1000) david     (1000)     3217 2021-09-07 06:51:03.000000 cfdm-1.9.0.4/cfdm/fieldancillary.py
+-rw-rw-r--   0 david     (1000) david     (1000)    42703 2022-07-18 08:28:33.000000 cfdm-1.9.0.4/cfdm/functions.py
+-rw-rw-r--   0 david     (1000) david     (1000)     3744 2022-07-18 08:28:33.000000 cfdm-1.9.0.4/cfdm/index.py
+-rw-rw-r--   0 david     (1000) david     (1000)     3423 2022-07-18 08:28:33.000000 cfdm-1.9.0.4/cfdm/interiorring.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2597 2021-09-07 06:51:03.000000 cfdm-1.9.0.4/cfdm/list.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-07-18 14:23:03.244628 cfdm-1.9.0.4/cfdm/mixin/
+-rw-rw-r--   0 david     (1000) david     (1000)      624 2022-07-18 08:28:33.000000 cfdm-1.9.0.4/cfdm/mixin/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)     8137 2021-11-24 14:25:03.000000 cfdm-1.9.0.4/cfdm/mixin/container.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2756 2022-07-18 08:28:33.000000 cfdm-1.9.0.4/cfdm/mixin/coordinate.py
+-rw-rw-r--   0 david     (1000) david     (1000)    42621 2022-07-18 08:28:33.000000 cfdm-1.9.0.4/cfdm/mixin/fielddomain.py
+-rw-rw-r--   0 david     (1000) david     (1000)   107060 2022-07-18 08:28:33.000000 cfdm-1.9.0.4/cfdm/mixin/netcdf.py
+-rw-rw-r--   0 david     (1000) david     (1000)     3593 2022-07-18 08:28:33.000000 cfdm-1.9.0.4/cfdm/mixin/parameters.py
+-rw-rw-r--   0 david     (1000) david     (1000)     3478 2022-07-18 08:28:33.000000 cfdm-1.9.0.4/cfdm/mixin/parametersdomainancillaries.py
+-rw-rw-r--   0 david     (1000) david     (1000)    13658 2022-07-18 08:28:33.000000 cfdm-1.9.0.4/cfdm/mixin/properties.py
+-rw-rw-r--   0 david     (1000) david     (1000)    26475 2022-07-18 08:28:33.000000 cfdm-1.9.0.4/cfdm/mixin/propertiesdata.py
+-rw-rw-r--   0 david     (1000) david     (1000)    54538 2022-07-18 08:28:33.000000 cfdm-1.9.0.4/cfdm/mixin/propertiesdatabounds.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1812 2021-09-07 06:51:03.000000 cfdm-1.9.0.4/cfdm/nodecountproperties.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2084 2021-09-07 06:51:03.000000 cfdm-1.9.0.4/cfdm/partnodecountproperties.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-07-18 14:23:03.244628 cfdm-1.9.0.4/cfdm/read_write/
+-rw-rw-r--   0 david     (1000) david     (1000)       90 2021-01-22 18:34:02.000000 cfdm-1.9.0.4/cfdm/read_write/__init__.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-07-18 14:23:03.244628 cfdm-1.9.0.4/cfdm/read_write/abstract/
+-rw-rw-r--   0 david     (1000) david     (1000)       44 2021-01-22 18:34:02.000000 cfdm-1.9.0.4/cfdm/read_write/abstract/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1235 2021-05-10 16:58:27.000000 cfdm-1.9.0.4/cfdm/read_write/abstract/abstractio.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-07-18 14:23:03.248628 cfdm-1.9.0.4/cfdm/read_write/netcdf/
+-rw-rw-r--   0 david     (1000) david     (1000)       72 2020-07-03 10:25:19.000000 cfdm-1.9.0.4/cfdm/read_write/netcdf/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1607 2021-01-22 18:34:02.000000 cfdm-1.9.0.4/cfdm/read_write/netcdf/constants.py
+-rw-rw-r--   0 david     (1000) david     (1000)   232225 2022-07-18 08:28:41.000000 cfdm-1.9.0.4/cfdm/read_write/netcdf/netcdfread.py
+-rw-rw-r--   0 david     (1000) david     (1000)   177665 2022-07-18 13:59:11.000000 cfdm-1.9.0.4/cfdm/read_write/netcdf/netcdfwrite.py
+-rw-rw-r--   0 david     (1000) david     (1000)    14818 2022-07-18 08:28:33.000000 cfdm-1.9.0.4/cfdm/read_write/read.py
+-rw-rw-r--   0 david     (1000) david     (1000)    22283 2022-07-18 08:28:33.000000 cfdm-1.9.0.4/cfdm/read_write/write.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-07-18 14:23:03.268627 cfdm-1.9.0.4/cfdm/test/
+-rw-rw-r--   0 david     (1000) david     (1000)        0 2020-03-20 18:57:35.000000 cfdm-1.9.0.4/cfdm/test/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)    44392 2022-07-18 08:28:33.000000 cfdm-1.9.0.4/cfdm/test/create_test_files.py
+-rw-rw-r--   0 david     (1000) david     (1000)     5199 2021-09-07 06:51:03.000000 cfdm-1.9.0.4/cfdm/test/run_tests.py
+-rw-rw-r--   0 david     (1000) david     (1000)     9100 2021-09-07 06:51:03.000000 cfdm-1.9.0.4/cfdm/test/setup_create_field.py
+-rw-rw-r--   0 david     (1000) david     (1000)     9175 2021-09-07 06:51:03.000000 cfdm-1.9.0.4/cfdm/test/setup_create_field_2.py
+-rw-rw-r--   0 david     (1000) david     (1000)     9597 2021-09-07 06:51:03.000000 cfdm-1.9.0.4/cfdm/test/setup_create_field_3.py
+-rw-rw-r--   0 david     (1000) david     (1000)     5881 2021-09-07 06:51:03.000000 cfdm-1.9.0.4/cfdm/test/test_AuxiliaryCoordinate.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1693 2021-09-07 06:51:03.000000 cfdm-1.9.0.4/cfdm/test/test_CFDMImplementation.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2209 2021-09-07 06:51:03.000000 cfdm-1.9.0.4/cfdm/test/test_CellMeasure.py
+-rw-rw-r--   0 david     (1000) david     (1000)     4837 2021-09-07 06:51:03.000000 cfdm-1.9.0.4/cfdm/test/test_CellMethod.py
+-rw-rw-r--   0 david     (1000) david     (1000)    17748 2021-09-07 06:51:03.000000 cfdm-1.9.0.4/cfdm/test/test_Constructs.py
+-rw-rw-r--   0 david     (1000) david     (1000)     8643 2022-01-31 11:09:58.000000 cfdm-1.9.0.4/cfdm/test/test_CoordinateReference.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1219 2021-09-07 06:51:03.000000 cfdm-1.9.0.4/cfdm/test/test_Count.py
+-rw-rw-r--   0 david     (1000) david     (1000)    20770 2022-07-18 08:28:33.000000 cfdm-1.9.0.4/cfdm/test/test_Data.py
+-rw-rw-r--   0 david     (1000) david     (1000)     3482 2021-09-07 06:51:03.000000 cfdm-1.9.0.4/cfdm/test/test_DimensionCoordinate.py
+-rw-rw-r--   0 david     (1000) david     (1000)     5617 2022-07-18 08:28:33.000000 cfdm-1.9.0.4/cfdm/test/test_Domain.py
+-rw-rw-r--   0 david     (1000) david     (1000)     4659 2022-07-18 08:28:33.000000 cfdm-1.9.0.4/cfdm/test/test_DomainAncillary.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2615 2021-09-07 06:51:03.000000 cfdm-1.9.0.4/cfdm/test/test_DomainAxis.py
+-rw-rw-r--   0 david     (1000) david     (1000)    22053 2022-07-18 08:28:33.000000 cfdm-1.9.0.4/cfdm/test/test_Field.py
+-rw-rw-r--   0 david     (1000) david     (1000)     3536 2021-09-07 06:51:03.000000 cfdm-1.9.0.4/cfdm/test/test_FieldAncillary.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1210 2021-09-07 06:51:03.000000 cfdm-1.9.0.4/cfdm/test/test_Index.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1620 2021-09-07 06:51:03.000000 cfdm-1.9.0.4/cfdm/test/test_InteriorRing.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1193 2021-09-07 06:51:03.000000 cfdm-1.9.0.4/cfdm/test/test_List.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1642 2021-09-07 06:51:03.000000 cfdm-1.9.0.4/cfdm/test/test_NodeCountProperties.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1449 2021-09-07 06:51:03.000000 cfdm-1.9.0.4/cfdm/test/test_NumpyArray.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1668 2021-09-07 06:51:03.000000 cfdm-1.9.0.4/cfdm/test/test_PartNodeCountProperties.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1620 2022-07-18 08:28:33.000000 cfdm-1.9.0.4/cfdm/test/test_RaggedContiguousArray.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1602 2022-07-18 08:28:33.000000 cfdm-1.9.0.4/cfdm/test/test_RaggedIndexedArray.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1690 2022-07-18 08:28:33.000000 cfdm-1.9.0.4/cfdm/test/test_RaggedIndexedContiguousArray.py
+-rw-rw-r--   0 david     (1000) david     (1000)     8342 2021-09-07 06:51:03.000000 cfdm-1.9.0.4/cfdm/test/test_core_1.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1235 2021-09-07 06:51:03.000000 cfdm-1.9.0.4/cfdm/test/test_core_2.py
+-rw-rw-r--   0 david     (1000) david     (1000)    11044 2022-07-18 08:28:41.000000 cfdm-1.9.0.4/cfdm/test/test_decorators.py
+-rw-rw-r--   0 david     (1000) david     (1000)     9485 2021-09-07 06:51:03.000000 cfdm-1.9.0.4/cfdm/test/test_docstring.py
+-rw-rw-r--   0 david     (1000) david     (1000)    14747 2021-09-07 06:51:03.000000 cfdm-1.9.0.4/cfdm/test/test_dsg.py
+-rw-rw-r--   0 david     (1000) david     (1000)     5612 2022-07-18 08:28:33.000000 cfdm-1.9.0.4/cfdm/test/test_external.py
+-rw-rw-r--   0 david     (1000) david     (1000)    19903 2022-07-18 08:28:33.000000 cfdm-1.9.0.4/cfdm/test/test_functions.py
+-rw-rw-r--   0 david     (1000) david     (1000)    12115 2022-07-18 08:28:33.000000 cfdm-1.9.0.4/cfdm/test/test_gathering.py
+-rw-rw-r--   0 david     (1000) david     (1000)    10868 2021-09-07 06:51:03.000000 cfdm-1.9.0.4/cfdm/test/test_geometry.py
+-rw-rw-r--   0 david     (1000) david     (1000)    19010 2022-03-10 18:06:42.000000 cfdm-1.9.0.4/cfdm/test/test_groups.py
+-rw-rw-r--   0 david     (1000) david     (1000)    24265 2022-07-18 08:28:33.000000 cfdm-1.9.0.4/cfdm/test/test_netCDF.py
+-rw-rw-r--   0 david     (1000) david     (1000)    32353 2022-07-18 08:28:41.000000 cfdm-1.9.0.4/cfdm/test/test_read_write.py
+-rw-rw-r--   0 david     (1000) david     (1000)     4011 2021-09-07 06:51:03.000000 cfdm-1.9.0.4/cfdm/test/test_string.py
+-rw-rw-r--   0 david     (1000) david     (1000)     3164 2021-09-07 06:51:03.000000 cfdm-1.9.0.4/cfdm/test/test_style.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-07-18 14:23:03.228628 cfdm-1.9.0.4/cfdm.egg-info/
+-rw-rw-r--   0 david     (1000) david     (1000)     4319 2022-07-18 14:23:03.000000 cfdm-1.9.0.4/cfdm.egg-info/PKG-INFO
+-rw-rw-r--   0 david     (1000) david     (1000)     4320 2022-07-18 14:23:03.000000 cfdm-1.9.0.4/cfdm.egg-info/SOURCES.txt
+-rw-rw-r--   0 david     (1000) david     (1000)        1 2022-07-18 14:23:03.000000 cfdm-1.9.0.4/cfdm.egg-info/dependency_links.txt
+-rw-rw-r--   0 david     (1000) david     (1000)      241 2022-07-18 14:23:03.000000 cfdm-1.9.0.4/cfdm.egg-info/requires.txt
+-rw-rw-r--   0 david     (1000) david     (1000)        5 2022-07-18 14:23:03.000000 cfdm-1.9.0.4/cfdm.egg-info/top_level.txt
+-rw-rw-r--   0 david     (1000) david     (1000)      872 2021-09-07 06:51:03.000000 cfdm-1.9.0.4/pyproject.toml
+-rw-rw-r--   0 david     (1000) david     (1000)       81 2022-03-10 18:16:14.000000 cfdm-1.9.0.4/requirements.txt
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2022-07-18 14:23:03.268627 cfdm-1.9.0.4/scripts/
+-rwxrwxr-x   0 david     (1000) david     (1000)     4671 2021-09-07 06:51:03.000000 cfdm-1.9.0.4/scripts/cfdump
+-rw-rw-r--   0 david     (1000) david     (1000)       38 2022-07-18 14:23:03.268627 cfdm-1.9.0.4/setup.cfg
+-rwxrwxr-x   0 david     (1000) david     (1000)     5907 2021-09-21 13:39:06.000000 cfdm-1.9.0.4/setup.py
```

### Comparing `cfdm-1.9.0.3/CODE_OF_CONDUCT.md` & `cfdm-1.9.0.4/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `cfdm-1.9.0.3/CONTRIBUTING.md` & `cfdm-1.9.0.4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `cfdm-1.9.0.3/Changelog.rst` & `cfdm-1.9.0.4/Changelog.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Version 1.9.0.4
+---------------
+
+**2022-07-18**
+
+* Upgrade to allow cfdm to work with Python 3.10
+  (https://github.com/NCAS-CMS/cfdm/issues/187)
+* Fix bug that caused a hang when reading zero-length files
+  (https://github.com/NCAS-CMS/cfdm/issues/190)
+* Fix bug to prevent error when writing vlen strings to a netCDF file
+  when compression has been set (for `netCDF4>=1.6.0`)
+  (https://github.com/NCAS-CMS/cfdm/issues/199)
+  
+----
+
 Version 1.9.0.3
 ---------------
 
 **2022-03-10**
 
 * Fixed bug that caused a failure from `cfdm.write` when writing
   identical (auxiliary) coordinates to different data variables in
```

### Comparing `cfdm-1.9.0.3/LICENSE` & `cfdm-1.9.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cfdm-1.9.0.3/PKG-INFO` & `cfdm-1.9.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cfdm
-Version: 1.9.0.3
+Version: 1.9.0.4
 Summary: A Python reference implementation of the CF data model
 Home-page: https://ncas-cms.github.io/cfdm
 Author: David Hassell, Sadie Bartholomew
 Author-email: david.hassell@ncas.ac.uk
 Maintainer: David Hassell, Sadie Bartholomew
 License: MIT
 Download-URL: https://pypi.org/project/cfdm/#files
```

### Comparing `cfdm-1.9.0.3/README.md` & `cfdm-1.9.0.4/README.md`

 * *Files identical despite different names*

### Comparing `cfdm-1.9.0.3/cfdm/__init__.py` & `cfdm-1.9.0.4/cfdm/__init__.py`

 * *Files identical despite different names*

### Comparing `cfdm-1.9.0.3/cfdm/abstract/implementation.py` & `cfdm-1.9.0.4/cfdm/abstract/implementation.py`

 * *Files identical despite different names*

### Comparing `cfdm-1.9.0.3/cfdm/auxiliarycoordinate.py` & `cfdm-1.9.0.4/cfdm/auxiliarycoordinate.py`

 * *Files identical despite different names*

### Comparing `cfdm-1.9.0.3/cfdm/bounds.py` & `cfdm-1.9.0.4/cfdm/bounds.py`

 * *Files identical despite different names*

### Comparing `cfdm-1.9.0.3/cfdm/cellmeasure.py` & `cfdm-1.9.0.4/cfdm/cellmeasure.py`

 * *Files identical despite different names*

### Comparing `cfdm-1.9.0.3/cfdm/cellmethod.py` & `cfdm-1.9.0.4/cfdm/cellmethod.py`

 * *Files identical despite different names*

### Comparing `cfdm-1.9.0.3/cfdm/cfdmimplementation.py` & `cfdm-1.9.0.4/cfdm/cfdmimplementation.py`

 * *Files identical despite different names*

### Comparing `cfdm-1.9.0.3/cfdm/constants.py` & `cfdm-1.9.0.4/cfdm/constants.py`

 * *Files identical despite different names*

### Comparing `cfdm-1.9.0.3/cfdm/constructs.py` & `cfdm-1.9.0.4/cfdm/constructs.py`

 * *Files identical despite different names*

### Comparing `cfdm-1.9.0.3/cfdm/coordinateconversion.py` & `cfdm-1.9.0.4/cfdm/coordinateconversion.py`

 * *Files identical despite different names*

### Comparing `cfdm-1.9.0.3/cfdm/coordinatereference.py` & `cfdm-1.9.0.4/cfdm/coordinatereference.py`

 * *Files identical despite different names*

### Comparing `cfdm-1.9.0.3/cfdm/core/__init__.py` & `cfdm-1.9.0.4/cfdm/core/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """"""
 
-__date__ = "2022-03-10"
+__date__ = "2022-07-18"
 __cf_version__ = "1.9"
-__version__ = "1.9.0.3"
+__version__ = "1.9.0.4"
 
 from packaging.version import Version
 import platform
 
 _requires = (
     "numpy",
     "netCDF4",
```

### Comparing `cfdm-1.9.0.3/cfdm/core/abstract/container.py` & `cfdm-1.9.0.4/cfdm/core/abstract/container.py`

 * *Files identical despite different names*

### Comparing `cfdm-1.9.0.3/cfdm/core/abstract/coordinate.py` & `cfdm-1.9.0.4/cfdm/core/abstract/coordinate.py`

 * *Files identical despite different names*

### Comparing `cfdm-1.9.0.3/cfdm/core/abstract/parameters.py` & `cfdm-1.9.0.4/cfdm/core/abstract/parameters.py`

 * *Files identical despite different names*

### Comparing `cfdm-1.9.0.3/cfdm/core/abstract/parametersdomainancillaries.py` & `cfdm-1.9.0.4/cfdm/core/abstract/parametersdomainancillaries.py`

 * *Files identical despite different names*

### Comparing `cfdm-1.9.0.3/cfdm/core/abstract/properties.py` & `cfdm-1.9.0.4/cfdm/core/abstract/properties.py`

 * *Files identical despite different names*

### Comparing `cfdm-1.9.0.3/cfdm/core/abstract/propertiesdata.py` & `cfdm-1.9.0.4/cfdm/core/abstract/propertiesdata.py`

 * *Files identical despite different names*

### Comparing `cfdm-1.9.0.3/cfdm/core/abstract/propertiesdatabounds.py` & `cfdm-1.9.0.4/cfdm/core/abstract/propertiesdatabounds.py`

 * *Files identical despite different names*

### Comparing `cfdm-1.9.0.3/cfdm/core/auxiliarycoordinate.py` & `cfdm-1.9.0.4/cfdm/core/auxiliarycoordinate.py`

 * *Files identical despite different names*

### Comparing `cfdm-1.9.0.3/cfdm/core/bounds.py` & `cfdm-1.9.0.4/cfdm/core/bounds.py`

 * *Files identical despite different names*

### Comparing `cfdm-1.9.0.3/cfdm/core/cellmeasure.py` & `cfdm-1.9.0.4/cfdm/core/cellmeasure.py`

 * *Files identical despite different names*

### Comparing `cfdm-1.9.0.3/cfdm/core/cellmethod.py` & `cfdm-1.9.0.4/cfdm/core/cellmethod.py`

 * *Files identical despite different names*

### Comparing `cfdm-1.9.0.3/cfdm/core/constructs.py` & `cfdm-1.9.0.4/cfdm/core/constructs.py`

 * *Files identical despite different names*

### Comparing `cfdm-1.9.0.3/cfdm/core/coordinateconversion.py` & `cfdm-1.9.0.4/cfdm/core/coordinateconversion.py`

 * *Files identical despite different names*

### Comparing `cfdm-1.9.0.3/cfdm/core/coordinatereference.py` & `cfdm-1.9.0.4/cfdm/core/coordinatereference.py`

 * *Files identical despite different names*

### Comparing `cfdm-1.9.0.3/cfdm/core/data/abstract/array.py` & `cfdm-1.9.0.4/cfdm/core/data/abstract/array.py`

 * *Files identical despite different names*

### Comparing `cfdm-1.9.0.3/cfdm/core/data/data.py` & `cfdm-1.9.0.4/cfdm/core/data/data.py`

 * *Files identical despite different names*

### Comparing `cfdm-1.9.0.3/cfdm/core/data/numpyarray.py` & `cfdm-1.9.0.4/cfdm/core/data/numpyarray.py`

 * *Files identical despite different names*

### Comparing `cfdm-1.9.0.3/cfdm/core/datum.py` & `cfdm-1.9.0.4/cfdm/core/datum.py`

 * *Files identical despite different names*

### Comparing `cfdm-1.9.0.3/cfdm/core/dimensioncoordinate.py` & `cfdm-1.9.0.4/cfdm/core/dimensioncoordinate.py`

 * *Files identical despite different names*

### Comparing `cfdm-1.9.0.3/cfdm/core/docstring/docstring.py` & `cfdm-1.9.0.4/cfdm/core/docstring/docstring.py`

 * *Files identical despite different names*

### Comparing `cfdm-1.9.0.3/cfdm/core/domain.py` & `cfdm-1.9.0.4/cfdm/core/domain.py`

 * *Files identical despite different names*

### Comparing `cfdm-1.9.0.3/cfdm/core/domainancillary.py` & `cfdm-1.9.0.4/cfdm/core/domainancillary.py`

 * *Files identical despite different names*

### Comparing `cfdm-1.9.0.3/cfdm/core/domainaxis.py` & `cfdm-1.9.0.4/cfdm/core/domainaxis.py`

 * *Files identical despite different names*

### Comparing `cfdm-1.9.0.3/cfdm/core/field.py` & `cfdm-1.9.0.4/cfdm/core/field.py`

 * *Files identical despite different names*

### Comparing `cfdm-1.9.0.3/cfdm/core/fieldancillary.py` & `cfdm-1.9.0.4/cfdm/core/fieldancillary.py`

 * *Files identical despite different names*

### Comparing `cfdm-1.9.0.3/cfdm/core/functions.py` & `cfdm-1.9.0.4/cfdm/core/functions.py`

 * *Files identical despite different names*

### Comparing `cfdm-1.9.0.3/cfdm/core/interiorring.py` & `cfdm-1.9.0.4/cfdm/core/interiorring.py`

 * *Files identical despite different names*

### Comparing `cfdm-1.9.0.3/cfdm/core/meta/docstringrewrite.py` & `cfdm-1.9.0.4/cfdm/core/meta/docstringrewrite.py`

 * *Files 0% similar despite different names*

```diff
@@ -193,18 +193,18 @@
                 docstring_rewrite,
             )
 
             # Redecorate
             if is_classmethod:
                 attrs[attr_name] = classmethod(attr)
 
-            if is_staticmethod:
+            elif is_staticmethod:
                 attrs[attr_name] = staticmethod(attr)
 
-            if is_wrapped:
+            elif is_wrapped:
                 wrapper.__doc__ = attr.__doc__
                 wrapper.__wrapped__ = attr
                 attrs[attr_name] = wrapper
 
         # ------------------------------------------------------------
         # Now loop round the parent classes, copying any methods that
         # they override and rewriting those docstrings.
```

### Comparing `cfdm-1.9.0.3/cfdm/core/mixin/fielddomain.py` & `cfdm-1.9.0.4/cfdm/core/mixin/fielddomain.py`

 * *Files identical despite different names*

### Comparing `cfdm-1.9.0.3/cfdm/count.py` & `cfdm-1.9.0.4/cfdm/count.py`

 * *Files identical despite different names*

### Comparing `cfdm-1.9.0.3/cfdm/data/abstract/compressedarray.py` & `cfdm-1.9.0.4/cfdm/data/abstract/compressedarray.py`

 * *Files identical despite different names*

### Comparing `cfdm-1.9.0.3/cfdm/data/data.py` & `cfdm-1.9.0.4/cfdm/data/data.py`

 * *Files identical despite different names*

### Comparing `cfdm-1.9.0.3/cfdm/data/gatheredarray.py` & `cfdm-1.9.0.4/cfdm/data/gatheredarray.py`

 * *Files identical despite different names*

### Comparing `cfdm-1.9.0.3/cfdm/data/mixin/arraymixin.py` & `cfdm-1.9.0.4/cfdm/data/mixin/arraymixin.py`

 * *Files identical despite different names*

### Comparing `cfdm-1.9.0.3/cfdm/data/mixin/raggedcontiguous.py` & `cfdm-1.9.0.4/cfdm/data/mixin/raggedcontiguous.py`

 * *Files identical despite different names*

### Comparing `cfdm-1.9.0.3/cfdm/data/mixin/raggedindexed.py` & `cfdm-1.9.0.4/cfdm/data/mixin/raggedindexed.py`

 * *Files identical despite different names*

### Comparing `cfdm-1.9.0.3/cfdm/data/netcdfarray.py` & `cfdm-1.9.0.4/cfdm/data/netcdfarray.py`

 * *Files identical despite different names*

### Comparing `cfdm-1.9.0.3/cfdm/data/numpyarray.py` & `cfdm-1.9.0.4/cfdm/data/numpyarray.py`

 * *Files identical despite different names*

### Comparing `cfdm-1.9.0.3/cfdm/data/raggedcontiguousarray.py` & `cfdm-1.9.0.4/cfdm/data/raggedcontiguousarray.py`

 * *Files identical despite different names*

### Comparing `cfdm-1.9.0.3/cfdm/data/raggedindexedarray.py` & `cfdm-1.9.0.4/cfdm/data/raggedindexedarray.py`

 * *Files identical despite different names*

### Comparing `cfdm-1.9.0.3/cfdm/data/raggedindexedcontiguousarray.py` & `cfdm-1.9.0.4/cfdm/data/raggedindexedcontiguousarray.py`

 * *Files identical despite different names*

### Comparing `cfdm-1.9.0.3/cfdm/datum.py` & `cfdm-1.9.0.4/cfdm/datum.py`

 * *Files identical despite different names*

### Comparing `cfdm-1.9.0.3/cfdm/decorators.py` & `cfdm-1.9.0.4/cfdm/decorators.py`

 * *Files identical despite different names*

### Comparing `cfdm-1.9.0.3/cfdm/dimensioncoordinate.py` & `cfdm-1.9.0.4/cfdm/dimensioncoordinate.py`

 * *Files identical despite different names*

### Comparing `cfdm-1.9.0.3/cfdm/docstring/docstring.py` & `cfdm-1.9.0.4/cfdm/docstring/docstring.py`

 * *Files identical despite different names*

### Comparing `cfdm-1.9.0.3/cfdm/domain.py` & `cfdm-1.9.0.4/cfdm/domain.py`

 * *Files identical despite different names*

### Comparing `cfdm-1.9.0.3/cfdm/domainancillary.py` & `cfdm-1.9.0.4/cfdm/domainancillary.py`

 * *Files identical despite different names*

### Comparing `cfdm-1.9.0.3/cfdm/domainaxis.py` & `cfdm-1.9.0.4/cfdm/domainaxis.py`

 * *Files identical despite different names*

### Comparing `cfdm-1.9.0.3/cfdm/examplefield.py` & `cfdm-1.9.0.4/cfdm/examplefield.py`

 * *Files identical despite different names*

### Comparing `cfdm-1.9.0.3/cfdm/field.py` & `cfdm-1.9.0.4/cfdm/field.py`

 * *Files identical despite different names*

### Comparing `cfdm-1.9.0.3/cfdm/fieldancillary.py` & `cfdm-1.9.0.4/cfdm/fieldancillary.py`

 * *Files identical despite different names*

### Comparing `cfdm-1.9.0.3/cfdm/functions.py` & `cfdm-1.9.0.4/cfdm/functions.py`

 * *Files identical despite different names*

### Comparing `cfdm-1.9.0.3/cfdm/index.py` & `cfdm-1.9.0.4/cfdm/index.py`

 * *Files identical despite different names*

### Comparing `cfdm-1.9.0.3/cfdm/interiorring.py` & `cfdm-1.9.0.4/cfdm/interiorring.py`

 * *Files identical despite different names*

### Comparing `cfdm-1.9.0.3/cfdm/list.py` & `cfdm-1.9.0.4/cfdm/list.py`

 * *Files identical despite different names*

### Comparing `cfdm-1.9.0.3/cfdm/mixin/__init__.py` & `cfdm-1.9.0.4/cfdm/mixin/__init__.py`

 * *Files identical despite different names*

### Comparing `cfdm-1.9.0.3/cfdm/mixin/container.py` & `cfdm-1.9.0.4/cfdm/mixin/container.py`

 * *Files identical despite different names*

### Comparing `cfdm-1.9.0.3/cfdm/mixin/coordinate.py` & `cfdm-1.9.0.4/cfdm/mixin/coordinate.py`

 * *Files identical despite different names*

### Comparing `cfdm-1.9.0.3/cfdm/mixin/fielddomain.py` & `cfdm-1.9.0.4/cfdm/mixin/fielddomain.py`

 * *Files identical despite different names*

### Comparing `cfdm-1.9.0.3/cfdm/mixin/netcdf.py` & `cfdm-1.9.0.4/cfdm/mixin/netcdf.py`

 * *Files identical despite different names*

### Comparing `cfdm-1.9.0.3/cfdm/mixin/parameters.py` & `cfdm-1.9.0.4/cfdm/mixin/parameters.py`

 * *Files identical despite different names*

### Comparing `cfdm-1.9.0.3/cfdm/mixin/parametersdomainancillaries.py` & `cfdm-1.9.0.4/cfdm/mixin/parametersdomainancillaries.py`

 * *Files identical despite different names*

### Comparing `cfdm-1.9.0.3/cfdm/mixin/properties.py` & `cfdm-1.9.0.4/cfdm/mixin/properties.py`

 * *Files identical despite different names*

### Comparing `cfdm-1.9.0.3/cfdm/mixin/propertiesdata.py` & `cfdm-1.9.0.4/cfdm/mixin/propertiesdata.py`

 * *Files identical despite different names*

### Comparing `cfdm-1.9.0.3/cfdm/mixin/propertiesdatabounds.py` & `cfdm-1.9.0.4/cfdm/mixin/propertiesdatabounds.py`

 * *Files identical despite different names*

### Comparing `cfdm-1.9.0.3/cfdm/nodecountproperties.py` & `cfdm-1.9.0.4/cfdm/nodecountproperties.py`

 * *Files identical despite different names*

### Comparing `cfdm-1.9.0.3/cfdm/partnodecountproperties.py` & `cfdm-1.9.0.4/cfdm/partnodecountproperties.py`

 * *Files identical despite different names*

### Comparing `cfdm-1.9.0.3/cfdm/read_write/abstract/abstractio.py` & `cfdm-1.9.0.4/cfdm/read_write/abstract/abstractio.py`

 * *Files identical despite different names*

### Comparing `cfdm-1.9.0.3/cfdm/read_write/netcdf/constants.py` & `cfdm-1.9.0.4/cfdm/read_write/netcdf/constants.py`

 * *Files identical despite different names*

### Comparing `cfdm-1.9.0.3/cfdm/read_write/netcdf/netcdfread.py` & `cfdm-1.9.0.4/cfdm/read_write/netcdf/netcdfread.py`

 * *Files 0% similar despite different names*

```diff
@@ -520,18 +520,19 @@
         except UnicodeDecodeError:
             pass
         except Exception:
             pass
         else:
             try:
                 line = fh.readline()
-
                 # Match comment and blank lines at the top of the file
                 while re.match(r"^\s*//|^\s*$", line):
                     line = fh.readline()
+                    if not line:
+                        break
 
                 if line.startswith("netcdf "):
                     cdl = True
             except UnicodeDecodeError:
                 pass
 
         try:
```

### Comparing `cfdm-1.9.0.3/cfdm/read_write/netcdf/netcdfwrite.py` & `cfdm-1.9.0.4/cfdm/read_write/netcdf/netcdfwrite.py`

 * *Files 0% similar despite different names*

```diff
@@ -2652,15 +2652,17 @@
             "endian": g["endian"],
             "chunksizes": chunksizes,
             "least_significant_digit": lsd,
         }
         if fill_value is not None:
             kwargs["fill_value"] = fill_value
 
-        kwargs.update(g["netcdf_compression"])
+        # Add compression parameters (but not for vlen strings).
+        if kwargs["datatype"] != str:
+            kwargs.update(g["netcdf_compression"])
 
         # Note: this is a trivial assignment in standalone cfdm, but required
         # for non-trivial customisation applied by subclasses e.g. in cf-python
         kwargs = self._customize_createVariable(cfvar, kwargs)
 
         logger.info(
             f"        to netCDF variable: {ncvar}({', '.join(ncdimensions)})"
```

### Comparing `cfdm-1.9.0.3/cfdm/read_write/read.py` & `cfdm-1.9.0.4/cfdm/read_write/read.py`

 * *Files identical despite different names*

### Comparing `cfdm-1.9.0.3/cfdm/read_write/write.py` & `cfdm-1.9.0.4/cfdm/read_write/write.py`

 * *Files identical despite different names*

### Comparing `cfdm-1.9.0.3/cfdm/test/create_test_files.py` & `cfdm-1.9.0.4/cfdm/test/create_test_files.py`

 * *Files identical despite different names*

### Comparing `cfdm-1.9.0.3/cfdm/test/run_tests.py` & `cfdm-1.9.0.4/cfdm/test/run_tests.py`

 * *Files identical despite different names*

### Comparing `cfdm-1.9.0.3/cfdm/test/setup_create_field.py` & `cfdm-1.9.0.4/cfdm/test/setup_create_field.py`

 * *Files identical despite different names*

### Comparing `cfdm-1.9.0.3/cfdm/test/setup_create_field_2.py` & `cfdm-1.9.0.4/cfdm/test/setup_create_field_2.py`

 * *Files identical despite different names*

### Comparing `cfdm-1.9.0.3/cfdm/test/setup_create_field_3.py` & `cfdm-1.9.0.4/cfdm/test/setup_create_field_3.py`

 * *Files identical despite different names*

### Comparing `cfdm-1.9.0.3/cfdm/test/test_AuxiliaryCoordinate.py` & `cfdm-1.9.0.4/cfdm/test/test_AuxiliaryCoordinate.py`

 * *Files identical despite different names*

### Comparing `cfdm-1.9.0.3/cfdm/test/test_CFDMImplementation.py` & `cfdm-1.9.0.4/cfdm/test/test_CFDMImplementation.py`

 * *Files identical despite different names*

### Comparing `cfdm-1.9.0.3/cfdm/test/test_CellMeasure.py` & `cfdm-1.9.0.4/cfdm/test/test_CellMeasure.py`

 * *Files identical despite different names*

### Comparing `cfdm-1.9.0.3/cfdm/test/test_CellMethod.py` & `cfdm-1.9.0.4/cfdm/test/test_CellMethod.py`

 * *Files identical despite different names*

### Comparing `cfdm-1.9.0.3/cfdm/test/test_Constructs.py` & `cfdm-1.9.0.4/cfdm/test/test_Constructs.py`

 * *Files identical despite different names*

### Comparing `cfdm-1.9.0.3/cfdm/test/test_CoordinateReference.py` & `cfdm-1.9.0.4/cfdm/test/test_CoordinateReference.py`

 * *Files identical despite different names*

### Comparing `cfdm-1.9.0.3/cfdm/test/test_Count.py` & `cfdm-1.9.0.4/cfdm/test/test_Count.py`

 * *Files identical despite different names*

### Comparing `cfdm-1.9.0.3/cfdm/test/test_Data.py` & `cfdm-1.9.0.4/cfdm/test/test_Data.py`

 * *Files identical despite different names*

### Comparing `cfdm-1.9.0.3/cfdm/test/test_DimensionCoordinate.py` & `cfdm-1.9.0.4/cfdm/test/test_DimensionCoordinate.py`

 * *Files identical despite different names*

### Comparing `cfdm-1.9.0.3/cfdm/test/test_Domain.py` & `cfdm-1.9.0.4/cfdm/test/test_Domain.py`

 * *Files identical despite different names*

### Comparing `cfdm-1.9.0.3/cfdm/test/test_DomainAncillary.py` & `cfdm-1.9.0.4/cfdm/test/test_DomainAncillary.py`

 * *Files identical despite different names*

### Comparing `cfdm-1.9.0.3/cfdm/test/test_DomainAxis.py` & `cfdm-1.9.0.4/cfdm/test/test_DomainAxis.py`

 * *Files identical despite different names*

### Comparing `cfdm-1.9.0.3/cfdm/test/test_Field.py` & `cfdm-1.9.0.4/cfdm/test/test_Field.py`

 * *Files identical despite different names*

### Comparing `cfdm-1.9.0.3/cfdm/test/test_FieldAncillary.py` & `cfdm-1.9.0.4/cfdm/test/test_FieldAncillary.py`

 * *Files identical despite different names*

### Comparing `cfdm-1.9.0.3/cfdm/test/test_Index.py` & `cfdm-1.9.0.4/cfdm/test/test_Index.py`

 * *Files identical despite different names*

### Comparing `cfdm-1.9.0.3/cfdm/test/test_InteriorRing.py` & `cfdm-1.9.0.4/cfdm/test/test_InteriorRing.py`

 * *Files identical despite different names*

### Comparing `cfdm-1.9.0.3/cfdm/test/test_List.py` & `cfdm-1.9.0.4/cfdm/test/test_List.py`

 * *Files identical despite different names*

### Comparing `cfdm-1.9.0.3/cfdm/test/test_NodeCountProperties.py` & `cfdm-1.9.0.4/cfdm/test/test_NodeCountProperties.py`

 * *Files identical despite different names*

### Comparing `cfdm-1.9.0.3/cfdm/test/test_NumpyArray.py` & `cfdm-1.9.0.4/cfdm/test/test_NumpyArray.py`

 * *Files identical despite different names*

### Comparing `cfdm-1.9.0.3/cfdm/test/test_PartNodeCountProperties.py` & `cfdm-1.9.0.4/cfdm/test/test_PartNodeCountProperties.py`

 * *Files identical despite different names*

### Comparing `cfdm-1.9.0.3/cfdm/test/test_RaggedContiguousArray.py` & `cfdm-1.9.0.4/cfdm/test/test_RaggedContiguousArray.py`

 * *Files identical despite different names*

### Comparing `cfdm-1.9.0.3/cfdm/test/test_RaggedIndexedArray.py` & `cfdm-1.9.0.4/cfdm/test/test_RaggedIndexedArray.py`

 * *Files identical despite different names*

### Comparing `cfdm-1.9.0.3/cfdm/test/test_RaggedIndexedContiguousArray.py` & `cfdm-1.9.0.4/cfdm/test/test_RaggedIndexedContiguousArray.py`

 * *Files identical despite different names*

### Comparing `cfdm-1.9.0.3/cfdm/test/test_core_1.py` & `cfdm-1.9.0.4/cfdm/test/test_core_1.py`

 * *Files identical despite different names*

### Comparing `cfdm-1.9.0.3/cfdm/test/test_core_2.py` & `cfdm-1.9.0.4/cfdm/test/test_core_2.py`

 * *Files identical despite different names*

### Comparing `cfdm-1.9.0.3/cfdm/test/test_decorators.py` & `cfdm-1.9.0.4/cfdm/test/test_decorators.py`

 * *Files 2% similar despite different names*

```diff
@@ -194,35 +194,35 @@
                         self.assertNotIn(msg, catch.output)
 
             # Cases where verbose is set; value should override log_level...
 
             # Highest verbosity case (note -1 == 'DEBUG', highest verbosity):
             # all messages should appear, regardless of global log_level:
             for argument in (-1, "DEBUG", "debug", "Debug", "DeBuG"):
-                with self.assertLogs(level=cfdm.log_level().value) as catch:
+                with self.assertLogs(level=-1) as catch:
                     function_to_call_to_test(verbose=argument)
                     for msg in log_message:
                         self.assertIn(msg, catch.output)
 
             # Lowest verbosity case ('WARNING' / 1) excluding special case of
             # 'DISABLE' (see note above): only warning messages should appear,
             # regardless of global log_level value set:
             for argument in (1, "WARNING", "warning", "Warning", "WaRning"):
-                with self.assertLogs(level=cfdm.log_level().value) as catch:
+                with self.assertLogs(level=1) as catch:
                     function_to_call_to_test(verbose=argument)
                     for msg in log_message:
                         if msg.split(":")[0] == "WARNING":
                             self.assertIn(msg, catch.output)
                         else:
                             self.assertNotIn(msg, catch.output)
 
             # Boolean cases for testing backwards compatibility...
 
             # ... verbose=True should be equivalent to verbose=3 now:
-            with self.assertLogs(level=cfdm.log_level().value) as catch:
+            with self.assertLogs(level=3) as catch:
                 function_to_call_to_test(verbose=True)
                 for msg in log_message:
                     if msg.split(":")[0] == "DEBUG":
                         self.assertNotIn(msg, catch.output)
                     else:
                         self.assertIn(msg, catch.output)
```

### Comparing `cfdm-1.9.0.3/cfdm/test/test_docstring.py` & `cfdm-1.9.0.4/cfdm/test/test_docstring.py`

 * *Files identical despite different names*

### Comparing `cfdm-1.9.0.3/cfdm/test/test_dsg.py` & `cfdm-1.9.0.4/cfdm/test/test_dsg.py`

 * *Files identical despite different names*

### Comparing `cfdm-1.9.0.3/cfdm/test/test_external.py` & `cfdm-1.9.0.4/cfdm/test/test_external.py`

 * *Files identical despite different names*

### Comparing `cfdm-1.9.0.3/cfdm/test/test_functions.py` & `cfdm-1.9.0.4/cfdm/test/test_functions.py`

 * *Files identical despite different names*

### Comparing `cfdm-1.9.0.3/cfdm/test/test_gathering.py` & `cfdm-1.9.0.4/cfdm/test/test_gathering.py`

 * *Files identical despite different names*

### Comparing `cfdm-1.9.0.3/cfdm/test/test_geometry.py` & `cfdm-1.9.0.4/cfdm/test/test_geometry.py`

 * *Files identical despite different names*

### Comparing `cfdm-1.9.0.3/cfdm/test/test_groups.py` & `cfdm-1.9.0.4/cfdm/test/test_groups.py`

 * *Files identical despite different names*

### Comparing `cfdm-1.9.0.3/cfdm/test/test_netCDF.py` & `cfdm-1.9.0.4/cfdm/test/test_netCDF.py`

 * *Files identical despite different names*

### Comparing `cfdm-1.9.0.3/cfdm/test/test_read_write.py` & `cfdm-1.9.0.4/cfdm/test/test_read_write.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,25 +17,25 @@
 
 # Set up temporary files
 n_tmpfiles = 9
 tmpfiles = [
     tempfile.mkstemp("_test_read_write.nc", dir=os.getcwd())[1]
     for i in range(n_tmpfiles)
 ]
-(
+[
     tmpfile,
     tmpfileh,
     tmpfileh2,
     tmpfileh3,
     tmpfilec,
     tmpfilec2,
     tmpfilec3,
     tmpfile0,
     tmpfile1,
-) = tmpfiles
+] = tmpfiles
 
 
 def _remove_tmpfiles():
     """Remove temporary files created during tests."""
     for f in tmpfiles:
         try:
             os.remove(f)
@@ -852,13 +852,23 @@
 
     def test_write_filename_expansion(self):
         """Test the writing to a file name that requires expansions."""
         f = cfdm.example_field(0)
         filename = os.path.join("$PWD", os.path.basename(tmpfile))
         cfdm.write(f, filename)
 
+    def test_read_zero_length_file(self):
+        """Test reading a zero length file raises an exception."""
+        # Create zero-length file
+        tmpfile = tempfile.mkstemp("_test_read_write.nc", dir=os.getcwd())[1]
+        tmpfiles.append(tmpfile)
+        subprocess.run(f"touch {tmpfile}", shell=True, check=True)
+
+        with self.assertRaises(OSError):
+            cfdm.read(tmpfile)
+
 
 if __name__ == "__main__":
     print("Run date:", datetime.datetime.now())
     cfdm.environment()
     print("")
     unittest.main(verbosity=2)
```

### Comparing `cfdm-1.9.0.3/cfdm/test/test_string.py` & `cfdm-1.9.0.4/cfdm/test/test_string.py`

 * *Files identical despite different names*

### Comparing `cfdm-1.9.0.3/cfdm/test/test_style.py` & `cfdm-1.9.0.4/cfdm/test/test_style.py`

 * *Files identical despite different names*

### Comparing `cfdm-1.9.0.3/cfdm.egg-info/PKG-INFO` & `cfdm-1.9.0.4/cfdm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cfdm
-Version: 1.9.0.3
+Version: 1.9.0.4
 Summary: A Python reference implementation of the CF data model
 Home-page: https://ncas-cms.github.io/cfdm
 Author: David Hassell, Sadie Bartholomew
 Author-email: david.hassell@ncas.ac.uk
 Maintainer: David Hassell, Sadie Bartholomew
 License: MIT
 Download-URL: https://pypi.org/project/cfdm/#files
```

### Comparing `cfdm-1.9.0.3/cfdm.egg-info/SOURCES.txt` & `cfdm-1.9.0.4/cfdm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cfdm-1.9.0.3/pyproject.toml` & `cfdm-1.9.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cfdm-1.9.0.3/scripts/cfdump` & `cfdm-1.9.0.4/scripts/cfdump`

 * *Files identical despite different names*

### Comparing `cfdm-1.9.0.3/setup.py` & `cfdm-1.9.0.4/setup.py`

 * *Files identical despite different names*

