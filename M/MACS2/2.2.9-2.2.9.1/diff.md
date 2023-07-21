# Comparing `tmp/MACS2-2.2.9.tar.gz` & `tmp/MACS2-2.2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MACS2-2.2.9.tar", last modified: Fri Jul 21 14:00:17 2023, max compression
+gzip compressed data, was "MACS2-2.2.9.1.tar", last modified: Fri Jul 21 14:30:03 2023, max compression
```

## Comparing `MACS2-2.2.9.tar` & `MACS2-2.2.9.1.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:00:17.698569 MACS2-2.2.9/
--rw-r--r--   0 runner    (1001) docker     (123)    80507 2023-07-21 13:59:50.000000 MACS2-2.2.9/ChangeLog
--rw-r--r--   0 runner    (1001) docker     (123)     4704 2023-07-21 13:59:50.000000 MACS2-2.2.9/INSTALL.md
--rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-07-21 13:59:50.000000 MACS2-2.2.9/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:00:17.682568 MACS2-2.2.9/MACS2/
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-07-21 13:59:50.000000 MACS2-2.2.9/MACS2/Constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:00:17.698569 MACS2-2.2.9/MACS2/IO/
--rw-r--r--   0 runner    (1001) docker     (123)  1186051 2023-07-21 14:00:10.000000 MACS2-2.2.9/MACS2/IO/BedGraph.c
--rw-r--r--   0 runner    (1001) docker     (123)    43892 2023-07-21 13:59:50.000000 MACS2-2.2.9/MACS2/IO/BedGraph.pyx
--rw-r--r--   0 runner    (1001) docker     (123)   312644 2023-07-21 14:00:10.000000 MACS2-2.2.9/MACS2/IO/BedGraphIO.c
--rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-07-21 13:59:50.000000 MACS2-2.2.9/MACS2/IO/BedGraphIO.pyx
--rw-r--r--   0 runner    (1001) docker     (123)  1638518 2023-07-21 14:00:11.000000 MACS2-2.2.9/MACS2/IO/CallPeakUnit.c
--rw-r--r--   0 runner    (1001) docker     (123)    83101 2023-07-21 13:59:50.000000 MACS2-2.2.9/MACS2/IO/CallPeakUnit.pyx
--rw-r--r--   0 runner    (1001) docker     (123)  1582530 2023-07-21 13:59:50.000000 MACS2-2.2.9/MACS2/IO/CallPeakUnitPrecompiled.c
--rw-r--r--   0 runner    (1001) docker     (123)  1213319 2023-07-21 14:00:12.000000 MACS2-2.2.9/MACS2/IO/FixWidthTrack.c
--rw-r--r--   0 runner    (1001) docker     (123)    37584 2023-07-21 13:59:50.000000 MACS2-2.2.9/MACS2/IO/FixWidthTrack.pyx
--rw-r--r--   0 runner    (1001) docker     (123)   958410 2023-07-21 14:00:12.000000 MACS2-2.2.9/MACS2/IO/PairedEndTrack.c
--rw-r--r--   0 runner    (1001) docker     (123)    23052 2023-07-21 13:59:50.000000 MACS2-2.2.9/MACS2/IO/PairedEndTrack.pyx
--rw-r--r--   0 runner    (1001) docker     (123)  1766592 2023-07-21 14:00:13.000000 MACS2-2.2.9/MACS2/IO/Parser.c
--rw-r--r--   0 runner    (1001) docker     (123)    51333 2023-07-21 13:59:50.000000 MACS2-2.2.9/MACS2/IO/Parser.pyx
--rw-r--r--   0 runner    (1001) docker     (123)  1478779 2023-07-21 14:00:14.000000 MACS2-2.2.9/MACS2/IO/PeakIO.c
--rw-r--r--   0 runner    (1001) docker     (123)    51188 2023-07-21 13:59:50.000000 MACS2-2.2.9/MACS2/IO/PeakIO.pyx
--rw-r--r--   0 runner    (1001) docker     (123)  1881571 2023-07-21 14:00:15.000000 MACS2-2.2.9/MACS2/IO/ScoreTrack.c
--rw-r--r--   0 runner    (1001) docker     (123)    69236 2023-07-21 13:59:50.000000 MACS2-2.2.9/MACS2/IO/ScoreTrack.pyx
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 13:59:50.000000 MACS2-2.2.9/MACS2/IO/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28454 2023-07-21 13:59:50.000000 MACS2-2.2.9/MACS2/OptValidator.py
--rw-r--r--   0 runner    (1001) docker     (123)    10842 2023-07-21 13:59:50.000000 MACS2-2.2.9/MACS2/OutputWriter.py
--rw-r--r--   0 runner    (1001) docker     (123)   463153 2023-07-21 14:00:15.000000 MACS2-2.2.9/MACS2/PeakDetect.c
--rw-r--r--   0 runner    (1001) docker     (123)    23222 2023-07-21 13:59:50.000000 MACS2-2.2.9/MACS2/PeakDetect.pyx
--rw-r--r--   0 runner    (1001) docker     (123)   905459 2023-07-21 14:00:15.000000 MACS2-2.2.9/MACS2/PeakModel.c
--rw-r--r--   0 runner    (1001) docker     (123)    25219 2023-07-21 13:59:50.000000 MACS2-2.2.9/MACS2/PeakModel.pyx
--rw-r--r--   0 runner    (1001) docker     (123)   788633 2023-07-21 14:00:16.000000 MACS2-2.2.9/MACS2/Pileup.c
--rw-r--r--   0 runner    (1001) docker     (123)    31947 2023-07-21 13:59:50.000000 MACS2-2.2.9/MACS2/Pileup.pyx
--rw-r--r--   0 runner    (1001) docker     (123)   599325 2023-07-21 14:00:17.000000 MACS2-2.2.9/MACS2/Prob.c
--rw-r--r--   0 runner    (1001) docker     (123)    24670 2023-07-21 13:59:50.000000 MACS2-2.2.9/MACS2/Prob.pyx
--rw-r--r--   0 runner    (1001) docker     (123)   550376 2023-07-21 14:00:17.000000 MACS2-2.2.9/MACS2/Signal.c
--rw-r--r--   0 runner    (1001) docker     (123)    13890 2023-07-21 13:59:50.000000 MACS2-2.2.9/MACS2/Signal.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-07-21 13:59:50.000000 MACS2-2.2.9/MACS2/Statistics.pyx
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-21 13:59:50.000000 MACS2-2.2.9/MACS2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-07-21 13:59:50.000000 MACS2-2.2.9/MACS2/bdgbroadcall_cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-07-21 13:59:50.000000 MACS2-2.2.9/MACS2/bdgcmp_cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4318 2023-07-21 13:59:50.000000 MACS2-2.2.9/MACS2/bdgdiff_cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-07-21 13:59:50.000000 MACS2-2.2.9/MACS2/bdgopt_cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-07-21 13:59:50.000000 MACS2-2.2.9/MACS2/bdgpeakcall_cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)    13945 2023-07-21 13:59:50.000000 MACS2-2.2.9/MACS2/cPosValCalculation.c
--rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-07-21 13:59:50.000000 MACS2-2.2.9/MACS2/cPosValCalculation.h
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-07-21 13:59:50.000000 MACS2-2.2.9/MACS2/cPosValCalculation.pxd
--rw-r--r--   0 runner    (1001) docker     (123)    19674 2023-07-21 13:59:50.000000 MACS2-2.2.9/MACS2/callpeak_cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-07-21 13:59:50.000000 MACS2-2.2.9/MACS2/cmbreps_cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     9715 2023-07-21 13:59:50.000000 MACS2-2.2.9/MACS2/diffpeak_cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4583 2023-07-21 13:59:50.000000 MACS2-2.2.9/MACS2/filterdup_cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)    21042 2023-07-21 13:59:50.000000 MACS2-2.2.9/MACS2/khash.h
--rw-r--r--   0 runner    (1001) docker     (123)     3199 2023-07-21 13:59:50.000000 MACS2-2.2.9/MACS2/khash.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-07-21 13:59:50.000000 MACS2-2.2.9/MACS2/pileup_cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3178 2023-07-21 13:59:50.000000 MACS2-2.2.9/MACS2/predictd_cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3888 2023-07-21 13:59:50.000000 MACS2-2.2.9/MACS2/randsample_cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6845 2023-07-21 13:59:50.000000 MACS2-2.2.9/MACS2/refinepeak_cmd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:00:17.682568 MACS2-2.2.9/MACS2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    26444 2023-07-21 14:00:17.000000 MACS2-2.2.9/MACS2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-07-21 14:00:17.000000 MACS2-2.2.9/MACS2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 14:00:17.000000 MACS2-2.2.9/MACS2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-21 14:00:17.000000 MACS2-2.2.9/MACS2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-21 14:00:17.000000 MACS2-2.2.9/MACS2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-21 13:59:50.000000 MACS2-2.2.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    26444 2023-07-21 14:00:17.698569 MACS2-2.2.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    25478 2023-07-21 13:59:50.000000 MACS2-2.2.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:00:17.698569 MACS2-2.2.9/bin/
--rw-r--r--   0 runner    (1001) docker     (123)    67799 2023-07-21 13:59:50.000000 MACS2-2.2.9/bin/macs2
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-21 13:59:50.000000 MACS2-2.2.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 14:00:17.698569 MACS2-2.2.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-07-21 13:59:50.000000 MACS2-2.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:30:03.820698 MACS2-2.2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    80509 2023-07-21 14:29:40.000000 MACS2-2.2.9.1/ChangeLog
+-rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-07-21 14:29:40.000000 MACS2-2.2.9.1/INSTALL.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-07-21 14:29:40.000000 MACS2-2.2.9.1/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:30:03.804698 MACS2-2.2.9.1/MACS2/
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-07-21 14:29:40.000000 MACS2-2.2.9.1/MACS2/Constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:30:03.820698 MACS2-2.2.9.1/MACS2/IO/
+-rw-r--r--   0 runner    (1001) docker     (123)  1186051 2023-07-21 14:29:56.000000 MACS2-2.2.9.1/MACS2/IO/BedGraph.c
+-rw-r--r--   0 runner    (1001) docker     (123)    43892 2023-07-21 14:29:40.000000 MACS2-2.2.9.1/MACS2/IO/BedGraph.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)   312644 2023-07-21 14:29:57.000000 MACS2-2.2.9.1/MACS2/IO/BedGraphIO.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-07-21 14:29:40.000000 MACS2-2.2.9.1/MACS2/IO/BedGraphIO.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)  1638518 2023-07-21 14:29:57.000000 MACS2-2.2.9.1/MACS2/IO/CallPeakUnit.c
+-rw-r--r--   0 runner    (1001) docker     (123)    83101 2023-07-21 14:29:40.000000 MACS2-2.2.9.1/MACS2/IO/CallPeakUnit.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)  1582530 2023-07-21 14:29:40.000000 MACS2-2.2.9.1/MACS2/IO/CallPeakUnitPrecompiled.c
+-rw-r--r--   0 runner    (1001) docker     (123)  1213319 2023-07-21 14:29:58.000000 MACS2-2.2.9.1/MACS2/IO/FixWidthTrack.c
+-rw-r--r--   0 runner    (1001) docker     (123)    37584 2023-07-21 14:29:40.000000 MACS2-2.2.9.1/MACS2/IO/FixWidthTrack.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)   958410 2023-07-21 14:29:59.000000 MACS2-2.2.9.1/MACS2/IO/PairedEndTrack.c
+-rw-r--r--   0 runner    (1001) docker     (123)    23052 2023-07-21 14:29:40.000000 MACS2-2.2.9.1/MACS2/IO/PairedEndTrack.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)  1766592 2023-07-21 14:30:00.000000 MACS2-2.2.9.1/MACS2/IO/Parser.c
+-rw-r--r--   0 runner    (1001) docker     (123)    51333 2023-07-21 14:29:40.000000 MACS2-2.2.9.1/MACS2/IO/Parser.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)  1478779 2023-07-21 14:30:00.000000 MACS2-2.2.9.1/MACS2/IO/PeakIO.c
+-rw-r--r--   0 runner    (1001) docker     (123)    51188 2023-07-21 14:29:40.000000 MACS2-2.2.9.1/MACS2/IO/PeakIO.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)  1881571 2023-07-21 14:30:01.000000 MACS2-2.2.9.1/MACS2/IO/ScoreTrack.c
+-rw-r--r--   0 runner    (1001) docker     (123)    69236 2023-07-21 14:29:40.000000 MACS2-2.2.9.1/MACS2/IO/ScoreTrack.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 14:29:40.000000 MACS2-2.2.9.1/MACS2/IO/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28454 2023-07-21 14:29:40.000000 MACS2-2.2.9.1/MACS2/OptValidator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10842 2023-07-21 14:29:40.000000 MACS2-2.2.9.1/MACS2/OutputWriter.py
+-rw-r--r--   0 runner    (1001) docker     (123)   463153 2023-07-21 14:30:01.000000 MACS2-2.2.9.1/MACS2/PeakDetect.c
+-rw-r--r--   0 runner    (1001) docker     (123)    23222 2023-07-21 14:29:40.000000 MACS2-2.2.9.1/MACS2/PeakDetect.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)   905459 2023-07-21 14:30:02.000000 MACS2-2.2.9.1/MACS2/PeakModel.c
+-rw-r--r--   0 runner    (1001) docker     (123)    25219 2023-07-21 14:29:40.000000 MACS2-2.2.9.1/MACS2/PeakModel.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)   788633 2023-07-21 14:30:02.000000 MACS2-2.2.9.1/MACS2/Pileup.c
+-rw-r--r--   0 runner    (1001) docker     (123)    31947 2023-07-21 14:29:40.000000 MACS2-2.2.9.1/MACS2/Pileup.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)   599325 2023-07-21 14:30:03.000000 MACS2-2.2.9.1/MACS2/Prob.c
+-rw-r--r--   0 runner    (1001) docker     (123)    24670 2023-07-21 14:29:40.000000 MACS2-2.2.9.1/MACS2/Prob.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)   550376 2023-07-21 14:30:03.000000 MACS2-2.2.9.1/MACS2/Signal.c
+-rw-r--r--   0 runner    (1001) docker     (123)    13890 2023-07-21 14:29:40.000000 MACS2-2.2.9.1/MACS2/Signal.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-07-21 14:29:40.000000 MACS2-2.2.9.1/MACS2/Statistics.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-21 14:29:40.000000 MACS2-2.2.9.1/MACS2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-07-21 14:29:40.000000 MACS2-2.2.9.1/MACS2/bdgbroadcall_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-07-21 14:29:40.000000 MACS2-2.2.9.1/MACS2/bdgcmp_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4318 2023-07-21 14:29:40.000000 MACS2-2.2.9.1/MACS2/bdgdiff_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-07-21 14:29:40.000000 MACS2-2.2.9.1/MACS2/bdgopt_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-07-21 14:29:40.000000 MACS2-2.2.9.1/MACS2/bdgpeakcall_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13945 2023-07-21 14:29:40.000000 MACS2-2.2.9.1/MACS2/cPosValCalculation.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-07-21 14:29:40.000000 MACS2-2.2.9.1/MACS2/cPosValCalculation.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-07-21 14:29:40.000000 MACS2-2.2.9.1/MACS2/cPosValCalculation.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    19674 2023-07-21 14:29:40.000000 MACS2-2.2.9.1/MACS2/callpeak_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-07-21 14:29:40.000000 MACS2-2.2.9.1/MACS2/cmbreps_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9715 2023-07-21 14:29:40.000000 MACS2-2.2.9.1/MACS2/diffpeak_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4583 2023-07-21 14:29:40.000000 MACS2-2.2.9.1/MACS2/filterdup_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21042 2023-07-21 14:29:40.000000 MACS2-2.2.9.1/MACS2/khash.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3199 2023-07-21 14:29:40.000000 MACS2-2.2.9.1/MACS2/khash.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-07-21 14:29:40.000000 MACS2-2.2.9.1/MACS2/pileup_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3178 2023-07-21 14:29:40.000000 MACS2-2.2.9.1/MACS2/predictd_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3888 2023-07-21 14:29:40.000000 MACS2-2.2.9.1/MACS2/randsample_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6845 2023-07-21 14:29:40.000000 MACS2-2.2.9.1/MACS2/refinepeak_cmd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:30:03.804698 MACS2-2.2.9.1/MACS2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    26681 2023-07-21 14:30:03.000000 MACS2-2.2.9.1/MACS2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-07-21 14:30:03.000000 MACS2-2.2.9.1/MACS2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 14:30:03.000000 MACS2-2.2.9.1/MACS2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-21 14:30:03.000000 MACS2-2.2.9.1/MACS2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-21 14:30:03.000000 MACS2-2.2.9.1/MACS2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-21 14:29:40.000000 MACS2-2.2.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    26681 2023-07-21 14:30:03.820698 MACS2-2.2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    25713 2023-07-21 14:29:40.000000 MACS2-2.2.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:30:03.820698 MACS2-2.2.9.1/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)    67799 2023-07-21 14:29:40.000000 MACS2-2.2.9.1/bin/macs2
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-21 14:29:40.000000 MACS2-2.2.9.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 14:30:03.820698 MACS2-2.2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-07-21 14:29:40.000000 MACS2-2.2.9.1/setup.py
```

### Comparing `MACS2-2.2.9/ChangeLog` & `MACS2-2.2.9.1/ChangeLog`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-2020-07-20  Tao Liu  <vladimir.liu@gmail.com>
-   MACS version 2.2.9
+2020-07-21  Tao Liu  <vladimir.liu@gmail.com>
+   MACS version 2.2.9.1
    
    * Bug fix:
      
     Cython has a major upgrade to 3.0, and can't work directly with
     MACS2 codes, so we changed the requirement for Cython to 0.29.*.
     
     Python support has been changed to 3.7 to 3.11. Numpy >=0.19.
```

