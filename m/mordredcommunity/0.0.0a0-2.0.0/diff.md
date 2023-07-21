# Comparing `tmp/mordredcommunity-0.0.0a0.tar.gz` & `tmp/mordredcommunity-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mordredcommunity-0.0.0a0.tar", last modified: Thu Jul 20 15:25:03 2023, max compression
+gzip compressed data, was "mordredcommunity-2.0.0.tar", last modified: Fri Jul 21 16:38:58 2023, max compression
```

## Comparing `mordredcommunity-0.0.0a0.tar` & `mordredcommunity-2.0.0.tar`

### file list

```diff
@@ -1,109 +1,107 @@
-drwxr-xr-x   0 jackson    (501) staff       (20)        0 2023-07-20 15:25:03.184342 mordredcommunity-0.0.0a0/
--rw-r--r--   0 jackson    (501) staff       (20)     1493 2023-07-20 15:08:13.000000 mordredcommunity-0.0.0a0/LICENSE
--rw-r--r--   0 jackson    (501) staff       (20)      607 2023-07-20 15:25:03.183808 mordredcommunity-0.0.0a0/PKG-INFO
--rw-r--r--   0 jackson    (501) staff       (20)     6902 2023-07-20 15:08:13.000000 mordredcommunity-0.0.0a0/README.rst
-drwxr-xr-x   0 jackson    (501) staff       (20)        0 2023-07-20 15:25:03.081404 mordredcommunity-0.0.0a0/mordred/
--rw-r--r--   0 jackson    (501) staff       (20)     1988 2023-07-20 15:08:13.000000 mordredcommunity-0.0.0a0/mordred/ABCIndex.py
--rw-r--r--   0 jackson    (501) staff       (20)     1810 2023-07-20 15:08:13.000000 mordredcommunity-0.0.0a0/mordred/AcidBase.py
--rw-r--r--   0 jackson    (501) staff       (20)     1272 2023-07-20 15:08:13.000000 mordredcommunity-0.0.0a0/mordred/AdjacencyMatrix.py
--rw-r--r--   0 jackson    (501) staff       (20)      947 2023-07-20 15:08:13.000000 mordredcommunity-0.0.0a0/mordred/Aromatic.py
--rw-r--r--   0 jackson    (501) staff       (20)     2939 2023-07-20 15:08:13.000000 mordredcommunity-0.0.0a0/mordred/AtomCount.py
--rw-r--r--   0 jackson    (501) staff       (20)     7796 2023-07-20 15:08:13.000000 mordredcommunity-0.0.0a0/mordred/Autocorrelation.py
--rw-r--r--   0 jackson    (501) staff       (20)     3003 2023-07-20 15:08:13.000000 mordredcommunity-0.0.0a0/mordred/BCUT.py
--rw-r--r--   0 jackson    (501) staff       (20)      733 2023-07-20 15:08:13.000000 mordredcommunity-0.0.0a0/mordred/BalabanJ.py
--rw-r--r--   0 jackson    (501) staff       (20)     2410 2023-07-20 15:08:13.000000 mordredcommunity-0.0.0a0/mordred/BaryszMatrix.py
--rw-r--r--   0 jackson    (501) staff       (20)      711 2023-07-20 15:08:13.000000 mordredcommunity-0.0.0a0/mordred/BertzCT.py
--rw-r--r--   0 jackson    (501) staff       (20)     2711 2023-07-20 15:08:13.000000 mordredcommunity-0.0.0a0/mordred/BondCount.py
--rw-r--r--   0 jackson    (501) staff       (20)     9304 2023-07-20 15:08:13.000000 mordredcommunity-0.0.0a0/mordred/CPSA.py
--rw-r--r--   0 jackson    (501) staff       (20)     3502 2023-07-20 15:08:13.000000 mordredcommunity-0.0.0a0/mordred/CarbonTypes.py
--rw-r--r--   0 jackson    (501) staff       (20)     6216 2023-07-20 15:08:13.000000 mordredcommunity-0.0.0a0/mordred/Chi.py
--rw-r--r--   0 jackson    (501) staff       (20)     1882 2023-07-20 15:08:13.000000 mordredcommunity-0.0.0a0/mordred/Constitutional.py
--rw-r--r--   0 jackson    (501) staff       (20)     5891 2023-07-20 15:08:13.000000 mordredcommunity-0.0.0a0/mordred/DetourMatrix.py
--rw-r--r--   0 jackson    (501) staff       (20)     1262 2023-07-20 15:08:13.000000 mordredcommunity-0.0.0a0/mordred/DistanceMatrix.py
--rw-r--r--   0 jackson    (501) staff       (20)     3679 2023-07-20 15:08:13.000000 mordredcommunity-0.0.0a0/mordred/EState.py
--rw-r--r--   0 jackson    (501) staff       (20)      957 2023-07-20 15:08:13.000000 mordredcommunity-0.0.0a0/mordred/EccentricConnectivityIndex.py
--rw-r--r--   0 jackson    (501) staff       (20)    20747 2023-07-20 15:08:13.000000 mordredcommunity-0.0.0a0/mordred/ExtendedTopochemicalAtom.py
--rw-r--r--   0 jackson    (501) staff       (20)      978 2023-07-20 15:08:13.000000 mordredcommunity-0.0.0a0/mordred/FragmentComplexity.py
--rw-r--r--   0 jackson    (501) staff       (20)     1873 2023-07-20 15:08:13.000000 mordredcommunity-0.0.0a0/mordred/Framework.py
--rw-r--r--   0 jackson    (501) staff       (20)     2504 2023-07-20 15:08:13.000000 mordredcommunity-0.0.0a0/mordred/GeometricalIndex.py
--rw-r--r--   0 jackson    (501) staff       (20)     1459 2023-07-20 15:08:13.000000 mordredcommunity-0.0.0a0/mordred/GravitationalIndex.py
--rw-r--r--   0 jackson    (501) staff       (20)     1041 2023-07-20 15:08:13.000000 mordredcommunity-0.0.0a0/mordred/HydrogenBond.py
--rw-r--r--   0 jackson    (501) staff       (20)     7358 2023-07-20 15:08:13.000000 mordredcommunity-0.0.0a0/mordred/InformationContent.py
--rw-r--r--   0 jackson    (501) staff       (20)     2177 2023-07-20 15:08:13.000000 mordredcommunity-0.0.0a0/mordred/KappaShapeIndex.py
--rw-r--r--   0 jackson    (501) staff       (20)     1448 2023-07-20 15:08:13.000000 mordredcommunity-0.0.0a0/mordred/Lipinski.py
--rw-r--r--   0 jackson    (501) staff       (20)     1540 2023-07-20 15:08:13.000000 mordredcommunity-0.0.0a0/mordred/LogS.py
--rw-r--r--   0 jackson    (501) staff       (20)      667 2023-07-20 15:08:13.000000 mordredcommunity-0.0.0a0/mordred/McGowanVolume.py
--rw-r--r--   0 jackson    (501) staff       (20)     2214 2023-07-20 15:08:13.000000 mordredcommunity-0.0.0a0/mordred/MoRSE.py
--rw-r--r--   0 jackson    (501) staff       (20)     2718 2023-07-20 15:08:13.000000 mordredcommunity-0.0.0a0/mordred/MoeType.py
--rw-r--r--   0 jackson    (501) staff       (20)     2736 2023-07-20 15:08:13.000000 mordredcommunity-0.0.0a0/mordred/MolecularDistanceEdge.py
--rw-r--r--   0 jackson    (501) staff       (20)     4271 2023-07-20 15:08:13.000000 mordredcommunity-0.0.0a0/mordred/MolecularId.py
--rw-r--r--   0 jackson    (501) staff       (20)     1655 2023-07-20 15:08:13.000000 mordredcommunity-0.0.0a0/mordred/MomentOfInertia.py
--rw-r--r--   0 jackson    (501) staff       (20)      543 2023-07-20 15:08:13.000000 mordredcommunity-0.0.0a0/mordred/PBF.py
--rw-r--r--   0 jackson    (501) staff       (20)     4030 2023-07-20 15:08:13.000000 mordredcommunity-0.0.0a0/mordred/PathCount.py
--rw-r--r--   0 jackson    (501) staff       (20)     1565 2023-07-20 15:08:13.000000 mordredcommunity-0.0.0a0/mordred/Polarizability.py
--rw-r--r--   0 jackson    (501) staff       (20)     4512 2023-07-20 15:08:13.000000 mordredcommunity-0.0.0a0/mordred/RingCount.py
--rw-r--r--   0 jackson    (501) staff       (20)     1368 2023-07-20 15:08:13.000000 mordredcommunity-0.0.0a0/mordred/RotatableBond.py
--rw-r--r--   0 jackson    (501) staff       (20)      990 2023-07-20 15:08:13.000000 mordredcommunity-0.0.0a0/mordred/SLogP.py
--rw-r--r--   0 jackson    (501) staff       (20)     3438 2023-07-20 15:08:13.000000 mordredcommunity-0.0.0a0/mordred/TopoPSA.py
--rw-r--r--   0 jackson    (501) staff       (20)     2607 2023-07-20 15:08:13.000000 mordredcommunity-0.0.0a0/mordred/TopologicalCharge.py
--rw-r--r--   0 jackson    (501) staff       (20)     2414 2023-07-20 15:08:13.000000 mordredcommunity-0.0.0a0/mordred/TopologicalIndex.py
--rw-r--r--   0 jackson    (501) staff       (20)     1602 2023-07-20 15:08:13.000000 mordredcommunity-0.0.0a0/mordred/VdwVolumeABC.py
--rw-r--r--   0 jackson    (501) staff       (20)      943 2023-07-20 15:08:13.000000 mordredcommunity-0.0.0a0/mordred/VertexAdjacencyInformation.py
--rw-r--r--   0 jackson    (501) staff       (20)     2156 2023-07-20 15:08:13.000000 mordredcommunity-0.0.0a0/mordred/WalkCount.py
--rw-r--r--   0 jackson    (501) staff       (20)     1141 2023-07-20 15:08:13.000000 mordredcommunity-0.0.0a0/mordred/Weight.py
--rw-r--r--   0 jackson    (501) staff       (20)      995 2023-07-20 15:08:13.000000 mordredcommunity-0.0.0a0/mordred/WienerIndex.py
--rw-r--r--   0 jackson    (501) staff       (20)     2111 2023-07-20 15:08:13.000000 mordredcommunity-0.0.0a0/mordred/ZagrebIndex.py
--rw-r--r--   0 jackson    (501) staff       (20)      336 2023-07-20 15:16:18.000000 mordredcommunity-0.0.0a0/mordred/__init__.py
--rw-r--r--   0 jackson    (501) staff       (20)     6320 2023-07-20 15:08:13.000000 mordredcommunity-0.0.0a0/mordred/__main__.py
--rw-r--r--   0 jackson    (501) staff       (20)     8724 2023-07-20 15:08:13.000000 mordredcommunity-0.0.0a0/mordred/_atomic_property.py
-drwxr-xr-x   0 jackson    (501) staff       (20)        0 2023-07-20 15:25:03.098379 mordredcommunity-0.0.0a0/mordred/_base/
--rw-r--r--   0 jackson    (501) staff       (20)     2261 2023-07-20 15:08:13.000000 mordredcommunity-0.0.0a0/mordred/_base/__init__.py
--rw-r--r--   0 jackson    (501) staff       (20)    12984 2023-07-20 15:08:13.000000 mordredcommunity-0.0.0a0/mordred/_base/calculator.py
--rw-r--r--   0 jackson    (501) staff       (20)     2430 2023-07-20 15:08:13.000000 mordredcommunity-0.0.0a0/mordred/_base/context.py
--rw-r--r--   0 jackson    (501) staff       (20)     9671 2023-07-20 15:08:13.000000 mordredcommunity-0.0.0a0/mordred/_base/descriptor.py
--rw-r--r--   0 jackson    (501) staff       (20)      400 2023-07-20 15:08:13.000000 mordredcommunity-0.0.0a0/mordred/_base/pandas_module.py
--rw-r--r--   0 jackson    (501) staff       (20)     2169 2023-07-20 15:08:13.000000 mordredcommunity-0.0.0a0/mordred/_base/parallel.py
--rw-r--r--   0 jackson    (501) staff       (20)     4323 2023-07-20 15:08:13.000000 mordredcommunity-0.0.0a0/mordred/_base/result.py
--rw-r--r--   0 jackson    (501) staff       (20)      435 2023-07-20 15:08:13.000000 mordredcommunity-0.0.0a0/mordred/_base/util.py
--rw-r--r--   0 jackson    (501) staff       (20)     3336 2023-07-20 15:08:13.000000 mordredcommunity-0.0.0a0/mordred/_graph_matrix.py
--rw-r--r--   0 jackson    (501) staff       (20)     6191 2023-07-20 15:08:13.000000 mordredcommunity-0.0.0a0/mordred/_matrix_attributes.py
--rw-r--r--   0 jackson    (501) staff       (20)     2230 2023-07-20 15:08:13.000000 mordredcommunity-0.0.0a0/mordred/_util.py
-drwxr-xr-x   0 jackson    (501) staff       (20)        0 2023-07-20 15:25:03.099860 mordredcommunity-0.0.0a0/mordred/descriptors/
--rw-r--r--   0 jackson    (501) staff       (20)     1044 2023-07-20 15:08:13.000000 mordredcommunity-0.0.0a0/mordred/descriptors/__init__.py
-drwxr-xr-x   0 jackson    (501) staff       (20)        0 2023-07-20 15:25:03.101175 mordredcommunity-0.0.0a0/mordred/error/
--rw-r--r--   0 jackson    (501) staff       (20)     2045 2023-07-20 15:08:13.000000 mordredcommunity-0.0.0a0/mordred/error/__init__.py
-drwxr-xr-x   0 jackson    (501) staff       (20)        0 2023-07-20 15:25:03.106903 mordredcommunity-0.0.0a0/mordred/surface_area/
--rw-r--r--   0 jackson    (501) staff       (20)      519 2023-07-20 15:08:13.000000 mordredcommunity-0.0.0a0/mordred/surface_area/__init__.py
--rw-r--r--   0 jackson    (501) staff       (20)     1422 2023-07-20 15:08:13.000000 mordredcommunity-0.0.0a0/mordred/surface_area/__main__.py
--rw-r--r--   0 jackson    (501) staff       (20)     2392 2023-07-20 15:08:13.000000 mordredcommunity-0.0.0a0/mordred/surface_area/_mesh.py
--rw-r--r--   0 jackson    (501) staff       (20)     3433 2023-07-20 15:08:13.000000 mordredcommunity-0.0.0a0/mordred/surface_area/_sasa.py
-drwxr-xr-x   0 jackson    (501) staff       (20)        0 2023-07-20 15:25:03.149508 mordredcommunity-0.0.0a0/mordred/tests/
--rw-r--r--   0 jackson    (501) staff       (20)      633 2023-07-20 15:08:13.000000 mordredcommunity-0.0.0a0/mordred/tests/Dummy.py
--rw-r--r--   0 jackson    (501) staff       (20)       28 2023-07-20 15:08:13.000000 mordredcommunity-0.0.0a0/mordred/tests/__init__.py
--rw-r--r--   0 jackson    (501) staff       (20)      421 2023-07-20 15:08:13.000000 mordredcommunity-0.0.0a0/mordred/tests/__main__.py
--rw-r--r--   0 jackson    (501) staff       (20)      587 2023-07-20 15:08:13.000000 mordredcommunity-0.0.0a0/mordred/tests/test_ABCIndex.py
--rw-r--r--   0 jackson    (501) staff       (20)     4162 2023-07-20 15:08:13.000000 mordredcommunity-0.0.0a0/mordred/tests/test_ETA.py
--rw-r--r--   0 jackson    (501) staff       (20)     1589 2023-07-20 15:08:13.000000 mordredcommunity-0.0.0a0/mordred/tests/test_SASA.py
--rw-r--r--   0 jackson    (501) staff       (20)      417 2023-07-20 15:08:13.000000 mordredcommunity-0.0.0a0/mordred/tests/test_SLogP.py
--rw-r--r--   0 jackson    (501) staff       (20)     4689 2023-07-20 15:08:13.000000 mordredcommunity-0.0.0a0/mordred/tests/test_VEA.py
--rw-r--r--   0 jackson    (501) staff       (20)     3249 2023-07-20 15:08:13.000000 mordredcommunity-0.0.0a0/mordred/tests/test_atomic_property.py
--rw-r--r--   0 jackson    (501) staff       (20)      976 2023-07-20 15:08:13.000000 mordredcommunity-0.0.0a0/mordred/tests/test_attributes.py
--rw-r--r--   0 jackson    (501) staff       (20)     1082 2023-07-20 15:08:13.000000 mordredcommunity-0.0.0a0/mordred/tests/test_base.py
--rw-r--r--   0 jackson    (501) staff       (20)     2115 2023-07-20 15:08:13.000000 mordredcommunity-0.0.0a0/mordred/tests/test_by_references.py
--rw-r--r--   0 jackson    (501) staff       (20)      646 2023-07-20 15:08:13.000000 mordredcommunity-0.0.0a0/mordred/tests/test_compose_descriptor.py
--rw-r--r--   0 jackson    (501) staff       (20)      610 2023-07-20 15:08:13.000000 mordredcommunity-0.0.0a0/mordred/tests/test_exceptions.py
--rw-r--r--   0 jackson    (501) staff       (20)      750 2023-07-20 15:08:13.000000 mordredcommunity-0.0.0a0/mordred/tests/test_import_all_descriptors.py
--rw-r--r--   0 jackson    (501) staff       (20)      266 2023-07-20 15:08:13.000000 mordredcommunity-0.0.0a0/mordred/tests/test_json.py
--rw-r--r--   0 jackson    (501) staff       (20)     4754 2023-07-20 15:08:13.000000 mordredcommunity-0.0.0a0/mordred/tests/test_mordred_main.py
--rw-r--r--   0 jackson    (501) staff       (20)      607 2023-07-20 15:08:13.000000 mordredcommunity-0.0.0a0/mordred/tests/test_pandas.py
--rw-r--r--   0 jackson    (501) staff       (20)      863 2023-07-20 15:08:13.000000 mordredcommunity-0.0.0a0/mordred/tests/test_parallel.py
--rw-r--r--   0 jackson    (501) staff       (20)     1052 2023-07-20 15:08:13.000000 mordredcommunity-0.0.0a0/mordred/tests/test_pickle.py
--rw-r--r--   0 jackson    (501) staff       (20)     2300 2023-07-20 15:08:13.000000 mordredcommunity-0.0.0a0/mordred/tests/test_result_type.py
-drwxr-xr-x   0 jackson    (501) staff       (20)        0 2023-07-20 15:25:03.181723 mordredcommunity-0.0.0a0/mordredcommunity.egg-info/
--rw-r--r--   0 jackson    (501) staff       (20)      607 2023-07-20 15:25:02.000000 mordredcommunity-0.0.0a0/mordredcommunity.egg-info/PKG-INFO
--rw-r--r--   0 jackson    (501) staff       (20)     2592 2023-07-20 15:25:02.000000 mordredcommunity-0.0.0a0/mordredcommunity.egg-info/SOURCES.txt
--rw-r--r--   0 jackson    (501) staff       (20)        1 2023-07-20 15:25:02.000000 mordredcommunity-0.0.0a0/mordredcommunity.egg-info/dependency_links.txt
--rw-r--r--   0 jackson    (501) staff       (20)       52 2023-07-20 15:25:02.000000 mordredcommunity-0.0.0a0/mordredcommunity.egg-info/requires.txt
--rw-r--r--   0 jackson    (501) staff       (20)        8 2023-07-20 15:25:02.000000 mordredcommunity-0.0.0a0/mordredcommunity.egg-info/top_level.txt
--rw-r--r--   0 jackson    (501) staff       (20)     1018 2023-07-20 15:24:48.000000 mordredcommunity-0.0.0a0/pyproject.toml
--rw-r--r--   0 jackson    (501) staff       (20)       38 2023-07-20 15:25:03.184473 mordredcommunity-0.0.0a0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:38:58.311249 mordredcommunity-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5753 2023-07-21 16:38:58.311249 mordredcommunity-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5144 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:38:58.299249 mordredcommunity-2.0.0/mordred/
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/ABCIndex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/AcidBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/AdjacencyMatrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/Aromatic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2949 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/AtomCount.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7796 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/Autocorrelation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/BCUT.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/BalabanJ.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/BaryszMatrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/BertzCT.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/BondCount.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9304 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/CPSA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/CarbonTypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6216 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/Chi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/Constitutional.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5927 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/DetourMatrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/DistanceMatrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/EState.py
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/EccentricConnectivityIndex.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20747 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/ExtendedTopochemicalAtom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/FragmentComplexity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/Framework.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/GeometricalIndex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/GravitationalIndex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/HydrogenBond.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7355 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/InformationContent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/KappaShapeIndex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/Lipinski.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/LogS.py
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/McGowanVolume.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/MoRSE.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/MoeType.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/MolecularDistanceEdge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4271 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/MolecularId.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/MomentOfInertia.py
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/PBF.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4030 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/PathCount.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/Polarizability.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4512 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/RingCount.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/RotatableBond.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/SLogP.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/TopoPSA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/TopologicalCharge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/TopologicalIndex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/VdwVolumeABC.py
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/VertexAdjacencyInformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/WalkCount.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/Weight.py
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/WienerIndex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/ZagrebIndex.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6462 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8724 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/_atomic_property.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:38:58.299249 mordredcommunity-2.0.0/mordred/_base/
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/_base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12279 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/_base/calculator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/_base/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9681 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/_base/descriptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/_base/pandas_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/_base/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4323 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/_base/result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/_base/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/_graph_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6191 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/_matrix_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:38:58.299249 mordredcommunity-2.0.0/mordred/descriptors/
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/descriptors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:38:58.303249 mordredcommunity-2.0.0/mordred/error/
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/error/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:38:58.303249 mordredcommunity-2.0.0/mordred/surface_area/
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/surface_area/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/surface_area/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/surface_area/_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3433 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/surface_area/_sasa.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:38:58.307249 mordredcommunity-2.0.0/mordred/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/tests/Dummy.py
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/tests/test_ABCIndex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4227 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/tests/test_ETA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/tests/test_SASA.py
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/tests/test_SLogP.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/tests/test_VEA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/tests/test_atomic_property.py
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/tests/test_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/tests/test_by_references.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/tests/test_compose_descriptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/tests/test_import_all_descriptors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/tests/test_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4905 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/tests/test_mordred_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/tests/test_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/tests/test_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/tests/test_pickle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/mordred/tests/test_result_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:38:58.311249 mordredcommunity-2.0.0/mordredcommunity.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5753 2023-07-21 16:38:58.000000 mordredcommunity-2.0.0/mordredcommunity.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-07-21 16:38:58.000000 mordredcommunity-2.0.0/mordredcommunity.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 16:38:58.000000 mordredcommunity-2.0.0/mordredcommunity.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-21 16:38:58.000000 mordredcommunity-2.0.0/mordredcommunity.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-21 16:38:58.000000 mordredcommunity-2.0.0/mordredcommunity.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-07-21 16:38:46.000000 mordredcommunity-2.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 16:38:58.311249 mordredcommunity-2.0.0/setup.cfg
```

### Comparing `mordredcommunity-0.0.0a0/LICENSE` & `mordredcommunity-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mordredcommunity-0.0.0a0/mordred/ABCIndex.py` & `mordredcommunity-2.0.0/mordred/ABCIndex.py`

 * *Files 10% similar despite different names*

```diff
@@ -49,15 +49,15 @@
     def _each_bond(bond):
         du = bond.GetBeginAtom().GetDegree()
         dv = bond.GetEndAtom().GetDegree()
 
         return np.sqrt((du + dv - 2.0) / (du * dv))
 
     def calculate(self):
