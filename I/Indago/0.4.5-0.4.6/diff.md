# Comparing `tmp/Indago-0.4.5-py3-none-any.whl.zip` & `tmp/Indago-0.4.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,23 +1,383 @@
-Zip file size: 60487 bytes, number of entries: 21
--rw-r--r--  2.0 unx     1062 b- defN 23-Jun-01 11:48 indago/__init__.py
--rw-r--r--  2.0 unx     6956 b- defN 23-Mar-15 10:01 indago/_abc.py
--rw-r--r--  2.0 unx     7210 b- defN 23-Mar-15 10:01 indago/_ba.py
--rw-r--r--  2.0 unx    12174 b- defN 23-Mar-15 10:01 indago/_de.py
--rw-r--r--  2.0 unx    21848 b- defN 23-Mar-15 16:02 indago/_direct_search.py
--rw-r--r--  2.0 unx     7545 b- defN 23-Mar-15 10:01 indago/_efo.py
--rw-r--r--  2.0 unx    11124 b- defN 23-Mar-15 10:01 indago/_fwa.py
--rw-r--r--  2.0 unx    38281 b- defN 23-Mar-15 10:01 indago/_mmo.py
--rw-r--r--  2.0 unx     6123 b- defN 23-Mar-15 10:01 indago/_mrfo.py
--rw-r--r--  2.0 unx    67766 b- defN 23-Jun-01 10:04 indago/_optimizer.py
--rw-r--r--  2.0 unx    15867 b- defN 23-Jun-01 09:49 indago/_pso.py
--rw-r--r--  2.0 unx     3826 b- defN 23-Mar-15 10:01 indago/_sa.py
--rw-r--r--  2.0 unx     8539 b- defN 23-Mar-15 10:01 indago/_ssa.py
--rw-r--r--  2.0 unx    21438 b- defN 23-Feb-16 08:53 indago/_utility.py
--rw-r--r--  2.0 unx       67 b- defN 21-Sep-22 11:40 indago/benchmarks/__init__.py
--rw-r--r--  2.0 unx    18220 b- defN 23-Mar-15 10:01 indago/benchmarks/_cec.py
--rw-r--r--  2.0 unx     5884 b- defN 20-Oct-10 06:48 indago/benchmarks/_shortest_path.py
--rw-r--r--  2.0 unx     1513 b- defN 23-Jun-01 11:52 Indago-0.4.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-01 11:52 Indago-0.4.5.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 23-Jun-01 11:52 Indago-0.4.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1575 b- defN 23-Jun-01 11:52 Indago-0.4.5.dist-info/RECORD
-21 files, 257117 bytes uncompressed, 58007 bytes compressed:  77.4%
+Zip file size: 3045790 bytes, number of entries: 381
+-rw-r--r--  2.0 unx     1062 b- defN 23-Jul-21 13:48 indago/__init__.py
+-rw-r--r--  2.0 unx     6670 b- defN 23-Jul-06 19:56 indago/_abc.py
+-rw-r--r--  2.0 unx     7214 b- defN 23-Jul-06 19:56 indago/_ba.py
+-rw-r--r--  2.0 unx    12441 b- defN 23-Jul-06 19:56 indago/_de.py
+-rw-r--r--  2.0 unx    22297 b- defN 23-Jul-06 19:56 indago/_direct_search.py
+-rw-r--r--  2.0 unx     7272 b- defN 23-Jul-06 19:56 indago/_efo.py
+-rw-r--r--  2.0 unx    11187 b- defN 23-Jul-06 19:56 indago/_fwa.py
+-rw-r--r--  2.0 unx    38302 b- defN 23-Jul-09 09:04 indago/_mmo.py
+-rw-r--r--  2.0 unx     6352 b- defN 23-Jul-06 19:56 indago/_mrfo.py
+-rw-r--r--  2.0 unx    69664 b- defN 23-Jul-14 20:05 indago/_optimizer.py
+-rw-r--r--  2.0 unx    16180 b- defN 23-Jul-06 19:56 indago/_pso.py
+-rw-r--r--  2.0 unx     3720 b- defN 23-Jul-06 19:56 indago/_sa.py
+-rw-r--r--  2.0 unx     8518 b- defN 23-Jul-06 19:56 indago/_ssa.py
+-rw-r--r--  2.0 unx    21438 b- defN 23-Feb-15 22:09 indago/_utility.py
+-rw-r--r--  2.0 unx       67 b- defN 22-Nov-08 19:54 indago/benchmarks/__init__.py
+-rw-r--r--  2.0 unx    18220 b- defN 23-Mar-26 20:52 indago/benchmarks/_cec.py
+-rw-r--r--  2.0 unx     5884 b- defN 22-Nov-08 19:54 indago/benchmarks/_shortest_path.py
+-rw-r--r--  2.0 unx     2510 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_10_D10.txt
+-rw-r--r--  2.0 unx   250100 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_10_D100.txt
+-rw-r--r--  2.0 unx      102 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_10_D2.txt
+-rw-r--r--  2.0 unx    10020 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_10_D20.txt
+-rw-r--r--  2.0 unx    22530 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_10_D30.txt
+-rw-r--r--  2.0 unx    62550 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_10_D50.txt
+-rw-r--r--  2.0 unx     2510 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_11_D10.txt
+-rw-r--r--  2.0 unx   250100 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_11_D100.txt
+-rw-r--r--  2.0 unx      102 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_11_D2.txt
+-rw-r--r--  2.0 unx    10020 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_11_D20.txt
+-rw-r--r--  2.0 unx    22530 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_11_D30.txt
+-rw-r--r--  2.0 unx    62550 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_11_D50.txt
+-rw-r--r--  2.0 unx     2510 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_12_D10.txt
+-rw-r--r--  2.0 unx   250100 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_12_D100.txt
+-rw-r--r--  2.0 unx      102 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_12_D2.txt
+-rw-r--r--  2.0 unx    10020 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_12_D20.txt
+-rw-r--r--  2.0 unx    22530 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_12_D30.txt
+-rw-r--r--  2.0 unx    62550 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_12_D50.txt
+-rw-r--r--  2.0 unx     2510 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_13_D10.txt
+-rw-r--r--  2.0 unx   250100 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_13_D100.txt
+-rw-r--r--  2.0 unx      102 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_13_D2.txt
+-rw-r--r--  2.0 unx    10020 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_13_D20.txt
+-rw-r--r--  2.0 unx    22530 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_13_D30.txt
+-rw-r--r--  2.0 unx    62550 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_13_D50.txt
+-rw-r--r--  2.0 unx     2510 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_14_D10.txt
+-rw-r--r--  2.0 unx   250100 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_14_D100.txt
+-rw-r--r--  2.0 unx      102 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_14_D2.txt
+-rw-r--r--  2.0 unx    10020 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_14_D20.txt
+-rw-r--r--  2.0 unx    22530 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_14_D30.txt
+-rw-r--r--  2.0 unx    62550 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_14_D50.txt
+-rw-r--r--  2.0 unx     2510 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_15_D10.txt
+-rw-r--r--  2.0 unx   250100 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_15_D100.txt
+-rw-r--r--  2.0 unx      102 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_15_D2.txt
+-rw-r--r--  2.0 unx    10020 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_15_D20.txt
+-rw-r--r--  2.0 unx    22530 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_15_D30.txt
+-rw-r--r--  2.0 unx    62550 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_15_D50.txt
+-rw-r--r--  2.0 unx     2510 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_16_D10.txt
+-rw-r--r--  2.0 unx   250100 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_16_D100.txt
+-rw-r--r--  2.0 unx      102 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_16_D2.txt
+-rw-r--r--  2.0 unx    10020 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_16_D20.txt
+-rw-r--r--  2.0 unx    22530 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_16_D30.txt
+-rw-r--r--  2.0 unx    62550 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_16_D50.txt
+-rw-r--r--  2.0 unx     2510 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_17_D10.txt
+-rw-r--r--  2.0 unx   250100 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_17_D100.txt
+-rw-r--r--  2.0 unx      102 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_17_D2.txt
+-rw-r--r--  2.0 unx    10020 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_17_D20.txt
+-rw-r--r--  2.0 unx    22530 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_17_D30.txt
+-rw-r--r--  2.0 unx    62550 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_17_D50.txt
+-rw-r--r--  2.0 unx     2510 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_18_D10.txt
+-rw-r--r--  2.0 unx   250100 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_18_D100.txt
+-rw-r--r--  2.0 unx      102 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_18_D2.txt
+-rw-r--r--  2.0 unx    10020 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_18_D20.txt
+-rw-r--r--  2.0 unx    22530 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_18_D30.txt
+-rw-r--r--  2.0 unx    62550 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_18_D50.txt
+-rw-r--r--  2.0 unx     2510 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_19_D10.txt
+-rw-r--r--  2.0 unx   250100 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_19_D100.txt
+-rw-r--r--  2.0 unx      102 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_19_D2.txt
+-rw-r--r--  2.0 unx    10020 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_19_D20.txt
+-rw-r--r--  2.0 unx    22530 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_19_D30.txt
+-rw-r--r--  2.0 unx    62550 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_19_D50.txt
+-rw-r--r--  2.0 unx     2510 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_1_D10.txt
+-rw-r--r--  2.0 unx   250100 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_1_D100.txt
+-rw-r--r--  2.0 unx      102 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_1_D2.txt
+-rw-r--r--  2.0 unx    10020 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_1_D20.txt
+-rw-r--r--  2.0 unx    22530 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_1_D30.txt
+-rw-r--r--  2.0 unx    62550 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_1_D50.txt
+-rw-r--r--  2.0 unx     2510 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_20_D10.txt
+-rw-r--r--  2.0 unx   250100 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_20_D100.txt
+-rw-r--r--  2.0 unx      102 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_20_D2.txt
+-rw-r--r--  2.0 unx    10020 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_20_D20.txt
+-rw-r--r--  2.0 unx    22530 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_20_D30.txt
+-rw-r--r--  2.0 unx    62550 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_20_D50.txt
+-rw-r--r--  2.0 unx     2510 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_21_D10.txt
+-rw-r--r--  2.0 unx   250100 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_21_D100.txt
+-rw-r--r--  2.0 unx      102 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_21_D2.txt
+-rw-r--r--  2.0 unx    10020 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_21_D20.txt
+-rw-r--r--  2.0 unx    22530 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_21_D30.txt
+-rw-r--r--  2.0 unx    62550 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_21_D50.txt
+-rw-r--r--  2.0 unx     2510 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_22_D10.txt
+-rw-r--r--  2.0 unx   250100 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_22_D100.txt
+-rw-r--r--  2.0 unx      102 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_22_D2.txt
+-rw-r--r--  2.0 unx    10020 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_22_D20.txt
+-rw-r--r--  2.0 unx    22530 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_22_D30.txt
+-rw-r--r--  2.0 unx    62550 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_22_D50.txt
+-rw-r--r--  2.0 unx    25100 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_23_D10.txt
+-rw-r--r--  2.0 unx  2501000 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_23_D100.txt
+-rw-r--r--  2.0 unx      816 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_23_D2.txt
+-rw-r--r--  2.0 unx   100200 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_23_D20.txt
+-rw-r--r--  2.0 unx   225300 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_23_D30.txt
+-rw-r--r--  2.0 unx   625500 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_23_D50.txt
+-rw-r--r--  2.0 unx    25100 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_24_D10.txt
+-rw-r--r--  2.0 unx  2501000 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_24_D100.txt
+-rw-r--r--  2.0 unx      816 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_24_D2.txt
+-rw-r--r--  2.0 unx   100200 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_24_D20.txt
+-rw-r--r--  2.0 unx   225300 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_24_D30.txt
+-rw-r--r--  2.0 unx   625500 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_24_D50.txt
+-rw-r--r--  2.0 unx    25100 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_25_D10.txt
+-rw-r--r--  2.0 unx  2501000 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_25_D100.txt
+-rw-r--r--  2.0 unx      816 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_25_D2.txt
+-rw-r--r--  2.0 unx   100200 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_25_D20.txt
+-rw-r--r--  2.0 unx   225300 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_25_D30.txt
+-rw-r--r--  2.0 unx   625500 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_25_D50.txt
+-rw-r--r--  2.0 unx    25100 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_26_D10.txt
+-rw-r--r--  2.0 unx  2501000 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_26_D100.txt
+-rw-r--r--  2.0 unx      816 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_26_D2.txt
+-rw-r--r--  2.0 unx   100200 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_26_D20.txt
+-rw-r--r--  2.0 unx   225300 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_26_D30.txt
+-rw-r--r--  2.0 unx   625500 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_26_D50.txt
+-rw-r--r--  2.0 unx    25100 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_27_D10.txt
+-rw-r--r--  2.0 unx  2501000 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_27_D100.txt
+-rw-r--r--  2.0 unx      816 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_27_D2.txt
+-rw-r--r--  2.0 unx   100200 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_27_D20.txt
+-rw-r--r--  2.0 unx   225300 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_27_D30.txt
+-rw-r--r--  2.0 unx   625500 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_27_D50.txt
+-rw-r--r--  2.0 unx    25100 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_28_D10.txt
+-rw-r--r--  2.0 unx  2501000 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_28_D100.txt
+-rw-r--r--  2.0 unx      816 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_28_D2.txt
+-rw-r--r--  2.0 unx   100200 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_28_D20.txt
+-rw-r--r--  2.0 unx   225300 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_28_D30.txt
+-rw-r--r--  2.0 unx   625500 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_28_D50.txt
+-rw-r--r--  2.0 unx    25100 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_29_D10.txt
+-rw-r--r--  2.0 unx  2501000 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_29_D100.txt
+-rw-r--r--  2.0 unx      816 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_29_D2.txt
+-rw-r--r--  2.0 unx   100200 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_29_D20.txt
+-rw-r--r--  2.0 unx   225300 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_29_D30.txt
+-rw-r--r--  2.0 unx   625500 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_29_D50.txt
+-rw-r--r--  2.0 unx     2510 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_2_D10.txt
+-rw-r--r--  2.0 unx   250100 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_2_D100.txt
+-rw-r--r--  2.0 unx      102 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_2_D2.txt
+-rw-r--r--  2.0 unx    10020 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_2_D20.txt
+-rw-r--r--  2.0 unx    22530 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_2_D30.txt
+-rw-r--r--  2.0 unx    62550 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_2_D50.txt
+-rw-r--r--  2.0 unx    25100 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_30_D10.txt
+-rw-r--r--  2.0 unx  2501000 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_30_D100.txt
+-rw-r--r--  2.0 unx      816 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_30_D2.txt
+-rw-r--r--  2.0 unx   100200 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_30_D20.txt
+-rw-r--r--  2.0 unx   225300 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_30_D30.txt
+-rw-r--r--  2.0 unx   625500 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_30_D50.txt
+-rw-r--r--  2.0 unx     2510 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_3_D10.txt
+-rw-r--r--  2.0 unx   250100 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_3_D100.txt
+-rw-r--r--  2.0 unx      102 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_3_D2.txt
+-rw-r--r--  2.0 unx    10020 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_3_D20.txt
+-rw-r--r--  2.0 unx    22530 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_3_D30.txt
+-rw-r--r--  2.0 unx    62550 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_3_D50.txt
+-rw-r--r--  2.0 unx     2510 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_4_D10.txt
+-rw-r--r--  2.0 unx   250100 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_4_D100.txt
+-rw-r--r--  2.0 unx      102 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_4_D2.txt
+-rw-r--r--  2.0 unx    10020 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_4_D20.txt
+-rw-r--r--  2.0 unx    22530 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_4_D30.txt
+-rw-r--r--  2.0 unx    62550 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_4_D50.txt
+-rw-r--r--  2.0 unx     2510 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_5_D10.txt
+-rw-r--r--  2.0 unx   250100 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_5_D100.txt
+-rw-r--r--  2.0 unx      102 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_5_D2.txt
+-rw-r--r--  2.0 unx    10020 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_5_D20.txt
+-rw-r--r--  2.0 unx    22530 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_5_D30.txt
+-rw-r--r--  2.0 unx    62550 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_5_D50.txt
+-rw-r--r--  2.0 unx     2510 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_6_D10.txt
+-rw-r--r--  2.0 unx   250100 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_6_D100.txt
+-rw-r--r--  2.0 unx      102 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_6_D2.txt
+-rw-r--r--  2.0 unx    10020 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_6_D20.txt
+-rw-r--r--  2.0 unx    22530 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_6_D30.txt
+-rw-r--r--  2.0 unx    62550 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_6_D50.txt
+-rw-r--r--  2.0 unx     2510 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_7_D10.txt
+-rw-r--r--  2.0 unx   250100 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_7_D100.txt
+-rw-r--r--  2.0 unx      102 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_7_D2.txt
+-rw-r--r--  2.0 unx    10020 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_7_D20.txt
+-rw-r--r--  2.0 unx    22530 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_7_D30.txt
+-rw-r--r--  2.0 unx    62550 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_7_D50.txt
+-rw-r--r--  2.0 unx     2510 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_8_D10.txt
+-rw-r--r--  2.0 unx   250100 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_8_D100.txt
+-rw-r--r--  2.0 unx      102 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_8_D2.txt
+-rw-r--r--  2.0 unx    10020 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_8_D20.txt
+-rw-r--r--  2.0 unx    22530 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_8_D30.txt
+-rw-r--r--  2.0 unx    62550 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_8_D50.txt
+-rw-r--r--  2.0 unx     2510 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_9_D10.txt
+-rw-r--r--  2.0 unx   250100 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_9_D100.txt
+-rw-r--r--  2.0 unx      102 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_9_D2.txt
+-rw-r--r--  2.0 unx    10020 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_9_D20.txt
+-rw-r--r--  2.0 unx    22530 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_9_D30.txt
+-rw-r--r--  2.0 unx    62550 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/M_9_D50.txt
+-rw-r--r--  2.0 unx     2501 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shift_data_1.txt
+-rw-r--r--  2.0 unx     2501 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shift_data_10.txt
+-rw-r--r--  2.0 unx     2501 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shift_data_11.txt
+-rw-r--r--  2.0 unx     2501 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shift_data_12.txt
+-rw-r--r--  2.0 unx     2501 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shift_data_13.txt
+-rw-r--r--  2.0 unx     2501 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shift_data_14.txt
+-rw-r--r--  2.0 unx     2501 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shift_data_15.txt
+-rw-r--r--  2.0 unx     2501 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shift_data_16.txt
+-rw-r--r--  2.0 unx     2501 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shift_data_17.txt
+-rw-r--r--  2.0 unx     2501 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shift_data_18.txt
+-rw-r--r--  2.0 unx     2501 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shift_data_19.txt
+-rw-r--r--  2.0 unx     2501 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shift_data_2.txt
+-rw-r--r--  2.0 unx     2501 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shift_data_20.txt
+-rw-r--r--  2.0 unx     2501 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shift_data_21.txt
+-rw-r--r--  2.0 unx     2501 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shift_data_22.txt
+-rw-r--r--  2.0 unx    25010 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shift_data_23.txt
+-rw-r--r--  2.0 unx    25010 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shift_data_24.txt
+-rw-r--r--  2.0 unx    25010 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shift_data_25.txt
+-rw-r--r--  2.0 unx    25010 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shift_data_26.txt
+-rw-r--r--  2.0 unx    25010 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shift_data_27.txt
+-rw-r--r--  2.0 unx    25010 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shift_data_28.txt
+-rw-r--r--  2.0 unx    25010 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shift_data_29.txt
+-rw-r--r--  2.0 unx     2501 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shift_data_3.txt
+-rw-r--r--  2.0 unx    25010 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shift_data_30.txt
+-rw-r--r--  2.0 unx     2501 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shift_data_4.txt
+-rw-r--r--  2.0 unx     2501 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shift_data_5.txt
+-rw-r--r--  2.0 unx     2501 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shift_data_6.txt
+-rw-r--r--  2.0 unx     2501 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shift_data_7.txt
+-rw-r--r--  2.0 unx     2501 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shift_data_8.txt
+-rw-r--r--  2.0 unx     2501 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shift_data_9.txt
+-rw-r--r--  2.0 unx       21 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_10_D10.txt
+-rw-r--r--  2.0 unx      292 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_10_D100.txt
+-rw-r--r--  2.0 unx       51 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_10_D20.txt
+-rw-r--r--  2.0 unx       81 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_10_D30.txt
+-rw-r--r--  2.0 unx      141 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_10_D50.txt
+-rw-r--r--  2.0 unx       21 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_11_D10.txt
+-rw-r--r--  2.0 unx      292 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_11_D100.txt
+-rw-r--r--  2.0 unx       51 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_11_D20.txt
+-rw-r--r--  2.0 unx       81 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_11_D30.txt
+-rw-r--r--  2.0 unx      141 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_11_D50.txt
+-rw-r--r--  2.0 unx       21 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_12_D10.txt
+-rw-r--r--  2.0 unx      292 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_12_D100.txt
+-rw-r--r--  2.0 unx       51 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_12_D20.txt
+-rw-r--r--  2.0 unx       81 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_12_D30.txt
+-rw-r--r--  2.0 unx      141 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_12_D50.txt
+-rw-r--r--  2.0 unx       21 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_13_D10.txt
+-rw-r--r--  2.0 unx      292 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_13_D100.txt
+-rw-r--r--  2.0 unx       51 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_13_D20.txt
+-rw-r--r--  2.0 unx       81 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_13_D30.txt
+-rw-r--r--  2.0 unx      141 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_13_D50.txt
+-rw-r--r--  2.0 unx       21 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_14_D10.txt
+-rw-r--r--  2.0 unx      292 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_14_D100.txt
+-rw-r--r--  2.0 unx       51 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_14_D20.txt
+-rw-r--r--  2.0 unx       81 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_14_D30.txt
+-rw-r--r--  2.0 unx      141 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_14_D50.txt
+-rw-r--r--  2.0 unx       21 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_15_D10.txt
+-rw-r--r--  2.0 unx      292 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_15_D100.txt
+-rw-r--r--  2.0 unx       51 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_15_D20.txt
+-rw-r--r--  2.0 unx       81 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_15_D30.txt
+-rw-r--r--  2.0 unx      141 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_15_D50.txt
+-rw-r--r--  2.0 unx       21 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_16_D10.txt
+-rw-r--r--  2.0 unx      292 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_16_D100.txt
+-rw-r--r--  2.0 unx       51 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_16_D20.txt
+-rw-r--r--  2.0 unx       81 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_16_D30.txt
+-rw-r--r--  2.0 unx      141 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_16_D50.txt
+-rw-r--r--  2.0 unx       21 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_17_D10.txt
+-rw-r--r--  2.0 unx      292 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_17_D100.txt
+-rw-r--r--  2.0 unx       51 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_17_D20.txt
+-rw-r--r--  2.0 unx       81 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_17_D30.txt
+-rw-r--r--  2.0 unx      141 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_17_D50.txt
+-rw-r--r--  2.0 unx       21 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_18_D10.txt
+-rw-r--r--  2.0 unx      292 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_18_D100.txt
+-rw-r--r--  2.0 unx       51 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_18_D20.txt
+-rw-r--r--  2.0 unx       81 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_18_D30.txt
+-rw-r--r--  2.0 unx      141 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_18_D50.txt
+-rw-r--r--  2.0 unx       21 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_19_D10.txt
+-rw-r--r--  2.0 unx      292 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_19_D100.txt
+-rw-r--r--  2.0 unx       51 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_19_D20.txt
+-rw-r--r--  2.0 unx       81 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_19_D30.txt
+-rw-r--r--  2.0 unx      141 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_19_D50.txt
+-rw-r--r--  2.0 unx       21 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_1_D10.txt
+-rw-r--r--  2.0 unx      292 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_1_D100.txt
+-rw-r--r--  2.0 unx       51 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_1_D20.txt
+-rw-r--r--  2.0 unx       81 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_1_D30.txt
+-rw-r--r--  2.0 unx      141 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_1_D50.txt
+-rw-r--r--  2.0 unx       21 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_20_D10.txt
+-rw-r--r--  2.0 unx      292 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_20_D100.txt
+-rw-r--r--  2.0 unx       51 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_20_D20.txt
+-rw-r--r--  2.0 unx       81 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_20_D30.txt
+-rw-r--r--  2.0 unx      141 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_20_D50.txt
+-rw-r--r--  2.0 unx       21 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_21_D10.txt
+-rw-r--r--  2.0 unx      292 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_21_D100.txt
+-rw-r--r--  2.0 unx       51 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_21_D20.txt
+-rw-r--r--  2.0 unx       81 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_21_D30.txt
+-rw-r--r--  2.0 unx      141 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_21_D50.txt
+-rw-r--r--  2.0 unx       21 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_22_D10.txt
+-rw-r--r--  2.0 unx      292 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_22_D100.txt
+-rw-r--r--  2.0 unx       51 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_22_D20.txt
+-rw-r--r--  2.0 unx       81 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_22_D30.txt
+-rw-r--r--  2.0 unx      141 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_22_D50.txt
+-rw-r--r--  2.0 unx      210 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_23_D10.txt
+-rw-r--r--  2.0 unx     2920 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_23_D100.txt
+-rw-r--r--  2.0 unx      510 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_23_D20.txt
+-rw-r--r--  2.0 unx      810 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_23_D30.txt
+-rw-r--r--  2.0 unx     1410 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_23_D50.txt
+-rw-r--r--  2.0 unx      210 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_24_D10.txt
+-rw-r--r--  2.0 unx     2920 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_24_D100.txt
+-rw-r--r--  2.0 unx      510 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_24_D20.txt
+-rw-r--r--  2.0 unx      810 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_24_D30.txt
+-rw-r--r--  2.0 unx     1410 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_24_D50.txt
+-rw-r--r--  2.0 unx      210 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_25_D10.txt
+-rw-r--r--  2.0 unx     2920 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_25_D100.txt
+-rw-r--r--  2.0 unx      510 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_25_D20.txt
+-rw-r--r--  2.0 unx      810 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_25_D30.txt
+-rw-r--r--  2.0 unx     1410 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_25_D50.txt
+-rw-r--r--  2.0 unx      210 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_26_D10.txt
+-rw-r--r--  2.0 unx     2920 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_26_D100.txt
+-rw-r--r--  2.0 unx      510 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_26_D20.txt
+-rw-r--r--  2.0 unx      810 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_26_D30.txt
+-rw-r--r--  2.0 unx     1410 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_26_D50.txt
+-rw-r--r--  2.0 unx      210 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_27_D10.txt
+-rw-r--r--  2.0 unx     2920 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_27_D100.txt
+-rw-r--r--  2.0 unx      510 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_27_D20.txt
+-rw-r--r--  2.0 unx      810 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_27_D30.txt
+-rw-r--r--  2.0 unx     1410 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_27_D50.txt
+-rw-r--r--  2.0 unx      210 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_28_D10.txt
+-rw-r--r--  2.0 unx     2920 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_28_D100.txt
+-rw-r--r--  2.0 unx      510 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_28_D20.txt
+-rw-r--r--  2.0 unx      810 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_28_D30.txt
+-rw-r--r--  2.0 unx     1410 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_28_D50.txt
+-rw-r--r--  2.0 unx      210 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_29_D10.txt
+-rw-r--r--  2.0 unx     2920 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_29_D100.txt
+-rw-r--r--  2.0 unx      510 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_29_D20.txt
+-rw-r--r--  2.0 unx      810 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_29_D30.txt
+-rw-r--r--  2.0 unx     1410 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_29_D50.txt
+-rw-r--r--  2.0 unx       21 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_2_D10.txt
+-rw-r--r--  2.0 unx      292 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_2_D100.txt
+-rw-r--r--  2.0 unx       51 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_2_D20.txt
+-rw-r--r--  2.0 unx       81 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_2_D30.txt
+-rw-r--r--  2.0 unx      141 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_2_D50.txt
+-rw-r--r--  2.0 unx      210 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_30_D10.txt
+-rw-r--r--  2.0 unx     2920 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_30_D100.txt
+-rw-r--r--  2.0 unx      510 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_30_D20.txt
+-rw-r--r--  2.0 unx      810 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_30_D30.txt
+-rw-r--r--  2.0 unx     1410 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_30_D50.txt
+-rw-r--r--  2.0 unx       21 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_3_D10.txt
+-rw-r--r--  2.0 unx      292 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_3_D100.txt
+-rw-r--r--  2.0 unx       51 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_3_D20.txt
+-rw-r--r--  2.0 unx       81 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_3_D30.txt
+-rw-r--r--  2.0 unx      141 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_3_D50.txt
+-rw-r--r--  2.0 unx       21 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_4_D10.txt
+-rw-r--r--  2.0 unx      292 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_4_D100.txt
+-rw-r--r--  2.0 unx       51 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_4_D20.txt
+-rw-r--r--  2.0 unx       81 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_4_D30.txt
+-rw-r--r--  2.0 unx      141 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_4_D50.txt
+-rw-r--r--  2.0 unx       21 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_5_D10.txt
+-rw-r--r--  2.0 unx      292 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_5_D100.txt
+-rw-r--r--  2.0 unx       51 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_5_D20.txt
+-rw-r--r--  2.0 unx       81 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_5_D30.txt
+-rw-r--r--  2.0 unx      141 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_5_D50.txt
+-rw-r--r--  2.0 unx       21 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_6_D10.txt
+-rw-r--r--  2.0 unx      292 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_6_D100.txt
+-rw-r--r--  2.0 unx       51 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_6_D20.txt
+-rw-r--r--  2.0 unx       81 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_6_D30.txt
+-rw-r--r--  2.0 unx      141 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_6_D50.txt
+-rw-r--r--  2.0 unx       21 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_7_D10.txt
+-rw-r--r--  2.0 unx      292 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_7_D100.txt
+-rw-r--r--  2.0 unx       51 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_7_D20.txt
+-rw-r--r--  2.0 unx       81 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_7_D30.txt
+-rw-r--r--  2.0 unx      141 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_7_D50.txt
+-rw-r--r--  2.0 unx       21 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_8_D10.txt
+-rw-r--r--  2.0 unx      292 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_8_D100.txt
+-rw-r--r--  2.0 unx       51 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_8_D20.txt
+-rw-r--r--  2.0 unx       81 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_8_D30.txt
+-rw-r--r--  2.0 unx      141 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_8_D50.txt
+-rw-r--r--  2.0 unx       21 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_9_D10.txt
+-rw-r--r--  2.0 unx      292 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_9_D100.txt
+-rw-r--r--  2.0 unx       51 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_9_D20.txt
+-rw-r--r--  2.0 unx       81 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_9_D30.txt
+-rw-r--r--  2.0 unx      141 b- defN 22-Nov-08 19:54 indago/benchmarks/cec2014_data/shuffle_data_9_D50.txt
+-rw-r--r--  2.0 unx     1513 b- defN 23-Jul-21 13:48 Indago-0.4.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-21 13:48 Indago-0.4.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 23-Jul-21 13:48 Indago-0.4.6.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx    39265 b- defN 23-Jul-21 13:49 Indago-0.4.6.dist-info/RECORD
+381 files, 36087431 bytes uncompressed, 2981546 bytes compressed:  91.7%
```

## zipnote {}

```diff
@@ -45,20 +45,1100 @@
 
 Filename: indago/benchmarks/_cec.py
 Comment: 
 
 Filename: indago/benchmarks/_shortest_path.py
 Comment: 
 