### Comparing `MACS2-2.2.9/INSTALL.md` & `MACS2-2.2.9.1/INSTALL.md`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 
 The easiest way to install MACS is through PyPI system. Get `pip` if
 it's not available in your system. If you create a virtual environment
 as described before, your `pip` command will install everything under
 the folder you specified previously through `python3 -m env` command.
 
 Then under the command line, type `pip install macs2`. PyPI will
-install Numpy automatically if it is absent.
+install Cython and Numpy automatically when necessary.
 
 To upgrade MACS2, type `pip install --upgrade macs2`. It will check
 currently installed MACS2, compare the version with the one on PyPI
 repository, download and install a newer version while necessary.
 
 ## Install through Conda
```

### Comparing `MACS2-2.2.9/LICENSE` & `MACS2-2.2.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `MACS2-2.2.9/MACS2/Constants.py` & `MACS2-2.2.9.1/MACS2/Constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-MACS_VERSION = "2.2.9"
+MACS_VERSION = "2.2.9.1"
 FILTERDUP_VERSION = "1.0.0 20140616"
 RANDSAMPLE_VERSION = "1.0.0 20120703"
 MAX_PAIRNUM = 1000
 MAX_LAMBDA  = 100000
 FESTEP      = 20
 BUFFER_SIZE = 100000                   # np array will increase at step of 1 million items
```