-        return np.float(np.sum(self._each_bond(bond) for bond in self.mol.GetBonds()))
+        return float(sum(self._each_bond(bond) for bond in self.mol.GetBonds()))
 
 
 class ABCGGIndex(ABCIndexBase):
     r"""Graovac-Ghorbani atom-bond connectivity index descriptor.
 
     References:
         * Furtula, B. Atom-bond connectivity index versus Graovac-Ghorbani analog. MATCH Commun. Math. Comput. Chem 75, 233-242 (2016).
@@ -80,10 +80,8 @@
 
         nu = np.sum(D[u, :] < D[v, :])
         nv = np.sum(D[v, :] < D[u, :])
 
         return np.sqrt((nu + nv - 2.0) / (nu * nv))
 
     def calculate(self, D):
-        return np.float(
-            np.sum(self._each_bond(bond, D) for bond in self.mol.GetBonds())
-        )
+        return float(sum(self._each_bond(bond, D) for bond in self.mol.GetBonds()))
```

### Comparing `mordredcommunity-0.0.0a0/mordred/AcidBase.py` & `mordredcommunity-2.0.0/mordred/AcidBase.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-0.0.0a0/mordred/AdjacencyMatrix.py` & `mordredcommunity-2.0.0/mordred/AdjacencyMatrix.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,19 @@
-from distutils.version import StrictVersion
+from packaging.version import Version as StrictVersion
 
 from ._base import Descriptor
 from ._graph_matrix import AdjacencyMatrix as A
 from ._matrix_attributes import SM1, methods, get_method
 
 __all__ = ("AdjacencyMatrix",)
 
+try:
+    from importlib.metadata import version
+except ImportError:
+    from importlib_metadata import version
 
 _version_remove_SM1_A = StrictVersion("1.1.0")
 
 
 class AdjacencyMatrix(Descriptor):
     r"""adjacency matrix descriptor.
