# Comparing `tmp/pami-2023.7.21.tar.gz` & `tmp/pami-2023.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pami-2023.7.21.tar", last modified: Fri Jul 21 11:53:35 2023, max compression
+gzip compressed data, was "pami-2023.7.7.tar", last modified: Tue Jul 18 12:23:34 2023, max compression
```

## Comparing `pami-2023.7.21.tar` & `pami-2023.7.7.tar`

### file list

```diff
@@ -1,428 +1,434 @@
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-21 11:53:35.600457 pami-2023.7.21/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    35149 2023-07-20 11:14:51.000000 pami-2023.7.21/LICENSE
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-21 11:53:35.536643 pami-2023.7.21/PAMI/
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-21 11:53:35.536816 pami-2023.7.21/PAMI/AssociationRules/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/AssociationRules/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-21 11:53:35.537742 pami-2023.7.21/PAMI/AssociationRules/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     8002 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/AssociationRules/basic/ARWithConfidence.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     8028 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/AssociationRules/basic/ARWithLeverage.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     8068 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/AssociationRules/basic/ARWithLift.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    12384 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/AssociationRules/basic/RuleMiner.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/AssociationRules/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6542 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/AssociationRules/basic/abstract.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      139 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-21 11:53:35.537907 pami-2023.7.21/PAMI/correlatedPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/correlatedPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-21 11:53:35.539295 pami-2023.7.21/PAMI/correlatedPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    24475 2023-07-21 10:42:12.000000 pami-2023.7.21/PAMI/correlatedPattern/basic/CPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    25915 2023-07-21 11:07:26.000000 pami-2023.7.21/PAMI/correlatedPattern/basic/CPGrowthPlus.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/correlatedPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6065 2023-07-21 11:06:55.000000 pami-2023.7.21/PAMI/correlatedPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-21 11:53:35.539530 pami-2023.7.21/PAMI/coveragePattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/coveragePattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-21 11:53:35.540260 pami-2023.7.21/PAMI/coveragePattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    13779 2023-07-21 11:20:16.000000 pami-2023.7.21/PAMI/coveragePattern/basic/CMine.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    16070 2023-07-20 11:24:17.000000 pami-2023.7.21/PAMI/coveragePattern/basic/CPPG.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/coveragePattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     7018 2023-07-21 11:15:56.000000 pami-2023.7.21/PAMI/coveragePattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-21 11:53:35.541749 pami-2023.7.21/PAMI/extras/
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-21 11:53:35.542989 pami-2023.7.21/PAMI/extras/DF2DB/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     2178 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/extras/DF2DB/DF2DB.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     2243 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/extras/DF2DB/DF2DBPlus.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/extras/DF2DB/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     1607 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/extras/DF2DB/createTDB.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     4185 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/extras/DF2DB/denseDF2DB.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     4917 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/extras/DF2DB/denseDF2DBPlus.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     9942 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/extras/DF2DB/denseDF2DB_dump.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     3607 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/extras/DF2DB/sparseDF2DB.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     3359 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/extras/DF2DB/sparseDF2DBPlus.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/extras/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-21 11:53:35.543341 pami-2023.7.21/PAMI/extras/calculateMISValues/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/extras/calculateMISValues/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     3741 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/extras/calculateMISValues/usingBeta.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     3794 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/extras/calculateMISValues/usingSD.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-21 11:53:35.544252 pami-2023.7.21/PAMI/extras/dbStats/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/extras/dbStats/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    13043 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/extras/dbStats/fuzzyDatabaseStats.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    14661 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/extras/dbStats/temporalDatabaseStats.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     9364 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/extras/dbStats/transactionalDatabaseStats.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    13229 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/extras/dbStats/uncertainTemporalDatabaseStats.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    10040 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/extras/dbStats/uncertainTransactionalDatabaseStats.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    11775 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/extras/dbStats/utilityDatabaseStats.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-21 11:53:35.544883 pami-2023.7.21/PAMI/extras/fuzzyTransformation/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/extras/fuzzyTransformation/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     5195 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/extras/fuzzyTransformation/abstract.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     5925 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/extras/fuzzyTransformation/temporalToFuzzy.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     5919 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/extras/fuzzyTransformation/transactionalToFuzzyTimeSeries.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     5803 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/extras/fuzzyTransformation/utilityToFuzzy.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-21 11:53:35.545394 pami-2023.7.21/PAMI/extras/generateDatabase/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/extras/generateDatabase/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     2877 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/extras/generateDatabase/generateSpatioTemporalDatabase.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     7092 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/extras/generateDatabase/generateTemporalDatabase.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     3444 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/extras/generateDatabase/generateTransactionalDatabase.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     3593 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/extras/generateLatexGraphFile.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-21 11:53:35.546141 pami-2023.7.21/PAMI/extras/graph/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/extras/graph/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     1656 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/extras/graph/dataFrameInToFigures.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     2954 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/extras/graph/generateLatexFileFromDataFrame.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     1167 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/extras/graph/plotLineGraphFromDictionary.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     1753 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/extras/graph/plotLineGraphsFromDataFrame.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     2203 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/extras/graph/visualizePatterns.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-21 11:53:35.546272 pami-2023.7.21/PAMI/extras/image2Database/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/extras/image2Database/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-21 11:53:35.546529 pami-2023.7.21/PAMI/extras/imageProcessing/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/extras/imageProcessing/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     4582 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/extras/imageProcessing/imagery2Databases.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-21 11:53:35.546806 pami-2023.7.21/PAMI/extras/neighbours/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/extras/neighbours/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     2834 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/extras/neighbours/findNeighboursUsingEuclidean.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     3031 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/extras/plotPointOnMap.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     3214 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/extras/plotPointOnMap_dump.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     2178 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/extras/scatterPlotSpatialPoints.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-21 11:53:35.548244 pami-2023.7.21/PAMI/extras/syntheticDatabaseGenerator/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/extras/syntheticDatabaseGenerator/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     2332 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/extras/syntheticDatabaseGenerator/createSyntheticGeoreferentialTemporal.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     2297 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/extras/syntheticDatabaseGenerator/createSyntheticGeoreferentialTransactions.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     2555 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/extras/syntheticDatabaseGenerator/createSyntheticGeoreferentialUncertainTransaction.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     1887 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/extras/syntheticDatabaseGenerator/createSyntheticTemporal.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     1860 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/extras/syntheticDatabaseGenerator/createSyntheticTransactions.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     2126 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/extras/syntheticDatabaseGenerator/createSyntheticUncertainTemporal.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     2079 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/extras/syntheticDatabaseGenerator/createSyntheticUncertainTransactions.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     2265 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/extras/syntheticDatabaseGenerator/createSyntheticUtility.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     1827 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/extras/topKPatterns.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      473 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/extras/uncertaindb_convert.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-21 11:53:35.548423 pami-2023.7.21/PAMI/faultTolerantFrequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/faultTolerantFrequentPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-21 11:53:35.549372 pami-2023.7.21/PAMI/faultTolerantFrequentPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    14656 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/faultTolerantFrequentPattern/basic/FTApriori.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    21114 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/faultTolerantFrequentPattern/basic/FTFPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    14988 2023-07-20 11:24:17.000000 pami-2023.7.21/PAMI/faultTolerantFrequentPattern/basic/VBFTMine.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/faultTolerantFrequentPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6691 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/faultTolerantFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-21 11:53:35.549537 pami-2023.7.21/PAMI/frequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/frequentPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-21 11:53:35.550621 pami-2023.7.21/PAMI/frequentPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    13124 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/frequentPattern/basic/Apriori.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    12531 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/frequentPattern/basic/ECLAT.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    13188 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/frequentPattern/basic/ECLATDiffset.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    13480 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/frequentPattern/basic/ECLATbitset.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    20324 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/frequentPattern/basic/FPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/frequentPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     7733 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/frequentPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-21 11:53:35.551081 pami-2023.7.21/PAMI/frequentPattern/closed/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    19874 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/frequentPattern/closed/CHARM.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/frequentPattern/closed/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6445 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/frequentPattern/closed/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-21 11:53:35.552530 pami-2023.7.21/PAMI/frequentPattern/cuda/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/frequentPattern/cuda/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6564 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/frequentPattern/cuda/abstract.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    13459 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/frequentPattern/cuda/cuApriori.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    14203 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/frequentPattern/cuda/cuAprioriBit.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    13085 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/frequentPattern/cuda/cuEclat.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    13942 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/frequentPattern/cuda/cuEclatBit.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     5738 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/frequentPattern/cuda/cudaAprioriGCT.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     8648 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/frequentPattern/cuda/cudaAprioriTID.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     5576 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/frequentPattern/cuda/cudaEclatGCT.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-21 11:53:35.553053 pami-2023.7.21/PAMI/frequentPattern/maximal/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    25097 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/frequentPattern/maximal/MaxFPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/frequentPattern/maximal/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6436 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/frequentPattern/maximal/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-21 11:53:35.554006 pami-2023.7.21/PAMI/frequentPattern/pyspark/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/frequentPattern/pyspark/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     5603 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/frequentPattern/pyspark/abstract.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    13209 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/frequentPattern/pyspark/parallelApriori.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    11487 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/frequentPattern/pyspark/parallelECLAT.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    16147 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/frequentPattern/pyspark/parallelFPGrowth.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-21 11:53:35.554798 pami-2023.7.21/PAMI/frequentPattern/topk/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    14674 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/frequentPattern/topk/FAE.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/frequentPattern/topk/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     4575 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/frequentPattern/topk/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-21 11:53:35.554945 pami-2023.7.21/PAMI/frequentSpatialPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/frequentSpatialPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-21 11:53:35.555603 pami-2023.7.21/PAMI/frequentSpatialPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    20041 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/frequentSpatialPattern/basic/FSPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    19099 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/frequentSpatialPattern/basic/SpatialECLAT.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/frequentSpatialPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6680 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/frequentSpatialPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-21 11:53:35.555765 pami-2023.7.21/PAMI/fuzzyCorrelatedPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/fuzzyCorrelatedPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-21 11:53:35.556259 pami-2023.7.21/PAMI/fuzzyCorrelatedPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    25239 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/fuzzyCorrelatedPattern/basic/FCPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/fuzzyCorrelatedPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6635 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/fuzzyCorrelatedPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-21 11:53:35.556391 pami-2023.7.21/PAMI/fuzzyFrequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/fuzzyFrequentPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-21 11:53:35.558193 pami-2023.7.21/PAMI/fuzzyFrequentPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    20733 2023-07-20 11:24:17.000000 pami-2023.7.21/PAMI/fuzzyFrequentPattern/basic/FFIMiner.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    24620 2023-07-20 11:24:18.000000 pami-2023.7.21/PAMI/fuzzyFrequentPattern/basic/FFIMiner_old.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/fuzzyFrequentPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6450 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/fuzzyFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-21 11:53:35.558372 pami-2023.7.21/PAMI/fuzzyFrequentSpatialPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/fuzzyFrequentSpatialPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-21 11:53:35.559046 pami-2023.7.21/PAMI/fuzzyFrequentSpatialPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    23992 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/fuzzyFrequentSpatialPattern/basic/FFSPMiner.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    26791 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/fuzzyFrequentSpatialPattern/basic/FFSPMiner_old.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/fuzzyFrequentSpatialPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6580 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/fuzzyFrequentSpatialPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-21 11:53:35.559243 pami-2023.7.21/PAMI/fuzzyPartialPeriodicPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/fuzzyPartialPeriodicPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-21 11:53:35.559572 pami-2023.7.21/PAMI/fuzzyPartialPeriodicPattern/irregularTimeSeries/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/fuzzyPartialPeriodicPattern/irregularTimeSeries/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6449 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/fuzzyPartialPeriodicPattern/irregularTimeSeries/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-21 11:53:35.559728 pami-2023.7.21/PAMI/fuzzyPeriodicFrequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/fuzzyPeriodicFrequentPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-21 11:53:35.560493 pami-2023.7.21/PAMI/fuzzyPeriodicFrequentPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    23521 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/fuzzyPeriodicFrequentPattern/basic/FPFPMiner.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    25345 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/fuzzyPeriodicFrequentPattern/basic/FPFPMiner_old.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/fuzzyPeriodicFrequentPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6668 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/fuzzyPeriodicFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-21 11:53:35.560651 pami-2023.7.21/PAMI/fuzzySpatialPeriodicFrequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/fuzzySpatialPeriodicFrequentPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-21 11:53:35.561311 pami-2023.7.21/PAMI/fuzzySpatialPeriodicFrequentPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    26817 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/fuzzySpatialPeriodicFrequentPattern/basic/FGPFPMiner.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    32216 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/fuzzySpatialPeriodicFrequentPattern/basic/FGPFPMiner_old.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/fuzzySpatialPeriodicFrequentPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6618 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/fuzzySpatialPeriodicFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-21 11:53:35.561810 pami-2023.7.21/PAMI/geoReferencedFrequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    28518 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/geoReferencedFrequentPattern/GFPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/geoReferencedFrequentPattern/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     5007 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/geoReferencedFrequentPattern/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-21 11:53:35.561956 pami-2023.7.21/PAMI/geoReferencedPeriodicFrequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/geoReferencedPeriodicFrequentPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-21 11:53:35.562400 pami-2023.7.21/PAMI/geoReferencedPeriodicFrequentPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    19950 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/geoReferencedPeriodicFrequentPattern/basic/GPFPMiner.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/geoReferencedPeriodicFrequentPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6774 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/geoReferencedPeriodicFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-21 11:53:35.562918 pami-2023.7.21/PAMI/georeferencedFrequentSequencePattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/georeferencedFrequentSequencePattern/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6676 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/georeferencedFrequentSequencePattern/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-21 11:53:35.563200 pami-2023.7.21/PAMI/highUtilityFrequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/highUtilityFrequentPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-21 11:53:35.564059 pami-2023.7.21/PAMI/highUtilityFrequentPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    35398 2023-07-20 11:24:18.000000 pami-2023.7.21/PAMI/highUtilityFrequentPattern/basic/HUFIM.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/highUtilityFrequentPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6081 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/highUtilityFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-21 11:53:35.564189 pami-2023.7.21/PAMI/highUtilityFrequentSpatialPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/highUtilityFrequentSpatialPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-21 11:53:35.564586 pami-2023.7.21/PAMI/highUtilityFrequentSpatialPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    39910 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/highUtilityFrequentSpatialPattern/basic/SHUFIM.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/highUtilityFrequentSpatialPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6181 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/highUtilityFrequentSpatialPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-21 11:53:35.564735 pami-2023.7.21/PAMI/highUtilityPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/highUtilityPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-21 11:53:35.565554 pami-2023.7.21/PAMI/highUtilityPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    32744 2023-07-20 11:24:18.000000 pami-2023.7.21/PAMI/highUtilityPattern/basic/EFIM.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    24844 2023-07-20 11:24:18.000000 pami-2023.7.21/PAMI/highUtilityPattern/basic/HMiner.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    26560 2023-07-20 11:24:18.000000 pami-2023.7.21/PAMI/highUtilityPattern/basic/UPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/highUtilityPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     5053 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/highUtilityPattern/basic/abstract.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    16478 2023-07-20 11:24:18.000000 pami-2023.7.21/PAMI/highUtilityPattern/basic/efimParallel.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-21 11:53:35.566002 pami-2023.7.21/PAMI/highUtilityPattern/parallel/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/highUtilityPattern/parallel/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     5053 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/highUtilityPattern/parallel/abstract.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    16480 2023-07-20 11:24:18.000000 pami-2023.7.21/PAMI/highUtilityPattern/parallel/efimparallel.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-21 11:53:35.567102 pami-2023.7.21/PAMI/highUtilityPatternsInStreams/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    29434 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/highUtilityPatternsInStreams/HUPMS.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    33678 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/highUtilityPatternsInStreams/SHUGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/highUtilityPatternsInStreams/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     5195 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/highUtilityPatternsInStreams/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-21 11:53:35.567367 pami-2023.7.21/PAMI/highUtilitySpatialPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/highUtilitySpatialPattern/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6718 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/highUtilitySpatialPattern/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-21 11:53:35.567939 pami-2023.7.21/PAMI/highUtilitySpatialPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    27632 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/highUtilitySpatialPattern/basic/HDSHUIM.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    34623 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/highUtilitySpatialPattern/basic/SHUIM.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/highUtilitySpatialPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     5955 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/highUtilitySpatialPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-21 11:53:35.568356 pami-2023.7.21/PAMI/highUtilitySpatialPattern/topk/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    35216 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/highUtilitySpatialPattern/topk/TKSHUIM.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/highUtilitySpatialPattern/topk/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6625 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/highUtilitySpatialPattern/topk/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-21 11:53:35.568489 pami-2023.7.21/PAMI/localPeriodicPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/localPeriodicPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-21 11:53:35.569538 pami-2023.7.21/PAMI/localPeriodicPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    32664 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/localPeriodicPattern/basic/LPPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    21999 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/localPeriodicPattern/basic/LPPMBreadth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    21120 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/localPeriodicPattern/basic/LPPMDepth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/localPeriodicPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     8378 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/localPeriodicPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-21 11:53:35.569842 pami-2023.7.21/PAMI/multipleMinimumSupportBasedFrequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/multipleMinimumSupportBasedFrequentPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-21 11:53:35.570462 pami-2023.7.21/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    23034 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/CFPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    22318 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/CFPGrowthPlus.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     5913 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-21 11:53:35.570622 pami-2023.7.21/PAMI/partialPeriodicFrequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/partialPeriodicFrequentPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-21 11:53:35.573292 pami-2023.7.21/PAMI/partialPeriodicFrequentPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    27316 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/partialPeriodicFrequentPattern/basic/GPFgrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    21102 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/partialPeriodicFrequentPattern/basic/PPF_DFS.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/partialPeriodicFrequentPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     5392 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/partialPeriodicFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-21 11:53:35.573557 pami-2023.7.21/PAMI/partialPeriodicPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/partialPeriodicPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-21 11:53:35.580349 pami-2023.7.21/PAMI/partialPeriodicPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    50844 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/partialPeriodicPattern/basic/GThreePGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     4195 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/partialPeriodicPattern/basic/Gabstract.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    24330 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/partialPeriodicPattern/basic/PPPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    17878 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/partialPeriodicPattern/basic/PPP_ECLAT.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/partialPeriodicPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     5572 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/partialPeriodicPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-21 11:53:35.580968 pami-2023.7.21/PAMI/partialPeriodicPattern/closed/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    21069 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/partialPeriodicPattern/closed/PPPClose.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/partialPeriodicPattern/closed/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     5595 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/partialPeriodicPattern/closed/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-21 11:53:35.581445 pami-2023.7.21/PAMI/partialPeriodicPattern/maximal/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    28482 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/partialPeriodicPattern/maximal/Max3PGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/partialPeriodicPattern/maximal/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     4261 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/partialPeriodicPattern/maximal/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-21 11:53:35.582549 pami-2023.7.21/PAMI/partialPeriodicPattern/timeSeries/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    26058 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/partialPeriodicPattern/timeSeries/PPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/partialPeriodicPattern/timeSeries/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     5550 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/partialPeriodicPattern/timeSeries/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-21 11:53:35.583066 pami-2023.7.21/PAMI/partialPeriodicPattern/topk/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/partialPeriodicPattern/topk/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     7837 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/partialPeriodicPattern/topk/abstract.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    17705 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/partialPeriodicPattern/topk/k3PMiner.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-21 11:53:35.583256 pami-2023.7.21/PAMI/partialPeriodicSpatialPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/partialPeriodicSpatialPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-21 11:53:35.583699 pami-2023.7.21/PAMI/partialPeriodicSpatialPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    19876 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/partialPeriodicSpatialPattern/basic/STEclat.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/partialPeriodicSpatialPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6165 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/partialPeriodicSpatialPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-21 11:53:35.583835 pami-2023.7.21/PAMI/periodicCorrelatedPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/periodicCorrelatedPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-21 11:53:35.584279 pami-2023.7.21/PAMI/periodicCorrelatedPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    27518 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/periodicCorrelatedPattern/basic/EPCPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/periodicCorrelatedPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6652 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/periodicCorrelatedPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-21 11:53:35.584432 pami-2023.7.21/PAMI/periodicFrequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/periodicFrequentPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-21 11:53:35.585627 pami-2023.7.21/PAMI/periodicFrequentPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    15591 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/periodicFrequentPattern/basic/PFECLAT.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    25146 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/periodicFrequentPattern/basic/PFPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    24942 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/periodicFrequentPattern/basic/PFPGrowthPlus.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    16311 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/periodicFrequentPattern/basic/PFPMC.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    33244 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/periodicFrequentPattern/basic/PSGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      726 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/periodicFrequentPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6525 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/periodicFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-21 11:53:35.586098 pami-2023.7.21/PAMI/periodicFrequentPattern/closed/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    21540 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/periodicFrequentPattern/closed/CPFPMiner.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/periodicFrequentPattern/closed/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6538 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/periodicFrequentPattern/closed/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-21 11:53:35.587274 pami-2023.7.21/PAMI/periodicFrequentPattern/cuda/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/periodicFrequentPattern/cuda/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6564 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/periodicFrequentPattern/cuda/abstract.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    19356 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/periodicFrequentPattern/cuda/cuGPFMiner.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    17474 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/periodicFrequentPattern/cuda/gPFMinerBit.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-21 11:53:35.587737 pami-2023.7.21/PAMI/periodicFrequentPattern/maximal/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    28740 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/periodicFrequentPattern/maximal/MaxPFGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/periodicFrequentPattern/maximal/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     7873 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/periodicFrequentPattern/maximal/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-21 11:53:35.587874 pami-2023.7.21/PAMI/periodicFrequentPattern/topk/
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-21 11:53:35.588304 pami-2023.7.21/PAMI/periodicFrequentPattern/topk/TopkPFP/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    18066 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/periodicFrequentPattern/topk/TopkPFP/TopkPFP.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/periodicFrequentPattern/topk/TopkPFP/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6898 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/periodicFrequentPattern/topk/TopkPFP/abstract.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/periodicFrequentPattern/topk/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-21 11:53:35.588702 pami-2023.7.21/PAMI/periodicFrequentPattern/topk/kPFPMiner/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/periodicFrequentPattern/topk/kPFPMiner/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     4583 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/periodicFrequentPattern/topk/kPFPMiner/abstract.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    17235 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/periodicFrequentPattern/topk/kPFPMiner/kPFPMiner.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-21 11:53:35.588869 pami-2023.7.21/PAMI/recurringPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/recurringPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-21 11:53:35.589261 pami-2023.7.21/PAMI/recurringPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    26300 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/recurringPattern/basic/RPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/recurringPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6632 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/recurringPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-21 11:53:35.589391 pami-2023.7.21/PAMI/relativeFrequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/relativeFrequentPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-21 11:53:35.589958 pami-2023.7.21/PAMI/relativeFrequentPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    26259 2023-07-20 11:24:18.000000 pami-2023.7.21/PAMI/relativeFrequentPattern/basic/RSFPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/relativeFrequentPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     4261 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/relativeFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-21 11:53:35.590090 pami-2023.7.21/PAMI/relativeHighUtilityPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/relativeHighUtilityPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-21 11:53:35.590478 pami-2023.7.21/PAMI/relativeHighUtilityPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    33570 2023-07-20 11:24:18.000000 pami-2023.7.21/PAMI/relativeHighUtilityPattern/basic/RHUIM.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/relativeHighUtilityPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     7391 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/relativeHighUtilityPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-21 11:53:35.590716 pami-2023.7.21/PAMI/sequence/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/sequence/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-21 11:53:35.590808 pami-2023.7.21/PAMI/sequentialPatternMining/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/sequentialPatternMining/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-21 11:53:35.591708 pami-2023.7.21/PAMI/sequentialPatternMining/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    41062 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/sequentialPatternMining/basic/SPADE.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/sequentialPatternMining/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6554 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/sequentialPatternMining/basic/abstract.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    22592 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/sequentialPatternMining/basic/prefixSpan.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-21 11:53:35.592122 pami-2023.7.21/PAMI/sequentialPatternMining/closed/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/sequentialPatternMining/closed/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6279 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/sequentialPatternMining/closed/abstract.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/sequentialPatternMining/closed/bide.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-21 11:53:35.592225 pami-2023.7.21/PAMI/stablePeriodicFrequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/stablePeriodicFrequentPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-21 11:53:35.592939 pami-2023.7.21/PAMI/stablePeriodicFrequentPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    16341 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/stablePeriodicFrequentPattern/basic/SPPEclat.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    25169 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/stablePeriodicFrequentPattern/basic/SPPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    17918 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/stablePeriodicFrequentPattern/basic/SPPGrowthDump.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/stablePeriodicFrequentPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     7258 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/stablePeriodicFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-21 11:53:35.593392 pami-2023.7.21/PAMI/stablePeriodicFrequentPattern/topK/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    26386 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/stablePeriodicFrequentPattern/topK/TSPIN.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/stablePeriodicFrequentPattern/topK/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     7177 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/stablePeriodicFrequentPattern/topK/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-21 11:53:35.593532 pami-2023.7.21/PAMI/uncertainFrequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/uncertainFrequentPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-21 11:53:35.595637 pami-2023.7.21/PAMI/uncertainFrequentPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    25974 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/uncertainFrequentPattern/basic/CUFPTree.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    26009 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/uncertainFrequentPattern/basic/PUFGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    18710 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/uncertainFrequentPattern/basic/TUFP.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    27060 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/uncertainFrequentPattern/basic/TubeP.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    27823 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/uncertainFrequentPattern/basic/TubeS.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    25507 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/uncertainFrequentPattern/basic/UFGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    19046 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/uncertainFrequentPattern/basic/UVECLAT.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/uncertainFrequentPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     4962 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/uncertainFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-21 11:53:35.595795 pami-2023.7.21/PAMI/uncertainPeriodicFrequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/uncertainPeriodicFrequentPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-21 11:53:35.596487 pami-2023.7.21/PAMI/uncertainPeriodicFrequentPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    31127 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/uncertainPeriodicFrequentPattern/basic/UPFPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    31329 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/uncertainPeriodicFrequentPattern/basic/UPFPGrowthPlus.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/uncertainPeriodicFrequentPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6551 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/uncertainPeriodicFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-21 11:53:35.596646 pami-2023.7.21/PAMI/weightedFrequentNeighbourhoodPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/weightedFrequentNeighbourhoodPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-21 11:53:35.597137 pami-2023.7.21/PAMI/weightedFrequentNeighbourhoodPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    27481 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/weightedFrequentNeighbourhoodPattern/basic/SWFPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/weightedFrequentNeighbourhoodPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6693 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/weightedFrequentNeighbourhoodPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-21 11:53:35.597351 pami-2023.7.21/PAMI/weightedFrequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/weightedFrequentPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-21 11:53:35.597830 pami-2023.7.21/PAMI/weightedFrequentPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    23852 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/weightedFrequentPattern/basic/WFIM.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/weightedFrequentPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6737 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/weightedFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-21 11:53:35.597989 pami-2023.7.21/PAMI/weightedFrequentRegularPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/weightedFrequentRegularPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-21 11:53:35.598436 pami-2023.7.21/PAMI/weightedFrequentRegularPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    27228 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/weightedFrequentRegularPattern/basic/WFRIMiner.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/weightedFrequentRegularPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     7555 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/weightedFrequentRegularPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-21 11:53:35.598589 pami-2023.7.21/PAMI/weightedUncertainFrequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/weightedUncertainFrequentPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-21 11:53:35.599062 pami-2023.7.21/PAMI/weightedUncertainFrequentPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    29070 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/weightedUncertainFrequentPattern/basic/WUFIM.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/weightedUncertainFrequentPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     4782 2023-07-20 11:14:51.000000 pami-2023.7.21/PAMI/weightedUncertainFrequentPattern/basic/abstract.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    39001 2023-07-21 11:53:35.600223 pami-2023.7.21/PKG-INFO
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    38368 2023-07-20 16:46:24.000000 pami-2023.7.21/README.md
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-21 11:53:35.599869 pami-2023.7.21/pami.egg-info/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    39001 2023-07-21 11:53:35.000000 pami-2023.7.21/pami.egg-info/PKG-INFO
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    14915 2023-07-21 11:53:35.000000 pami-2023.7.21/pami.egg-info/SOURCES.txt
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-21 11:53:35.000000 pami-2023.7.21/pami.egg-info/dependency_links.txt
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      109 2023-07-21 11:53:35.000000 pami-2023.7.21/pami.egg-info/requires.txt
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        5 2023-07-21 11:53:35.000000 pami-2023.7.21/pami.egg-info/top_level.txt
--rw-r--r--   0 udaykiranrage   (501) staff       (20)       38 2023-07-21 11:53:35.600506 pami-2023.7.21/setup.cfg
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     1263 2023-07-21 11:52:36.000000 pami-2023.7.21/setup.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.306139 pami-2023.7.7/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    35149 2023-06-03 08:26:58.000000 pami-2023.7.7/LICENSE
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.213420 pami-2023.7.7/PAMI/
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.213780 pami-2023.7.7/PAMI/AssociationRules/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/AssociationRules/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.215229 pami-2023.7.7/PAMI/AssociationRules/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     8001 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/AssociationRules/basic/ARWithConfidence.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     8038 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/AssociationRules/basic/ARWithLeverage.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     8085 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/AssociationRules/basic/ARWithLift.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    12384 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/AssociationRules/basic/RuleMiner.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/AssociationRules/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6547 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/AssociationRules/basic/abstract.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      139 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.215381 pami-2023.7.7/PAMI/correlatedPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/correlatedPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.216924 pami-2023.7.7/PAMI/correlatedPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    24417 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/correlatedPattern/basic/CPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    25824 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/correlatedPattern/basic/CPGrowthPlus.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/correlatedPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6055 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/correlatedPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.217089 pami-2023.7.7/PAMI/coveragePatterns/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/coveragePatterns/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.218352 pami-2023.7.7/PAMI/coveragePatterns/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    13995 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/coveragePatterns/basic/CMine.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    16075 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/coveragePatterns/basic/CPPG.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/coveragePatterns/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6938 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/coveragePatterns/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.219319 pami-2023.7.7/PAMI/extras/
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.221044 pami-2023.7.7/PAMI/extras/DF2DB/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     2178 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/extras/DF2DB/DF2DB.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     2243 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/extras/DF2DB/DF2DBPlus.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/DF2DB/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     1607 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/extras/DF2DB/createTDB.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     4185 2023-07-05 02:36:31.000000 pami-2023.7.7/PAMI/extras/DF2DB/denseDF2DB.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     4917 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/extras/DF2DB/denseDF2DBPlus.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     9942 2023-07-05 02:36:31.000000 pami-2023.7.7/PAMI/extras/DF2DB/denseDF2DB_dump.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     3607 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/extras/DF2DB/sparseDF2DB.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     3359 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/extras/DF2DB/sparseDF2DBPlus.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.221516 pami-2023.7.7/PAMI/extras/calculateMISValues/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/calculateMISValues/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     3741 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/calculateMISValues/usingBeta.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     3794 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/calculateMISValues/usingSD.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.223716 pami-2023.7.7/PAMI/extras/dbStats/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/dbStats/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    13043 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/extras/dbStats/fuzzyDatabaseStats.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    14661 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/extras/dbStats/temporalDatabaseStats.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     9364 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/extras/dbStats/transactionalDatabaseStats.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    13229 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/extras/dbStats/uncertainTemporalDatabaseStats.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    10040 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/extras/dbStats/uncertainTransactionalDatabaseStats.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    11775 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/extras/dbStats/utilityDatabaseStats.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.225281 pami-2023.7.7/PAMI/extras/fuzzyTransformation/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/fuzzyTransformation/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5195 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/fuzzyTransformation/abstract.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5925 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/fuzzyTransformation/temporalToFuzzy.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5919 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/fuzzyTransformation/transactionalToFuzzyTimeSeries.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5803 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/fuzzyTransformation/utilityToFuzzy.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.227961 pami-2023.7.7/PAMI/extras/generateDatabase/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/generateDatabase/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     2877 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/generateDatabase/generateSpatioTemporalDatabase.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     7092 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/extras/generateDatabase/generateTemporalDatabase.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     3444 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/extras/generateDatabase/generateTransactionalDatabase.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     3593 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/generateLatexGraphFile.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.231441 pami-2023.7.7/PAMI/extras/graph/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/graph/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     1656 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/graph/dataFrameInToFigures.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     2954 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/graph/generateLatexFileFromDataFrame.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     1167 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/graph/plotLineGraphFromDictionary.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     1753 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/graph/plotLineGraphsFromDataFrame.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     2203 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/graph/visualizePatterns.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.231576 pami-2023.7.7/PAMI/extras/image2Database/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/image2Database/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.231920 pami-2023.7.7/PAMI/extras/imageProcessing/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/imageProcessing/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     4582 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/imageProcessing/imagery2Databases.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.232234 pami-2023.7.7/PAMI/extras/neighbours/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/neighbours/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     2834 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/neighbours/findNeighboursUsingEuclidean.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     3031 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/plotPointOnMap.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     3214 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/plotPointOnMap_dump.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     2178 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/scatterPlotSpatialPoints.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.233791 pami-2023.7.7/PAMI/extras/syntheticDatabaseGenerator/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/extras/syntheticDatabaseGenerator/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     2280 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/extras/syntheticDatabaseGenerator/createSyntheticGeoreferentialTemporal.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     2257 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/extras/syntheticDatabaseGenerator/createSyntheticGeoreferentialTransactions.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     2509 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/extras/syntheticDatabaseGenerator/createSyntheticGeoreferentialUncertainTransaction.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     1887 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/extras/syntheticDatabaseGenerator/createSyntheticTemporal.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     1860 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/extras/syntheticDatabaseGenerator/createSyntheticTransactions.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     2124 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/extras/syntheticDatabaseGenerator/createSyntheticUncertainTemporal.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     2075 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/extras/syntheticDatabaseGenerator/createSyntheticUncertainTransactions.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     2265 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/extras/syntheticDatabaseGenerator/createSyntheticUtility.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     1827 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/topKPatterns.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      473 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/uncertaindb_convert.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.233937 pami-2023.7.7/PAMI/faultTolerantFrequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/faultTolerantFrequentPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.235273 pami-2023.7.7/PAMI/faultTolerantFrequentPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    14656 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/faultTolerantFrequentPattern/basic/FTApriori.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    21114 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/faultTolerantFrequentPattern/basic/FTFPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    14992 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/faultTolerantFrequentPattern/basic/VBFTMine.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/faultTolerantFrequentPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6691 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/faultTolerantFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.235589 pami-2023.7.7/PAMI/frequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/frequentPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.237534 pami-2023.7.7/PAMI/frequentPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    13124 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/frequentPattern/basic/Apriori.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    12531 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/frequentPattern/basic/ECLAT.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    13188 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/frequentPattern/basic/ECLATDiffset.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    13480 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/frequentPattern/basic/ECLATbitset.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    20324 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/frequentPattern/basic/FPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/frequentPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     7733 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/frequentPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.238433 pami-2023.7.7/PAMI/frequentPattern/closed/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    19874 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/frequentPattern/closed/CHARM.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/frequentPattern/closed/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6445 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/frequentPattern/closed/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.240335 pami-2023.7.7/PAMI/frequentPattern/cuda/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/frequentPattern/cuda/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6564 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/frequentPattern/cuda/abstract.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    13459 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/frequentPattern/cuda/cuApriori.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    14203 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/frequentPattern/cuda/cuAprioriBit.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    13085 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/frequentPattern/cuda/cuEclat.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    13942 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/frequentPattern/cuda/cuEclatBit.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5738 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/frequentPattern/cuda/cudaAprioriGCT.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     8648 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/frequentPattern/cuda/cudaAprioriTID.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5576 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/frequentPattern/cuda/cudaEclatGCT.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.241160 pami-2023.7.7/PAMI/frequentPattern/maximal/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    25097 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/frequentPattern/maximal/MaxFPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/frequentPattern/maximal/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6436 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/frequentPattern/maximal/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.242453 pami-2023.7.7/PAMI/frequentPattern/pyspark/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/frequentPattern/pyspark/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5603 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/frequentPattern/pyspark/abstract.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    13209 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/frequentPattern/pyspark/parallelApriori.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    11487 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/frequentPattern/pyspark/parallelECLAT.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    16147 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/frequentPattern/pyspark/parallelFPGrowth.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.243543 pami-2023.7.7/PAMI/frequentPattern/topk/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    14674 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/frequentPattern/topk/FAE.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/frequentPattern/topk/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     4575 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/frequentPattern/topk/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.243784 pami-2023.7.7/PAMI/frequentSpatialPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/frequentSpatialPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.244809 pami-2023.7.7/PAMI/frequentSpatialPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    20041 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/frequentSpatialPattern/basic/FSPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    19099 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/frequentSpatialPattern/basic/SpatialECLAT.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/frequentSpatialPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6680 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/frequentSpatialPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.245067 pami-2023.7.7/PAMI/fuzzyCorrelatedPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/fuzzyCorrelatedPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.245890 pami-2023.7.7/PAMI/fuzzyCorrelatedPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    25239 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/fuzzyCorrelatedPattern/basic/FCPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/fuzzyCorrelatedPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6635 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/fuzzyCorrelatedPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.246160 pami-2023.7.7/PAMI/fuzzyFrequentPatterns/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/fuzzyFrequentPatterns/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.247438 pami-2023.7.7/PAMI/fuzzyFrequentPatterns/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    20740 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/fuzzyFrequentPatterns/basic/FFIMiner.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    24624 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/fuzzyFrequentPatterns/basic/FFIMiner_old.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/fuzzyFrequentPatterns/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6450 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/fuzzyFrequentPatterns/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.247699 pami-2023.7.7/PAMI/fuzzyFrequentSpatialPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/fuzzyFrequentSpatialPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.248928 pami-2023.7.7/PAMI/fuzzyFrequentSpatialPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    23992 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/fuzzyFrequentSpatialPattern/basic/FFSPMiner.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    26791 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/fuzzyFrequentSpatialPattern/basic/FFSPMiner_old.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/fuzzyFrequentSpatialPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6580 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/fuzzyFrequentSpatialPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.249301 pami-2023.7.7/PAMI/fuzzyPartialPeriodicPatterns/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/fuzzyPartialPeriodicPatterns/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.249802 pami-2023.7.7/PAMI/fuzzyPartialPeriodicPatterns/irregularTimeSeries/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/fuzzyPartialPeriodicPatterns/irregularTimeSeries/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6449 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/fuzzyPartialPeriodicPatterns/irregularTimeSeries/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.250466 pami-2023.7.7/PAMI/fuzzyPeriodicFrequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/fuzzyPeriodicFrequentPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.251507 pami-2023.7.7/PAMI/fuzzyPeriodicFrequentPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    23521 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/fuzzyPeriodicFrequentPattern/basic/FPFPMiner.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    25345 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/fuzzyPeriodicFrequentPattern/basic/FPFPMiner_old.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/fuzzyPeriodicFrequentPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6668 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/fuzzyPeriodicFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.251792 pami-2023.7.7/PAMI/fuzzySpatialPeriodicFrequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/fuzzySpatialPeriodicFrequentPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.252874 pami-2023.7.7/PAMI/fuzzySpatialPeriodicFrequentPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    26817 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/fuzzySpatialPeriodicFrequentPattern/basic/FGPFPMiner.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    32216 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/fuzzySpatialPeriodicFrequentPattern/basic/FGPFPMiner_old.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/fuzzySpatialPeriodicFrequentPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6618 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/fuzzySpatialPeriodicFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.254340 pami-2023.7.7/PAMI/geoReferencedFrequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    28518 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/geoReferencedFrequentPattern/GFPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/geoReferencedFrequentPattern/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5007 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/geoReferencedFrequentPattern/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.255007 pami-2023.7.7/PAMI/geoReferencedPeriodicFrequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/geoReferencedPeriodicFrequentPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.255910 pami-2023.7.7/PAMI/geoReferencedPeriodicFrequentPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    19950 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/geoReferencedPeriodicFrequentPattern/basic/GPFPMiner.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/geoReferencedPeriodicFrequentPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6774 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/geoReferencedPeriodicFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.256357 pami-2023.7.7/PAMI/georeferencedFrequentSequencePattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/georeferencedFrequentSequencePattern/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6676 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/georeferencedFrequentSequencePattern/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.256630 pami-2023.7.7/PAMI/highUtilityFrequentPatterns/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/highUtilityFrequentPatterns/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.257531 pami-2023.7.7/PAMI/highUtilityFrequentPatterns/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    35401 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/highUtilityFrequentPatterns/basic/HUFIM.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/highUtilityFrequentPatterns/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6081 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/highUtilityFrequentPatterns/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.257812 pami-2023.7.7/PAMI/highUtilityFrequentSpatialPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/highUtilityFrequentSpatialPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.261273 pami-2023.7.7/PAMI/highUtilityFrequentSpatialPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    39910 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/highUtilityFrequentSpatialPattern/basic/SHUFIM.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/highUtilityFrequentSpatialPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6181 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/highUtilityFrequentSpatialPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.261803 pami-2023.7.7/PAMI/highUtilityPatterns/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/highUtilityPatterns/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.264098 pami-2023.7.7/PAMI/highUtilityPatterns/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    32747 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/highUtilityPatterns/basic/EFIM.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    24847 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/highUtilityPatterns/basic/HMiner.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    26567 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/highUtilityPatterns/basic/UPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/highUtilityPatterns/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5053 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/highUtilityPatterns/basic/abstract.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    16479 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/highUtilityPatterns/basic/efimParallel.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.265044 pami-2023.7.7/PAMI/highUtilityPatterns/parallel/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/highUtilityPatterns/parallel/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5053 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/highUtilityPatterns/parallel/abstract.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    16481 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/highUtilityPatterns/parallel/efimparallel.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.265480 pami-2023.7.7/PAMI/highUtilitySpatialPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/highUtilitySpatialPattern/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6718 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/highUtilitySpatialPattern/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.266895 pami-2023.7.7/PAMI/highUtilitySpatialPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    27632 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/highUtilitySpatialPattern/basic/HDSHUIM.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    34623 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/highUtilitySpatialPattern/basic/SHUIM.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/highUtilitySpatialPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5955 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/highUtilitySpatialPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.267687 pami-2023.7.7/PAMI/highUtilitySpatialPattern/topk/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    35216 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/highUtilitySpatialPattern/topk/TKSHUIM.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/highUtilitySpatialPattern/topk/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6625 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/highUtilitySpatialPattern/topk/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.267930 pami-2023.7.7/PAMI/localPeriodicPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/localPeriodicPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.269128 pami-2023.7.7/PAMI/localPeriodicPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    32664 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/localPeriodicPattern/basic/LPPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    21999 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/localPeriodicPattern/basic/LPPMBreadth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    21120 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/localPeriodicPattern/basic/LPPMDepth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/localPeriodicPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     8378 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/localPeriodicPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.269369 pami-2023.7.7/PAMI/multipleMinimumSupportBasedFrequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/multipleMinimumSupportBasedFrequentPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.270382 pami-2023.7.7/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    23034 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/CFPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    22318 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/CFPGrowthPlus.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5913 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.270633 pami-2023.7.7/PAMI/partialPeriodicFrequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/partialPeriodicFrequentPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.271619 pami-2023.7.7/PAMI/partialPeriodicFrequentPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    27316 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/partialPeriodicFrequentPattern/basic/GPFgrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    21102 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/partialPeriodicFrequentPattern/basic/PPF_DFS.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/partialPeriodicFrequentPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5392 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/partialPeriodicFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.271849 pami-2023.7.7/PAMI/partialPeriodicPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/partialPeriodicPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.273903 pami-2023.7.7/PAMI/partialPeriodicPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    50844 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/partialPeriodicPattern/basic/GThreePGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     4195 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/partialPeriodicPattern/basic/Gabstract.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    24330 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/partialPeriodicPattern/basic/PPPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    17878 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/partialPeriodicPattern/basic/PPP_ECLAT.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/partialPeriodicPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5572 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/partialPeriodicPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.274936 pami-2023.7.7/PAMI/partialPeriodicPattern/closed/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    21069 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/partialPeriodicPattern/closed/PPPClose.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/partialPeriodicPattern/closed/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5595 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/partialPeriodicPattern/closed/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.275960 pami-2023.7.7/PAMI/partialPeriodicPattern/maximal/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    28482 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/partialPeriodicPattern/maximal/Max3PGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/partialPeriodicPattern/maximal/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     4261 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/partialPeriodicPattern/maximal/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.276849 pami-2023.7.7/PAMI/partialPeriodicPattern/timeSeries/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    26058 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/partialPeriodicPattern/timeSeries/PPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/partialPeriodicPattern/timeSeries/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5550 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/partialPeriodicPattern/timeSeries/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.277438 pami-2023.7.7/PAMI/partialPeriodicPattern/topk/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/partialPeriodicPattern/topk/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     7837 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/partialPeriodicPattern/topk/abstract.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    17705 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/partialPeriodicPattern/topk/k3PMiner.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.277755 pami-2023.7.7/PAMI/partialPeriodicSpatialPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/partialPeriodicSpatialPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.278324 pami-2023.7.7/PAMI/partialPeriodicSpatialPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    19876 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/partialPeriodicSpatialPattern/basic/STEclat.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/partialPeriodicSpatialPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6165 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/partialPeriodicSpatialPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.278541 pami-2023.7.7/PAMI/periodicCorrelatedPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/periodicCorrelatedPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.279293 pami-2023.7.7/PAMI/periodicCorrelatedPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    27518 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/periodicCorrelatedPattern/basic/EPCPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/periodicCorrelatedPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6652 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/periodicCorrelatedPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.279512 pami-2023.7.7/PAMI/periodicFrequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/periodicFrequentPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.281487 pami-2023.7.7/PAMI/periodicFrequentPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    15591 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/periodicFrequentPattern/basic/PFECLAT.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    25146 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/periodicFrequentPattern/basic/PFPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    24942 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/periodicFrequentPattern/basic/PFPGrowthPlus.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    16311 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/periodicFrequentPattern/basic/PFPMC.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    33244 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/periodicFrequentPattern/basic/PSGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      726 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/periodicFrequentPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6525 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/periodicFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.282417 pami-2023.7.7/PAMI/periodicFrequentPattern/closed/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    21540 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/periodicFrequentPattern/closed/CPFPMiner.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/periodicFrequentPattern/closed/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6538 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/periodicFrequentPattern/closed/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.283856 pami-2023.7.7/PAMI/periodicFrequentPattern/cuda/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/periodicFrequentPattern/cuda/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6564 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/periodicFrequentPattern/cuda/abstract.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    19727 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/periodicFrequentPattern/cuda/cuGPFMiner.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    17474 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/periodicFrequentPattern/cuda/gPFMinerBit.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.284826 pami-2023.7.7/PAMI/periodicFrequentPattern/maximal/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    28740 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/periodicFrequentPattern/maximal/MaxPFGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/periodicFrequentPattern/maximal/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     7873 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/periodicFrequentPattern/maximal/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.285069 pami-2023.7.7/PAMI/periodicFrequentPattern/topk/
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.285761 pami-2023.7.7/PAMI/periodicFrequentPattern/topk/TopkPFP/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    18066 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/periodicFrequentPattern/topk/TopkPFP/TopkPFP.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/periodicFrequentPattern/topk/TopkPFP/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6898 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/periodicFrequentPattern/topk/TopkPFP/abstract.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/periodicFrequentPattern/topk/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.286394 pami-2023.7.7/PAMI/periodicFrequentPattern/topk/kPFPMiner/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/periodicFrequentPattern/topk/kPFPMiner/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     4583 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/periodicFrequentPattern/topk/kPFPMiner/abstract.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    17235 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/periodicFrequentPattern/topk/kPFPMiner/kPFPMiner.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.286673 pami-2023.7.7/PAMI/recurringPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/recurringPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.287396 pami-2023.7.7/PAMI/recurringPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    26300 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/recurringPattern/basic/RPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/recurringPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6632 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/recurringPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.287636 pami-2023.7.7/PAMI/relativeFrequentPatterns/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/relativeFrequentPatterns/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.288407 pami-2023.7.7/PAMI/relativeFrequentPatterns/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    26260 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/relativeFrequentPatterns/basic/RSFPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/relativeFrequentPatterns/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     4261 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/relativeFrequentPatterns/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.288643 pami-2023.7.7/PAMI/relativeHighUtilityPatterns/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/relativeHighUtilityPatterns/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.289267 pami-2023.7.7/PAMI/relativeHighUtilityPatterns/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    33573 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/relativeHighUtilityPatterns/basic/RHUIM.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/relativeHighUtilityPatterns/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     7391 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/relativeHighUtilityPatterns/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.289510 pami-2023.7.7/PAMI/sequentialPatternMining/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/sequentialPatternMining/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.290707 pami-2023.7.7/PAMI/sequentialPatternMining/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    41062 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/sequentialPatternMining/basic/SPADE.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/sequentialPatternMining/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6554 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/sequentialPatternMining/basic/abstract.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    22592 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/sequentialPatternMining/basic/prefixSpan.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.291328 pami-2023.7.7/PAMI/sequentialPatternMining/closed/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/sequentialPatternMining/closed/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6279 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/sequentialPatternMining/closed/abstract.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/sequentialPatternMining/closed/bide.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.291420 pami-2023.7.7/PAMI/stablePeriodicFrequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/stablePeriodicFrequentPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.292688 pami-2023.7.7/PAMI/stablePeriodicFrequentPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    16341 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/stablePeriodicFrequentPattern/basic/SPPEclat.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    25169 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/stablePeriodicFrequentPattern/basic/SPPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    17918 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/stablePeriodicFrequentPattern/basic/SPPGrowthDump.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/stablePeriodicFrequentPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     7258 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/stablePeriodicFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.293628 pami-2023.7.7/PAMI/stablePeriodicFrequentPattern/topK/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    26386 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/stablePeriodicFrequentPattern/topK/TSPIN.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/stablePeriodicFrequentPattern/topK/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     7177 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/stablePeriodicFrequentPattern/topK/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.293913 pami-2023.7.7/PAMI/streams/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/streams/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.294014 pami-2023.7.7/PAMI/streams/frequentPatterns/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/streams/frequentPatterns/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.294626 pami-2023.7.7/PAMI/streams/frequentPatterns/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    31851 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/streams/frequentPatterns/basic/FPStream.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/streams/frequentPatterns/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     7792 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/streams/frequentPatterns/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.295292 pami-2023.7.7/PAMI/streams/highUtility/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    29434 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/streams/highUtility/HUPMS.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    33678 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/streams/highUtility/SHUGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/streams/highUtility/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5195 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/streams/highUtility/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.295424 pami-2023.7.7/PAMI/uncertainFrequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/uncertainFrequentPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.298349 pami-2023.7.7/PAMI/uncertainFrequentPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    25974 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/uncertainFrequentPattern/basic/CUFPTree.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    26009 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/uncertainFrequentPattern/basic/PUFGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    18710 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/uncertainFrequentPattern/basic/TUFP.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    27060 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/uncertainFrequentPattern/basic/TubeP.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    27823 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/uncertainFrequentPattern/basic/TubeS.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    25507 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/uncertainFrequentPattern/basic/UFGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    19046 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/uncertainFrequentPattern/basic/UVECLAT.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/uncertainFrequentPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     4962 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/uncertainFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.298597 pami-2023.7.7/PAMI/uncertainPeriodicFrequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/uncertainPeriodicFrequentPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.299797 pami-2023.7.7/PAMI/uncertainPeriodicFrequentPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    31127 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/uncertainPeriodicFrequentPattern/basic/UPFPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    31329 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/uncertainPeriodicFrequentPattern/basic/UPFPGrowthPlus.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/uncertainPeriodicFrequentPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6551 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/uncertainPeriodicFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.300033 pami-2023.7.7/PAMI/weightedFrequentNeighbourhoodPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/weightedFrequentNeighbourhoodPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.300646 pami-2023.7.7/PAMI/weightedFrequentNeighbourhoodPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    27481 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/weightedFrequentNeighbourhoodPattern/basic/SWFPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/weightedFrequentNeighbourhoodPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6693 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/weightedFrequentNeighbourhoodPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.300913 pami-2023.7.7/PAMI/weightedFrequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/weightedFrequentPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.301700 pami-2023.7.7/PAMI/weightedFrequentPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    23852 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/weightedFrequentPattern/basic/WFIM.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/weightedFrequentPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6737 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/weightedFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.302005 pami-2023.7.7/PAMI/weightedFrequentRegularPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/weightedFrequentRegularPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.302627 pami-2023.7.7/PAMI/weightedFrequentRegularPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    27228 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/weightedFrequentRegularPattern/basic/WFRIMiner.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/weightedFrequentRegularPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     7555 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/weightedFrequentRegularPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.303017 pami-2023.7.7/PAMI/weightedUncertainFrequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/weightedUncertainFrequentPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.304367 pami-2023.7.7/PAMI/weightedUncertainFrequentPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    29070 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/weightedUncertainFrequentPattern/basic/WUFIM.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/weightedUncertainFrequentPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     4782 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/weightedUncertainFrequentPattern/basic/abstract.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    35126 2023-07-18 12:23:34.305978 pami-2023.7.7/PKG-INFO
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    34480 2023-07-07 08:24:43.000000 pami-2023.7.7/README.md
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.305715 pami-2023.7.7/pami.egg-info/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    35126 2023-07-18 12:23:34.000000 pami-2023.7.7/pami.egg-info/PKG-INFO
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    15099 2023-07-18 12:23:34.000000 pami-2023.7.7/pami.egg-info/SOURCES.txt
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-18 12:23:34.000000 pami-2023.7.7/pami.egg-info/dependency_links.txt
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      102 2023-07-18 12:23:34.000000 pami-2023.7.7/pami.egg-info/requires.txt
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        5 2023-07-18 12:23:34.000000 pami-2023.7.7/pami.egg-info/top_level.txt
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)       38 2023-07-18 12:23:34.306190 pami-2023.7.7/setup.cfg
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     1289 2023-07-18 12:22:32.000000 pami-2023.7.7/setup.py
```

### Comparing `pami-2023.7.21/LICENSE` & `pami-2023.7.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/AssociationRules/basic/ARWithConfidence.py` & `pami-2023.7.7/PAMI/AssociationRules/basic/ARWithConfidence.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,54 +1,54 @@
 from PAMI.AssociationRules.basic import abstract as _ab
 
 
 class Confidence:
 