### Comparing `MACS2-2.2.9/MACS2/IO/BedGraph.c` & `MACS2-2.2.9.1/MACS2/IO/BedGraph.c`

 * *Files identical despite different names*

### Comparing `MACS2-2.2.9/MACS2/IO/BedGraph.pyx` & `MACS2-2.2.9.1/MACS2/IO/BedGraph.pyx`

 * *Files identical despite different names*

### Comparing `MACS2-2.2.9/MACS2/IO/BedGraphIO.c` & `MACS2-2.2.9.1/MACS2/IO/BedGraphIO.c`

 * *Files identical despite different names*

### Comparing `MACS2-2.2.9/MACS2/IO/BedGraphIO.pyx` & `MACS2-2.2.9.1/MACS2/IO/BedGraphIO.pyx`

 * *Files identical despite different names*

### Comparing `MACS2-2.2.9/MACS2/IO/CallPeakUnit.c` & `MACS2-2.2.9.1/MACS2/IO/CallPeakUnit.c`

 * *Files identical despite different names*

### Comparing `MACS2-2.2.9/MACS2/IO/CallPeakUnit.pyx` & `MACS2-2.2.9.1/MACS2/IO/CallPeakUnit.pyx`

 * *Files identical despite different names*

### Comparing `MACS2-2.2.9/MACS2/IO/CallPeakUnitPrecompiled.c` & `MACS2-2.2.9.1/MACS2/IO/CallPeakUnitPrecompiled.c`

 * *Files identical despite different names*