```

### Comparing `mordredcommunity-0.0.0a0/mordred/Aromatic.py` & `mordredcommunity-2.0.0/mordred/Aromatic.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-0.0.0a0/mordred/AtomCount.py` & `mordredcommunity-2.0.0/mordred/AtomCount.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from distutils.version import StrictVersion
+from packaging.version import Version as StrictVersion
 
 from rdkit.Chem import rdMolDescriptors
 
 from ._base import Descriptor
 from ._atomic_property import halogen
 
 __all__ = ("AtomCount",)
@@ -83,15 +83,15 @@
                 "X",
             ]
 
         return map(cls, t)
 
     @property
     def explicit_hydrogens(self):
-        u"""Require explicit_hydrogens when type is "H" or "Atom"."""
+        """Require explicit_hydrogens when type is "H" or "Atom"."""
         return self._type in {"H", "Atom"}
 
     def __str__(self):
         return "n" + self._type
 
     def parameters(self):
         return (self._type,)
```

### Comparing `mordredcommunity-0.0.0a0/mordred/Autocorrelation.py` & `mordredcommunity-2.0.0/mordred/Autocorrelation.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-0.0.0a0/mordred/BCUT.py` & `mordredcommunity-2.0.0/mordred/BCUT.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-0.0.0a0/mordred/BalabanJ.py` & `mordredcommunity-2.0.0/mordred/BalabanJ.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-0.0.0a0/mordred/BaryszMatrix.py` & `mordredcommunity-2.0.0/mordred/BaryszMatrix.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-0.0.0a0/mordred/BertzCT.py` & `mordredcommunity-2.0.0/mordred/BertzCT.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-0.0.0a0/mordred/BondCount.py` & `mordredcommunity-2.0.0/mordred/BondCount.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-0.0.0a0/mordred/CPSA.py` & `mordredcommunity-2.0.0/mordred/CPSA.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-0.0.0a0/mordred/CarbonTypes.py` & `mordredcommunity-2.0.0/mordred/CarbonTypes.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-0.0.0a0/mordred/Chi.py` & `mordredcommunity-2.0.0/mordred/Chi.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-0.0.0a0/mordred/Constitutional.py` & `mordredcommunity-2.0.0/mordred/Constitutional.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-0.0.0a0/mordred/DetourMatrix.py` & `mordredcommunity-2.0.0/mordred/DetourMatrix.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,15 +114,17 @@
         self.C = {
             (i, j): calc_weight(i, j) for i in self.nodes for j in self.nodes if i <= j
         }
 
     def __call__(self):
         timeout_at = None if self.timeout is None else time.time() + self.timeout
 
