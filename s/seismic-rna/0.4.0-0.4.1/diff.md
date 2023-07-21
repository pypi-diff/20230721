# Comparing `tmp/seismic-rna-0.4.0.tar.gz` & `tmp/seismic-rna-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seismic-rna-0.4.0.tar", last modified: Thu Jul 20 03:05:22 2023, max compression
+gzip compressed data, was "seismic-rna-0.4.1.tar", last modified: Fri Jul 21 02:50:00 2023, max compression
```

## Comparing `seismic-rna-0.4.0.tar` & `seismic-rna-0.4.1.tar`

### file list

```diff
@@ -1,118 +1,118 @@
-drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-20 03:05:22.202409 seismic-rna-0.4.0/
--rw-r--r--   0 mfa        (503) staff       (20)    35150 2023-06-29 02:33:57.000000 seismic-rna-0.4.0/LICENSE
--rw-r--r--   0 mfa        (503) staff       (20)     1910 2023-07-20 03:05:22.201989 seismic-rna-0.4.0/PKG-INFO
--rw-r--r--   0 mfa        (503) staff       (20)     1347 2023-07-19 21:38:18.000000 seismic-rna-0.4.0/README.md
--rw-r--r--   0 mfa        (503) staff       (20)     1037 2023-07-20 02:41:04.000000 seismic-rna-0.4.0/pyproject.toml
--rw-r--r--   0 mfa        (503) staff       (20)       38 2023-07-20 03:05:22.202533 seismic-rna-0.4.0/setup.cfg
-drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-20 03:05:22.092853 seismic-rna-0.4.0/src/
-drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-20 03:05:22.105316 seismic-rna-0.4.0/src/seismic_rna.egg-info/
--rw-r--r--   0 mfa        (503) staff       (20)     1910 2023-07-20 03:05:22.000000 seismic-rna-0.4.0/src/seismic_rna.egg-info/PKG-INFO
--rw-r--r--   0 mfa        (503) staff       (20)     3039 2023-07-20 03:05:22.000000 seismic-rna-0.4.0/src/seismic_rna.egg-info/SOURCES.txt
--rw-r--r--   0 mfa        (503) staff       (20)        1 2023-07-20 03:05:22.000000 seismic-rna-0.4.0/src/seismic_rna.egg-info/dependency_links.txt
--rw-r--r--   0 mfa        (503) staff       (20)       53 2023-07-20 03:05:22.000000 seismic-rna-0.4.0/src/seismic_rna.egg-info/entry_points.txt
--rw-r--r--   0 mfa        (503) staff       (20)      176 2023-07-20 03:05:22.000000 seismic-rna-0.4.0/src/seismic_rna.egg-info/requires.txt
--rw-r--r--   0 mfa        (503) staff       (20)       11 2023-07-20 03:05:22.000000 seismic-rna-0.4.0/src/seismic_rna.egg-info/top_level.txt
-drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-20 03:05:22.108263 seismic-rna-0.4.0/src/seismicrna/
--rw-r--r--   0 mfa        (503) staff       (20)      201 2023-07-16 01:27:23.000000 seismic-rna-0.4.0/src/seismicrna/__init__.py
-drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-20 03:05:22.114635 seismic-rna-0.4.0/src/seismicrna/align/
--rw-r--r--   0 mfa        (503) staff       (20)       35 2023-06-29 02:17:49.000000 seismic-rna-0.4.0/src/seismicrna/align/__init__.py
--rw-r--r--   0 mfa        (503) staff       (20)    22758 2023-07-05 00:01:54.000000 seismic-rna-0.4.0/src/seismicrna/align/fq2bam.py
--rwxr-xr-x   0 mfa        (503) staff       (20)    20020 2023-07-09 17:46:17.000000 seismic-rna-0.4.0/src/seismicrna/align/fqutil.py
--rw-r--r--   0 mfa        (503) staff       (20)     7600 2023-07-20 02:53:44.000000 seismic-rna-0.4.0/src/seismicrna/align/main.py
--rwxr-xr-x   0 mfa        (503) staff       (20)     9115 2023-06-29 02:17:49.000000 seismic-rna-0.4.0/src/seismicrna/align/strandedness.py
--rw-r--r--   0 mfa        (503) staff       (20)        0 2023-06-29 02:17:49.000000 seismic-rna-0.4.0/src/seismicrna/align/test.py
-drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-20 03:05:22.121762 seismic-rna-0.4.0/src/seismicrna/cluster/
--rw-r--r--   0 mfa        (503) staff       (20)       35 2023-06-29 02:17:49.000000 seismic-rna-0.4.0/src/seismicrna/cluster/__init__.py
--rw-r--r--   0 mfa        (503) staff       (20)    13197 2023-07-15 21:12:26.000000 seismic-rna-0.4.0/src/seismicrna/cluster/compare.py
--rw-r--r--   0 mfa        (503) staff       (20)    18681 2023-06-29 02:17:49.000000 seismic-rna-0.4.0/src/seismicrna/cluster/em.py
--rw-r--r--   0 mfa        (503) staff       (20)     6262 2023-06-29 02:17:49.000000 seismic-rna-0.4.0/src/seismicrna/cluster/krun.py
--rw-r--r--   0 mfa        (503) staff       (20)     4209 2023-06-29 02:17:49.000000 seismic-rna-0.4.0/src/seismicrna/cluster/load.py
--rw-r--r--   0 mfa        (503) staff       (20)     2464 2023-07-16 00:26:28.000000 seismic-rna-0.4.0/src/seismicrna/cluster/main.py
--rw-r--r--   0 mfa        (503) staff       (20)     1264 2023-07-15 00:22:05.000000 seismic-rna-0.4.0/src/seismicrna/cluster/names.py
--rw-r--r--   0 mfa        (503) staff       (20)     2862 2023-06-29 02:17:49.000000 seismic-rna-0.4.0/src/seismicrna/cluster/report.py
--rw-r--r--   0 mfa        (503) staff       (20)     4981 2023-06-29 02:17:49.000000 seismic-rna-0.4.0/src/seismicrna/cluster/write.py
-drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-20 03:05:22.156614 seismic-rna-0.4.0/src/seismicrna/core/
--rw-r--r--   0 mfa        (503) staff       (20)        0 2023-06-29 02:17:49.000000 seismic-rna-0.4.0/src/seismicrna/core/__init__.py
--rw-r--r--   0 mfa        (503) staff       (20)    15704 2023-06-29 18:01:10.000000 seismic-rna-0.4.0/src/seismicrna/core/bitcall.py
--rw-r--r--   0 mfa        (503) staff       (20)    19264 2023-07-07 22:07:51.000000 seismic-rna-0.4.0/src/seismicrna/core/bitvect.py
--rw-r--r--   0 mfa        (503) staff       (20)    18165 2023-07-19 23:10:51.000000 seismic-rna-0.4.0/src/seismicrna/core/cli.py
--rw-r--r--   0 mfa        (503) staff       (20)     1120 2023-06-29 21:48:51.000000 seismic-rna-0.4.0/src/seismicrna/core/depend.py
--rw-r--r--   0 mfa        (503) staff       (20)     6844 2023-06-29 02:17:49.000000 seismic-rna-0.4.0/src/seismicrna/core/docdef.py
--rw-r--r--   0 mfa        (503) staff       (20)     2201 2023-06-29 02:17:49.000000 seismic-rna-0.4.0/src/seismicrna/core/docstring.py
--rw-r--r--   0 mfa        (503) staff       (20)     1972 2023-06-29 02:17:49.000000 seismic-rna-0.4.0/src/seismicrna/core/dump.py
--rw-r--r--   0 mfa        (503) staff       (20)      628 2023-06-29 02:17:49.000000 seismic-rna-0.4.0/src/seismicrna/core/files.py
--rw-r--r--   0 mfa        (503) staff       (20)     7933 2023-07-07 22:47:51.000000 seismic-rna-0.4.0/src/seismicrna/core/load.py
--rw-r--r--   0 mfa        (503) staff       (20)     2837 2023-07-07 02:37:13.000000 seismic-rna-0.4.0/src/seismicrna/core/logs.py
--rw-r--r--   0 mfa        (503) staff       (20)    14124 2023-06-29 02:17:49.000000 seismic-rna-0.4.0/src/seismicrna/core/mu.py
--rw-r--r--   0 mfa        (503) staff       (20)    10537 2023-06-30 18:53:43.000000 seismic-rna-0.4.0/src/seismicrna/core/mu_test.py
--rw-r--r--   0 mfa        (503) staff       (20)    14509 2023-07-12 20:28:15.000000 seismic-rna-0.4.0/src/seismicrna/core/parallel.py
--rw-r--r--   0 mfa        (503) staff       (20)    23511 2023-07-07 00:11:58.000000 seismic-rna-0.4.0/src/seismicrna/core/path.py
--rw-r--r--   0 mfa        (503) staff       (20)    29387 2023-07-14 20:09:45.000000 seismic-rna-0.4.0/src/seismicrna/core/rel.py
--rw-r--r--   0 mfa        (503) staff       (20)    45953 2023-06-30 18:58:01.000000 seismic-rna-0.4.0/src/seismicrna/core/rel_test.py
--rw-r--r--   0 mfa        (503) staff       (20)    29740 2023-07-12 04:26:52.000000 seismic-rna-0.4.0/src/seismicrna/core/report.py
--rw-r--r--   0 mfa        (503) staff       (20)     9169 2023-06-29 02:17:49.000000 seismic-rna-0.4.0/src/seismicrna/core/rna.py
--rw-r--r--   0 mfa        (503) staff       (20)    27329 2023-07-09 16:52:06.000000 seismic-rna-0.4.0/src/seismicrna/core/sect.py
--rw-r--r--   0 mfa        (503) staff       (20)     7101 2023-07-06 00:49:26.000000 seismic-rna-0.4.0/src/seismicrna/core/sect_test.py
--rw-r--r--   0 mfa        (503) staff       (20)     9798 2023-06-30 03:50:29.000000 seismic-rna-0.4.0/src/seismicrna/core/seq.py
--rw-r--r--   0 mfa        (503) staff       (20)     6634 2023-06-30 14:56:23.000000 seismic-rna-0.4.0/src/seismicrna/core/seq_test.py
--rw-r--r--   0 mfa        (503) staff       (20)     2799 2023-06-29 21:49:14.000000 seismic-rna-0.4.0/src/seismicrna/core/shell.py
--rw-r--r--   0 mfa        (503) staff       (20)     1054 2023-06-29 19:54:35.000000 seismic-rna-0.4.0/src/seismicrna/core/sim.py
--rw-r--r--   0 mfa        (503) staff       (20)      769 2023-07-06 00:49:45.000000 seismic-rna-0.4.0/src/seismicrna/core/sim_test.py
--rw-r--r--   0 mfa        (503) staff       (20)      758 2023-06-29 02:17:49.000000 seismic-rna-0.4.0/src/seismicrna/core/types.py
--rwxr-xr-x   0 mfa        (503) staff       (20)    14291 2023-06-30 03:36:23.000000 seismic-rna-0.4.0/src/seismicrna/core/xam.py
-drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-20 03:05:22.160082 seismic-rna-0.4.0/src/seismicrna/demult/
--rw-r--r--   0 mfa        (503) staff       (20)       35 2023-06-29 02:17:49.000000 seismic-rna-0.4.0/src/seismicrna/demult/__init__.py
--rw-r--r--   0 mfa        (503) staff       (20)    42624 2023-07-19 22:35:50.000000 seismic-rna-0.4.0/src/seismicrna/demult/demultiplex.py
--rw-r--r--   0 mfa        (503) staff       (20)     2103 2023-07-19 22:35:50.000000 seismic-rna-0.4.0/src/seismicrna/demult/main.py
-drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-20 03:05:22.166810 seismic-rna-0.4.0/src/seismicrna/draw/
--rw-r--r--   0 mfa        (503) staff       (20)      256 2023-06-29 19:38:33.000000 seismic-rna-0.4.0/src/seismicrna/draw/__init__.py
--rw-r--r--   0 mfa        (503) staff       (20)      225 2023-06-29 02:17:49.000000 seismic-rna-0.4.0/src/seismicrna/draw/load_dataset.py
--rw-r--r--   0 mfa        (503) staff       (20)     6013 2023-06-29 02:17:49.000000 seismic-rna-0.4.0/src/seismicrna/draw/main.py
--rw-r--r--   0 mfa        (503) staff       (20)     6656 2023-06-29 02:17:49.000000 seismic-rna-0.4.0/src/seismicrna/draw/manipulator.py
--rw-r--r--   0 mfa        (503) staff       (20)    17447 2023-06-29 19:43:29.000000 seismic-rna-0.4.0/src/seismicrna/draw/plotter.py
--rw-r--r--   0 mfa        (503) staff       (20)    15931 2023-06-29 02:17:49.000000 seismic-rna-0.4.0/src/seismicrna/draw/study.py
--rw-r--r--   0 mfa        (503) staff       (20)    11285 2023-06-29 02:17:49.000000 seismic-rna-0.4.0/src/seismicrna/draw/util.py
-drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-20 03:05:22.174579 seismic-rna-0.4.0/src/seismicrna/graph/
--rw-r--r--   0 mfa        (503) staff       (20)       22 2023-06-29 02:17:49.000000 seismic-rna-0.4.0/src/seismicrna/graph/__init__.py
--rw-r--r--   0 mfa        (503) staff       (20)     8731 2023-07-14 21:02:58.000000 seismic-rna-0.4.0/src/seismicrna/graph/base.py
--rw-r--r--   0 mfa        (503) staff       (20)     3539 2023-07-15 02:04:52.000000 seismic-rna-0.4.0/src/seismicrna/graph/color.py
--rw-r--r--   0 mfa        (503) staff       (20)     2701 2023-07-12 18:10:50.000000 seismic-rna-0.4.0/src/seismicrna/graph/default.py
--rw-r--r--   0 mfa        (503) staff       (20)     7493 2023-07-16 00:28:27.000000 seismic-rna-0.4.0/src/seismicrna/graph/hist.py
--rw-r--r--   0 mfa        (503) staff       (20)      337 2023-06-29 02:17:49.000000 seismic-rna-0.4.0/src/seismicrna/graph/main.py
--rw-r--r--   0 mfa        (503) staff       (20)    13371 2023-07-16 00:27:55.000000 seismic-rna-0.4.0/src/seismicrna/graph/seq.py
-drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-20 03:05:22.176462 seismic-rna-0.4.0/src/seismicrna/image/
--rw-r--r--   0 mfa        (503) staff       (20)        0 2023-07-09 20:01:37.000000 seismic-rna-0.4.0/src/seismicrna/image/__init__.py
--rw-r--r--   0 mfa        (503) staff       (20)     3492 2023-07-12 02:42:12.000000 seismic-rna-0.4.0/src/seismicrna/image/logo.py
--rw-r--r--   0 mfa        (503) staff       (20)     9616 2023-07-16 01:27:58.000000 seismic-rna-0.4.0/src/seismicrna/main.py
-drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-20 03:05:22.181066 seismic-rna-0.4.0/src/seismicrna/mask/
--rw-r--r--   0 mfa        (503) staff       (20)       35 2023-06-29 02:17:49.000000 seismic-rna-0.4.0/src/seismicrna/mask/__init__.py
--rw-r--r--   0 mfa        (503) staff       (20)     4074 2023-07-08 00:07:16.000000 seismic-rna-0.4.0/src/seismicrna/mask/load.py
--rw-r--r--   0 mfa        (503) staff       (20)     4447 2023-07-16 00:26:07.000000 seismic-rna-0.4.0/src/seismicrna/mask/main.py
--rw-r--r--   0 mfa        (503) staff       (20)     1315 2023-06-29 02:17:49.000000 seismic-rna-0.4.0/src/seismicrna/mask/report.py
--rw-r--r--   0 mfa        (503) staff       (20)    14222 2023-07-15 22:36:16.000000 seismic-rna-0.4.0/src/seismicrna/mask/write.py
--rw-r--r--   0 mfa        (503) staff       (20)      164 2023-07-16 01:29:14.000000 seismic-rna-0.4.0/src/seismicrna/meta.py
-drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-20 03:05:22.190927 seismic-rna-0.4.0/src/seismicrna/relate/
--rw-r--r--   0 mfa        (503) staff       (20)       35 2023-06-29 02:17:49.000000 seismic-rna-0.4.0/src/seismicrna/relate/__init__.py
--rw-r--r--   0 mfa        (503) staff       (20)     1413 2023-06-29 02:17:49.000000 seismic-rna-0.4.0/src/seismicrna/relate/export.py
--rw-r--r--   0 mfa        (503) staff       (20)     3241 2023-06-29 02:17:49.000000 seismic-rna-0.4.0/src/seismicrna/relate/load.py
--rw-r--r--   0 mfa        (503) staff       (20)     3096 2023-07-20 02:49:54.000000 seismic-rna-0.4.0/src/seismicrna/relate/main.py
--rw-r--r--   0 mfa        (503) staff       (20)    28055 2023-06-29 02:17:49.000000 seismic-rna-0.4.0/src/seismicrna/relate/relate.py
--rw-r--r--   0 mfa        (503) staff       (20)     1509 2023-06-29 02:17:49.000000 seismic-rna-0.4.0/src/seismicrna/relate/report.py
--rw-r--r--   0 mfa        (503) staff       (20)    10170 2023-06-30 02:27:38.000000 seismic-rna-0.4.0/src/seismicrna/relate/sam.py
--rw-r--r--   0 mfa        (503) staff       (20)     2984 2023-06-29 02:17:49.000000 seismic-rna-0.4.0/src/seismicrna/relate/seqpos.py
--rw-r--r--   0 mfa        (503) staff       (20)     3066 2023-06-29 02:17:49.000000 seismic-rna-0.4.0/src/seismicrna/relate/test.py
--rw-r--r--   0 mfa        (503) staff       (20)    15085 2023-07-10 03:02:51.000000 seismic-rna-0.4.0/src/seismicrna/relate/write.py
-drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-20 03:05:22.193789 seismic-rna-0.4.0/src/seismicrna/struct/
--rw-r--r--   0 mfa        (503) staff       (20)       35 2023-06-29 02:17:49.000000 seismic-rna-0.4.0/src/seismicrna/struct/__init__.py
--rw-r--r--   0 mfa        (503) staff       (20)     3827 2023-07-19 23:10:12.000000 seismic-rna-0.4.0/src/seismicrna/struct/main.py
--rw-r--r--   0 mfa        (503) staff       (20)     1850 2023-07-09 19:43:33.000000 seismic-rna-0.4.0/src/seismicrna/struct/rnastructure.py
-drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-20 03:05:22.199327 seismic-rna-0.4.0/src/seismicrna/table/
--rw-r--r--   0 mfa        (503) staff       (20)       35 2023-06-29 02:17:49.000000 seismic-rna-0.4.0/src/seismicrna/table/__init__.py
--rw-r--r--   0 mfa        (503) staff       (20)     9414 2023-07-15 00:14:41.000000 seismic-rna-0.4.0/src/seismicrna/table/base.py
--rw-r--r--   0 mfa        (503) staff       (20)     7236 2023-07-15 00:22:19.000000 seismic-rna-0.4.0/src/seismicrna/table/load.py
--rw-r--r--   0 mfa        (503) staff       (20)     1724 2023-07-16 00:27:03.000000 seismic-rna-0.4.0/src/seismicrna/table/main.py
--rw-r--r--   0 mfa        (503) staff       (20)    16181 2023-07-15 00:02:34.000000 seismic-rna-0.4.0/src/seismicrna/table/tabulate.py
--rw-r--r--   0 mfa        (503) staff       (20)     4684 2023-07-15 00:02:34.000000 seismic-rna-0.4.0/src/seismicrna/table/write.py
-drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-20 03:05:22.201223 seismic-rna-0.4.0/src/seismicrna/test/
--rw-r--r--   0 mfa        (503) staff       (20)       35 2023-06-29 02:17:49.000000 seismic-rna-0.4.0/src/seismicrna/test/__init__.py
--rw-r--r--   0 mfa        (503) staff       (20)      971 2023-07-06 00:56:02.000000 seismic-rna-0.4.0/src/seismicrna/test/main.py
+drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-21 02:50:00.061316 seismic-rna-0.4.1/
+-rw-r--r--   0 mfa        (503) staff       (20)    35150 2023-06-29 02:33:57.000000 seismic-rna-0.4.1/LICENSE
+-rw-r--r--   0 mfa        (503) staff       (20)     1910 2023-07-21 02:50:00.060911 seismic-rna-0.4.1/PKG-INFO
+-rw-r--r--   0 mfa        (503) staff       (20)     1347 2023-07-19 21:38:18.000000 seismic-rna-0.4.1/README.md
+-rw-r--r--   0 mfa        (503) staff       (20)     1037 2023-07-21 02:49:16.000000 seismic-rna-0.4.1/pyproject.toml
+-rw-r--r--   0 mfa        (503) staff       (20)       38 2023-07-21 02:50:00.061411 seismic-rna-0.4.1/setup.cfg
+drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-21 02:49:59.934843 seismic-rna-0.4.1/src/
+drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-21 02:49:59.946192 seismic-rna-0.4.1/src/seismic_rna.egg-info/
+-rw-r--r--   0 mfa        (503) staff       (20)     1910 2023-07-21 02:49:59.000000 seismic-rna-0.4.1/src/seismic_rna.egg-info/PKG-INFO
+-rw-r--r--   0 mfa        (503) staff       (20)     3039 2023-07-21 02:49:59.000000 seismic-rna-0.4.1/src/seismic_rna.egg-info/SOURCES.txt
+-rw-r--r--   0 mfa        (503) staff       (20)        1 2023-07-21 02:49:59.000000 seismic-rna-0.4.1/src/seismic_rna.egg-info/dependency_links.txt
+-rw-r--r--   0 mfa        (503) staff       (20)       53 2023-07-21 02:49:59.000000 seismic-rna-0.4.1/src/seismic_rna.egg-info/entry_points.txt
+-rw-r--r--   0 mfa        (503) staff       (20)      176 2023-07-21 02:49:59.000000 seismic-rna-0.4.1/src/seismic_rna.egg-info/requires.txt
+-rw-r--r--   0 mfa        (503) staff       (20)       11 2023-07-21 02:49:59.000000 seismic-rna-0.4.1/src/seismic_rna.egg-info/top_level.txt
+drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-21 02:49:59.948989 seismic-rna-0.4.1/src/seismicrna/
+-rw-r--r--   0 mfa        (503) staff       (20)      201 2023-07-16 01:27:23.000000 seismic-rna-0.4.1/src/seismicrna/__init__.py
+drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-21 02:49:59.955338 seismic-rna-0.4.1/src/seismicrna/align/
+-rw-r--r--   0 mfa        (503) staff       (20)       35 2023-06-29 02:17:49.000000 seismic-rna-0.4.1/src/seismicrna/align/__init__.py
+-rw-r--r--   0 mfa        (503) staff       (20)    22758 2023-07-05 00:01:54.000000 seismic-rna-0.4.1/src/seismicrna/align/fq2bam.py
+-rwxr-xr-x   0 mfa        (503) staff       (20)    20020 2023-07-09 17:46:17.000000 seismic-rna-0.4.1/src/seismicrna/align/fqutil.py
+-rw-r--r--   0 mfa        (503) staff       (20)     7600 2023-07-20 02:53:44.000000 seismic-rna-0.4.1/src/seismicrna/align/main.py
+-rwxr-xr-x   0 mfa        (503) staff       (20)     9115 2023-06-29 02:17:49.000000 seismic-rna-0.4.1/src/seismicrna/align/strandedness.py
+-rw-r--r--   0 mfa        (503) staff       (20)        0 2023-06-29 02:17:49.000000 seismic-rna-0.4.1/src/seismicrna/align/test.py
+drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-21 02:49:59.962752 seismic-rna-0.4.1/src/seismicrna/cluster/
+-rw-r--r--   0 mfa        (503) staff       (20)       35 2023-06-29 02:17:49.000000 seismic-rna-0.4.1/src/seismicrna/cluster/__init__.py
+-rw-r--r--   0 mfa        (503) staff       (20)    13197 2023-07-15 21:12:26.000000 seismic-rna-0.4.1/src/seismicrna/cluster/compare.py
+-rw-r--r--   0 mfa        (503) staff       (20)    18681 2023-06-29 02:17:49.000000 seismic-rna-0.4.1/src/seismicrna/cluster/em.py
+-rw-r--r--   0 mfa        (503) staff       (20)     6262 2023-06-29 02:17:49.000000 seismic-rna-0.4.1/src/seismicrna/cluster/krun.py
+-rw-r--r--   0 mfa        (503) staff       (20)     4209 2023-06-29 02:17:49.000000 seismic-rna-0.4.1/src/seismicrna/cluster/load.py
+-rw-r--r--   0 mfa        (503) staff       (20)     2464 2023-07-16 00:26:28.000000 seismic-rna-0.4.1/src/seismicrna/cluster/main.py
+-rw-r--r--   0 mfa        (503) staff       (20)     1264 2023-07-15 00:22:05.000000 seismic-rna-0.4.1/src/seismicrna/cluster/names.py
+-rw-r--r--   0 mfa        (503) staff       (20)     2862 2023-06-29 02:17:49.000000 seismic-rna-0.4.1/src/seismicrna/cluster/report.py
+-rw-r--r--   0 mfa        (503) staff       (20)     4981 2023-06-29 02:17:49.000000 seismic-rna-0.4.1/src/seismicrna/cluster/write.py
+drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-21 02:49:59.994103 seismic-rna-0.4.1/src/seismicrna/core/
+-rw-r--r--   0 mfa        (503) staff       (20)        0 2023-06-29 02:17:49.000000 seismic-rna-0.4.1/src/seismicrna/core/__init__.py
+-rw-r--r--   0 mfa        (503) staff       (20)    15704 2023-06-29 18:01:10.000000 seismic-rna-0.4.1/src/seismicrna/core/bitcall.py
+-rw-r--r--   0 mfa        (503) staff       (20)    19264 2023-07-07 22:07:51.000000 seismic-rna-0.4.1/src/seismicrna/core/bitvect.py
+-rw-r--r--   0 mfa        (503) staff       (20)    18165 2023-07-19 23:10:51.000000 seismic-rna-0.4.1/src/seismicrna/core/cli.py
+-rw-r--r--   0 mfa        (503) staff       (20)     1120 2023-06-29 21:48:51.000000 seismic-rna-0.4.1/src/seismicrna/core/depend.py
+-rw-r--r--   0 mfa        (503) staff       (20)     6844 2023-06-29 02:17:49.000000 seismic-rna-0.4.1/src/seismicrna/core/docdef.py
+-rw-r--r--   0 mfa        (503) staff       (20)     2201 2023-06-29 02:17:49.000000 seismic-rna-0.4.1/src/seismicrna/core/docstring.py
+-rw-r--r--   0 mfa        (503) staff       (20)     1972 2023-06-29 02:17:49.000000 seismic-rna-0.4.1/src/seismicrna/core/dump.py
+-rw-r--r--   0 mfa        (503) staff       (20)      628 2023-06-29 02:17:49.000000 seismic-rna-0.4.1/src/seismicrna/core/files.py
+-rw-r--r--   0 mfa        (503) staff       (20)     7933 2023-07-07 22:47:51.000000 seismic-rna-0.4.1/src/seismicrna/core/load.py
+-rw-r--r--   0 mfa        (503) staff       (20)     2837 2023-07-07 02:37:13.000000 seismic-rna-0.4.1/src/seismicrna/core/logs.py
+-rw-r--r--   0 mfa        (503) staff       (20)    14124 2023-06-29 02:17:49.000000 seismic-rna-0.4.1/src/seismicrna/core/mu.py
+-rw-r--r--   0 mfa        (503) staff       (20)    10537 2023-06-30 18:53:43.000000 seismic-rna-0.4.1/src/seismicrna/core/mu_test.py
+-rw-r--r--   0 mfa        (503) staff       (20)    14509 2023-07-12 20:28:15.000000 seismic-rna-0.4.1/src/seismicrna/core/parallel.py
+-rw-r--r--   0 mfa        (503) staff       (20)    23511 2023-07-07 00:11:58.000000 seismic-rna-0.4.1/src/seismicrna/core/path.py
+-rw-r--r--   0 mfa        (503) staff       (20)    29387 2023-07-14 20:09:45.000000 seismic-rna-0.4.1/src/seismicrna/core/rel.py
+-rw-r--r--   0 mfa        (503) staff       (20)    45953 2023-06-30 18:58:01.000000 seismic-rna-0.4.1/src/seismicrna/core/rel_test.py
+-rw-r--r--   0 mfa        (503) staff       (20)    29740 2023-07-12 04:26:52.000000 seismic-rna-0.4.1/src/seismicrna/core/report.py
+-rw-r--r--   0 mfa        (503) staff       (20)     9169 2023-06-29 02:17:49.000000 seismic-rna-0.4.1/src/seismicrna/core/rna.py
+-rw-r--r--   0 mfa        (503) staff       (20)    27329 2023-07-09 16:52:06.000000 seismic-rna-0.4.1/src/seismicrna/core/sect.py
+-rw-r--r--   0 mfa        (503) staff       (20)     7101 2023-07-06 00:49:26.000000 seismic-rna-0.4.1/src/seismicrna/core/sect_test.py
+-rw-r--r--   0 mfa        (503) staff       (20)     9798 2023-06-30 03:50:29.000000 seismic-rna-0.4.1/src/seismicrna/core/seq.py
+-rw-r--r--   0 mfa        (503) staff       (20)     6634 2023-06-30 14:56:23.000000 seismic-rna-0.4.1/src/seismicrna/core/seq_test.py
+-rw-r--r--   0 mfa        (503) staff       (20)     2799 2023-06-29 21:49:14.000000 seismic-rna-0.4.1/src/seismicrna/core/shell.py
+-rw-r--r--   0 mfa        (503) staff       (20)     1054 2023-06-29 19:54:35.000000 seismic-rna-0.4.1/src/seismicrna/core/sim.py
+-rw-r--r--   0 mfa        (503) staff       (20)      769 2023-07-06 00:49:45.000000 seismic-rna-0.4.1/src/seismicrna/core/sim_test.py
+-rw-r--r--   0 mfa        (503) staff       (20)      758 2023-06-29 02:17:49.000000 seismic-rna-0.4.1/src/seismicrna/core/types.py
+-rwxr-xr-x   0 mfa        (503) staff       (20)    14291 2023-06-30 03:36:23.000000 seismic-rna-0.4.1/src/seismicrna/core/xam.py
+drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-21 02:49:59.998782 seismic-rna-0.4.1/src/seismicrna/demult/
+-rw-r--r--   0 mfa        (503) staff       (20)       35 2023-06-29 02:17:49.000000 seismic-rna-0.4.1/src/seismicrna/demult/__init__.py
+-rw-r--r--   0 mfa        (503) staff       (20)    42624 2023-07-19 22:35:50.000000 seismic-rna-0.4.1/src/seismicrna/demult/demultiplex.py
+-rw-r--r--   0 mfa        (503) staff       (20)     2103 2023-07-19 22:35:50.000000 seismic-rna-0.4.1/src/seismicrna/demult/main.py
+drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-21 02:50:00.009013 seismic-rna-0.4.1/src/seismicrna/draw/
+-rw-r--r--   0 mfa        (503) staff       (20)      256 2023-06-29 19:38:33.000000 seismic-rna-0.4.1/src/seismicrna/draw/__init__.py
+-rw-r--r--   0 mfa        (503) staff       (20)      225 2023-06-29 02:17:49.000000 seismic-rna-0.4.1/src/seismicrna/draw/load_dataset.py
+-rw-r--r--   0 mfa        (503) staff       (20)     6013 2023-06-29 02:17:49.000000 seismic-rna-0.4.1/src/seismicrna/draw/main.py
+-rw-r--r--   0 mfa        (503) staff       (20)     6656 2023-06-29 02:17:49.000000 seismic-rna-0.4.1/src/seismicrna/draw/manipulator.py
+-rw-r--r--   0 mfa        (503) staff       (20)    17447 2023-06-29 19:43:29.000000 seismic-rna-0.4.1/src/seismicrna/draw/plotter.py
+-rw-r--r--   0 mfa        (503) staff       (20)    15931 2023-06-29 02:17:49.000000 seismic-rna-0.4.1/src/seismicrna/draw/study.py
+-rw-r--r--   0 mfa        (503) staff       (20)    11285 2023-06-29 02:17:49.000000 seismic-rna-0.4.1/src/seismicrna/draw/util.py
+drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-21 02:50:00.021994 seismic-rna-0.4.1/src/seismicrna/graph/
+-rw-r--r--   0 mfa        (503) staff       (20)       22 2023-06-29 02:17:49.000000 seismic-rna-0.4.1/src/seismicrna/graph/__init__.py
+-rw-r--r--   0 mfa        (503) staff       (20)     8731 2023-07-14 21:02:58.000000 seismic-rna-0.4.1/src/seismicrna/graph/base.py
+-rw-r--r--   0 mfa        (503) staff       (20)     3539 2023-07-15 02:04:52.000000 seismic-rna-0.4.1/src/seismicrna/graph/color.py
+-rw-r--r--   0 mfa        (503) staff       (20)     2701 2023-07-12 18:10:50.000000 seismic-rna-0.4.1/src/seismicrna/graph/default.py
+-rw-r--r--   0 mfa        (503) staff       (20)     7493 2023-07-16 00:28:27.000000 seismic-rna-0.4.1/src/seismicrna/graph/hist.py
+-rw-r--r--   0 mfa        (503) staff       (20)      337 2023-06-29 02:17:49.000000 seismic-rna-0.4.1/src/seismicrna/graph/main.py
+-rw-r--r--   0 mfa        (503) staff       (20)    13371 2023-07-16 00:27:55.000000 seismic-rna-0.4.1/src/seismicrna/graph/seq.py
+drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-21 02:50:00.027781 seismic-rna-0.4.1/src/seismicrna/image/
+-rw-r--r--   0 mfa        (503) staff       (20)        0 2023-07-09 20:01:37.000000 seismic-rna-0.4.1/src/seismicrna/image/__init__.py
+-rw-r--r--   0 mfa        (503) staff       (20)     3492 2023-07-12 02:42:12.000000 seismic-rna-0.4.1/src/seismicrna/image/logo.py
+-rw-r--r--   0 mfa        (503) staff       (20)     9616 2023-07-16 01:27:58.000000 seismic-rna-0.4.1/src/seismicrna/main.py
+drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-21 02:50:00.035121 seismic-rna-0.4.1/src/seismicrna/mask/
+-rw-r--r--   0 mfa        (503) staff       (20)       35 2023-06-29 02:17:49.000000 seismic-rna-0.4.1/src/seismicrna/mask/__init__.py
+-rw-r--r--   0 mfa        (503) staff       (20)     4074 2023-07-08 00:07:16.000000 seismic-rna-0.4.1/src/seismicrna/mask/load.py
+-rw-r--r--   0 mfa        (503) staff       (20)     4447 2023-07-16 00:26:07.000000 seismic-rna-0.4.1/src/seismicrna/mask/main.py
+-rw-r--r--   0 mfa        (503) staff       (20)     1315 2023-06-29 02:17:49.000000 seismic-rna-0.4.1/src/seismicrna/mask/report.py
+-rw-r--r--   0 mfa        (503) staff       (20)    14222 2023-07-15 22:36:16.000000 seismic-rna-0.4.1/src/seismicrna/mask/write.py
+-rw-r--r--   0 mfa        (503) staff       (20)      164 2023-07-16 01:29:14.000000 seismic-rna-0.4.1/src/seismicrna/meta.py
+drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-21 02:50:00.048107 seismic-rna-0.4.1/src/seismicrna/relate/
+-rw-r--r--   0 mfa        (503) staff       (20)       35 2023-06-29 02:17:49.000000 seismic-rna-0.4.1/src/seismicrna/relate/__init__.py
+-rw-r--r--   0 mfa        (503) staff       (20)     1413 2023-06-29 02:17:49.000000 seismic-rna-0.4.1/src/seismicrna/relate/export.py
+-rw-r--r--   0 mfa        (503) staff       (20)     3241 2023-06-29 02:17:49.000000 seismic-rna-0.4.1/src/seismicrna/relate/load.py
+-rw-r--r--   0 mfa        (503) staff       (20)     3096 2023-07-20 02:49:54.000000 seismic-rna-0.4.1/src/seismicrna/relate/main.py
+-rw-r--r--   0 mfa        (503) staff       (20)    28055 2023-06-29 02:17:49.000000 seismic-rna-0.4.1/src/seismicrna/relate/relate.py
+-rw-r--r--   0 mfa        (503) staff       (20)     1509 2023-06-29 02:17:49.000000 seismic-rna-0.4.1/src/seismicrna/relate/report.py
+-rw-r--r--   0 mfa        (503) staff       (20)    10170 2023-06-30 02:27:38.000000 seismic-rna-0.4.1/src/seismicrna/relate/sam.py
+-rw-r--r--   0 mfa        (503) staff       (20)     2984 2023-06-29 02:17:49.000000 seismic-rna-0.4.1/src/seismicrna/relate/seqpos.py
+-rw-r--r--   0 mfa        (503) staff       (20)     3066 2023-06-29 02:17:49.000000 seismic-rna-0.4.1/src/seismicrna/relate/test.py
+-rw-r--r--   0 mfa        (503) staff       (20)    15085 2023-07-10 03:02:51.000000 seismic-rna-0.4.1/src/seismicrna/relate/write.py
+drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-21 02:50:00.051917 seismic-rna-0.4.1/src/seismicrna/struct/
+-rw-r--r--   0 mfa        (503) staff       (20)       35 2023-06-29 02:17:49.000000 seismic-rna-0.4.1/src/seismicrna/struct/__init__.py
+-rw-r--r--   0 mfa        (503) staff       (20)     3827 2023-07-19 23:10:12.000000 seismic-rna-0.4.1/src/seismicrna/struct/main.py
+-rw-r--r--   0 mfa        (503) staff       (20)     1850 2023-07-09 19:43:33.000000 seismic-rna-0.4.1/src/seismicrna/struct/rnastructure.py
+drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-21 02:50:00.058045 seismic-rna-0.4.1/src/seismicrna/table/
+-rw-r--r--   0 mfa        (503) staff       (20)       35 2023-06-29 02:17:49.000000 seismic-rna-0.4.1/src/seismicrna/table/__init__.py
+-rw-r--r--   0 mfa        (503) staff       (20)     9380 2023-07-20 23:21:09.000000 seismic-rna-0.4.1/src/seismicrna/table/base.py
+-rw-r--r--   0 mfa        (503) staff       (20)     7236 2023-07-15 00:22:19.000000 seismic-rna-0.4.1/src/seismicrna/table/load.py
+-rw-r--r--   0 mfa        (503) staff       (20)     1724 2023-07-16 00:27:03.000000 seismic-rna-0.4.1/src/seismicrna/table/main.py
+-rw-r--r--   0 mfa        (503) staff       (20)    15792 2023-07-21 02:45:00.000000 seismic-rna-0.4.1/src/seismicrna/table/tabulate.py
+-rw-r--r--   0 mfa        (503) staff       (20)     4684 2023-07-15 00:02:34.000000 seismic-rna-0.4.1/src/seismicrna/table/write.py
+drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-21 02:50:00.060093 seismic-rna-0.4.1/src/seismicrna/test/
+-rw-r--r--   0 mfa        (503) staff       (20)       35 2023-06-29 02:17:49.000000 seismic-rna-0.4.1/src/seismicrna/test/__init__.py
+-rw-r--r--   0 mfa        (503) staff       (20)      971 2023-07-06 00:56:02.000000 seismic-rna-0.4.1/src/seismicrna/test/main.py
```

### Comparing `seismic-rna-0.4.0/LICENSE` & `seismic-rna-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.4.0/PKG-INFO` & `seismic-rna-0.4.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seismic-rna
-Version: 0.4.0
+Version: 0.4.1
 Summary: RNA Structure Ensemble Inference via Sequencing, Mutation Identification, and Clustering
 Author: Matty Allan, Yves Martin, Scott Grote, Alberic de Lajarte
 License: GPL-3.0-only
 Project-URL: Homepage, https://github.com/rouskinlab/seismic-rna
 Project-URL: Bug Tracker, https://github.com/rouskinlab/seismic-rna/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `seismic-rna-0.4.0/README.md` & `seismic-rna-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.4.0/pyproject.toml` & `seismic-rna-0.4.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "seismic-rna"