### Comparing `MACS2-2.2.9/MACS2/IO/FixWidthTrack.c` & `MACS2-2.2.9.1/MACS2/IO/FixWidthTrack.c`

 * *Files identical despite different names*

### Comparing `MACS2-2.2.9/MACS2/IO/FixWidthTrack.pyx` & `MACS2-2.2.9.1/MACS2/IO/FixWidthTrack.pyx`

 * *Files identical despite different names*

### Comparing `MACS2-2.2.9/MACS2/IO/PairedEndTrack.c` & `MACS2-2.2.9.1/MACS2/IO/PairedEndTrack.c`

 * *Files identical despite different names*

### Comparing `MACS2-2.2.9/MACS2/IO/PairedEndTrack.pyx` & `MACS2-2.2.9.1/MACS2/IO/PairedEndTrack.pyx`

 * *Files identical despite different names*

### Comparing `MACS2-2.2.9/MACS2/IO/Parser.c` & `MACS2-2.2.9.1/MACS2/IO/Parser.c`

 * *Files identical despite different names*

### Comparing `MACS2-2.2.9/MACS2/IO/Parser.pyx` & `MACS2-2.2.9.1/MACS2/IO/Parser.pyx`

 * *Files identical despite different names*

### Comparing `MACS2-2.2.9/MACS2/IO/PeakIO.c` & `MACS2-2.2.9.1/MACS2/IO/PeakIO.c`

 * *Files identical despite different names*