-        for bcc in networkx.biconnected_component_subgraphs(self.G, False):
+        for bcc in (
+            self.G.subgraph(c) for c in networkx.biconnected_components(self.G)
+        ):
             lsp = LongestSimplePath(bcc, self.weight, timeout_at)()
             nodes = set()
             for a, b in lsp:
                 nodes.add(a)
                 nodes.add(b)
             self.Q.append((nodes, lsp))
```

### Comparing `mordredcommunity-0.0.0a0/mordred/DistanceMatrix.py` & `mordredcommunity-2.0.0/mordred/DistanceMatrix.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from distutils.version import StrictVersion
+from packaging.version import Version as StrictVersion
 
 from ._base import Descriptor
 from ._graph_matrix import DistanceMatrix as D
 from ._matrix_attributes import SM1, methods, get_method
 
 __all__ = ("DistanceMatrix",)
```

### Comparing `mordredcommunity-0.0.0a0/mordred/EState.py` & `mordredcommunity-2.0.0/mordred/EState.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-0.0.0a0/mordred/EccentricConnectivityIndex.py` & `mordredcommunity-2.0.0/mordred/EccentricConnectivityIndex.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-0.0.0a0/mordred/ExtendedTopochemicalAtom.py` & `mordredcommunity-2.0.0/mordred/ExtendedTopochemicalAtom.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-0.0.0a0/mordred/FragmentComplexity.py` & `mordredcommunity-2.0.0/mordred/FragmentComplexity.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-0.0.0a0/mordred/Framework.py` & `mordredcommunity-2.0.0/mordred/Framework.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-0.0.0a0/mordred/GeometricalIndex.py` & `mordredcommunity-2.0.0/mordred/GeometricalIndex.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-0.0.0a0/mordred/GravitationalIndex.py` & `mordredcommunity-2.0.0/mordred/GravitationalIndex.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-0.0.0a0/mordred/HydrogenBond.py` & `mordredcommunity-2.0.0/mordred/HydrogenBond.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-0.0.0a0/mordred/InformationContent.py` & `mordredcommunity-2.0.0/mordred/InformationContent.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     def expand(self):
         self._expand(self.tree)
 
     def _expand(self, tree):
         for src, dst in list(tree.items()):
             self.visited.add(src)
 
-            if dst is ():
+            if not dst:
                 tree[src] = {
                     n.GetIdx(): ()
                     for n in self.atoms[src][2]
                     if n.GetIdx() not in self.visited
                 }
 
             else:
@@ -62,15 +62,14 @@
 
     def _code(self, tree, before, trail):
         if len(tree) == 0:
             yield trail
 
         else:
             for src, dst in tree.items():
-
                 code = []
                 if before is not None:
                     bt = self.bonds[before, src]
                     code.append(bt)
 
                 code.append(self.atoms[src][:2])