-version = "0.4.0"
+version = "0.4.1"
 authors = [
     {name="Matty Allan"},
     {name="Yves Martin"},
     {name="Scott Grote"},
     {name="Alberic de Lajarte"},
 ]
 description = "RNA Structure Ensemble Inference via Sequencing, Mutation Identification, and Clustering"
```

### Comparing `seismic-rna-0.4.0/src/seismic_rna.egg-info/PKG-INFO` & `seismic-rna-0.4.1/src/seismic_rna.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seismic-rna
-Version: 0.4.0
+Version: 0.4.1
 Summary: RNA Structure Ensemble Inference via Sequencing, Mutation Identification, and Clustering
 Author: Matty Allan, Yves Martin, Scott Grote, Alberic de Lajarte
 License: GPL-3.0-only
 Project-URL: Homepage, https://github.com/rouskinlab/seismic-rna
 Project-URL: Bug Tracker, https://github.com/rouskinlab/seismic-rna/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `seismic-rna-0.4.0/src/seismic_rna.egg-info/SOURCES.txt` & `seismic-rna-0.4.1/src/seismic_rna.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.4.0/src/seismicrna/align/fq2bam.py` & `seismic-rna-0.4.1/src/seismicrna/align/fq2bam.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.4.0/src/seismicrna/align/fqutil.py` & `seismic-rna-0.4.1/src/seismicrna/align/fqutil.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.4.0/src/seismicrna/align/main.py` & `seismic-rna-0.4.1/src/seismicrna/align/main.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.4.0/src/seismicrna/align/strandedness.py` & `seismic-rna-0.4.1/src/seismicrna/align/strandedness.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.4.0/src/seismicrna/cluster/compare.py` & `seismic-rna-0.4.1/src/seismicrna/cluster/compare.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.4.0/src/seismicrna/cluster/em.py` & `seismic-rna-0.4.1/src/seismicrna/cluster/em.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.4.0/src/seismicrna/cluster/krun.py` & `seismic-rna-0.4.1/src/seismicrna/cluster/krun.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.4.0/src/seismicrna/cluster/load.py` & `seismic-rna-0.4.1/src/seismicrna/cluster/load.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.4.0/src/seismicrna/cluster/main.py` & `seismic-rna-0.4.1/src/seismicrna/cluster/main.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.4.0/src/seismicrna/cluster/names.py` & `seismic-rna-0.4.1/src/seismicrna/cluster/names.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.4.0/src/seismicrna/cluster/report.py` & `seismic-rna-0.4.1/src/seismicrna/cluster/report.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.4.0/src/seismicrna/cluster/write.py` & `seismic-rna-0.4.1/src/seismicrna/cluster/write.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.4.0/src/seismicrna/core/bitcall.py` & `seismic-rna-0.4.1/src/seismicrna/core/bitcall.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.4.0/src/seismicrna/core/bitvect.py` & `seismic-rna-0.4.1/src/seismicrna/core/bitvect.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.4.0/src/seismicrna/core/cli.py` & `seismic-rna-0.4.1/src/seismicrna/core/cli.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.4.0/src/seismicrna/core/depend.py` & `seismic-rna-0.4.1/src/seismicrna/core/depend.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.4.0/src/seismicrna/core/docdef.py` & `seismic-rna-0.4.1/src/seismicrna/core/docdef.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.4.0/src/seismicrna/core/docstring.py` & `seismic-rna-0.4.1/src/seismicrna/core/docstring.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.4.0/src/seismicrna/core/dump.py` & `seismic-rna-0.4.1/src/seismicrna/core/dump.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.4.0/src/seismicrna/core/files.py` & `seismic-rna-0.4.1/src/seismicrna/core/files.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.4.0/src/seismicrna/core/load.py` & `seismic-rna-0.4.1/src/seismicrna/core/load.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.4.0/src/seismicrna/core/logs.py` & `seismic-rna-0.4.1/src/seismicrna/core/logs.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.4.0/src/seismicrna/core/mu.py` & `seismic-rna-0.4.1/src/seismicrna/core/mu.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.4.0/src/seismicrna/core/mu_test.py` & `seismic-rna-0.4.1/src/seismicrna/core/mu_test.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.4.0/src/seismicrna/core/parallel.py` & `seismic-rna-0.4.1/src/seismicrna/core/parallel.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.4.0/src/seismicrna/core/path.py` & `seismic-rna-0.4.1/src/seismicrna/core/path.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.4.0/src/seismicrna/core/rel.py` & `seismic-rna-0.4.1/src/seismicrna/core/rel.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.4.0/src/seismicrna/core/rel_test.py` & `seismic-rna-0.4.1/src/seismicrna/core/rel_test.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.4.0/src/seismicrna/core/report.py` & `seismic-rna-0.4.1/src/seismicrna/core/report.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.4.0/src/seismicrna/core/rna.py` & `seismic-rna-0.4.1/src/seismicrna/core/rna.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.4.0/src/seismicrna/core/sect.py` & `seismic-rna-0.4.1/src/seismicrna/core/sect.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.4.0/src/seismicrna/core/sect_test.py` & `seismic-rna-0.4.1/src/seismicrna/core/sect_test.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.4.0/src/seismicrna/core/seq.py` & `seismic-rna-0.4.1/src/seismicrna/core/seq.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.4.0/src/seismicrna/core/seq_test.py` & `seismic-rna-0.4.1/src/seismicrna/core/seq_test.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.4.0/src/seismicrna/core/shell.py` & `seismic-rna-0.4.1/src/seismicrna/core/shell.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.4.0/src/seismicrna/core/sim.py` & `seismic-rna-0.4.1/src/seismicrna/core/sim.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.4.0/src/seismicrna/core/sim_test.py` & `seismic-rna-0.4.1/src/seismicrna/core/sim_test.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.4.0/src/seismicrna/core/types.py` & `seismic-rna-0.4.1/src/seismicrna/core/types.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.4.0/src/seismicrna/core/xam.py` & `seismic-rna-0.4.1/src/seismicrna/core/xam.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.4.0/src/seismicrna/demult/demultiplex.py` & `seismic-rna-0.4.1/src/seismicrna/demult/demultiplex.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.4.0/src/seismicrna/demult/main.py` & `seismic-rna-0.4.1/src/seismicrna/demult/main.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.4.0/src/seismicrna/draw/main.py` & `seismic-rna-0.4.1/src/seismicrna/draw/main.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.4.0/src/seismicrna/draw/manipulator.py` & `seismic-rna-0.4.1/src/seismicrna/draw/manipulator.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.4.0/src/seismicrna/draw/plotter.py` & `seismic-rna-0.4.1/src/seismicrna/draw/plotter.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.4.0/src/seismicrna/draw/study.py` & `seismic-rna-0.4.1/src/seismicrna/draw/study.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.4.0/src/seismicrna/draw/util.py` & `seismic-rna-0.4.1/src/seismicrna/draw/util.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.4.0/src/seismicrna/graph/base.py` & `seismic-rna-0.4.1/src/seismicrna/graph/base.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.4.0/src/seismicrna/graph/color.py` & `seismic-rna-0.4.1/src/seismicrna/graph/color.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.4.0/src/seismicrna/graph/default.py` & `seismic-rna-0.4.1/src/seismicrna/graph/default.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.4.0/src/seismicrna/graph/hist.py` & `seismic-rna-0.4.1/src/seismicrna/graph/hist.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.4.0/src/seismicrna/graph/seq.py` & `seismic-rna-0.4.1/src/seismicrna/graph/seq.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.4.0/src/seismicrna/image/logo.py` & `seismic-rna-0.4.1/src/seismicrna/image/logo.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.4.0/src/seismicrna/main.py` & `seismic-rna-0.4.1/src/seismicrna/main.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.4.0/src/seismicrna/mask/load.py` & `seismic-rna-0.4.1/src/seismicrna/mask/load.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.4.0/src/seismicrna/mask/main.py` & `seismic-rna-0.4.1/src/seismicrna/mask/main.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.4.0/src/seismicrna/mask/report.py` & `seismic-rna-0.4.1/src/seismicrna/mask/report.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.4.0/src/seismicrna/mask/write.py` & `seismic-rna-0.4.1/src/seismicrna/mask/write.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.4.0/src/seismicrna/relate/export.py` & `seismic-rna-0.4.1/src/seismicrna/relate/export.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.4.0/src/seismicrna/relate/load.py` & `seismic-rna-0.4.1/src/seismicrna/relate/load.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.4.0/src/seismicrna/relate/main.py` & `seismic-rna-0.4.1/src/seismicrna/relate/main.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.4.0/src/seismicrna/relate/relate.py` & `seismic-rna-0.4.1/src/seismicrna/relate/relate.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.4.0/src/seismicrna/relate/report.py` & `seismic-rna-0.4.1/src/seismicrna/relate/report.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.4.0/src/seismicrna/relate/sam.py` & `seismic-rna-0.4.1/src/seismicrna/relate/sam.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.4.0/src/seismicrna/relate/seqpos.py` & `seismic-rna-0.4.1/src/seismicrna/relate/seqpos.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.4.0/src/seismicrna/relate/test.py` & `seismic-rna-0.4.1/src/seismicrna/relate/test.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.4.0/src/seismicrna/relate/write.py` & `seismic-rna-0.4.1/src/seismicrna/relate/write.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.4.0/src/seismicrna/struct/main.py` & `seismic-rna-0.4.1/src/seismicrna/struct/main.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.4.0/src/seismicrna/struct/rnastructure.py` & `seismic-rna-0.4.1/src/seismicrna/struct/rnastructure.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.4.0/src/seismicrna/table/base.py` & `seismic-rna-0.4.1/src/seismicrna/table/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     'g': SUB_G_REL,
     't': SUB_T_REL,
     'd': DELET_REL,
     'i': INSRT_REL,
 }
 
 # Columns of each relation-based table