### Comparing `MACS2-2.2.9/MACS2/IO/PeakIO.pyx` & `MACS2-2.2.9.1/MACS2/IO/PeakIO.pyx`

 * *Files identical despite different names*

### Comparing `MACS2-2.2.9/MACS2/IO/ScoreTrack.c` & `MACS2-2.2.9.1/MACS2/IO/ScoreTrack.c`

 * *Files identical despite different names*

### Comparing `MACS2-2.2.9/MACS2/IO/ScoreTrack.pyx` & `MACS2-2.2.9.1/MACS2/IO/ScoreTrack.pyx`

 * *Files identical despite different names*

### Comparing `MACS2-2.2.9/MACS2/OptValidator.py` & `MACS2-2.2.9.1/MACS2/OptValidator.py`

 * *Files identical despite different names*

### Comparing `MACS2-2.2.9/MACS2/OutputWriter.py` & `MACS2-2.2.9.1/MACS2/OutputWriter.py`

 * *Files identical despite different names*

### Comparing `MACS2-2.2.9/MACS2/PeakDetect.c` & `MACS2-2.2.9.1/MACS2/PeakDetect.c`

 * *Files identical despite different names*

### Comparing `MACS2-2.2.9/MACS2/PeakDetect.pyx` & `MACS2-2.2.9.1/MACS2/PeakDetect.pyx`

 * *Files identical despite different names*

