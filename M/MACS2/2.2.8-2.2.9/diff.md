# Comparing `tmp/MACS2-2.2.8.tar.gz` & `tmp/MACS2-2.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MACS2-2.2.8.tar", last modified: Mon May 15 14:09:33 2023, max compression
+gzip compressed data, was "MACS2-2.2.9.tar", last modified: Fri Jul 21 14:00:17 2023, max compression
```

## Comparing `MACS2-2.2.8.tar` & `MACS2-2.2.9.tar`

### file list

```diff
@@ -1,58 +1,71 @@
-drwxr-xr-x   0 ta32852  (6769229) ROSWELL\Domain Users (735121457)        0 2023-05-15 14:09:33.322432 MACS2-2.2.8/
--rw-r--r--   0 ta32852  (6769229) ROSWELL\Domain Users (735121457)    80103 2023-05-12 19:58:26.000000 MACS2-2.2.8/ChangeLog
--rw-r--r--   0 ta32852  (6769229) ROSWELL\Domain Users (735121457)     5500 2023-05-12 19:42:10.000000 MACS2-2.2.8/INSTALL.md
--rw-r--r--   0 ta32852  (6769229) ROSWELL\Domain Users (735121457)     1623 2023-05-12 19:42:10.000000 MACS2-2.2.8/LICENSE
-drwxr-xr-x   0 ta32852  (6769229) ROSWELL\Domain Users (735121457)        0 2023-05-15 14:09:33.314275 MACS2-2.2.8/MACS2/
--rw-r--r--   0 ta32852  (6769229) ROSWELL\Domain Users (735121457)      843 2023-05-12 19:57:33.000000 MACS2-2.2.8/MACS2/Constants.py
-drwxr-xr-x   0 ta32852  (6769229) ROSWELL\Domain Users (735121457)        0 2023-05-15 14:09:33.321725 MACS2-2.2.8/MACS2/IO/
--rw-r--r--   0 ta32852  (6769229) ROSWELL\Domain Users (735121457)    43892 2023-05-12 19:42:10.000000 MACS2-2.2.8/MACS2/IO/BedGraph.pyx
--rw-r--r--   0 ta32852  (6769229) ROSWELL\Domain Users (735121457)     4778 2023-05-12 19:42:10.000000 MACS2-2.2.8/MACS2/IO/BedGraphIO.pyx
--rw-r--r--   0 ta32852  (6769229) ROSWELL\Domain Users (735121457)    83101 2023-05-12 19:42:10.000000 MACS2-2.2.8/MACS2/IO/CallPeakUnit.pyx
--rw-r--r--   0 ta32852  (6769229) ROSWELL\Domain Users (735121457)  1582530 2023-05-12 19:42:10.000000 MACS2-2.2.8/MACS2/IO/CallPeakUnitPrecompiled.c
--rw-r--r--   0 ta32852  (6769229) ROSWELL\Domain Users (735121457)    37584 2023-05-12 19:42:10.000000 MACS2-2.2.8/MACS2/IO/FixWidthTrack.pyx
--rw-r--r--   0 ta32852  (6769229) ROSWELL\Domain Users (735121457)    23052 2023-05-12 19:42:10.000000 MACS2-2.2.8/MACS2/IO/PairedEndTrack.pyx
--rw-r--r--   0 ta32852  (6769229) ROSWELL\Domain Users (735121457)    51333 2023-05-12 19:42:10.000000 MACS2-2.2.8/MACS2/IO/Parser.pyx
--rw-r--r--   0 ta32852  (6769229) ROSWELL\Domain Users (735121457)    51188 2023-05-12 19:42:10.000000 MACS2-2.2.8/MACS2/IO/PeakIO.pyx
--rw-r--r--   0 ta32852  (6769229) ROSWELL\Domain Users (735121457)    69236 2023-05-12 19:42:10.000000 MACS2-2.2.8/MACS2/IO/ScoreTrack.pyx
--rw-r--r--   0 ta32852  (6769229) ROSWELL\Domain Users (735121457)        0 2023-05-12 19:42:10.000000 MACS2-2.2.8/MACS2/IO/__init__.py
--rw-r--r--   0 ta32852  (6769229) ROSWELL\Domain Users (735121457)    28454 2023-05-12 19:42:10.000000 MACS2-2.2.8/MACS2/OptValidator.py
--rw-r--r--   0 ta32852  (6769229) ROSWELL\Domain Users (735121457)    10842 2023-05-12 19:42:10.000000 MACS2-2.2.8/MACS2/OutputWriter.py
--rw-r--r--   0 ta32852  (6769229) ROSWELL\Domain Users (735121457)    23222 2023-05-12 19:42:10.000000 MACS2-2.2.8/MACS2/PeakDetect.pyx
--rw-r--r--   0 ta32852  (6769229) ROSWELL\Domain Users (735121457)    25219 2023-05-12 19:42:10.000000 MACS2-2.2.8/MACS2/PeakModel.pyx
--rw-r--r--   0 ta32852  (6769229) ROSWELL\Domain Users (735121457)    31947 2023-05-12 19:42:10.000000 MACS2-2.2.8/MACS2/Pileup.pyx
--rw-r--r--   0 ta32852  (6769229) ROSWELL\Domain Users (735121457)    24670 2023-05-12 19:42:10.000000 MACS2-2.2.8/MACS2/Prob.pyx
--rw-r--r--   0 ta32852  (6769229) ROSWELL\Domain Users (735121457)    13890 2023-05-12 19:42:10.000000 MACS2-2.2.8/MACS2/Signal.pyx
--rw-r--r--   0 ta32852  (6769229) ROSWELL\Domain Users (735121457)     3291 2023-05-12 19:42:10.000000 MACS2-2.2.8/MACS2/Statistics.pyx
--rw-r--r--   0 ta32852  (6769229) ROSWELL\Domain Users (735121457)       24 2023-05-12 19:42:10.000000 MACS2-2.2.8/MACS2/__init__.py
--rw-r--r--   0 ta32852  (6769229) ROSWELL\Domain Users (735121457)     2141 2023-05-12 19:42:10.000000 MACS2-2.2.8/MACS2/bdgbroadcall_cmd.py
--rw-r--r--   0 ta32852  (6769229) ROSWELL\Domain Users (735121457)     3712 2023-05-12 19:42:10.000000 MACS2-2.2.8/MACS2/bdgcmp_cmd.py
--rw-r--r--   0 ta32852  (6769229) ROSWELL\Domain Users (735121457)     4318 2023-05-12 19:42:10.000000 MACS2-2.2.8/MACS2/bdgdiff_cmd.py
--rw-r--r--   0 ta32852  (6769229) ROSWELL\Domain Users (735121457)     2388 2023-05-12 19:42:10.000000 MACS2-2.2.8/MACS2/bdgopt_cmd.py
--rw-r--r--   0 ta32852  (6769229) ROSWELL\Domain Users (735121457)     2696 2023-05-12 19:42:10.000000 MACS2-2.2.8/MACS2/bdgpeakcall_cmd.py
--rw-r--r--   0 ta32852  (6769229) ROSWELL\Domain Users (735121457)    13945 2023-05-12 19:42:10.000000 MACS2-2.2.8/MACS2/cPosValCalculation.c
--rw-r--r--   0 ta32852  (6769229) ROSWELL\Domain Users (735121457)     1785 2023-05-12 19:42:10.000000 MACS2-2.2.8/MACS2/cPosValCalculation.h
--rw-r--r--   0 ta32852  (6769229) ROSWELL\Domain Users (735121457)     1157 2023-05-12 19:42:10.000000 MACS2-2.2.8/MACS2/cPosValCalculation.pxd
--rw-r--r--   0 ta32852  (6769229) ROSWELL\Domain Users (735121457)    19674 2023-05-12 19:42:10.000000 MACS2-2.2.8/MACS2/callpeak_cmd.py
--rw-r--r--   0 ta32852  (6769229) ROSWELL\Domain Users (735121457)     1944 2023-05-12 19:42:10.000000 MACS2-2.2.8/MACS2/cmbreps_cmd.py
--rw-r--r--   0 ta32852  (6769229) ROSWELL\Domain Users (735121457)     9715 2023-05-12 19:42:10.000000 MACS2-2.2.8/MACS2/diffpeak_cmd.py
--rw-r--r--   0 ta32852  (6769229) ROSWELL\Domain Users (735121457)     4583 2023-05-12 19:42:10.000000 MACS2-2.2.8/MACS2/filterdup_cmd.py
--rw-r--r--   0 ta32852  (6769229) ROSWELL\Domain Users (735121457)    21042 2023-05-12 19:42:10.000000 MACS2-2.2.8/MACS2/khash.h
--rw-r--r--   0 ta32852  (6769229) ROSWELL\Domain Users (735121457)     3199 2023-05-12 19:42:10.000000 MACS2-2.2.8/MACS2/khash.pxd
--rw-r--r--   0 ta32852  (6769229) ROSWELL\Domain Users (735121457)     3964 2023-05-12 19:42:10.000000 MACS2-2.2.8/MACS2/pileup_cmd.py
--rw-r--r--   0 ta32852  (6769229) ROSWELL\Domain Users (735121457)     3178 2023-05-12 19:42:10.000000 MACS2-2.2.8/MACS2/predictd_cmd.py
--rw-r--r--   0 ta32852  (6769229) ROSWELL\Domain Users (735121457)     3888 2023-05-12 19:42:10.000000 MACS2-2.2.8/MACS2/randsample_cmd.py
--rw-r--r--   0 ta32852  (6769229) ROSWELL\Domain Users (735121457)     6845 2023-05-12 19:42:10.000000 MACS2-2.2.8/MACS2/refinepeak_cmd.py
-drwxr-xr-x   0 ta32852  (6769229) ROSWELL\Domain Users (735121457)        0 2023-05-15 14:09:33.315621 MACS2-2.2.8/MACS2.egg-info/
--rw-r--r--   0 ta32852  (6769229) ROSWELL\Domain Users (735121457)    26018 2023-05-15 14:09:32.000000 MACS2-2.2.8/MACS2.egg-info/PKG-INFO
--rw-r--r--   0 ta32852  (6769229) ROSWELL\Domain Users (735121457)     1080 2023-05-15 14:09:33.000000 MACS2-2.2.8/MACS2.egg-info/SOURCES.txt
--rw-r--r--   0 ta32852  (6769229) ROSWELL\Domain Users (735121457)        1 2023-05-15 14:09:32.000000 MACS2-2.2.8/MACS2.egg-info/dependency_links.txt
--rw-r--r--   0 ta32852  (6769229) ROSWELL\Domain Users (735121457)       12 2023-05-15 14:09:33.000000 MACS2-2.2.8/MACS2.egg-info/requires.txt
--rw-r--r--   0 ta32852  (6769229) ROSWELL\Domain Users (735121457)        6 2023-05-15 14:09:33.000000 MACS2-2.2.8/MACS2.egg-info/top_level.txt
--rw-r--r--   0 ta32852  (6769229) ROSWELL\Domain Users (735121457)      223 2023-05-12 19:42:10.000000 MACS2-2.2.8/MANIFEST.in
--rw-r--r--   0 ta32852  (6769229) ROSWELL\Domain Users (735121457)    26018 2023-05-15 14:09:33.322556 MACS2-2.2.8/PKG-INFO
--rw-r--r--   0 ta32852  (6769229) ROSWELL\Domain Users (735121457)    25022 2023-05-12 20:00:48.000000 MACS2-2.2.8/README.md
-drwxr-xr-x   0 ta32852  (6769229) ROSWELL\Domain Users (735121457)        0 2023-05-15 14:09:33.321997 MACS2-2.2.8/bin/
--rw-r--r--   0 ta32852  (6769229) ROSWELL\Domain Users (735121457)    67799 2023-05-12 19:42:10.000000 MACS2-2.2.8/bin/macs2
--rw-r--r--   0 ta32852  (6769229) ROSWELL\Domain Users (735121457)       96 2023-05-12 19:42:10.000000 MACS2-2.2.8/pyproject.toml
--rw-r--r--   0 ta32852  (6769229) ROSWELL\Domain Users (735121457)       51 2023-05-15 14:09:33.323033 MACS2-2.2.8/setup.cfg
--rw-r--r--   0 ta32852  (6769229) ROSWELL\Domain Users (735121457)     5484 2023-05-12 19:58:40.000000 MACS2-2.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:00:17.698569 MACS2-2.2.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    80507 2023-07-21 13:59:50.000000 MACS2-2.2.9/ChangeLog
+-rw-r--r--   0 runner    (1001) docker     (123)     4704 2023-07-21 13:59:50.000000 MACS2-2.2.9/INSTALL.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-07-21 13:59:50.000000 MACS2-2.2.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:00:17.682568 MACS2-2.2.9/MACS2/
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-07-21 13:59:50.000000 MACS2-2.2.9/MACS2/Constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:00:17.698569 MACS2-2.2.9/MACS2/IO/
+-rw-r--r--   0 runner    (1001) docker     (123)  1186051 2023-07-21 14:00:10.000000 MACS2-2.2.9/MACS2/IO/BedGraph.c
+-rw-r--r--   0 runner    (1001) docker     (123)    43892 2023-07-21 13:59:50.000000 MACS2-2.2.9/MACS2/IO/BedGraph.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)   312644 2023-07-21 14:00:10.000000 MACS2-2.2.9/MACS2/IO/BedGraphIO.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-07-21 13:59:50.000000 MACS2-2.2.9/MACS2/IO/BedGraphIO.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)  1638518 2023-07-21 14:00:11.000000 MACS2-2.2.9/MACS2/IO/CallPeakUnit.c
+-rw-r--r--   0 runner    (1001) docker     (123)    83101 2023-07-21 13:59:50.000000 MACS2-2.2.9/MACS2/IO/CallPeakUnit.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)  1582530 2023-07-21 13:59:50.000000 MACS2-2.2.9/MACS2/IO/CallPeakUnitPrecompiled.c
+-rw-r--r--   0 runner    (1001) docker     (123)  1213319 2023-07-21 14:00:12.000000 MACS2-2.2.9/MACS2/IO/FixWidthTrack.c
+-rw-r--r--   0 runner    (1001) docker     (123)    37584 2023-07-21 13:59:50.000000 MACS2-2.2.9/MACS2/IO/FixWidthTrack.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)   958410 2023-07-21 14:00:12.000000 MACS2-2.2.9/MACS2/IO/PairedEndTrack.c
+-rw-r--r--   0 runner    (1001) docker     (123)    23052 2023-07-21 13:59:50.000000 MACS2-2.2.9/MACS2/IO/PairedEndTrack.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)  1766592 2023-07-21 14:00:13.000000 MACS2-2.2.9/MACS2/IO/Parser.c
+-rw-r--r--   0 runner    (1001) docker     (123)    51333 2023-07-21 13:59:50.000000 MACS2-2.2.9/MACS2/IO/Parser.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)  1478779 2023-07-21 14:00:14.000000 MACS2-2.2.9/MACS2/IO/PeakIO.c
+-rw-r--r--   0 runner    (1001) docker     (123)    51188 2023-07-21 13:59:50.000000 MACS2-2.2.9/MACS2/IO/PeakIO.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)  1881571 2023-07-21 14:00:15.000000 MACS2-2.2.9/MACS2/IO/ScoreTrack.c
+-rw-r--r--   0 runner    (1001) docker     (123)    69236 2023-07-21 13:59:50.000000 MACS2-2.2.9/MACS2/IO/ScoreTrack.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 13:59:50.000000 MACS2-2.2.9/MACS2/IO/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28454 2023-07-21 13:59:50.000000 MACS2-2.2.9/MACS2/OptValidator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10842 2023-07-21 13:59:50.000000 MACS2-2.2.9/MACS2/OutputWriter.py
+-rw-r--r--   0 runner    (1001) docker     (123)   463153 2023-07-21 14:00:15.000000 MACS2-2.2.9/MACS2/PeakDetect.c
+-rw-r--r--   0 runner    (1001) docker     (123)    23222 2023-07-21 13:59:50.000000 MACS2-2.2.9/MACS2/PeakDetect.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)   905459 2023-07-21 14:00:15.000000 MACS2-2.2.9/MACS2/PeakModel.c
+-rw-r--r--   0 runner    (1001) docker     (123)    25219 2023-07-21 13:59:50.000000 MACS2-2.2.9/MACS2/PeakModel.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)   788633 2023-07-21 14:00:16.000000 MACS2-2.2.9/MACS2/Pileup.c
+-rw-r--r--   0 runner    (1001) docker     (123)    31947 2023-07-21 13:59:50.000000 MACS2-2.2.9/MACS2/Pileup.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)   599325 2023-07-21 14:00:17.000000 MACS2-2.2.9/MACS2/Prob.c
+-rw-r--r--   0 runner    (1001) docker     (123)    24670 2023-07-21 13:59:50.000000 MACS2-2.2.9/MACS2/Prob.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)   550376 2023-07-21 14:00:17.000000 MACS2-2.2.9/MACS2/Signal.c
+-rw-r--r--   0 runner    (1001) docker     (123)    13890 2023-07-21 13:59:50.000000 MACS2-2.2.9/MACS2/Signal.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-07-21 13:59:50.000000 MACS2-2.2.9/MACS2/Statistics.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-21 13:59:50.000000 MACS2-2.2.9/MACS2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-07-21 13:59:50.000000 MACS2-2.2.9/MACS2/bdgbroadcall_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-07-21 13:59:50.000000 MACS2-2.2.9/MACS2/bdgcmp_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4318 2023-07-21 13:59:50.000000 MACS2-2.2.9/MACS2/bdgdiff_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-07-21 13:59:50.000000 MACS2-2.2.9/MACS2/bdgopt_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-07-21 13:59:50.000000 MACS2-2.2.9/MACS2/bdgpeakcall_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13945 2023-07-21 13:59:50.000000 MACS2-2.2.9/MACS2/cPosValCalculation.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-07-21 13:59:50.000000 MACS2-2.2.9/MACS2/cPosValCalculation.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-07-21 13:59:50.000000 MACS2-2.2.9/MACS2/cPosValCalculation.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    19674 2023-07-21 13:59:50.000000 MACS2-2.2.9/MACS2/callpeak_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-07-21 13:59:50.000000 MACS2-2.2.9/MACS2/cmbreps_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9715 2023-07-21 13:59:50.000000 MACS2-2.2.9/MACS2/diffpeak_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4583 2023-07-21 13:59:50.000000 MACS2-2.2.9/MACS2/filterdup_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21042 2023-07-21 13:59:50.000000 MACS2-2.2.9/MACS2/khash.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3199 2023-07-21 13:59:50.000000 MACS2-2.2.9/MACS2/khash.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-07-21 13:59:50.000000 MACS2-2.2.9/MACS2/pileup_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3178 2023-07-21 13:59:50.000000 MACS2-2.2.9/MACS2/predictd_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3888 2023-07-21 13:59:50.000000 MACS2-2.2.9/MACS2/randsample_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6845 2023-07-21 13:59:50.000000 MACS2-2.2.9/MACS2/refinepeak_cmd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:00:17.682568 MACS2-2.2.9/MACS2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    26444 2023-07-21 14:00:17.000000 MACS2-2.2.9/MACS2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-07-21 14:00:17.000000 MACS2-2.2.9/MACS2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 14:00:17.000000 MACS2-2.2.9/MACS2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-21 14:00:17.000000 MACS2-2.2.9/MACS2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-21 14:00:17.000000 MACS2-2.2.9/MACS2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-21 13:59:50.000000 MACS2-2.2.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    26444 2023-07-21 14:00:17.698569 MACS2-2.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    25478 2023-07-21 13:59:50.000000 MACS2-2.2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 14:00:17.698569 MACS2-2.2.9/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)    67799 2023-07-21 13:59:50.000000 MACS2-2.2.9/bin/macs2
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-21 13:59:50.000000 MACS2-2.2.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 14:00:17.698569 MACS2-2.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-07-21 13:59:50.000000 MACS2-2.2.9/setup.py
```

### Comparing `MACS2-2.2.8/ChangeLog` & `MACS2-2.2.9/ChangeLog`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+2020-07-20  Tao Liu  <vladimir.liu@gmail.com>
+   MACS version 2.2.9
+   
+   * Bug fix:
+     
+    Cython has a major upgrade to 3.0, and can't work directly with
+    MACS2 codes, so we changed the requirement for Cython to 0.29.*.
+    
+    Python support has been changed to 3.7 to 3.11. Numpy >=0.19.
+    
+    We tested MACS2 on Mac OS12 through Github Actions as well.
+    
+    Thank @jemajet! #569
+    
 2023-05-12 Philippa Doherty <philippa.doherty@roswellpark.org>
 	MACS version 2.2.8
 
 	* Bug fix:
 
 	MACS2 typo in `setup.py`: `numpy>=>=1.17` -> `numpy>=1.17`
 	PR #543, issues #535, #541, #544
```