-TABLE_COLUMNS = [rel for rel in REL_CODES.values() if rel != INFOR_REL]
+TABLE_RELS = list(REL_CODES.values())
 
 
 # Table Base Classes ###################################################
 
 class Table(ABC):
     """ Table base class. """
```

### Comparing `seismic-rna-0.4.0/src/seismicrna/table/load.py` & `seismic-rna-0.4.1/src/seismicrna/table/load.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.4.0/src/seismicrna/table/main.py` & `seismic-rna-0.4.1/src/seismicrna/table/main.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.4.0/src/seismicrna/table/tabulate.py` & `seismic-rna-0.4.1/src/seismicrna/table/tabulate.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,36 @@
 from abc import ABC, abstractmethod
 from functools import cache, cached_property
 from logging import getLogger
+from typing import Any
 
 import numpy as np
 import pandas as pd
 
 from .base import (COVER_REL, DELET_REL, INSRT_REL, MATCH_REL, MUTAT_REL,
                    SUBST_REL, SUB_A_REL, SUB_C_REL, SUB_G_REL, SUB_T_REL,
-                   CLUST_INDEX_NAMES, REL_NAME, R_ADJ_TITLE, R_OBS_TITLE,
-                   READ_TITLE, REL_CODES, TABLE_COLUMNS)
+                   INFOR_REL, CLUST_INDEX_NAMES, R_ADJ_TITLE, R_OBS_TITLE,
+                   READ_TITLE, REL_NAME, REL_CODES, TABLE_RELS)
 from ..cluster.load import ClustLoader
 from ..core.bitcall import BitCaller, SemiBitCaller
 from ..core.bitvect import BitCounter, ClustBitCounter
 from ..core.mu import calc_f_obs_df, calc_mu_adj_df
 from ..core.sect import Section, INDEX_NAMES
 from ..mask.load import MaskLoader
 from ..relate.load import RelateLoader
 
 logger = getLogger(__name__)
 
 # These relationships must be computed, else adjust_counts() will fail.
 REQUIRED_RELS = MATCH_REL, MUTAT_REL
 