-Filename: Indago-0.4.5.dist-info/METADATA
+Filename: indago/benchmarks/cec2014_data/M_10_D10.txt
 Comment: 
 
-Filename: Indago-0.4.5.dist-info/WHEEL
+Filename: indago/benchmarks/cec2014_data/M_10_D100.txt
 Comment: 
 
-Filename: Indago-0.4.5.dist-info/top_level.txt
+Filename: indago/benchmarks/cec2014_data/M_10_D2.txt
 Comment: 
 
-Filename: Indago-0.4.5.dist-info/RECORD
+Filename: indago/benchmarks/cec2014_data/M_10_D20.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_10_D30.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_10_D50.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_11_D10.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_11_D100.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_11_D2.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_11_D20.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_11_D30.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_11_D50.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_12_D10.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_12_D100.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_12_D2.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_12_D20.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_12_D30.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_12_D50.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_13_D10.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_13_D100.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_13_D2.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_13_D20.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_13_D30.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_13_D50.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_14_D10.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_14_D100.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_14_D2.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_14_D20.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_14_D30.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_14_D50.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_15_D10.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_15_D100.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_15_D2.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_15_D20.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_15_D30.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_15_D50.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_16_D10.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_16_D100.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_16_D2.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_16_D20.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_16_D30.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_16_D50.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_17_D10.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_17_D100.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_17_D2.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_17_D20.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_17_D30.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_17_D50.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_18_D10.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_18_D100.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_18_D2.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_18_D20.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_18_D30.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_18_D50.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_19_D10.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_19_D100.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_19_D2.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_19_D20.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_19_D30.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_19_D50.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_1_D10.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_1_D100.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_1_D2.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_1_D20.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_1_D30.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_1_D50.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_20_D10.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_20_D100.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_20_D2.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_20_D20.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_20_D30.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_20_D50.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_21_D10.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_21_D100.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_21_D2.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_21_D20.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_21_D30.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_21_D50.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_22_D10.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_22_D100.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_22_D2.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_22_D20.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_22_D30.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_22_D50.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_23_D10.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_23_D100.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_23_D2.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_23_D20.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_23_D30.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_23_D50.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_24_D10.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_24_D100.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_24_D2.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_24_D20.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_24_D30.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_24_D50.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_25_D10.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_25_D100.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_25_D2.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_25_D20.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_25_D30.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_25_D50.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_26_D10.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_26_D100.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_26_D2.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_26_D20.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_26_D30.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_26_D50.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_27_D10.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_27_D100.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_27_D2.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_27_D20.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_27_D30.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_27_D50.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_28_D10.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_28_D100.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_28_D2.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_28_D20.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_28_D30.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_28_D50.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_29_D10.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_29_D100.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_29_D2.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_29_D20.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_29_D30.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_29_D50.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_2_D10.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_2_D100.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_2_D2.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_2_D20.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_2_D30.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_2_D50.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_30_D10.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_30_D100.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_30_D2.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_30_D20.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_30_D30.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_30_D50.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_3_D10.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_3_D100.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_3_D2.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_3_D20.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_3_D30.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_3_D50.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_4_D10.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_4_D100.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_4_D2.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_4_D20.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_4_D30.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_4_D50.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_5_D10.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_5_D100.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_5_D2.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_5_D20.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_5_D30.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_5_D50.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_6_D10.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_6_D100.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_6_D2.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_6_D20.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_6_D30.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_6_D50.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_7_D10.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_7_D100.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_7_D2.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_7_D20.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_7_D30.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_7_D50.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_8_D10.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_8_D100.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_8_D2.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_8_D20.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_8_D30.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_8_D50.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_9_D10.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_9_D100.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_9_D2.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_9_D20.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_9_D30.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/M_9_D50.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shift_data_1.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shift_data_10.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shift_data_11.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shift_data_12.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shift_data_13.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shift_data_14.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shift_data_15.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shift_data_16.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shift_data_17.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shift_data_18.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shift_data_19.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shift_data_2.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shift_data_20.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shift_data_21.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shift_data_22.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shift_data_23.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shift_data_24.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shift_data_25.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shift_data_26.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shift_data_27.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shift_data_28.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shift_data_29.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shift_data_3.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shift_data_30.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shift_data_4.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shift_data_5.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shift_data_6.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shift_data_7.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shift_data_8.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shift_data_9.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_10_D10.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_10_D100.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_10_D20.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_10_D30.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_10_D50.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_11_D10.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_11_D100.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_11_D20.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_11_D30.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_11_D50.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_12_D10.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_12_D100.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_12_D20.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_12_D30.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_12_D50.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_13_D10.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_13_D100.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_13_D20.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_13_D30.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_13_D50.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_14_D10.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_14_D100.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_14_D20.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_14_D30.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_14_D50.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_15_D10.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_15_D100.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_15_D20.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_15_D30.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_15_D50.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_16_D10.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_16_D100.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_16_D20.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_16_D30.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_16_D50.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_17_D10.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_17_D100.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_17_D20.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_17_D30.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_17_D50.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_18_D10.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_18_D100.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_18_D20.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_18_D30.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_18_D50.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_19_D10.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_19_D100.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_19_D20.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_19_D30.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_19_D50.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_1_D10.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_1_D100.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_1_D20.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_1_D30.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_1_D50.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_20_D10.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_20_D100.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_20_D20.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_20_D30.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_20_D50.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_21_D10.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_21_D100.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_21_D20.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_21_D30.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_21_D50.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_22_D10.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_22_D100.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_22_D20.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_22_D30.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_22_D50.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_23_D10.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_23_D100.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_23_D20.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_23_D30.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_23_D50.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_24_D10.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_24_D100.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_24_D20.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_24_D30.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_24_D50.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_25_D10.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_25_D100.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_25_D20.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_25_D30.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_25_D50.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_26_D10.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_26_D100.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_26_D20.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_26_D30.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_26_D50.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_27_D10.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_27_D100.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_27_D20.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_27_D30.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_27_D50.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_28_D10.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_28_D100.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_28_D20.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_28_D30.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_28_D50.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_29_D10.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_29_D100.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_29_D20.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_29_D30.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_29_D50.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_2_D10.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_2_D100.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_2_D20.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_2_D30.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_2_D50.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_30_D10.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_30_D100.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_30_D20.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_30_D30.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_30_D50.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_3_D10.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_3_D100.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_3_D20.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_3_D30.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_3_D50.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_4_D10.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_4_D100.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_4_D20.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_4_D30.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_4_D50.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_5_D10.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_5_D100.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_5_D20.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_5_D30.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_5_D50.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_6_D10.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_6_D100.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_6_D20.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_6_D30.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_6_D50.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_7_D10.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_7_D100.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_7_D20.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_7_D30.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_7_D50.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_8_D10.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_8_D100.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_8_D20.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_8_D30.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_8_D50.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_9_D10.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_9_D100.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_9_D20.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_9_D30.txt
+Comment: 
+
+Filename: indago/benchmarks/cec2014_data/shuffle_data_9_D50.txt
+Comment: 
+
+Filename: Indago-0.4.6.dist-info/METADATA
+Comment: 
+
+Filename: Indago-0.4.6.dist-info/WHEEL
+Comment: 
+
+Filename: Indago-0.4.6.dist-info/top_level.txt
+Comment: 
+
+Filename: Indago-0.4.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## indago/__init__.py

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 
 