```

### Comparing `mordredcommunity-0.0.0a0/mordred/KappaShapeIndex.py` & `mordredcommunity-2.0.0/mordred/KappaShapeIndex.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-0.0.0a0/mordred/Lipinski.py` & `mordredcommunity-2.0.0/mordred/Lipinski.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-0.0.0a0/mordred/LogS.py` & `mordredcommunity-2.0.0/mordred/LogS.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-0.0.0a0/mordred/McGowanVolume.py` & `mordredcommunity-2.0.0/mordred/McGowanVolume.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-0.0.0a0/mordred/MoRSE.py` & `mordredcommunity-2.0.0/mordred/MoRSE.py`

 * *Files 4% similar despite different names*

```diff
@@ -79,10 +79,10 @@
             with self.rethrow_zerodiv():
                 sr = (self._distance - 1) * D
                 np.fill_diagonal(sr, 1)
                 n = np.sin(sr) / sr
 
         np.fill_diagonal(n, 0)
 
-        return np.float(0.5 * A.dot(n).dot(A.T))
+        return float(0.5 * np.ravel(A.dot(n).dot(A.T))[0])
 
     rtype = float
```

### Comparing `mordredcommunity-0.0.0a0/mordred/MoeType.py` & `mordredcommunity-2.0.0/mordred/MoeType.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-0.0.0a0/mordred/MolecularDistanceEdge.py` & `mordredcommunity-2.0.0/mordred/MolecularDistanceEdge.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from six import string_types, integer_types
-from numpy import product
+from numpy import prod
 
 from ._base import Descriptor
 from ._graph_matrix import Valence, DistanceMatrix
 from ._atomic_property import GetAtomicNumber, GetElementSymbol
 
 __all__ = ("MolecularDistanceEdge",)
 
@@ -81,12 +81,12 @@
             if self.mol.GetAtomWithIdx(i).GetAtomicNum()
             == self.mol.GetAtomWithIdx(j).GetAtomicNum()
             == self._atomic_num
         ]
         n = len(Dv)
 
         with self.rethrow_zerodiv():
-            dx = product(Dv) ** (1.0 / (2.0 * n))
+            dx = prod(Dv) ** (1.0 / (2.0 * n))
 
-        return n / (dx ** 2)
+        return n / (dx**2)
 
     rtype = float
```

### Comparing `mordredcommunity-0.0.0a0/mordred/MolecularId.py` & `mordredcommunity-2.0.0/mordred/MolecularId.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-0.0.0a0/mordred/MomentOfInertia.py` & `mordredcommunity-2.0.0/mordred/MomentOfInertia.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-0.0.0a0/mordred/PBF.py` & `mordredcommunity-2.0.0/mordred/PBF.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-0.0.0a0/mordred/PathCount.py` & `mordredcommunity-2.0.0/mordred/PathCount.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-0.0.0a0/mordred/Polarizability.py` & `mordredcommunity-2.0.0/mordred/Polarizability.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-0.0.0a0/mordred/RingCount.py` & `mordredcommunity-2.0.0/mordred/RingCount.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-0.0.0a0/mordred/RotatableBond.py` & `mordredcommunity-2.0.0/mordred/RotatableBond.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-0.0.0a0/mordred/SLogP.py` & `mordredcommunity-2.0.0/mordred/SLogP.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-0.0.0a0/mordred/TopoPSA.py` & `mordredcommunity-2.0.0/mordred/TopoPSA.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-0.0.0a0/mordred/TopologicalCharge.py` & `mordredcommunity-2.0.0/mordred/TopologicalCharge.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-0.0.0a0/mordred/TopologicalIndex.py` & `mordredcommunity-2.0.0/mordred/TopologicalIndex.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-0.0.0a0/mordred/VdwVolumeABC.py` & `mordredcommunity-2.0.0/mordred/VdwVolumeABC.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-0.0.0a0/mordred/VertexAdjacencyInformation.py` & `mordredcommunity-2.0.0/mordred/VertexAdjacencyInformation.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-0.0.0a0/mordred/WalkCount.py` & `mordredcommunity-2.0.0/mordred/WalkCount.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-0.0.0a0/mordred/Weight.py` & `mordredcommunity-2.0.0/mordred/Weight.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-0.0.0a0/mordred/WienerIndex.py` & `mordredcommunity-2.0.0/mordred/WienerIndex.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-0.0.0a0/mordred/ZagrebIndex.py` & `mordredcommunity-2.0.0/mordred/ZagrebIndex.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-0.0.0a0/mordred/__main__.py` & `mordredcommunity-2.0.0/mordred/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,19 +5,26 @@
 import logging
 import argparse
 from importlib import import_module
 from multiprocessing import freeze_support
 
 from rdkit import Chem
 
-from . import Calculator, __version__, descriptors
+from . import Calculator, descriptors
 from ._base import get_descriptors_in_module
 from ._util import PathType, module_prog
 from .error import Missing, MissingValueBase
 
+try:
+    from importlib.metadata import version
+except ImportError:
+    from importlib_metadata import version
+
+__version__ = version("mordredcommunity")
+
 
 def smiles_parser(path):
     with open(path) as file:
         for line in file:
             line = line.strip().split()
             if len(line) == 1:
                 smi = line[0]
```

### Comparing `mordredcommunity-0.0.0a0/mordred/_atomic_property.py` & `mordredcommunity-2.0.0/mordred/_atomic_property.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-0.0.0a0/mordred/_base/__init__.py` & `mordredcommunity-2.0.0/mordred/_base/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,27 +3,25 @@
 from .util import is_missing
 from ..error import MissingValueBase
 from .result import Result
 from .parallel import parallel
 from .calculator import (
     Calculator,
     get_descriptors_in_module,
-    get_descriptors_from_module,
 )
 from .descriptor import (
     Descriptor,
     ConstDescriptor,
     UnaryOperatingDescriptor,
     BinaryOperatingDescriptor,
 )
 
 __all__ = (
     "Descriptor",
     "Calculator",
-    "get_descriptors_from_module",
     "get_descriptors_in_module",
     "is_missing",
     "Result",
 )
 
 
 def _Descriptor__call__(self, mol, id=-1):
```

### Comparing `mordredcommunity-0.0.0a0/mordred/_base/calculator.py` & `mordredcommunity-2.0.0/mordred/_base/calculator.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,30 @@
 from __future__ import print_function
 
 import sys
 import warnings
 from types import ModuleType
 from contextlib import contextmanager
 from multiprocessing import cpu_count
-from distutils.version import StrictVersion
+from packaging.version import Version as StrictVersion
 
 from .._util import Capture, DummyBar
 from ..error import Error, Missing, MultipleFragments, DuplicatedDescriptorName
 from .result import Result
 from .context import Context
-from .._version import __version__
 from .descriptor import Descriptor, MissingValueException, is_descriptor_class
 
 try:
+    from importlib.metadata import version as importlib_version
+except ImportError:
+    from importlib_metadata import version as importlib_version
+
+__version__ = importlib_version("mordredcommunity")
+
+try:
     from tqdm import tqdm
     from .._util import NotebookWrapper
 except ImportError:
     tqdm = NotebookWrapper = DummyBar
 
 
 class Calculator(object):
@@ -190,14 +196,15 @@
             ignore_3D(bool): ignore 3D descriptors
 
         """
         if version is None:
             version = __version__
 
         version = StrictVersion(version)
+
         return self._register(desc, version, ignore_3D)
 
     def _register(self, desc, version, ignore_3D):
         if not hasattr(desc, "__iter__"):
             if is_descriptor_class(desc):
                 if desc.since > version:
                     return
@@ -397,48 +404,14 @@
         return MordredDataFrame(
             (list(r) for r in self.map(mols, nproc, nmols, quiet, ipynb, id)),
             columns=[str(d) for d in self.descriptors],
             index=index,
         )
 
 
-def get_descriptors_from_module(mdl, submodule=False):
-    r"""[DEPRECATED] Get descriptors from module.
-
-    Parameters:
-        mdl(module): module to search
-
-    Returns:
-        [Descriptor]
-
-    """
-    warnings.warn("use get_descriptors_in_module", DeprecationWarning)
-    __all__ = getattr(mdl, "__all__", None)
-    if __all__ is None:
-        __all__ = dir(mdl)
-
-    all_functions = (getattr(mdl, name) for name in __all__ if name[:1] != "_")
-
-    if submodule:
-        descs = [
-            d
-            for fn in all_functions
-            if is_descriptor_class(fn) or isinstance(fn, ModuleType)
-            for d in (
-                [fn]
-                if is_descriptor_class(fn)
-                else get_descriptors_from_module(fn, submodule=True)
-            )
-        ]
-    else:
-        descs = [fn for fn in all_functions if is_descriptor_class(fn)]
-
-    return descs
-
-
 def get_descriptors_in_module(mdl, submodule=True):
     r"""Get descriptors in module.
 
     Parameters:
         mdl(module): module to search
         submodule(bool): search recursively