+# These relationships are of all subtypes of mutations.
+SUBMUTS = [SUBST_REL, SUB_A_REL, SUB_C_REL, SUB_G_REL, SUB_T_REL,
+           DELET_REL, INSRT_REL]
+
 
 # Tabulator Classes ####################################################
 
 class Tabulator(ABC):
     """ Base class for tabulating data for multiple tables from a report
     loader. """
 
@@ -89,49 +94,54 @@
         """ Count the bits per position. """
 
     @abstractmethod
     def tabulate_by_read(self):
         """ Count the bits per read. """
 
 
-class AvgTabulator(Tabulator, ABC):
+class EnsembleTabulator(Tabulator, ABC):
 
     @property
     def columns(self):
-        return pd.Index(TABLE_COLUMNS, name=REL_NAME)
+        return pd.Index(TABLE_RELS, name=REL_NAME)
 
     def tabulate_by_pos(self):
         # Assemble the DataFrame from the bit counts.
         data = pd.DataFrame.from_dict({rel: counter.n_affi_per_pos
                                        for rel, counter
                                        in self.bit_counts.items()})
+        # Add a column for the informative bits.
+        data[INFOR_REL] = data[MATCH_REL] + data[MUTAT_REL]
         # Rename the index of the positions and bases.
         data.index.rename(INDEX_NAMES, inplace=True)
         # Include all columns of relationships, even those not counted.
         return data.reindex(columns=self.columns)
 
     def tabulate_by_read(self):
         """ Count the bits per read. """