### Comparing `MACS2-2.2.9/MACS2/PeakModel.c` & `MACS2-2.2.9.1/MACS2/PeakModel.c`

 * *Files identical despite different names*

### Comparing `MACS2-2.2.9/MACS2/PeakModel.pyx` & `MACS2-2.2.9.1/MACS2/PeakModel.pyx`

 * *Files identical despite different names*

### Comparing `MACS2-2.2.9/MACS2/Pileup.c` & `MACS2-2.2.9.1/MACS2/Pileup.c`

 * *Files identical despite different names*

### Comparing `MACS2-2.2.9/MACS2/Pileup.pyx` & `MACS2-2.2.9.1/MACS2/Pileup.pyx`

 * *Files identical despite different names*

### Comparing `MACS2-2.2.9/MACS2/Prob.c` & `MACS2-2.2.9.1/MACS2/Prob.c`

 * *Files identical despite different names*

### Comparing `MACS2-2.2.9/MACS2/Prob.pyx` & `MACS2-2.2.9.1/MACS2/Prob.pyx`

 * *Files identical despite different names*

### Comparing `MACS2-2.2.9/MACS2/Signal.c` & `MACS2-2.2.9.1/MACS2/Signal.c`

 * *Files identical despite different names*

### Comparing `MACS2-2.2.9/MACS2/Signal.pyx` & `MACS2-2.2.9.1/MACS2/Signal.pyx`

 * *Files identical despite different names*

### Comparing `MACS2-2.2.9/MACS2/Statistics.pyx` & `MACS2-2.2.9.1/MACS2/Statistics.pyx`

 * *Files identical despite different names*

### Comparing `MACS2-2.2.9/MACS2/bdgbroadcall_cmd.py` & `MACS2-2.2.9.1/MACS2/bdgbroadcall_cmd.py`

 * *Files identical despite different names*

### Comparing `MACS2-2.2.9/MACS2/bdgcmp_cmd.py` & `MACS2-2.2.9.1/MACS2/bdgcmp_cmd.py`

 * *Files identical despite different names*

### Comparing `MACS2-2.2.9/MACS2/bdgdiff_cmd.py` & `MACS2-2.2.9.1/MACS2/bdgdiff_cmd.py`

 * *Files identical despite different names*