-    def __init__(self, patterns, singleItems, minConf):
+    def __init__(self, patterns, singleItems, threshold):
         """
         :param inputFile: input file name or path
         :type inputFile: str
         :param sep:
         """
         self._frequentPatterns = patterns
         self._singleItems = singleItems
-        self._minConf = minConf
+        self._threshold = threshold
         self._finalPatterns = {}
 
     def _generation(self, prefix, suffix):
         if len(suffix) == 1:
-            conf = self._generateWithConfidence(prefix, suffix[0])
+            conf = self._generaeWithConfidence(prefix, suffix[0])
         for i in range(len(suffix)):
             suffix1 = suffix[:i] + suffix[i + 1:]
             prefix1 = prefix + ' ' + suffix[i]
             for j in range(i + 1, len(suffix)):
-                self._generateWithConfidence(prefix + ' ' + suffix[i], suffix[j])
+                self._generaeWithConfidence(prefix + ' ' + suffix[i], suffix[j])
                 # self._generation(prefix+ ' ' +suffix[i], suffix[i+1:])
             self._generation(prefix1, suffix1)
 
-    def _generateWithConfidence(self, lhs, rhs):
+    def _generaeWithConfidence(self, lhs, rhs):
         s = lhs + '\t' + rhs
         if self._frequentPatterns.get(s) == None:
             return 0
         minimum = self._frequentPatterns[s]
         conflhs = minimum / self._frequentPatterns[lhs]
         confrhs = minimum / self._frequentPatterns[rhs]
-        if conflhs >= self._minConf:
+        if conflhs >= self._threshold:
             s1 = lhs + '->' + rhs
             self._finalPatterns[s1] = conflhs
-        if confrhs >= self._minConf:
+        if confrhs >= self._threshold:
             s1 = rhs + '->' + lhs
             self._finalPatterns[s1] = confrhs
 
     def run(self):
         for i in range(len(self._singleItems)):
             suffix = self._singleItems[:i] + self._singleItems[i + 1:]
             prefix = self._singleItems[i]
             for j in range(i + 1, len(self._singleItems)):
-                self._generateWithConfidence(self._singleItems[i], self._singleItems[j])
+                self._generaeWithConfidence(self._singleItems[i], self._singleItems[j])
             self._generation(prefix, suffix)
 
 
 class ARWithConfidence:
     """
         temporalDatabaseStats is class to get stats of database.
         
@@ -117,15 +117,15 @@
                     print("File Not Found")
                     quit()
         return k
 
     def startMine(self):
         self._startTime = _ab._time.time()
         k = self._readPatterns()
-        a = Confidence(self._frequentPatterns, k, self._minConf)
+        a = Confidence(self._frequentPatterns, k, self._threshold)
         a.run()
         self._finalPatterns = a._finalPatterns
         self._endTime = _ab._time.time()
         process = _ab._psutil.Process(_ab._os.getpid())
         self._memoryUSS = float()
         self._memoryRSS = float()
         self._memoryUSS = process.memory_full_info().uss
@@ -205,12 +205,12 @@
         _ap.startMine()
         print("Total number of Association Rules:", len(_ap.getPatterns()))
         _ap.save(_ab._sys.argv[2])
         print("Total Memory in USS:", _ap.getMemoryUSS())
         print("Total Memory in RSS", _ap.getMemoryRSS())
         print("Total ExecutionTime in ms:", _ap.getRuntime())
     else:
-        # _ap = ARWithConfidence('patterns.txt', 0.8, '\t')
-        # _ap.startMine()
-        # _ap.save('output.txt')
-        # _ap.printResults()
-        print("Error! The number of input parameters do not match the total number of parameters provided")
+        _ap = ARWithConfidence('patterns.txt', 0.8, '\t')
+        _ap.startMine()
+        _ap.save('output.txt')
+        _ap.printResults()
+        print("Error! The number of input parameters do not match the total number of parameters provided")
```

### Comparing `pami-2023.7.21/PAMI/AssociationRules/basic/ARWithLeverage.py` & `pami-2023.7.7/PAMI/AssociationRules/basic/ARWithLeverage.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from PAMI.AssociationRules.basic import abstract as _ab
 
 
 class Leverage:
 
-    def __init__(self, patterns, singleItems, minConf):
+    def __init__(self, patterns, singleItems, threshold):
         """
         :param inputFile: input file name or path
         :type inputFile: str
         :param sep:
         """
         self._frequentPatterns = patterns
         self._singleItems = singleItems
-        self._minConf = minConf
+        self._threshold = threshold
         self._finalPatterns = {}
 
     def _generation(self, prefix, suffix):
         if len(suffix) == 1:
             conf = self._generateWithLeverage(prefix, suffix[0])
         for i in range(len(suffix)):
             suffix1 = suffix[:i] + suffix[i + 1:]
@@ -29,18 +29,18 @@
         if self._frequentPatterns.get(s) == None:
             return 0
         minimum = self._frequentPatterns[s]
         conflhs = minimum / self._frequentPatterns[lhs]
         confrhs = minimum / self._frequentPatterns[rhs]
         liftlhs = conflhs - self._frequentPatterns[rhs] * self._frequentPatterns[lhs]
         rightrhs = confrhs - self._frequentPatterns[lhs] * self._frequentPatterns[rhs]
-        if liftlhs >= self._minConf:
+        if liftlhs >= self._threshold:
             s1 = lhs + '->' + rhs
             self._finalPatterns[s1] = conflhs
-        if rightrhs >= self._minConf:
+        if rightrhs >= self._threshold:
             s1 = rhs + '->' + lhs
             self._finalPatterns[s1] = confrhs
 
     def run(self):
         for i in range(len(self._singleItems)):
             suffix = self._singleItems[:i] + self._singleItems[i + 1:]
             prefix = self._singleItems[i]
@@ -63,22 +63,22 @@
         threshold: condition to satisfy
             int
         Methods:
         -------
         startMine()
     """
 
-    def __init__(self, iFile, minConf, sep):
+    def __init__(self, iFile, threshold, sep):
         """
         :param inputFile: input file name or path
         :type inputFile: str
         :param sep:
         """
         self._iFile = iFile
-        self._minConf = minConf
+        self._threshold = threshold
         self._finalPatterns = {}
         self._sep = sep
 
     def _readPatterns(self):
         self._frequentPatterns = {}
         k = []
         if isinstance(self._iFile, _ab._pd.DataFrame):
@@ -118,15 +118,15 @@
                     print("File Not Found")
                     quit()
         return k
 
     def startMine(self):
         self._startTime = _ab._time.time()
         k = self._readPatterns()
-        a = Leverage(self._frequentPatterns, k, self._minConf)
+        a = Leverage(self._frequentPatterns, k, self._threshold)
         a.run()
         self._finalPatterns = a._finalPatterns
         self._endTime = _ab._time.time()
         process = _ab._psutil.Process(_ab._os.getpid())
         self._memoryUSS = float()
         self._memoryRSS = float()
         self._memoryUSS = process.memory_full_info().uss
@@ -206,14 +206,14 @@
         _ap.startMine()
         print("Total number of Association Rules:", len(_ap.getPatterns()))
         _ap.save(_ab._sys.argv[2])
         print("Total Memory in USS:", _ap.getMemoryUSS())
         print("Total Memory in RSS", _ap.getMemoryRSS())
         print("Total ExecutionTime in ms:", _ap.getRuntime())
     else:
-        # _ap = ARWithLeverage('patterns.txt', 0.8, '\t')
-        # _ap.startMine()
-        # _ap.save('output.txt')
-        # _ap.printResults()
+        _ap = ARWithLeverage('patterns.txt', 0.8, '\t')
+        _ap.startMine()
+        _ap.save('output.txt')
+        _ap.printResults()
         print("Error! The number of input parameters do not match the total number of parameters provided")
```

### Comparing `pami-2023.7.21/PAMI/AssociationRules/basic/ARWithLift.py` & `pami-2023.7.7/PAMI/AssociationRules/basic/ARWithLift.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from PAMI.AssociationRules.basic import abstract as _ab
 
 class Lift:
 
-    def __init__(self, patterns, singleItems, minConf):
+    def __init__(self, patterns, singleItems, threshold):
         """
         :param inputFile: input file name or path
         :type inputFile: str
         :param sep:
         """
         self._frequentPatterns = patterns
         self._singleItems = singleItems
-        self._minConf = minConf
+        self._threshold = threshold
         self._finalPatterns = {}
 
     def _generation(self, prefix, suffix):
         if len(suffix) == 1:
             self._generateWithLift(prefix, suffix[0])
         for i in range(len(suffix)):
             suffix1 = suffix[:i] + suffix[i + 1:]
@@ -29,18 +29,18 @@
         if self._frequentPatterns.get(s) == None:
             return 0
         minimum = self._frequentPatterns[s]
         conflhs = minimum / self._frequentPatterns[lhs]
         confrhs = minimum / self._frequentPatterns[rhs]
         liftlhs = conflhs / self._frequentPatterns[rhs] * self._frequentPatterns[lhs]
         rightrhs = confrhs / self._frequentPatterns[lhs] * self._frequentPatterns[rhs]
-        if liftlhs >= self._minConf:
+        if liftlhs >= self._threshold:
             s1 = lhs + '->' + rhs
             self._finalPatterns[s1] = conflhs
-        if rightrhs >= self._minConf:
+        if rightrhs >= self._threshold:
             s1 = rhs + '->' + lhs
             self._finalPatterns[s1] = confrhs
 
     def run(self):
         for i in range(len(self._singleItems)):
             suffix = self._singleItems[:i] + self._singleItems[i + 1:]
             prefix = self._singleItems[i]
@@ -61,22 +61,22 @@
         threshold: condition to satisfy
             int
         Methods:
         -------
         startMine()
     """
 
-    def __init__(self, iFile, minConf, sep):
+    def __init__(self, iFile, threshold, sep):
         """
         :param inputFile: input file name or path
         :type inputFile: str
         :param sep:
         """
         self._iFile = iFile
-        self._minConf = minConf
+        self._threshold = threshold
         self._finalPatterns = {}
         self._sep = sep
 
     def _readPatterns(self):
         self._frequentPatterns = {}
         k = []
         if isinstance(self._iFile, _ab._pd.DataFrame):
@@ -116,15 +116,15 @@
                     print("File Not Found")
                     quit()
         return k
 
     def startMine(self):
         self._startTime = _ab._time.time()
         k = self._readPatterns()
-        a = Lift(self._frequentPatterns, k, self._minConf)
+        a = Lift(self._frequentPatterns, k, self._threshold)
         a.run()
         self._finalPatterns = a._finalPatterns
         self._endTime = _ab._time.time()
         process = _ab._psutil.Process(_ab._os.getpid())
         self._memoryUSS = float()
         self._memoryRSS = float()
         self._memoryUSS = process.memory_full_info().uss
@@ -208,8 +208,8 @@
         print("Total Memory in RSS", _ap.getMemoryRSS())
         print("Total ExecutionTime in ms:", _ap.getRuntime())
     else:
         _ap = ARWithLift('patterns.txt', 0.8, '\t')
         _ap.startMine()
         _ap.save('output.txt')
         _ap.printResults()
-        print("Error! The number of input parameters do not match the total number of parameters provided")
+        print("Error! The number of input parameters do not match the total number of parameters provided")
```

### Comparing `pami-2023.7.21/PAMI/AssociationRules/basic/RuleMiner.py` & `pami-2023.7.7/PAMI/AssociationRules/basic/RuleMiner.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/AssociationRules/basic/abstract.py` & `pami-2023.7.7/PAMI/frequentPattern/maximal/abstract.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,31 +22,29 @@
 #      but WITHOUT ANY WARRANTY; without even the implied warranty of
 #      MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #      GNU General Public License for more details.
 #
 #      You should have received a copy of the GNU General Public License
 #      along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
-# from abc import ABC as _ABC, abstractmethod as _abstractmethod
 from abc import ABC as _ABC, abstractmethod as _abstractmethod
 import time as _time
 import csv as _csv
 import pandas as _pd
 from collections import defaultdict as _defaultdict
 from itertools import combinations as _c
 import os as _os
 import os.path as _ospath
 import psutil as _psutil
 import sys as _sys
 import validators as _validators
 from urllib.request import urlopen as _urlopen
-import functools as _functools
 
 
-class _AssociationRules(_ABC):
+class _frequentPatterns(_ABC):
     """ This abstract base class defines the variables and methods that every frequent pattern mining algorithm must
         employ in PAMI
 
 
        Attributes:
        ----------
         iFile : str