-__version__ = '0.4.5'
+__version__ = '0.4.6'
 
 from indago._optimizer import Optimizer, CandidateState
 from indago._utility import minimize, minimize_exhaustive, inspect, inspect_optimizers
 
 from indago._pso import PSO
 from indago._fwa import FWA
 from indago._ssa import SSA
```

## indago/_abc.py

```diff
@@ -2,26 +2,15 @@
 """ARTIFICIAL BEE COLONY ALGORITHM"""
 
 
 import numpy as np
 from ._optimizer import Optimizer, CandidateState 
 
 
-class Bee(CandidateState):
-    """ABC agent class.
-         
-    Returns
-    -------
-    agent : Bee
-        Bee instance.
-    """
-    
-    def __init__(self, optimizer: Optimizer):
-        CandidateState.__init__(self, optimizer)
-        #self.trials = 0#np.zeros([optimizer.dimensions], dtype=np.int32) #* np.nan
+Bee = CandidateState
 
 
 class ABC(Optimizer):
     """Artificial Bee Colony Algorithm class method class.
     
     Attributes
     ----------
@@ -94,23 +83,23 @@
         self.cS = np.array([Bee(self) for c in range(self.params['pop_size'])], dtype=Bee)
         self.cS_k = np.array([Bee(self) for c in range(self.params['pop_size'])], dtype=Bee)
 
         # Generate initial trial and probability vectors
         self.trials = np.zeros([self.params['pop_size']],dtype=np.int32)
         self.probability = np.zeros([self.params['pop_size']])
 
-        n0 = 0 if self._cs0 is None else self._cs0.size
+        n0 = 0 if self._cS0 is None else self._cS0.size
         for p in range(self.params['pop_size']):
             
             # Random position
             self.cS[p].X =  np.random.uniform(self.lb, self.ub)
 
             # Using specified particles initial positions
             if p < n0:
-                self.cS[p] = self._cs0[p].copy()
+                self.cS[p] = self._cS0[p].copy()
             
         # Evaluate
         if n0 < self.params['pop_size']:
             err_msg = self.collective_evaluation(self.cS[n0:])
         # err_msg = self.collective_evaluation(self.cS)
         # err_msg = self.collective_evaluation(self.cS_k)
         #self.cS_k = np.copy(self.cS)
@@ -148,18 +137,18 @@
             phi = np.random.uniform(-1,1)
             
             for i in range(self.dimensions):
                 if i != d: self.cS_k[p].X[i] = self.cS[p].X[i]
      
             self.cS_k[p].X[d] = self.cS[p].X[d] + phi*(self.cS[p].X[d] - self.cS[k].X[d])
             
-            cP.clip()
+            cP.clip(self)
                 
         for cP in self.cS:
-            cP.clip()
+            cP.clip(self)
 
         err_msg = self.collective_evaluation(self.cS_k)
         
         for p, cP in enumerate(self.cS_k):
             if self.cS_k[p] < self.cS[p]:
                 self.cS[p] = self.cS_k[p].copy()
                 self.trials[p] = 0
```

## indago/_ba.py

```diff
@@ -120,23 +120,23 @@
         self._evaluate_initial_candidates()
         err_msg = None
 
         # Generate a swarm
         self.cS = np.array([Bat(self) for c in range(self.params['pop_size'])], dtype=Bat)
 
         # Generate initial positions
-        n0 = 0 if self._cs0 is None else self._cs0.size
+        n0 = 0 if self._cS0 is None else self._cS0.size
         for p in range(self.params['pop_size']):
             
             # Random position
             self.cS[p].X = np.random.uniform(self.lb, self.ub)
             
             # Using specified particles initial positions
             if p < n0:
-                self.cS[p] = self._cs0[p].copy()
+                self.cS[p] = self._cS0[p].copy()
             
             # Generate velocity
             self.cS[p].V = 0.0
             
             # Frequency
             self.cS[p].Freq = np.random.uniform(self.params['freq_range'][0], self.params['freq_range'][1])
             
@@ -201,15 +201,15 @@
 
                 cP.V = cP.V + (cP.X - self.best.X)*cP.Freq
                 cP.X = cP.X + cP.V
                 
                 if np.random.uniform() > cP.r:
                     cP.X = self.best.X + 0.05*np.abs(self.lb - self.ub)*np.random.normal(size=self.dimensions)*A_avg
                                        
-                cP.clip()
+                cP.clip(self)
                
             #Evaluate swarm
             for p, cP in enumerate(self.cS):
                 # Update personal best
                 if cP <= self.cB[p] and np.random.uniform() < cP.A:
                     self.cB[p] = cP.copy()
                     cP.A = alpha*cP.A
```

## indago/_de.py

```diff
@@ -137,14 +137,18 @@
 
         Returns
         -------
         err_msg : str or None
             Error message (if any).
         """
 