+        # Assemble the DataFrame from the bit counts.
         data = pd.DataFrame.from_dict({rel: counter.n_affi_per_read
                                        for rel, counter
                                        in self.bit_counts.items()})
+        # Add a column for the informative bits.
+        data[INFOR_REL] = data[MATCH_REL] + data[MUTAT_REL]
         # Rename the index of the read names.
         data.index.rename(READ_TITLE, inplace=True)
         # Include all columns of relationships, even those not counted.
         return data.reindex(columns=self.columns)
 
 
 class NullableTabulator(Tabulator, ABC):
 
     @classmethod
     def get_null_value(cls):
         return np.nan
 
 
-class RelTabulator(AvgTabulator):
+class RelTabulator(EnsembleTabulator):
 
     @classmethod
     def get_null_value(cls):
         return 0
 
     @cached_property
     def bit_counts(self):
@@ -142,15 +152,15 @@
             bit_counts[name] = BitCounter(
                 self.section,
                 bit_caller.iter(self._loader.iter_batches_processed())
             )
         return bit_counts
 
 
-class MaskTabulator(AvgTabulator, NullableTabulator):
+class MaskTabulator(EnsembleTabulator, NullableTabulator):
 
     @cached_property
     def bit_counts(self):
         return {
             rel: BitCounter(self.section,
                             self._loader.iter_batches_processed(bit_caller=bc,
                                                                 **kwargs))
@@ -175,67 +185,84 @@
     def get_read_names(self):
         return self._loader.import_loader.get_read_names()
 
     @cached_property
     def columns(self):
         return pd.MultiIndex.from_tuples([(order, cluster, rel)
                                           for order, cluster in self.ord_clust
-                                          for rel in TABLE_COLUMNS],
+                                          for rel in TABLE_RELS],
                                          names=CLUST_INDEX_NAMES)
 
     @cached_property
     def bit_counts(self):
         return dict(
             (rel, ClustBitCounter(
                 self.section,
                 self.ord_clust,
                 self._loader.iter_batches_processed(bit_caller=bc, **kwargs)
             )) for rel, bc, kwargs in self.iter_bit_callers()
         )
 