@@ -87,36 +85,37 @@
         getMemoryRSS()
             This function outputs the total amount of RSS memory consumed by a mining algorithm
         getRuntime()
             This function outputs the total runtime of a mining algorithm
 
     """
 
-    def __init__(self, iFile, minConf, sep="\t"):
+    def __init__(self, iFile, minSup, sep="\t"):
         """
         :param iFile: Input file name or path of the input file
         :type iFile: str or DataFrame
         :param minSup: The user can specify minSup either in count or proportion of database size.
             If the program detects the data type of minSup is integer, then it treats minSup is expressed in count.
             Otherwise, it will be treated as float.
             Example: minSup=10 will be treated as integer, while minSup=10.0 will be treated as float
         :type minSup: int or float or str
         :param sep: separator used to distinguish items from each other. The default separator is tab space. However, users can override the default separator
         :type sep: str
         """
 
         self._iFile = iFile
         self._sep = sep
-        self._minConf = minConf
+        self._minSup = minSup
         self._finalPatterns = {}
         self._oFile = str()
-        self._memoryUSS = float()
-        self._memoryRSS = float()
         self._startTime = float()
         self._endTime = float()
+        self._memoryRSS = float()
+        self._memoryUSS = float()
+
 
     @_abstractmethod
     def startMine(self):
         """Code for the mining process will start from this function"""
 
         pass
 
@@ -150,18 +149,19 @@
 
     @_abstractmethod
     def getMemoryRSS(self):
         """Total amount of RSS memory consumed by the program will be retrieved from this function"""
 
         pass
 
+
     @_abstractmethod
     def getRuntime(self):
         """Total amount of runtime taken by the program will be retrieved from this function"""
 
         pass
 
     @_abstractmethod
     def printResults(self):
-        """ To print result of the execution"""
+        """To print the statistics."""
 
         pass
```

### Comparing `pami-2023.7.21/PAMI/correlatedPattern/__init__.py` & `pami-2023.7.7/PAMI/correlatedPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/correlatedPattern/basic/CPGrowth.py` & `pami-2023.7.7/PAMI/correlatedPattern/basic/CPGrowth.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-# CPGrowth is one of the fundamental algorithm to discover correlated patterns in a transactional database.
+# CPGrowth is one of the fundamental algorithm to discover correlated frequent patterns in a transactional database.
 #
 # **Importing this algorithm into a python program**
 # --------------------------------------------------------
 #
 #
-#             from PAMI.correlatedPattern.basic import CPGrowth as alg
+#             from PAMI.correlatedSpatialPattern.basic import CSPGrowth as alg
 #
-#             obj = alg.CPGrowth(iFile, minSup, minAllConf, sep)
+#             obj = alg.CSPGrowth(iFile, frequentPatternsFile, measure, threshold)
 #
 #             obj.startMine()
 #
 #             Rules = obj.getPatterns()
 #
 #             print("Total number of  Patterns:", len(Patterns))
 #
@@ -53,15 +53,15 @@
 
 """
 
 from PAMI.correlatedPattern.basic import abstract as _ab
 
 class _Node:
     """
-    A class used to represent the node of correlatedPatternTree
+    A class used to represent the node of frequentPatternTree
 
 
     Attributes :
     ----------
         itemId : int
             storing item of a node
         counter : int
@@ -73,15 +73,15 @@
         nodeLink : node
             Points to the node with same itemId
 
     Methods :
     -------
 
         getChild(itemName)
-            returns the node with same itemName from correlatedPatternTree
+            returns the node with same itemName from frequentPatternTree
     """
 
     def __init__(self):
         self.itemId = -1
         self.counter = 1
         self.parent = None
         self.child = []
@@ -92,15 +92,15 @@
             if i.itemId == id1:
                 return i
         return None
 
 
 class _Tree:
     """
-        A class used to represent the correlatedPatternGrowth tree structure
+        A class used to represent the frequentPatternGrowth tree structure
 
     Attributes :
     ----------
         headerList : list
             storing the list of items in tree sorted in ascending of their supports
         mapItemNodes : dictionary
             storing the nodes with same item name
@@ -111,34 +111,34 @@
 
 
     Methods :
     -------
         createHeaderList(items,minSup)
             takes items only which are greater than minSup and sort the items in ascending order
         addTransaction(transaction)
-            creating transaction as a branch in correlatedPatternTree
+            creating transaction as a branch in frequentPatternTree
         fixNodeLinks(item,newNode)
             To create the link for nodes with same item
         printTree(Node)
-            gives the details of node in correlatedPatternGrowth tree
+            gives the details of node in frequentPatternGrowth tree
         addPrefixPath(prefix,port,minSup)
            It takes the items in prefix pattern whose support is >=minSup and construct a subtree
     """
 
     def __init__(self):
         self.headerList = []
         self.mapItemNodes = {}
         self.mapItemLastNodes = {}
         self.root = _Node()
 
     def addTransaction(self, transaction):
         """
         adding transaction into tree
 
-        :param transaction : it represents a single transaction in a database
+        :param transaction : it represents the one transactions in database
         :type transaction : list
         """
 
         current = self.root
         for i in transaction:
             child = current.getChild(i)
             if child is None:
@@ -150,36 +150,37 @@
                 current = newNode
             else:
                 child.counter += 1
                 current = child
 
     def fixNodeLinks(self, item, newNode):
         """
-        Fixing node link for the newNode that inserted into correlatedPatternTree
+        Fixing node link for the newNode that inserted into frequentPatternTree
 
         :param item: it represents the item of newNode
         :type item : int
-        :param newNode : it represents the newNode that inserted in correlatedPatternTree
+        :param newNode : it represents the newNode that inserted in frequentPatternTree
         :type newNode : Node
 
         """
         if item in self.mapItemLastNodes.keys():
             lastNode = self.mapItemLastNodes[item]
             lastNode.nodeLink = newNode
         self.mapItemLastNodes[item] = newNode
         if item not in self.mapItemNodes.keys():
             self.mapItemNodes[item] = newNode
 
     def printTree(self, root):
         """
-        This method is to find the details of parent, children, and support of a Node
+        This method is to find the details of parent,children,support of Node
 
-        :param root: it represents the Node in correlatedPatternTree
+        :param root: it represents the Node in frequentPatternTree
         :type root: Node
 
+        
         """
 
         if root.child is None:
             return
         else:
             for i in root.child:
                 print(i.itemId, i.counter, i.parent.itemId)
@@ -200,15 +201,15 @@
             if y >= minSup:
                 t1.append(x)
         itemSetBuffer = [k for k, v in sorted(mapSupport.items(), key=lambda x: x[1], reverse=True)]
         self.headerList = [i for i in t1 if i in itemSetBuffer]
 
     def addPrefixPath(self, prefix, mapSupportBeta, minSup):
         """
-        To construct the conditional tree with prefix paths of a node in correlatedPatternTree
+        To construct the conditional tree with prefix paths of a node in frequentPatternTree
 
         :param prefix : it represents the prefix items of a Node
         :type prefix : list
         :param mapSupportBeta : it represents the items with their supports
         :param mapSupportBeta : dictionary
         :param minSup : to check the item meets with minSup
         :param minSup : float
@@ -231,32 +232,26 @@
                 else:
                     child.counter += pathCount
                     current = child
 
 
 class CPGrowth(_ab._correlatedPatterns):
     """
-    :Description: CPGrowth is one of the fundamental algorithm to discover correlated  patterns in a
-    transactional database. It is based on the traditional FP-Growth algorithm. This algorithm uses depth-first
-    search technique to find all correlated patterns in a transactional database.
+    :Description: CPGrowth is one of the fundamental algorithm to discover correlated frequent patterns in a transactional database. It is based on the traditional Fpgrowth Algorithm, this algorithm uses breadth-first search technique to find the correlated Frequent patterns in transactional database.
 
     :Reference: Lee, Y.K., Kim, W.Y., Cao, D., Han, J. (2003). CoMine: efficient mining of correlated patterns. In ICDM (pp. 581–584).
-
     :param  iFile: str :
-                   Name of the Input file to mine complete set of correlated patterns
+                   Name of the Input file to mine complete set of frequent patterns
     :param  oFile: str :
-                   Name of the output file to store complete set of correlated patterns
+                   Name of the output file to store complete set of frequent patterns
     :param  minSup: int or float or str :
-                   The user can specify minSup either in count or proportion of database size. If the program detects
-                   the data type of minSup is integer, then it treats minSup is expressed in count.
-    :param minAllConf: float :
-                    The user can specify minAllConf values within the range (0, 1).
+                   The user can specify minSup either in count or proportion of database size. If the program detects the data type of minSup is integer, then it treats minSup is expressed in count.
+    :param minAllConf: str : Name of Neighbourhood file name
     :param  sep: str :
-                   This variable is used to distinguish items from one another in a transaction. The default seperator
-                   is tab space. However, the users can override their default separator.
+                   This variable is used to distinguish items from one another in a transaction. The default seperator is tab space. However, the users can override their default separator.
 
 
 
 
 
     :Attributes:
 
@@ -290,37 +285,37 @@
            it represents the constraint for pattern length
 
 
     **Methods to execute code on terminal**
     ----------------------------------------
 
             Format:
-                      >>> python3 CPGrowth.py <inputFile> <outputFile> <minSup> <minAllConf> <sep>
+                      >>> python3 CSPGrowth.py <inputFile> <outputFile> <neighbourFile> <minSup> <minAllConf> <sep>
             Example:
-                      >>>  python3 CPGrowth.py sampleTDB.txt output.txt 0.25 0.2
+                      >>>  python3 CSPGrowth.py sampleTDB.txt output.txt sampleN.txt 0.25 0.2
 
                      .. note:: minSup will be considered in percentage of database transactions
 
     **Importing this algorithm into a python program**
     --------------------------------------------------------------------------------
     .. code-block:: python
 
-            from PAMI.correlatedPattern.basic import CPGrowth as alg
+            from PAMI.correlatedSpatialPattern.basic import CSPGrowth as alg
 
-            obj = alg.CPGrowth(iFile, minSup, minAllConf,sep)
+            obj = alg.CSPGrowth(iFile, frequentPatternsFile, measure, threshold)
 
             obj.startMine()
 
-            patterns = obj.getPatterns()
+            Rules = obj.getPatterns()
 
-            print("Total number of  Patterns:", len(patterns))
+            print("Total number of  Patterns:", len(Patterns))
 
             obj.savePatterns(oFile)
 
-            df = obj.getPatternsAsDataFrame()
+            Df = obj.getPatternsAsDataFrame()
 
             memUSS = obj.getMemoryUSS()
 
             print("Total Memory in USS:", memUSS)
 
             memRSS = obj.getMemoryRSS()
 
@@ -406,37 +401,36 @@
         maximums = 0
         for ele in range(prefixLength):
             i = prefix[ele]
             if maximums < self._mapSupport.get(i):
                 maximums = self._mapSupport.get(i)
         return s / maximums
 
-    def _correlatedOneItem(self):
-        """
-            Generating One correlated itemsets
+    def _frequentOneItem(self):
+        """Generating One frequent items sets
+
         """
         self._mapSupport = {}
         for i in self._Database:
             for j in i:
                 if j not in self._mapSupport:
                     self._mapSupport[j] = 1
                 else:
                     self._mapSupport[j] += 1
 
     def _saveItemSet(self, prefix, prefixLength, support):
-        """
-        To save the correlated patterns mined form correlatedPatternTree
+        """To save the frequent patterns mined form frequentPatternTree
 
-        :param prefix: the correlated pattern
+        :param prefix: the frequent pattern
         :type prefix: list
-        :param prefixLength : the length of a correlated pattern
+        :param prefixLength : the length of a frequent pattern
         :type prefixLength : int
         :param support: the support of a pattern
         :type support :  int
-        :The correlated patterns were stored in a global variable finalPatterns
+        :The frequent patterns are update into global variable finalPatterns
         """
         allconf = self._getRatio(prefix, prefixLength, support)
         if allconf < self._minAllConf:
             return
         l = []
         for i in range(prefixLength):
             l.append(prefix[i])
@@ -458,15 +452,15 @@
                 value = float(value)
                 value = (len(self._Database) * value)
             else:
                 value = int(value)
         return value
 
     def _saveAllCombinations(self, tempBuffer, s, position, prefix, prefixLength):
-        """Generating all the combinations for items in single branch in correlatedPatternTree
+        """Generating all the combinations for items in single branch in frequentPatternTree
 
         :param tempBuffer: items in a list
         :type tempBuffer: list
         :param s : support at leaf node of a branch
         :param position : the length of a tempBuffer
         :type position : int
         :param prefix : it represents the list of leaf node
@@ -481,59 +475,59 @@
             for j in range(position):
                 isSet = i & (1 << j)
                 if isSet > 0:
                     prefix.insert(newPrefixLength, tempBuffer[j].itemId)
                     newPrefixLength += 1
             self._saveItemSet(prefix, newPrefixLength, s)
 
-    def _correlatedPatternGrowthGenerate(self, correlatedPatternTree, prefix, prefixLength, mapSupport):
+    def _frequentPatternGrowthGenerate(self, frequentPatternTree, prefix, prefixLength, mapSupport):
         """
 
         Mining the fp tree
 
-        :param correlatedPatternTree: it represents the correlatedPatternTree
-        :type correlatedPatternTree: class Tree
+        :param frequentPatternTree: it represents the frequentPatternTree
+        :type frequentPatternTree: class Tree
         :param prefix : it represents a empty list and store the patterns that are mined
         :type prefix : list
-        :param prefixLength : the length of prefix
+        :param param prefixLength : the length of prefix
         :type prefixLength :int
         :param mapSupport : it represents the support of item
         :type mapSupport : dictionary
 
         """
 
         singlePath = True
         position = 0
         s = 0
-        if len(correlatedPatternTree.root.child) > 1:
+        if len(frequentPatternTree.root.child) > 1:
             singlePath = False
         else:
-            currentNode = correlatedPatternTree.root.child[0]
+            currentNode = frequentPatternTree.root.child[0]
             while True:
                 if len(currentNode.child) > 1:
                     singlePath = False
                     break
                 self._fpNodeTempBuffer.insert(position, currentNode)
                 s = currentNode.counter
                 position += 1
                 if len(currentNode.child) == 0:
                     break
                 currentNode = currentNode.child[0]
         if singlePath is True:
             self._saveAllCombinations(self._fpNodeTempBuffer, s, position, prefix, prefixLength)
         else:
-            for i in reversed(correlatedPatternTree.headerList):
+            for i in reversed(frequentPatternTree.headerList):
                 item = i
                 support = mapSupport[i]
                 betaSupport = support
                 prefix.insert(prefixLength, item)
                 self._saveItemSet(prefix, prefixLength + 1, betaSupport)
                 if prefixLength + 1 < self._maxPatternLength:
                     prefixPaths = []
-                    path = correlatedPatternTree.mapItemNodes.get(item)
+                    path = frequentPatternTree.mapItemNodes.get(item)
                     mapSupportBeta = {}
                     while path is not None:
                         if path.parent.itemId != -1:
                             prefixPath = []
                             prefixPath.append(path)
                             pathCount = path.counter
                             parent1 = path.parent
@@ -547,43 +541,43 @@
                             prefixPaths.append(prefixPath)
                         path = path.nodeLink
                     treeBeta = _Tree()
                     for k in prefixPaths:
                         treeBeta.addPrefixPath(k, mapSupportBeta, self._minSup)
                     if len(treeBeta.root.child) > 0:
                         treeBeta.createHeaderList(mapSupportBeta, self._minSup)
-                        self._correlatedPatternGrowthGenerate(treeBeta, prefix, prefixLength + 1, mapSupportBeta)
+                        self._frequentPatternGrowthGenerate(treeBeta, prefix, prefixLength + 1, mapSupportBeta)
     
     def startMine(self):
         """
         main method to start
 
         """
         self._startTime = _ab._time.time()
         if self._iFile is None:
             raise Exception("Please enter the file path or file name:")
         self._creatingItemSets()
         self._minSup = self._convert(self._minSup)
         self._tree = _Tree()
         self._finalPatterns = {}
-        self._correlatedOneItem()
+        self._frequentOneItem()
         self._mapSupport = {k: v for k, v in self._mapSupport.items() if v >= self._minSup}
         _itemSetBuffer = [k for k, v in sorted(self._mapSupport.items(), key=lambda x: x[1], reverse=True)]
         for i in self._Database:
             _transaction = []
             for j in i:
                 if j in _itemSetBuffer:
                     _transaction.append(j)
             _transaction.sort(key=lambda val: self._mapSupport[val], reverse=True)
             self._tree.addTransaction(_transaction)
         self._tree.createHeaderList(self._mapSupport, self._minSup)
         if len(self._tree.headerList) > 0:
             self._itemSetBuffer = []
-            self._correlatedPatternGrowthGenerate(self._tree, self._itemSetBuffer, 0, self._mapSupport)
-        print("Correlated patterns were generated successfully using CPGrowth algorithm")
+            self._frequentPatternGrowthGenerate(self._tree, self._itemSetBuffer, 0, self._mapSupport)
+        print("Correlated Frequent patterns were generated successfully using CorrelatedPatternGrowth algorithm")
         self._endTime = _ab._time.time()
         self._memoryUSS = float()
         self._memoryRSS = float()
         process = _ab._psutil.Process(_ab._os.getpid())
         self._memoryUSS = process.memory_full_info().uss
         self._memoryRSS = process.memory_info().rss
 
@@ -617,17 +611,17 @@
         """
 
         return self._endTime - self._startTime
 
     def getPatternsAsDataFrame(self):
         """
 
-        Storing final correlated patterns in a dataframe
+        Storing final frequent patterns in a dataframe
 
-        :return: returning correlated patterns in a dataframe
+        :return: returning frequent patterns in a dataframe
         :rtype: pd.DataFrame
         """
 
         dataframe = {}
         data = []
         for a, b in self._finalPatterns.items():
             pat = " "
@@ -635,15 +629,15 @@
                 pat += str(i) + " "
             data.append([pat, b[0], b[1]])
             dataframe = _ab._pd.DataFrame(data, columns=['Patterns', 'Support', 'Confidence'])
         return dataframe
 
     def save(self, outFile):
         """
-        Complete set of correlated patterns will be saved into an output file
+        Complete set of frequent patterns will be loaded in to a output file
 
         :param outFile: name of the output file
         :type outFile: file
         """
         self._oFile = outFile
         writer = open(self._oFile, 'w+')
         for x, y in self._finalPatterns.items():
@@ -651,17 +645,17 @@
             for i in x:
                 pat += str(i) + "\t"
             patternsAndSupport = pat.strip() + ":" + str(y[0]) + ":" + str(y[1])
             writer.write("%s \n" % patternsAndSupport)
 
     def getPatterns(self):
         """
-        Function to send the set of correlated patterns after completion of the mining process
+        Function to send the set of frequent patterns after completion of the mining process
 
-        :return: returning correlated patterns
+        :return: returning frequent patterns
         :rtype: dict
         """
         return self._finalPatterns
 
     def printResults(self):
         print("Total number of Correlated Patterns:", len(self.getPatterns()))
         print("Total Memory in USS:", self.getMemoryUSS())
```

### Comparing `pami-2023.7.21/PAMI/correlatedPattern/basic/CPGrowthPlus.py` & `pami-2023.7.7/PAMI/correlatedPattern/basic/CPGrowthPlus.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-# CPGrowthPlus is one of the efficient algorithm to discover Correlated patterns in a transactional database.
+# CPGrowthPlus is one of the efficient algorithm to discover Correlated frequent patterns in a transactional database.
 #
 #  **Importing this algorithm into a python program**
 #   -----------------------------------------------
 #
-#                 from PAMI.correlatedPattern.basic import CPGrowthPlus as alg
+#                 from PAMI.coveragePattern.basic import CPPG as alg
 #
-#                 obj = alg.CPGrowthPlus(iFile, minSup, minAllConf, sep)
+#                 obj = alg.CPPG(iFile, minRF, minCS, maxOR)
 #
 #                 obj.startMine()
 #
-#                 correlatedPattern = obj.getPatterns()
+#                 coveragePatterns = obj.getPatterns()
 #
-#                 print("Total number of correlated Patterns:", len(correlatedPattern))
+#                 print("Total number of coverage Patterns:", len(coveragePatterns))
 #
 #                 obj.save(oFile)
 #
 #                 Df = obj.getPatternsAsDataFrame()
 #
 #                 memUSS = obj.getMemoryUSS()
 #
@@ -25,14 +25,17 @@
 #
 #                 print("Total Memory in RSS", memRSS)
 #
 #                 run = obj.getRuntime()
 #
 #                 print("Total ExecutionTime in seconds:", run)
 
+
+
+
 __copyright__ = """
  Copyright (C)  2021 Rage Uday Kiran
 
      This program is free software: you can redistribute it and/or modify
      it under the terms of the GNU General Public License as published by
      the Free Software Foundation, either version 3 of the License, or
      (at your option) any later version.
@@ -46,17 +49,18 @@
      along with this program.  If not, see <https://www.gnu.org/licenses/>.
      Copyright (C)  2021 Rage Uday Kiran
 """
 
 from PAMI.correlatedPattern.basic import abstract as _ab
 
 
+
 class _Node:
     """
-        A class used to represent the node of correlatedPatternTree
+        A class used to represent the node of frequentPatternTree
 
     Attributes :
     ----------
         itemId: int
             storing item of a node
         counter: int
             To maintain the support of node
@@ -67,15 +71,15 @@
         nodeLink : node
             Points to the node with same itemId
 
     Methods :
     -------
 
         getChild(itemName)
-            returns the node with same itemName from correlatedPatternTree
+            returns the node with same itemName from frequentPatternTree
     """
 
     def __init__(self):
         self.itemId = -1
         self.counter = 1
         self.parent = None
         self.child = []
@@ -83,27 +87,27 @@
 
     def getChild(self, itemName):
         """
         Retrieving the child from the tree
 
             :param itemName: name of the child
             :type itemName: list
-            :return: returns the node with same itemName from correlatedPatternTree
+            :return: returns the node with same itemName from frequentPatternTree
             :rtype: list
 
         """
         for i in self.child:
             if i.itemId == itemName:
                 return i
         return None
 
 
 class _Tree:
     """
-        A class used to represent the correlatedPatternGrowth tree structure
+        A class used to represent the frequentPatternGrowth tree structure
 
     Attributes :
     ----------
         headerList : list
             storing the list of items in tree sorted in ascending of their supports
         mapItemNodes : dictionary
             storing the nodes with same item name
@@ -113,34 +117,34 @@
             representing the root Node in a tree
 
     Methods :
     -------
         createHeaderList(items,minSup)
             takes items only which are greater than minSup and sort the items in ascending order
         addTransaction(transaction)
-            creating transaction as a branch in correlatedPatternTree
+            creating transaction as a branch in frequentPatternTree
         fixNodeLinks(item,newNode)
             To create the link for nodes with same item
         printTree(Node)
-            gives the details of node in correlatedPatternGrowth tree
+            gives the details of node in frequentPatternGrowth tree
         addPrefixPath(prefix,port,minSup)
            It takes the items in prefix pattern whose support is >=minSup and construct a subtree
     """
 
     def __init__(self):
         self.headerList = []
         self.mapItemNodes = {}
         self.mapItemLastNodes = {}
         self.root = _Node()
 
     def addTransaction(self, transaction):
         """
         Adding a transaction into a tree
 
-        :param transaction: it represents a transaction in a database
+        :param transaction: it represents the one transactions in database
         :type transaction: list
         """
 
         # This method taken a transaction as input and returns the tree
         current = self.root
         for i in transaction:
             child = current.getChild(i)
@@ -153,78 +157,80 @@
                 current = newNode
             else:
                 child.counter += 1
                 current = child
 
     def fixNodeLinks(self, item, newNode):
         """
-        Fixing node link for the newNode that inserted into correlatedPatternTree
+        Fixing node link for the newNode that inserted into frequentPatternTree
 
         :param item: it represents the item of newNode
         :type item: int
-        :param newNode: it represents the newNode that inserted in correlatedPatternTree
+        :param newNode: it represents the newNode that inserted in frequentPatternTree
         :type newNode: Node
 
         """
         if item in self.mapItemLastNodes.keys():
             lastNode = self.mapItemLastNodes[item]
             lastNode.nodeLink = newNode
         self.mapItemLastNodes[item] = newNode
         if item not in self.mapItemNodes.keys():
             self.mapItemNodes[item] = newNode
 
     def printTree(self, root):
         """
 
-        Print the details of Node in correlatedPatternTree
+        Print the details of Node in frequentPatternTree
 
-        :param root: it represents the Node in correlatedPatternTree
+        :param root: it represents the Node in frequentPatternTree
         :type root: Node
 
         """
+
         # this method is used print the details of tree
         if not root.child:
             return
         else:
             for i in root.child:
                 print(i.itemId, i.counter, i.parent.itemId)
                 self.printTree(i)
 
     def createHeaderList(self, mapSupport, minSup):
         """
+
         To create the headerList
 
         :param mapSupport: it represents the items with their supports
         :type mapSupport: dictionary
         :param minSup: it represents the minSup
         :param minSup: float
 
         """
-        # the correlatedPatternTree always maintains the header table to start the mining from leaf nodes
+        # the frequentPatternTree always maintains the header table to start the mining from leaf nodes
         t1 = []
         for x, y in mapSupport.items():
             if y >= minSup:
                 t1.append(x)
-        itemSetBuffer = [k for k, v in sorted(mapSupport.items(), key=lambda val: val[1], reverse=True)]
+        itemSetBuffer = [k for k, v in sorted(mapSupport.items(), key=lambda x: x[1], reverse=True)]
         self.headerList = [i for i in t1 if i in itemSetBuffer]
 
     def addPrefixPath(self, prefix, mapSupportBeta, minSup):
         """
 
-        To construct the conditional tree with prefix paths of a node in correlatedPatternTree
+        To construct the conditional tree with prefix paths of a node in frequentPatternTree
 
         :param prefix: it represents the prefix items of a Node
         :type prefix: list
         :param mapSupportBeta: it represents the items with their supports
         :param mapSupportBeta: dictionary
         :param minSup: to check the item meets with minSup
         :param minSup: float
 
         """
-        # this method is used to add prefix paths in conditional trees of correlatedPatternTree
+        # this method is used to add prefix paths in conditional trees of frequentPatternTree
         pathCount = prefix[0].counter
         current = self.root
         prefix.reverse()
         for i in range(0, len(prefix) - 1):
             pathItem = prefix[i]
             if mapSupportBeta.get(pathItem.itemId) >= minSup:
                 child = current.getChild(pathItem.itemId)
@@ -239,27 +245,27 @@
                 else:
                     child.counter += pathCount
                     current = child
 
 
 class CPGrowthPlus(_ab._correlatedPatterns):
     """ 
-    :Description:    CPGrowthPlus is one of the efficient algorithm to discover correlated patterns in a transactional database.
+    :Description:    CPGrowthPlus is one of the efficient algorithm to discover Correlated frequent patterns in a transactional database.
                      Using Item Support Intervals technique which is generating correlated patterns of higher order by combining only with items that
                      have support within specified interval.
 
     :Reference:
         Uday Kiran R., Kitsuregawa M. (2012) Efficient Discovery of Correlated Patterns in Transactional Databases Using Items’ Support Intervals.
         In: Liddle S.W., Schewe KD., Tjoa A.M., Zhou X. (eds) Database and Expert Systems Applications. DEXA 2012. Lecture Notes in Computer Science, vol 7446. Springer, Berlin, Heidelberg.
         https://doi.org/10.1007/978-3-642-32600-4_18
 
     :param  iFile: str :
-                   Name of the Input file to mine complete set of correlated patterns
+                   Name of the Input file to mine complete set of frequent patterns
     :param  oFile: str :
-                   Name of the output file to store complete set of correlated patterns
+                   Name of the output file to store complete set of frequent patterns
     :param  minSup: int or float or str :
                    The user can specify minSup either in count or proportion of database size. If the program detects the data type of minSup is integer, then it treats minSup is expressed in count.
     :param  minAllConf: str :
                    Name of Neighbourhood file name
     :param  sep: str :
                    This variable is used to distinguish items from one another in a transaction. The default seperator is tab space. However, the users can override their default separator.
 
@@ -295,39 +301,39 @@
         maxPatternLength : int
            it represents the constraint for pattern length
 
     **Methods to execute code on terminal**
     ---------------------------------------
 
             Format:
-                      >>>  python3 CPGrowthPlus.py <inputFile> <outputFile> <minSup> <minAllConf> <sep>
+                      >>>  python3 CPPG.py <inputFile> <outputFile> <minRF> <minCS> <maxOR> <'\t'>
 
             Example:
-                      >>>   python3 CPGrowthPlus.py sampleTDB.txt patterns.txt 0.4 0.5 ','
+                      >>>   python3 CPPG.py sampleTDB.txt patterns.txt 0.4 0.7 0.5 ','
 
 
 
     **Importing this algorithm into a python program**
     -----------------------------------------------------------------
 
     .. code-block:: python
 
-                from PAMI.correlatedPattern.basic import CPGrowthPlus as alg
+                from PAMI.coveragePattern.basic import CPPG as alg
 
-                obj = alg.CPGrowthPlus(iFile, minSup, minAllConf, sep)
+                obj = alg.CPPG(iFile, minRF, minCS, maxOR)
 
                 obj.startMine()
 
-                correlatedPatterns = obj.getPatterns()
+                coveragePatterns = obj.getPatterns()
 
-                print("Total number of correlated patterns:", len(correlatedPatterns))
+                print("Total number of coverage Patterns:", len(coveragePatterns))
 
                 obj.save(oFile)
 
-                df = obj.getPatternsAsDataFrame()
+                Df = obj.getPatternsAsDataFrame()
 
                 memUSS = obj.getMemoryUSS()
 
                 print("Total Memory in USS:", memUSS)
 
                 memRSS = obj.getMemoryRSS()
 
@@ -366,15 +372,17 @@
 
     def __init__(self, iFile, minSup, minAllConf, sep="\t"):
         super().__init__(iFile, minSup, minAllConf, sep)
 
     def _creatingItemSets(self):
         """
             Storing the complete transactions of the database/input file in a database variable
-        """
+
+
+            """
         self._Database = []
         if isinstance(self._iFile, _ab._pd.DataFrame):
             if self._iFile.empty:
                 print("its empty..")
             i = self._iFile.columns.values.tolist()
             if 'Transactions' in i:
                 self._Database = self._iFile['Transactions'].tolist()
@@ -395,48 +403,48 @@
                             temp = [i.rstrip() for i in line.split(self._sep)]
                             temp = [x for x in temp if x]
                             self._Database.append(temp)
                 except IOError:
                     print("File Not Found")
                     quit()
 
-    def _correlatedOneItem(self):
+    def _frequentOneItem(self):
         """
-        Generating One correlated items sets
+        Generating One frequent items sets
 
         """
         self._mapSupport = {}
         for i in self._Database:
             for j in i:
                 if j not in self._mapSupport:
                     self._mapSupport[j] = 1
                 else:
                     self._mapSupport[j] += 1
 
     def _saveItemSet(self, prefix, prefixLength, support, ratio):
         """
-        To save the correlated patterns mined form correlatedPatternTree
+        To save the frequent patterns mined form frequentPatternTree
 
-        :param prefix: the correlated pattern
+        :param prefix: the frequent pattern
         :type prefix: list
-        :param prefixLength: the length of a correlated pattern
+        :param prefixLength: the length of a frequent pattern
         :type prefixLength: int
         :param support: the support of a pattern
         :type support:  int
         """
 
         sample = []
         for i in range(prefixLength):
             sample.append(prefix[i])
         self._itemSetCount += 1
         self._finalPatterns[tuple(sample)] = [support, ratio]
 
     def _saveAllCombinations(self, tempBuffer, s, position, prefix, prefixLength):
         """
-        Generating all the combinations for items in single branch in correlatedPatternTree
+        Generating all the combinations for items in single branch in frequentPatternTree
 
         :param tempBuffer: items in a list
         :type tempBuffer: list
         :param s: support at leaf node of a branch
         :param position: the length of a tempBuffer
         :type position: int
         :param prefix: it represents the list of leaf node
@@ -453,63 +461,63 @@
                 if isSet > 0:
                     prefix.insert(newPrefixLength, tempBuffer[j].itemId)
                     newPrefixLength += 1
             ratio = s/self._mapSupport[self._getMaxItem(prefix, newPrefixLength)]
             if ratio >= self._minAllConf:
                 self._saveItemSet(prefix, newPrefixLength, s, ratio)
 
-    def _correlatedPatternGrowthGenerate(self, correlatedPatternTree, prefix, prefixLength, mapSupport, minConf):
+    def _frequentPatternGrowthGenerate(self, frequentPatternTree, prefix, prefixLength, mapSupport, minConf):
         """
         Mining the fp tree
 
-        :param correlatedPatternTree: it represents the correlatedPatternTree
-        :type correlatedPatternTree: class Tree
+        :param frequentPatternTree: it represents the frequentPatternTree
+        :type frequentPatternTree: class Tree
         :param prefix: it represents a empty list and store the patterns that are mined
         :type prefix: list
         :param param prefixLength: the length of prefix
         :type prefixLength: int
         :param mapSupport : it represents the support of item
         :type mapSupport : dictionary
         """
         singlePath = True
         position = 0
         s = 0
-        if len(correlatedPatternTree.root.child) > 1:
+        if len(frequentPatternTree.root.child) > 1:
             singlePath = False
         else:
-            currentNode = correlatedPatternTree.root.child[0]
+            currentNode = frequentPatternTree.root.child[0]
             while True:
                 if len(currentNode.child) > 1:
                     singlePath = False
                     break
                 self._fpNodeTempBuffer.insert(position, currentNode)
                 s = currentNode.counter
                 position += 1
                 if len(currentNode.child) == 0:
                     break
                 currentNode = currentNode.child[0]
         if singlePath is True:
             self._saveAllCombinations(self._fpNodeTempBuffer, s, position, prefix, prefixLength)
         else:
-            for i in reversed(correlatedPatternTree.headerList):
+            for i in reversed(frequentPatternTree.headerList):
                 item = i
                 support = mapSupport[i]
                 low = max(int(_ab._math.floor(mapSupport[i]*self._minAllConf)), self._minSup)
                 high = max(int(_ab._math.floor(mapSupport[i]/minConf)), self._minSup)
-                betaSupport = support
+                betaSupport = support              
                 prefix.insert(prefixLength, item)
                 max1 = self._getMaxItem(prefix, prefixLength)
                 if self._mapSupport[max1] < self._mapSupport[item]:
                     max1 = item
                 ratio = support / self._mapSupport[max1]
                 if ratio >= self._minAllConf:
                     self._saveItemSet(prefix, prefixLength + 1, betaSupport, ratio)
                 if prefixLength + 1 < self._maxPatternLength:
                     prefixPaths = []
-                    path = correlatedPatternTree.mapItemNodes.get(item)
+                    path = frequentPatternTree.mapItemNodes.get(item)
                     mapSupportBeta = {}
                     while path is not None:
                         if path.parent.itemId != -1:
                             prefixPath = [path]
                             pathCount = path.counter
                             parent1 = path.parent
                             if mapSupport.get(parent1.itemId) >= low and mapSupport.get(parent1.itemId) <= high:
@@ -527,15 +535,15 @@
                                 prefixPaths.append(prefixPath)
                         path = path.nodeLink
                     treeBeta = _Tree()
                     for k in prefixPaths:
                         treeBeta.addPrefixPath(k, mapSupportBeta, self._minSup)
                     if len(treeBeta.root.child) > 0:
                         treeBeta.createHeaderList(mapSupportBeta, self._minSup)
-                        self._correlatedPatternGrowthGenerate(treeBeta, prefix, prefixLength + 1, mapSupportBeta, minConf)
+                        self._frequentPatternGrowthGenerate(treeBeta, prefix, prefixLength + 1, mapSupportBeta, minConf)
 
     def _convert(self, value):
         """
         to convert the type of user specified minSup value
         :param value: user specified minSup value
         :return: converted type
         """
@@ -561,28 +569,28 @@
             raise Exception("Please enter the file path or file name:")
         if self._minSup is None:
             raise Exception("Please enter the Minimum Support")
         self._creatingItemSets()
         self._finalPatterns = {}
         self._tree = _Tree()
         self._minSup = self._convert(self._minSup)
-        self._correlatedOneItem()
+        self._frequentOneItem()
         self._mapSupport = {k: v for k, v in self._mapSupport.items() if v >= self._minSup}
         _itemSetBuffer = [k for k, v in sorted(self._mapSupport.items(), key=lambda x: x[1], reverse=True)]
         for i in self._Database:
             _transaction = []
             for j in i:
                 if j in _itemSetBuffer:
                     _transaction.append(j)
             _transaction.sort(key=lambda val: self._mapSupport[val], reverse=True)
             self._tree.addTransaction(_transaction)
         self._tree.createHeaderList(self._mapSupport, self._minSup)
         if len(self._tree.headerList) > 0:
             self._itemSetBuffer = []
-            self._correlatedPatternGrowthGenerate(self._tree, self._itemSetBuffer, 0, self._mapSupport, self._minAllConf)
+            self._frequentPatternGrowthGenerate(self._tree, self._itemSetBuffer, 0, self._mapSupport, self._minAllConf)
         print("Correlated Frequent patterns were generated successfully using CorrelatedPatternGrowth algorithm")
         self._endTime = _ab._time.time()
         process = _ab._psutil.Process(_ab._os.getpid())
         self._memoryRSS = float()
         self._memoryUSS = float()
         self._memoryUSS = process.memory_full_info().uss
         self._memoryRSS = process.memory_info().rss
@@ -609,31 +617,31 @@
 
     def _getMaxItem(self, prefix, prefixLength):
         maxItem = prefix[0]
         for i in range(prefixLength):
             if self._mapSupport[maxItem] < self._mapSupport[prefix[i]]:
                 maxItem = prefix[i]
         return maxItem
-
+    
     def getRuntime(self):
         """
         Calculating the total amount of runtime taken by the mining process
 
 
         :return: returning total amount of runtime taken by the mining process
         :rtype: float
         """
 
         return self._endTime - self._startTime
 
     def getPatternsAsDataFrame(self):
         """
-        Storing final correlated patterns in a dataframe
+        Storing final frequent patterns in a dataframe
 
-        :return: returning correlated patterns in a dataframe
+        :return: returning frequent patterns in a dataframe
         :rtype: pd.DataFrame
         """
 
         dataframe = {}
         data = []
         for a, b in self._finalPatterns.items():
             pat = " "
@@ -641,15 +649,15 @@
                 pat += str(i) + " "
             data.append([pat, b[0], b[1]])
             dataframe = _ab._pd.DataFrame(data, columns=['Patterns', 'Support', 'Confidence'])
         return dataframe
 
     def save(self, outFile):
         """
-        Complete set of correlated patterns will be loaded in to a output file
+        Complete set of frequent patterns will be loaded in to a output file
 
         :param outFile: name of the output file
         :type outFile: file
         """
         self._oFile = outFile
         writer = open(self._oFile, 'w+')
         for x, y in self._finalPatterns.items():
@@ -657,17 +665,17 @@
             for i in x:
                 pattern = pattern + i + "\t"
             s1 = str(pattern.strip()) + ":" + str(y[0]) + ":" + str(y[1])
             writer.write("%s \n" % s1)
 
     def getPatterns(self):
         """
-        Function to send the set of correlated patterns after completion of the mining process
+        Function to send the set of frequent patterns after completion of the mining process
 
-        :return: returning correlated patterns
+        :return: returning frequent patterns
         :rtype: dict
         """
         return self._finalPatterns
 
     def printResults(self):
         print("Total number of Correlated Patterns:", len(self.getPatterns()))
         print("Total Memory in USS:", self.getMemoryUSS())
@@ -686,8 +694,8 @@
         _correlatedPatterns = _ap.getPatterns()
         print("Total number of Correlated-Frequent Patterns:", len(_ap.getPatterns()))
         _ap.save(_ab._sys.argv[2])
         print("Total Memory in USS:", _ap.getMemoryUSS())
         print("Total Memory in RSS", _ap.getMemoryRSS())
         print("Total ExecutionTime in seconds:", _ap.getRuntime())
     else:
-        print("Error! The number of input parameters do not match the total number of parameters provided")
+        print("Error! The number of input parameters do not match the total number of parameters provided")
```

### Comparing `pami-2023.7.21/PAMI/correlatedPattern/basic/__init__.py` & `pami-2023.7.7/PAMI/correlatedPattern/basic/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/correlatedPattern/basic/abstract.py` & `pami-2023.7.7/PAMI/frequentSpatialPattern/basic/abstract.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,57 +8,70 @@
 #      This program is distributed in the hope that it will be useful,
 #      but WITHOUT ANY WARRANTY; without even the implied warranty of
 #      MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #      GNU General Public License for more details.
 #
 #      You should have received a copy of the GNU General Public License
 #      along with this program.  If not, see <https://www.gnu.org/licenses/>.
+#
+#      This program is free software: you can redistribute it and/or modify
+#      it under the terms of the GNU General Public License as published by
+#      the Free Software Foundation, either version 3 of the License, or
+#      (at your option) any later version.
+#
+#      This program is distributed in the hope that it will be useful,
+#      but WITHOUT ANY WARRANTY; without even the implied warranty of
+#      MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+#      GNU General Public License for more details.
+#
+#      You should have received a copy of the GNU General Public License
+#      along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 from abc import ABC as _ABC, abstractmethod as _abstractmethod
 import time as _time
 import csv as _csv
 import pandas as _pd
 from collections import defaultdict as _defaultdict
 from itertools import combinations as _c
 import os as _os
 import os.path as _ospath
 import psutil as _psutil
+import sys as _sys
 import validators as _validators
 from urllib.request import urlopen as _urlopen
-import sys as _sys
-import math as _math
+from collections import OrderedDict as _OrderedDict
 
 
-class _correlatedPatterns(_ABC):
-    """ This abstract base class defines the variables and methods that every correlated pattern mining algorithm must
+class _spatialFrequentPatterns(_ABC):
+    """ This abstract base class defines the variables and methods that every frequent pattern mining algorithm must
         employ in PAMI
 
 
     Attributes :
     ----------
         iFile : str
             Input file name or path of the input file
+        nFile: str
+            Neighbourhoof file name
         minSup: integer or float or str
             The user can specify minSup either in count or proportion of database size.
             If the program detects the data type of minSup is integer, then it treats minSup is expressed in count.
             Otherwise, it will be treated as float.
             Example: minSup=10 will be treated as integer, while minSup=10.0 will be treated as float
-        minAllConf: float
-            The user given minimum all confidence Ratio(should be in range of 0 to 1)
         sep : str
             This variable is used to distinguish items from one another in a transaction. The default seperator is tab space or \t.
             However, the users can override their default separator
         startTime:float
             To record the start time of the algorithm
         endTime:float
             To record the completion time of the algorithm
         finalPatterns: dict
             Storing the complete set of patterns in a dictionary variable
         oFile : str
-            Name of the output file to store complete set of correlated patterns
+            Name of the output file to store complete set of frequent patterns
         memoryUSS : float
             To store the total amount of USS memory consumed by the program
         memoryRSS : float
             To store the total amount of RSS memory consumed by the program
 
     Methods :
     -------
@@ -75,66 +88,67 @@
         getMemoryRSS()
             This function outputs the total amount of RSS memory consumed by a mining algorithm
         getRuntime()
             This function outputs the total runtime of a mining algorithm
 
     """
 
-    def __init__(self, iFile, minSup, minAllConf, sep="\t"):
+    def __init__(self, iFile, nFile, minSup, sep="\t"):
         """
         :param iFile: Input file name or path of the input file
         :type iFile: str
+        :param nFile: Neighbourhood name of the input
+        :type nFile: str
         :param minSup: The user can specify minSup either in count or proportion of database size.
             If the program detects the data type of minSup is integer, then it treats minSup is expressed in count.
             Otherwise, it will be treated as float.
             Example: minSup=10 will be treated as integer, while minSup=10.0 will be treated as float
         :type minSup: int or float or str
-        :param minAllConf: The user given minimum all confidence Ratio(should be in range of 0 to 1)
-        :type minAllConf :float
         :param sep: separator used to distinguish items from each other. The default separator is tab space. However, users can override the default separator
         :type sep: str
         """
 
         self._iFile = iFile
+        self._nFile = nFile
+        self._oFile = str()
         self._sep = sep
         self._minSup = minSup
-        self._minAllConf = minAllConf
-        self._finalPatterns = {}
-        self._oFile = str()
-        self._memoryRSS = float()
-        self._memoryUSS = float()
         self._startTime = float()
         self._endTime = float()
+        self._memoryUSS = float()
+        self._memoryRSS = float()
+        self._finalPatterns = {}
+        self._oFile = str()
 
 
     @_abstractmethod
     def startMine(self):
         """Code for the mining process will start from this function"""
 
         pass
 
     @_abstractmethod
     def getPatterns(self):
-        """Complete set of correlated patterns generated will be retrieved from this function"""
+        """Complete set of frequent patterns generated will be retrieved from this function"""
 
         pass
 
     @_abstractmethod
     def save(self, oFile):
-        """Complete set of correlated patterns will be saved in to an output file from this function
+        """Complete set of frequent patterns will be saved in to an output file from this function
 
         :param oFile: Name of the output file
         :type oFile: file
         """
 
         pass
 
     @_abstractmethod
     def getPatternsAsDataFrame(self):
-        """Complete set of correlated patterns will be loaded in to data frame from this function"""
+        """Complete set of frequent patterns will be loaded in to data frame from this function"""
 
         pass
 
     @_abstractmethod
     def getMemoryUSS(self):
         """Total amount of USS memory consumed by the program will be retrieved from this function"""
 
@@ -151,10 +165,11 @@
     def getRuntime(self):
         """Total amount of runtime taken by the program will be retrieved from this function"""
 
         pass
 
     @_abstractmethod
     def printResults(self):
-        """ To print the results of execution."""
+
+        """ To print the results of execution"""
 
         pass
```

### Comparing `pami-2023.7.21/PAMI/coveragePattern/basic/CMine.py` & `pami-2023.7.7/PAMI/coveragePatterns/basic/CMine.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 #
 #                 from PAMI.coveragePattern.basic import CMine as alg
 #
 #                 obj = alg.CMine(iFile, minRF, minCS, maxOR, seperator)
 #
 #                 obj.startMine()
 #
-#                 coveragePattern = obj.getPatterns()
+#                 coveragePatterns = obj.getPatterns()
 #
-#                 print("Total number of coverage Patterns:", len(coveragePattern))
+#                 print("Total number of coverage Patterns:", len(coveragePatterns))
 #
 #                 obj.save(oFile)
 #
 #                 Df = obj.getPatternsAsDataFrame()
 #
 #                 memUSS = obj.getMemoryUSS()
 #
@@ -46,15 +46,15 @@
      You should have received a copy of the GNU General Public License
      along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """
 
 
 
 
-from PAMI.coveragePattern.basic import abstract as _ab
+from PAMI.coveragePatterns.basic import abstract as _ab
 
 class CMine(_ab._coveragePatterns):
     """
 
     :Description:  CMine algorithms aims to discover the coverage patterns in transactional databases.
 
     :Reference:    Bhargav Sripada, Polepalli Krishna Reddy, Rage Uday Kiran:
@@ -111,17 +111,17 @@
 
                 from PAMI.coveragePattern.basic import CMine as alg
 
                 obj = alg.CMine(iFile, minRF, minCS, maxOR, seperator)
 
                 obj.startMine()
 
-                coveragePattern = obj.getPatterns()
+                coveragePatterns = obj.getPatterns()
 
-                print("Total number of coverage Patterns:", len(coveragePattern))
+                print("Total number of coverage Patterns:", len(coveragePatterns))
 
                 obj.save(oFile)
 
                 Df = obj.getPatternsAsDataFrame()
 
                 memUSS = obj.getMemoryUSS()
 
@@ -373,8 +373,13 @@
         _ap.startMine()
         print("Total number of coverage Patterns:", len(_ap.getPatterns()))
         _ap.save(_ab._sys.argv[2])
         print("Total Memory in USS:", _ap.getMemoryUSS())
         print("Total Memory in RSS", _ap.getMemoryRSS())
         print("Total ExecutionTime in ms:", _ap.getRuntime())
     else:
+        _ap = CPPG('sample.txt', 0.4, 0.7, 0.5, ' ')
+        _ap.startMine()
+        print("Total number of Coverage Patterns:", len(_ap.getPatterns()))
+        _ap.save('output.txt')
+        _ap.printResults()
         print("Error! The number of input parameters do not match the total number of parameters provided")
```

### Comparing `pami-2023.7.21/PAMI/coveragePattern/basic/CPPG.py` & `pami-2023.7.7/PAMI/coveragePatterns/basic/CPPG.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 #
 #             from PAMI.coveragePattern.basic import CPPG as alg
 #
 #             obj = alg.CPPG(iFile, minRF, minCS, maxOR)
 #
 #             obj.startMine()
 #
-#             coveragePattern = obj.getPatterns()
+#             coveragePatterns = obj.getPatterns()
 #
-#             print("Total number of coverage Patterns:", len(coveragePattern))
+#             print("Total number of coverage Patterns:", len(coveragePatterns))
 #
 #             obj.save(oFile)
 #
 #             Df = obj.getPatternsAsDataFrame()
 #
 #             memUSS = obj.getMemoryUSS()
 #
@@ -45,15 +45,15 @@
      MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
      GNU General Public License for more details.
 
      You should have received a copy of the GNU General Public License
      along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """
 
-from PAMI.coveragePattern.basic import abstract as _ab
+from PAMI.coveragePatterns.basic import abstract as _ab
 
 
 _maxPer = float()
 _minSup = float()
 _lno = int()
 
 
@@ -120,17 +120,17 @@
 
                 from PAMI.coveragePattern.basic import CPPG as alg
 
                 obj = alg.CPPG(iFile, minRF, minCS, maxOR)
 
                 obj.startMine()
 
-                coveragePattern = obj.getPatterns()
+                coveragePatterns = obj.getPatterns()
 
-                print("Total number of coverage Patterns:", len(coveragePattern))
+                print("Total number of coverage Patterns:", len(coveragePatterns))
 
                 obj.save(oFile)
 
                 Df = obj.getPatternsAsDataFrame()
 
                 memUSS = obj.getMemoryUSS()
```

### Comparing `pami-2023.7.21/PAMI/coveragePattern/basic/abstract.py` & `pami-2023.7.7/PAMI/coveragePatterns/basic/abstract.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 import psutil as _psutil
 import sys as _sys
 import validators as _validators
 from urllib.request import urlopen as _urlopen
 
 
 class _coveragePatterns(_ABC):
-    """ This abstract base class defines the variables and methods that every coverage pattern mining algorithm must
+    """ This abstract base class defines the variables and methods that every periodic-frequent pattern mining algorithm must
         employ in PAMI
 
        Attributes
         ----------
         iFile : str
             Input file name or path of the input file
         minCS: int or float or str
@@ -50,60 +50,59 @@
             The user can specify minRF either in count or proportion of database size.
             If the program detects the data type of minRF is integer, then it treats minRF is expressed in count.
             Otherwise, it will be treated as float.
             Example: minRF=10 will be treated as integer, while minRF=10.0 will be treated as float
         sep : str
             This variable is used to distinguish items from one another in a transaction. The default seperator is tab space or \t.
             However, the users can override their default separator.
-        startTime: float
+        startTime:float
             To record the start time of the algorithm
-        endTime: float
+        endTime:float
             To record the completion time of the algorithm
         finalPatterns: dict
             Storing the complete set of patterns in a dictionary variable
         oFile : str
-            Name of the output file to store complete set of coverage patterns
+            Name of the output file to store complete set of periodic-frequent patterns
         memoryUSS : float
             To store the total amount of USS memory consumed by the program
         memoryRSS : float
             To store the total amount of RSS memory consumed by the program
 
         Methods
         -------
         startMine()
             Mining process will start from here
         getPatterns()
             Complete set of patterns will be retrieved with this function
         save(oFile)
-            Complete set of coverage patterns will be loaded in to a output file
+            Complete set of periodic-frequent patterns will be loaded in to a output file
         getPatternsAsDataFrame()
-            Complete set of coverage patterns will be loaded in to data frame
+            Complete set of periodic-frequent patterns will be loaded in to data frame
         getMemoryUSS()
             Total amount of USS memory consumed by the program will be retrieved from this function
         getMemoryRSS()
             Total amount of RSS memory consumed by the program will be retrieved from this function
         getRuntime()
             Total amount of runtime taken by the program will be retrieved from this function
     """
 
-    def __init__(self, iFile, minRF, minCS, maxOR, sep='\t'):
+    def __init__(self, iFile, minRF, minCS, maxOR, sep = '\t'):
         """
         :param iFile: Input file name or path of the input file
         :type iFile: str
-        :param minRF: The user can specify minimum relative frequency either in count or proportion of database size.
-            If the program detects the data type of minRF is integer, then it treats minRF is expressed in count.
+        :param minSup: The user can specify minSup either in count or proportion of database size.
+            If the program detects the data type of minSup is integer, then it treats minSup is expressed in count.
             Otherwise, it will be treated as float.
-            Example: minRF=10 will be treated as integer, while minRF=10.0 will be treated as float
-        :type minRF: int or float or str
-        :param minCS: The user can specify minimum coverage support either in count or proportion of database size.
+            Example: minSup=10 will be treated as integer, while minSup=10.0 will be treated as float
+        :type minSup: int or float or str
+        :param maxPer: The user can specify maxPer either in count or proportion of database size.
             If the program detects the data type of maxPer is integer, then it treats maxPer is expressed in count.
             Otherwise, it will be treated as float.
             Example: maxPer=10 will be treated as integer, while maxPer=10.0 will be treated as float
-        :param maxOR: The user can specify maximum overlap ratio either in count or proportion of database size.
-        :type maxOR: int or float or str
+        :type maxPer: int or float or str
         :param sep: separator used in user specified input file
         :type sep: str
         """
 
         self._iFile = iFile
         self._minCS = minCS
         self._minRF = minRF
@@ -120,31 +119,31 @@
     def startMine(self):
         """Code for the mining process will start from this function"""
 
         pass
 
     @_abstractmethod
     def getPatterns(self):
-        """Complete set of coverage patterns generated will be retrieved from this function"""
+        """Complete set of periodic-frequent patterns generated will be retrieved from this function"""
 
         pass
 
     @_abstractmethod
     def save(self, oFile):
-        """Complete set of coverage patterns will be saved in to an output file from this function
+        """Complete set of periodic-frequent patterns will be saved in to an output file from this function
 
         :param oFile: Name of the output file
         :type oFile: file
         """
 
         pass
 
     @_abstractmethod
     def getPatternsAsDataFrame(self):
-        """Complete set of coverage patterns will be loaded in to data frame from this function"""
+        """Complete set of periodic-frequent patterns will be loaded in to data frame from this function"""
 
         pass
 
     @_abstractmethod
     def getMemoryUSS(self):
         """Total amount of USS memory consumed by the program will be retrieved from this function"""
```

### Comparing `pami-2023.7.21/PAMI/extras/DF2DB/DF2DB.py` & `pami-2023.7.7/PAMI/extras/DF2DB/DF2DB.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/extras/DF2DB/DF2DBPlus.py` & `pami-2023.7.7/PAMI/extras/DF2DB/DF2DBPlus.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/extras/DF2DB/createTDB.py` & `pami-2023.7.7/PAMI/extras/DF2DB/createTDB.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/extras/DF2DB/denseDF2DB.py` & `pami-2023.7.7/PAMI/extras/DF2DB/denseDF2DB.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/extras/DF2DB/denseDF2DBPlus.py` & `pami-2023.7.7/PAMI/extras/DF2DB/denseDF2DBPlus.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/extras/DF2DB/denseDF2DB_dump.py` & `pami-2023.7.7/PAMI/extras/DF2DB/denseDF2DB_dump.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/extras/DF2DB/sparseDF2DB.py` & `pami-2023.7.7/PAMI/extras/DF2DB/sparseDF2DB.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/extras/DF2DB/sparseDF2DBPlus.py` & `pami-2023.7.7/PAMI/extras/DF2DB/sparseDF2DBPlus.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/extras/calculateMISValues/usingBeta.py` & `pami-2023.7.7/PAMI/extras/calculateMISValues/usingBeta.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/extras/calculateMISValues/usingSD.py` & `pami-2023.7.7/PAMI/extras/calculateMISValues/usingSD.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/extras/dbStats/fuzzyDatabaseStats.py` & `pami-2023.7.7/PAMI/extras/dbStats/fuzzyDatabaseStats.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/extras/dbStats/temporalDatabaseStats.py` & `pami-2023.7.7/PAMI/extras/dbStats/temporalDatabaseStats.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/extras/dbStats/transactionalDatabaseStats.py` & `pami-2023.7.7/PAMI/extras/dbStats/transactionalDatabaseStats.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/extras/dbStats/uncertainTemporalDatabaseStats.py` & `pami-2023.7.7/PAMI/extras/dbStats/uncertainTemporalDatabaseStats.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/extras/dbStats/uncertainTransactionalDatabaseStats.py` & `pami-2023.7.7/PAMI/extras/dbStats/uncertainTransactionalDatabaseStats.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/extras/dbStats/utilityDatabaseStats.py` & `pami-2023.7.7/PAMI/extras/dbStats/utilityDatabaseStats.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/extras/fuzzyTransformation/abstract.py` & `pami-2023.7.7/PAMI/extras/fuzzyTransformation/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/extras/fuzzyTransformation/temporalToFuzzy.py` & `pami-2023.7.7/PAMI/extras/fuzzyTransformation/temporalToFuzzy.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/extras/fuzzyTransformation/transactionalToFuzzyTimeSeries.py` & `pami-2023.7.7/PAMI/extras/fuzzyTransformation/transactionalToFuzzyTimeSeries.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/extras/fuzzyTransformation/utilityToFuzzy.py` & `pami-2023.7.7/PAMI/extras/fuzzyTransformation/utilityToFuzzy.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/extras/generateDatabase/generateSpatioTemporalDatabase.py` & `pami-2023.7.7/PAMI/extras/generateDatabase/generateSpatioTemporalDatabase.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/extras/generateDatabase/generateTemporalDatabase.py` & `pami-2023.7.7/PAMI/extras/generateDatabase/generateTemporalDatabase.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/extras/generateDatabase/generateTransactionalDatabase.py` & `pami-2023.7.7/PAMI/extras/generateDatabase/generateTransactionalDatabase.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/extras/generateLatexGraphFile.py` & `pami-2023.7.7/PAMI/extras/generateLatexGraphFile.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/extras/graph/dataFrameInToFigures.py` & `pami-2023.7.7/PAMI/extras/graph/dataFrameInToFigures.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/extras/graph/generateLatexFileFromDataFrame.py` & `pami-2023.7.7/PAMI/extras/graph/generateLatexFileFromDataFrame.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/extras/graph/plotLineGraphFromDictionary.py` & `pami-2023.7.7/PAMI/extras/graph/plotLineGraphFromDictionary.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/extras/graph/plotLineGraphsFromDataFrame.py` & `pami-2023.7.7/PAMI/extras/graph/plotLineGraphsFromDataFrame.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/extras/graph/visualizePatterns.py` & `pami-2023.7.7/PAMI/extras/graph/visualizePatterns.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/extras/imageProcessing/imagery2Databases.py` & `pami-2023.7.7/PAMI/extras/imageProcessing/imagery2Databases.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/extras/neighbours/findNeighboursUsingEuclidean.py` & `pami-2023.7.7/PAMI/extras/neighbours/findNeighboursUsingEuclidean.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/extras/plotPointOnMap.py` & `pami-2023.7.7/PAMI/extras/plotPointOnMap.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/extras/plotPointOnMap_dump.py` & `pami-2023.7.7/PAMI/extras/plotPointOnMap_dump.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/extras/scatterPlotSpatialPoints.py` & `pami-2023.7.7/PAMI/extras/scatterPlotSpatialPoints.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/extras/syntheticDatabaseGenerator/createSyntheticGeoreferentialTemporal.py` & `pami-2023.7.7/PAMI/extras/syntheticDatabaseGenerator/createSyntheticGeoreferentialTemporal.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,65 +4,65 @@
 
 class createSyntheticGeoreferentialTemporal:
     """
         This class create synthetic geo-referential temporal database. 
 
         Attribute:
         ----------
-        totalTransactions : int
+        transactions : pandas.DataFrame
             No of transactions
-        noOfItems : int or float
+        items : int or float
             No of items
-        avgTransactionLength : str
+        avgTransaction : str
             The length of average transaction
         outputFile: str
             Name of the output file.
 
         Methods:
         --------
-        createGeoreferentialTemporalDatabase(outputFile)
-            Create geo-referential temporal database and store into outputFile
+        getGeoreferentialTemporalDatabase(outputFile)
+            Create geo-referential temporal database store into outputFile
 
         Credits:
         ---------
              The complete program was written by  P.Likhitha   under the supervision of Professor Rage Uday Kiran.
 
     """
     
     def __init__(self, transactions, items, avgTransaction):
-        self._totalTransactions = transactions
-        self._noOfItems = items
-        self._avgTransactionLength = avgTransaction
+        self._transactions = transactions
+        self._items = items
+        self._avgTransaction = avgTransaction
     
     def createGeoreferentialTemporalDatabase(self, outputFile):
         """
         create transactional database and return outputFileName
         :param outputFile: file name or path to store database
         :type outputFile: str
         :return: outputFile name
         """
         writer = open(outputFile, 'w+')
         items = []
         count = 1
-        for i in range(self._noOfItems):
-            lat = _rd.randint(1, self._noOfItems)
-            lon = _rd.randint(1, self._noOfItems)
+        for i in range(self._items):
+            lat = _rd.randint(1, self._items)
+            lon = _rd.randint(1, self._items)
             if lat == lon:
-                lon = _rd.randint(1, self._noOfItems)
+                lon = _rd.randint(1, self._items)
             stt = '(' + str(lat) + ' ' + str(lon) + ')'
             items.append(stt)
-        for i in range(self._totalTransactions):
-            length = _rd.randint(1, self._avgTransactionLength + 20)
+        for i in range(self._transactions):
+            length = _rd.randint(1, self._avgTransaction + 20)
             st = str(count)
             for i in range(length):
                 rd = _rd.randint(0, len(items) - 1)
                 item = items[rd]
                 st = st + str(item) + '\t'
             writer.write("%s \n" % st)
             count += 1
             
 if __name__ == "__main__":
     _ap = str()
     _ap = createSyntheticGeoreferentialTemporal(100000, 870, 10)
     _ap.createGeoreferentialTemporalDatabase("T10_geo_temp.txt")
 else:
-    print("Error! The number of input parameters do not match the total number of parameters provided")
+    print("Error! The number of input parameters do not match the total number of parameters provided")
```

### Comparing `pami-2023.7.21/PAMI/extras/syntheticDatabaseGenerator/createSyntheticGeoreferentialTransactions.py` & `pami-2023.7.7/PAMI/extras/syntheticDatabaseGenerator/createSyntheticGeoreferentialTransactions.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,64 +4,64 @@
 
 class createSyntheticGeoreferentialTransaction:
     """
         This class create synthetic geo-referential transaction database. 
 
         Attribute:
         ----------
-        totalTransactions : int
+        transactions : pandas.DataFrame
             No of transactions
-        items : int 
+        items : int or float
             No of items
-        avgTransactionLength : str
+        avgTransaction : str
             The length of average transaction
         outputFile: str
             Name of the output file.
 
         Methods:
         --------
-        createGeoreferentialTransactionDatabase(outputFile)
-            Create geo-referential transactional database and store into outputFile
+        getGeoreferentialTransactionDatabase(outputFile)
+            Create geo-referential transactional database store into outputFile
 
 
         Credits:
         ---------
              The complete program was written by  P.Likhitha   under the supervision of Professor Rage Uday Kiran.
 
     """
     
     def __init__(self, transactions, items, avgTransaction):
-        self._totalTransactions = transactions
-        self._noOfItems = items
-        self._avgTransactionLength = avgTransaction
+        self._transactions = transactions
+        self._items = items
+        self._avgTransaction = avgTransaction
     
     def createGeoreferentialTransactionalDatabase(self, outputFile):
         """
         create transactional database and return outputFileName
         :param outputFile: file name or path to store database
         :type outputFile: str
         :return: outputFile name
         """
         writer = open(outputFile, 'w+')
         items = []
-        for i in range(self._noOfItems):
-            lat = _rd.randint(1, self._noOfItems)
-            lon = _rd.randint(1, self._noOfItems)
+        for i in range(self._items):
+            lat = _rd.randint(1, self._items)
+            lon = _rd.randint(1, self._items)
             if lat == lon:
-                lon = _rd.randint(1, self._noOfItems)
+                lon = _rd.randint(1, self._items)
             stt = '(' + str(lat) + ' ' + str(lon) + ')'
             items.append(stt)
-        for i in range(self._totalTransactions):
-            length = _rd.randint(1, self._avgTransactionLength + 20)
+        for i in range(self._transactions):
+            length = _rd.randint(1, self._avgTransaction + 20)
             st = str()
             for i in range(length):
                 rd = _rd.randint(0, len(items) - 1)
                 item = items[rd]
                 st = st + str(item) + '\t'
             writer.write("%s \n" % st)
             
 if __name__ == "__main__":
     _ap = str()
     _ap = createSyntheticGeoreferentialTransaction(100000, 870, 10)
     _ap.createGeoreferentialTransactionalDatabase("T10_geo.txt")
 else:
-    print("Error! The number of input parameters do not match the total number of parameters provided")
+    print("Error! The number of input parameters do not match the total number of parameters provided")
```

### Comparing `pami-2023.7.21/PAMI/extras/syntheticDatabaseGenerator/createSyntheticGeoreferentialUncertainTransaction.py` & `pami-2023.7.7/PAMI/extras/syntheticDatabaseGenerator/createSyntheticGeoreferentialUncertainTransaction.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,64 +1,64 @@
 import random as _rd
 import sys as _sys
 
 
 class createSyntheticGeoreferentialUncertainTransaction:
     """
-        This class is to create synthetic geo-referential uncertain transaction database. 
+        This class create synthetic geo-referential uncertain transaction database. 
 
         Attribute:
         ----------
-        totalTransactions : int
+        transactions : pandas.DataFrame
             No of transactions
-        noOfItems : int 
+        items : int or float
             No of items
-        avgTransactionLength : int
+        avgTransaction : str
             The length of average transaction
         outputFile: str
             Name of the output file.
 
         Methods:
         --------