+        if self.variant == 'LSHADE':
+            assert self.max_iterations or self.max_evaluations or self.max_elapsed_time, \
+                'optimizer.max_iteration, optimizer.max_evaluations, or self.max_elapsed_time should be provided for this method/variant'
+
         self._evaluate_initial_candidates()
         err_msg = None
 
         # Generate a population
         self.Pop = np.array([Solution(self) for c in \
                              range(self.params['pop_init'])], dtype=Solution)
         
@@ -156,23 +160,23 @@
         self.A = np.empty([0])
         
         # Prepare historical memory
         self.M_CR = np.full(self.params['hist_size'], 0.5)
         self.M_F = np.full(self.params['hist_size'], 0.5)
 
         # Generate initial positions
-        n0 = 0 if self._cs0 is None else self._cs0.size
+        n0 = 0 if self._cS0 is None else self._cS0.size
         for i in range(self.params['pop_init']):
             
             # Random position
             self.Pop[i].X = np.random.uniform(self.lb, self.ub)
             
             # Using specified particles initial positions
             if i < n0:
-                self.Pop[i] = self._cs0[i].copy()
+                self.Pop[i] = self._cS0[i].copy()
 
         # Evaluate
         if n0 < self.params['pop_init']:
             err_msg = self.collective_evaluation(self.Pop[n0:])
 
         # if all candidates are NaNs
         if np.isnan([p.f for p in self.Pop]).all():