+    @staticmethod
+    def _slice_rel(counts: pd.DataFrame, rel: str, values: Any | None = None):
+        """ Slice one relationship from all clusters. """
+        slicer = slice(None), slice(None), rel
+        if values is None:
+            return counts.loc[:, slicer]
+        counts.loc[:, slicer] = values
+
     @cache
     def tabulate_by_pos(self):
         """ DataFrame of the bit count for each position and caller. """
-        # Initialize an empty DataFrame of adjusted counts.
-        counts_adj = pd.DataFrame(self.get_null_value(),
-                                  index=self._loader.section.unmasked,
-                                  columns=self.columns)
-        # Fill in the DataFrame one cluster at a time.
-        for order, k in self.ord_clust:
-            # Initialize a DataFrame of observed counts for the cluster.
-            counts_obs = pd.DataFrame(self.get_null_value(),
-                                      index=self._loader.section.unmasked,
-                                      columns=TABLE_COLUMNS)
-            # Fill in the observed counts column by column.
-            for rel in counts_obs.columns.to_list():
-                counts = self.bit_counts[rel].n_affi_per_pos.loc[:, (order, k)]
-                counts_obs.loc[:, rel] = counts
+        # Initialize an empty DataFrame of observed counts.
+        counts = pd.DataFrame(self.get_null_value(),
+                              index=self._loader.section.unmasked,
+                              columns=self.columns)
+        # Fill the observed counts one relationship at a time.
+        for rel in TABLE_RELS:
+            try:
+                counter = self.bit_counts[rel]
+            except KeyError:
+                # The relationship was not among those tabulated.
+                pass
+            else:
+                self._slice_rel(counts, rel, counter.n_affi_per_pos.values)
+        # Count the informative bits.
+        self._slice_rel(counts, INFOR_REL,
+                        self._slice_rel(counts, MATCH_REL).values
+                        + self._slice_rel(counts, MUTAT_REL).values)
+        # Adjust the counts for each cluster.
+        for ok in self.ord_clust:
             # Adjust the counts to correct for observer bias.