-        createGeoreferentialuncertainTransactionDatabase(outputFile)
+        getGeoreferentialuncertainTransactionDatabase(outputFile)
             Create geo-referential transactional database store into outputFile
 
         Credits:
         ---------
              The complete program was written by  P.Likhitha   under the supervision of Professor Rage Uday Kiran.
 
 
 
 
 
     """
     
     def __init__(self, transactions, items, avgTransaction):
-        self._totalTransactions = transactions
-        self._noOfItems = items
-        self._avgTransactionLength = avgTransaction
+        self._transactions = transactions
+        self._items = items
+        self._avgTransaction = avgTransaction
     
     def createGeoreferentialUncertainTransactionalDatabase(self, outputFile):
         """
         create transactional database and return outputFileName
         :param outputFile: file name or path to store database
         :type outputFile: str
         :return: outputFile name
         """
         writer = open(outputFile, 'w+')
         items = []
-        for i in range(self._noOfItems):
-            lat = _rd.randint(1, self._noOfItems)
-            lon = _rd.randint(1, self._noOfItems)
+        for i in range(self._items):
+            lat = _rd.randint(1, self._items)
+            lon = _rd.randint(1, self._items)
             if lat == lon:
-                lon = _rd.randint(1, self._noOfItems)
+                lon = _rd.randint(1, self._items)
             stt = '(' + str(lat) + ' ' + str(lon) + ')'
             items.append(stt)
-        for i in range(self._totalTransactions):
-            length = _rd.randint(1, self._avgTransactionLength + 20)
+        for i in range(self._transactions):
+            length = _rd.randint(1, self._avgTransaction + 20)
             st = str()
             st1 = str()
             for i in range(length):
                 rd = _rd.randint(0, len(items) - 1)
                 item = items[rd]
                 probability = _rd.uniform(0, 1)
                 st = st + str(item) + '\t'
@@ -68,8 +68,8 @@
             writer.write("%s \n" % st1)
             
 if __name__ == "__main__":
     _ap = str()
     _ap = createSyntheticGeoreferentialUncertainTransaction(100000, 870, 10)
     _ap.createGeoreferentialUncertainTransactionalDatabase("T10_geo_un.txt")
 else:
-    print("Error! The number of input parameters do not match the total number of parameters provided")
+    print("Error! The number of input parameters do not match the total number of parameters provided")
```

### Comparing `pami-2023.7.21/PAMI/extras/syntheticDatabaseGenerator/createSyntheticTemporal.py` & `pami-2023.7.7/PAMI/extras/syntheticDatabaseGenerator/createSyntheticTemporal.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/extras/syntheticDatabaseGenerator/createSyntheticTransactions.py` & `pami-2023.7.7/PAMI/extras/syntheticDatabaseGenerator/createSyntheticTransactions.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/extras/syntheticDatabaseGenerator/createSyntheticUncertainTemporal.py` & `pami-2023.7.7/PAMI/extras/syntheticDatabaseGenerator/createSyntheticUncertainTemporal.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     """
         This class create synthetic temporal database. 
 
         Attribute:
         ----------
         totalTransactions : int
             Total no of transactions
-        noOfItems : int 
+        items : int 
             No of items
         avgTransactionLength : int
             The length of average transaction
         outputFile: str
             Name of the output file.
 
         Methods:
@@ -29,15 +29,15 @@
 
 
     """
     
     def __init__(self, totalTransactions, items, avgTransaction):
         self._totalTransactions = totalTransactions
         self._items = items
-        self._avgTransactionLength = avgTransaction
+        self._avgTransactionLength = avgTransactionLength
     
     def createUncertainTemporalDatabase(self, outputFile):
         """
         create transactional database and return outputFileName
         :param outputFile: file name or path to store database
         :type outputFile: str
         :return: outputFile name
@@ -45,15 +45,15 @@
         writer = open(outputFile, 'w+')
         count = 1
         for i in range(self._totalTransactions):
             length = _rd.randint(1, self._avgTransactionLength + 20)
             st = str(count) + '\t'
             st1 = str()
             for i in range(length):
-                item = _rd.randint(1, self._noOfItems)
+                item = _rd.randint(1, self._items)
                 probability = _rd.uniform(0, 1)
                 st = st + str(item) + '\t'
                 st1 = st1 + str(probability) + '\t'
             writer.write("%s:" % st)
             writer.write("%s \n" % st1)
             count += 1
```

### Comparing `pami-2023.7.21/PAMI/extras/syntheticDatabaseGenerator/createSyntheticUncertainTransactions.py` & `pami-2023.7.7/PAMI/extras/syntheticDatabaseGenerator/createSyntheticUncertainTransactions.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     """
         This class create synthetic transaction database. 
 
         Attribute:
         ----------
         totalTransactions : int
             No of transactions
-        noOfItems : int 
+        items : int 
             No of items
         avgTransactionLength : str
             The length of average transaction
         outputFile: str
             Name of the output file.
 
         Nethods:
```

### Comparing `pami-2023.7.21/PAMI/extras/syntheticDatabaseGenerator/createSyntheticUtility.py` & `pami-2023.7.7/PAMI/extras/syntheticDatabaseGenerator/createSyntheticUtility.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,15 +10,15 @@
         ----------
         totalTransactions : int
             No of transactions
         noOfItems : int 
             No of items
         maxUtilRange: int
             Maximum utility range
-        avgTransactionLength : int
+        avgTransactionLength : str
             The length of average transaction
         outputFile: str
             Name of the output file.
 
         Nethods:
         --------
         createUtilitylDatabase(outputFile)
```

### Comparing `pami-2023.7.21/PAMI/extras/topKPatterns.py` & `pami-2023.7.7/PAMI/extras/topKPatterns.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/faultTolerantFrequentPattern/basic/FTApriori.py` & `pami-2023.7.7/PAMI/faultTolerantFrequentPattern/basic/FTApriori.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/faultTolerantFrequentPattern/basic/FTFPGrowth.py` & `pami-2023.7.7/PAMI/faultTolerantFrequentPattern/basic/FTFPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/faultTolerantFrequentPattern/basic/VBFTMine.py` & `pami-2023.7.7/PAMI/faultTolerantFrequentPattern/basic/VBFTMine.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 #
 # import PAMI.faultTolerantFrequentPattern.basic.VBFTMine as alg
 #
 # obj = alg.VBFTMine(iFile, minSup, itemSup, minLength, faultTolerance)
 #
 # obj.startMine()
 #
-# faultTolerantFrequentPattern = obj.getPatterns()
+# faultTolerantFrequentPatterns = obj.getPatterns()
 #
-# print("Total number of Fault Tolerant Frequent Patterns:", len(faultTolerantFrequentPattern))
+# print("Total number of Fault Tolerant Frequent Patterns:", len(faultTolerantFrequentPatterns))
 #
 # obj.save(oFile)
 #
 # Df = obj.getPatternInDataFrame()
 #
 # print("Total Memory in USS:", obj.getMemoryUSS())
 #
@@ -112,17 +112,17 @@
     
         import PAMI.faultTolerantFrequentPattern.basic.VBFTMine as alg
 
         obj = alg.VBFTMine(iFile, minSup, itemSup, minLength, faultTolerance)
 
         obj.startMine()
 
-        faultTolerantFrequentPattern = obj.getPatterns()
+        faultTolerantFrequentPatterns = obj.getPatterns()
 
-        print("Total number of Fault Tolerant Frequent Patterns:", len(faultTolerantFrequentPattern))
+        print("Total number of Fault Tolerant Frequent Patterns:", len(faultTolerantFrequentPatterns))
 
         obj.save(oFile)
 
         Df = obj.getPatternInDataFrame()
 
         print("Total Memory in USS:", obj.getMemoryUSS())
```

### Comparing `pami-2023.7.21/PAMI/faultTolerantFrequentPattern/basic/abstract.py` & `pami-2023.7.7/PAMI/faultTolerantFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/frequentPattern/__init__.py` & `pami-2023.7.7/PAMI/frequentPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/frequentPattern/basic/Apriori.py` & `pami-2023.7.7/PAMI/frequentPattern/basic/Apriori.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/frequentPattern/basic/ECLAT.py` & `pami-2023.7.7/PAMI/frequentPattern/basic/ECLAT.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/frequentPattern/basic/ECLATDiffset.py` & `pami-2023.7.7/PAMI/frequentPattern/basic/ECLATDiffset.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/frequentPattern/basic/ECLATbitset.py` & `pami-2023.7.7/PAMI/frequentPattern/basic/ECLATbitset.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/frequentPattern/basic/FPGrowth.py` & `pami-2023.7.7/PAMI/frequentPattern/basic/FPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/frequentPattern/basic/abstract.py` & `pami-2023.7.7/PAMI/frequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/frequentPattern/closed/CHARM.py` & `pami-2023.7.7/PAMI/frequentPattern/closed/CHARM.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/frequentPattern/closed/abstract.py` & `pami-2023.7.7/PAMI/frequentPattern/closed/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/frequentPattern/cuda/abstract.py` & `pami-2023.7.7/PAMI/frequentPattern/cuda/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/frequentPattern/cuda/cuApriori.py` & `pami-2023.7.7/PAMI/frequentPattern/cuda/cuApriori.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/frequentPattern/cuda/cuAprioriBit.py` & `pami-2023.7.7/PAMI/frequentPattern/cuda/cuAprioriBit.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/frequentPattern/cuda/cuEclat.py` & `pami-2023.7.7/PAMI/frequentPattern/cuda/cuEclat.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/frequentPattern/cuda/cuEclatBit.py` & `pami-2023.7.7/PAMI/frequentPattern/cuda/cuEclatBit.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/frequentPattern/cuda/cudaAprioriGCT.py` & `pami-2023.7.7/PAMI/frequentPattern/cuda/cudaAprioriGCT.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/frequentPattern/cuda/cudaAprioriTID.py` & `pami-2023.7.7/PAMI/frequentPattern/cuda/cudaAprioriTID.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/frequentPattern/cuda/cudaEclatGCT.py` & `pami-2023.7.7/PAMI/frequentPattern/cuda/cudaEclatGCT.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/frequentPattern/maximal/MaxFPGrowth.py` & `pami-2023.7.7/PAMI/frequentPattern/maximal/MaxFPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/frequentPattern/maximal/__init__.py` & `pami-2023.7.7/PAMI/frequentPattern/maximal/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/frequentPattern/maximal/abstract.py` & `pami-2023.7.7/PAMI/fuzzyFrequentPatterns/basic/abstract.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,23 +34,24 @@
 from itertools import combinations as _c
 import os as _os
 import os.path as _ospath
 import psutil as _psutil
 import sys as _sys
 import validators as _validators
 from urllib.request import urlopen as _urlopen
+import functools as _functools
 
 
-class _frequentPatterns(_ABC):
+class _fuzzyFrequentPattenrs(_ABC):
     """ This abstract base class defines the variables and methods that every frequent pattern mining algorithm must
         employ in PAMI
 
 
-       Attributes:
-       ----------
+    Attributes :
+    ----------
         iFile : str
             Input file name or path of the input file
         minSup: integer or float or str
             The user can specify minSup either in count or proportion of database size.
             If the program detects the data type of minSup is integer, then it treats minSup is expressed in count.
             Otherwise, it will be treated as float.
             Example: minSup=10 will be treated as integer, while minSup=10.0 will be treated as float
@@ -66,16 +67,16 @@
         oFile : str
             Name of the output file to store complete set of frequent patterns
         memoryUSS : float
             To store the total amount of USS memory consumed by the program
         memoryRSS : float
             To store the total amount of RSS memory consumed by the program
 
-       Methods:
-       -------
+    Methods :
+    -------
         startMine()
             Calling this function will start the actual mining process
         getPatterns()
             This function will output all interesting patterns discovered by an algorithm
         save(oFile)
             This function will store the discovered patterns in an output file specified by the user
         getPatternsAsDataFrame()
@@ -88,34 +89,33 @@
             This function outputs the total runtime of a mining algorithm
 
     """
 
     def __init__(self, iFile, minSup, sep="\t"):
         """
         :param iFile: Input file name or path of the input file
-        :type iFile: str or DataFrame
+        :type iFile: str
         :param minSup: The user can specify minSup either in count or proportion of database size.
             If the program detects the data type of minSup is integer, then it treats minSup is expressed in count.
             Otherwise, it will be treated as float.
             Example: minSup=10 will be treated as integer, while minSup=10.0 will be treated as float
         :type minSup: int or float or str
         :param sep: separator used to distinguish items from each other. The default separator is tab space. However, users can override the default separator
         :type sep: str
         """
 
         self._iFile = iFile
         self._sep = sep
         self._minSup = minSup
-        self._finalPatterns = {}
-        self._oFile = str()
         self._startTime = float()
         self._endTime = float()
-        self._memoryRSS = float()
         self._memoryUSS = float()
-
+        self._memoryRSS = float()
+        self._oFile = str()
+        self._finalPatterns = {}
 
     @_abstractmethod
     def startMine(self):
         """Code for the mining process will start from this function"""
 
         pass
 
@@ -154,14 +154,14 @@
         pass
 
 
     @_abstractmethod
     def getRuntime(self):
         """Total amount of runtime taken by the program will be retrieved from this function"""
 
-        pass
+
 
     @_abstractmethod
     def printResults(self):
-        """To print the statistics."""
+        """ To print all the results of execution"""
 
         pass
```

### Comparing `pami-2023.7.21/PAMI/frequentPattern/pyspark/abstract.py` & `pami-2023.7.7/PAMI/frequentPattern/pyspark/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/frequentPattern/pyspark/parallelApriori.py` & `pami-2023.7.7/PAMI/frequentPattern/pyspark/parallelApriori.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/frequentPattern/pyspark/parallelECLAT.py` & `pami-2023.7.7/PAMI/frequentPattern/pyspark/parallelECLAT.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/frequentPattern/pyspark/parallelFPGrowth.py` & `pami-2023.7.7/PAMI/frequentPattern/pyspark/parallelFPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/frequentPattern/topk/FAE.py` & `pami-2023.7.7/PAMI/frequentPattern/topk/FAE.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/frequentPattern/topk/abstract.py` & `pami-2023.7.7/PAMI/frequentPattern/topk/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/frequentSpatialPattern/__init__.py` & `pami-2023.7.7/PAMI/frequentSpatialPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/frequentSpatialPattern/basic/FSPGrowth.py` & `pami-2023.7.7/PAMI/frequentSpatialPattern/basic/FSPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/frequentSpatialPattern/basic/SpatialECLAT.py` & `pami-2023.7.7/PAMI/frequentSpatialPattern/basic/SpatialECLAT.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/frequentSpatialPattern/basic/abstract.py` & `pami-2023.7.7/PAMI/georeferencedFrequentSequencePattern/abstract.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,19 +37,17 @@
 import psutil as _psutil
 import sys as _sys
 import validators as _validators
 from urllib.request import urlopen as _urlopen
 from collections import OrderedDict as _OrderedDict
 
 
-class _spatialFrequentPatterns(_ABC):
+class _sequentialSpatialPatterns(_ABC):
     """ This abstract base class defines the variables and methods that every frequent pattern mining algorithm must
         employ in PAMI
-
-
     Attributes :
     ----------
         iFile : str
             Input file name or path of the input file
         nFile: str
             Neighbourhoof file name
         minSup: integer or float or str
@@ -68,15 +66,14 @@
             Storing the complete set of patterns in a dictionary variable
         oFile : str
             Name of the output file to store complete set of frequent patterns
         memoryUSS : float
             To store the total amount of USS memory consumed by the program
         memoryRSS : float
             To store the total amount of RSS memory consumed by the program
-
     Methods :
     -------
         startMine()
             Calling this function will start the actual mining process
         getPatterns()
             This function will output all interesting patterns discovered by an algorithm
         save(oFile)
@@ -85,15 +82,14 @@
             The function outputs the patterns generated by an algorithm as a data frame
         getMemoryUSS()
             This function outputs the total amount of USS memory consumed by a mining algorithm
         getMemoryRSS()
             This function outputs the total amount of RSS memory consumed by a mining algorithm
         getRuntime()
             This function outputs the total runtime of a mining algorithm
-
     """
 
     def __init__(self, iFile, nFile, minSup, sep="\t"):
         """
         :param iFile: Input file name or path of the input file
         :type iFile: str
         :param nFile: Neighbourhood name of the input
@@ -131,15 +127,14 @@
         """Complete set of frequent patterns generated will be retrieved from this function"""
 
         pass
 
     @_abstractmethod
     def save(self, oFile):
         """Complete set of frequent patterns will be saved in to an output file from this function
-
         :param oFile: Name of the output file
         :type oFile: file
         """
 
         pass
 
     @_abstractmethod
@@ -168,8 +163,8 @@
         pass
 
     @_abstractmethod
     def printResults(self):
 
         """ To print the results of execution"""
 
-        pass
+        pass
```

### Comparing `pami-2023.7.21/PAMI/fuzzyCorrelatedPattern/__init__.py` & `pami-2023.7.7/PAMI/fuzzyCorrelatedPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/fuzzyCorrelatedPattern/basic/FCPGrowth.py` & `pami-2023.7.7/PAMI/fuzzyCorrelatedPattern/basic/FCPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/fuzzyCorrelatedPattern/basic/__init__.py` & `pami-2023.7.7/PAMI/fuzzyCorrelatedPattern/basic/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/fuzzyCorrelatedPattern/basic/abstract.py` & `pami-2023.7.7/PAMI/fuzzyCorrelatedPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/fuzzyFrequentPattern/__init__.py` & `pami-2023.7.7/PAMI/fuzzyFrequentPatterns/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/fuzzyFrequentPattern/basic/FFIMiner.py` & `pami-2023.7.7/PAMI/fuzzyFrequentPatterns/basic/FFIMiner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # **Importing this algorithm into a python program**
 # --------------------------------------------------------
 #
-#     from PAMI.fuzzyFrequentPattern import FFIMiner as alg
+#     from PAMI.fuzzyFrequentPatterns import FFIMiner as alg
 #
 #     obj = alg.FFIMiner("input.txt", 2)
 #
 #     obj.startMine()
 #
-#     fuzzyFrequentPattern = obj.getPatterns()
+#     fuzzyFrequentPatterns = obj.getPatterns()
 #
-#     print("Total number of Fuzzy Frequent Patterns:", len(fuzzyFrequentPattern))
+#     print("Total number of Fuzzy Frequent Patterns:", len(fuzzyFrequentPatterns))
 #
 #     obj.save("outputFile")
 #
 #     memUSS = obj.getMemoryUSS()
 #
 #     print("Total Memory in USS:", memUSS)
 #
@@ -42,15 +42,15 @@
 
      You should have received a copy of the GNU General Public License
      along with this program.  If not, see <https://www.gnu.org/licenses/>.
      Copyright (C)  2021 Rage Uday Kiran
 
 """
 
-from PAMI.fuzzyFrequentPattern.basic import abstract as _ab
+from PAMI.fuzzyFrequentPatterns.basic import abstract as _ab
 
 
 class _FFList:
     """
      A class represent a Fuzzy List of an element
 
     Attributes :
@@ -217,23 +217,23 @@
             >>> python3  FFIMiner.py sampleTDB.txt output.txt 6  (minSup will be considered in support count or frequency)
 
 
     Sample run of importing the code:
     ----------------------------------
     .. code-block:: python
 
-        from PAMI.fuzzyFrequentPattern import FFIMiner as alg
+        from PAMI.fuzzyFrequentPatterns import FFIMiner as alg
 
         obj = alg.FFIMiner("input.txt", 2)
 
         obj.startMine()
 
-        fuzzyFrequentPattern = obj.getPatterns()
+        fuzzyFrequentPatterns = obj.getPatterns()
 
-        print("Total number of Fuzzy Frequent Patterns:", len(fuzzyFrequentPattern))
+        print("Total number of Fuzzy Frequent Patterns:", len(fuzzyFrequentPatterns))
 
         obj.save("outputFile")
 
         memUSS = obj.getMemoryUSS()
 
         print("Total Memory in USS:", memUSS)
```

### Comparing `pami-2023.7.21/PAMI/fuzzyFrequentPattern/basic/FFIMiner_old.py` & `pami-2023.7.7/PAMI/fuzzyFrequentPatterns/basic/FFIMiner_old.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 
-from PAMI.fuzzyFrequentPattern.basic import abstract as _ab
+from PAMI.fuzzyFrequentPatterns.basic import abstract as _ab
 
 
 class _FFList:
     """
      A class represent a Fuzzy List of an element
 
     Attributes :
@@ -203,23 +203,23 @@
                                                       (it will consider '\t' as a separator)
 
             python3  FFIMinerMiner.py sampleTDB.txt output.txt 6 , (it consider ',' as a separator)
 
     Sample run of importing the code:
     -------------------------------
 
-        from PAMI.fuzzyFrequentPattern import FFIMiner as alg
+        from PAMI.fuzzyFrequentPatterns import FFIMiner as alg
 
         obj = alg.FFIMiner("input.txt", "fuzzyMembership.txt" 2)
 
         obj.startMine()
 
-        fuzzyFrequentPattern = obj.getPatterns()
+        fuzzyFrequentPatterns = obj.getPatterns()
 
-        print("Total number of Fuzzy Frequent Patterns:", len(fuzzyFrequentPattern))
+        print("Total number of Fuzzy Frequent Patterns:", len(fuzzyFrequentPatterns))
 
         obj.save("outputFile")
 
         memUSS = obj.getMemoryUSS()
 
         print("Total Memory in USS:", memUSS)
```

### Comparing `pami-2023.7.21/PAMI/fuzzyFrequentPattern/basic/abstract.py` & `pami-2023.7.7/PAMI/fuzzyPartialPeriodicPatterns/irregularTimeSeries/abstract.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 import psutil as _psutil
 import sys as _sys
 import validators as _validators
 from urllib.request import urlopen as _urlopen
 import functools as _functools
 
 
-class _fuzzyFrequentPattenrs(_ABC):
+class _fuzzyPartialPattenrs(_ABC):
     """ This abstract base class defines the variables and methods that every frequent pattern mining algorithm must
         employ in PAMI
 
 
     Attributes :
     ----------
         iFile : str
```

### Comparing `pami-2023.7.21/PAMI/fuzzyFrequentSpatialPattern/__init__.py` & `pami-2023.7.7/PAMI/fuzzyFrequentSpatialPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/fuzzyFrequentSpatialPattern/basic/FFSPMiner.py` & `pami-2023.7.7/PAMI/fuzzyFrequentSpatialPattern/basic/FFSPMiner.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/fuzzyFrequentSpatialPattern/basic/FFSPMiner_old.py` & `pami-2023.7.7/PAMI/fuzzyFrequentSpatialPattern/basic/FFSPMiner_old.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/fuzzyFrequentSpatialPattern/basic/abstract.py` & `pami-2023.7.7/PAMI/fuzzyFrequentSpatialPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/fuzzyPartialPeriodicPattern/irregularTimeSeries/abstract.py` & `pami-2023.7.7/PAMI/sequentialPatternMining/basic/abstract.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 #      but WITHOUT ANY WARRANTY; without even the implied warranty of
 #      MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #      GNU General Public License for more details.
 #
 #      You should have received a copy of the GNU General Public License
 #      along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
+# from abc import ABC as _ABC, abstractmethod as _abstractmethod
 from abc import ABC as _ABC, abstractmethod as _abstractmethod
 import time as _time
 import csv as _csv
 import pandas as _pd
 from collections import defaultdict as _defaultdict
 from itertools import combinations as _c
 import os as _os
@@ -37,20 +38,20 @@
 import psutil as _psutil
 import sys as _sys
 import validators as _validators
 from urllib.request import urlopen as _urlopen
 import functools as _functools
 
 
-class _fuzzyPartialPattenrs(_ABC):
-    """ This abstract base class defines the variables and methods that every frequent pattern mining algorithm must
+class _sequentialPatterns(_ABC):
+    """
+    This abstract base class defines the variables and methods that every frequent pattern mining algorithm in sequential databases must
         employ in PAMI
 
-
-    Attributes :
+    Attributes:
     ----------
         iFile : str
             Input file name or path of the input file
         minSup: integer or float or str
             The user can specify minSup either in count or proportion of database size.
             If the program detects the data type of minSup is integer, then it treats minSup is expressed in count.
             Otherwise, it will be treated as float.
@@ -67,15 +68,15 @@
         oFile : str
             Name of the output file to store complete set of frequent patterns
         memoryUSS : float
             To store the total amount of USS memory consumed by the program
         memoryRSS : float
             To store the total amount of RSS memory consumed by the program
 
-    Methods :
+    Methods:
     -------
         startMine()
             Calling this function will start the actual mining process
         getPatterns()
             This function will output all interesting patterns discovered by an algorithm
         save(oFile)
             This function will store the discovered patterns in an output file specified by the user
@@ -83,39 +84,38 @@
             The function outputs the patterns generated by an algorithm as a data frame
         getMemoryUSS()
             This function outputs the total amount of USS memory consumed by a mining algorithm
         getMemoryRSS()
             This function outputs the total amount of RSS memory consumed by a mining algorithm
         getRuntime()
             This function outputs the total runtime of a mining algorithm
-
     """
 
     def __init__(self, iFile, minSup, sep="\t"):
         """
         :param iFile: Input file name or path of the input file
-        :type iFile: str
+        :type iFile: str or DataFrame
         :param minSup: The user can specify minSup either in count or proportion of database size.
             If the program detects the data type of minSup is integer, then it treats minSup is expressed in count.
             Otherwise, it will be treated as float.
             Example: minSup=10 will be treated as integer, while minSup=10.0 will be treated as float
         :type minSup: int or float or str
         :param sep: separator used to distinguish items from each other. The default separator is tab space. However, users can override the default separator
         :type sep: str
         """
 
         self._iFile = iFile
         self._sep = sep
         self._minSup = minSup
-        self._startTime = float()
-        self._endTime = float()
+        self._finalPatterns = {}
+        self._oFile = str()
         self._memoryUSS = float()
         self._memoryRSS = float()
-        self._oFile = str()
-        self._finalPatterns = {}
+        self._startTime = float()
+        self._endTime = float()
 
     @_abstractmethod
     def startMine(self):
         """Code for the mining process will start from this function"""
 
         pass
 
@@ -124,15 +124,14 @@
         """Complete set of frequent patterns generated will be retrieved from this function"""
 
         pass
 
     @_abstractmethod
     def save(self, oFile):
         """Complete set of frequent patterns will be saved in to an output file from this function
-
         :param oFile: Name of the output file
         :type oFile: file
         """
 
         pass
 
     @_abstractmethod
@@ -149,19 +148,18 @@
 
     @_abstractmethod
     def getMemoryRSS(self):
         """Total amount of RSS memory consumed by the program will be retrieved from this function"""
 
         pass
 
-
     @_abstractmethod
     def getRuntime(self):
         """Total amount of runtime taken by the program will be retrieved from this function"""
 
-
+        pass
 
     @_abstractmethod
     def printResults(self):
-        """ To print all the results of execution"""
+        """ To print result of the execution"""
 
         pass
```

### Comparing `pami-2023.7.21/PAMI/fuzzyPeriodicFrequentPattern/__init__.py` & `pami-2023.7.7/PAMI/fuzzyPeriodicFrequentPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/fuzzyPeriodicFrequentPattern/basic/FPFPMiner.py` & `pami-2023.7.7/PAMI/fuzzyPeriodicFrequentPattern/basic/FPFPMiner.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/fuzzyPeriodicFrequentPattern/basic/FPFPMiner_old.py` & `pami-2023.7.7/PAMI/fuzzyPeriodicFrequentPattern/basic/FPFPMiner_old.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/fuzzyPeriodicFrequentPattern/basic/__init__.py` & `pami-2023.7.7/PAMI/fuzzyPeriodicFrequentPattern/basic/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/fuzzyPeriodicFrequentPattern/basic/abstract.py` & `pami-2023.7.7/PAMI/fuzzyPeriodicFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/fuzzySpatialPeriodicFrequentPattern/basic/FGPFPMiner.py` & `pami-2023.7.7/PAMI/fuzzySpatialPeriodicFrequentPattern/basic/FGPFPMiner.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/fuzzySpatialPeriodicFrequentPattern/basic/FGPFPMiner_old.py` & `pami-2023.7.7/PAMI/fuzzySpatialPeriodicFrequentPattern/basic/FGPFPMiner_old.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/fuzzySpatialPeriodicFrequentPattern/basic/abstract.py` & `pami-2023.7.7/PAMI/fuzzySpatialPeriodicFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/geoReferencedFrequentPattern/GFPGrowth.py` & `pami-2023.7.7/PAMI/geoReferencedFrequentPattern/GFPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/geoReferencedFrequentPattern/abstract.py` & `pami-2023.7.7/PAMI/geoReferencedFrequentPattern/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/geoReferencedPeriodicFrequentPattern/basic/GPFPMiner.py` & `pami-2023.7.7/PAMI/geoReferencedPeriodicFrequentPattern/basic/GPFPMiner.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/geoReferencedPeriodicFrequentPattern/basic/abstract.py` & `pami-2023.7.7/PAMI/geoReferencedPeriodicFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/georeferencedFrequentSequencePattern/abstract.py` & `pami-2023.7.7/PAMI/AssociationRules/basic/abstract.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,38 +22,39 @@
 #      but WITHOUT ANY WARRANTY; without even the implied warranty of
 #      MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #      GNU General Public License for more details.
 #
 #      You should have received a copy of the GNU General Public License
 #      along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
+# from abc import ABC as _ABC, abstractmethod as _abstractmethod
 from abc import ABC as _ABC, abstractmethod as _abstractmethod
 import time as _time
 import csv as _csv
 import pandas as _pd
 from collections import defaultdict as _defaultdict
 from itertools import combinations as _c
 import os as _os
 import os.path as _ospath
 import psutil as _psutil
 import sys as _sys
 import validators as _validators
 from urllib.request import urlopen as _urlopen
-from collections import OrderedDict as _OrderedDict
+import functools as _functools
 
 
-class _sequentialSpatialPatterns(_ABC):
+class _AssociationRules(_ABC):
     """ This abstract base class defines the variables and methods that every frequent pattern mining algorithm must
         employ in PAMI
-    Attributes :
-    ----------
+
+
+       Attributes:
+       ----------
         iFile : str
             Input file name or path of the input file
-        nFile: str
-            Neighbourhoof file name
         minSup: integer or float or str
             The user can specify minSup either in count or proportion of database size.
             If the program detects the data type of minSup is integer, then it treats minSup is expressed in count.
             Otherwise, it will be treated as float.
             Example: minSup=10 will be treated as integer, while minSup=10.0 will be treated as float
         sep : str
             This variable is used to distinguish items from one another in a transaction. The default seperator is tab space or \t.
@@ -66,59 +67,56 @@
             Storing the complete set of patterns in a dictionary variable
         oFile : str
             Name of the output file to store complete set of frequent patterns
         memoryUSS : float
             To store the total amount of USS memory consumed by the program
         memoryRSS : float
             To store the total amount of RSS memory consumed by the program
-    Methods :
-    -------
+
+       Methods:
+       -------
         startMine()
             Calling this function will start the actual mining process
         getPatterns()
             This function will output all interesting patterns discovered by an algorithm
         save(oFile)
             This function will store the discovered patterns in an output file specified by the user
         getPatternsAsDataFrame()
             The function outputs the patterns generated by an algorithm as a data frame
         getMemoryUSS()
             This function outputs the total amount of USS memory consumed by a mining algorithm
         getMemoryRSS()
             This function outputs the total amount of RSS memory consumed by a mining algorithm
         getRuntime()
             This function outputs the total runtime of a mining algorithm
+
     """
 
-    def __init__(self, iFile, nFile, minSup, sep="\t"):
+    def __init__(self, iFile, threshold, sep="\t"):
         """
         :param iFile: Input file name or path of the input file
-        :type iFile: str
-        :param nFile: Neighbourhood name of the input
-        :type nFile: str
+        :type iFile: str or DataFrame
         :param minSup: The user can specify minSup either in count or proportion of database size.
             If the program detects the data type of minSup is integer, then it treats minSup is expressed in count.
             Otherwise, it will be treated as float.
             Example: minSup=10 will be treated as integer, while minSup=10.0 will be treated as float
         :type minSup: int or float or str
         :param sep: separator used to distinguish items from each other. The default separator is tab space. However, users can override the default separator
         :type sep: str
         """
 
         self._iFile = iFile
-        self._nFile = nFile
-        self._oFile = str()
         self._sep = sep
-        self._minSup = minSup
-        self._startTime = float()
-        self._endTime = float()
-        self._memoryUSS = float()
-        self._memoryRSS = float()
+        self._threshold = threshold
         self._finalPatterns = {}
         self._oFile = str()
-
+        self._memoryUSS = float()
+        self._memoryRSS = float()
+        self._startTime = float()
+        self._endTime = float()
 
     @_abstractmethod
     def startMine(self):
         """Code for the mining process will start from this function"""
 
         pass
 
@@ -127,14 +125,15 @@
         """Complete set of frequent patterns generated will be retrieved from this function"""
 
         pass
 
     @_abstractmethod
     def save(self, oFile):
         """Complete set of frequent patterns will be saved in to an output file from this function
+
         :param oFile: Name of the output file
         :type oFile: file
         """
 
         pass
 
     @_abstractmethod
@@ -151,20 +150,18 @@
 
     @_abstractmethod
     def getMemoryRSS(self):
         """Total amount of RSS memory consumed by the program will be retrieved from this function"""
 
         pass
 
-
     @_abstractmethod
     def getRuntime(self):
         """Total amount of runtime taken by the program will be retrieved from this function"""
 
         pass
 
     @_abstractmethod
     def printResults(self):
-
-        """ To print the results of execution"""
+        """ To print result of the execution"""
 
         pass
```

### Comparing `pami-2023.7.21/PAMI/highUtilityFrequentPattern/basic/HUFIM.py` & `pami-2023.7.7/PAMI/highUtilityFrequentPatterns/basic/HUFIM.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 # **Importing this algorithm into a python program**
 # --------------------------------------------------------
 #
 #
-#     from PAMI.highUtilityFrequentPattern.basic import HUFIM as alg
+#     from PAMI.highUtilityFrequentPatterns.basic import HUFIM as alg
 #
 #     ob j =alg.HUFIM("input.txt", 35, 20)
 #
 #     obj.startMine()
 #
 #     Patterns = obj.getPatterns()
 #
@@ -45,15 +45,15 @@
      You should have received a copy of the GNU General Public License
      along with this program.  If not, see <https://www.gnu.org/licenses/>.
      Copyright (C)  2021 Rage Uday Kiran
 
 """
 
 