```

## indago/_direct_search.py

```diff
@@ -90,27 +90,20 @@
         None
             Nothing
         """
 
         self._evaluate_initial_candidates()
         err_msg = None
         
-        # Prepare GaoHan parameters
-        if self.variant == 'GaoHan':
-            self.params['alpha'] = 1.0
-            self.params['gamma'] = 1 + 2 / self.dimensions
-            self.params['rho'] = 0.75 - 1 / 2 / self.dimensions
-            self.params['sigma'] = 1 - 1 / self.dimensions
-
         # Generate set of points
         self.cS = np.array([CandidateState(self) for _ in range(self.dimensions + 1)], \
                             dtype=CandidateState)
 
         # Generate initial positions
-        self.cS[0] = self._cs0[0].copy()
+        self.cS[0] = self._cS0[0].copy()
 
         for p in range(1, self.dimensions + 1):
 
             # Random position
             dx = np.zeros([self.dimensions])
             dx[p - 1] = self.params['init_step']
             self.cS[p].X = self.cS[0].X + dx * (self.ub - self.lb)
@@ -125,14 +118,26 @@
         Returns
         -------
         optimum: CandidateState
             Best solution found during the NelderMead optimization.
         """
         self._check_params()
         self._init_method()
+        
+        # Prepare parameters
+        if self.variant == 'Vanilla':
+            alpha = self.params['alpha']
+            gamma = self.params['gamma']
+            rho = self.params['rho']
+            sigma = self.params['sigma']
+        elif self.variant == 'GaoHan':
+            alpha = 1.0
+            gamma = 1 + 2 / self.dimensions
+            rho = 0.75 - 1 / 2 / self.dimensions
+            sigma = 1 - 1 / self.dimensions
 
         while True:
             self.cS = np.sort(self.cS)
             reduction = False
 
             self._progress_log()
 
@@ -145,71 +150,70 @@
             for p in range(self.dimensions):
                 X0 += self.cS[p].X
             X0 /= self.dimensions
 
             dX = X0 - self.cS[-1].X
 
             # Reflection
-            Xr = X0 + self.params['alpha'] * dX
+            Xr = X0 + alpha * dX
             Xr = np.clip(Xr, self.lb, self.ub)
             cR = CandidateState(self)
             cR.X = Xr
 
             self.collective_evaluation([cR])
 
             if self.cS[0] <= cR <= self.cS[-2]:
                 self.cS[-1] = cR.copy()
 
             elif cR < self.cS[0]:
                 # Expansion
-                Xe = X0 + self.params['gamma'] * dX
+                Xe = X0 + gamma * dX
                 Xe = np.clip(Xe, self.lb, self.ub)
                 cE = CandidateState(self)
                 cE.X = Xe
 
                 self.collective_evaluation([cE])
 
                 if cE < cR:
                     self.cS[-1] = cE.copy()
                 else:
                     self.cS[-1] = cR.copy()
 
             elif cR < self.cS[-1]:
                 # Contraction
-                Xc = X0 + self.params['rho'] * dX
+                Xc = X0 + rho * dX
                 Xc = np.clip(Xc, self.lb, self.ub)
                 cC = CandidateState(self)
                 cC.X = Xc
 
                 self.collective_evaluation([cC])
 
                 if cC < self.cS[-1]:
                     self.cS[-1] = cC.copy()
                 else:
                     reduction = True
 
             else:
                 # Internal contraction
-                Xc = X0 - self.params['rho'] * dX
+                Xc = X0 - rho * dX
                 Xc = np.clip(Xc, self.lb, self.ub)
                 cC = CandidateState(self)
                 cC.X = Xc
 
                 self.collective_evaluation([cC])
 
                 if cC < self.cS[-1]:
                     self.cS[-1] = cC.copy()
                 else:
                     reduction = True
 
-
             # Reduction
             if reduction:
                 for p in range(1, self.dimensions + 1):
-                    self.cS[p].X = self.cS[0].X + self.params['sigma'] * (self.cS[p].X - self.cS[0].X)
+                    self.cS[p].X = self.cS[0].X + sigma * (self.cS[p].X - self.cS[0].X)
                     # self.cS[p].evaluate()
                 self.collective_evaluation(self.cS[1:])
 
             if self._finalize_iteration():
                 break
 
         return self.best
@@ -227,34 +231,39 @@
     """
 
     def __init__(self):
         Optimizer.__init__(self)
         self.X0 = 1
         self.X = None
         self.variant = 'Vanilla'
-        self.params = {'n': 10, 'xtol': 1e-6}
+        self.params = {}
 
     def _check_params(self):
         """Private method which prepares the parameters to be validated by Optimizer._check_params.
         
         Returns
         -------
         None
             Nothing
         """
-
+        
         defined_params = list(self.params.keys())
         mandatory_params, optional_params = [], []
         
-        if 'n' in self.params:
+        if 'n' in defined_params:
             self.params['n'] = int(self.params['n'])
 
         if self.variant == 'Vanilla':
-            mandatory_params = ''.split()
-            optional_params = 'n xtol'.split()
+            mandatory_params = 'n xtol'.split()
+            if 'n' not in self.params:
+                self.params['n'] = 10
+                defined_params += 'n'.split()
+            if 'xtol' not in self.params:
+                self.params['xtol'] = 1e-6
+                defined_params += 'xtol'.split()
 
         else:
             assert False, f'Unknown variant! {self.variant}'
 
         for param in mandatory_params:
             # if param not in defined_params:
             #    print('Error: Missing parameter (%s)' % param)
@@ -277,15 +286,15 @@
             Nothing
         """
         
         self._evaluate_initial_candidates()
 
         self._n = self.params['n']
         self._I = np.arange(-self._n, self._n + 1)
-        self._x = self._cs0[0].copy()
+        self._x = self._cS0[0].copy()
 
         # The initial mesh always fills entire domain and initial point is snapped tzo the grid
         # self._center = 0.5 * (self.lb + self.ub)
         self._center = self._x.X
         self._X_map = [self._I for i in range(self.dimensions)]
         self._reinit_grid(self._center, 1, 'Initial grid')
         self._x = self._y_to_x(self._y)
@@ -485,15 +494,17 @@
         Returns
         -------
         optimum: CandidateState
             Best solution found during the MSGS optimization.
         """
         
         self._check_params()
-        self._init_method()
+        err_msg = self._init_method()
+        assert not err_msg, \
+            f'Error: {err_msg} OPTIMIZATION ABORTED'
 
         k, k_max = 0, 2
         d = self.dimensions
 
         scale = 1
         grid_action = 'none'
         action = 'find_dir_3p'
@@ -635,9 +646,13 @@
 
             else:
                 assert False, f'Unknown action {action=}'
 
             if self._finalize_iteration():
                 break
 
+        assert not err_msg, \
+            f'Error: {err_msg} OPTIMIZATION ABORTED'
+
         return self.best
 
+
```

## indago/_efo.py

```diff
@@ -2,26 +2,15 @@
 """Electromagnetic Field Optimization method"""
 
 import numpy as np
 from ._optimizer import Optimizer, CandidateState 
 from scipy.constants import golden_ratio as phi
 
 
-class emParticle(CandidateState):
-    """EFO emParticle class. An emParticle is a member of EFO population.
-         
-    Returns
-    -------
-    emp : emParticle
-        emParticle instance.
-    """
-    
-    def __init__(self, optimizer: Optimizer):
-        CandidateState.__init__(self, optimizer)
-
+emParticle = CandidateState
 
 class EFO(Optimizer):
     """Electromagnetic Field Optimization method class.
     
     Reference: Abedinpourshotorban, H., Shamsuddin, S.M., Beheshti, Z., & Jawawi, D.N. (2016). 
     Electromagnetic field optimization: a physics-inspired metaheuristic 
     optimization algorithm. Swarm and Evolutionary Computation, 26, 8-22.
@@ -110,23 +99,23 @@
         # Generate a population
         self.cS = np.array([emParticle(self) \
                             for _ in range(self.params['pop_size'])], 
                             dtype=emParticle)
         self.cNew = emParticle(self)
         
         # Initialize
-        n0 = 0 if self._cs0 is None else self._cs0.size
+        n0 = 0 if self._cS0 is None else self._cS0.size
         for i, p in enumerate(self.cS):
             
             # Random position
             self.cS[i].X = np.random.uniform(self.lb, self.ub)
             
             # Using specified particles initial positions
             if i < n0:
-                self.cS[i] = self._cs0[i].copy()
+                self.cS[i] = self._cS0[i].copy()
                     
         self.cNew.X = np.random.uniform(self.ub, self.lb)
         
         # Evaluate
         if n0 < self.cS.size:
             err_msg = self.collective_evaluation(self.cS[n0:])
         self.cS = np.sort(self.cS)
```

## indago/_fwa.py

```diff
@@ -91,23 +91,23 @@
 
         self._evaluate_initial_candidates()
         err_msg = None
 
         self.cX = np.array([CandidateState(self) for p in range(self.params['n'])])
         
         # Generate initial positions
-        n0 = 0 if self._cs0 is None else self._cs0.size
+        n0 = 0 if self._cS0 is None else self._cS0.size
         for p in range(self.params['n']):
             
             # Random position
             self.cX[p].X = np.random.uniform(self.lb, self.ub, self.dimensions)
             
             # Using specified initial positions
             if p < n0:
-                self.cX[p] = self._cs0[p].copy()
+                self.cX[p] = self._cS0[p].copy()
 
         # Evaluate all
         if n0 < self.params['n']:
             err_msg = self.collective_evaluation(self.cX[n0:])
 
         # if all candidates are NaNs       
         if np.isnan([p.f for p in self.cX]).all():
@@ -139,25 +139,26 @@
         n = self.params['n']
 
         while True:
 
             explosion_sparks = self._explosion()
             mutation_sparks = self._gaussian_mutation()
 