### Comparing `MACS2-2.2.9/MACS2/bdgopt_cmd.py` & `MACS2-2.2.9.1/MACS2/bdgopt_cmd.py`

 * *Files identical despite different names*

### Comparing `MACS2-2.2.9/MACS2/bdgpeakcall_cmd.py` & `MACS2-2.2.9.1/MACS2/bdgpeakcall_cmd.py`

 * *Files identical despite different names*

### Comparing `MACS2-2.2.9/MACS2/cPosValCalculation.c` & `MACS2-2.2.9.1/MACS2/cPosValCalculation.c`

 * *Files identical despite different names*

### Comparing `MACS2-2.2.9/MACS2/cPosValCalculation.h` & `MACS2-2.2.9.1/MACS2/cPosValCalculation.h`

 * *Files identical despite different names*

### Comparing `MACS2-2.2.9/MACS2/cPosValCalculation.pxd` & `MACS2-2.2.9.1/MACS2/cPosValCalculation.pxd`

 * *Files identical despite different names*

### Comparing `MACS2-2.2.9/MACS2/callpeak_cmd.py` & `MACS2-2.2.9.1/MACS2/callpeak_cmd.py`

 * *Files identical despite different names*

### Comparing `MACS2-2.2.9/MACS2/cmbreps_cmd.py` & `MACS2-2.2.9.1/MACS2/cmbreps_cmd.py`

 * *Files identical despite different names*

### Comparing `MACS2-2.2.9/MACS2/diffpeak_cmd.py` & `MACS2-2.2.9.1/MACS2/diffpeak_cmd.py`

 * *Files identical despite different names*

### Comparing `MACS2-2.2.9/MACS2/filterdup_cmd.py` & `MACS2-2.2.9.1/MACS2/filterdup_cmd.py`

 * *Files identical despite different names*

### Comparing `MACS2-2.2.9/MACS2/khash.h` & `MACS2-2.2.9.1/MACS2/khash.h`

 * *Files identical despite different names*

### Comparing `MACS2-2.2.9/MACS2/khash.pxd` & `MACS2-2.2.9.1/MACS2/khash.pxd`

 * *Files identical despite different names*

### Comparing `MACS2-2.2.9/MACS2/pileup_cmd.py` & `MACS2-2.2.9.1/MACS2/pileup_cmd.py`

 * *Files identical despite different names*

### Comparing `MACS2-2.2.9/MACS2/predictd_cmd.py` & `MACS2-2.2.9.1/MACS2/predictd_cmd.py`

 * *Files identical despite different names*

### Comparing `MACS2-2.2.9/MACS2/randsample_cmd.py` & `MACS2-2.2.9.1/MACS2/randsample_cmd.py`

 * *Files identical despite different names*

### Comparing `MACS2-2.2.9/MACS2/refinepeak_cmd.py` & `MACS2-2.2.9.1/MACS2/refinepeak_cmd.py`

 * *Files identical despite different names*

### Comparing `MACS2-2.2.9/MACS2.egg-info/PKG-INFO` & `MACS2-2.2.9.1/MACS2.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MACS2
-Version: 2.2.9
+Version: 2.2.9.1
 Summary: Model Based Analysis for ChIP-Seq data
 Home-page: http://github.com/macs3-project/MACS/
 Author: Tao Liu
 Author-email: vladimir.liu@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
@@ -52,17 +52,17 @@
 applied to any "DNA enrichment assays" if the question to be asked is
 simply: *where we can find significant reads coverage than the random
 background*.
 
 *Note: new development on MACS has been moved to MACS3 repository,
 we will only fix installation issues on MACS2.*
 
-## Recent Changes for MACS (2.2.9)
+## Recent Changes for MACS (2.2.9.1)
 
-### 2.2.9
+### 2.2.9.1
     * Bug fix:
      
     Cython has a major upgrade to 3.0, and can't work directly with
     MACS2 codes, so we changed the requirement for Cython to 0.29.*.
     
     Python support has been changed to 3.7 to 3.11. Numpy >=0.19.
     
@@ -152,15 +152,19 @@
 	standard result can be found; 4. prockreport monitor CPU time and 
 	memory usage in 1 sec interval -- a bit more accurate.
 	
 	2) Python3.5 support is removed. Now MACS2 requires Python>=3.6.
 
 ## Install
 