```

### Comparing `mordredcommunity-0.0.0a0/mordred/_base/context.py` & `mordredcommunity-2.0.0/mordred/_base/context.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-0.0.0a0/mordred/_base/descriptor.py` & `mordredcommunity-2.0.0/mordred/_base/descriptor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 import inspect
 import operator
 from abc import ABCMeta, abstractmethod
 from contextlib import contextmanager
-from distutils.version import StrictVersion
+from packaging.version import Version as StrictVersion
 
 import six
 import numpy as np
 from rdkit import Chem
 
 if hasattr(inspect, "getfullargspec"):
 
     def getargs(func):
         return tuple(inspect.getfullargspec(func).args[1:])
 
-
 else:
 
     def getargs(func):
         try:
             return tuple(inspect.getargspec(func).args[1:])
         except TypeError:
             return ()
```

### Comparing `mordredcommunity-0.0.0a0/mordred/_base/parallel.py` & `mordredcommunity-2.0.0/mordred/_base/parallel.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-0.0.0a0/mordred/_base/result.py` & `mordredcommunity-2.0.0/mordred/_base/result.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-0.0.0a0/mordred/_graph_matrix.py` & `mordredcommunity-2.0.0/mordred/_graph_matrix.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-0.0.0a0/mordred/_matrix_attributes.py` & `mordredcommunity-2.0.0/mordred/_matrix_attributes.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-0.0.0a0/mordred/_util.py` & `mordredcommunity-2.0.0/mordred/_util.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-0.0.0a0/mordred/descriptors/__init__.py` & `mordredcommunity-2.0.0/mordred/descriptors/__init__.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-0.0.0a0/mordred/error/__init__.py` & `mordredcommunity-2.0.0/mordred/error/__init__.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-0.0.0a0/mordred/surface_area/__init__.py` & `mordredcommunity-2.0.0/mordred/surface_area/__init__.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-0.0.0a0/mordred/surface_area/__main__.py` & `mordredcommunity-2.0.0/mordred/surface_area/__main__.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-0.0.0a0/mordred/surface_area/_mesh.py` & `mordredcommunity-2.0.0/mordred/surface_area/_mesh.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-0.0.0a0/mordred/surface_area/_sasa.py` & `mordredcommunity-2.0.0/mordred/surface_area/_sasa.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-0.0.0a0/mordred/tests/Dummy.py` & `mordredcommunity-2.0.0/mordred/tests/Dummy.py`

 * *Files identical despite different names*

### Comparing `mordredcommunity-0.0.0a0/mordred/tests/test_ABCIndex.py` & `mordredcommunity-2.0.0/mordred/tests/test_ABCIndex.py`

 * *Files 25% similar despite different names*

```diff
@@ -18,9 +18,9 @@
     abc = ABCIndex()
     abcgg = ABCGGIndex()
 
     for line in data.split("\n"):
         smi, dABC, dABCGG = line.strip().split()
 
         mol = Chem.MolFromSmiles(smi)
-        yield assert_almost_equal, abc(mol), float(dABC), 2
-        yield assert_almost_equal, abcgg(mol), float(dABCGG), 2
+        assert assert_almost_equal(abc(mol), float(dABC), 2) is None
+        assert assert_almost_equal(abcgg(mol), float(dABCGG), 2) is None
```

### Comparing `mordredcommunity-0.0.0a0/mordred/tests/test_ETA.py` & `mordredcommunity-2.0.0/mordred/tests/test_ETA.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,10 +111,13 @@
     calc = Calculator(ExtendedTopochemicalAtom)
 
     for smi, desireds in references.items():
         mol = Chem.MolFromSmiles(smi)
         actuals = {str(d): v for d, v in zip(calc.descriptors, calc(mol))}
 
         for name, desired in desireds.items():