+            # self.cX = np.array([], dtype=CandidateState)
             #self.__mapping_rule(sparks, self.lb, self.ub, self.dimensions)
             for cS in (explosion_sparks + mutation_sparks):
                 
                 ilb = cS.X < self.lb
                 cS.X[ilb] = self.lb[ilb]
                 iub = cS.X > self.ub
                 cS.X[iub] = self.ub[iub]
 
                 self.cX = np.append(self.cX, [cS])
 
-            err_msg = self.collective_evaluation(self.cX)
+            err_msg = self.collective_evaluation(self.cX[n:])
             if err_msg:
                 break
 
             self.cX = np.sort(self.cX)[:n]
 
             if self._finalize_iteration():
                 break
```

## indago/_mmo.py

```diff
@@ -325,14 +325,15 @@
                 # Using specified initial positions
                 if self.X0:
                     if p < np.shape(self.X0)[0]:
                         self.cX[p].X = self.X0[p]
     
             # Evaluate all
             err_msg = self.collective_evaluation(self.cX)
+            
             # if all candidates are NaNs       
             if np.isnan([p.f for p in self.cX]).all():
                 err_msg = 'ALL CANDIDATES FAILED TO EVALUATE.'
             if err_msg:
                 return err_msg
     
             # Sort
@@ -353,23 +354,23 @@
             self.A = np.empty([0])
             
             # Prepare historical memory
             self.M_CR = np.full(self.params['hist_size'], 0.5)
             self.M_F = np.full(self.params['hist_size'], 0.5)
     
             # Generate initial positions
-            n0 = 0 if self._cs0 is None else self._cs0.size
+            n0 = 0 if self._cS0 is None else self._cS0.size
             for i in range(self.params['pop_init']):
                 
                 # Random position
                 self.Pop[i].X = np.random.uniform(self.lb, self.ub)
                 
                 # Using specified particles initial positions
                 if i < n0:
-                    self.Pop[i] = self._cs0[i].copy()
+                    self.Pop[i] = self._cS0[i].copy()
 
             # Evaluate
             err_msg = self.collective_evaluation(self.Pop)
             
             # if all candidates are NaNs       
             if np.isnan([p.f for p in self.Pop]).all():
                 err_msg = 'ALL CANDIDATES FAILED TO EVALUATE.'
@@ -384,23 +385,23 @@
             self.ABC_cS_k = np.array([Bee(self) for c in range(self.params['pop_size'])], dtype=Bee)
 
             # Generate initial trial and probability vectors
 
             self.trials = np.zeros([self.params['pop_size']],dtype=np.int_)
             self.probability = np.zeros([self.params['pop_size']])
             
-            n0 = 0 if self._cs0 is None else self._cs0.size
+            n0 = 0 if self._cS0 is None else self._cS0.size
             for p in range(self.params['pop_size']):
                 
                 # Random position
                 self.ABC_cS[p].X =  np.random.uniform(self.lb, self.ub)
 
                 # Using specified particles initial positions
                 if p < n0:
-                    self.ABC_cS[p] = self._cs0[p].copy()
+                    self.ABC_cS[p] = self._cS0[p].copy()
                 
             # Evaluate
             if n0 < self.params['pop_size']:
                 err_msg = self.collective_evaluation(self.ABC_cS[n0:])
             # err_msg = self.collective_evaluation(self.ABC_cS)
             # err_msg = self.collective_evaluation(self.ABC_cS_k)
             #self.ABC_cS_k = np.copy(self.ABC_cS)
@@ -566,18 +567,18 @@
             phi = np.random.uniform(-1,1)
             
             for i in range(self.dimensions):
                 if i != d: self.ABC_cS_k[p].X[i] = self.ABC_cS[p].X[i]
      
             self.ABC_cS_k[p].X[d] = self.ABC_cS[p].X[d] + phi*(self.ABC_cS[p].X[d] - self.ABC_cS[k].X[d])
             
-            cP.clip()
+            cP.clip(self)
                 
         for cP in self.ABC_cS:
-            cP.clip()
+            cP.clip(self)
 
         err_msg = self.collective_evaluation(self.ABC_cS_k)
         
         for p, cP in enumerate(self.ABC_cS_k):
             if self.ABC_cS_k[p] < self.ABC_cS[p]:
                 self.ABC_cS[p] = self.ABC_cS_k[p].copy()
                 self.trials[p] = 0
@@ -637,41 +638,40 @@
                 if self.params['inertia'] == 'LDIW':
                     w = 1.0 - (1.0 - 0.4) * self._progress_factor()
     
                 if self.methods['PSO'] == 'TVAC':
                     c1 = 2.5 - (2.5 - 0.5) * self._progress_factor()
                     c2 = 0.5 + (2.5 - 0.5) * self._progress_factor()
     
-                if self.params['inertia'] == 'anakatabatic':
-    
+                if self.params['inertia'] == 'anakatabatic':  
                     theta = np.arctan2(self.dF, np.min(self.dF))
                     theta[theta < 0] = theta[theta < 0] + 2 * np.pi  # 3rd quadrant
                     # fix for atan2(0,0)=0
                     theta0 = theta < 1e-300
                     theta[theta0] = np.pi / 4 + \
                         np.random.rand(np.sum(theta0)) * np.pi
                     w_start = self.params['akb_fun_start'](theta)
                     w_stop = self.params['akb_fun_stop'](theta)
                     #print(w_start)
                     w = w_start * (1 - self._progress_factor()) \
                         + w_stop * self._progress_factor()
-                
+
                 w = w * np.ones(self.params['swarm_size']) # ensure w is a vector
                 
                 # Calculate new velocity and new position
                 
                 for p, cP in enumerate(self.cS):
     
                     cP.V = w[p] * cP.V + \
                                    c1 * R1[p, :] * (self.cB[p].X - cP.X) + \
                                    c2 * R2[p, :] * (self.cB[self.BI[p]].X - cP.X)
                     cP.X = cP.X + cP.V        
                     
                     # Correct position to the bounds
-                    cP.clip()    
+                    cP.clip(self)
                     
                 # Get old fitness
                 f_old = np.array([cP.f for cP in self.cS])
     
                 # Evaluate swarm
                 err_msg = self.collective_evaluation(self.cS)
                 if err_msg:
@@ -707,15 +707,15 @@
                     ilb = cS.X < self.lb
                     cS.X[ilb] = self.lb[ilb]
                     iub = cS.X > self.ub
                     cS.X[iub] = self.ub[iub]
     
                     self.cX = np.append(self.cX, [cS])
     
-                err_msg = self.collective_evaluation(self.cX)
+                err_msg = self.collective_evaluation(self.cX[n:])
                 if err_msg:
                     break
     
                 self.cX = np.sort(self.cX)[:n]
             
             """ DE iteration """
             if 'DE' in self.methods:
@@ -778,20 +778,20 @@
                         S_df = np.append(S_df, p.f - t.f)
                         # Update population
                         p.X = np.copy(t.X)
                         p.f = t.f
     
                 # Memory update
                 if np.size(S_CR) != 0 and np.size(S_F) != 0:
-                    w = S_df / np.sum(S_df)
+                    w_DE = S_df / np.sum(S_df)
                     if np.isnan(self.M_CR[K]) or np.max(S_CR) < 1e-100:
                         self.M_CR[K] = np.nan
                     else:
-                        self.M_CR[K] = np.sum(w * S_CR**2) / np.sum(w * S_CR)
-                    self.M_F[K] = np.sum(w * S_F**2) / np.sum(w * S_F)
+                        self.M_CR[K] = np.sum(w_DE * S_CR**2) / np.sum(w_DE * S_CR)
+                    self.M_F[K] = np.sum(w_DE * S_F**2) / np.sum(w_DE * S_F)
                     K += 1
                     if K >= self.params['hist_size']:
                         K = 0
                         
                 # Linear Population Size Reduction (LPSR)
                 if self.methods == 'LSHADE':
                     N_init = self.params['pop_init']
```

## indago/_mrfo.py

```diff
@@ -66,31 +66,33 @@
         Initializes and evaluates the swarm.
 
         Returns
         -------
         err_msg : str or None
             Error message (if any).
         """
+        assert self.max_iterations or self.max_evaluations or self.max_elapsed_time, \
+            'optimizer.max_iteration, optimizer.max_evaluations, or self.max_elapsed_time should be provided for this method/variant'
 
         self._evaluate_initial_candidates()
         err_msg = None
 
         # Generate a swarm
         self.cS = np.array([CandidateState(self) for c in range(self.params['pop_size'])], dtype=CandidateState)
         
         # Generate initial positions
-        n0 = 0 if self._cs0 is None else self._cs0.size
+        n0 = 0 if self._cS0 is None else self._cS0.size
         for p in range(self.params['pop_size']):
             
             # Random position
             self.cS[p].X = np.random.uniform(self.lb, self.ub)
             
             # Using specified particles initial positions
             if p < n0:
-                self.cS[p] = self._cs0[p].copy()
+                self.cS[p] = self._cS0[p].copy()
 
         # Evaluate
         if n0 < self.params['pop_size']:
             err_msg = self.collective_evaluation(self.cS[n0:])
         # if all candidates are NaNs       
         if np.isnan([cP.f for cP in self.cS]).all():
             err_msg = 'ALL CANDIDATES FAILED TO EVALUATE.'
@@ -142,28 +144,28 @@
                 r = np.random.uniform(size=self.dimensions)
                 alpha = 2*r*np.sqrt(np.abs(np.log(r)))
                 self.cS[0].X = X_[0].X + r*(self.best.X - X_[0].X) + alpha*(self.best.X - X_[0].X)
                 for p in range(1, len(self.cS)):
                     self.cS[p].X = X_[p].X + r*(self.cS[p-1].X - X_[p].X) + alpha*(self.best.X - X_[p].X)
             
             for cP in self.cS:                              
-                cP.clip()
+                cP.clip(self)
             
             err_msg = self.collective_evaluation(self.cS)
             if err_msg:
                 break
                                
             # SOMERSAULT FORAGING        
             r2 = np.random.uniform(size=self.dimensions)
             r3 = np.random.uniform(size=self.dimensions)
             for p, p_ in zip(self.cS, X_):
                 p.X = p_.X + self.params['f_som']*(r2*self.best.X - r3*p_.X)
             
             for cP in self.cS:                              
-                cP.clip()
+                cP.clip(self)
                 
             err_msg = self.collective_evaluation(self.cS)
             if err_msg:
                 break
             
             if self._finalize_iteration():
                 break
```

## indago/_optimizer.py

```diff
@@ -1,8 +1,9 @@
 # -*- coding: utf-8 -*-
+import copy
 import os.path
 
 import numpy as np
 import matplotlib.pyplot as plt
 from datetime import datetime
 import time
 import multiprocessing
@@ -70,15 +71,15 @@
     best : CandidateState
         The best candidate state insofar encountered in the optimization process.
     X0 : ndarray or int
         Starting point(s) for the optimization. 1d ndarray, or 2d ndarray with each row representing one design vector.
         If int, represents the number of random candidates generated at the start of optimization. 
         Each method embeds these candidates, fully or partially, in initial population, swarm or starting points. 
         Initial candidates are selected in order of their fitness. 
-    _cs0 : ndarray
+    _cS0 : ndarray
         A private array of CandidateState instances populated and evaluated according to given Optimizer.X0 parameter.
         The array is adopted in each method for establishing initial population, swarm or starting point.
     _evaluated_candidates : ndarray of CandidateState
         A private array used as a buffer of evaluated candidates in current iteration. Enables forwarding a list of all
         evaluated candidates in an interation to be forwarded to post_iteration_processing function even if multiple
         collective evaluations are utilized in a single iteration of a method.
     history : dictionary
@@ -170,15 +171,15 @@
         self.target_fitness = None
         self.max_elapsed_time = None
         
         self.lb = None
         self.ub = None
         self.best = None
         self.X0 = None
-        self._cs0 = None
+        self._cS0 = None
         self._evaluated_candidates = np.array([], dtype=CandidateState)
 
         self.history = None
         self.monitoring = None
         self._progress_log = None
         self.convergence_log_file = None
 
@@ -533,16 +534,16 @@
                         'O': np.full([0, self.objectives], np.zeros(self.objectives)),
                         'C': np.full([0, self.constraints], np.zeros(self.constraints)),
                         'f': np.full([0, 1], 0),
                         }
         self._init_convergence_log()
 
     def _evaluate_initial_candidates(self):
-        """Private method for evaluating initial canidates.
-        TODO
+        """Private method for evaluating initial canidates. This method populates and evaluates private list of initial
+        candidates (Optimizer._cS0) according to provided initial points Optimizer.X0.
 
         Returns
         -------
         None
             Nothing
         """
         