-from PAMI.highUtilityFrequentPattern.basic import abstract as _ab
+from PAMI.highUtilityFrequentPatterns.basic import abstract as _ab
 
 
 class _Transaction:
     """
         A class to store Transaction of a database
 
     Attributes:
@@ -396,15 +396,15 @@
 
             >>>  python3 HUFIM.py sampleTDB.txt output.txt 35 20 , (it will consider "," as separator)
 
     Sample run of importing the code:
     -------------------------------
     .. code-block:: python
 
-        from PAMI.highUtilityFrequentPattern.basic import HUFIM as alg
+        from PAMI.highUtilityFrequentPatterns.basic import HUFIM as alg
 
         obj=alg.HUFIM("input.txt", 35, 20)
 
         obj.startMine()
 
         Patterns = obj.getPatterns()
```

### Comparing `pami-2023.7.21/PAMI/highUtilityFrequentPattern/basic/abstract.py` & `pami-2023.7.7/PAMI/highUtilityFrequentPatterns/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/highUtilityFrequentSpatialPattern/__init__.py` & `pami-2023.7.7/PAMI/highUtilityFrequentSpatialPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/highUtilityFrequentSpatialPattern/basic/SHUFIM.py` & `pami-2023.7.7/PAMI/highUtilityFrequentSpatialPattern/basic/SHUFIM.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/highUtilityFrequentSpatialPattern/basic/abstract.py` & `pami-2023.7.7/PAMI/highUtilityFrequentSpatialPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/highUtilityPattern/basic/EFIM.py` & `pami-2023.7.7/PAMI/highUtilityPatterns/basic/EFIM.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 # **Importing this algorithm into a python program**
 # --------------------------------------------------------
 #
-#         from PAMI.highUtilityPattern.basic import EFIM as alg
+#         from PAMI.highUtilityPatterns.basic import EFIM as alg
 #
 #         obj=alg.EFIM("input.txt",35)
 #
 #         obj.startMine()
 #
 #         Patterns = obj.getPatterns()
 #
@@ -44,15 +44,15 @@
 
      You should have received a copy of the GNU General Public License
      along with this program.  If not, see <https://www.gnu.org/licenses/>.
      Copyright (C)  2021 Rage Uday Kiran
 
 """
 
-from PAMI.highUtilityPattern.basic import abstract as _ab
+from PAMI.highUtilityPatterns.basic import abstract as _ab
 
 
 class _Transaction:
     """
         A class to store Transaction of a database
 
     Attributes:
@@ -373,15 +373,15 @@
            >>> python3 EFIM sampleTDB.txt output.txt 35  (it will consider "\t" as separator)
            >>> python3 EFIM sampleTDB.txt output.txt 35 , (it will consider "," as separator)
 
     Sample run of importing the code:
     -------------------------------------
     .. code-block:: python
         
-        from PAMI.highUtilityPattern.basic import EFIM as alg
+        from PAMI.highUtilityPatterns.basic import EFIM as alg
 
         obj=alg.EFIM("input.txt",35)
 
         obj.startMine()
 
         Patterns = obj.getPatterns()
```

### Comparing `pami-2023.7.21/PAMI/highUtilityPattern/basic/HMiner.py` & `pami-2023.7.7/PAMI/highUtilityPatterns/basic/HMiner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 # **Importing this algorithm into a python program**
 # --------------------------------------------------------
 #
 #
-#     from PAMI.highUtilityPattern.basic import HMiner as alg
+#     from PAMI.highUtilityPatterns.basic import HMiner as alg
 #
 #     obj = alg.HMiner("input.txt", 35)
 #
 #     obj.startMine()
 #
 #     Patterns = obj.getPatterns()
 #
@@ -42,15 +42,15 @@
 
      You should have received a copy of the GNU General Public License
      along with this program.  If not, see <https://www.gnu.org/licenses/>.
      Copyright (C)  2021 Rage Uday Kiran
 
 """
 
-from PAMI.highUtilityPattern.basic import abstract as _ab
+from PAMI.highUtilityPatterns.basic import abstract as _ab
 
 
 class _Element:
     """
     A class represents an Element of a utility list .
     Attributes :
     ----------
@@ -199,15 +199,15 @@
 
             >>> python3 HMiner.py sampleTDB.txt output.txt 35 (separator will be "\t")
 
     Sample run of importing the code:
     --------------------------------------
     .. code-block:: python
 
-        from PAMI.highUtilityPattern.basic import HMiner as alg
+        from PAMI.highUtilityPatterns.basic import HMiner as alg
         
         obj = alg.HMiner("input.txt",35)
         
         obj.startMine()
         
         Patterns = obj.getPatterns()
```

### Comparing `pami-2023.7.21/PAMI/highUtilityPattern/basic/UPGrowth.py` & `pami-2023.7.7/PAMI/highUtilityPatterns/basic/UPGrowth.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 
 # **Importing this algorithm into a python program**
 # --------------------------------------------------------
 #
 #
-#     from PAMI.highUtilityPattern.basic import UPGrowth as alg
+#     from PAMI.highUtilityPatterns.basic import UPGrowth as alg
 #
 #     obj=alg.UPGrowth("input.txt",35)
 #
 #     obj.startMine()
 #
-#     highUtilityPattern = obj.getPatterns()
+#     highUtilityPatterns = obj.getPatterns()
 #
-#     print("Total number of Spatial Frequent Patterns:", len(highUtilityPattern))
+#     print("Total number of Spatial Frequent Patterns:", len(highUtilityPatterns))
 #
 #     obj.save("output")
 #
 #     memUSS = obj.getMemoryUSS()
 #
 #     print("Total Memory in USS:", memUSS)
 #
@@ -42,15 +42,15 @@
 
      You should have received a copy of the GNU General Public License
      along with this program.  If not, see <https://www.gnu.org/licenses/>.
      Copyright (C)  2021 Rage Uday Kiran
 
 """
 
-from PAMI.highUtilityPattern.basic import abstract as _ab
+from PAMI.highUtilityPatterns.basic import abstract as _ab
 
 
 class _UPItem:
     """
     A class to represent the UPItem
 
     Attribute :
@@ -379,23 +379,23 @@
         ------------
           >>> python3 UPGrowth sampleTDB.txt output.txt sampleN.txt 35  (it will consider "\t" as separator)
 
     Sample run of importing the code:
     -------------------------------------
     .. code-block:: python
     
-        from PAMI.highUtilityPattern.basic import UPGrowth as alg
+        from PAMI.highUtilityPatterns.basic import UPGrowth as alg
 
         obj=alg.UPGrowth("input.txt",35)
 
         obj.startMine()
 
-        highUtilityPattern = obj.getPatterns()
+        highUtilityPatterns = obj.getPatterns()
 
-        print("Total number of Spatial Frequent Patterns:", len(highUtilityPattern))
+        print("Total number of Spatial Frequent Patterns:", len(highUtilityPatterns))
 
         obj.save("output")
 
         memUSS = obj.getMemoryUSS()
 
         print("Total Memory in USS:", memUSS)
```

### Comparing `pami-2023.7.21/PAMI/highUtilityPattern/basic/abstract.py` & `pami-2023.7.7/PAMI/highUtilityPatterns/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/highUtilityPattern/basic/efimParallel.py` & `pami-2023.7.7/PAMI/highUtilityPatterns/basic/efimParallel.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
      You should have received a copy of the GNU General Public License
      along with this program.  If not, see <https://www.gnu.org/licenses/>.
      Copyright (C)  2021 Rage Uday Kiran
 
 """
 
-from PAMI.highUtilityPattern.basic import abstract as _ab
+from PAMI.highUtilityPatterns.basic import abstract as _ab
 
 class efimParallel(_ab._utilityPatterns):
     """
     Description:
     -----------
     EFIM is one of the fastest algorithm to mine High Utility ItemSets from transactional databases.
```

### Comparing `pami-2023.7.21/PAMI/highUtilityPattern/parallel/abstract.py` & `pami-2023.7.7/PAMI/highUtilityPatterns/parallel/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/highUtilityPattern/parallel/efimparallel.py` & `pami-2023.7.7/PAMI/highUtilityPatterns/parallel/efimparallel.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
      You should have received a copy of the GNU General Public License
      along with this program.  If not, see <https://www.gnu.org/licenses/>.
      Copyright (C)  2021 Rage Uday Kiran
 
 """
 
-from PAMI.highUtilityPattern.parallel import abstract as _ab
+from PAMI.highUtilityPatterns.parallel import abstract as _ab
 
 class efimParallel(_ab._utilityPatterns):
     """
     Description:
     -----------
     EFIM is one of the fastest algorithm to mine High Utility ItemSets from transactional databases.
```

### Comparing `pami-2023.7.21/PAMI/highUtilityPatternsInStreams/HUPMS.py` & `pami-2023.7.7/PAMI/streams/highUtility/HUPMS.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/highUtilityPatternsInStreams/SHUGrowth.py` & `pami-2023.7.7/PAMI/streams/highUtility/SHUGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/highUtilityPatternsInStreams/abstract.py` & `pami-2023.7.7/PAMI/streams/highUtility/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/highUtilitySpatialPattern/__init__.py` & `pami-2023.7.7/PAMI/highUtilitySpatialPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/highUtilitySpatialPattern/abstract.py` & `pami-2023.7.7/PAMI/highUtilitySpatialPattern/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/highUtilitySpatialPattern/basic/HDSHUIM.py` & `pami-2023.7.7/PAMI/highUtilitySpatialPattern/basic/HDSHUIM.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/highUtilitySpatialPattern/basic/SHUIM.py` & `pami-2023.7.7/PAMI/highUtilitySpatialPattern/basic/SHUIM.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/highUtilitySpatialPattern/basic/abstract.py` & `pami-2023.7.7/PAMI/highUtilitySpatialPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/highUtilitySpatialPattern/topk/TKSHUIM.py` & `pami-2023.7.7/PAMI/highUtilitySpatialPattern/topk/TKSHUIM.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/highUtilitySpatialPattern/topk/abstract.py` & `pami-2023.7.7/PAMI/highUtilitySpatialPattern/topk/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/localPeriodicPattern/basic/LPPGrowth.py` & `pami-2023.7.7/PAMI/localPeriodicPattern/basic/LPPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/localPeriodicPattern/basic/LPPMBreadth.py` & `pami-2023.7.7/PAMI/localPeriodicPattern/basic/LPPMBreadth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/localPeriodicPattern/basic/LPPMDepth.py` & `pami-2023.7.7/PAMI/localPeriodicPattern/basic/LPPMDepth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/localPeriodicPattern/basic/abstract.py` & `pami-2023.7.7/PAMI/localPeriodicPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/CFPGrowth.py` & `pami-2023.7.7/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/CFPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/CFPGrowthPlus.py` & `pami-2023.7.7/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/CFPGrowthPlus.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/abstract.py` & `pami-2023.7.7/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/partialPeriodicFrequentPattern/basic/GPFgrowth.py` & `pami-2023.7.7/PAMI/partialPeriodicFrequentPattern/basic/GPFgrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/partialPeriodicFrequentPattern/basic/PPF_DFS.py` & `pami-2023.7.7/PAMI/partialPeriodicFrequentPattern/basic/PPF_DFS.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/partialPeriodicFrequentPattern/basic/abstract.py` & `pami-2023.7.7/PAMI/partialPeriodicFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/partialPeriodicPattern/__init__.py` & `pami-2023.7.7/PAMI/partialPeriodicPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/partialPeriodicPattern/basic/GThreePGrowth.py` & `pami-2023.7.7/PAMI/partialPeriodicPattern/basic/GThreePGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/partialPeriodicPattern/basic/Gabstract.py` & `pami-2023.7.7/PAMI/partialPeriodicPattern/basic/Gabstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/partialPeriodicPattern/basic/PPPGrowth.py` & `pami-2023.7.7/PAMI/partialPeriodicPattern/basic/PPPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/partialPeriodicPattern/basic/PPP_ECLAT.py` & `pami-2023.7.7/PAMI/partialPeriodicPattern/basic/PPP_ECLAT.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/partialPeriodicPattern/basic/__init__.py` & `pami-2023.7.7/PAMI/partialPeriodicPattern/basic/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/partialPeriodicPattern/basic/abstract.py` & `pami-2023.7.7/PAMI/partialPeriodicPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/partialPeriodicPattern/closed/PPPClose.py` & `pami-2023.7.7/PAMI/partialPeriodicPattern/closed/PPPClose.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/partialPeriodicPattern/closed/abstract.py` & `pami-2023.7.7/PAMI/partialPeriodicPattern/closed/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/partialPeriodicPattern/maximal/Max3PGrowth.py` & `pami-2023.7.7/PAMI/partialPeriodicPattern/maximal/Max3PGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/partialPeriodicPattern/maximal/__init__.py` & `pami-2023.7.7/PAMI/partialPeriodicPattern/maximal/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/partialPeriodicPattern/maximal/abstract.py` & `pami-2023.7.7/PAMI/partialPeriodicPattern/maximal/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/partialPeriodicPattern/timeSeries/PPGrowth.py` & `pami-2023.7.7/PAMI/partialPeriodicPattern/timeSeries/PPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/partialPeriodicPattern/timeSeries/abstract.py` & `pami-2023.7.7/PAMI/partialPeriodicPattern/timeSeries/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/partialPeriodicPattern/topk/abstract.py` & `pami-2023.7.7/PAMI/partialPeriodicPattern/topk/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/partialPeriodicPattern/topk/k3PMiner.py` & `pami-2023.7.7/PAMI/partialPeriodicPattern/topk/k3PMiner.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/partialPeriodicSpatialPattern/basic/STEclat.py` & `pami-2023.7.7/PAMI/partialPeriodicSpatialPattern/basic/STEclat.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/partialPeriodicSpatialPattern/basic/abstract.py` & `pami-2023.7.7/PAMI/partialPeriodicSpatialPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/periodicCorrelatedPattern/basic/EPCPGrowth.py` & `pami-2023.7.7/PAMI/periodicCorrelatedPattern/basic/EPCPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/periodicCorrelatedPattern/basic/abstract.py` & `pami-2023.7.7/PAMI/periodicCorrelatedPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/periodicFrequentPattern/__init__.py` & `pami-2023.7.7/PAMI/periodicFrequentPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/periodicFrequentPattern/basic/PFECLAT.py` & `pami-2023.7.7/PAMI/periodicFrequentPattern/basic/PFECLAT.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/periodicFrequentPattern/basic/PFPGrowth.py` & `pami-2023.7.7/PAMI/periodicFrequentPattern/basic/PFPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/periodicFrequentPattern/basic/PFPGrowthPlus.py` & `pami-2023.7.7/PAMI/periodicFrequentPattern/basic/PFPGrowthPlus.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/periodicFrequentPattern/basic/PFPMC.py` & `pami-2023.7.7/PAMI/periodicFrequentPattern/basic/PFPMC.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/periodicFrequentPattern/basic/PSGrowth.py` & `pami-2023.7.7/PAMI/periodicFrequentPattern/basic/PSGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/periodicFrequentPattern/basic/__init__.py` & `pami-2023.7.7/PAMI/periodicFrequentPattern/basic/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/periodicFrequentPattern/basic/abstract.py` & `pami-2023.7.7/PAMI/periodicFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/periodicFrequentPattern/closed/CPFPMiner.py` & `pami-2023.7.7/PAMI/periodicFrequentPattern/closed/CPFPMiner.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/periodicFrequentPattern/closed/__init__.py` & `pami-2023.7.7/PAMI/periodicFrequentPattern/closed/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/periodicFrequentPattern/closed/abstract.py` & `pami-2023.7.7/PAMI/periodicFrequentPattern/closed/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/periodicFrequentPattern/cuda/abstract.py` & `pami-2023.7.7/PAMI/periodicFrequentPattern/cuda/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/periodicFrequentPattern/cuda/cuGPFMiner.py` & `pami-2023.7.7/PAMI/periodicFrequentPattern/cuda/cuGPFMiner.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,15 +118,20 @@
             Complete set of periodic-frequent patterns will be loaded in to a dataframe
         getMemoryUSS()
             Total amount of USS memory consumed by the mining process will be retrieved from this function
         getMemoryRSS()
             Total amount of RSS memory consumed by the mining process will be retrieved from this function
         getRuntime()
             Total amount of runtime taken by the mining process will be retrieved from this function
-
+        creatingOneItemSets()
+            Scan the database and store the items with their timestamps which are periodic frequent 
+        getPeriodAndSupport()
+            Calculates the support and period for a list of timestamps.
+        Generation()
+            Used to implement prefix class equivalence method to generate the periodic patterns recursively
             
 
     **Methods to execute code on terminal**
 
             Format:
                         >>>  python3 PFECLAT.py <inputFile> <outputFile> <minSup>
             Example:
@@ -258,14 +263,16 @@
                     return;
                 }
             }
         }
 
     }
     
+    
+    
     ''', 'supportAndPeriod')
 
     def _convert(self, value):
         """
         To convert the given user specified value
 
         :param value: user specified value
```

### Comparing `pami-2023.7.21/PAMI/periodicFrequentPattern/cuda/gPFMinerBit.py` & `pami-2023.7.7/PAMI/periodicFrequentPattern/cuda/gPFMinerBit.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/periodicFrequentPattern/maximal/MaxPFGrowth.py` & `pami-2023.7.7/PAMI/periodicFrequentPattern/maximal/MaxPFGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/periodicFrequentPattern/maximal/__init__.py` & `pami-2023.7.7/PAMI/periodicFrequentPattern/maximal/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/periodicFrequentPattern/maximal/abstract.py` & `pami-2023.7.7/PAMI/periodicFrequentPattern/maximal/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/periodicFrequentPattern/topk/TopkPFP/TopkPFP.py` & `pami-2023.7.7/PAMI/periodicFrequentPattern/topk/TopkPFP/TopkPFP.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/periodicFrequentPattern/topk/TopkPFP/abstract.py` & `pami-2023.7.7/PAMI/periodicFrequentPattern/topk/TopkPFP/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/periodicFrequentPattern/topk/kPFPMiner/abstract.py` & `pami-2023.7.7/PAMI/periodicFrequentPattern/topk/kPFPMiner/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/periodicFrequentPattern/topk/kPFPMiner/kPFPMiner.py` & `pami-2023.7.7/PAMI/periodicFrequentPattern/topk/kPFPMiner/kPFPMiner.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/recurringPattern/basic/RPGrowth.py` & `pami-2023.7.7/PAMI/recurringPattern/basic/RPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/recurringPattern/basic/abstract.py` & `pami-2023.7.7/PAMI/recurringPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/relativeFrequentPattern/basic/RSFPGrowth.py` & `pami-2023.7.7/PAMI/relativeFrequentPatterns/basic/RSFPGrowth.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 
      You should have received a copy of the GNU General Public License
      along with this program.  If not, see <https://www.gnu.org/licenses/>.
      Copyright (C)  2021 Rage Uday Kiran
 
 """
 
-from PAMI.relativeFrequentPattern.basic import abstract as _ab
+from PAMI.relativeFrequentPatterns.basic import abstract as _ab
 
 
 class _Node:
     """
         A class used to represent the node of frequentPatterntree
 
     Attributes:
```

### Comparing `pami-2023.7.21/PAMI/relativeFrequentPattern/basic/abstract.py` & `pami-2023.7.7/PAMI/relativeFrequentPatterns/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/relativeHighUtilityPattern/basic/RHUIM.py` & `pami-2023.7.7/PAMI/relativeHighUtilityPatterns/basic/RHUIM.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 # **Importing this algorithm into a python program**
 # --------------------------------------------------------
 #
 #
-#     from PAMI.relativeHighUtilityPattern.basic import RHUIM as alg
+#     from PAMI.relativeHighUtilityPatterns.basic import RHUIM as alg
 #
 #     obj = alg.RHUIM("input.txt", 35, 20)
 #
 #     obj.startMine()
 #
 #     frequentPatterns = obj.getPatterns()
 #
@@ -46,15 +46,15 @@
      You should have received a copy of the GNU General Public License
      along with this program.  If not, see <https://www.gnu.org/licenses/>.
      Copyright (C)  2021 Rage Uday Kiran
 
 """
 
 
-from PAMI.relativeHighUtilityPattern.basic import abstract as _ab
+from PAMI.relativeHighUtilityPatterns.basic import abstract as _ab
 
 
 class _Transaction:
     """
         A class to store Transaction of a database
 
     Attributes:
@@ -379,15 +379,15 @@
                       >>>  python3 RHUIM.py sampleTDB.txt output.txt 35 20
 
 
     **Importing this algorithm into a python program**
 
     .. code-block:: python
 
-            from PAMI.relativeHighUtilityPattern.basic import RHUIM as alg
+            from PAMI.relativeHighUtilityPatterns.basic import RHUIM as alg
 
             obj=alg.RHUIM("input.txt", 35, 20)
 
             obj.startMine()
 
             frequentPatterns = obj.getPatterns()
```

### Comparing `pami-2023.7.21/PAMI/relativeHighUtilityPattern/basic/abstract.py` & `pami-2023.7.7/PAMI/relativeHighUtilityPatterns/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/sequentialPatternMining/basic/SPADE.py` & `pami-2023.7.7/PAMI/sequentialPatternMining/basic/SPADE.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/sequentialPatternMining/basic/abstract.py` & `pami-2023.7.7/PAMI/sequentialPatternMining/closed/abstract.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,37 +22,35 @@
 #      but WITHOUT ANY WARRANTY; without even the implied warranty of
 #      MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #      GNU General Public License for more details.
 #
 #      You should have received a copy of the GNU General Public License
 #      along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
-# from abc import ABC as _ABC, abstractmethod as _abstractmethod
 from abc import ABC as _ABC, abstractmethod as _abstractmethod
 import time as _time
 import csv as _csv
 import pandas as _pd
-from collections import defaultdict as _defaultdict
+from collections import defaultdict as _dd
 from itertools import combinations as _c
 import os as _os
 import os.path as _ospath
 import psutil as _psutil
+import resource as _resource
+import math as _math
 import sys as _sys
-import validators as _validators
-from urllib.request import urlopen as _urlopen
-import functools as _functools
 
 
-class _sequentialPatterns(_ABC):
-    """
-    This abstract base class defines the variables and methods that every frequent pattern mining algorithm in sequential databases must
+class _frequentPatterns(_ABC):
+    """ This abstract base class defines the variables and methods that every frequent pattern mining algorithm must
         employ in PAMI
 
-    Attributes:
-    ----------
+
+       Attributes:
+       ----------
         iFile : str
             Input file name or path of the input file
         minSup: integer or float or str
             The user can specify minSup either in count or proportion of database size.
             If the program detects the data type of minSup is integer, then it treats minSup is expressed in count.
             Otherwise, it will be treated as float.
             Example: minSup=10 will be treated as integer, while minSup=10.0 will be treated as float
@@ -68,54 +66,55 @@
         oFile : str
             Name of the output file to store complete set of frequent patterns
         memoryUSS : float
             To store the total amount of USS memory consumed by the program
         memoryRSS : float
             To store the total amount of RSS memory consumed by the program
 
-    Methods:
-    -------
+       Methods:
+       -------
         startMine()
             Calling this function will start the actual mining process
         getPatterns()
             This function will output all interesting patterns discovered by an algorithm
         save(oFile)
             This function will store the discovered patterns in an output file specified by the user
         getPatternsAsDataFrame()
             The function outputs the patterns generated by an algorithm as a data frame
         getMemoryUSS()
             This function outputs the total amount of USS memory consumed by a mining algorithm
         getMemoryRSS()
             This function outputs the total amount of RSS memory consumed by a mining algorithm
         getRuntime()
             This function outputs the total runtime of a mining algorithm
+
     """
 
     def __init__(self, iFile, minSup, sep="\t"):
         """
         :param iFile: Input file name or path of the input file
-        :type iFile: str or DataFrame
+        :type iFile: str
         :param minSup: The user can specify minSup either in count or proportion of database size.
             If the program detects the data type of minSup is integer, then it treats minSup is expressed in count.
             Otherwise, it will be treated as float.
             Example: minSup=10 will be treated as integer, while minSup=10.0 will be treated as float
         :type minSup: int or float or str
         :param sep: separator used to distinguish items from each other. The default separator is tab space. However, users can override the default separator
         :type sep: str
         """
 
         self._iFile = iFile
         self._sep = sep
         self._minSup = minSup
-        self._finalPatterns = {}
         self._oFile = str()
-        self._memoryUSS = float()
-        self._memoryRSS = float()
+        self._finalPatterns = {}
         self._startTime = float()
         self._endTime = float()
+        self._memoryUSS = float()
+        self._memoryRSS = float()
 
     @_abstractmethod
     def startMine(self):
         """Code for the mining process will start from this function"""
 
         pass
 
@@ -124,14 +123,15 @@
         """Complete set of frequent patterns generated will be retrieved from this function"""
 
         pass
 
     @_abstractmethod
     def save(self, oFile):
         """Complete set of frequent patterns will be saved in to an output file from this function
+
         :param oFile: Name of the output file
         :type oFile: file
         """
 
         pass
 
     @_abstractmethod
@@ -153,13 +153,7 @@
         pass
 
     @_abstractmethod
     def getRuntime(self):
         """Total amount of runtime taken by the program will be retrieved from this function"""
 
         pass
-
-    @_abstractmethod
-    def printResults(self):
-        """ To print result of the execution"""
-
-        pass
```

### Comparing `pami-2023.7.21/PAMI/sequentialPatternMining/basic/prefixSpan.py` & `pami-2023.7.7/PAMI/sequentialPatternMining/basic/prefixSpan.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/sequentialPatternMining/closed/abstract.py` & `pami-2023.7.7/PAMI/correlatedPattern/basic/abstract.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,56 +8,46 @@
 #      This program is distributed in the hope that it will be useful,
 #      but WITHOUT ANY WARRANTY; without even the implied warranty of
 #      MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #      GNU General Public License for more details.
 #
 #      You should have received a copy of the GNU General Public License
 #      along with this program.  If not, see <https://www.gnu.org/licenses/>.
-#
-#      This program is free software: you can redistribute it and/or modify
-#      it under the terms of the GNU General Public License as published by
-#      the Free Software Foundation, either version 3 of the License, or
-#      (at your option) any later version.
-#
-#      This program is distributed in the hope that it will be useful,
-#      but WITHOUT ANY WARRANTY; without even the implied warranty of
-#      MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#      GNU General Public License for more details.
-#
-#      You should have received a copy of the GNU General Public License
-#      along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 from abc import ABC as _ABC, abstractmethod as _abstractmethod
 import time as _time
 import csv as _csv
 import pandas as _pd
-from collections import defaultdict as _dd
+from collections import defaultdict as _defaultdict
 from itertools import combinations as _c
 import os as _os
 import os.path as _ospath
 import psutil as _psutil
-import resource as _resource
-import math as _math
+import validators as _validators
+from urllib.request import urlopen as _urlopen
 import sys as _sys
+import math as _math
 
 
-class _frequentPatterns(_ABC):
+class _correlatedPatterns(_ABC):
     """ This abstract base class defines the variables and methods that every frequent pattern mining algorithm must
         employ in PAMI
 
 
-       Attributes:
-       ----------
+    Attributes :
+    ----------
         iFile : str
             Input file name or path of the input file
         minSup: integer or float or str
             The user can specify minSup either in count or proportion of database size.
             If the program detects the data type of minSup is integer, then it treats minSup is expressed in count.
             Otherwise, it will be treated as float.
             Example: minSup=10 will be treated as integer, while minSup=10.0 will be treated as float
+        minAllConf: float
+            The user given minimum all confidence Ratio(should be in range of 0 to 1)
         sep : str
             This variable is used to distinguish items from one another in a transaction. The default seperator is tab space or \t.
             However, the users can override their default separator
         startTime:float
             To record the start time of the algorithm
         endTime:float
             To record the completion time of the algorithm
@@ -66,16 +56,16 @@
         oFile : str
             Name of the output file to store complete set of frequent patterns
         memoryUSS : float
             To store the total amount of USS memory consumed by the program
         memoryRSS : float
             To store the total amount of RSS memory consumed by the program
 
-       Methods:
-       -------
+    Methods :
+    -------
         startMine()
             Calling this function will start the actual mining process
         getPatterns()
             This function will output all interesting patterns discovered by an algorithm
         save(oFile)
             This function will store the discovered patterns in an output file specified by the user
         getPatternsAsDataFrame()
@@ -85,36 +75,40 @@
         getMemoryRSS()
             This function outputs the total amount of RSS memory consumed by a mining algorithm
         getRuntime()
             This function outputs the total runtime of a mining algorithm
 
     """
 
-    def __init__(self, iFile, minSup, sep="\t"):
+    def __init__(self, iFile, minSup, minAllConf, sep="\t"):
         """
         :param iFile: Input file name or path of the input file
         :type iFile: str
         :param minSup: The user can specify minSup either in count or proportion of database size.
             If the program detects the data type of minSup is integer, then it treats minSup is expressed in count.
             Otherwise, it will be treated as float.
             Example: minSup=10 will be treated as integer, while minSup=10.0 will be treated as float
         :type minSup: int or float or str