-            yield assert_almost_equal, actuals[name], desired, 2, "{} of {}".format(
-                name, smi
+            assert (
+                assert_almost_equal(
+                    actuals[name], desired, 2, "{} of {}".format(name, smi)
+                )
+                is None
             )
```

### Comparing `mordredcommunity-0.0.0a0/mordred/tests/test_SASA.py` & `mordredcommunity-2.0.0/mordred/tests/test_SASA.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import os
 
 from rdkit import Chem
 
-from nose.tools import ok_
 from mordred.CPSA import TotalSurfaceArea
 from mordred.surface_area import SurfaceArea
 
 # calculated by pymol
 txt_data = """
 Hexane               296.910
 Benzene              243.552
@@ -54,12 +53,12 @@
             continue
 
         desired = data[name]
 
         e = abs((actual - desired) / desired)
         p = 0.05
 
-        yield ok_, e < p, "large SASA error in {}: {}".format(name, e)
+        assert e < p, "large SASA error in {}: {}".format(name, e)
 
         e = abs((tsa(mol) - desired) / desired)
 
-        yield ok_, e < p, "large SASA error in {}: {}".format(name, e)
+        assert e < p, "large SASA error in {}: {}".format(name, e)
```

### Comparing `mordredcommunity-0.0.0a0/mordred/tests/test_VEA.py` & `mordredcommunity-2.0.0/mordred/tests/test_VEA.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,14 +78,15 @@
             actual = actuals[desc]
             decimal, desired = desireds[desc]
             if desired is None:
                 continue
 
             assert not is_missing(actual), actual
 
-            yield (
-                assert_almost_equal,
-                actual,
-                desired,
-                decimal,
-                "{} of {}".format(desc, smi),
-            )
+            assert (
+                assert_almost_equal(
+                    actual,
+                    desired,
+                    decimal,
+                    "{} of {}".format(desc, smi),
+                )
+            ) is None
```

### Comparing `mordredcommunity-0.0.0a0/mordred/tests/test_atomic_property.py` & `mordredcommunity-2.0.0/mordred/tests/test_atomic_property.py`

 * *Files 7% similar despite different names*

```diff
@@ -39,16 +39,16 @@
 implicitHs = {
     key: Chem.MolFromSmiles(smi).GetAtomWithIdx(1) for key, smi in _data.items()
 }
 
 
 def make_cases(results, fn, decimal=7):
     for key, result in results.items():
-        yield assert_almost_equal, result, fn(explicitHs[key]), decimal, key
-        yield assert_almost_equal, result, fn(implicitHs[key]), decimal, key
+        assert assert_almost_equal(result, fn(explicitHs[key]), decimal, key) is None
+        assert assert_almost_equal(result, fn(implicitHs[key]), decimal, key) is None
 
 
 def test_sigma():
     results = {
         ">C<": 4,
         ">CH-": 3,
         "-CH2-": 2,  # noqa: S001
@@ -71,16 +71,15 @@
         "-SH": 1,
         "-S-": 2,  # noqa: S001
         "=S": 1,
         "-Cl": 1,  # noqa: S001
         "-Br": 1,  # noqa: S001
         "-I": 1,
     }
-    for test in make_cases(results, _atomic_property.get_sigma_electrons):
-        yield test
+    make_cases(results, _atomic_property.get_sigma_electrons)
 
 
 def test_valence_sigma():
     results = {
         ">C<": 4,
         ">CH-": 3,
         "-CH2-": 2,  # noqa: S001
@@ -101,16 +100,15 @@
         "=O": 6,
         "-F": 7,  # noqa: S001
         "-S-": 0.67,
         "-Cl": 0.78,  # noqa: S001
         "-Br": 0.26,  # noqa: S001
         "-I": 0.16,
     }
-    for test in make_cases(results, _atomic_property.get_valence_electrons, 2):
-        yield test
+    make_cases(results, _atomic_property.get_valence_electrons, 2)
 
 
 def test_IntrinsicState():
     results = {
         ">C<": 1.25,
         ">CH-": 1.3333,
         "-CH2-": 1.5,  # noqa: S001
@@ -128,9 +126,8 @@
         "=NH": 5.0,
         "#N": 6.0,  # noqa: S001
         "-OH": 6.0,
         "=O": 7.0,
         "-F": 8.0,  # noqa: S001
     }
 
-    for test in make_cases(results, _atomic_property.get_intrinsic_state, 3):
-        yield test
+    make_cases(results, _atomic_property.get_intrinsic_state, 3)
```

### Comparing `mordredcommunity-0.0.0a0/mordred/tests/test_by_references.py` & `mordredcommunity-2.0.0/mordred/tests/test_by_references.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 
 import yaml
 import numpy as np
 from rdkit import Chem
 from numpy.testing import assert_almost_equal
 
 from mordred import Calculator, Polarizability, descriptors
-from nose.tools import eq_
 from mordred.error import MissingValueBase
 
 try:
     from yaml import CLoader as Loader
 except ImportError:
     from yaml import Loader
 
@@ -47,26 +46,24 @@
             desireds = (
                 (mname, zip(dnames, values if isinstance(values, list) else [values]))
                 for mname, values in test["results"].items()
             )
 
             digit = test.get("digit")
             if digit is None:
-                assert_f = eq_
-            else:
+                digit = 0  # exact match
 
-                def assert_f(a, d, m):
-                    if np.isnan(d):
-                        assert isinstance(a, MissingValueBase)
-                        return
+            def assert_f(a, d, m):
+                if np.isnan(d):
+                    assert isinstance(a, MissingValueBase)
+                    return
 
-                    assert_almost_equal(a, d, digit, m)
+                assert_almost_equal(a, d, digit, m)
 
             for mname, descs in desireds:
                 for dname, desired in descs:
                     if not desired == "skip":
-                        yield (
-                            assert_f,
+                        assert_f(
                             actuals[mname][dname],
                             desired,
                             "{} of {}".format(dname, mname),
                         )
```

### Comparing `mordredcommunity-0.0.0a0/mordred/tests/test_compose_descriptor.py` & `mordredcommunity-2.0.0/mordred/tests/test_compose_descriptor.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import math
 import operator
 
 import six
 from rdkit import Chem
 
-from nose.tools import eq_
 
 from .. import ABCIndex
 
 binary = [
     operator.add,
     operator.sub,
     operator.mul,
@@ -27,11 +26,11 @@
 
 def test_compose_descriptor():
     L = ABCIndex.ABCIndex()
     r = ABCIndex.ABCGGIndex()
     m = Chem.MolFromSmiles("c1ccccc1C")
 
     for op in binary:
-        yield eq_, op(L, r)(m), op(L(m), r(m))
+        assert op(L, r)(m) == op(L(m), r(m))
 
     for op in unary:
-        yield eq_, op(L)(m), op(L(m))
+        assert op(L)(m) == op(L(m))
```

### Comparing `mordredcommunity-0.0.0a0/mordred/tests/test_exceptions.py` & `mordredcommunity-2.0.0/mordred/tests/test_exceptions.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from rdkit import Chem
 
 from mordred import Calculator, Descriptor
-from nose.tools import eq_
 from mordred.error import Error
 
 
 class RaiseDescriptor(Descriptor):
     def parameters(self):
         return ()
 
@@ -21,8 +20,8 @@
 
 
 def test_catch_non_critical_error():
     calc = Calculator(RaiseDescriptor(ValueError("test exception"), False))
 
     result = calc(mol)[0]
     assert isinstance(result, Error)
-    eq_(result.error.args, ("test exception",))
+    assert result.error.args == ("test exception",)
```

### Comparing `mordredcommunity-0.0.0a0/mordred/tests/test_mordred_main.py` & `mordredcommunity-2.0.0/mordred/tests/test_mordred_main.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,22 +2,28 @@
 import sys
 import shutil
 import tempfile
 from contextlib import contextmanager
 
 from rdkit.Chem import AllChem as Chem
 
-from nose.tools import eq_
 
-from .. import Calculator, __version__, descriptors
+from .. import Calculator, descriptors
 from ..__main__ import main as mordred
 
 Nd2D = len(Calculator(descriptors, ignore_3D=True).descriptors)
 Nd3D = len(Calculator(descriptors, ignore_3D=False).descriptors)
 
+try:
+    from importlib.metadata import version
+except ImportError:
+    from importlib_metadata import version
+
+__version__ = version("mordredcommunity")
+
 
 def in_(a, s):
     assert a in s, "{!r} not in {!r}".format(a, s)
 
 
 @contextmanager
 def isolate():
@@ -69,49 +75,46 @@
         os.remove(epath)
 
     return r
 
 
 def test_no_args():
     stdout, stderr, exitcode = command(mordred)
-    eq_(exitcode, 2)
-    eq_(stdout, "")
+    assert exitcode == 2
+    assert stdout == ""
     in_("usage:", stderr)
     # python3 or python2
     assert (
         "the following arguments are required: INPUT" in stderr
         or "too few arguments" in stderr
     )
 
 
 def test_help():
     stdout, stderr, exitcode = command(mordred, "-h")
-    eq_(exitcode, 0)
-    eq_(stderr, "")
+    assert exitcode == 0
+    assert stderr == ""
     in_("usage:", stdout)
     in_("descriptors:", stdout)
 
 
 def test_version():
     stdout, stderr, exitcode = command(mordred, "--version")
-    eq_(exitcode, 0)
+    assert exitcode == 0
 
     vstr = "mordred-{}\n".format(__version__)
 
-    if stderr == "":  # python 3
-        eq_(stdout, vstr)
-    else:  # python2
-        eq_(stderr, vstr)
+    assert stdout == vstr
 
 
 def test_missing_file():
     with isolate():
         stdout, stderr, exitcode = command(mordred, "missing.smi")
-        eq_(exitcode, 2)
-        eq_(stdout, "")
+        assert exitcode == 2
+        assert stdout == ""
         in_("usage:", stderr)
         in_("invalid PathType value", stderr)
 
 
 def number_of_field(output):
     return len(list(filter(lambda c: c == ",", output.split("\n")[0])))
 
@@ -119,74 +122,74 @@
 def test_smi():
     with isolate():
         with open("input.smi", "w") as f:
             f.write("c1ccccc1 Benzene\n")
 
         stdout, stderr, exitcode = command(mordred, "input.smi", "-q", "-o", "-")
 
-        eq_(exitcode, 0)
-        eq_(number_of_field(stdout), Nd2D)
-        eq_(stdout.split("\n")[1].split(",")[0], "Benzene")
-        eq_(stderr, "")
+        assert exitcode == 0
+        assert number_of_field(stdout) == Nd2D
+        assert stdout.split("\n")[1].split(",")[0] == "Benzene"
+        assert stderr == ""
 
 
 def test_smi_without_name():
     with isolate():
         with open("input.smi", "w") as f:
             f.write("c1ccccc1\n")
 
         stdout, stderr, exitcode = command(mordred, "input.smi", "-q", "-o", "-")
 
-        eq_(exitcode, 0)
-        eq_(number_of_field(stdout), Nd2D)
-        eq_(stdout.split("\n")[1].split(",")[0], "c1ccccc1")
-        eq_(stderr, "")
+        assert exitcode == 0
+        assert number_of_field(stdout) == Nd2D
+        assert stdout.split("\n")[1].split(",")[0] == "c1ccccc1"
+        assert stderr == ""
 
 
 def test_sdf():
     with isolate():
         mol = Chem.MolFromSmiles("c1ccccc1")
         mol.SetProp("_Name", "Benzene")
         Chem.MolToMolFile(mol, "input.sdf")
 
         stdout, stderr, exitcode = command(
             mordred, "input.sdf", "-q", "-o", "output.csv"
         )
 
-        eq_(exitcode, 0)
-        eq_(stdout, "")
-        eq_(stderr, "")
+        assert exitcode == 0
+        assert stdout == ""
+        assert stderr == ""
         output = open("output.csv").read()
-        eq_(number_of_field(output), Nd2D)
-        eq_(output.split("\n")[1].split(",")[0], "Benzene")
+        assert number_of_field(output) == Nd2D
+        assert output.split("\n")[1].split(",")[0] == "Benzene"
 
 
 def test_sdf_3D():
     with isolate():
         mol = Chem.MolFromSmiles("c1ccccc1")
         Chem.EmbedMolecule(mol)
         mol.SetProp("_Name", "Benzene")
         Chem.MolToMolFile(mol, "input.sdf")
 
         stdout, stderr, exitcode = command(
             mordred, "input.sdf", "-q", "-o", "output.csv", "-3"
         )
 
-        eq_(exitcode, 0)
-        eq_(stdout, "")
-        eq_(stderr, "")
+        assert exitcode == 0
+        assert stdout == ""
+        assert stderr == ""
         output = open("output.csv").read()
-        eq_(number_of_field(output), Nd3D)
-        eq_(output.split("\n")[1].split(",")[0], "Benzene")
+        assert number_of_field(output) == Nd3D
+        assert output.split("\n")[1].split(",")[0] == "Benzene"
 
 
 def test_verbose():
     with isolate():
         with open("input.smi", "w") as f:
             f.write("c1ccccc1 Benzene\n")
 
         r = command(mordred, "input.smi", "-o", "-", "-q", "-vv")
 
-        eq_(r.exitcode, 0)
-        eq_(number_of_field(r.stdout), Nd2D)
-        eq_(r.stdout.split("\n")[1].split(",")[0], "Benzene")
-        in_("[Missing]", r.stderr)
+        assert r.exitcode == 0
+        assert number_of_field(r.stdout) == Nd2D
+        assert r.stdout.split("\n")[1].split(",")[0] == "Benzene"
+        assert "[Missing]" in r.stderr
```

### Comparing `mordredcommunity-0.0.0a0/mordred/tests/test_parallel.py` & `mordredcommunity-2.0.0/mordred/tests/test_parallel.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 import os
 
 from rdkit.Chem import AllChem as Chem
 from numpy.testing import assert_almost_equal
 
 from mordred import Calculator, descriptors
-from nose.tools import eq_
 from mordred.error import MissingValueBase
 
 data_file = os.path.join(os.path.dirname(__file__), "references", "structures.sdf")
 
 
 def test_parallel():
     calc = Calculator(descriptors)
     mols = [m for m in Chem.SDMolSupplier(data_file, removeHs=False)]
 
     for serial, parallel in zip(
         calc.map(mols, nproc=1, quiet=True), calc.map(mols, quiet=True)
     ):
         for d, s, p in zip(calc.descriptors, serial, parallel):
-
             if isinstance(s, MissingValueBase):
-                yield eq_, s.error.__class__, p.error.__class__
+                assert s.error.__class__ == p.error.__class__
             else:
                 msg = "{} (serial: {}, parallel: {})".format(str(d), s, p)
-                yield assert_almost_equal, s, p, 7, msg
+                assert assert_almost_equal(s, p, 7, msg) is None
```

### Comparing `mordredcommunity-0.0.0a0/mordred/tests/test_pickle.py` & `mordredcommunity-2.0.0/mordred/tests/test_pickle.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,30 +2,29 @@
 import pickle
 
 import six
 from rdkit import Chem
 from numpy.testing import assert_almost_equal
 
 from mordred import Calculator, descriptors
-from nose.tools import eq_
 from mordred.error import MissingValueBase
 
 
 def test_pickle_calculator():
     orig = Calculator(descriptors)
     d0 = orig.descriptors[0]
     d1 = orig.descriptors[1]
     orig.register(
         [
             d0 + d1,
             d0 - d1,
             d0 * d1,
             d0 // d1,
             d0 % d1,
-            d0 ** d1,
+            d0**d1,
             -d0,
             +d1,
             abs(d0),
             math.trunc(d0),
         ]
     )
 
@@ -33,14 +32,14 @@
         orig.register([math.ceil(d0), math.floor(d1)])
 
     pickled = pickle.loads(pickle.dumps(orig))
 
     mol = Chem.MolFromSmiles("c1ccccc1C(O)O")
 
     for a, b in zip(orig.descriptors, pickled.descriptors):
-        yield eq_, a, b
+        assert a == b
 
     for a, b in zip(orig(mol), pickled(mol)):
         if isinstance(a, MissingValueBase):
-            yield eq_, a.__class__, b.__class__
+            assert a.__class__ == b.__class__
         else:
-            yield assert_almost_equal, a, b
+            assert_almost_equal(a, b)
```

### Comparing `mordredcommunity-0.0.0a0/mordredcommunity.egg-info/SOURCES.txt` & `mordredcommunity-2.0.0/mordredcommunity.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 LICENSE
-README.rst
+README.md
 pyproject.toml
 mordred/ABCIndex.py
 mordred/AcidBase.py
 mordred/AdjacencyMatrix.py
 mordred/Aromatic.py
 mordred/AtomCount.py
 mordred/Autocorrelation.py
@@ -69,23 +69,21 @@
 mordred/error/__init__.py
 mordred/surface_area/__init__.py
 mordred/surface_area/__main__.py
 mordred/surface_area/_mesh.py
 mordred/surface_area/_sasa.py
 mordred/tests/Dummy.py
 mordred/tests/__init__.py
-mordred/tests/__main__.py
 mordred/tests/test_ABCIndex.py
 mordred/tests/test_ETA.py
 mordred/tests/test_SASA.py
 mordred/tests/test_SLogP.py
 mordred/tests/test_VEA.py
 mordred/tests/test_atomic_property.py
 mordred/tests/test_attributes.py
-mordred/tests/test_base.py
 mordred/tests/test_by_references.py
 mordred/tests/test_compose_descriptor.py
 mordred/tests/test_exceptions.py
 mordred/tests/test_import_all_descriptors.py
 mordred/tests/test_json.py
 mordred/tests/test_mordred_main.py
 mordred/tests/test_pandas.py
```

### Comparing `mordredcommunity-0.0.0a0/pyproject.toml` & `mordredcommunity-2.0.0/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,38 +1,44 @@
 [build-system]
 requires = ["setuptools>=64"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mordredcommunity"
-version = "0.0.0a0"
+version = "2.0.0"
 authors = [{ name = "Jackson Burns", email = "jwburns@mit.edu" }]
 license = { text = "BSD-3-Clause" }
 description = "Community-Maintained Version of mordred"
 classifiers = [
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 urls = { Homepage = "https://github.com/JacksonBurns/mordred-community" }
 requires-python = ">=3.7"
-dependencies = ["six==1.*", "numpy==1.*", "networkx>=3"]
+dependencies = [
+    "rdkit",
+    "six",
+    "numpy",
+    "networkx",
+    "importlib-metadata ; python_version < '3.8'",
+]
 
 [project.optional-dependencies]
-full = ["pandas", "tqdm"]
+full = ["pandas", "tqdm", "pyyaml"]
 
 [project.readme]
 file = "README.md"
-content-type = "text/x-rst"
+content-type = "text/markdown"
 
 [tool.isort]
 profile = "black"
 
 [tool.setuptools]
 include-package-data = true
 
 [tool.setuptools.packages.find]
 where = ["."]
 include = ["mordred*"]
-exclude = ["docs*", "examples*", "extra*"]
+exclude = ["docs*", "examples*"]
```