@@ -551,36 +552,36 @@
                 "optimizer.X0 should be 1d or 2d np.array, or integer"
             if isinstance(self.X0, np.ndarray):
                 assert self.X0.ndim == 1 or self.X0.ndim == 2, \
                     "optimizer.X0 should be 1d or 2d np.array"
                 # if 1D convert to 2D
                 if self.X0.ndim == 1:
                     self.X0 = np.array([self.X0])
-                self._cs0 = np.array([CandidateState(optimizer=self) for i in range(self.X0.shape[0])])
-                for i, cs in enumerate(self._cs0):
+                self._cS0 = np.array([CandidateState(optimizer=self) for i in range(self.X0.shape[0])])
+                for i, cs in enumerate(self._cS0):
                     cs.X = self.X0[i, :]
 
             if isinstance(self.X0, int):
                 assert self.X0 > 0, \
                     "optimizer.X0 should be a positive integer"
                 n = self.X0
-                self._cs0 = np.array([CandidateState(optimizer=self) for i in range(n)])
-                for cs in self._cs0:
+                self._cS0 = np.array([CandidateState(optimizer=self) for i in range(n)])
+                for cs in self._cS0:
                     cs.X = np.random.uniform(self.lb, self.ub, self.dimensions)
-            self.log(f'Evaluating {self._cs0.size} initial candidates...')
-            self.collective_evaluation(self._cs0)
-            self._cs0 = np.sort(self._cs0)
+            self.log(f'Evaluating {self._cS0.size} initial candidates...')
+            self.collective_evaluation(self._cS0)
+            self._cS0 = np.sort(self._cS0)
 
-            self.log(', '.join([f'{cs.f}' for cs in self._cs0]))
+            self.log(', '.join([f'{cs.f}' for cs in self._cS0]))
         else:
             self.best = None
 
     def _init_convergence_log(self):
-        """Private method for initializing convergence log.
-        TODO
+        """Private method for initializing convergence log. It creates log file and writes optimization setup summary
+        and header row.
 
         Returns
         -------
         None
             Nothing
         """
         
@@ -666,15 +667,15 @@
                 f'Warning: Excessive parameter {param}'
 
     def __str__(self):
         """Method for a useful printout of optimizer properties. 
         
         Returns
         -------
-        printout : str - TODO check
+        printout : str
             String of the fancy table of optimizer properties.
         """
         
         table = Table(title=f'Indago {type(self).__name__} Optimizer')
 
         table.add_column('Property', justify='left', style='magenta')
         table.add_column('Value', justify='left', style='cyan')
@@ -721,15 +722,15 @@
             print(' ' * indent + msg)
         if self.convergence_log_file:
             log_file = open(self.convergence_log_file, 'a')
             log_file.write(f'#  {msg}\n')
             log_file.close()
 
     def __progress_log_basic(self):
-        """TODO
+        """A private function used to produce and print a line for each iteration.
         
         Returns
         -------
         None
             Nothing
         """
         
@@ -747,15 +748,15 @@
             else:
                 line += f', {cl}: [green bold]{cv}[/green bold]'
         line += f', fit: [magenta bold]{self.best.f}[/magenta bold]'
         self.rich_console.print(line)
         #self.log(line)
 
     def __convergence_log_line(self):
-        """TODO
+        """A private function used to produce and write a line to convergence log file for each iteration.
         
         Returns
         -------
         None
             Nothing
         """
         
@@ -790,23 +791,23 @@
         
         while True:
             _s = ''.join(np.random.choice([c for c in string.ascii_lowercase]) for _ in range(16))
             if _s not in self._unique_str_list:
                 self._unique_str_list.append(_s)
                 return _s
 
-    def optimize(self, hotstart=False, seed=None):
+    def optimize(self, resume=False, seed=None):
         """Method which starts the optimization. The method wraps ``_run`` method 
         of the optimizer's subclass.
 
         Parameters
         ----------
-        hotstart : bool
+        resume : bool
             If True, the user is intentionally running an optimizer instance which was run earlier.
-            Otherwise error is thrown when trying to re-run an optimizer instance.
+            Otherwise, error is thrown when trying to re-run an optimizer instance.
 
         seed : int or None
             A random seed. Use the same value for reproducing identical stochastic procedures.
 
         Returns
         -------
         optimum : CandidateState
@@ -842,41 +843,42 @@
         """A private method used to evaluate all specified stopping conditions.
 
         Returns
         -------
         stop : bool
             ``True`` or ``False``, whether the optimization should stop.
         """
-        
+        stop = False
+
         # Stop if maximum number of iterations reached
         if self.max_iterations:
             if self.it > self.max_iterations:
                 self.log(f'Maximum number of iterations reached ({self.max_iterations})')
-                return True
+                stop = True
             
         # Stop if maximum number of evaluations surpassed
         if self.max_evaluations:
             if self.eval > self.max_evaluations:
                 self.log(f'Maximum number of evaluations reached ({self.eval})')
-                return True
+                stop = True
 
         # Stop if fitness threshold achieved
         if self.target_fitness:
             if self.best.f < self.target_fitness and np.all(self.best.C <= 0):
                 self.log(f'Target fitness achieved {self.best.f} < {self.target_fitness}')
-                return True
+                stop = True
 
         # Stop if maximum number of stalled iterations surpassed
         if self.max_stalled_iterations:
             f_hist = self.history['f'].flatten()
             # f_hist = np.array([r[2].f for r in self.results.cHistory])
             self._stalled_it = np.size(np.where(f_hist == f_hist[-1])) - 1
             if self._stalled_it > self.max_stalled_iterations:
                 self.log(f'Stalled for the last {self._stalled_it} iterations, optimization stopped')
-                return True
+                stop = True
             
         # Stop if maximum number of stalled evaluations surpassed
         if self.max_stalled_evaluations:
             f_hist = self.history['f'].flatten()
             # f_hist = np.array([r[2].f for r in self.results.cHistory])
             stalled_it = np.size(np.where(f_hist == f_hist[-1])) - 1
             # print(f'{stalled_it=}, {self.it=}')
@@ -885,24 +887,27 @@
             else:
                 self._stalled_eval = self.eval - self.history['eval'][-stalled_it - 1][0]
             # print(f'new: {self.stalled_eval=}')
             # self.stalled_eval = self.eval - self.results.cHistory[-stalled_it][1]
             # print(f'old: {self.stalled_eval=}')
             if self._stalled_eval > self.max_stalled_evaluations:
                 self.log(f'Stalled for the last {self._stalled_eval} evaluations, optimization stopped')
-                return True
+                stop = True
         
         # Stop if maximum elapsed time reached
         if self.max_elapsed_time:
             if self.elapsed_time > self.max_elapsed_time:
                 self.log(f'Maximum elapsed time reached ({self.max_elapsed_time} s)')
-                return True
-            
+                stop = True
+
+        if self.monitoring == 'dashboard':
+            self.live.update(self.__update_progress_bar())
+
         # No criteria satisfied
-        return False
+        return stop
 
     def _finalize_iteration(self):
         """A private method used to perform all administrative tasks at the end of a method's iteration.
     
         Returns
         -------
         stop : bool
@@ -917,23 +922,27 @@
         # Post iterational processing
         if self.post_iteration_processing:
             _candidates = np.sort(self._evaluated_candidates)
             self.post_iteration_processing(self.it, _candidates, self.best)
 
         # Flushing evaluated candidates
         self._evaluated_candidates = np.array([], dtype=CandidateState)
-        
-        # Counting iterations
-        self.it += 1
+
         
         # Tracking time
         self.elapsed_time = time.time() - self._clock_start
-        
+
         # Checking stopping criteria
-        return self._stopping_criteria()
+        if self._stopping_criteria():
+            return True
+        else:
+            # Counting iterations
+            self.it += 1
+            return False
+
     
     """
     # These two functions were added to fix some multiprocessing-related problems on HPC.
     # Since then, a cleaner fix for this kind of problems was implemented (commit bb5d22cd).
     # These two are now commented out, hopefully they will not be missed by anyone. :)
     
     def __getstate__(self):
@@ -1069,20 +1078,39 @@
         self.eval += n
 
         if self.number_of_processes > 1:
             err_msg = self._multiprocess_evaluate(candidates)
         
         else:
             for p in range(n):
+
                 if self.forward_unique_str:
                     candidates[p].unique_str = self._gen_unique_str()
-                    candidates[p].evaluate(candidates[p].unique_str)
+                    result = self._evaluation_function_safe(candidates[p].X, candidates[p].unique_str)
                 else:
-                    candidates[p].evaluate()
+                    result = self._evaluation_function_safe(candidates[p].X)
 
+                if self.objectives == 1 and self.constraints == 0:
+                    # Fast evaluation
+                    candidates[p].f = result
+                    candidates[p].O[0] = result
+                else:
+                    # Full evaluation
+                    for io in range(self.objectives):
+                        candidates[p].O[io] = result[io]
+                    candidates[p].f = np.dot(candidates[p].O, self.objective_weights)
+                    for ic in range(self.constraints):
+                        candidates[p].C[ic] = result[self.objectives + ic]
+
+                # if self.forward_unique_str:
+                #     candidates[p].unique_str = self._gen_unique_str()
+                #     candidates[p].evaluate(candidates[p].unique_str)
+                # else:
+                #     # candidates[p].evaluate()
+                #     self.evaluation_function(candidates[p])
                 # if failed evaluation
                 if np.isnan(candidates[p].f):
                     self.eval_fail_count += 1
 
                     if self.eval_fail_behavior == 'ignore':
                         # report to log evaluation failed
                         if self.monitoring == 'basic':