+        :param minAllConf: The user given minimum all confidence Ratio(should be in range of 0 to 1)
+        :type minAllConf :float
         :param sep: separator used to distinguish items from each other. The default separator is tab space. However, users can override the default separator
         :type sep: str
         """
 
         self._iFile = iFile
         self._sep = sep
         self._minSup = minSup
-        self._oFile = str()
+        self._minAllConf = minAllConf
         self._finalPatterns = {}
+        self._oFile = str()
+        self._memoryRSS = float()
+        self._memoryUSS = float()
         self._startTime = float()
         self._endTime = float()
-        self._memoryUSS = float()
-        self._memoryRSS = float()
+
 
     @_abstractmethod
     def startMine(self):
         """Code for the mining process will start from this function"""
 
         pass
 
@@ -148,12 +142,19 @@
 
     @_abstractmethod
     def getMemoryRSS(self):
         """Total amount of RSS memory consumed by the program will be retrieved from this function"""
 
         pass
 
+
     @_abstractmethod
     def getRuntime(self):
         """Total amount of runtime taken by the program will be retrieved from this function"""
 
         pass
+
+    @_abstractmethod
+    def printResults(self):
+        """ To print the results of execution."""
+
+        pass
```

### Comparing `pami-2023.7.21/PAMI/stablePeriodicFrequentPattern/basic/SPPEclat.py` & `pami-2023.7.7/PAMI/stablePeriodicFrequentPattern/basic/SPPEclat.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/stablePeriodicFrequentPattern/basic/SPPGrowth.py` & `pami-2023.7.7/PAMI/stablePeriodicFrequentPattern/basic/SPPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/stablePeriodicFrequentPattern/basic/SPPGrowthDump.py` & `pami-2023.7.7/PAMI/stablePeriodicFrequentPattern/basic/SPPGrowthDump.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/stablePeriodicFrequentPattern/basic/abstract.py` & `pami-2023.7.7/PAMI/stablePeriodicFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/stablePeriodicFrequentPattern/topK/TSPIN.py` & `pami-2023.7.7/PAMI/stablePeriodicFrequentPattern/topK/TSPIN.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/stablePeriodicFrequentPattern/topK/abstract.py` & `pami-2023.7.7/PAMI/stablePeriodicFrequentPattern/topK/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/uncertainFrequentPattern/__init__.py` & `pami-2023.7.7/PAMI/uncertainFrequentPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/uncertainFrequentPattern/basic/CUFPTree.py` & `pami-2023.7.7/PAMI/uncertainFrequentPattern/basic/CUFPTree.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/uncertainFrequentPattern/basic/PUFGrowth.py` & `pami-2023.7.7/PAMI/uncertainFrequentPattern/basic/PUFGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/uncertainFrequentPattern/basic/TUFP.py` & `pami-2023.7.7/PAMI/uncertainFrequentPattern/basic/TUFP.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/uncertainFrequentPattern/basic/TubeP.py` & `pami-2023.7.7/PAMI/uncertainFrequentPattern/basic/TubeP.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/uncertainFrequentPattern/basic/TubeS.py` & `pami-2023.7.7/PAMI/uncertainFrequentPattern/basic/TubeS.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/uncertainFrequentPattern/basic/UFGrowth.py` & `pami-2023.7.7/PAMI/uncertainFrequentPattern/basic/UFGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/uncertainFrequentPattern/basic/UVECLAT.py` & `pami-2023.7.7/PAMI/uncertainFrequentPattern/basic/UVECLAT.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/uncertainFrequentPattern/basic/abstract.py` & `pami-2023.7.7/PAMI/uncertainFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/uncertainPeriodicFrequentPattern/__init__.py` & `pami-2023.7.7/PAMI/uncertainPeriodicFrequentPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/uncertainPeriodicFrequentPattern/basic/UPFPGrowth.py` & `pami-2023.7.7/PAMI/uncertainPeriodicFrequentPattern/basic/UPFPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/uncertainPeriodicFrequentPattern/basic/UPFPGrowthPlus.py` & `pami-2023.7.7/PAMI/uncertainPeriodicFrequentPattern/basic/UPFPGrowthPlus.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/uncertainPeriodicFrequentPattern/basic/abstract.py` & `pami-2023.7.7/PAMI/uncertainPeriodicFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/weightedFrequentNeighbourhoodPattern/basic/SWFPGrowth.py` & `pami-2023.7.7/PAMI/weightedFrequentNeighbourhoodPattern/basic/SWFPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/weightedFrequentNeighbourhoodPattern/basic/abstract.py` & `pami-2023.7.7/PAMI/weightedFrequentNeighbourhoodPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/weightedFrequentPattern/basic/WFIM.py` & `pami-2023.7.7/PAMI/weightedFrequentPattern/basic/WFIM.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/weightedFrequentPattern/basic/abstract.py` & `pami-2023.7.7/PAMI/weightedFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/weightedFrequentRegularPattern/basic/WFRIMiner.py` & `pami-2023.7.7/PAMI/weightedFrequentRegularPattern/basic/WFRIMiner.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/weightedFrequentRegularPattern/basic/abstract.py` & `pami-2023.7.7/PAMI/weightedFrequentRegularPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/weightedUncertainFrequentPattern/basic/WUFIM.py` & `pami-2023.7.7/PAMI/weightedUncertainFrequentPattern/basic/WUFIM.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PAMI/weightedUncertainFrequentPattern/basic/abstract.py` & `pami-2023.7.7/PAMI/weightedUncertainFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.21/PKG-INFO` & `pami-2023.7.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 Metadata-Version: 2.1
 Name: pami
-Version: 2023.7.21
+Version: 2023.7.7
 Summary: This software is being developed at the University of Aizu, Aizu-Wakamatsu, Fukushima, Japan
-Home-page: https://github.com/udayLab/PAMI
+Home-page: https://github.com/udayRage/PAMI
 Author: Rage Uday Kiran
 Author-email: uday.rage@gmail.com
 License: GPLv3
 Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 Provides-Extra: gpu
 Provides-Extra: spark
 License-File: LICENSE
 
 ![PyPI](https://img.shields.io/pypi/v/PAMI)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/PAMI)
 [![GitHub license](https://img.shields.io/github/license/UdayLab/PAMI)](https://github.com/UdayLab/PAMI/blob/main/LICENSE)
 ![PyPI - Implementation](https://img.shields.io/pypi/implementation/PAMI)
-[![Documentation Status](https://readthedocs.org/projects/pami-1/badge/?version=latest)](https://pami-1.readthedocs.io/en/latest/?badge=latest)
 ![PyPI - Wheel](https://img.shields.io/pypi/wheel/PAMI)
 ![PyPI - Status](https://img.shields.io/pypi/status/PAMI)
 [![GitHub issues](https://img.shields.io/github/issues/UdayLab/PAMI)](https://github.com/UdayLab/PAMI/issues)
 [![GitHub forks](https://img.shields.io/github/forks/UdayLab/PAMI)](https://github.com/UdayLab/PAMI/network)
 [![GitHub stars](https://img.shields.io/github/stars/UdayLab/PAMI)](https://github.com/UdayLab/PAMI/stargazers)
 [![Downloads](https://static.pepy.tech/badge/pami)](https://pepy.tech/project/pami)
 [![Downloads](https://static.pepy.tech/badge/pami/month)](https://pepy.tech/project/pami)
@@ -38,21 +37,21 @@
 PAttern MIning (PAMI) is a Python library containing several algorithms to discover user interest-based patterns in transactional/temporal/geo-referential/sequence databases across multiple computing platforms.
 
 
 1. User manual https://udaylab.github.io/PAMI/manuals/index.html
 
 2. Coders manual https://udaylab.github.io/PAMI/codersManual/index.html
 
-3. Code documentation https://pami-1.readthedocs.io 
+3. Code documentation [PAMI documentation](https://raw.githack.com/UdayLab/PAMI/main/htmlDocs/_build/html/index.html)
 
-4. Datasets   https://u-aizu.ac.jp/~udayrage/datasets.html
+3. Datasets   https://u-aizu.ac.jp/~udayrage/datasets.html
 
-5. Discussions on PAMI usage https://github.com/UdayLab/PAMI/discussions
+4. Discussions on PAMI usage https://github.com/UdayLab/PAMI/discussions
 
-6. Report issues https://github.com/UdayLab/PAMI/issues
+5. Report issues https://github.com/UdayLab/PAMI/issues
   
  # Recent versions  
 
 - Version 2023.07.07: New algorithms: cuApriroi, cuAprioriBit, cuEclat, cuEclatBit, gPPMiner, cuGPFMiner, FPStream, HUPMS, SHUPGrowth New codes to generate synthetic databases
 - Version 2023.06.20: Fuzzy Partial Periodic, Periodic Patterns in High Utility, Code Documentation, help() function Update 
 - Version 2023.03.01: prefixSpan and SPADE   
 
@@ -78,106 +77,106 @@
 ### Transactional databases
 1. Frequent pattern mining: [Sample](https://udayrage.github.io/PAMI/frequentPatternMining.html)
 
 | Basic                                                                                                                                                                                                                            | Closed                                                                                                                                                                                                           | Maximal                                                                                                                   | Top-k                                                                                                                                                                                                  | CUDA           | pyspark                                                                                                                                                                                                                                               |
 |----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | Apriori [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/basic/Apriori/APRIORI-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/basic/Apriori/Apriori-ad.md)              | Closed [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/closed/CHARM/CHARM-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/closed/CHARM/CHARM-ad.md) | maxFP-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/maximal/MaxFPGrowth/MaxFPGrowth-st.md) | topK [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/topk/FAE-st.pdf)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/topk/FAE-ad.pdf) | cudaAprioriGCT | parallelApriori [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/parallelApriori/parallelApriori-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/parallelApriori/ParallelApriori-ad%20(1).md) |
 | FP-growth  [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/basic/FPGrowth/fpGrowth_basic.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/basic/FPGrowth/fpGrowth_adv.md)         |                                                                                                                                                                                                                  |                                                                                                                           |                                                                                                                                                                                                        | cudaAprioriTID | parallelFPGrowth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/parallelFPGrowth/parallelFPGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/parallelFPGrowth/ParallelFPGrowth-ad%20.md) |
-| ECLAT  [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLAT/ECLAT-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLAT/Eclat-ad.md)  |                                                                                                                                                                                                                  |                                                                                                                           |                                                                                                                                                                                                        | cudaEclatGCT   | parallelECLAT [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/parallelECLAT/parallelECLAT-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/ParallelECLAT-ad.pdf)             |
+| ECLAT  [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLAT/ECLAT-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLAT/Eclat-ad.md)                   |                                                                                                                                                                                                                  |                                                                                                                           |                                                                                                                                                                                                        | cudaEclatGCT   | parallelECLAT [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/parallelECLAT/parallelECLAT-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/ParallelECLAT-ad.pdf)             |
 | ECLAT-bitSet [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLATbitset/ECLATbitset-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLATbitset/Eclatbitset-ad.md) |                                                                                                                                                                                                                  |                                                                                                                           |                                                                                                                                                                                                        |                |                                                                                                                                                                                                                                                       |
 | ECLAT-diffset [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLATDiffset/ECLATDiffset-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLATDiffset/EclatDiffset-ad.md)                                                                                                                                                                                                                    |                                                                                                                                                                                                                  |                                                                                                                           |                                                                                                                                                                                                        |                |
 
 2. Relative frequent pattern mining: [Sample](https://udayrage.github.io/PAMI/relativeFrequentPatternMining.html)
 
-| Basic                                                                                                                                                                                                                                          |
-|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| RSFP  [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/relativeFrequentPatterns/RSFPGrowth/RSFPGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/relativeFrequentPatterns/RSFPGrowth/RSFPGrowt-ad.md) |
+| Basic |
+|-------|
+| RSFP  [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/relativeFrequentPatterns/RSFPGrowth/RSFPGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/relativeFrequentPatterns/RSFPGrowth/RSFPGrowt-ad.md)|
 
 
 3. Frequent pattern with multiple minimum support: [Sample](https://udayrage.github.io/PAMI/multipleMinSupFrequentPatternMining.html)
 
 | Basic       |
 |-------------|
 | CFPGrowth   |
 | CFPGrowth++ |
 
 
 
 4. Correlated pattern mining: [Sample](https://udayrage.github.io/PAMI/correlatePatternMining.html)
 
-| Basic                                                                                                                                                                                                                                           |
-|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| CP-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/correlatedPattern/CPGrowth/CPGrowth-st.md) -[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/correlatedPattern/CPGrowth/CPGrowth-ad.md)                  |
-| CP-growth++ [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/correlatedPattern/CPGrowthPlus/CPGrowthPuls-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/correlatedPattern/CPGrowthPlus/CPGrowthPlus-ad.md) |
+| Basic                                                                                                                                                                                                            |
+|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| CP-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/correlatedPattern/CPGrowth/CPGrowth-st.md) -[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/correlatedPattern/CPGrowth/CPGrowth-ad.md) |
+| CP-growth++ [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/correlatedPattern/CPGrowthPlus/CPGrowthPuls-st.md)                                                                                              -[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/correlatedPattern/CPGrowthPlus/CPGrowthPlus-ad.md)|
 
 
 ### Temporal databases
 
 
 1. Periodic-frequent pattern mining: [Sample](https://udayrage.github.io/PAMI/periodicFrequentPatternMining.html)
 
-| Basic                                                                                                                                                                                                                                                                             | Closed                                                                                                                                                                                                                                                   | Maximal                                                                                                                                                                                                                                            | Top-K                                                                                                                                                                                                                                                        |
-|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| PFP-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFPGrowth/PFPGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFPGrowth/PFPGrowth-ad.md)                      | CPFP [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/closed/CPFPMiner/CPFPMiner-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/closed/CPFPMiner/CPFPMiner-ad.md) | maxPF-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/maximal/MaxPFGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/maximal/MaxPFGrowth-ad.md) | kPFPMiner [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/topk/kPFPMiner/kPFPMiner-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/topk/kPFPMiner/kPFPMiner-ad%20.md) |
-| PFP-growth++ [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFPGrowthPlus/PFPGrowthPlus-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFPGrowthPlus/PFPGrowthPlus-ad%20.md) |                                                                                                                                                                                                                                                          |                                                                                                                                                                                                                                                    |
-| PS-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PSGrowth/PSGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PSGrowth/PSGrowth-ad.md)                           |                                                                                                                                                                                                                                                          |                                                                                                                                                                                                                                                    |
-| PFP-ECLAT [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFECLAT/PFECLAT-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFECLAT/PFECLAT-ad%20.md)                            |                                                                                                                                                                                                                                                          |                                                                                                                                                                                                                                                    |
+| Basic                                                                                                                                                                                                                                                | Closed                                                                                                                                                                                                                                 | Maximal                                                                                                                           | Top-K |
+|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------| -----------------------------------------------------------------------------------------------------------------------------------|
+| PFP-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFPGrowth/PFPGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFPGrowth/PFPGrowth-ad.md)       | CPFP [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/closed/CPFPMiner/CPFPMiner-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/closed/CPFPMiner/CPFPMiner-ad.md) | maxPF-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/maximal/MaxPFGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/maximal/MaxPFGrowth-ad.md) |  kPFPMiner [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/topk/kPFPMiner/kPFPMiner-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/topk/kPFPMiner/kPFPMiner-ad%20.md) |
+| PFP-growth++ [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFPGrowthPlus/PFPGrowthPlus-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFPGrowthPlus/PFPGrowthPlus-ad%20.md) |                                                                                                                                                                                                                                        |                                                                                                                                   |
+| PS-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PSGrowth/PSGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PSGrowth/PSGrowth-ad.md)              |                                                                                                                                                                                                                                        |                                                                                                                                   |
+| PFP-ECLAT [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFECLAT/PFECLAT-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFECLAT/PFECLAT-ad%20.md)                |                                                                                                                                                                                                                                        |                                                                                                                                   |
 
 
 2. Local periodic pattern mining: [Sample](https://udayrage.github.io/PAMI/localPeriodicPatternMining.html)
 
-| Basic                                                                                                                                  |
-|----------------------------------------------------------------------------------------------------------------------------------------|
-| LPPGrowth   [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/localPeriodicPatterns/basic/LPPGrowth/LPPGrowth-st.md)     |
-| LPPMBreadth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/localPeriodicPatterns/basic/LPPMBreadth/LPPMBreadth-st.md) |
-| LPPMDepth   [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/localPeriodicPatterns/basic/LPPMDepth/LPPMDepth-st.md)     |
+| Basic       |
+|-------------|
+| LPPGrowth   [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/localPeriodicPatterns/basic/LPPGrowth/LPPGrowth-st.md)|
+| LPPMBreadth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/localPeriodicPatterns/basic/LPPMBreadth/LPPMBreadth-st.md)|
+| LPPMDepth   [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/localPeriodicPatterns/basic/LPPMDepth/LPPMDepth-st.md)|
 
 3. Partial periodic-frequent pattern mining: [Sample](https://udayrage.github.io/PAMI/partialPeriodicFrequentPattern.html)
 
-| Basic                                                                                                                                                                                                                                              |
-|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| Basic                                                                                                                                                                                                                                      |
+|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | GPF-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicFrequentPatterns/GPFGrowth/GPFgrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicFrequentPattern/PPF_DFS-ad.pdf) |
-| PPF-DFS [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicFrequentPatterns/PPF_DFS/PPF_DFS-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicFrequentPattern/PPF_DFS-ad.pdf)        |
+| PPF-DFS [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicFrequentPatterns/PPF_DFS/PPF_DFS-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicFrequentPattern/PPF_DFS-ad.pdf)    |
 
 4. Partial periodic pattern mining: [Sample](https://udayrage.github.io/PAMI/partialPeriodicPatternMining.html)
 
-| Basic                                                                                                                                                                                                                                                              | Closed                                                                                                                                                                                                                               | Maximal                                                                                                                         |
-|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------|
-| 3P-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/PPPGrowth/PPPGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/PPPGrowth/PPPGrowth-ad.md)          | 3P-close [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPattern/closed/PPPClose-st.pdf)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPattern/closed/PPPClose-ad.pdf) | max3P-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPattern/maximal/Max3PGrowth-st.pdf) |                                                                                                                                                                                                                                         |                                                                                                                                  |               | |
-| 3P-ECLAT [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/PPPECLAT/PPP_ECLAT-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/PPPECLAT/PPP_ECLAT-ad.md)             |                                                                                                                                                                                                                                      |                                                                                                                                 |
-| G3P-Growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/G3PGrowth/GThreePGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/G3PGrowth/GThreePGrowth-ad.md) |                                                                                                                                                                                                                                      |                                                                                                                                 |
+| Basic                                                                                                                                                                                                                                         | Closed                                                                                                                                                                                                                                 | Maximal                                                                                                                          |
+|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------|
+| 3P-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/PPPGrowth/PPPGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/PPPGrowth/PPPGrowth-ad.md) | 3P-close [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPattern/closed/PPPClose-st.pdf)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPattern/closed/PPPClose-ad.pdf) | max3P-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPattern/maximal/Max3PGrowth-st.pdf) |                                                                                                                                                                                                                                         |                                                                                                                                  |               | |
+| 3P-ECLAT [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/PPPECLAT/PPP_ECLAT-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/PPPECLAT/PPP_ECLAT-ad.md)|  |  |
+| G3P-Growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/G3PGrowth/GThreePGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/G3PGrowth/GThreePGrowth-ad.md) | | |
 
 
 5. Periodic correlated pattern mining: [Sample](https://udayrage.github.io/PAMI/periodicCorrelatedPatternMining.html)
 
-| Basic                                                                                                                                                                                                                                                                     |
-|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| Basic                                                                                                                                                                                                                                 |
+|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | EPCP-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/correlated/EPCPGrowth/EPCPGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/correlated/EPCPGrowth/EPCPGrowth-ad.md) |
 
 6. Stable periodic pattern mining: [Sample](https://udayrage.github.io/PAMI/stablePeriodicPatterns.html)
 
-| Basic                                                                                                                                                                                                                                                           | TopK  |
-|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-------|
-| SPP-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/stablePeriodicFrequentPatterns/SPPGrowth/SPPGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/stablePeriodicFrequentPatterns/SPPGrowth/SPPGrowth-ad%20.md) | TSPIN |
-| SPP-ECLAT  [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/stablePeriodicFrequentPatterns/SPPEclat/SPPECLAT-st-2.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/stablePeriodicFrequentPatterns/SPPEclat/SPPECLAT-ad%20.md)   |       |
+| Basic      | TopK |
+|------------|------|
+| SPP-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/stablePeriodicFrequentPatterns/SPPGrowth/SPPGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/stablePeriodicFrequentPatterns/SPPGrowth/SPPGrowth-ad%20.md)| TSPIN  |
+| SPP-ECLAT  [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/stablePeriodicFrequentPatterns/SPPEclat/SPPECLAT-st-2.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/stablePeriodicFrequentPatterns/SPPEclat/SPPECLAT-ad%20.md) |  |
 
 ### Geo-referenced (or spatiotemporal) databases
 
 1. Frequent spatial pattern mining: [Sample](https://udayrage.github.io/PAMI/frequentSpatialPatternMining.html)
 
-| Basic                                                                                                                                                                                                                               |
-|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| Basic                                                                                                                                                                                                                                 |
+|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | spatialECLAT  [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentSpatialPattern/SpatialECLAT-st.pdf)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentSpatialPattern/SpatialECLAT-ad.pdf) |
 | FSP-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentSpatialPattern/FSPGrowth-st.pdf)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentSpatialPattern/FSPGrowth-ad.pdf)          |
 
 2. Geo referenced Periodic frequent pattern mining: [Sample](https://udayrage.github.io/PAMI/periodicFrequentSpatial.html)
 
-| Basic                                                                                                                                                                                                                                                           |
-|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| GPFPMiner [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/spatial/GPFPMiner/GPFPMiner-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/spatial/GPFPMiner/GPFPMiner-ad.md) |
+| Basic     |
+|-----------|
+| GPFPMiner [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/spatial/GPFPMiner/GPFPMiner-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/spatial/GPFPMiner/GPFPMiner-ad.md)  |
 
 3. Partial periodic spatial pattern mining:[Sample](https://udayrage.github.io/PAMI/partialPeriodicSpatialPatternMining.html)
 
 | Basic   |
 |---------|
 | STECLAT [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/spatial/STECLAT/STECLAT-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/spatial/STECLAT/STECLAT-ad.md)|
 
@@ -313,38 +312,20 @@
     
 | Basic       |
 |-------------|
 | SPADE [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/sequencePatternMining/basic/SPADE/Spade-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/sequencePatternMining/basic/SPADE/Spade-ad.md)|
 | prefixSpan [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/sequencePatternMining/basic/prefixSpan/PrifixSpan-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/sequencePatternMining/basic/prefixSpan/PrifixSpan-ad.md)|
 
 
-2. Geo-referenced Frequent Sequence Pattern mining
-
-| Basic |
-|-------|
-|GFSP-Miner|
-
+2, Geo-referenced Frequent Sequence Pattern
 ### Timeseries databases
 
 
 ## 2. Mining Streams
-
-1. Frequent pattern mining
-
-|Basic|
-|-----|
- |to be written|
-
-2. High utility pattern mining
-
-| Basic |
-|-------|
- | HUPMS |
-
-
+   __coming soon__    
 
 ## 3. Mining Graphs
 __coming soon__
```

### Comparing `pami-2023.7.21/README.md` & `pami-2023.7.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 ![PyPI](https://img.shields.io/pypi/v/PAMI)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/PAMI)
 [![GitHub license](https://img.shields.io/github/license/UdayLab/PAMI)](https://github.com/UdayLab/PAMI/blob/main/LICENSE)
 ![PyPI - Implementation](https://img.shields.io/pypi/implementation/PAMI)
-[![Documentation Status](https://readthedocs.org/projects/pami-1/badge/?version=latest)](https://pami-1.readthedocs.io/en/latest/?badge=latest)
 ![PyPI - Wheel](https://img.shields.io/pypi/wheel/PAMI)
 ![PyPI - Status](https://img.shields.io/pypi/status/PAMI)
 [![GitHub issues](https://img.shields.io/github/issues/UdayLab/PAMI)](https://github.com/UdayLab/PAMI/issues)
 [![GitHub forks](https://img.shields.io/github/forks/UdayLab/PAMI)](https://github.com/UdayLab/PAMI/network)
 [![GitHub stars](https://img.shields.io/github/stars/UdayLab/PAMI)](https://github.com/UdayLab/PAMI/stargazers)
 [![Downloads](https://static.pepy.tech/badge/pami)](https://pepy.tech/project/pami)
 [![Downloads](https://static.pepy.tech/badge/pami/month)](https://pepy.tech/project/pami)
@@ -19,21 +18,21 @@
 PAttern MIning (PAMI) is a Python library containing several algorithms to discover user interest-based patterns in transactional/temporal/geo-referential/sequence databases across multiple computing platforms.
 
 
 1. User manual https://udaylab.github.io/PAMI/manuals/index.html
 
 2. Coders manual https://udaylab.github.io/PAMI/codersManual/index.html
 
-3. Code documentation https://pami-1.readthedocs.io 
+3. Code documentation [PAMI documentation](https://raw.githack.com/UdayLab/PAMI/main/htmlDocs/_build/html/index.html)
 
-4. Datasets   https://u-aizu.ac.jp/~udayrage/datasets.html
+3. Datasets   https://u-aizu.ac.jp/~udayrage/datasets.html
 
-5. Discussions on PAMI usage https://github.com/UdayLab/PAMI/discussions
+4. Discussions on PAMI usage https://github.com/UdayLab/PAMI/discussions
 
-6. Report issues https://github.com/UdayLab/PAMI/issues
+5. Report issues https://github.com/UdayLab/PAMI/issues
   
  # Recent versions  
 
 - Version 2023.07.07: New algorithms: cuApriroi, cuAprioriBit, cuEclat, cuEclatBit, gPPMiner, cuGPFMiner, FPStream, HUPMS, SHUPGrowth New codes to generate synthetic databases
 - Version 2023.06.20: Fuzzy Partial Periodic, Periodic Patterns in High Utility, Code Documentation, help() function Update 
 - Version 2023.03.01: prefixSpan and SPADE   
 
@@ -59,106 +58,106 @@
 ### Transactional databases
 1. Frequent pattern mining: [Sample](https://udayrage.github.io/PAMI/frequentPatternMining.html)
 
 | Basic                                                                                                                                                                                                                            | Closed                                                                                                                                                                                                           | Maximal                                                                                                                   | Top-k                                                                                                                                                                                                  | CUDA           | pyspark                                                                                                                                                                                                                                               |
 |----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | Apriori [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/basic/Apriori/APRIORI-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/basic/Apriori/Apriori-ad.md)              | Closed [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/closed/CHARM/CHARM-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/closed/CHARM/CHARM-ad.md) | maxFP-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/maximal/MaxFPGrowth/MaxFPGrowth-st.md) | topK [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/topk/FAE-st.pdf)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/topk/FAE-ad.pdf) | cudaAprioriGCT | parallelApriori [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/parallelApriori/parallelApriori-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/parallelApriori/ParallelApriori-ad%20(1).md) |
 | FP-growth  [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/basic/FPGrowth/fpGrowth_basic.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/basic/FPGrowth/fpGrowth_adv.md)         |                                                                                                                                                                                                                  |                                                                                                                           |                                                                                                                                                                                                        | cudaAprioriTID | parallelFPGrowth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/parallelFPGrowth/parallelFPGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/parallelFPGrowth/ParallelFPGrowth-ad%20.md) |
-| ECLAT  [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLAT/ECLAT-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLAT/Eclat-ad.md)  |                                                                                                                                                                                                                  |                                                                                                                           |                                                                                                                                                                                                        | cudaEclatGCT   | parallelECLAT [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/parallelECLAT/parallelECLAT-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/ParallelECLAT-ad.pdf)             |
+| ECLAT  [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLAT/ECLAT-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLAT/Eclat-ad.md)                   |                                                                                                                                                                                                                  |                                                                                                                           |                                                                                                                                                                                                        | cudaEclatGCT   | parallelECLAT [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/parallelECLAT/parallelECLAT-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/ParallelECLAT-ad.pdf)             |
 | ECLAT-bitSet [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLATbitset/ECLATbitset-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLATbitset/Eclatbitset-ad.md) |                                                                                                                                                                                                                  |                                                                                                                           |                                                                                                                                                                                                        |                |                                                                                                                                                                                                                                                       |
 | ECLAT-diffset [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLATDiffset/ECLATDiffset-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLATDiffset/EclatDiffset-ad.md)                                                                                                                                                                                                                    |                                                                                                                                                                                                                  |                                                                                                                           |                                                                                                                                                                                                        |                |
 
 2. Relative frequent pattern mining: [Sample](https://udayrage.github.io/PAMI/relativeFrequentPatternMining.html)
 
-| Basic                                                                                                                                                                                                                                          |
-|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| RSFP  [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/relativeFrequentPatterns/RSFPGrowth/RSFPGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/relativeFrequentPatterns/RSFPGrowth/RSFPGrowt-ad.md) |
+| Basic |
+|-------|
+| RSFP  [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/relativeFrequentPatterns/RSFPGrowth/RSFPGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/relativeFrequentPatterns/RSFPGrowth/RSFPGrowt-ad.md)|
 
 
 3. Frequent pattern with multiple minimum support: [Sample](https://udayrage.github.io/PAMI/multipleMinSupFrequentPatternMining.html)
 
 | Basic       |
 |-------------|
 | CFPGrowth   |
 | CFPGrowth++ |
 
 
 
 4. Correlated pattern mining: [Sample](https://udayrage.github.io/PAMI/correlatePatternMining.html)
 
-| Basic                                                                                                                                                                                                                                           |
-|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| CP-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/correlatedPattern/CPGrowth/CPGrowth-st.md) -[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/correlatedPattern/CPGrowth/CPGrowth-ad.md)                  |
-| CP-growth++ [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/correlatedPattern/CPGrowthPlus/CPGrowthPuls-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/correlatedPattern/CPGrowthPlus/CPGrowthPlus-ad.md) |
+| Basic                                                                                                                                                                                                            |
+|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| CP-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/correlatedPattern/CPGrowth/CPGrowth-st.md) -[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/correlatedPattern/CPGrowth/CPGrowth-ad.md) |
+| CP-growth++ [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/correlatedPattern/CPGrowthPlus/CPGrowthPuls-st.md)                                                                                              -[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/correlatedPattern/CPGrowthPlus/CPGrowthPlus-ad.md)|
 
 
 ### Temporal databases
 
 
 1. Periodic-frequent pattern mining: [Sample](https://udayrage.github.io/PAMI/periodicFrequentPatternMining.html)
 
-| Basic                                                                                                                                                                                                                                                                             | Closed                                                                                                                                                                                                                                                   | Maximal                                                                                                                                                                                                                                            | Top-K                                                                                                                                                                                                                                                        |
-|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| PFP-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFPGrowth/PFPGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFPGrowth/PFPGrowth-ad.md)                      | CPFP [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/closed/CPFPMiner/CPFPMiner-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/closed/CPFPMiner/CPFPMiner-ad.md) | maxPF-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/maximal/MaxPFGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/maximal/MaxPFGrowth-ad.md) | kPFPMiner [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/topk/kPFPMiner/kPFPMiner-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/topk/kPFPMiner/kPFPMiner-ad%20.md) |
-| PFP-growth++ [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFPGrowthPlus/PFPGrowthPlus-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFPGrowthPlus/PFPGrowthPlus-ad%20.md) |                                                                                                                                                                                                                                                          |                                                                                                                                                                                                                                                    |
-| PS-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PSGrowth/PSGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PSGrowth/PSGrowth-ad.md)                           |                                                                                                                                                                                                                                                          |                                                                                                                                                                                                                                                    |
-| PFP-ECLAT [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFECLAT/PFECLAT-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFECLAT/PFECLAT-ad%20.md)                            |                                                                                                                                                                                                                                                          |                                                                                                                                                                                                                                                    |
+| Basic                                                                                                                                                                                                                                                | Closed                                                                                                                                                                                                                                 | Maximal                                                                                                                           | Top-K |
+|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------| -----------------------------------------------------------------------------------------------------------------------------------|
+| PFP-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFPGrowth/PFPGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFPGrowth/PFPGrowth-ad.md)       | CPFP [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/closed/CPFPMiner/CPFPMiner-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/closed/CPFPMiner/CPFPMiner-ad.md) | maxPF-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/maximal/MaxPFGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/maximal/MaxPFGrowth-ad.md) |  kPFPMiner [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/topk/kPFPMiner/kPFPMiner-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/topk/kPFPMiner/kPFPMiner-ad%20.md) |
+| PFP-growth++ [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFPGrowthPlus/PFPGrowthPlus-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFPGrowthPlus/PFPGrowthPlus-ad%20.md) |                                                                                                                                                                                                                                        |                                                                                                                                   |
+| PS-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PSGrowth/PSGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PSGrowth/PSGrowth-ad.md)              |                                                                                                                                                                                                                                        |                                                                                                                                   |
+| PFP-ECLAT [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFECLAT/PFECLAT-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFECLAT/PFECLAT-ad%20.md)                |                                                                                                                                                                                                                                        |                                                                                                                                   |
 
 
 2. Local periodic pattern mining: [Sample](https://udayrage.github.io/PAMI/localPeriodicPatternMining.html)
 
-| Basic                                                                                                                                  |
-|----------------------------------------------------------------------------------------------------------------------------------------|
-| LPPGrowth   [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/localPeriodicPatterns/basic/LPPGrowth/LPPGrowth-st.md)     |
-| LPPMBreadth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/localPeriodicPatterns/basic/LPPMBreadth/LPPMBreadth-st.md) |
-| LPPMDepth   [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/localPeriodicPatterns/basic/LPPMDepth/LPPMDepth-st.md)     |
+| Basic       |
+|-------------|
+| LPPGrowth   [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/localPeriodicPatterns/basic/LPPGrowth/LPPGrowth-st.md)|
+| LPPMBreadth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/localPeriodicPatterns/basic/LPPMBreadth/LPPMBreadth-st.md)|
+| LPPMDepth   [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/localPeriodicPatterns/basic/LPPMDepth/LPPMDepth-st.md)|
 
 3. Partial periodic-frequent pattern mining: [Sample](https://udayrage.github.io/PAMI/partialPeriodicFrequentPattern.html)
 
-| Basic                                                                                                                                                                                                                                              |
-|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| Basic                                                                                                                                                                                                                                      |
+|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | GPF-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicFrequentPatterns/GPFGrowth/GPFgrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicFrequentPattern/PPF_DFS-ad.pdf) |
-| PPF-DFS [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicFrequentPatterns/PPF_DFS/PPF_DFS-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicFrequentPattern/PPF_DFS-ad.pdf)        |
+| PPF-DFS [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicFrequentPatterns/PPF_DFS/PPF_DFS-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicFrequentPattern/PPF_DFS-ad.pdf)    |
 
 4. Partial periodic pattern mining: [Sample](https://udayrage.github.io/PAMI/partialPeriodicPatternMining.html)
 
-| Basic                                                                                                                                                                                                                                                              | Closed                                                                                                                                                                                                                               | Maximal                                                                                                                         |
-|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------|
-| 3P-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/PPPGrowth/PPPGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/PPPGrowth/PPPGrowth-ad.md)          | 3P-close [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPattern/closed/PPPClose-st.pdf)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPattern/closed/PPPClose-ad.pdf) | max3P-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPattern/maximal/Max3PGrowth-st.pdf) |                                                                                                                                                                                                                                         |                                                                                                                                  |               | |
-| 3P-ECLAT [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/PPPECLAT/PPP_ECLAT-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/PPPECLAT/PPP_ECLAT-ad.md)             |                                                                                                                                                                                                                                      |                                                                                                                                 |
-| G3P-Growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/G3PGrowth/GThreePGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/G3PGrowth/GThreePGrowth-ad.md) |                                                                                                                                                                                                                                      |                                                                                                                                 |
+| Basic                                                                                                                                                                                                                                         | Closed                                                                                                                                                                                                                                 | Maximal                                                                                                                          |
+|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------|
+| 3P-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/PPPGrowth/PPPGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/PPPGrowth/PPPGrowth-ad.md) | 3P-close [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPattern/closed/PPPClose-st.pdf)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPattern/closed/PPPClose-ad.pdf) | max3P-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPattern/maximal/Max3PGrowth-st.pdf) |                                                                                                                                                                                                                                         |                                                                                                                                  |               | |
+| 3P-ECLAT [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/PPPECLAT/PPP_ECLAT-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/PPPECLAT/PPP_ECLAT-ad.md)|  |  |
+| G3P-Growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/G3PGrowth/GThreePGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/G3PGrowth/GThreePGrowth-ad.md) | | |
 
 
 5. Periodic correlated pattern mining: [Sample](https://udayrage.github.io/PAMI/periodicCorrelatedPatternMining.html)
 
-| Basic                                                                                                                                                                                                                                                                     |
-|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| Basic                                                                                                                                                                                                                                 |
+|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | EPCP-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/correlated/EPCPGrowth/EPCPGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/correlated/EPCPGrowth/EPCPGrowth-ad.md) |
 
 6. Stable periodic pattern mining: [Sample](https://udayrage.github.io/PAMI/stablePeriodicPatterns.html)
 
-| Basic                                                                                                                                                                                                                                                           | TopK  |
-|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-------|
-| SPP-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/stablePeriodicFrequentPatterns/SPPGrowth/SPPGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/stablePeriodicFrequentPatterns/SPPGrowth/SPPGrowth-ad%20.md) | TSPIN |
-| SPP-ECLAT  [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/stablePeriodicFrequentPatterns/SPPEclat/SPPECLAT-st-2.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/stablePeriodicFrequentPatterns/SPPEclat/SPPECLAT-ad%20.md)   |       |
+| Basic      | TopK |
+|------------|------|
+| SPP-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/stablePeriodicFrequentPatterns/SPPGrowth/SPPGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/stablePeriodicFrequentPatterns/SPPGrowth/SPPGrowth-ad%20.md)| TSPIN  |
+| SPP-ECLAT  [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/stablePeriodicFrequentPatterns/SPPEclat/SPPECLAT-st-2.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/stablePeriodicFrequentPatterns/SPPEclat/SPPECLAT-ad%20.md) |  |
 
 ### Geo-referenced (or spatiotemporal) databases
 
 1. Frequent spatial pattern mining: [Sample](https://udayrage.github.io/PAMI/frequentSpatialPatternMining.html)
 
-| Basic                                                                                                                                                                                                                               |
-|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| Basic                                                                                                                                                                                                                                 |
+|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | spatialECLAT  [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentSpatialPattern/SpatialECLAT-st.pdf)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentSpatialPattern/SpatialECLAT-ad.pdf) |
 | FSP-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentSpatialPattern/FSPGrowth-st.pdf)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentSpatialPattern/FSPGrowth-ad.pdf)          |
 
 2. Geo referenced Periodic frequent pattern mining: [Sample](https://udayrage.github.io/PAMI/periodicFrequentSpatial.html)
 
-| Basic                                                                                                                                                                                                                                                           |
-|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| GPFPMiner [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/spatial/GPFPMiner/GPFPMiner-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/spatial/GPFPMiner/GPFPMiner-ad.md) |
+| Basic     |
+|-----------|
+| GPFPMiner [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/spatial/GPFPMiner/GPFPMiner-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/spatial/GPFPMiner/GPFPMiner-ad.md)  |
 
 3. Partial periodic spatial pattern mining:[Sample](https://udayrage.github.io/PAMI/partialPeriodicSpatialPatternMining.html)
 
 | Basic   |
 |---------|
 | STECLAT [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/spatial/STECLAT/STECLAT-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/spatial/STECLAT/STECLAT-ad.md)|
 
@@ -294,36 +293,18 @@
     
 | Basic       |
 |-------------|
 | SPADE [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/sequencePatternMining/basic/SPADE/Spade-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/sequencePatternMining/basic/SPADE/Spade-ad.md)|
 | prefixSpan [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/sequencePatternMining/basic/prefixSpan/PrifixSpan-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/sequencePatternMining/basic/prefixSpan/PrifixSpan-ad.md)|
 
 
-2. Geo-referenced Frequent Sequence Pattern mining
-
-| Basic |
-|-------|
-|GFSP-Miner|
-
+2, Geo-referenced Frequent Sequence Pattern
 ### Timeseries databases
 
 
 ## 2. Mining Streams
-
-1. Frequent pattern mining
-
-|Basic|
-|-----|
- |to be written|
-
-2. High utility pattern mining
-
-| Basic |
-|-------|
- | HUPMS |
-
-
+   __coming soon__    
 
 ## 3. Mining Graphs
 __coming soon__
```

### Comparing `pami-2023.7.21/pami.egg-info/PKG-INFO` & `pami-2023.7.7/pami.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 Metadata-Version: 2.1
 Name: pami
-Version: 2023.7.21
+Version: 2023.7.7
 Summary: This software is being developed at the University of Aizu, Aizu-Wakamatsu, Fukushima, Japan
-Home-page: https://github.com/udayLab/PAMI
+Home-page: https://github.com/udayRage/PAMI
 Author: Rage Uday Kiran
 Author-email: uday.rage@gmail.com
 License: GPLv3
 Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 Provides-Extra: gpu
 Provides-Extra: spark
 License-File: LICENSE
 
 ![PyPI](https://img.shields.io/pypi/v/PAMI)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/PAMI)
 [![GitHub license](https://img.shields.io/github/license/UdayLab/PAMI)](https://github.com/UdayLab/PAMI/blob/main/LICENSE)
 ![PyPI - Implementation](https://img.shields.io/pypi/implementation/PAMI)
-[![Documentation Status](https://readthedocs.org/projects/pami-1/badge/?version=latest)](https://pami-1.readthedocs.io/en/latest/?badge=latest)
 ![PyPI - Wheel](https://img.shields.io/pypi/wheel/PAMI)
 ![PyPI - Status](https://img.shields.io/pypi/status/PAMI)
 [![GitHub issues](https://img.shields.io/github/issues/UdayLab/PAMI)](https://github.com/UdayLab/PAMI/issues)
 [![GitHub forks](https://img.shields.io/github/forks/UdayLab/PAMI)](https://github.com/UdayLab/PAMI/network)
 [![GitHub stars](https://img.shields.io/github/stars/UdayLab/PAMI)](https://github.com/UdayLab/PAMI/stargazers)
 [![Downloads](https://static.pepy.tech/badge/pami)](https://pepy.tech/project/pami)
 [![Downloads](https://static.pepy.tech/badge/pami/month)](https://pepy.tech/project/pami)
@@ -38,21 +37,21 @@
 PAttern MIning (PAMI) is a Python library containing several algorithms to discover user interest-based patterns in transactional/temporal/geo-referential/sequence databases across multiple computing platforms.
 
 
 1. User manual https://udaylab.github.io/PAMI/manuals/index.html
 
 2. Coders manual https://udaylab.github.io/PAMI/codersManual/index.html
 
-3. Code documentation https://pami-1.readthedocs.io 
+3. Code documentation [PAMI documentation](https://raw.githack.com/UdayLab/PAMI/main/htmlDocs/_build/html/index.html)
 
-4. Datasets   https://u-aizu.ac.jp/~udayrage/datasets.html
+3. Datasets   https://u-aizu.ac.jp/~udayrage/datasets.html
 
-5. Discussions on PAMI usage https://github.com/UdayLab/PAMI/discussions
+4. Discussions on PAMI usage https://github.com/UdayLab/PAMI/discussions
 
-6. Report issues https://github.com/UdayLab/PAMI/issues
+5. Report issues https://github.com/UdayLab/PAMI/issues
   
  # Recent versions  
 
 - Version 2023.07.07: New algorithms: cuApriroi, cuAprioriBit, cuEclat, cuEclatBit, gPPMiner, cuGPFMiner, FPStream, HUPMS, SHUPGrowth New codes to generate synthetic databases
 - Version 2023.06.20: Fuzzy Partial Periodic, Periodic Patterns in High Utility, Code Documentation, help() function Update 
 - Version 2023.03.01: prefixSpan and SPADE   
 
@@ -78,106 +77,106 @@
 ### Transactional databases
 1. Frequent pattern mining: [Sample](https://udayrage.github.io/PAMI/frequentPatternMining.html)
 
 | Basic                                                                                                                                                                                                                            | Closed                                                                                                                                                                                                           | Maximal                                                                                                                   | Top-k                                                                                                                                                                                                  | CUDA           | pyspark                                                                                                                                                                                                                                               |
 |----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | Apriori [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/basic/Apriori/APRIORI-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/basic/Apriori/Apriori-ad.md)              | Closed [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/closed/CHARM/CHARM-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/closed/CHARM/CHARM-ad.md) | maxFP-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/maximal/MaxFPGrowth/MaxFPGrowth-st.md) | topK [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/topk/FAE-st.pdf)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/topk/FAE-ad.pdf) | cudaAprioriGCT | parallelApriori [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/parallelApriori/parallelApriori-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/parallelApriori/ParallelApriori-ad%20(1).md) |
 | FP-growth  [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/basic/FPGrowth/fpGrowth_basic.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/basic/FPGrowth/fpGrowth_adv.md)         |                                                                                                                                                                                                                  |                                                                                                                           |                                                                                                                                                                                                        | cudaAprioriTID | parallelFPGrowth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/parallelFPGrowth/parallelFPGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/parallelFPGrowth/ParallelFPGrowth-ad%20.md) |
-| ECLAT  [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLAT/ECLAT-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLAT/Eclat-ad.md)  |                                                                                                                                                                                                                  |                                                                                                                           |                                                                                                                                                                                                        | cudaEclatGCT   | parallelECLAT [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/parallelECLAT/parallelECLAT-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/ParallelECLAT-ad.pdf)             |
+| ECLAT  [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLAT/ECLAT-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLAT/Eclat-ad.md)                   |                                                                                                                                                                                                                  |                                                                                                                           |                                                                                                                                                                                                        | cudaEclatGCT   | parallelECLAT [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/parallelECLAT/parallelECLAT-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/ParallelECLAT-ad.pdf)             |
 | ECLAT-bitSet [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLATbitset/ECLATbitset-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLATbitset/Eclatbitset-ad.md) |                                                                                                                                                                                                                  |                                                                                                                           |                                                                                                                                                                                                        |                |                                                                                                                                                                                                                                                       |
 | ECLAT-diffset [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLATDiffset/ECLATDiffset-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLATDiffset/EclatDiffset-ad.md)                                                                                                                                                                                                                    |                                                                                                                                                                                                                  |                                                                                                                           |                                                                                                                                                                                                        |                |
 
 2. Relative frequent pattern mining: [Sample](https://udayrage.github.io/PAMI/relativeFrequentPatternMining.html)
 
-| Basic                                                                                                                                                                                                                                          |
-|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| RSFP  [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/relativeFrequentPatterns/RSFPGrowth/RSFPGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/relativeFrequentPatterns/RSFPGrowth/RSFPGrowt-ad.md) |
+| Basic |
+|-------|
+| RSFP  [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/relativeFrequentPatterns/RSFPGrowth/RSFPGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/relativeFrequentPatterns/RSFPGrowth/RSFPGrowt-ad.md)|
 
 
 3. Frequent pattern with multiple minimum support: [Sample](https://udayrage.github.io/PAMI/multipleMinSupFrequentPatternMining.html)
 
 | Basic       |
 |-------------|
 | CFPGrowth   |
 | CFPGrowth++ |
 
 
 
 4. Correlated pattern mining: [Sample](https://udayrage.github.io/PAMI/correlatePatternMining.html)
 
-| Basic                                                                                                                                                                                                                                           |
-|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| CP-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/correlatedPattern/CPGrowth/CPGrowth-st.md) -[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/correlatedPattern/CPGrowth/CPGrowth-ad.md)                  |
-| CP-growth++ [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/correlatedPattern/CPGrowthPlus/CPGrowthPuls-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/correlatedPattern/CPGrowthPlus/CPGrowthPlus-ad.md) |
+| Basic                                                                                                                                                                                                            |
+|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| CP-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/correlatedPattern/CPGrowth/CPGrowth-st.md) -[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/correlatedPattern/CPGrowth/CPGrowth-ad.md) |
+| CP-growth++ [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/correlatedPattern/CPGrowthPlus/CPGrowthPuls-st.md)                                                                                              -[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/correlatedPattern/CPGrowthPlus/CPGrowthPlus-ad.md)|
 
 
 ### Temporal databases
 
 
 1. Periodic-frequent pattern mining: [Sample](https://udayrage.github.io/PAMI/periodicFrequentPatternMining.html)
 
-| Basic                                                                                                                                                                                                                                                                             | Closed                                                                                                                                                                                                                                                   | Maximal                                                                                                                                                                                                                                            | Top-K                                                                                                                                                                                                                                                        |
-|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| PFP-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFPGrowth/PFPGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFPGrowth/PFPGrowth-ad.md)                      | CPFP [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/closed/CPFPMiner/CPFPMiner-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/closed/CPFPMiner/CPFPMiner-ad.md) | maxPF-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/maximal/MaxPFGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/maximal/MaxPFGrowth-ad.md) | kPFPMiner [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/topk/kPFPMiner/kPFPMiner-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/topk/kPFPMiner/kPFPMiner-ad%20.md) |
-| PFP-growth++ [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFPGrowthPlus/PFPGrowthPlus-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFPGrowthPlus/PFPGrowthPlus-ad%20.md) |                                                                                                                                                                                                                                                          |                                                                                                                                                                                                                                                    |
-| PS-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PSGrowth/PSGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PSGrowth/PSGrowth-ad.md)                           |                                                                                                                                                                                                                                                          |                                                                                                                                                                                                                                                    |
-| PFP-ECLAT [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFECLAT/PFECLAT-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFECLAT/PFECLAT-ad%20.md)                            |                                                                                                                                                                                                                                                          |                                                                                                                                                                                                                                                    |
+| Basic                                                                                                                                                                                                                                                | Closed                                                                                                                                                                                                                                 | Maximal                                                                                                                           | Top-K |
+|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------| -----------------------------------------------------------------------------------------------------------------------------------|
+| PFP-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFPGrowth/PFPGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFPGrowth/PFPGrowth-ad.md)       | CPFP [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/closed/CPFPMiner/CPFPMiner-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/closed/CPFPMiner/CPFPMiner-ad.md) | maxPF-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/maximal/MaxPFGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/maximal/MaxPFGrowth-ad.md) |  kPFPMiner [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/topk/kPFPMiner/kPFPMiner-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/topk/kPFPMiner/kPFPMiner-ad%20.md) |
+| PFP-growth++ [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFPGrowthPlus/PFPGrowthPlus-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFPGrowthPlus/PFPGrowthPlus-ad%20.md) |                                                                                                                                                                                                                                        |                                                                                                                                   |
+| PS-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PSGrowth/PSGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PSGrowth/PSGrowth-ad.md)              |                                                                                                                                                                                                                                        |                                                                                                                                   |
+| PFP-ECLAT [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFECLAT/PFECLAT-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFECLAT/PFECLAT-ad%20.md)                |                                                                                                                                                                                                                                        |                                                                                                                                   |
 
 
 2. Local periodic pattern mining: [Sample](https://udayrage.github.io/PAMI/localPeriodicPatternMining.html)
 
-| Basic                                                                                                                                  |
-|----------------------------------------------------------------------------------------------------------------------------------------|
-| LPPGrowth   [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/localPeriodicPatterns/basic/LPPGrowth/LPPGrowth-st.md)     |
-| LPPMBreadth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/localPeriodicPatterns/basic/LPPMBreadth/LPPMBreadth-st.md) |
-| LPPMDepth   [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/localPeriodicPatterns/basic/LPPMDepth/LPPMDepth-st.md)     |
+| Basic       |
+|-------------|
+| LPPGrowth   [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/localPeriodicPatterns/basic/LPPGrowth/LPPGrowth-st.md)|
+| LPPMBreadth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/localPeriodicPatterns/basic/LPPMBreadth/LPPMBreadth-st.md)|
+| LPPMDepth   [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/localPeriodicPatterns/basic/LPPMDepth/LPPMDepth-st.md)|
 
 3. Partial periodic-frequent pattern mining: [Sample](https://udayrage.github.io/PAMI/partialPeriodicFrequentPattern.html)
 
-| Basic                                                                                                                                                                                                                                              |
-|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| Basic                                                                                                                                                                                                                                      |
+|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | GPF-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicFrequentPatterns/GPFGrowth/GPFgrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicFrequentPattern/PPF_DFS-ad.pdf) |
-| PPF-DFS [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicFrequentPatterns/PPF_DFS/PPF_DFS-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicFrequentPattern/PPF_DFS-ad.pdf)        |
+| PPF-DFS [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicFrequentPatterns/PPF_DFS/PPF_DFS-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicFrequentPattern/PPF_DFS-ad.pdf)    |
 
 4. Partial periodic pattern mining: [Sample](https://udayrage.github.io/PAMI/partialPeriodicPatternMining.html)
 
-| Basic                                                                                                                                                                                                                                                              | Closed                                                                                                                                                                                                                               | Maximal                                                                                                                         |
-|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------|
-| 3P-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/PPPGrowth/PPPGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/PPPGrowth/PPPGrowth-ad.md)          | 3P-close [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPattern/closed/PPPClose-st.pdf)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPattern/closed/PPPClose-ad.pdf) | max3P-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPattern/maximal/Max3PGrowth-st.pdf) |                                                                                                                                                                                                                                         |                                                                                                                                  |               | |
-| 3P-ECLAT [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/PPPECLAT/PPP_ECLAT-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/PPPECLAT/PPP_ECLAT-ad.md)             |                                                                                                                                                                                                                                      |                                                                                                                                 |
-| G3P-Growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/G3PGrowth/GThreePGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/G3PGrowth/GThreePGrowth-ad.md) |                                                                                                                                                                                                                                      |                                                                                                                                 |
+| Basic                                                                                                                                                                                                                                         | Closed                                                                                                                                                                                                                                 | Maximal                                                                                                                          |
+|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------|
+| 3P-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/PPPGrowth/PPPGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/PPPGrowth/PPPGrowth-ad.md) | 3P-close [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPattern/closed/PPPClose-st.pdf)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPattern/closed/PPPClose-ad.pdf) | max3P-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPattern/maximal/Max3PGrowth-st.pdf) |                                                                                                                                                                                                                                         |                                                                                                                                  |               | |
+| 3P-ECLAT [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/PPPECLAT/PPP_ECLAT-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/PPPECLAT/PPP_ECLAT-ad.md)|  |  |
+| G3P-Growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/G3PGrowth/GThreePGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/G3PGrowth/GThreePGrowth-ad.md) | | |
 
 
 5. Periodic correlated pattern mining: [Sample](https://udayrage.github.io/PAMI/periodicCorrelatedPatternMining.html)
 
-| Basic                                                                                                                                                                                                                                                                     |
-|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| Basic                                                                                                                                                                                                                                 |
+|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | EPCP-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/correlated/EPCPGrowth/EPCPGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/correlated/EPCPGrowth/EPCPGrowth-ad.md) |
 
 6. Stable periodic pattern mining: [Sample](https://udayrage.github.io/PAMI/stablePeriodicPatterns.html)
 
-| Basic                                                                                                                                                                                                                                                           | TopK  |
-|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-------|
-| SPP-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/stablePeriodicFrequentPatterns/SPPGrowth/SPPGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/stablePeriodicFrequentPatterns/SPPGrowth/SPPGrowth-ad%20.md) | TSPIN |
-| SPP-ECLAT  [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/stablePeriodicFrequentPatterns/SPPEclat/SPPECLAT-st-2.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/stablePeriodicFrequentPatterns/SPPEclat/SPPECLAT-ad%20.md)   |       |
+| Basic      | TopK |
+|------------|------|
+| SPP-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/stablePeriodicFrequentPatterns/SPPGrowth/SPPGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/stablePeriodicFrequentPatterns/SPPGrowth/SPPGrowth-ad%20.md)| TSPIN  |
+| SPP-ECLAT  [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/stablePeriodicFrequentPatterns/SPPEclat/SPPECLAT-st-2.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/stablePeriodicFrequentPatterns/SPPEclat/SPPECLAT-ad%20.md) |  |
 
 ### Geo-referenced (or spatiotemporal) databases
 
 1. Frequent spatial pattern mining: [Sample](https://udayrage.github.io/PAMI/frequentSpatialPatternMining.html)
 
-| Basic                                                                                                                                                                                                                               |
-|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| Basic                                                                                                                                                                                                                                 |
+|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | spatialECLAT  [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentSpatialPattern/SpatialECLAT-st.pdf)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentSpatialPattern/SpatialECLAT-ad.pdf) |
 | FSP-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentSpatialPattern/FSPGrowth-st.pdf)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentSpatialPattern/FSPGrowth-ad.pdf)          |
 
 2. Geo referenced Periodic frequent pattern mining: [Sample](https://udayrage.github.io/PAMI/periodicFrequentSpatial.html)
 
-| Basic                                                                                                                                                                                                                                                           |
-|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| GPFPMiner [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/spatial/GPFPMiner/GPFPMiner-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/spatial/GPFPMiner/GPFPMiner-ad.md) |
+| Basic     |
+|-----------|
+| GPFPMiner [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/spatial/GPFPMiner/GPFPMiner-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/spatial/GPFPMiner/GPFPMiner-ad.md)  |
 
 3. Partial periodic spatial pattern mining:[Sample](https://udayrage.github.io/PAMI/partialPeriodicSpatialPatternMining.html)
 
 | Basic   |
 |---------|
 | STECLAT [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/spatial/STECLAT/STECLAT-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/spatial/STECLAT/STECLAT-ad.md)|
 
@@ -313,38 +312,20 @@
     
 | Basic       |
 |-------------|
 | SPADE [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/sequencePatternMining/basic/SPADE/Spade-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/sequencePatternMining/basic/SPADE/Spade-ad.md)|
 | prefixSpan [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/sequencePatternMining/basic/prefixSpan/PrifixSpan-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/sequencePatternMining/basic/prefixSpan/PrifixSpan-ad.md)|
 
 
-2. Geo-referenced Frequent Sequence Pattern mining
-
-| Basic |
-|-------|
-|GFSP-Miner|
-
+2, Geo-referenced Frequent Sequence Pattern
 ### Timeseries databases
 
 
 ## 2. Mining Streams
-
-1. Frequent pattern mining
-
-|Basic|
-|-----|
- |to be written|
-
-2. High utility pattern mining
-
-| Basic |
-|-------|
- | HUPMS |
-
-
+   __coming soon__    
 
 ## 3. Mining Graphs
 __coming soon__
```

### Comparing `pami-2023.7.21/pami.egg-info/SOURCES.txt` & `pami-2023.7.7/pami.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -10,19 +10,19 @@
 PAMI/AssociationRules/basic/__init__.py
 PAMI/AssociationRules/basic/abstract.py
 PAMI/correlatedPattern/__init__.py
 PAMI/correlatedPattern/basic/CPGrowth.py
 PAMI/correlatedPattern/basic/CPGrowthPlus.py
 PAMI/correlatedPattern/basic/__init__.py
 PAMI/correlatedPattern/basic/abstract.py
-PAMI/coveragePattern/__init__.py
-PAMI/coveragePattern/basic/CMine.py
-PAMI/coveragePattern/basic/CPPG.py
-PAMI/coveragePattern/basic/__init__.py
-PAMI/coveragePattern/basic/abstract.py
+PAMI/coveragePatterns/__init__.py
+PAMI/coveragePatterns/basic/CMine.py
+PAMI/coveragePatterns/basic/CPPG.py
+PAMI/coveragePatterns/basic/__init__.py
+PAMI/coveragePatterns/basic/abstract.py
 PAMI/extras/__init__.py
 PAMI/extras/generateLatexGraphFile.py
 PAMI/extras/plotPointOnMap.py
 PAMI/extras/plotPointOnMap_dump.py
 PAMI/extras/scatterPlotSpatialPoints.py
 PAMI/extras/topKPatterns.py
 PAMI/extras/uncertaindb_convert.py
@@ -116,27 +116,27 @@
 PAMI/frequentSpatialPattern/basic/SpatialECLAT.py
 PAMI/frequentSpatialPattern/basic/__init__.py
 PAMI/frequentSpatialPattern/basic/abstract.py
 PAMI/fuzzyCorrelatedPattern/__init__.py
 PAMI/fuzzyCorrelatedPattern/basic/FCPGrowth.py
 PAMI/fuzzyCorrelatedPattern/basic/__init__.py
 PAMI/fuzzyCorrelatedPattern/basic/abstract.py
-PAMI/fuzzyFrequentPattern/__init__.py
-PAMI/fuzzyFrequentPattern/basic/FFIMiner.py
-PAMI/fuzzyFrequentPattern/basic/FFIMiner_old.py
-PAMI/fuzzyFrequentPattern/basic/__init__.py
-PAMI/fuzzyFrequentPattern/basic/abstract.py
+PAMI/fuzzyFrequentPatterns/__init__.py
+PAMI/fuzzyFrequentPatterns/basic/FFIMiner.py
+PAMI/fuzzyFrequentPatterns/basic/FFIMiner_old.py
+PAMI/fuzzyFrequentPatterns/basic/__init__.py
+PAMI/fuzzyFrequentPatterns/basic/abstract.py
 PAMI/fuzzyFrequentSpatialPattern/__init__.py
 PAMI/fuzzyFrequentSpatialPattern/basic/FFSPMiner.py
 PAMI/fuzzyFrequentSpatialPattern/basic/FFSPMiner_old.py
 PAMI/fuzzyFrequentSpatialPattern/basic/__init__.py
 PAMI/fuzzyFrequentSpatialPattern/basic/abstract.py
-PAMI/fuzzyPartialPeriodicPattern/__init__.py
-PAMI/fuzzyPartialPeriodicPattern/irregularTimeSeries/__init__.py
-PAMI/fuzzyPartialPeriodicPattern/irregularTimeSeries/abstract.py
+PAMI/fuzzyPartialPeriodicPatterns/__init__.py
+PAMI/fuzzyPartialPeriodicPatterns/irregularTimeSeries/__init__.py
+PAMI/fuzzyPartialPeriodicPatterns/irregularTimeSeries/abstract.py
 PAMI/fuzzyPeriodicFrequentPattern/__init__.py
 PAMI/fuzzyPeriodicFrequentPattern/basic/FPFPMiner.py
 PAMI/fuzzyPeriodicFrequentPattern/basic/FPFPMiner_old.py
 PAMI/fuzzyPeriodicFrequentPattern/basic/__init__.py
 PAMI/fuzzyPeriodicFrequentPattern/basic/abstract.py
 PAMI/fuzzySpatialPeriodicFrequentPattern/__init__.py
 PAMI/fuzzySpatialPeriodicFrequentPattern/basic/FGPFPMiner.py
@@ -148,36 +148,32 @@
 PAMI/geoReferencedFrequentPattern/abstract.py
 PAMI/geoReferencedPeriodicFrequentPattern/__init__.py
 PAMI/geoReferencedPeriodicFrequentPattern/basic/GPFPMiner.py
 PAMI/geoReferencedPeriodicFrequentPattern/basic/__init__.py
 PAMI/geoReferencedPeriodicFrequentPattern/basic/abstract.py
 PAMI/georeferencedFrequentSequencePattern/__init__.py
 PAMI/georeferencedFrequentSequencePattern/abstract.py
-PAMI/highUtilityFrequentPattern/__init__.py
-PAMI/highUtilityFrequentPattern/basic/HUFIM.py
-PAMI/highUtilityFrequentPattern/basic/__init__.py
-PAMI/highUtilityFrequentPattern/basic/abstract.py
+PAMI/highUtilityFrequentPatterns/__init__.py
+PAMI/highUtilityFrequentPatterns/basic/HUFIM.py
+PAMI/highUtilityFrequentPatterns/basic/__init__.py
+PAMI/highUtilityFrequentPatterns/basic/abstract.py
 PAMI/highUtilityFrequentSpatialPattern/__init__.py
 PAMI/highUtilityFrequentSpatialPattern/basic/SHUFIM.py
 PAMI/highUtilityFrequentSpatialPattern/basic/__init__.py
 PAMI/highUtilityFrequentSpatialPattern/basic/abstract.py
-PAMI/highUtilityPattern/__init__.py
-PAMI/highUtilityPattern/basic/EFIM.py
-PAMI/highUtilityPattern/basic/HMiner.py
-PAMI/highUtilityPattern/basic/UPGrowth.py
-PAMI/highUtilityPattern/basic/__init__.py
-PAMI/highUtilityPattern/basic/abstract.py
-PAMI/highUtilityPattern/basic/efimParallel.py
-PAMI/highUtilityPattern/parallel/__init__.py
-PAMI/highUtilityPattern/parallel/abstract.py
-PAMI/highUtilityPattern/parallel/efimparallel.py
-PAMI/highUtilityPatternsInStreams/HUPMS.py
-PAMI/highUtilityPatternsInStreams/SHUGrowth.py
-PAMI/highUtilityPatternsInStreams/__init__.py
-PAMI/highUtilityPatternsInStreams/abstract.py
+PAMI/highUtilityPatterns/__init__.py
+PAMI/highUtilityPatterns/basic/EFIM.py
+PAMI/highUtilityPatterns/basic/HMiner.py
+PAMI/highUtilityPatterns/basic/UPGrowth.py
+PAMI/highUtilityPatterns/basic/__init__.py
+PAMI/highUtilityPatterns/basic/abstract.py
+PAMI/highUtilityPatterns/basic/efimParallel.py
+PAMI/highUtilityPatterns/parallel/__init__.py
+PAMI/highUtilityPatterns/parallel/abstract.py
+PAMI/highUtilityPatterns/parallel/efimparallel.py
 PAMI/highUtilitySpatialPattern/__init__.py
 PAMI/highUtilitySpatialPattern/abstract.py
 PAMI/highUtilitySpatialPattern/basic/HDSHUIM.py
 PAMI/highUtilitySpatialPattern/basic/SHUIM.py
 PAMI/highUtilitySpatialPattern/basic/__init__.py
 PAMI/highUtilitySpatialPattern/basic/abstract.py
 PAMI/highUtilitySpatialPattern/topk/TKSHUIM.py
@@ -251,23 +247,22 @@
 PAMI/periodicFrequentPattern/topk/kPFPMiner/__init__.py
 PAMI/periodicFrequentPattern/topk/kPFPMiner/abstract.py
 PAMI/periodicFrequentPattern/topk/kPFPMiner/kPFPMiner.py
 PAMI/recurringPattern/__init__.py
 PAMI/recurringPattern/basic/RPGrowth.py
 PAMI/recurringPattern/basic/__init__.py
 PAMI/recurringPattern/basic/abstract.py
-PAMI/relativeFrequentPattern/__init__.py
-PAMI/relativeFrequentPattern/basic/RSFPGrowth.py
-PAMI/relativeFrequentPattern/basic/__init__.py
-PAMI/relativeFrequentPattern/basic/abstract.py
-PAMI/relativeHighUtilityPattern/__init__.py
-PAMI/relativeHighUtilityPattern/basic/RHUIM.py
-PAMI/relativeHighUtilityPattern/basic/__init__.py
-PAMI/relativeHighUtilityPattern/basic/abstract.py
-PAMI/sequence/__init__.py
+PAMI/relativeFrequentPatterns/__init__.py
+PAMI/relativeFrequentPatterns/basic/RSFPGrowth.py
+PAMI/relativeFrequentPatterns/basic/__init__.py
+PAMI/relativeFrequentPatterns/basic/abstract.py
+PAMI/relativeHighUtilityPatterns/__init__.py
+PAMI/relativeHighUtilityPatterns/basic/RHUIM.py
+PAMI/relativeHighUtilityPatterns/basic/__init__.py
+PAMI/relativeHighUtilityPatterns/basic/abstract.py
 PAMI/sequentialPatternMining/__init__.py
 PAMI/sequentialPatternMining/basic/SPADE.py
 PAMI/sequentialPatternMining/basic/__init__.py
 PAMI/sequentialPatternMining/basic/abstract.py
 PAMI/sequentialPatternMining/basic/prefixSpan.py
 PAMI/sequentialPatternMining/closed/__init__.py
 PAMI/sequentialPatternMining/closed/abstract.py
@@ -277,14 +272,23 @@
 PAMI/stablePeriodicFrequentPattern/basic/SPPGrowth.py
 PAMI/stablePeriodicFrequentPattern/basic/SPPGrowthDump.py
 PAMI/stablePeriodicFrequentPattern/basic/__init__.py
 PAMI/stablePeriodicFrequentPattern/basic/abstract.py
 PAMI/stablePeriodicFrequentPattern/topK/TSPIN.py
 PAMI/stablePeriodicFrequentPattern/topK/__init__.py
 PAMI/stablePeriodicFrequentPattern/topK/abstract.py
+PAMI/streams/__init__.py
+PAMI/streams/frequentPatterns/__init__.py
+PAMI/streams/frequentPatterns/basic/FPStream.py
+PAMI/streams/frequentPatterns/basic/__init__.py
+PAMI/streams/frequentPatterns/basic/abstract.py
+PAMI/streams/highUtility/HUPMS.py
+PAMI/streams/highUtility/SHUGrowth.py
+PAMI/streams/highUtility/__init__.py
+PAMI/streams/highUtility/abstract.py
 PAMI/uncertainFrequentPattern/__init__.py
 PAMI/uncertainFrequentPattern/basic/CUFPTree.py
 PAMI/uncertainFrequentPattern/basic/PUFGrowth.py
 PAMI/uncertainFrequentPattern/basic/TUFP.py
 PAMI/uncertainFrequentPattern/basic/TubeP.py
 PAMI/uncertainFrequentPattern/basic/TubeS.py
 PAMI/uncertainFrequentPattern/basic/UFGrowth.py
```

### Comparing `pami-2023.7.21/setup.py` & `pami-2023.7.7/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 import setuptools
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setuptools.setup(
-    name='pami',
-    version='2023.07.21',
-    author='Rage Uday Kiran',
-    author_email='uday.rage@gmail.com',
-    description='This software is being developed at the University of Aizu, Aizu-Wakamatsu, Fukushima, Japan',
-    long_description=long_description,
-    long_description_content_type='text/markdown',
+    name = 'pami',
+    version = '2023.07.07',
+    author = 'Rage Uday Kiran',
+    author_email = 'uday.rage@gmail.com',
+    description = 'This software is being developed at the University of Aizu, Aizu-Wakamatsu, Fukushima, Japan',
+    long_description = long_description,
+    long_description_content_type = 'text/markdown',
     packages=setuptools.find_packages(),
-    url='https://github.com/udayLab/PAMI',
+    url = 'https://github.com/udayRage/PAMI',
     license='GPLv3',
     install_requires=[            # All necessary packages utilized by our PAMI software
         'psutil',
         'pandas',
         'plotly',
         'matplotlib',
         'resource',
         'validators',
         'urllib3',
         'Pillow',
         'numpy',
     ],
-    extras_require={
-        'gpu':  ['cupy', 'pycuda'],
+    extras_require = {
+        'gpu':  ['cupy'],
         'spark': ['pyspark'],
     },
-    classifiers=[
-        'Development Status :: 4 - Beta',      # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
+    classifiers = [
+        'Development Status :: 5 - Production/Stable',      # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
         'Operating System :: OS Independent',
     ],
-    python_requires='>=3.5',
+    python_requires = '>=3.5',
 )
```