-Please check the file 'INSTALL.md' in the distribution.
+Please check the file 'INSTALL.md' in the distribution. In general,
+you can install through PyPI as `pip install macs2`. To use virtual 
+environment is highly recommended. Or you can install after
+unzipping the released package downloaded from Github, then use 
+`pip install .` command.
 
 ## Usage
 
 ```
 macs2 [-h] [--version]
     {callpeak,bdgpeakcall,bdgbroadcall,bdgcmp,bdgopt,cmbreps,bdgdiff,filterdup,predictd,pileup,randsample,refinepeak}
 ```
```

### Comparing `MACS2-2.2.9/MACS2.egg-info/SOURCES.txt` & `MACS2-2.2.9.1/MACS2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `MACS2-2.2.9/PKG-INFO` & `MACS2-2.2.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MACS2
-Version: 2.2.9
+Version: 2.2.9.1
 Summary: Model Based Analysis for ChIP-Seq data
 Home-page: http://github.com/macs3-project/MACS/
 Author: Tao Liu
 Author-email: vladimir.liu@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
@@ -52,17 +52,17 @@
 applied to any "DNA enrichment assays" if the question to be asked is
 simply: *where we can find significant reads coverage than the random
 background*.
 
 *Note: new development on MACS has been moved to MACS3 repository,
 we will only fix installation issues on MACS2.*
 
-## Recent Changes for MACS (2.2.9)
+## Recent Changes for MACS (2.2.9.1)
 
-### 2.2.9
+### 2.2.9.1
     * Bug fix:
      
     Cython has a major upgrade to 3.0, and can't work directly with
     MACS2 codes, so we changed the requirement for Cython to 0.29.*.
     
     Python support has been changed to 3.7 to 3.11. Numpy >=0.19.
     
@@ -152,15 +152,19 @@
 	standard result can be found; 4. prockreport monitor CPU time and 
 	memory usage in 1 sec interval -- a bit more accurate.
 	
 	2) Python3.5 support is removed. Now MACS2 requires Python>=3.6.
 
 ## Install
 
-Please check the file 'INSTALL.md' in the distribution.
+Please check the file 'INSTALL.md' in the distribution. In general,
+you can install through PyPI as `pip install macs2`. To use virtual 
+environment is highly recommended. Or you can install after
+unzipping the released package downloaded from Github, then use 
+`pip install .` command.
 
 ## Usage
 
 ```
 macs2 [-h] [--version]
     {callpeak,bdgpeakcall,bdgbroadcall,bdgcmp,bdgopt,cmbreps,bdgdiff,filterdup,predictd,pileup,randsample,refinepeak}
 ```
```

### Comparing `MACS2-2.2.9/README.md` & `MACS2-2.2.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -27,17 +27,17 @@
 applied to any "DNA enrichment assays" if the question to be asked is
 simply: *where we can find significant reads coverage than the random
 background*.
 
 *Note: new development on MACS has been moved to MACS3 repository,
 we will only fix installation issues on MACS2.*
 
-## Recent Changes for MACS (2.2.9)
+## Recent Changes for MACS (2.2.9.1)
 
-### 2.2.9
+### 2.2.9.1
     * Bug fix:
      
     Cython has a major upgrade to 3.0, and can't work directly with
     MACS2 codes, so we changed the requirement for Cython to 0.29.*.
     
     Python support has been changed to 3.7 to 3.11. Numpy >=0.19.
     
@@ -127,15 +127,19 @@
 	standard result can be found; 4. prockreport monitor CPU time and 
 	memory usage in 1 sec interval -- a bit more accurate.
 	
 	2) Python3.5 support is removed. Now MACS2 requires Python>=3.6.
 
 ## Install
 
-Please check the file 'INSTALL.md' in the distribution.
+Please check the file 'INSTALL.md' in the distribution. In general,
+you can install through PyPI as `pip install macs2`. To use virtual 
+environment is highly recommended. Or you can install after
+unzipping the released package downloaded from Github, then use 
+`pip install .` command.
 
 ## Usage
 
 ```
 macs2 [-h] [--version]
     {callpeak,bdgpeakcall,bdgbroadcall,bdgcmp,bdgopt,cmbreps,bdgdiff,filterdup,predictd,pileup,randsample,refinepeak}
 ```
```

### Comparing `MACS2-2.2.9/bin/macs2` & `MACS2-2.2.9.1/bin/macs2`

 * *Files identical despite different names*

### Comparing `MACS2-2.2.9/setup.py` & `MACS2-2.2.9.1/setup.py`

 * *Files identical despite different names*