@@ -1144,15 +1172,15 @@
             self.live.update(self.__update_progress_bar())
         
         # return error message if any
         if err_msg:
             return err_msg
 
     def _update_history(self):
-        """TODO
+        """Private method that updates Optimizer.history dictionary entries according to current Optimizer.best CandidateState
 
         Returns
         -------
         None
             Nothing
         """
 
@@ -1166,19 +1194,20 @@
             self.history['eval'][-1] = self.eval
             self.history['X'][-1] = self.best.X
             self.history['O'][-1] = self.best.O
             self.history['C'][-1] = self.best.C
             self.history['f'][-1] = self.best.f
 
     def plot_history(self, axes=None):
-        """Plot convergence. TODO
+        """Plot the convergence of optimization variables, objectives, constraints and fitness.
 
         Parameters
         ----------
-        axes : TODO
+        axes : list of matplotlib.axes
+            A list of four axes objects for plotting optimization variables, objectives, constraints and fitness, respectively.
 
         Returns
         -------
         None
             Nothing
         """
 
@@ -1219,14 +1248,15 @@
                 C = self.history['C'][:, i]
                 ax_c.plot(E, C, lw=1, label=self.constraint_labels[i])
                 I = C > 0
                 ax_c.plot(E[I], C[I], 'r.')
             c_lim = ax_c.get_ylim()[0], ax_c.get_ylim()[1]
             ax_c.fill_between(E[:i_feasible], ax_c.get_ylim()[0], ax_c.get_ylim()[1],
                               color='red', alpha=0.2)
+            ax_c.plot([], [], 'r.', label='Violated constraint')
             ax_c.axhline(0, c='r', lw=1)
             ax_c.set_ylim(c_lim)
             ax_c.set_ylabel('Constraints')
             ax_c.legend()
 
         # Plot fitness
         if ax_f:
@@ -1265,69 +1295,71 @@
     Returns
     -------
     CandidateState
         CandidateState instance.
     """
     
     def __init__(self, optimizer: Optimizer):        
-        self._optimizer = optimizer
+        # self._optimizer = optimizer
         self.X = np.zeros(optimizer.dimensions) * np.nan
         self.O = np.zeros(optimizer.objectives) * np.nan
         self.C = np.zeros(optimizer.constraints) * np.nan
         self.f = np.nan
                     
         # Evaluation
-        if self._optimizer.objectives == 1 and self._optimizer.constraints == 0:
+        if optimizer.objectives == 1 and optimizer.constraints == 0:
             self._evaluate = self._eval_fast
         else:
             self._evaluate = self._eval_full
         
         # Comparison operators
-        if self._optimizer.objectives == 1 and self._optimizer.constraints == 0:
+        if optimizer.objectives == 1 and optimizer.constraints == 0:
             self._eq_fn = self._eq_fast
             self._lt_fn = self._lt_fast 
             #self.__gt__ = self._gt_fast
         else:
             self._eq_fn = self._eq_full
             self._lt_fn = self._lt_full 
             #self.__gt__ = self._gt_full
 
-        if self._optimizer.forward_unique_str:
-            self.unique_str = None
+        # if optimizer.forward_unique_str:
+        self.unique_str = None
             
-    def clip(self):
+    def clip(self, optimizer):
         """Method for clipping (trimming) the design vector (CandidateState.X) 
         values to lower and upper bounds.
         
         Returns
         -------
         None
             Nothing
         """
         
-        self.X = np.clip(self.X, self._optimizer.lb, self._optimizer.ub)
+        self.X = np.clip(self.X, optimizer.lb, optimizer.ub)
 
     def copy(self):
         """Method for creating a true (deep) copy of the CandidateState. 
         
         Returns
         -------
         CandidateState
             CandidateState instance
         """
         
-        cP = self.__class__(self._optimizer)         
+        # cP = self.__class__(self._optimizer)
+        cP = copy.deepcopy(self)
         # Real copy for ndarrays
         # cP.X = np.copy(self.X)
         # cP.O = np.copy(self.O)
         # cP.C = np.copy(self.C)
         # cP.f = self.f
 
-        if self._optimizer.forward_unique_str:
-            cP.unique_str = self.unique_str
+        # if self._optimizer.forward_unique_str:
+        # if self.unique_str:
+        cP.unique_str = self.unique_str
 
         for var, value in vars(self).items():
             if not var.startswith('_'):
                 if isinstance(value, (int, float, str, bool)):
                     setattr(cP, var, value)
                 elif isinstance(value, (list, dict)) and len(value) > 0:
                     setattr(cP, var, value)
```

## indago/_pso.py

```diff
@@ -180,36 +180,40 @@
 
         Returns
         -------
         err_msg : str or None
             Error message (if any).
         """
 
+        if self.variant == 'TVAC' or self.params['inertia'] == 'anakatabatic':
+            assert self.max_iterations or self.max_evaluations or self.max_elapsed_time, \
+                'optimizer.max_iteration, optimizer.max_evaluations, or self.max_elapsed_time should be provided for this method/variant'
+
         self._evaluate_initial_candidates()
         err_msg = None
         
         # Bounds for position and velocity
         self._v_max = 0.2 * (self.ub - self.lb)
 
         # Generate a swarm
         self.cS = np.array([Particle(self) for c in range(self.params['swarm_size'])], dtype=Particle)
         
         # Prepare arrays
         self._dF = np.empty([self.params['swarm_size']]) * np.nan
 
         # Generate initial positions
-        n0 = 0 if self._cs0 is None else self._cs0.size
+        n0 = 0 if self._cS0 is None else self._cS0.size
         for p in range(self.params['swarm_size']):
             
             # Random position
             self.cS[p].X = np.random.uniform(self.lb, self.ub)
             
             # Using specified particles initial positions
             if p < n0:
-                self.cS[p] = self._cs0[p].copy()
+                self.cS[p] = self._cS0[p].copy()
                     
             # Generate velocity
             self.cS[p].V = np.random.uniform(-self._v_max, self._v_max)
 
             # No fitness change at the start
             self._dF[p] = 0.0
 
@@ -325,15 +329,15 @@
                 
                 cP.V = w[p] * cP.V + \
                                c1 * R1[p, :] * (self.cB[p].X - cP.X) + \
                                c2 * R2[p, :] * (self.cB[self.BI[p]].X - cP.X)
                 cP.X = cP.X + cP.V        
                 
                 # Correct position to the bounds
-                cP.clip()
+                cP.clip(self)
                 
             # Get old fitness
             f_old = np.array([cP.f for cP in self.cS])
 
             # Evaluate swarm
             err_msg = self.collective_evaluation(self.cS)
             if err_msg:
```

## indago/_sa.py

```diff
@@ -4,18 +4,15 @@
 
 
 import numpy as np
 from ._optimizer import Optimizer, CandidateState 
 import random as rnd
 
 
-class Agent(CandidateState):
-    
-    def __init__(self, optimizer: Optimizer):
-        CandidateState.__init__(self, optimizer)
+Agent = CandidateState
 
 class SA(Optimizer):
     """Simulated Annealing Algorithm class
     
     Returns
     -------
     optimizer : SA
@@ -54,22 +51,22 @@
         self._evaluate_initial_candidates()
         err_msg = None
 
         # Generate agents
         self.cS = np.array([Agent(self) for c in range(self.params['pop'])], dtype=Agent)
 
         # Generate initial points
-        n0 = 0 if self._cs0 is None else self._cs0.size
+        n0 = 0 if self._cS0 is None else self._cS0.size
         for p in range(self.params['pop']):
             # Random position
             self.cS[p].X =  np.random.uniform(self.lb, self.ub)
 
             # Using specified initial positions
             if p < n0:
-                self.cS[p] = self._cs0[p].copy()
+                self.cS[p] = self._cS0[p].copy()
 
         # Evaluate
         if n0 < self.params['pop']:
             err_msg = self.collective_evaluation(self.cS[n0:])
 
         # if all candidates are NaNs       
         if np.isnan([cP.f for cP in self.cS]).all():
```

## indago/_ssa.py

```diff
@@ -1,25 +1,15 @@
 # -*- coding: utf-8 -*-
 
 import numpy as np
 from ._optimizer import Optimizer, CandidateState 
 from scipy.special import gamma
 
 
-class FlyingSquirrel(CandidateState):
-    """SSA agent class.
-    
-    Returns
-    -------
-    FS : FlyingSquirrel
-        FlyingSquirrel instance.        
-    """
-    
-    def __init__(self, optimizer: Optimizer):
-        CandidateState.__init__(self, optimizer)
+FlyingSquirrel = CandidateState
 
 
 class SSA(Optimizer):
     """Squirrel Search Algorithm method class.
     
     Reference: Jain, M., Singh, V., & Rani, A. (2019). A novel nature-inspired algorithm 
     for optimization: Squirrel search algorithm. Swarm and evolutionary computation, 
@@ -91,29 +81,32 @@
         Initializes and evaluates the swarm.
 
         Returns
         -------
         None
             Nothing
         """
-        
+
+        assert self.max_iterations or self.max_evaluations or self.max_elapsed_time, \
+            'optimizer.max_iteration, optimizer.max_evaluations, or self.max_elapsed_time should be provided for this method/variant'
+
         err_msg = None
 
         # Generate a swarm of FS
         self.cS = np.array([FlyingSquirrel(self) for c in range(self.params['pop_size'])], \
                             dtype=FlyingSquirrel)
         
         # Generate initial positions
-        n0 = 0 if self._cs0 is None else self._cs0.size
+        n0 = 0 if self._cS0 is None else self._cS0.size
         for p in range(self.params['pop_size']):            
             # Random position
             self.cS[p].X = np.random.uniform(self.lb, self.ub)           
             # Using specified particles initial positions
             if p < n0:
-                self.cS[p] = self._cs0[p].copy()
+                self.cS[p] = self._cS0[p].copy()
         
         # Evaluate
         if n0 < self.params['pop_size']:
             err_msg = self.collective_evaluation(self.cS[n0:])
 
         # if all candidates are NaNs       
         if np.isnan([cP.f for cP in self.cS]).all():
@@ -217,15 +210,15 @@
             # Random-Levy relocation at the end of winter season
             if (Sc < Scmin).all():
                 for fs in FSnt:
                     fs.X = self.lb + Levy() * (self.ub - self.lb)
             
             # Correct position to the bounds
             for cP in self.cS:               
-                cP.clip()       
+                cP.clip(self)
                 
             # Evaluate swarm
             err_msg = self.collective_evaluation(self.cS)
             if err_msg:
                 break
              
             if self._finalize_iteration():
```

## Comparing `Indago-0.4.5.dist-info/METADATA` & `Indago-0.4.6.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Indago
-Version: 0.4.5
+Version: 0.4.6
 Summary: Numerical optimization framework
 Home-page: http://sim.riteh.hr/
 Author: sim.riteh.hr
 Author-email: stefan.ivic@riteh.hr
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