### Comparing `MACS2-2.2.8/INSTALL.md` & `MACS2-2.2.9/INSTALL.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 # INSTALL Guide For MACS
-Time-stamp: <2019-12-12 13:26:11 taoliu>
+Time-stamp: <2023-07-20 10:26:11 taoliu>
 
 Please check the following instructions to complete your installation.
 
 ## Prerequisites
 
-MACS v2.2.x requires Python3. We have tested MACS in Python3.6, 3.7
-and 3.8. 
+MACS v2.2.x requires Python3. We have tested MACS in Python 3.7 to
+3.11.
 
-MACS also requires [Numpy](http://www.scipy.org/Download) (>=1.17).
+MACS also requires [Numpy](http://www.scipy.org/Download) (>=1.19).
 
 GCC is required to compile `.c` codes in MACS v2 package, and python
 header files are needed. If you are using Mac OSX, I recommend you
 install Xcode; if you are using Linux, you need to make sure
 `python-dev` package is installed -- the actual package name depends
 on the Linux OS distribution, you are using.
 
-[Cython](http://cython.org/) is **NOT** required although most of MACS
-codes are written in Cython. But if you plan to generate `.c` files
-from `.pyx` by yourself, you can install Cython (>=0.29), then use
-`setup.py` script.
+[Cython](http://cython.org/) is required to translate .pyx codes to .c
+code. The version of Cython has to be >=0.29 but lower than 3.0.
+
+If you use `pip` to install MACS2, the installer script will check the
+dependencies and install them when necessary.
 
 ## Prepare a virtual Python environment 
 
 I strongly recommend installing your MACS program in a virtual
 environment, so that you have full control of your installation and
 won't mess up with your system libraries. To learn about virtual
 environment, read [this
@@ -58,45 +59,28 @@
 ## Install through Debian APT
 
 MACS is included in Debian Stretch/Buster/Unstable blessed by some
 kind of Supper Cow Powers.
 
 ## Install from source
 
-MACS uses Python's [setuptools](https://setuptools.readthedocs.io) for
-source code installations. To install a source distribution of MACS,
-unpack the distribution tarball, or clone Git repository with `git
-clone git@github.com:taoliu/MACS.git`. Go to the directory where you
-unpacked MACS, and simply run the install script:
+MACS uses `pip` for source code installations. To install a source 
+distribution of MACS, unpack the distribution tarball. Go to the 
+directory where you cloned MACS from github, and simply run the
+install command:
 
- `$ python setup.py install`
+ `$ pip install .`
 
 By default, the script will install python library and executable
 codes according to the environment. When you run the command under
-virtualenv, the script will install to the virtual environment
-instead. When you run it without virtual environment, you may need to
-be root or administrator of the machine so as to complete the
-installation. Please contact the system administrator if you want
-their help. If you need to provide a nonstandard install prefix, or
-any other nonstandard options, you can provide many command line
-options to the install script. Use the `--help` option to see a brief
-list of available options:
-
- `$ python setup.py --help`
-
-For example, if I want to install everything under my own HOME
-directory, use this command:
-
- `$ python setup.py install --prefix /home/taoliu/`
-
-As mentioned in *Prerequisites*, you don't need to install Cython in
-order to install MACS. When Cython is available, this setup script
-will regenerate C codes from Pyx codes when necessary. When Cython is
-not available, this setup script will just use the C codes included in
-the release package (or your Github clone) for installation.
+virtualenv or conda environment, the script will install to the virtual
+environment instead. When you run the command without virtual environment, 
+you may need to be root or administrator of the machine so as to 
+complete the installation. Please contact the system administrator
+if you want their help. 
 
 ## Configure environment variables
 
 *Note*, if you are using a virtual environment, you should skip this
 section since all the corresponding environment variables have been
 correctly set while you `activate` the environment.
```

### Comparing `MACS2-2.2.8/LICENSE` & `MACS2-2.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `MACS2-2.2.8/MACS2/Constants.py` & `MACS2-2.2.9/MACS2/Constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-MACS_VERSION = "2.2.8"
+MACS_VERSION = "2.2.9"
 FILTERDUP_VERSION = "1.0.0 20140616"
 RANDSAMPLE_VERSION = "1.0.0 20120703"
 MAX_PAIRNUM = 1000
 MAX_LAMBDA  = 100000
 FESTEP      = 20
 BUFFER_SIZE = 100000                   # np array will increase at step of 1 million items
```

### Comparing `MACS2-2.2.8/MACS2/IO/BedGraph.pyx` & `MACS2-2.2.9/MACS2/IO/BedGraph.pyx`

 * *Files identical despite different names*

### Comparing `MACS2-2.2.8/MACS2/IO/BedGraphIO.pyx` & `MACS2-2.2.9/MACS2/IO/BedGraphIO.pyx`

 * *Files identical despite different names*

### Comparing `MACS2-2.2.8/MACS2/IO/CallPeakUnit.pyx` & `MACS2-2.2.9/MACS2/IO/CallPeakUnit.pyx`

 * *Files identical despite different names*

### Comparing `MACS2-2.2.8/MACS2/IO/CallPeakUnitPrecompiled.c` & `MACS2-2.2.9/MACS2/IO/CallPeakUnitPrecompiled.c`

 * *Files identical despite different names*

### Comparing `MACS2-2.2.8/MACS2/IO/FixWidthTrack.pyx` & `MACS2-2.2.9/MACS2/IO/FixWidthTrack.pyx`

 * *Files identical despite different names*

### Comparing `MACS2-2.2.8/MACS2/IO/PairedEndTrack.pyx` & `MACS2-2.2.9/MACS2/IO/PairedEndTrack.pyx`

 * *Files identical despite different names*

### Comparing `MACS2-2.2.8/MACS2/IO/Parser.pyx` & `MACS2-2.2.9/MACS2/IO/Parser.pyx`

 * *Files identical despite different names*

### Comparing `MACS2-2.2.8/MACS2/IO/PeakIO.pyx` & `MACS2-2.2.9/MACS2/IO/PeakIO.pyx`

 * *Files identical despite different names*

### Comparing `MACS2-2.2.8/MACS2/IO/ScoreTrack.pyx` & `MACS2-2.2.9/MACS2/IO/ScoreTrack.pyx`

 * *Files identical despite different names*

### Comparing `MACS2-2.2.8/MACS2/OptValidator.py` & `MACS2-2.2.9/MACS2/OptValidator.py`

 * *Files identical despite different names*

### Comparing `MACS2-2.2.8/MACS2/OutputWriter.py` & `MACS2-2.2.9/MACS2/OutputWriter.py`

 * *Files identical despite different names*

### Comparing `MACS2-2.2.8/MACS2/PeakDetect.pyx` & `MACS2-2.2.9/MACS2/PeakDetect.pyx`

 * *Files identical despite different names*

### Comparing `MACS2-2.2.8/MACS2/PeakModel.pyx` & `MACS2-2.2.9/MACS2/PeakModel.pyx`

 * *Files identical despite different names*

### Comparing `MACS2-2.2.8/MACS2/Pileup.pyx` & `MACS2-2.2.9/MACS2/Pileup.pyx`

 * *Files identical despite different names*

### Comparing `MACS2-2.2.8/MACS2/Prob.pyx` & `MACS2-2.2.9/MACS2/Prob.pyx`

 * *Files identical despite different names*

### Comparing `MACS2-2.2.8/MACS2/Signal.pyx` & `MACS2-2.2.9/MACS2/Signal.pyx`

 * *Files identical despite different names*

### Comparing `MACS2-2.2.8/MACS2/Statistics.pyx` & `MACS2-2.2.9/MACS2/Statistics.pyx`

 * *Files identical despite different names*

### Comparing `MACS2-2.2.8/MACS2/bdgbroadcall_cmd.py` & `MACS2-2.2.9/MACS2/bdgbroadcall_cmd.py`

 * *Files identical despite different names*

### Comparing `MACS2-2.2.8/MACS2/bdgcmp_cmd.py` & `MACS2-2.2.9/MACS2/bdgcmp_cmd.py`

 * *Files identical despite different names*

### Comparing `MACS2-2.2.8/MACS2/bdgdiff_cmd.py` & `MACS2-2.2.9/MACS2/bdgdiff_cmd.py`

 * *Files identical despite different names*

### Comparing `MACS2-2.2.8/MACS2/bdgopt_cmd.py` & `MACS2-2.2.9/MACS2/bdgopt_cmd.py`

 * *Files identical despite different names*

### Comparing `MACS2-2.2.8/MACS2/bdgpeakcall_cmd.py` & `MACS2-2.2.9/MACS2/bdgpeakcall_cmd.py`

 * *Files identical despite different names*

### Comparing `MACS2-2.2.8/MACS2/cPosValCalculation.c` & `MACS2-2.2.9/MACS2/cPosValCalculation.c`

 * *Files identical despite different names*

### Comparing `MACS2-2.2.8/MACS2/cPosValCalculation.h` & `MACS2-2.2.9/MACS2/cPosValCalculation.h`

 * *Files identical despite different names*

### Comparing `MACS2-2.2.8/MACS2/cPosValCalculation.pxd` & `MACS2-2.2.9/MACS2/cPosValCalculation.pxd`

 * *Files identical despite different names*

### Comparing `MACS2-2.2.8/MACS2/callpeak_cmd.py` & `MACS2-2.2.9/MACS2/callpeak_cmd.py`

 * *Files identical despite different names*

### Comparing `MACS2-2.2.8/MACS2/cmbreps_cmd.py` & `MACS2-2.2.9/MACS2/cmbreps_cmd.py`

 * *Files identical despite different names*

### Comparing `MACS2-2.2.8/MACS2/diffpeak_cmd.py` & `MACS2-2.2.9/MACS2/diffpeak_cmd.py`

 * *Files identical despite different names*

### Comparing `MACS2-2.2.8/MACS2/filterdup_cmd.py` & `MACS2-2.2.9/MACS2/filterdup_cmd.py`

 * *Files identical despite different names*

### Comparing `MACS2-2.2.8/MACS2/khash.h` & `MACS2-2.2.9/MACS2/khash.h`

 * *Files identical despite different names*

### Comparing `MACS2-2.2.8/MACS2/khash.pxd` & `MACS2-2.2.9/MACS2/khash.pxd`

 * *Files identical despite different names*

### Comparing `MACS2-2.2.8/MACS2/pileup_cmd.py` & `MACS2-2.2.9/MACS2/pileup_cmd.py`

 * *Files identical despite different names*

### Comparing `MACS2-2.2.8/MACS2/predictd_cmd.py` & `MACS2-2.2.9/MACS2/predictd_cmd.py`

 * *Files identical despite different names*

### Comparing `MACS2-2.2.8/MACS2/randsample_cmd.py` & `MACS2-2.2.9/MACS2/randsample_cmd.py`

 * *Files identical despite different names*

### Comparing `MACS2-2.2.8/MACS2/refinepeak_cmd.py` & `MACS2-2.2.9/MACS2/refinepeak_cmd.py`

 * *Files identical despite different names*

### Comparing `MACS2-2.2.8/MACS2.egg-info/PKG-INFO` & `MACS2-2.2.9/MACS2.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,29 @@
 Metadata-Version: 2.1
 Name: MACS2
-Version: 2.2.8
+Version: 2.2.9
 Summary: Model Based Analysis for ChIP-Seq data
-Home-page: http://github.com/taoliu/MACS/
+Home-page: http://github.com/macs3-project/MACS/
 Author: Tao Liu
 Author-email: vladimir.liu@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Cython
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # MACS: Model-based Analysis for ChIP-Seq
 
 ![Status](https://img.shields.io/pypi/status/macs2.svg) [![License](https://img.shields.io/github/license/taoliu/MACS)](https://github.com/taoliu/MACS/blob/master/LICENSE) ![Programming languages](https://img.shields.io/github/languages/top/taoliu/MACS) ![Commit activity](https://img.shields.io/github/commit-activity/m/taoliu/MACS) [![TravisCI Build Status](https://img.shields.io/travis/com/taoliu/MACS/master)](https://travis-ci.com/taoliu/MACS)
 
@@ -51,18 +49,33 @@
 position and orientation. MACS can be easily used for ChIP-Seq data
 alone, or with a control sample with the increase of
 specificity. Moreover, as a general peak-caller, MACS can also be
 applied to any "DNA enrichment assays" if the question to be asked is
 simply: *where we can find significant reads coverage than the random
 background*.
 
-## Recent Changes for MACS (2.2.8)
+*Note: new development on MACS has been moved to MACS3 repository,
+we will only fix installation issues on MACS2.*
+
+## Recent Changes for MACS (2.2.9)
+
+### 2.2.9
+    * Bug fix:
+     
+    Cython has a major upgrade to 3.0, and can't work directly with
+    MACS2 codes, so we changed the requirement for Cython to 0.29.*.
+    
+    Python support has been changed to 3.7 to 3.11. Numpy >=0.19.
+    
+    We tested MACS2 on Mac OS12 through Github Actions as well.
+    
+    Thank @jemajet! #569
 
 ### 2.2.8
-   * Bug fix:
+    * Bug fix:
 
 	MACS2 typo in 'setup.py': 'numpy>=>=1.17' -> 'numpy>=1.17'
 	PR #543, issues #535, #541, #544
 
 	Now test on and support Python 3.6/3.7/3.8/3.9/3.10/3.11
 
 ### 2.2.7.1
@@ -154,15 +167,15 @@
 
 Example for regular peak calling: `macs2 callpeak -t ChIP.bam -c
 Control.bam -f BAM -g hs -n test -B -q 0.01`
 
 Example for broad peak calling: `macs2 callpeak -t ChIP.bam -c
 Control.bam --broad -g hs --broad-cutoff 0.1`
 
-There are twelve functions available in MAC2S serving as sub-commands.
+There are twelve functions available in MACS2 serving as sub-commands.
 
 Subcommand | Description
 -----------|----------
 `callpeak` | Main MACS2 Function to call peaks from alignment results.
 `bdgpeakcall` | Call peaks from bedGraph output.
 `bdgbroadcall` | Call broad peaks from bedGraph output.
 `bdgcmp` | Comparing two signal tracks in bedGraph format.
@@ -581,9 +594,7 @@
    treatment 1. It will output consistent and unique sites according
    to parameter settings for minimum length, the maximum gap and
    cutoff.
 
 4. You can combine subcommands to do a step-by-step peak calling. Read
    detail at [MACS2
    wikipage](https://github.com/taoliu/MACS/wiki/Advanced%3A-Call-peaks-using-MACS2-subcommands)
-
-
```

### Comparing `MACS2-2.2.8/MACS2.egg-info/SOURCES.txt` & `MACS2-2.2.9/MACS2.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 ChangeLog
 INSTALL.md
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
-setup.cfg
 setup.py
 MACS2/Constants.py
 MACS2/OptValidator.py
 MACS2/OutputWriter.py
+MACS2/PeakDetect.c
 MACS2/PeakDetect.pyx
+MACS2/PeakModel.c
 MACS2/PeakModel.pyx
+MACS2/Pileup.c
 MACS2/Pileup.pyx
+MACS2/Prob.c
 MACS2/Prob.pyx
+MACS2/Signal.c
 MACS2/Signal.pyx
 MACS2/Statistics.pyx
 MACS2/__init__.py
 MACS2/bdgbroadcall_cmd.py
 MACS2/bdgcmp_cmd.py
 MACS2/bdgdiff_cmd.py
 MACS2/bdgopt_cmd.py
@@ -35,18 +39,26 @@
 MACS2/randsample_cmd.py
 MACS2/refinepeak_cmd.py
 MACS2.egg-info/PKG-INFO
 MACS2.egg-info/SOURCES.txt
 MACS2.egg-info/dependency_links.txt
 MACS2.egg-info/requires.txt
 MACS2.egg-info/top_level.txt
+MACS2/IO/BedGraph.c
 MACS2/IO/BedGraph.pyx
+MACS2/IO/BedGraphIO.c
 MACS2/IO/BedGraphIO.pyx
+MACS2/IO/CallPeakUnit.c
 MACS2/IO/CallPeakUnit.pyx
 MACS2/IO/CallPeakUnitPrecompiled.c
+MACS2/IO/FixWidthTrack.c
 MACS2/IO/FixWidthTrack.pyx
+MACS2/IO/PairedEndTrack.c
 MACS2/IO/PairedEndTrack.pyx
+MACS2/IO/Parser.c
 MACS2/IO/Parser.pyx
+MACS2/IO/PeakIO.c
 MACS2/IO/PeakIO.pyx
+MACS2/IO/ScoreTrack.c
 MACS2/IO/ScoreTrack.pyx
 MACS2/IO/__init__.py
 bin/macs2
```

### Comparing `MACS2-2.2.8/PKG-INFO` & `MACS2-2.2.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,29 @@
 Metadata-Version: 2.1
 Name: MACS2
-Version: 2.2.8
+Version: 2.2.9
 Summary: Model Based Analysis for ChIP-Seq data
-Home-page: http://github.com/taoliu/MACS/
+Home-page: http://github.com/macs3-project/MACS/
 Author: Tao Liu
 Author-email: vladimir.liu@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Cython
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # MACS: Model-based Analysis for ChIP-Seq
 
 ![Status](https://img.shields.io/pypi/status/macs2.svg) [![License](https://img.shields.io/github/license/taoliu/MACS)](https://github.com/taoliu/MACS/blob/master/LICENSE) ![Programming languages](https://img.shields.io/github/languages/top/taoliu/MACS) ![Commit activity](https://img.shields.io/github/commit-activity/m/taoliu/MACS) [![TravisCI Build Status](https://img.shields.io/travis/com/taoliu/MACS/master)](https://travis-ci.com/taoliu/MACS)
 
@@ -51,18 +49,33 @@
 position and orientation. MACS can be easily used for ChIP-Seq data
 alone, or with a control sample with the increase of
 specificity. Moreover, as a general peak-caller, MACS can also be
 applied to any "DNA enrichment assays" if the question to be asked is
 simply: *where we can find significant reads coverage than the random
 background*.
 
-## Recent Changes for MACS (2.2.8)
+*Note: new development on MACS has been moved to MACS3 repository,
+we will only fix installation issues on MACS2.*
+
+## Recent Changes for MACS (2.2.9)
+
+### 2.2.9
+    * Bug fix:
+     
+    Cython has a major upgrade to 3.0, and can't work directly with
+    MACS2 codes, so we changed the requirement for Cython to 0.29.*.
+    
+    Python support has been changed to 3.7 to 3.11. Numpy >=0.19.
+    
+    We tested MACS2 on Mac OS12 through Github Actions as well.
+    
+    Thank @jemajet! #569
 
 ### 2.2.8
-   * Bug fix:
+    * Bug fix:
 
 	MACS2 typo in 'setup.py': 'numpy>=>=1.17' -> 'numpy>=1.17'
 	PR #543, issues #535, #541, #544
 
 	Now test on and support Python 3.6/3.7/3.8/3.9/3.10/3.11
 
 ### 2.2.7.1
@@ -154,15 +167,15 @@
 
 Example for regular peak calling: `macs2 callpeak -t ChIP.bam -c
 Control.bam -f BAM -g hs -n test -B -q 0.01`
 
 Example for broad peak calling: `macs2 callpeak -t ChIP.bam -c
 Control.bam --broad -g hs --broad-cutoff 0.1`
 
-There are twelve functions available in MAC2S serving as sub-commands.
+There are twelve functions available in MACS2 serving as sub-commands.
 
 Subcommand | Description
 -----------|----------
 `callpeak` | Main MACS2 Function to call peaks from alignment results.
 `bdgpeakcall` | Call peaks from bedGraph output.
 `bdgbroadcall` | Call broad peaks from bedGraph output.
 `bdgcmp` | Comparing two signal tracks in bedGraph format.
@@ -581,9 +594,7 @@
    treatment 1. It will output consistent and unique sites according
    to parameter settings for minimum length, the maximum gap and
    cutoff.
 
 4. You can combine subcommands to do a step-by-step peak calling. Read
    detail at [MACS2
    wikipage](https://github.com/taoliu/MACS/wiki/Advanced%3A-Call-peaks-using-MACS2-subcommands)
-
-
```

### Comparing `MACS2-2.2.8/README.md` & `MACS2-2.2.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -24,18 +24,33 @@
 position and orientation. MACS can be easily used for ChIP-Seq data
 alone, or with a control sample with the increase of
 specificity. Moreover, as a general peak-caller, MACS can also be
 applied to any "DNA enrichment assays" if the question to be asked is
 simply: *where we can find significant reads coverage than the random
 background*.
 
-## Recent Changes for MACS (2.2.8)
+*Note: new development on MACS has been moved to MACS3 repository,
+we will only fix installation issues on MACS2.*
+
+## Recent Changes for MACS (2.2.9)
+
+### 2.2.9
+    * Bug fix:
+     
+    Cython has a major upgrade to 3.0, and can't work directly with
+    MACS2 codes, so we changed the requirement for Cython to 0.29.*.
+    
+    Python support has been changed to 3.7 to 3.11. Numpy >=0.19.
+    
+    We tested MACS2 on Mac OS12 through Github Actions as well.
+    
+    Thank @jemajet! #569
 
 ### 2.2.8
-   * Bug fix:
+    * Bug fix:
 
 	MACS2 typo in 'setup.py': 'numpy>=>=1.17' -> 'numpy>=1.17'
 	PR #543, issues #535, #541, #544
 
 	Now test on and support Python 3.6/3.7/3.8/3.9/3.10/3.11
 
 ### 2.2.7.1
@@ -127,15 +142,15 @@
 
 Example for regular peak calling: `macs2 callpeak -t ChIP.bam -c
 Control.bam -f BAM -g hs -n test -B -q 0.01`
 
 Example for broad peak calling: `macs2 callpeak -t ChIP.bam -c
 Control.bam --broad -g hs --broad-cutoff 0.1`
 
-There are twelve functions available in MAC2S serving as sub-commands.
+There are twelve functions available in MACS2 serving as sub-commands.
 
 Subcommand | Description
 -----------|----------
 `callpeak` | Main MACS2 Function to call peaks from alignment results.
 `bdgpeakcall` | Call peaks from bedGraph output.
 `bdgbroadcall` | Call broad peaks from bedGraph output.
 `bdgcmp` | Comparing two signal tracks in bedGraph format.
```

### Comparing `MACS2-2.2.8/bin/macs2` & `MACS2-2.2.9/bin/macs2`

 * *Files identical despite different names*

### Comparing `MACS2-2.2.8/setup.py` & `MACS2-2.2.9/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,104 +1,102 @@
 #!/usr/bin/env python3
-# Time-stamp: <2023-05-12 15:58:40 Tao Liu>
+# Time-stamp: <2023-07-20 09:58:20 Tao Liu>
 
 """Description: 
 
 Setup script for MACS -- Model Based Analysis for ChIP-Seq data
 
 This code is free software; you can redistribute it and/or modify it
 under the terms of the BSD License (see the file LICENSE included with
 the distribution).
 """
 
 import sys
 import os
+import re
 from setuptools import setup, Extension
-from distutils.version import LooseVersion
+from Cython.Build import cythonize
 import subprocess
+import sysconfig
+import numpy
 
-numpy_requires = '>=1.17'
-install_requires = [f"numpy{numpy_requires}",]
+install_requires = [ "numpy>=1.19",
+                     "cykhash>=2.0,<3.0",
+                     "Cython~=0.29" ]
+
+exec(open("MACS2/Constants.py").read())
+
+# classifiers
+classifiers =[\
+              'Development Status :: 5 - Production/Stable',
+              'Environment :: Console',
+              'Intended Audience :: Developers',
+              'Intended Audience :: Science/Research',              
+              'License :: OSI Approved :: BSD License',
+              'Operating System :: MacOS :: MacOS X',
+              'Operating System :: POSIX',
+              'Topic :: Scientific/Engineering :: Bio-Informatics',
+              'Programming Language :: Python :: 3.7',
+              'Programming Language :: Python :: 3.8',              
+              'Programming Language :: Python :: 3.9',
+              'Programming Language :: Python :: 3.10',
+              'Programming Language :: Python :: 3.11',              	      
+              'Programming Language :: Cython',
+              ]
+
+install_requires = [ "numpy>=1.19",
+                     "Cython~=0.29" ]
+
+tests_requires = [ 'pytest' ]
 
 def main():
-    if sys.version_info < (3,6):
-        sys.stderr.write("CRITICAL: Python version must >= 3.6!\n")
+    if sys.version_info < (3,7):
+        sys.stderr.write("CRITICAL: Python version must >= 3.7!\n")
         sys.exit(1)
-    cwd = os.path.abspath(os.path.dirname(__file__))
-
-    # install required numpy
-    p = subprocess.call([sys.executable, "-m", 'pip', 'install', f'numpy{numpy_requires}'],cwd=cwd)
-    if p != 0:
-        # Could be due to a too old pip version and build isolation, check that
-        try:
-            # Note, pip may not be installed or not have been used
-            import pip
-            if LooseVersion(pip.__version__) < LooseVersion('18.0.0'):
-                raise RuntimeError("Installing requirements failed. Possibly due "
-                                   "to `pip` being too old, found version {}, "
-                                   "needed is >= 18.0.0.".format(pip.__version__))
-            else:
-                raise RuntimeError("Installing requirements failed!")
-        except ImportError:
-            raise RuntimeError("Installing requirement failed! `pip` has to be installed!")
         
-    from numpy import get_include as numpy_get_include
-    numpy_include_dir = [numpy_get_include()]
+    # NumPy include dir
+    numpy_include_dir = [ numpy.get_include() ]
         
     # I intend to use -Ofast, however if gcc version < 4.6, this option is unavailable so...
     extra_c_args = ["-w","-O3","-ffast-math","-g0"] # for C, -Ofast implies -O3 and -ffast-math
 
-    ext_modules = [Extension("MACS2.Prob", ["MACS2/Prob.pyx"], libraries=["m"], include_dirs=numpy_include_dir, extra_compile_args=extra_c_args ),
+    ext_modules = [ \
+                   Extension("MACS2.Prob", ["MACS2/Prob.pyx"], libraries=["m"], include_dirs=numpy_include_dir, extra_compile_args=extra_c_args ),
                    Extension("MACS2.IO.Parser",["MACS2/IO/Parser.pyx"], include_dirs=numpy_include_dir, extra_compile_args=extra_c_args),
                    Extension("MACS2.Pileup", ["MACS2/Pileup.pyx","MACS2/cPosValCalculation.c"], include_dirs=numpy_include_dir, extra_compile_args=extra_c_args ),
                    Extension("MACS2.PeakModel", ["MACS2/PeakModel.pyx"], include_dirs=numpy_include_dir, extra_compile_args=extra_c_args),
                    Extension("MACS2.PeakDetect", ["MACS2/PeakDetect.pyx"], extra_compile_args=extra_c_args),
                    Extension("MACS2.Signal", ["MACS2/Signal.pyx"], include_dirs=numpy_include_dir, extra_compile_args=extra_c_args),
                    Extension("MACS2.IO.PeakIO", ["MACS2/IO/PeakIO.pyx"], extra_compile_args=extra_c_args),
                    Extension("MACS2.IO.BedGraphIO", ["MACS2/IO/BedGraphIO.pyx"], extra_compile_args=extra_c_args),                   
                    Extension("MACS2.IO.FixWidthTrack", ["MACS2/IO/FixWidthTrack.pyx"], include_dirs=numpy_include_dir, extra_compile_args=extra_c_args),
                    Extension("MACS2.IO.PairedEndTrack", ["MACS2/IO/PairedEndTrack.pyx"], include_dirs=numpy_include_dir, extra_compile_args=extra_c_args),
                    Extension("MACS2.IO.BedGraph", ["MACS2/IO/BedGraph.pyx"], libraries=["m"], extra_compile_args=extra_c_args),
                    Extension("MACS2.IO.ScoreTrack", ["MACS2/IO/ScoreTrack.pyx"], include_dirs=numpy_include_dir, extra_compile_args=extra_c_args ),
                    Extension("MACS2.IO.CallPeakUnit", ["MACS2/IO/CallPeakUnit.pyx"], include_dirs=numpy_include_dir, extra_compile_args=extra_c_args),
-                   #Extension("MACS2.Statistics", ["MACS2/Statistics.pyx"], libraries=["m"], include_dirs=["MACS2/",numpy_get_include()], extra_compile_args=extra_c_args),
-    ]
+                  ]
 
     with open("README.md", "r") as fh:
         long_description = fh.read()
         
     setup(name="MACS2",
-          version="2.2.8",
+          version=MACS_VERSION,
           description="Model Based Analysis for ChIP-Seq data",
           long_description = long_description,
           long_description_content_type="text/markdown",
           author='Tao Liu',
           author_email='vladimir.liu@gmail.com',
-          url='http://github.com/taoliu/MACS/',
+          url = 'http://github.com/macs3-project/MACS/',
           package_dir={'MACS2' : 'MACS2'},
           packages=['MACS2', 'MACS2.IO'],
           package_data={'MACS2':['*.pxd']},
           scripts=['bin/macs2', ],
-          classifiers=[
-              'Development Status :: 5 - Production/Stable',
-              'Environment :: Console',
-              'Intended Audience :: Developers',
-              'Intended Audience :: Science/Research',              
-              'License :: OSI Approved :: BSD License',
-              'Operating System :: MacOS :: MacOS X',
-              'Operating System :: POSIX',
-              'Topic :: Scientific/Engineering :: Bio-Informatics',
-              'Programming Language :: Python :: 3.6',
-              'Programming Language :: Python :: 3.7',
-              'Programming Language :: Python :: 3.9',
-              'Programming Language :: Python :: 3.10',
-              'Programming Language :: Python :: 3.11',              	      
-              'Programming Language :: Cython',
-              ],
+          classifiers=classifiers,
           install_requires=install_requires,
-          setup_requires=install_requires,          
-          python_requires='>=3.6',
-          ext_modules = ext_modules
+          setup_requires=install_requires,    
+          tests_require = tests_requires,
+          python_requires='>=3.7',
+          ext_modules = cythonize( ext_modules ),
           )
 
 if __name__ == '__main__':
     main()
```