-            counts = adjust_counts(counts_obs,
-                                   self._loader.section,
-                                   self._loader.min_mut_gap)
-            counts_adj.loc[:, (order, k)] = counts.values
-        return counts_adj
+            counts.loc[:, ok] = adjust_counts(counts.loc[:, ok],
+                                              self._loader.section,
+                                              self._loader.min_mut_gap).values
+        return counts
 
     def tabulate_by_read(self):
         """ DataFrame of the bit count for each read and caller. """
+
         # Initialize an empty DataFrame.
         counts = pd.DataFrame(self.get_null_value(),
                               index=pd.Index(self.get_read_names(),
                                              name=READ_TITLE),
                               columns=self.columns)
-        # Fill in the DataFrame column by column.
-        for col in self.columns:
-            # Split the column label into the clustering order, cluster
-            # number (k), and type of relationship (rel).
-            order, k, rel = col
-            ok = order, k
-            # Get the bit counter for the relationship and select the
-            # column for the clustering order and cluster number.
-            counts.loc[:, col] = self.bit_counts[rel].n_affi_per_read.loc[:, ok]
+        # Fill in the DataFrame one relationship at a time.
+        for rel in TABLE_RELS:
+            try:
+                counter = self.bit_counts[rel]
+            except KeyError:
+                # The relationship was not among those tabulated.
+                pass
+            else:
+                self._slice_rel(counts, rel, counter.n_affi_per_read.values)
+        # Count the informative bits.
+        self._slice_rel(counts, INFOR_REL,
+                        self._slice_rel(counts, MATCH_REL).values
+                        + self._slice_rel(counts, MUTAT_REL).values)
         return counts
 
     def tabulate_by_clust(self):
         """ Return the adjusted number of reads in each cluster as a
         Series with dimension (clusters). """
         return pd.DataFrame.from_dict({
             R_OBS_TITLE: self._loader.n_reads_obs,
@@ -283,15 +310,15 @@
     if rel_codes:
         # Use the selected relationships and two required relationships:
         # MATCH and MUTAT.
         call_rels = {REL_CODES[code] for code in rel_codes}
         call_rels.update(REQUIRED_RELS)
     else:
         # Use all types of relationships.
-        call_rels = set(TABLE_COLUMNS)
+        call_rels = set(TABLE_RELS)
     # Yield a BitCaller for each selected type of relationship.
     for rel, bit_caller, kwargs in _iter_bit_callers(section):
         if rel in call_rels:
             yield rel, bit_caller, kwargs
 
 
 def adjust_counts(counts_obs: pd.DataFrame,
@@ -314,80 +341,57 @@
     logger.debug(f"Adjusting mutation counts of table\n{counts_obs}")
     # Initialize an empty DataFrame of the adjusted counts with the same
     # index and columns as the observed counts.
     counts_adj = pd.DataFrame(np.nan,
                               index=counts_obs.index,
                               columns=counts_obs.columns)
     # Compute the observed fraction of mutations at each position.
-    nrefs_obs = counts_obs.loc[:, MATCH_REL]
-    nmuts_obs = counts_obs.loc[:, MUTAT_REL]
-    ninfo_obs = nrefs_obs + nmuts_obs
     with np.errstate(divide="ignore"):
         # Ignore division by zero, which is acceptable here because any
         # NaN values will be zeroed out subsequently.
-        fmuts_obs = nmuts_obs / ninfo_obs
-    # Fill missing NaN values with zero.
+        fmuts_obs = counts_obs.loc[:, MUTAT_REL] / counts_obs.loc[:, INFOR_REL]
+    # Fill any missing (NaN) values with zero.
     fmuts_obs.fillna(0., inplace=True)
     # Adjust the fraction of mutations to correct the observer bias.
     fmuts_adj = calc_mu_adj_df(fmuts_obs.to_frame(), section,
                                min_mut_gap).squeeze()
-    # Compute the fraction of reads that would be observed.
+    # Compute the fraction of all reads that would be observed.
     f_obs = float(calc_f_obs_df(fmuts_adj.to_frame(), section,
                                 min_mut_gap)[0])
-    # Assume that the total number of base calls including unobserved
-    # reads is the number observed divided by the fraction of the total
-    # reads that were observed.
+    # Assume that the observance bias affects the counts of covered and
+    # informative bases equally, so that we can define f_obs as follows:
+    # f_obs := ninfo_obs / ninfo_adj
+    # from which we can estimate the informative bases after adjustment:
+    # ninfo_adj = ninfo_obs / f_obs
+    ninfo_adj = counts_obs.loc[:, INFOR_REL] / f_obs
+    counts_adj.loc[:, INFOR_REL] = ninfo_adj
     counts_adj.loc[:, COVER_REL] = counts_obs.loc[:, COVER_REL] / f_obs
-    # Two conditions must be met:
-    # : The number of informative bases (matches + mutations) after
-    #   adjustment must equal the number before adjustment divided
-    #   by the fraction of reads that were observed:
-    #   (nrefs_adj + nmuts_adj) = (nrefs_obs + nmuts_obs) / f_obs
-    # : The fraction of mutations at each position after adjustment
-    #   must equal the adjusted number of mutations divided by the
-    #   adjusted number of informative bases:
-    #   nmuts_adj / (nrefs_adj + nmuts_adj) = fmuts_adj
-    # The two unknown variables (nrefs_adj and nmuts_adj) can be
-    # solved using the above system of two equations. By solving for
-    # (nrefs_adj + nmuts_adj) in both equations, we get:
-    # : (nrefs_adj + nmuts_adj) = (nrefs_obs + nmuts_obs) / f_obs
-    # : (nrefs_adj + nmuts_adj) = nmuts_adj / fmuts_adj {fmuts_adj > 0}
-    # Setting both right hand sides equal, nmuts_adj is solved:
-    # : (nrefs_obs + nmuts_obs) / f_obs = nmuts_adj / fmuts_adj
-    # : nmuts_adj = (nrefs_obs + nmuts_obs) * (fmuts_adj / f_obs)
-    nmuts_adj = ninfo_obs * (fmuts_adj / f_obs)
-    # Then, plugging this solution into the second equation:
-    # : nrefs_adj = nmuts_adj / fmuts_adj - nmuts_adj
-    #             = nmuts_adj * (1 / fmuts_adj - 1) {fmuts_adj > 0}
-    # If, on the other hand, fmuts_adj = 0, then
-    # : nmuts_adj = fmuts_adj * (nrefs_adj + nmuts_adj) = 0
-    # Thus, we solve for nrefs_adj using the first equation instead:
-    # : (nrefs_adj + nmuts_adj) = (nrefs_obs + nmuts_obs) / f_obs
-    # : nrefs_adj = nrefs_obs / f_obs
-    with np.errstate(divide="ignore"):
-        # Ignore division-by-zero warnings in np.reciprocal because
-        # positions where fmuts_adj = 0 are just skipped by np.where.
-        nrefs_adj = np.where(fmuts_adj > 0.,
-                             nmuts_adj * (np.reciprocal(fmuts_adj) - 1.),
-                             nrefs_obs / f_obs)
-        # Compute the factor by which nmuts was adjusted. Division by 0
-        # is possible if no mutations were observed, resulting in NaN
-        # values. Fill them with 1 so that the NaNs do not propagate
-        # when multiplying the number of mutations by nmuts_fac.
-        nmuts_fac = (nmuts_adj / nmuts_obs).fillna(1.)
-    counts_adj.loc[:, MATCH_REL] = nrefs_adj
+    # From the definition of the adjusted fraction of mutations:
+    # fmuts_adj := nmuts_adj / ninfo_adj
+    # we can also estimate the mutated bases after adjustment:
+    # nmuts_adj = fmuts_adj * ninfo_adj
+    nmuts_adj = fmuts_adj * ninfo_adj
     counts_adj.loc[:, MUTAT_REL] = nmuts_adj
-    # Adjust every type of mutation by this factor.
-    for mut in (SUBST_REL, SUB_A_REL, SUB_C_REL, SUB_G_REL, SUB_T_REL,
-                DELET_REL, INSRT_REL):
-        try:
-            counts_adj.loc[:, mut] = counts_obs.loc[:, mut] * nmuts_fac
-        except KeyError:
-            # The mutation was not in the table.
-            pass
+    # From the definition of informative bases:
+    # ninfo_adj := nrefs_adj + nmuts_adj
+    # we can estimate the matched bases after adjustment:
+    # nrefs_adj = ninfo_adj - nmuts_adj
+    nrefs_adj = ninfo_adj - nmuts_adj
+    counts_adj.loc[:, MATCH_REL] = nrefs_adj
+    # Compute the factor by which nmuts was adjusted for each position.
+    with np.errstate(divide="ignore"):
+        # Division by 0 is possible if no mutations were observed at a
+        # given position, resulting in a NaN value at that position.
+        adj_factor = nmuts_adj / counts_obs.loc[:, MUTAT_REL]
+    # So that the multiplication works properly, replace NaN values with
+    # 1 so that they do not propagate, then cast to a DataFrame so that
+    # the dimensions are correct.
+    adj_factor = adj_factor.fillna(1.).to_frame().values
+    # Adjust every subtype of mutation by this factor.
+    counts_adj.loc[:, SUBMUTS] = counts_obs.loc[:, SUBMUTS] * adj_factor
     return counts_adj
 
 
 def tabulate_loader(report_loader: RelateLoader | MaskLoader | ClustLoader,
                     rel_codes: str):
     """ Return a new DataLoader, choosing the subclass based on the type
     of the argument `report_loader`. """
```

### Comparing `seismic-rna-0.4.0/src/seismicrna/table/write.py` & `seismic-rna-0.4.1/src/seismicrna/table/write.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.4.0/src/seismicrna/test/main.py` & `seismic-rna-0.4.1/src/seismicrna/test/main.py`

 * *Files identical despite different names*

