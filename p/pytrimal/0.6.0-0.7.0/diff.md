# Comparing `tmp/pytrimal-0.6.0.tar.gz` & `tmp/pytrimal-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytrimal-0.6.0.tar", last modified: Sat Jun 24 10:15:16 2023, max compression
+gzip compressed data, was "pytrimal-0.7.0.tar", last modified: Fri Jul 21 18:59:43 2023, max compression
```

## Comparing `pytrimal-0.6.0.tar` & `pytrimal-0.7.0.tar`

### file list

```diff
@@ -1,344 +1,343 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 10:15:16.979654 pytrimal-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)     6595 2023-06-24 10:15:04.000000 pytrimal-0.6.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-06-24 10:15:04.000000 pytrimal-0.6.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-06-24 10:15:04.000000 pytrimal-0.6.0/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-06-24 10:15:04.000000 pytrimal-0.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    12722 2023-06-24 10:15:16.979654 pytrimal-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10931 2023-06-24 10:15:04.000000 pytrimal-0.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 10:15:16.887648 pytrimal-0.6.0/include/
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-06-24 10:15:04.000000 pytrimal-0.6.0/include/_unicode.pxd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 10:15:16.887648 pytrimal-0.6.0/include/cpu_features/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 10:15:04.000000 pytrimal-0.6.0/include/cpu_features/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-06-24 10:15:04.000000 pytrimal-0.6.0/include/cpu_features/aarch64.pxd
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-06-24 10:15:04.000000 pytrimal-0.6.0/include/cpu_features/arm.pxd
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-06-24 10:15:04.000000 pytrimal-0.6.0/include/cpu_features/x86.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-06-24 10:15:04.000000 pytrimal-0.6.0/include/iostream.pxd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 10:15:16.887648 pytrimal-0.6.0/include/trimal/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-24 10:15:04.000000 pytrimal-0.6.0/include/trimal/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-06-24 10:15:04.000000 pytrimal-0.6.0/include/trimal/alignment.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-06-24 10:15:04.000000 pytrimal-0.6.0/include/trimal/cleaner.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-06-24 10:15:04.000000 pytrimal-0.6.0/include/trimal/format_handling.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-06-24 10:15:04.000000 pytrimal-0.6.0/include/trimal/manager.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     8874 2023-06-24 10:15:04.000000 pytrimal-0.6.0/include/trimal/report_system.pxd
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-24 10:15:04.000000 pytrimal-0.6.0/include/trimal/sequences_matrix.pxd
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-24 10:15:04.000000 pytrimal-0.6.0/include/trimal/similarity_matrix.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-06-24 10:15:04.000000 pytrimal-0.6.0/include/trimal/statistics.pxd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 10:15:16.891649 pytrimal-0.6.0/patches/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-24 10:15:04.000000 pytrimal-0.6.0/patches/BaseFormatHandler.h.patch
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-24 10:15:04.000000 pytrimal-0.6.0/patches/Cleaner.cpp.patch
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-24 10:15:04.000000 pytrimal-0.6.0/patches/Cleaner.h.patch
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-24 10:15:04.000000 pytrimal-0.6.0/patches/Gaps.h.patch
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-06-24 10:15:04.000000 pytrimal-0.6.0/patches/Similarity.h.patch
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-06-24 10:15:04.000000 pytrimal-0.6.0/patches/clustal_state.cpp.patch
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-24 10:15:04.000000 pytrimal-0.6.0/patches/clustal_state.h.patch
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-24 10:15:04.000000 pytrimal-0.6.0/patches/fasta_m10_state.cpp.patch
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-24 10:15:04.000000 pytrimal-0.6.0/patches/fasta_m10_state.h.patch
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-06-24 10:15:04.000000 pytrimal-0.6.0/patches/fasta_state.cpp.patch
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-24 10:15:04.000000 pytrimal-0.6.0/patches/fasta_state.h.patch
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-24 10:15:04.000000 pytrimal-0.6.0/patches/htmlreport_state.cpp.patch
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-24 10:15:04.000000 pytrimal-0.6.0/patches/htmlreport_state.h.patch
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-24 10:15:04.000000 pytrimal-0.6.0/patches/mega_interleaved_state.cpp.patch
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-24 10:15:04.000000 pytrimal-0.6.0/patches/mega_interleaved_state.h.patch
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-24 10:15:04.000000 pytrimal-0.6.0/patches/mega_sequential_state.cpp.patch
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-24 10:15:04.000000 pytrimal-0.6.0/patches/mega_sequential_state.h.patch
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-24 10:15:04.000000 pytrimal-0.6.0/patches/nexus_m10_state.cpp.patch
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-24 10:15:04.000000 pytrimal-0.6.0/patches/nexus_m10_state.h.patch
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-06-24 10:15:04.000000 pytrimal-0.6.0/patches/nexus_state.cpp.patch
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-24 10:15:04.000000 pytrimal-0.6.0/patches/nexus_state.h.patch
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-24 10:15:04.000000 pytrimal-0.6.0/patches/phylip32_m10_state.cpp.patch
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-24 10:15:04.000000 pytrimal-0.6.0/patches/phylip32_m10_state.h.patch
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-06-24 10:15:04.000000 pytrimal-0.6.0/patches/phylip32_state.cpp.patch
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-24 10:15:04.000000 pytrimal-0.6.0/patches/phylip32_state.h.patch
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-24 10:15:04.000000 pytrimal-0.6.0/patches/phylip40_m10_state.cpp.patch
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-24 10:15:04.000000 pytrimal-0.6.0/patches/phylip40_m10_state.h.patch
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-06-24 10:15:04.000000 pytrimal-0.6.0/patches/phylip40_state.cpp.patch
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-24 10:15:04.000000 pytrimal-0.6.0/patches/phylip40_state.h.patch
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-24 10:15:04.000000 pytrimal-0.6.0/patches/phylip_paml_m10_state.cpp.patch
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-24 10:15:04.000000 pytrimal-0.6.0/patches/phylip_paml_m10_state.h.patch
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-24 10:15:04.000000 pytrimal-0.6.0/patches/phylip_paml_state.cpp.patch
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-24 10:15:04.000000 pytrimal-0.6.0/patches/phylip_paml_state.h.patch
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-06-24 10:15:04.000000 pytrimal-0.6.0/patches/pir_state.cpp.patch
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-24 10:15:04.000000 pytrimal-0.6.0/patches/pir_state.h.patch
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-24 10:15:04.000000 pytrimal-0.6.0/patches/similarityMatrix.h.patch
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-24 10:15:04.000000 pytrimal-0.6.0/patches/trimalManager.h.patch
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-24 10:15:16.000000 pytrimal-0.6.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 10:15:16.891649 pytrimal-0.6.0/pytrimal/
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-24 10:15:04.000000 pytrimal-0.6.0/pytrimal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-06-24 10:15:04.000000 pytrimal-0.6.0/pytrimal/_trimal.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     6424 2023-06-24 10:15:04.000000 pytrimal-0.6.0/pytrimal/_trimal.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    79527 2023-06-24 10:15:04.000000 pytrimal-0.6.0/pytrimal/_trimal.pyx
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-24 10:15:04.000000 pytrimal-0.6.0/pytrimal/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 10:15:16.891649 pytrimal-0.6.0/pytrimal/fileobj/
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-24 10:15:04.000000 pytrimal-0.6.0/pytrimal/fileobj/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-06-24 10:15:04.000000 pytrimal-0.6.0/pytrimal/fileobj/pyreadbuf.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-06-24 10:15:04.000000 pytrimal-0.6.0/pytrimal/fileobj/pyreadbuf.h
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-06-24 10:15:04.000000 pytrimal-0.6.0/pytrimal/fileobj/pyreadintobuf.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-06-24 10:15:04.000000 pytrimal-0.6.0/pytrimal/fileobj/pyreadintobuf.h
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-06-24 10:15:04.000000 pytrimal-0.6.0/pytrimal/fileobj/pywritebuf.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-06-24 10:15:04.000000 pytrimal-0.6.0/pytrimal/fileobj/pywritebuf.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 10:15:16.891649 pytrimal-0.6.0/pytrimal/impl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 10:15:04.000000 pytrimal-0.6.0/pytrimal/impl/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     3221 2023-06-24 10:15:04.000000 pytrimal-0.6.0/pytrimal/impl/avx.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-06-24 10:15:04.000000 pytrimal-0.6.0/pytrimal/impl/avx.h
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-06-24 10:15:04.000000 pytrimal-0.6.0/pytrimal/impl/avx.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     2883 2023-06-24 10:15:04.000000 pytrimal-0.6.0/pytrimal/impl/generic.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-06-24 10:15:04.000000 pytrimal-0.6.0/pytrimal/impl/generic.h
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-06-24 10:15:04.000000 pytrimal-0.6.0/pytrimal/impl/generic.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-06-24 10:15:04.000000 pytrimal-0.6.0/pytrimal/impl/mmx.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-06-24 10:15:04.000000 pytrimal-0.6.0/pytrimal/impl/mmx.h
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-06-24 10:15:04.000000 pytrimal-0.6.0/pytrimal/impl/mmx.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-06-24 10:15:04.000000 pytrimal-0.6.0/pytrimal/impl/neon.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-06-24 10:15:04.000000 pytrimal-0.6.0/pytrimal/impl/neon.h
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-06-24 10:15:04.000000 pytrimal-0.6.0/pytrimal/impl/neon.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-06-24 10:15:04.000000 pytrimal-0.6.0/pytrimal/impl/sse.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-06-24 10:15:04.000000 pytrimal-0.6.0/pytrimal/impl/sse.h
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-06-24 10:15:04.000000 pytrimal-0.6.0/pytrimal/impl/sse.pxd
--rw-r--r--   0 runner    (1001) docker     (123)    20527 2023-06-24 10:15:04.000000 pytrimal-0.6.0/pytrimal/impl/template.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 10:15:16.891649 pytrimal-0.6.0/pytrimal/patch/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 10:15:04.000000 pytrimal-0.6.0/pytrimal/patch/omp.h
--rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-06-24 10:15:04.000000 pytrimal-0.6.0/pytrimal/patch/reportsystem.cpp
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 10:15:04.000000 pytrimal-0.6.0/pytrimal/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 10:15:16.895649 pytrimal-0.6.0/pytrimal/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-24 10:15:04.000000 pytrimal-0.6.0/pytrimal/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-24 10:15:04.000000 pytrimal-0.6.0/pytrimal/tests/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-06-24 10:15:04.000000 pytrimal-0.6.0/pytrimal/tests/_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 10:15:16.899649 pytrimal-0.6.0/pytrimal/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)   178679 2023-06-24 10:15:04.000000 pytrimal-0.6.0/pytrimal/tests/data/ENOG411BWBU.automated1.fasta
--rw-r--r--   0 runner    (1001) docker     (123)    10138 2023-06-24 10:15:04.000000 pytrimal-0.6.0/pytrimal/tests/data/ENOG411BWBU.clusters10.fasta
--rw-r--r--   0 runner    (1001) docker     (123)     4892 2023-06-24 10:15:04.000000 pytrimal-0.6.0/pytrimal/tests/data/ENOG411BWBU.clusters5.fasta
--rw-r--r--   0 runner    (1001) docker     (123)   180351 2023-06-24 10:15:04.000000 pytrimal-0.6.0/pytrimal/tests/data/ENOG411BWBU.cons40.gt40.fasta
--rw-r--r--   0 runner    (1001) docker     (123)   161541 2023-06-24 10:15:04.000000 pytrimal-0.6.0/pytrimal/tests/data/ENOG411BWBU.cons60.gt90.fasta
--rw-r--r--   0 runner    (1001) docker     (123)   266668 2023-06-24 10:15:06.000000 pytrimal-0.6.0/pytrimal/tests/data/ENOG411BWBU.fasta
--rw-r--r--   0 runner    (1001) docker     (123)   178679 2023-06-24 10:15:04.000000 pytrimal-0.6.0/pytrimal/tests/data/ENOG411BWBU.gappyout.fasta
--rw-r--r--   0 runner    (1001) docker     (123)    13677 2023-06-24 10:15:04.000000 pytrimal-0.6.0/pytrimal/tests/data/ENOG411BWBU.id50.fasta
--rw-r--r--   0 runner    (1001) docker     (123)    73561 2023-06-24 10:15:04.000000 pytrimal-0.6.0/pytrimal/tests/data/ENOG411BWBU.id70.fasta
--rw-r--r--   0 runner    (1001) docker     (123)    97956 2023-06-24 10:15:04.000000 pytrimal-0.6.0/pytrimal/tests/data/ENOG411BWBU.maxidentity75.fasta
--rw-r--r--   0 runner    (1001) docker     (123)   265832 2023-06-24 10:15:04.000000 pytrimal-0.6.0/pytrimal/tests/data/ENOG411BWBU.noallgaps.fasta
--rw-r--r--   0 runner    (1001) docker     (123)   264560 2023-06-24 10:15:04.000000 pytrimal-0.6.0/pytrimal/tests/data/ENOG411BWBU.noduplicateseqs.fasta
--rw-r--r--   0 runner    (1001) docker     (123)   265832 2023-06-24 10:15:04.000000 pytrimal-0.6.0/pytrimal/tests/data/ENOG411BWBU.seq40.res60.fasta
--rw-r--r--   0 runner    (1001) docker     (123)   214721 2023-06-24 10:15:04.000000 pytrimal-0.6.0/pytrimal/tests/data/ENOG411BWBU.seq80.res80.fasta
--rw-r--r--   0 runner    (1001) docker     (123)   148792 2023-06-24 10:15:04.000000 pytrimal-0.6.0/pytrimal/tests/data/ENOG411BWBU.strict.fasta
--rw-r--r--   0 runner    (1001) docker     (123)   129773 2023-06-24 10:15:04.000000 pytrimal-0.6.0/pytrimal/tests/data/ENOG411BWBU.strictplus.fasta
--rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-06-24 10:15:04.000000 pytrimal-0.6.0/pytrimal/tests/data/PF12574.full.afa
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 10:15:04.000000 pytrimal-0.6.0/pytrimal/tests/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-06-24 10:15:06.000000 pytrimal-0.6.0/pytrimal/tests/data/example.001.AA.clw
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-24 10:15:04.000000 pytrimal-0.6.0/pytrimal/tests/data/example.001.gt90.w3.clw
--rw-r--r--   0 runner    (1001) docker     (123)   142966 2023-06-24 10:15:04.000000 pytrimal-0.6.0/pytrimal/tests/data/halorhodopsin.afa
--rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-06-24 10:15:04.000000 pytrimal-0.6.0/pytrimal/tests/data/pam70.json
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-24 10:15:04.000000 pytrimal-0.6.0/pytrimal/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)    14042 2023-06-24 10:15:04.000000 pytrimal-0.6.0/pytrimal/tests/test_alignment.py
--rw-r--r--   0 runner    (1001) docker     (123)     4712 2023-06-24 10:15:04.000000 pytrimal-0.6.0/pytrimal/tests/test_automatic_trimmer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3312 2023-06-24 10:15:04.000000 pytrimal-0.6.0/pytrimal/tests/test_doctest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4733 2023-06-24 10:15:04.000000 pytrimal-0.6.0/pytrimal/tests/test_manual_trimmer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-06-24 10:15:04.000000 pytrimal-0.6.0/pytrimal/tests/test_overlap_trimmer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-06-24 10:15:04.000000 pytrimal-0.6.0/pytrimal/tests/test_representative_trimmer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-06-24 10:15:04.000000 pytrimal-0.6.0/pytrimal/tests/test_similarity_matrix.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 10:15:16.891649 pytrimal-0.6.0/pytrimal.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12722 2023-06-24 10:15:16.000000 pytrimal-0.6.0/pytrimal.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14013 2023-06-24 10:15:16.000000 pytrimal-0.6.0/pytrimal.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 10:15:16.000000 pytrimal-0.6.0/pytrimal.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 10:15:16.000000 pytrimal-0.6.0/pytrimal.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-24 10:15:16.000000 pytrimal-0.6.0/pytrimal.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-24 10:15:16.000000 pytrimal-0.6.0/pytrimal.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-06-24 10:15:16.979654 pytrimal-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)    29800 2023-06-24 10:15:04.000000 pytrimal-0.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 10:15:16.883648 pytrimal-0.6.0/vendor/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 10:15:16.899649 pytrimal-0.6.0/vendor/trimal/
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)     6237 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/CHANGELOG
--rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 10:15:16.971654 pytrimal-0.6.0/vendor/trimal/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/alignments_comparison.1
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/alignments_comparison.2
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/alignments_comparison.3
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.001.AA.clw
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.001.AA.msl
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.001.AA.phy
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.002.AA.clw
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.002.AA.phy
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.003.AA.clw
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.004.AA.fasta
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.005.AA.fasta
--rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.006.AA.pir
--rw-r--r--   0 runner    (1001) docker     (123)    29920 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.007.AA.fasta
--rw-r--r--   0 runner    (1001) docker     (123)    14306 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.007.AA.only_seqs
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.009.AA.fasta
--rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.010.AA.fasta
--rw-r--r--   0 runner    (1001) docker     (123)    64904 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.011.AA.YKL197C.clw
--rw-r--r--   0 runner    (1001) docker     (123)    41006 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.011.AA.YKL197C.fasta
--rw-r--r--   0 runner    (1001) docker     (123)    40853 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.011.AA.YKL197C.phy
--rw-r--r--   0 runner    (1001) docker     (123)  2265147 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.012.AA.SuperAlignment.phy
--rw-r--r--   0 runner    (1001) docker     (123)  1246007 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.013.AA.SuperAlignment.phy
--rw-r--r--   0 runner    (1001) docker     (123) 26589443 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.014.AA.EggNOG.COG0591.fasta
--rw-r--r--   0 runner    (1001) docker     (123) 12097211 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.015.AA.bctoNOG.ENOG41099F3.fasta
--rw-r--r--   0 runner    (1001) docker     (123)   276588 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.016.AA.bctoNOG.ENOG41099FB.fasta
--rw-r--r--   0 runner    (1001) docker     (123)   138345 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.017.AA.bctoNOG.ENOG41099FJ.fasta
--rw-r--r--   0 runner    (1001) docker     (123)   203668 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.018.AA.bctoNOG.ENOG41099FV.fasta
--rw-r--r--   0 runner    (1001) docker     (123)   377416 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.019.AA.bctoNOG.ENOG41099HI.fasta
--rw-r--r--   0 runner    (1001) docker     (123)   453386 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.020.AA.bctoNOG.ENOG41099HN.fasta
--rw-r--r--   0 runner    (1001) docker     (123)   116996 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.021.AA.bctoNOG.ENOG41099I5.fasta
--rw-r--r--   0 runner    (1001) docker     (123)   155773 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.022.AA.bctoNOG.ENOG41099IZ.fasta
--rw-r--r--   0 runner    (1001) docker     (123)  2785573 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.023.AA.bctoNOG.ENOG41099K3.fasta
--rw-r--r--   0 runner    (1001) docker     (123)    13444 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.024.AA.bctoNOG.ENOG41099KM.fasta
--rw-r--r--   0 runner    (1001) docker     (123)  1608238 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.025.AA.bctoNOG.ENOG41099KP.fasta
--rw-r--r--   0 runner    (1001) docker     (123)   568299 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.026.AA.bctoNOG.ENOG41099MV.fasta
--rw-r--r--   0 runner    (1001) docker     (123)    50764 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.027.AA.bctoNOG.ENOG41099NY.fasta
--rw-r--r--   0 runner    (1001) docker     (123)   591641 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.028.AA.bctoNOG.ENOG41099PA.fasta
--rw-r--r--   0 runner    (1001) docker     (123)   139720 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.029.AA.bctoNOG.ENOG41099Q3.fasta
--rw-r--r--   0 runner    (1001) docker     (123)   186348 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.030.AA.bctoNOG.ENOG41099RG.fasta
--rw-r--r--   0 runner    (1001) docker     (123)   212250 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.031.AA.bctoNOG.ENOG41099UK.fasta
--rw-r--r--   0 runner    (1001) docker     (123)   387866 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.032.AA.bctoNOG.ENOG41099UW.fasta
--rw-r--r--   0 runner    (1001) docker     (123)   492698 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.033.AA.bctoNOG.ENOG41099VK.fasta
--rw-r--r--   0 runner    (1001) docker     (123)  1613156 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.034.AA.bctoNOG.ENOG41099WA.fasta
--rw-r--r--   0 runner    (1001) docker     (123)   610988 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.035.AA.bctoNOG.ENOG41099WF.fasta
--rw-r--r--   0 runner    (1001) docker     (123)   119286 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.036.AA.bctoNOG.ENOG41099XJ.fasta
--rw-r--r--   0 runner    (1001) docker     (123)   230484 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.037.AA.bctoNOG.ENOG41099XP.fasta
--rw-r--r--   0 runner    (1001) docker     (123)   261077 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.038.AA.bctoNOG.ENOG41099Y4.fasta
--rw-r--r--   0 runner    (1001) docker     (123)  3740628 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.039.AA.bctoNOG.ENOG41099YD.fasta
--rw-r--r--   0 runner    (1001) docker     (123)   506035 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.040.AA.bctoNOG.ENOG4109A32.fasta
--rw-r--r--   0 runner    (1001) docker     (123)    58122 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.041.AA.bctoNOG.ENOG4109A5T.fasta
--rw-r--r--   0 runner    (1001) docker     (123)    92703 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.042.AA.bctoNOG.ENOG4109A9M.fasta
--rw-r--r--   0 runner    (1001) docker     (123)    32257 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.043.AA.bctoNOG.ENOG4109ADN.fasta
--rw-r--r--   0 runner    (1001) docker     (123)    77067 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.044.AA.bctoNOG.ENOG4109AED.fasta
--rw-r--r--   0 runner    (1001) docker     (123)    22315 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.045.AA.bctoNOG.ENOG4109AGT.fasta
--rw-r--r--   0 runner    (1001) docker     (123)    22046 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.046.AA.bctoNOG.ENOG4109AGW.fasta
--rw-r--r--   0 runner    (1001) docker     (123)    22523 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.047.AA.bctoNOG.ENOG4109AIC.fasta
--rw-r--r--   0 runner    (1001) docker     (123)    15267 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.048.AA.bctoNOG.ENOG4109AJ3.fasta
--rw-r--r--   0 runner    (1001) docker     (123)    22263 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.049.AA.bctoNOG.ENOG4109AY5.fasta
--rw-r--r--   0 runner    (1001) docker     (123)    16768 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.050.AA.bctoNOG.ENOG4109B8Z.fasta
--rw-r--r--   0 runner    (1001) docker     (123)    35547 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.051.AA.bctoNOG.ENOG4109BCJ.fasta
--rw-r--r--   0 runner    (1001) docker     (123)    34229 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.052.AA.bctoNOG.ENOG4109CTU.fasta
--rw-r--r--   0 runner    (1001) docker     (123)    11810 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.053.AA.bctoNOG.ENOG4109CVC.fasta
--rw-r--r--   0 runner    (1001) docker     (123)    26156 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.054.AA.bctoNOG.ENOG4109FIT.fasta
--rw-r--r--   0 runner    (1001) docker     (123)     5970 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.055.AA.bctoNOG.ENOG4109GY9.fasta
--rw-r--r--   0 runner    (1001) docker     (123)    14878 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.056.AA.bctoNOG.ENOG4109IPJ.fasta
--rw-r--r--   0 runner    (1001) docker     (123)    55278 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.057.AA.bctoNOG.ENOG4109SZ2.fasta
--rw-r--r--   0 runner    (1001) docker     (123)    15249 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.058.AA.strNOG.ENOG411BBR6.fasta
--rw-r--r--   0 runner    (1001) docker     (123)    16927 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.059.AA.strNOG.ENOG411BBRR.fasta
--rw-r--r--   0 runner    (1001) docker     (123)    59625 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.060.AA.strNOG.ENOG411BBWK.fasta
--rw-r--r--   0 runner    (1001) docker     (123)    50162 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.061.AA.strNOG.ENOG411BCDZ.fasta
--rw-r--r--   0 runner    (1001) docker     (123)  1153350 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.062.AA.strNOG.ENOG411BCX3.fasta
--rw-r--r--   0 runner    (1001) docker     (123)    20437 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.063.AA.strNOG.ENOG411BDBU.fasta
--rw-r--r--   0 runner    (1001) docker     (123)   247440 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.064.AA.strNOG.ENOG411BDKC.fasta
--rw-r--r--   0 runner    (1001) docker     (123)    47806 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.065.AA.strNOG.ENOG411BDSZ.fasta
--rw-r--r--   0 runner    (1001) docker     (123)    27309 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.066.AA.strNOG.ENOG411BDUE.fasta
--rw-r--r--   0 runner    (1001) docker     (123)    51327 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.067.AA.strNOG.ENOG411BDX3.fasta
--rw-r--r--   0 runner    (1001) docker     (123)    16203 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.068.AA.strNOG.ENOG411BE45.fasta
--rw-r--r--   0 runner    (1001) docker     (123)    21963 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.069.AA.strNOG.ENOG411BE8B.fasta
--rw-r--r--   0 runner    (1001) docker     (123)    61363 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.070.AA.strNOG.ENOG411BEUV.fasta
--rw-r--r--   0 runner    (1001) docker     (123)    55532 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.071.AA.strNOG.ENOG411BEZ0.fasta
--rw-r--r--   0 runner    (1001) docker     (123)    11957 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.072.AA.strNOG.ENOG411BF1S.fasta
--rw-r--r--   0 runner    (1001) docker     (123)  2483264 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.073.AA.strNOG.ENOG411BFCW.fasta
--rw-r--r--   0 runner    (1001) docker     (123)    25440 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.074.AA.strNOG.ENOG411BFPF.fasta
--rw-r--r--   0 runner    (1001) docker     (123)    19199 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.075.AA.strNOG.ENOG411BFQS.fasta
--rw-r--r--   0 runner    (1001) docker     (123)    33482 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.076.AA.strNOG.ENOG411BH75.fasta
--rw-r--r--   0 runner    (1001) docker     (123)    72534 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.077.AA.strNOG.ENOG411BH79.fasta
--rw-r--r--   0 runner    (1001) docker     (123)    44284 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.078.AA.strNOG.ENOG411BH99.fasta
--rw-r--r--   0 runner    (1001) docker     (123)    13755 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.079.AA.strNOG.ENOG411BJDC.fasta
--rw-r--r--   0 runner    (1001) docker     (123)    23290 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.080.AA.strNOG.ENOG411BJIF.fasta
--rw-r--r--   0 runner    (1001) docker     (123)    12036 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.081.AA.strNOG.ENOG411BK9X.fasta
--rw-r--r--   0 runner    (1001) docker     (123)    26165 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.082.AA.strNOG.ENOG411BKC5.fasta
--rw-r--r--   0 runner    (1001) docker     (123)    13968 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.083.AA.strNOG.ENOG411BMKC.fasta
--rw-r--r--   0 runner    (1001) docker     (123)    10016 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.084.AA.strNOG.ENOG411BNP9.fasta
--rw-r--r--   0 runner    (1001) docker     (123)    10739 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.085.AA.strNOG.ENOG411BQTJ.fasta
--rw-r--r--   0 runner    (1001) docker     (123)    25977 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.086.AA.strNOG.ENOG411BR1D.fasta
--rw-r--r--   0 runner    (1001) docker     (123)     7768 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.087.AA.strNOG.ENOG411BRCH.fasta
--rw-r--r--   0 runner    (1001) docker     (123)    15763 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.088.AA.strNOG.ENOG411BSXF.fasta
--rw-r--r--   0 runner    (1001) docker     (123)    11736 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.089.AA.strNOG.ENOG411BV9B.fasta
--rw-r--r--   0 runner    (1001) docker     (123)  1574791 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.090.AA.strNOG.ENOG411BVKR.fasta
--rw-r--r--   0 runner    (1001) docker     (123)   473273 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.091.AA.strNOG.ENOG411BWBU.codon.fa
--rw-r--r--   0 runner    (1001) docker     (123)   266668 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.091.AA.strNOG.ENOG411BWBU.fasta
--rw-r--r--   0 runner    (1001) docker     (123)     4890 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.092.DNA.fasta
--rw-r--r--   0 runner    (1001) docker     (123)     4848 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.093.DNA.fasta
--rw-r--r--   0 runner    (1001) docker     (123)    10293 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/example.094.DNADeg.sequential_phy
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/matrix.BLOSUM62
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/dataset/matrix.Degenerated_DNA
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 10:15:16.971654 pytrimal-0.6.0/vendor/trimal/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 10:15:16.971654 pytrimal-0.6.0/vendor/trimal/include/Alignment/
--rw-r--r--   0 runner    (1001) docker     (123)     3823 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/include/Alignment/Alignment.h
--rw-r--r--   0 runner    (1001) docker     (123)     5402 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/include/Alignment/sequencesMatrix.h
--rw-r--r--   0 runner    (1001) docker     (123)    20122 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/include/Cleaner.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 10:15:16.971654 pytrimal-0.6.0/vendor/trimal/include/FormatHandling/
--rw-r--r--   0 runner    (1001) docker     (123)     4572 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/include/FormatHandling/BaseFormatHandler.h
--rw-r--r--   0 runner    (1001) docker     (123)     8554 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/include/FormatHandling/FormatManager.h
--rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/include/FormatHandling/clustal_state.h
--rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/include/FormatHandling/fasta_m10_state.h
--rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/include/FormatHandling/fasta_state.h
--rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/include/FormatHandling/formats_header.h
--rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/include/FormatHandling/htmlreport_state.h
--rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/include/FormatHandling/mega_interleaved_state.h
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/include/FormatHandling/mega_sequential_state.h
--rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/include/FormatHandling/nexus_m10_state.h
--rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/include/FormatHandling/nexus_state.h
--rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/include/FormatHandling/phylip32_m10_state.h
--rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/include/FormatHandling/phylip32_state.h
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/include/FormatHandling/phylip40_m10_state.h
--rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/include/FormatHandling/phylip40_state.h
--rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/include/FormatHandling/phylip_paml_m10_state.h
--rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/include/FormatHandling/phylip_paml_state.h
--rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/include/FormatHandling/pir_state.h
--rw-r--r--   0 runner    (1001) docker     (123)     4773 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/include/InternalBenchmarker.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 10:15:16.971654 pytrimal-0.6.0/vendor/trimal/include/RawText/
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/include/RawText/examples.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11662 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/include/RawText/legacyMenu.txt
--rw-r--r--   0 runner    (1001) docker     (123)    13285 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/include/RawText/menu.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 10:15:16.975654 pytrimal-0.6.0/vendor/trimal/include/Statistics/
--rw-r--r--   0 runner    (1001) docker     (123)     7931 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/include/Statistics/Consistency.h
--rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/include/Statistics/Gaps.h
--rw-r--r--   0 runner    (1001) docker     (123)     4871 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/include/Statistics/Manager.h
--rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/include/Statistics/Mold.h
--rw-r--r--   0 runner    (1001) docker     (123)     4935 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/include/Statistics/Similarity.h
--rw-r--r--   0 runner    (1001) docker     (123)     4262 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/include/Statistics/similarityMatrix.h
--rw-r--r--   0 runner    (1001) docker     (123)     9689 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/include/VCFHandler.h
--rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/include/defines.h
--rw-r--r--   0 runner    (1001) docker     (123)    18611 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/include/reportsystem.h
--rw-r--r--   0 runner    (1001) docker     (123)    13715 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/include/trimalManager.h
--rw-r--r--   0 runner    (1001) docker     (123)    15362 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/include/utils.h
--rw-r--r--   0 runner    (1001) docker     (123)     6542 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/include/values.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 10:15:16.975654 pytrimal-0.6.0/vendor/trimal/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 10:15:16.975654 pytrimal-0.6.0/vendor/trimal/source/Alignment/
--rw-r--r--   0 runner    (1001) docker     (123)   100282 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/source/Alignment/Alignment.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     8035 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/source/Alignment/sequencesMatrix.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    66998 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/source/Cleaner.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 10:15:16.975654 pytrimal-0.6.0/vendor/trimal/source/FormatHandling/
--rw-r--r--   0 runner    (1001) docker     (123)    12834 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/source/FormatHandling/BaseFormatHandler.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    10418 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/source/FormatHandling/clustal_state.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/source/FormatHandling/fasta_m10_state.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     7827 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/source/FormatHandling/fasta_state.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5265 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/source/FormatHandling/htmlreport_state.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     8309 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/source/FormatHandling/mega_interleaved_state.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    11393 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/source/FormatHandling/mega_sequential_state.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6813 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/source/FormatHandling/nexus_m10_state.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    11783 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/source/FormatHandling/nexus_state.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4753 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/source/FormatHandling/phylip32_m10_state.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    11330 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/source/FormatHandling/phylip32_state.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4832 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/source/FormatHandling/phylip40_m10_state.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    10907 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/source/FormatHandling/phylip40_state.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3927 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/source/FormatHandling/phylip_paml_m10_state.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/source/FormatHandling/phylip_paml_state.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     8406 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/source/FormatHandling/pir_state.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    16449 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/source/FormatHandling/readAlMain.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6977 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/source/InternalBenchmarker.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 10:15:16.979654 pytrimal-0.6.0/vendor/trimal/source/Statistics/
--rw-r--r--   0 runner    (1001) docker     (123)    32843 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/source/Statistics/Consistency.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    24994 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/source/Statistics/Gaps.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     7798 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/source/Statistics/Manager.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    13643 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/source/Statistics/Mold.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    24884 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/source/Statistics/Similarity.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    16144 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/source/Statistics/similarityMatrix.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    25928 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/source/VCFHandler.cpp
--rw-r--r--   0 runner    (1001) docker     (123)   126562 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/source/alignment.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    21325 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/source/compareFiles.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    90551 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/source/main.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 10:15:16.979654 pytrimal-0.6.0/vendor/trimal/source/reportMessages/
--rw-r--r--   0 runner    (1001) docker     (123)    17145 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/source/reportMessages/errorMessages.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/source/reportMessages/infoMessages.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/source/reportMessages/warningMessages.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     8144 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/source/reportsystem.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    71034 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/source/rwAlignment.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/source/trimAlMain.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    84059 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/source/trimalManager.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/source/typeHelper.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    30036 2023-06-24 10:15:06.000000 pytrimal-0.6.0/vendor/trimal/source/utils.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:59:43.055949 pytrimal-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     6744 2023-07-21 18:59:27.000000 pytrimal-0.7.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-07-21 18:59:27.000000 pytrimal-0.7.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-07-21 18:59:27.000000 pytrimal-0.7.0/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-21 18:59:27.000000 pytrimal-0.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    12634 2023-07-21 18:59:43.055949 pytrimal-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10843 2023-07-21 18:59:27.000000 pytrimal-0.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:59:42.935945 pytrimal-0.7.0/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:59:42.935945 pytrimal-0.7.0/include/cpu_features/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 18:59:27.000000 pytrimal-0.7.0/include/cpu_features/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-07-21 18:59:27.000000 pytrimal-0.7.0/include/cpu_features/aarch64.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-07-21 18:59:27.000000 pytrimal-0.7.0/include/cpu_features/arm.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-07-21 18:59:27.000000 pytrimal-0.7.0/include/cpu_features/x86.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-07-21 18:59:27.000000 pytrimal-0.7.0/include/iostream.pxd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:59:42.935945 pytrimal-0.7.0/include/trimal/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-21 18:59:27.000000 pytrimal-0.7.0/include/trimal/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-07-21 18:59:27.000000 pytrimal-0.7.0/include/trimal/alignment.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-07-21 18:59:27.000000 pytrimal-0.7.0/include/trimal/cleaner.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-07-21 18:59:27.000000 pytrimal-0.7.0/include/trimal/format_handling.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-07-21 18:59:27.000000 pytrimal-0.7.0/include/trimal/manager.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     8874 2023-07-21 18:59:27.000000 pytrimal-0.7.0/include/trimal/report_system.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-21 18:59:27.000000 pytrimal-0.7.0/include/trimal/sequences_matrix.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-07-21 18:59:27.000000 pytrimal-0.7.0/include/trimal/similarity_matrix.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-07-21 18:59:27.000000 pytrimal-0.7.0/include/trimal/statistics.pxd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:59:42.943946 pytrimal-0.7.0/patches/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-21 18:59:27.000000 pytrimal-0.7.0/patches/BaseFormatHandler.h.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-21 18:59:27.000000 pytrimal-0.7.0/patches/Cleaner.cpp.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-21 18:59:27.000000 pytrimal-0.7.0/patches/Cleaner.h.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-21 18:59:27.000000 pytrimal-0.7.0/patches/Gaps.h.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-21 18:59:27.000000 pytrimal-0.7.0/patches/Similarity.h.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-07-21 18:59:27.000000 pytrimal-0.7.0/patches/clustal_state.cpp.patch
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-21 18:59:27.000000 pytrimal-0.7.0/patches/clustal_state.h.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-21 18:59:27.000000 pytrimal-0.7.0/patches/fasta_m10_state.cpp.patch
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-21 18:59:27.000000 pytrimal-0.7.0/patches/fasta_m10_state.h.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-21 18:59:27.000000 pytrimal-0.7.0/patches/fasta_state.cpp.patch
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-21 18:59:27.000000 pytrimal-0.7.0/patches/fasta_state.h.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-21 18:59:27.000000 pytrimal-0.7.0/patches/htmlreport_state.cpp.patch
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-21 18:59:27.000000 pytrimal-0.7.0/patches/htmlreport_state.h.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-21 18:59:27.000000 pytrimal-0.7.0/patches/mega_interleaved_state.cpp.patch
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-21 18:59:27.000000 pytrimal-0.7.0/patches/mega_interleaved_state.h.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-21 18:59:27.000000 pytrimal-0.7.0/patches/mega_sequential_state.cpp.patch
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-21 18:59:27.000000 pytrimal-0.7.0/patches/mega_sequential_state.h.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-21 18:59:27.000000 pytrimal-0.7.0/patches/nexus_m10_state.cpp.patch
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-21 18:59:27.000000 pytrimal-0.7.0/patches/nexus_m10_state.h.patch
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-07-21 18:59:27.000000 pytrimal-0.7.0/patches/nexus_state.cpp.patch
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-21 18:59:27.000000 pytrimal-0.7.0/patches/nexus_state.h.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-21 18:59:27.000000 pytrimal-0.7.0/patches/phylip32_m10_state.cpp.patch
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-21 18:59:27.000000 pytrimal-0.7.0/patches/phylip32_m10_state.h.patch
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-07-21 18:59:27.000000 pytrimal-0.7.0/patches/phylip32_state.cpp.patch
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-21 18:59:27.000000 pytrimal-0.7.0/patches/phylip32_state.h.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-21 18:59:27.000000 pytrimal-0.7.0/patches/phylip40_m10_state.cpp.patch
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-21 18:59:27.000000 pytrimal-0.7.0/patches/phylip40_m10_state.h.patch
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-07-21 18:59:27.000000 pytrimal-0.7.0/patches/phylip40_state.cpp.patch
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-21 18:59:27.000000 pytrimal-0.7.0/patches/phylip40_state.h.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-21 18:59:27.000000 pytrimal-0.7.0/patches/phylip_paml_m10_state.cpp.patch
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-21 18:59:27.000000 pytrimal-0.7.0/patches/phylip_paml_m10_state.h.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-21 18:59:27.000000 pytrimal-0.7.0/patches/phylip_paml_state.cpp.patch
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-21 18:59:27.000000 pytrimal-0.7.0/patches/phylip_paml_state.h.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-21 18:59:27.000000 pytrimal-0.7.0/patches/pir_state.cpp.patch
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-21 18:59:27.000000 pytrimal-0.7.0/patches/pir_state.h.patch
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-21 18:59:27.000000 pytrimal-0.7.0/patches/similarityMatrix.h.patch
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-21 18:59:27.000000 pytrimal-0.7.0/patches/trimalManager.h.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-21 18:59:42.000000 pytrimal-0.7.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:59:42.943946 pytrimal-0.7.0/pytrimal/
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-07-21 18:59:27.000000 pytrimal-0.7.0/pytrimal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-07-21 18:59:27.000000 pytrimal-0.7.0/pytrimal/_trimal.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     6424 2023-07-21 18:59:27.000000 pytrimal-0.7.0/pytrimal/_trimal.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    80499 2023-07-21 18:59:27.000000 pytrimal-0.7.0/pytrimal/_trimal.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-21 18:59:27.000000 pytrimal-0.7.0/pytrimal/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:59:42.943946 pytrimal-0.7.0/pytrimal/fileobj/
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-21 18:59:27.000000 pytrimal-0.7.0/pytrimal/fileobj/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-07-21 18:59:27.000000 pytrimal-0.7.0/pytrimal/fileobj/pyreadbuf.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-21 18:59:27.000000 pytrimal-0.7.0/pytrimal/fileobj/pyreadbuf.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-07-21 18:59:27.000000 pytrimal-0.7.0/pytrimal/fileobj/pyreadintobuf.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-07-21 18:59:27.000000 pytrimal-0.7.0/pytrimal/fileobj/pyreadintobuf.h
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-21 18:59:27.000000 pytrimal-0.7.0/pytrimal/fileobj/pywritebuf.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-21 18:59:27.000000 pytrimal-0.7.0/pytrimal/fileobj/pywritebuf.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:59:42.947946 pytrimal-0.7.0/pytrimal/impl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 18:59:27.000000 pytrimal-0.7.0/pytrimal/impl/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     3221 2023-07-21 18:59:27.000000 pytrimal-0.7.0/pytrimal/impl/avx.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-07-21 18:59:27.000000 pytrimal-0.7.0/pytrimal/impl/avx.h
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-07-21 18:59:27.000000 pytrimal-0.7.0/pytrimal/impl/avx.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     2883 2023-07-21 18:59:27.000000 pytrimal-0.7.0/pytrimal/impl/generic.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-07-21 18:59:27.000000 pytrimal-0.7.0/pytrimal/impl/generic.h
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-07-21 18:59:27.000000 pytrimal-0.7.0/pytrimal/impl/generic.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-07-21 18:59:27.000000 pytrimal-0.7.0/pytrimal/impl/mmx.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-07-21 18:59:27.000000 pytrimal-0.7.0/pytrimal/impl/mmx.h
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-07-21 18:59:27.000000 pytrimal-0.7.0/pytrimal/impl/mmx.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-07-21 18:59:27.000000 pytrimal-0.7.0/pytrimal/impl/neon.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-07-21 18:59:27.000000 pytrimal-0.7.0/pytrimal/impl/neon.h
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-07-21 18:59:27.000000 pytrimal-0.7.0/pytrimal/impl/neon.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-07-21 18:59:27.000000 pytrimal-0.7.0/pytrimal/impl/sse.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-07-21 18:59:27.000000 pytrimal-0.7.0/pytrimal/impl/sse.h
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-07-21 18:59:27.000000 pytrimal-0.7.0/pytrimal/impl/sse.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    20527 2023-07-21 18:59:27.000000 pytrimal-0.7.0/pytrimal/impl/template.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:59:42.947946 pytrimal-0.7.0/pytrimal/patch/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 18:59:27.000000 pytrimal-0.7.0/pytrimal/patch/omp.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-07-21 18:59:27.000000 pytrimal-0.7.0/pytrimal/patch/reportsystem.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 18:59:27.000000 pytrimal-0.7.0/pytrimal/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:59:42.951946 pytrimal-0.7.0/pytrimal/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-07-21 18:59:27.000000 pytrimal-0.7.0/pytrimal/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-21 18:59:27.000000 pytrimal-0.7.0/pytrimal/tests/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-07-21 18:59:27.000000 pytrimal-0.7.0/pytrimal/tests/_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:59:42.955946 pytrimal-0.7.0/pytrimal/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   178679 2023-07-21 18:59:27.000000 pytrimal-0.7.0/pytrimal/tests/data/ENOG411BWBU.automated1.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)    10138 2023-07-21 18:59:27.000000 pytrimal-0.7.0/pytrimal/tests/data/ENOG411BWBU.clusters10.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)     4892 2023-07-21 18:59:27.000000 pytrimal-0.7.0/pytrimal/tests/data/ENOG411BWBU.clusters5.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)   180351 2023-07-21 18:59:27.000000 pytrimal-0.7.0/pytrimal/tests/data/ENOG411BWBU.cons40.gt40.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)   161541 2023-07-21 18:59:27.000000 pytrimal-0.7.0/pytrimal/tests/data/ENOG411BWBU.cons60.gt90.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)   266668 2023-07-21 18:59:31.000000 pytrimal-0.7.0/pytrimal/tests/data/ENOG411BWBU.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)   178679 2023-07-21 18:59:27.000000 pytrimal-0.7.0/pytrimal/tests/data/ENOG411BWBU.gappyout.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)    13677 2023-07-21 18:59:27.000000 pytrimal-0.7.0/pytrimal/tests/data/ENOG411BWBU.id50.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)    73561 2023-07-21 18:59:27.000000 pytrimal-0.7.0/pytrimal/tests/data/ENOG411BWBU.id70.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)    97956 2023-07-21 18:59:27.000000 pytrimal-0.7.0/pytrimal/tests/data/ENOG411BWBU.maxidentity75.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)   265832 2023-07-21 18:59:27.000000 pytrimal-0.7.0/pytrimal/tests/data/ENOG411BWBU.noallgaps.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)   264560 2023-07-21 18:59:27.000000 pytrimal-0.7.0/pytrimal/tests/data/ENOG411BWBU.noduplicateseqs.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)   265832 2023-07-21 18:59:27.000000 pytrimal-0.7.0/pytrimal/tests/data/ENOG411BWBU.seq40.res60.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)   214721 2023-07-21 18:59:27.000000 pytrimal-0.7.0/pytrimal/tests/data/ENOG411BWBU.seq80.res80.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)   148792 2023-07-21 18:59:27.000000 pytrimal-0.7.0/pytrimal/tests/data/ENOG411BWBU.strict.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)   129773 2023-07-21 18:59:27.000000 pytrimal-0.7.0/pytrimal/tests/data/ENOG411BWBU.strictplus.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-07-21 18:59:27.000000 pytrimal-0.7.0/pytrimal/tests/data/PF12574.full.afa
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 18:59:27.000000 pytrimal-0.7.0/pytrimal/tests/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-07-21 18:59:31.000000 pytrimal-0.7.0/pytrimal/tests/data/example.001.AA.clw
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-21 18:59:27.000000 pytrimal-0.7.0/pytrimal/tests/data/example.001.gt90.w3.clw
+-rw-r--r--   0 runner    (1001) docker     (123)   142966 2023-07-21 18:59:27.000000 pytrimal-0.7.0/pytrimal/tests/data/halorhodopsin.afa
+-rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-07-21 18:59:27.000000 pytrimal-0.7.0/pytrimal/tests/data/pam70.json
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-21 18:59:27.000000 pytrimal-0.7.0/pytrimal/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14042 2023-07-21 18:59:27.000000 pytrimal-0.7.0/pytrimal/tests/test_alignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4712 2023-07-21 18:59:27.000000 pytrimal-0.7.0/pytrimal/tests/test_automatic_trimmer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3312 2023-07-21 18:59:27.000000 pytrimal-0.7.0/pytrimal/tests/test_doctest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4733 2023-07-21 18:59:27.000000 pytrimal-0.7.0/pytrimal/tests/test_manual_trimmer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-07-21 18:59:27.000000 pytrimal-0.7.0/pytrimal/tests/test_overlap_trimmer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-07-21 18:59:27.000000 pytrimal-0.7.0/pytrimal/tests/test_representative_trimmer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-07-21 18:59:27.000000 pytrimal-0.7.0/pytrimal/tests/test_similarity_matrix.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:59:42.943946 pytrimal-0.7.0/pytrimal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12634 2023-07-21 18:59:42.000000 pytrimal-0.7.0/pytrimal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13992 2023-07-21 18:59:42.000000 pytrimal-0.7.0/pytrimal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 18:59:42.000000 pytrimal-0.7.0/pytrimal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 18:59:42.000000 pytrimal-0.7.0/pytrimal.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-21 18:59:42.000000 pytrimal-0.7.0/pytrimal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-21 18:59:42.000000 pytrimal-0.7.0/pytrimal.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-07-21 18:59:43.059949 pytrimal-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)    29892 2023-07-21 18:59:27.000000 pytrimal-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:59:42.931945 pytrimal-0.7.0/vendor/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:59:42.955946 pytrimal-0.7.0/vendor/trimal/
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)     6237 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/CHANGELOG
+-rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:59:43.043949 pytrimal-0.7.0/vendor/trimal/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/dataset/alignments_comparison.1
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/dataset/alignments_comparison.2
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/dataset/alignments_comparison.3
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/dataset/example.001.AA.clw
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/dataset/example.001.AA.msl
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/dataset/example.001.AA.phy
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/dataset/example.002.AA.clw
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/dataset/example.002.AA.phy
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/dataset/example.003.AA.clw
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/dataset/example.004.AA.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/dataset/example.005.AA.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/dataset/example.006.AA.pir
+-rw-r--r--   0 runner    (1001) docker     (123)    29920 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/dataset/example.007.AA.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)    14306 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/dataset/example.007.AA.only_seqs
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/dataset/example.009.AA.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/dataset/example.010.AA.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)    64904 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/dataset/example.011.AA.YKL197C.clw
+-rw-r--r--   0 runner    (1001) docker     (123)    41006 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/dataset/example.011.AA.YKL197C.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)    40853 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/dataset/example.011.AA.YKL197C.phy
+-rw-r--r--   0 runner    (1001) docker     (123)  2265147 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/dataset/example.012.AA.SuperAlignment.phy
+-rw-r--r--   0 runner    (1001) docker     (123)  1246007 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/dataset/example.013.AA.SuperAlignment.phy
+-rw-r--r--   0 runner    (1001) docker     (123) 26589443 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/dataset/example.014.AA.EggNOG.COG0591.fasta
+-rw-r--r--   0 runner    (1001) docker     (123) 12097211 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/dataset/example.015.AA.bctoNOG.ENOG41099F3.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)   276588 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/dataset/example.016.AA.bctoNOG.ENOG41099FB.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)   138345 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/dataset/example.017.AA.bctoNOG.ENOG41099FJ.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)   203668 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/dataset/example.018.AA.bctoNOG.ENOG41099FV.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)   377416 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/dataset/example.019.AA.bctoNOG.ENOG41099HI.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)   453386 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/dataset/example.020.AA.bctoNOG.ENOG41099HN.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)   116996 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/dataset/example.021.AA.bctoNOG.ENOG41099I5.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)   155773 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/dataset/example.022.AA.bctoNOG.ENOG41099IZ.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)  2785573 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/dataset/example.023.AA.bctoNOG.ENOG41099K3.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)    13444 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/dataset/example.024.AA.bctoNOG.ENOG41099KM.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)  1608238 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/dataset/example.025.AA.bctoNOG.ENOG41099KP.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)   568299 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/dataset/example.026.AA.bctoNOG.ENOG41099MV.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)    50764 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/dataset/example.027.AA.bctoNOG.ENOG41099NY.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)   591641 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/dataset/example.028.AA.bctoNOG.ENOG41099PA.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)   139720 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/dataset/example.029.AA.bctoNOG.ENOG41099Q3.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)   186348 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/dataset/example.030.AA.bctoNOG.ENOG41099RG.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)   212250 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/dataset/example.031.AA.bctoNOG.ENOG41099UK.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)   387866 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/dataset/example.032.AA.bctoNOG.ENOG41099UW.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)   492698 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/dataset/example.033.AA.bctoNOG.ENOG41099VK.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)  1613156 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/dataset/example.034.AA.bctoNOG.ENOG41099WA.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)   610988 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/dataset/example.035.AA.bctoNOG.ENOG41099WF.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)   119286 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/dataset/example.036.AA.bctoNOG.ENOG41099XJ.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)   230484 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/dataset/example.037.AA.bctoNOG.ENOG41099XP.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)   261077 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/dataset/example.038.AA.bctoNOG.ENOG41099Y4.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)  3740628 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/dataset/example.039.AA.bctoNOG.ENOG41099YD.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)   506035 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/dataset/example.040.AA.bctoNOG.ENOG4109A32.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)    58122 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/dataset/example.041.AA.bctoNOG.ENOG4109A5T.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)    92703 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/dataset/example.042.AA.bctoNOG.ENOG4109A9M.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)    32257 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/dataset/example.043.AA.bctoNOG.ENOG4109ADN.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)    77067 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/dataset/example.044.AA.bctoNOG.ENOG4109AED.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)    22315 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/dataset/example.045.AA.bctoNOG.ENOG4109AGT.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)    22046 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/dataset/example.046.AA.bctoNOG.ENOG4109AGW.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)    22523 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/dataset/example.047.AA.bctoNOG.ENOG4109AIC.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)    15267 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/dataset/example.048.AA.bctoNOG.ENOG4109AJ3.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)    22263 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/dataset/example.049.AA.bctoNOG.ENOG4109AY5.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)    16768 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/dataset/example.050.AA.bctoNOG.ENOG4109B8Z.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)    35547 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/dataset/example.051.AA.bctoNOG.ENOG4109BCJ.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)    34229 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/dataset/example.052.AA.bctoNOG.ENOG4109CTU.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)    11810 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/dataset/example.053.AA.bctoNOG.ENOG4109CVC.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)    26156 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/dataset/example.054.AA.bctoNOG.ENOG4109FIT.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)     5970 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/dataset/example.055.AA.bctoNOG.ENOG4109GY9.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)    14878 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/dataset/example.056.AA.bctoNOG.ENOG4109IPJ.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)    55278 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/dataset/example.057.AA.bctoNOG.ENOG4109SZ2.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)    15249 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/dataset/example.058.AA.strNOG.ENOG411BBR6.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)    16927 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/dataset/example.059.AA.strNOG.ENOG411BBRR.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)    59625 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/dataset/example.060.AA.strNOG.ENOG411BBWK.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)    50162 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/dataset/example.061.AA.strNOG.ENOG411BCDZ.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)  1153350 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/dataset/example.062.AA.strNOG.ENOG411BCX3.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)    20437 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/dataset/example.063.AA.strNOG.ENOG411BDBU.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)   247440 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/dataset/example.064.AA.strNOG.ENOG411BDKC.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)    47806 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/dataset/example.065.AA.strNOG.ENOG411BDSZ.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)    27309 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/dataset/example.066.AA.strNOG.ENOG411BDUE.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)    51327 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/dataset/example.067.AA.strNOG.ENOG411BDX3.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)    16203 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/dataset/example.068.AA.strNOG.ENOG411BE45.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)    21963 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/dataset/example.069.AA.strNOG.ENOG411BE8B.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)    61363 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/dataset/example.070.AA.strNOG.ENOG411BEUV.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)    55532 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/dataset/example.071.AA.strNOG.ENOG411BEZ0.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)    11957 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/dataset/example.072.AA.strNOG.ENOG411BF1S.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)  2483264 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/dataset/example.073.AA.strNOG.ENOG411BFCW.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)    25440 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/dataset/example.074.AA.strNOG.ENOG411BFPF.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)    19199 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/dataset/example.075.AA.strNOG.ENOG411BFQS.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)    33482 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/dataset/example.076.AA.strNOG.ENOG411BH75.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)    72534 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/dataset/example.077.AA.strNOG.ENOG411BH79.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)    44284 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/dataset/example.078.AA.strNOG.ENOG411BH99.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)    13755 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/dataset/example.079.AA.strNOG.ENOG411BJDC.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)    23290 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/dataset/example.080.AA.strNOG.ENOG411BJIF.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)    12036 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/dataset/example.081.AA.strNOG.ENOG411BK9X.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)    26165 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/dataset/example.082.AA.strNOG.ENOG411BKC5.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)    13968 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/dataset/example.083.AA.strNOG.ENOG411BMKC.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)    10016 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/dataset/example.084.AA.strNOG.ENOG411BNP9.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)    10739 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/dataset/example.085.AA.strNOG.ENOG411BQTJ.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)    25977 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/dataset/example.086.AA.strNOG.ENOG411BR1D.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)     7768 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/dataset/example.087.AA.strNOG.ENOG411BRCH.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)    15763 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/dataset/example.088.AA.strNOG.ENOG411BSXF.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)    11736 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/dataset/example.089.AA.strNOG.ENOG411BV9B.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)  1574791 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/dataset/example.090.AA.strNOG.ENOG411BVKR.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)   473273 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/dataset/example.091.AA.strNOG.ENOG411BWBU.codon.fa
+-rw-r--r--   0 runner    (1001) docker     (123)   266668 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/dataset/example.091.AA.strNOG.ENOG411BWBU.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)     4890 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/dataset/example.092.DNA.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)     4848 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/dataset/example.093.DNA.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)    10293 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/dataset/example.094.DNADeg.sequential_phy
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/dataset/matrix.BLOSUM62
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/dataset/matrix.Degenerated_DNA
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:59:43.043949 pytrimal-0.7.0/vendor/trimal/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:59:43.043949 pytrimal-0.7.0/vendor/trimal/include/Alignment/
+-rw-r--r--   0 runner    (1001) docker     (123)     3823 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/include/Alignment/Alignment.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5402 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/include/Alignment/sequencesMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (123)    20122 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/include/Cleaner.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:59:43.047949 pytrimal-0.7.0/vendor/trimal/include/FormatHandling/
+-rw-r--r--   0 runner    (1001) docker     (123)     4572 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/include/FormatHandling/BaseFormatHandler.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8554 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/include/FormatHandling/FormatManager.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/include/FormatHandling/clustal_state.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/include/FormatHandling/fasta_m10_state.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/include/FormatHandling/fasta_state.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/include/FormatHandling/formats_header.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/include/FormatHandling/htmlreport_state.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/include/FormatHandling/mega_interleaved_state.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/include/FormatHandling/mega_sequential_state.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/include/FormatHandling/nexus_m10_state.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/include/FormatHandling/nexus_state.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/include/FormatHandling/phylip32_m10_state.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/include/FormatHandling/phylip32_state.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/include/FormatHandling/phylip40_m10_state.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/include/FormatHandling/phylip40_state.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/include/FormatHandling/phylip_paml_m10_state.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/include/FormatHandling/phylip_paml_state.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/include/FormatHandling/pir_state.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4773 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/include/InternalBenchmarker.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:59:43.047949 pytrimal-0.7.0/vendor/trimal/include/RawText/
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/include/RawText/examples.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11662 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/include/RawText/legacyMenu.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    13285 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/include/RawText/menu.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:59:43.047949 pytrimal-0.7.0/vendor/trimal/include/Statistics/
+-rw-r--r--   0 runner    (1001) docker     (123)     7931 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/include/Statistics/Consistency.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/include/Statistics/Gaps.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4871 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/include/Statistics/Manager.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/include/Statistics/Mold.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4935 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/include/Statistics/Similarity.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4262 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/include/Statistics/similarityMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9689 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/include/VCFHandler.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/include/defines.h
+-rw-r--r--   0 runner    (1001) docker     (123)    18611 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/include/reportsystem.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13715 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/include/trimalManager.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15362 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/include/utils.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6542 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/include/values.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:59:43.051949 pytrimal-0.7.0/vendor/trimal/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:59:43.051949 pytrimal-0.7.0/vendor/trimal/source/Alignment/
+-rw-r--r--   0 runner    (1001) docker     (123)   100282 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/source/Alignment/Alignment.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8035 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/source/Alignment/sequencesMatrix.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    66998 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/source/Cleaner.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:59:43.055949 pytrimal-0.7.0/vendor/trimal/source/FormatHandling/
+-rw-r--r--   0 runner    (1001) docker     (123)    12834 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/source/FormatHandling/BaseFormatHandler.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10418 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/source/FormatHandling/clustal_state.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/source/FormatHandling/fasta_m10_state.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7827 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/source/FormatHandling/fasta_state.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5265 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/source/FormatHandling/htmlreport_state.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8309 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/source/FormatHandling/mega_interleaved_state.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11393 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/source/FormatHandling/mega_sequential_state.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6813 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/source/FormatHandling/nexus_m10_state.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11783 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/source/FormatHandling/nexus_state.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4753 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/source/FormatHandling/phylip32_m10_state.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11330 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/source/FormatHandling/phylip32_state.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4832 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/source/FormatHandling/phylip40_m10_state.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10907 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/source/FormatHandling/phylip40_state.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3927 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/source/FormatHandling/phylip_paml_m10_state.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/source/FormatHandling/phylip_paml_state.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8406 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/source/FormatHandling/pir_state.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    16449 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/source/FormatHandling/readAlMain.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6977 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/source/InternalBenchmarker.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:59:43.055949 pytrimal-0.7.0/vendor/trimal/source/Statistics/
+-rw-r--r--   0 runner    (1001) docker     (123)    32843 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/source/Statistics/Consistency.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    24994 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/source/Statistics/Gaps.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7798 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/source/Statistics/Manager.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    13643 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/source/Statistics/Mold.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    24884 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/source/Statistics/Similarity.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    16144 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/source/Statistics/similarityMatrix.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    25928 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/source/VCFHandler.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)   126562 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/source/alignment.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    21325 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/source/compareFiles.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    90551 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/source/main.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:59:43.055949 pytrimal-0.7.0/vendor/trimal/source/reportMessages/
+-rw-r--r--   0 runner    (1001) docker     (123)    17145 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/source/reportMessages/errorMessages.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/source/reportMessages/infoMessages.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/source/reportMessages/warningMessages.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8144 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/source/reportsystem.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    71034 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/source/rwAlignment.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/source/trimAlMain.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    84059 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/source/trimalManager.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/source/typeHelper.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    30036 2023-07-21 18:59:31.000000 pytrimal-0.7.0/vendor/trimal/source/utils.cpp
```

### Comparing `pytrimal-0.6.0/CHANGELOG.md` & `pytrimal-0.7.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,21 @@
 and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).
 
 
 ## [Unreleased]
 [Unreleased]: https://github.com/althonos/pytrimal/compare/v0.6.0...HEAD
 
 
+## [v0.7.0] - 2023-07-21
+[v0.7.0]: https://github.com/althonos/pytrimal/compare/v0.6.0...v0.7.0
+
+### Changed
+- Bumped Cython dependency to `v3.0`.
+
+
 ## [v0.6.0] - 2022-10-17
 [v0.6.0]: https://github.com/althonos/pytrimal/compare/v0.5.5...v0.6.0
 
 ### Fixed
 - Overflow in `calculateSpuriousVector` for certain sequence block sizes.
 - MMX backend never being used unless explicitly required even when being the best supported backend.
 ### Changed
```

### Comparing `pytrimal-0.6.0/CONTRIBUTING.md` & `pytrimal-0.7.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/COPYING` & `pytrimal-0.7.0/COPYING`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/MANIFEST.in` & `pytrimal-0.7.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/PKG-INFO` & `pytrimal-0.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytrimal
-Version: 0.6.0
+Version: 0.7.0
 Summary: Cython bindings and Python interface to trimAl, a tool for automated alignment trimming.
 Home-page: https://github.com/althonos/pytrimal
 Author: Martin Larralde
 Author-email: martin.larralde@embl.de
 License: GPLv3
 Project-URL: Documentation, https://pytrimal.readthedocs.io/en/stable/
 Project-URL: Bug Tracker, https://github.com/althonos/pytrimal/issues
@@ -50,15 +50,15 @@
 [![Python Versions](https://img.shields.io/pypi/pyversions/pytrimal.svg?style=flat-square&maxAge=600&logo=python)](https://pypi.org/project/pytrimal/#files)
 [![Python Implementations](https://img.shields.io/pypi/implementation/pytrimal.svg?style=flat-square&maxAge=600&label=impl)](https://pypi.org/project/pytrimal/#files)
 [![Source](https://img.shields.io/badge/source-GitHub-303030.svg?maxAge=2678400&style=flat-square)](https://github.com/althonos/pytrimal/)
 [![Mirror](https://img.shields.io/badge/mirror-EMBL-009f4d?style=flat-square&maxAge=2678400)](https://git.embl.de/larralde/pytrimal/)
 [![Issues](https://img.shields.io/github/issues/althonos/pytrimal.svg?style=flat-square&maxAge=600)](https://github.com/althonos/pytrimal/issues)
 [![Docs](https://img.shields.io/readthedocs/pytrimal/latest?style=flat-square&maxAge=600)](https://pytrimal.readthedocs.io)
 [![Changelog](https://img.shields.io/badge/keep%20a-changelog-8A0707.svg?maxAge=2678400&style=flat-square)](https://github.com/althonos/pytrimal/blob/main/CHANGELOG.md)
-[![Downloads](https://img.shields.io/badge/dynamic/json?style=flat-square&color=303f9f&maxAge=86400&label=downloads&query=%24.total_downloads&url=https%3A%2F%2Fapi.pepy.tech%2Fapi%2Fprojects%2Fpytrimal)](https://pepy.tech/project/pytrimal)
+[![Downloads](https://img.shields.io/pypi/dm/pytrimal?style=flat-square&color=303f9f&maxAge=86400&label=downloads)](https://pepy.tech/project/pytrimal)
 
 ***⚠️ This package is based on the release candidate of trimAl 2.0, and results
 may not be consistent across versions or with the trimAl 1.4 results.***
 
 ## 🗺️ Overview
 
 PytrimAl is a Python module that provides bindings to [trimAl](http://trimal.cgenomics.org/)
```

### Comparing `pytrimal-0.6.0/README.md` & `pytrimal-0.7.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 [![Python Versions](https://img.shields.io/pypi/pyversions/pytrimal.svg?style=flat-square&maxAge=600&logo=python)](https://pypi.org/project/pytrimal/#files)
 [![Python Implementations](https://img.shields.io/pypi/implementation/pytrimal.svg?style=flat-square&maxAge=600&label=impl)](https://pypi.org/project/pytrimal/#files)
 [![Source](https://img.shields.io/badge/source-GitHub-303030.svg?maxAge=2678400&style=flat-square)](https://github.com/althonos/pytrimal/)
 [![Mirror](https://img.shields.io/badge/mirror-EMBL-009f4d?style=flat-square&maxAge=2678400)](https://git.embl.de/larralde/pytrimal/)
 [![Issues](https://img.shields.io/github/issues/althonos/pytrimal.svg?style=flat-square&maxAge=600)](https://github.com/althonos/pytrimal/issues)
 [![Docs](https://img.shields.io/readthedocs/pytrimal/latest?style=flat-square&maxAge=600)](https://pytrimal.readthedocs.io)
 [![Changelog](https://img.shields.io/badge/keep%20a-changelog-8A0707.svg?maxAge=2678400&style=flat-square)](https://github.com/althonos/pytrimal/blob/main/CHANGELOG.md)
-[![Downloads](https://img.shields.io/badge/dynamic/json?style=flat-square&color=303f9f&maxAge=86400&label=downloads&query=%24.total_downloads&url=https%3A%2F%2Fapi.pepy.tech%2Fapi%2Fprojects%2Fpytrimal)](https://pepy.tech/project/pytrimal)
+[![Downloads](https://img.shields.io/pypi/dm/pytrimal?style=flat-square&color=303f9f&maxAge=86400&label=downloads)](https://pepy.tech/project/pytrimal)
 
 ***⚠️ This package is based on the release candidate of trimAl 2.0, and results
 may not be consistent across versions or with the trimAl 1.4 results.***
 
 ## 🗺️ Overview
 
 PytrimAl is a Python module that provides bindings to [trimAl](http://trimal.cgenomics.org/)
```

### Comparing `pytrimal-0.6.0/include/cpu_features/aarch64.pxd` & `pytrimal-0.7.0/include/cpu_features/aarch64.pxd`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/include/cpu_features/arm.pxd` & `pytrimal-0.7.0/include/cpu_features/arm.pxd`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/include/cpu_features/x86.pxd` & `pytrimal-0.7.0/include/cpu_features/x86.pxd`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/include/iostream.pxd` & `pytrimal-0.7.0/include/iostream.pxd`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/include/trimal/alignment.pxd` & `pytrimal-0.7.0/include/trimal/alignment.pxd`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/include/trimal/cleaner.pxd` & `pytrimal-0.7.0/include/trimal/cleaner.pxd`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/include/trimal/format_handling.pxd` & `pytrimal-0.7.0/include/trimal/format_handling.pxd`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/include/trimal/manager.pxd` & `pytrimal-0.7.0/include/trimal/manager.pxd`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/include/trimal/report_system.pxd` & `pytrimal-0.7.0/include/trimal/report_system.pxd`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/include/trimal/statistics.pxd` & `pytrimal-0.7.0/include/trimal/statistics.pxd`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/patches/clustal_state.cpp.patch` & `pytrimal-0.7.0/patches/clustal_state.cpp.patch`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/patches/fasta_state.cpp.patch` & `pytrimal-0.7.0/patches/fasta_state.cpp.patch`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/patches/nexus_state.cpp.patch` & `pytrimal-0.7.0/patches/nexus_state.cpp.patch`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/patches/phylip32_state.cpp.patch` & `pytrimal-0.7.0/patches/phylip32_state.cpp.patch`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/patches/phylip40_state.cpp.patch` & `pytrimal-0.7.0/patches/phylip40_state.cpp.patch`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/patches/pir_state.cpp.patch` & `pytrimal-0.7.0/patches/pir_state.cpp.patch`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/pytrimal/__init__.py` & `pytrimal-0.7.0/pytrimal/__init__.py`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/pytrimal/_trimal.pxd` & `pytrimal-0.7.0/pytrimal/_trimal.pxd`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/pytrimal/_trimal.pyi` & `pytrimal-0.7.0/pytrimal/_trimal.pyi`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/pytrimal/_trimal.pyx` & `pytrimal-0.7.0/pytrimal/_trimal.pyx`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,70 @@
 # distutils: language = c++
 # cython: language_level=3, linetrace=True, embedsignature=False, binding=False
 """Bindings to trimAl, a tool for automated alignment trimming.
 
+Example:
+    Create a multiple sequence alignment using the `~pytrimal.Alignment`
+    class constructor::
+
+        >>> import pytrimal
+        >>> msa = pytrimal.Alignment(
+        ...     names=[b"Sp8", b"Sp10", b"Sp26", b"Sp6", b"Sp17", b"Sp33"],
+        ...     sequences=[
+        ...         "-----GLGKVIV-YGIVLGTKSDQFSNWVVWLFPWNGLQIHMMGII",
+        ...         "-------DPAVL-FVIMLGTIT-KFS--SEWFFAWLGLEINMMVII",
+        ...         "AAAAAAAAALLTYLGLFLGTDYENFA--AAAANAWLGLEINMMAQI",
+        ...         "-----ASGAILT-LGIYLFTLCAVIS--VSWYLAWLGLEINMMAII",
+        ...         "--FAYTAPDLL-LIGFLLKTVA-TFG--DTWFQLWQGLDLNKMPVF",
+        ...         "-------PTILNIAGLHMETDI-NFS--LAWFQAWGGLEINKQAIL",
+        ...     ],
+        ... )
+
+    Then use a trimmer to trim the alignment, for instance with the
+    *automated1* algorithm:
+
+        >>> trimmer = AutomaticTrimmer("automated1")
+        >>> trimmed = trimmer.trim(msa)
+
+    The trimmed alignment supports the same methods as the original
+    alignment object:
+
+        >>> for sequence in trimmed.sequences:
+        ...     print(sequence)
+        VWLFPWNGLQIHMMGII
+        EWFFAWLGLEINMMVII
+        AAANAWLGLEINMMAQI
+        SWYLAWLGLEINMMAII
+        TWFQLWQGLDLNKMPVF
+        AWFQAWGGLEINKQAIL
+
 References:
     - Capella-Gutiérrez, Salvador, José M. Silla-Martínez, and Toni Gabaldón.
       *TrimAl: A Tool for Automated Alignment Trimming in Large-Scale
       Phylogenetic Analyses*. Bioinformatics 25, no. 15 (2009): 1972–73.
       :doi:`10.1093/bioinformatics/btp348`.
 
 """
 
 # --- C imports --------------------------------------------------------------
 
 cimport cython
-from _unicode cimport (
-    PyUnicode_New,
-    PyUnicode_READY,
-    PyUnicode_KIND,
-    PyUnicode_DATA,
-    PyUnicode_WRITE,
-)
 from cpython cimport Py_buffer
 from cpython.buffer cimport PyBUF_FORMAT, PyBUF_READ, PyBuffer_FillInfo
 from cpython.bytes cimport PyBytes_FromStringAndSize, PyBytes_AsString
 from cpython.list cimport PyList_New, PyList_SET_ITEM
 from cpython.mem cimport PyMem_Free, PyMem_Malloc
 from cpython.memoryview cimport PyMemoryView_FromMemory, PyMemoryView_GET_BUFFER
 from cpython.ref cimport Py_INCREF
+from cpython.unicode cimport (
+    PyUnicode_New,
+    PyUnicode_KIND,
+    PyUnicode_DATA,
+    PyUnicode_WRITE,
+)
 
 from libc.errno cimport errno
 from libc.math cimport NAN, isnan, sqrt
 from libc.stdio cimport printf
 from libc.string cimport memset
 from libcpp cimport bool
 from libcpp.string cimport string
@@ -41,21 +75,21 @@
 cimport trimal.format_handling
 cimport trimal.manager
 cimport trimal.report_system
 cimport trimal.similarity_matrix
 
 from pytrimal.fileobj cimport pyreadbuf, pyreadintobuf, pywritebuf
 from pytrimal.impl.generic cimport GenericSimilarity, GenericGaps, GenericCleaner
-IF SSE2_BUILD_SUPPORT:
+if SSE2_BUILD_SUPPORT:
     from pytrimal.impl.sse cimport SSESimilarity, SSEGaps, SSECleaner
-IF MMX_BUILD_SUPPORT:
+if MMX_BUILD_SUPPORT:
     from pytrimal.impl.mmx cimport MMXSimilarity, MMXGaps, MMXCleaner
-IF NEON_BUILD_SUPPORT:
+if NEON_BUILD_SUPPORT:
     from pytrimal.impl.neon cimport NEONSimilarity, NEONGaps, NEONCleaner
-IF AVX2_BUILD_SUPPORT:
+if AVX2_BUILD_SUPPORT:
     from pytrimal.impl.avx cimport AVXSimilarity, AVXGaps, AVXCleaner
 
 
 # --- Python imports ---------------------------------------------------------
 
 import os
 import threading
@@ -63,21 +97,22 @@
 import archspec.cpu
 
 include "_version.py"
 
 
 # --- Patch for PyPy 3.9 -----------------------------------------------------
 
-IF not HAS_PYINTERPRETERSTATE_GETID:
-    cdef extern from *:
-        """
-        int64_t PyInterpreterState_GetID(PyInterpreterState *interp) {
-            return 0;
-        }
-        """
+cdef extern from *:
+    """
+    #ifndef HAS_PYINTERPRETERSTATE_GETID
+    int64_t PyInterpreterState_GetID(PyInterpreterState *interp) {
+        return 0;
+    }
+    #endif
+    """
 
 
 # --- Constants --------------------------------------------------------------
 
 _TARGET_CPU           = TARGET_CPU
 _HOST_CPU             = archspec.cpu.host()
 _SSE2_BUILD_SUPPORT   = False
@@ -85,25 +120,25 @@
 _MMX_BUILD_SUPPORT    = False
 _MMX_RUNTIME_SUPPORT  = False
 _AVX2_BUILD_SUPPORT   = False
 _AVX2_RUNTIME_SUPPORT = False
 _NEON_BUILD_SUPPORT   = False
 _NEON_RUNTIME_SUPPORT = False
 
-IF TARGET_CPU == "x86" and TARGET_SYSTEM in ("freebsd", "linux_or_android", "macos", "windows"):
+if TARGET_CPU == "x86" and TARGET_SYSTEM in ("freebsd", "linux_or_android", "macos", "windows"):
     _MMX_BUILD_SUPPORT    = MMX_BUILD_SUPPORT
     _SSE2_BUILD_SUPPORT   = SSE2_BUILD_SUPPORT
     _AVX2_BUILD_SUPPORT   = AVX2_BUILD_SUPPORT
     _MMX_RUNTIME_SUPPORT  = "mmx" in _HOST_CPU.features
     _SSE2_RUNTIME_SUPPORT = "sse2" in _HOST_CPU.features
     _AVX2_RUNTIME_SUPPORT = "avx2" in _HOST_CPU.features
-ELIF TARGET_CPU == "arm" and TARGET_SYSTEM == "linux_or_android":
+elif TARGET_CPU == "arm" and TARGET_SYSTEM == "linux_or_android":
     _NEON_BUILD_SUPPORT   = NEON_BUILD_SUPPORT
     _NEON_RUNTIME_SUPPORT = "neon" in _HOST_CPU.features
-ELIF TARGET_CPU == "aarch64":
+elif TARGET_CPU == "aarch64":
     _NEON_BUILD_SUPPORT   = NEON_BUILD_SUPPORT
     _NEON_RUNTIME_SUPPORT = NEON_BUILD_SUPPORT  # always runtime support on Aarch64
 
 if _AVX2_RUNTIME_SUPPORT:
     _BEST_BACKEND = simd_backend.AVX2
 elif _SSE2_RUNTIME_SUPPORT:
     _BEST_BACKEND = simd_backend.SSE2
@@ -262,39 +297,40 @@
 
     cdef str _sequence(self, int index):
         """_sequence(self, index)\n--
 
         Return a single sequence in the alignment, creating a new string.
 
         """
-        cdef int index_ = index
+        cdef int    kind
+        cdef object seq
+        cdef char*  data
+        cdef size_t x      = 0
+        cdef int    index_ = index
+
         if index_ < 0:
             index_ += self._length
         if index_ < 0 or index_ >= self._length:
             raise IndexError(index)
         if self._index_mapping is not NULL:
             index_ = self._index_mapping[index_]
 
         assert index_ < self._ali.originalNumberOfSequences
-        IF SYS_VERSION_INFO_MAJOR <= 3 and SYS_VERSION_INFO_MAJOR <= 7 and SYS_IMPLEMENTATION_NAME == "pypy":
-            cdef bytes    seq  = PyBytes_FromStringAndSize(NULL, self._ali.numberOfResidues)
-            cdef char*    data = PyBytes_AsString(seq)
-            cdef size_t   x    = 0
+        if SYS_VERSION_INFO_MAJOR <= 3 and SYS_VERSION_INFO_MAJOR <= 7 and SYS_IMPLEMENTATION_NAME == "pypy":
+            seq  = PyBytes_FromStringAndSize(NULL, self._ali.numberOfResidues)
+            data = PyBytes_AsString(seq)
             for i in range(self._ali.originalNumberOfResidues):
                 if self._ali.saveResidues is NULL or self._ali.saveResidues[i] != -1:
                     data[x] = self._ali.sequences[index_][i]
                     x += 1
             return seq.decode('ascii')
-        ELSE:
-            cdef str      seq  = PyUnicode_New(self._ali.numberOfResidues, 0x7f)
-            IF SYS_VERSION_INFO_MAJOR <= 3 and SYS_VERSION_INFO_MINOR < 12:
-                PyUnicode_READY(seq)
-            cdef void*    data = PyUnicode_DATA(seq)
-            cdef int      kind = PyUnicode_KIND(seq)
-            cdef size_t   x    = 0
+        else:
+            seq  = PyUnicode_New(self._ali.numberOfResidues, 0x7f)
+            data = <char*> PyUnicode_DATA(seq)
+            kind = PyUnicode_KIND(seq)
             for i in range(self._ali.originalNumberOfResidues):
                 if self._ali.saveResidues is NULL or self._ali.saveResidues[i] != -1:
                     PyUnicode_WRITE(kind, data, x, self._ali.sequences[index_][i])
                     x += 1
             return seq
 
 
@@ -372,41 +408,41 @@
 
     cdef str _column(self, int index):
         """_column(self, index)\n--
 
         Return a single residue column in the alignment, creating a new string.
 
         """
-        cdef int index_ = index
-        cdef int length = self._ali.numberOfResidues
+        cdef object col
+        cdef int    kind
+        cdef char*  data
+        cdef size_t x      = 0
+        cdef int    index_ = index
+        cdef int    length = self._ali.numberOfResidues
 
         if index_ < 0:
             index_ += length
         if index_ < 0 or index_ >= self._length:
             raise IndexError(index)
         if self._index_mapping is not NULL:
             index_ = self._index_mapping[index_]
 
         assert index_ < self._ali.originalNumberOfResidues
-        IF SYS_VERSION_INFO_MAJOR <= 3 and SYS_VERSION_INFO_MAJOR <= 7 and SYS_IMPLEMENTATION_NAME == "pypy":
-            cdef bytes    col  = PyBytes_FromStringAndSize(NULL, self._ali.numberOfSequences)
-            cdef char*    data = PyBytes_AsString(col)
-            cdef size_t   x    = 0
+        if SYS_VERSION_INFO_MAJOR <= 3 and SYS_VERSION_INFO_MAJOR <= 7 and SYS_IMPLEMENTATION_NAME == "pypy":
+            col  = PyBytes_FromStringAndSize(NULL, self._ali.numberOfSequences)
+            data = PyBytes_AsString(col)
             for i in range(self._ali.originalNumberOfSequences):
                 if self._ali.saveSequences is NULL or self._ali.saveSequences[i] != -1:
                     data[x] = self._ali.sequences[i][index_]
                     x += 1
             return col.decode('ascii')
-        ELSE:
-            cdef str      col = PyUnicode_New(self._ali.numberOfSequences, 0x7f)
-            IF SYS_VERSION_INFO_MAJOR <= 3 and SYS_VERSION_INFO_MINOR < 12:
-                PyUnicode_READY(col)
-            cdef void*    data = PyUnicode_DATA(col)
-            cdef int      kind = PyUnicode_KIND(col)
-            cdef size_t   x    = 0
+        else:
+            col = PyUnicode_New(self._ali.numberOfSequences, 0x7f)
+            data = <char*> PyUnicode_DATA(col)
+            kind = PyUnicode_KIND(col)
             for i in range(self._ali.originalNumberOfSequences):
                 if self._ali.saveSequences is NULL or self._ali.saveSequences[i] != -1:
                     PyUnicode_WRITE(kind, data, x, self._ali.sequences[i][index_])
                     x += 1
             return col
 
 
@@ -550,17 +586,17 @@
         cdef char           cbuffer[DEFAULT_BUFFER_SIZE]
         cdef filebuf        fbuffer
         cdef pyreadbuf*     rbuffer   = NULL
         cdef pyreadintobuf* r2buffer  = NULL
         cdef istream*       stream    = NULL
         cdef Alignment      alignment = Alignment.__new__(Alignment)
 
-        IF SYS_VERSION_INFO_MAJOR == 3 and SYS_VERSION_INFO_MINOR < 6:
+        if SYS_VERSION_INFO_MAJOR == 3 and SYS_VERSION_INFO_MINOR < 6:
             TYPES = (str, bytes)
-        ELSE:
+        else:
             TYPES = (str, bytes, os.PathLike)
         if isinstance(file, TYPES):
             # check that file exists and is not a directory
             if not os.path.exists(file):
                 raise FileNotFoundError(file)
             elif os.path.isdir(file):
                 raise IsADirectoryError(file)
@@ -677,17 +713,17 @@
         cdef pywritebuf*                               pbuffer    = NULL
         cdef ostream*                                  stream     = NULL
 
         handler = manager.getFormatFromToken(format.lower().encode('ascii'))
         if handler is NULL:
             raise ValueError(f"Could not recognize alignment format: {format!r}")
 
-        IF SYS_VERSION_INFO_MAJOR == 3 and SYS_VERSION_INFO_MINOR < 6:
+        if SYS_VERSION_INFO_MAJOR == 3 and SYS_VERSION_INFO_MINOR < 6:
             TYPES = (str, bytes)
-        ELSE:
+        else:
             TYPES = (str, bytes, os.PathLike)
         if isinstance(file, TYPES):
             path_ = os.fsencode(file)
             if fbuffer.open(<const char*> path_, WRITEMODE) is NULL:
                 raise OSError(errno, f"Failed to open {file!r}")
             stream = new ostream(&fbuffer)
         else:
@@ -1145,69 +1181,69 @@
                 to accelerate computation of pairwise similarity statistics.
                 If `None` given, use the original code from trimAl.
 
         .. versionadded:: 0.2.0
            The ``backend`` keyword argument.
 
         """
-        IF TARGET_CPU == "x86":
+        if TARGET_CPU == "x86":
             if backend =="detect":
                 self._backend = simd_backend.GENERIC
-                IF MMX_BUILD_SUPPORT:
-                    if _MMX_RUNTIME_SUPPORT:
-                        self._backend = simd_backend.MMX
-                IF SSE2_BUILD_SUPPORT:
-                    if _SSE2_RUNTIME_SUPPORT:
-                        self._backend = simd_backend.SSE2
-                IF AVX2_BUILD_SUPPORT:
-                    if _AVX2_RUNTIME_SUPPORT:
-                        self._backend = simd_backend.AVX2
+                if MMX_BUILD_SUPPORT and _MMX_RUNTIME_SUPPORT:
+                    self._backend = simd_backend.MMX
+                if SSE2_BUILD_SUPPORT and _SSE2_RUNTIME_SUPPORT:
+                    self._backend = simd_backend.SSE2
+                if AVX2_BUILD_SUPPORT and _AVX2_RUNTIME_SUPPORT:
+                    self._backend = simd_backend.AVX2
             elif backend == "mmx":
-                IF not MMX_BUILD_SUPPORT:
+                if not MMX_BUILD_SUPPORT:
                     raise RuntimeError("Extension was compiled without MMX support")
-                if not _MMX_RUNTIME_SUPPORT:
+                elif not _MMX_RUNTIME_SUPPORT:
                     raise RuntimeError("Cannot run MMX instructions on this machine")
-                self._backend = simd_backend.MMX
+                else:
+                    self._backend = simd_backend.MMX
             elif backend == "avx":
-                IF not AVX2_BUILD_SUPPORT:
+                if not AVX2_BUILD_SUPPORT:
                     raise RuntimeError("Extension was compiled without AVX2 support")
-                if not _AVX2_RUNTIME_SUPPORT:
+                elif not _AVX2_RUNTIME_SUPPORT:
                     raise RuntimeError("Cannot run AVX2 instructions on this machine")
-                self._backend = simd_backend.AVX2
+                else:
+                    self._backend = simd_backend.AVX2
             elif backend == "sse":
-                IF not SSE2_BUILD_SUPPORT:
+                if not SSE2_BUILD_SUPPORT:
                     raise RuntimeError("Extension was compiled without SSE2 support")
-                if not _SSE2_RUNTIME_SUPPORT:
+                elif not _SSE2_RUNTIME_SUPPORT:
                     raise RuntimeError("Cannot run SSE2 instructions on this machine")
-                self._backend = simd_backend.SSE2
+                else:
+                    self._backend = simd_backend.SSE2
             elif backend == "generic":
                 self._backend = simd_backend.GENERIC
             elif backend is None:
                 self._backend = simd_backend.NONE
             else:
                 raise ValueError(f"Unsupported backend on this architecture: {backend}")
-        ELIF TARGET_CPU == "arm" or TARGET_CPU == "aarch64":
+        elif TARGET_CPU == "arm" or TARGET_CPU == "aarch64":
             if backend == "detect":
                 self._backend = simd_backend.GENERIC
-                IF NEON_BUILD_SUPPORT:
-                    if _NEON_RUNTIME_SUPPORT:
-                        self._backend = simd_backend.NEON
+                if NEON_BUILD_SUPPORT and _NEON_RUNTIME_SUPPORT:
+                    self._backend = simd_backend.NEON
             elif backend == "neon":
-                IF not NEON_BUILD_SUPPORT:
+                if not NEON_BUILD_SUPPORT:
                     raise RuntimeError("Extension was compiled without NEON support")
-                if not _NEON_RUNTIME_SUPPORT:
+                elif not _NEON_RUNTIME_SUPPORT:
                     raise RuntimeError("Cannot run NEON instructions on this machine")
-                self._backend = simd_backend.NEON
+                else:
+                    self._backend = simd_backend.NEON
             elif backend == "generic":
                 self._backend = simd_backend.GENERIC
             elif backend is None:
                 self._backend = simd_backend.NONE
             else:
                 raise ValueError(f"Unsupported backend on this architecture: {backend}")
-        ELSE:
+        else:
             if backend == "detect" or backend == "generic":
                 self._backend = simd_backend.GENERIC
             elif backend is None:
                 self._backend = simd_backend.NONE
             else:
                 raise ValueError(f"Unsupported backend on this architecture: {backend}")
 
@@ -1258,42 +1294,42 @@
             del manager.origAlig.Statistics.similarity
             manager.origAlig.Statistics.similarity = new GenericSimilarity(manager.origAlig)
             del manager.origAlig.Cleaning
             manager.origAlig.Cleaning = new GenericCleaner(manager.origAlig)
             del manager.origAlig.Statistics.gaps
             manager.origAlig.Statistics.gaps = new GenericGaps(manager.origAlig)
             manager.origAlig.Statistics.gaps.CalculateVectors()
-        IF MMX_BUILD_SUPPORT:
+        if MMX_BUILD_SUPPORT:
             if self._backend == simd_backend.MMX:
                 del manager.origAlig.Statistics.similarity
                 manager.origAlig.Statistics.similarity = new MMXSimilarity(manager.origAlig)
                 del manager.origAlig.Cleaning
                 manager.origAlig.Cleaning = new MMXCleaner(manager.origAlig)
                 del manager.origAlig.Statistics.gaps
                 manager.origAlig.Statistics.gaps = new MMXGaps(manager.origAlig)
                 manager.origAlig.Statistics.gaps.CalculateVectors()
-        IF AVX2_BUILD_SUPPORT:
+        if AVX2_BUILD_SUPPORT:
             if self._backend == simd_backend.AVX2:
                 del manager.origAlig.Statistics.similarity
                 manager.origAlig.Statistics.similarity = new AVXSimilarity(manager.origAlig)
                 del manager.origAlig.Cleaning
                 manager.origAlig.Cleaning = new AVXCleaner(manager.origAlig)
                 del manager.origAlig.Statistics.gaps
                 manager.origAlig.Statistics.gaps = new AVXGaps(manager.origAlig)
                 manager.origAlig.Statistics.gaps.CalculateVectors()
-        IF SSE2_BUILD_SUPPORT:
+        if SSE2_BUILD_SUPPORT:
             if self._backend == simd_backend.SSE2:
                 del manager.origAlig.Statistics.similarity
                 manager.origAlig.Statistics.similarity = new SSESimilarity(manager.origAlig)
                 del manager.origAlig.Cleaning
                 manager.origAlig.Cleaning = new SSECleaner(manager.origAlig)
                 del manager.origAlig.Statistics.gaps
                 manager.origAlig.Statistics.gaps = new SSEGaps(manager.origAlig)
                 manager.origAlig.Statistics.gaps.CalculateVectors()
-        IF NEON_BUILD_SUPPORT:
+        if NEON_BUILD_SUPPORT:
             if self._backend == simd_backend.NEON:
                 del manager.origAlig.Statistics.similarity
                 manager.origAlig.Statistics.similarity = new NEONSimilarity(manager.origAlig)
                 del manager.origAlig.Cleaning
                 manager.origAlig.Cleaning = new NEONCleaner(manager.origAlig)
                 del manager.origAlig.Statistics.gaps
                 manager.origAlig.Statistics.gaps = new NEONGaps(manager.origAlig)
@@ -1971,15 +2007,15 @@
                           * (self._smx.simMat[k][j] - self._smx.simMat[k][i])
                         )
                     self._smx.distMat[i][j] = self._smx.distMat[j][i] = sqrt(sum)
 
     def __len__(self):
         return self._smx.numPositions
 
-    IF SYS_IMPLEMENTATION_NAME == "cpython":
+    if SYS_IMPLEMENTATION_NAME == "cpython":
 
         def __getbuffer__(self, Py_buffer* buffer, int flags):
             # setup indexing information
             self._shape[0] = self._smx.numPositions
             self._shape[1] = self._smx.numPositions
             self._suboffsets[0] = 0
             self._suboffsets[1] = -1
```

### Comparing `pytrimal-0.6.0/pytrimal/fileobj/pyreadbuf.cpp` & `pytrimal-0.7.0/pytrimal/fileobj/pyreadbuf.cpp`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/pytrimal/fileobj/pyreadbuf.h` & `pytrimal-0.7.0/pytrimal/fileobj/pyreadbuf.h`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/pytrimal/fileobj/pyreadintobuf.cpp` & `pytrimal-0.7.0/pytrimal/fileobj/pyreadintobuf.cpp`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/pytrimal/fileobj/pyreadintobuf.h` & `pytrimal-0.7.0/pytrimal/fileobj/pyreadintobuf.h`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/pytrimal/fileobj/pywritebuf.cpp` & `pytrimal-0.7.0/pytrimal/fileobj/pywritebuf.cpp`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/pytrimal/impl/avx.cpp` & `pytrimal-0.7.0/pytrimal/impl/avx.cpp`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/pytrimal/impl/avx.h` & `pytrimal-0.7.0/pytrimal/impl/avx.h`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/pytrimal/impl/generic.cpp` & `pytrimal-0.7.0/pytrimal/impl/generic.cpp`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/pytrimal/impl/generic.h` & `pytrimal-0.7.0/pytrimal/impl/generic.h`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/pytrimal/impl/generic.pxd` & `pytrimal-0.7.0/pytrimal/impl/generic.pxd`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/pytrimal/impl/mmx.cpp` & `pytrimal-0.7.0/pytrimal/impl/mmx.cpp`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/pytrimal/impl/mmx.h` & `pytrimal-0.7.0/pytrimal/impl/mmx.h`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/pytrimal/impl/neon.cpp` & `pytrimal-0.7.0/pytrimal/impl/neon.cpp`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/pytrimal/impl/neon.h` & `pytrimal-0.7.0/pytrimal/impl/neon.h`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/pytrimal/impl/sse.cpp` & `pytrimal-0.7.0/pytrimal/impl/sse.cpp`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/pytrimal/impl/sse.h` & `pytrimal-0.7.0/pytrimal/impl/sse.h`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/pytrimal/impl/template.h` & `pytrimal-0.7.0/pytrimal/impl/template.h`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/pytrimal/patch/reportsystem.cpp` & `pytrimal-0.7.0/pytrimal/patch/reportsystem.cpp`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/pytrimal/tests/__init__.py` & `pytrimal-0.7.0/pytrimal/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/pytrimal/tests/_base.py` & `pytrimal-0.7.0/pytrimal/tests/_base.py`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/pytrimal/tests/data/ENOG411BWBU.automated1.fasta` & `pytrimal-0.7.0/pytrimal/tests/data/ENOG411BWBU.automated1.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/pytrimal/tests/data/ENOG411BWBU.clusters10.fasta` & `pytrimal-0.7.0/pytrimal/tests/data/ENOG411BWBU.clusters10.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/pytrimal/tests/data/ENOG411BWBU.clusters5.fasta` & `pytrimal-0.7.0/pytrimal/tests/data/ENOG411BWBU.clusters5.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/pytrimal/tests/data/ENOG411BWBU.cons40.gt40.fasta` & `pytrimal-0.7.0/pytrimal/tests/data/ENOG411BWBU.cons40.gt40.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/pytrimal/tests/data/ENOG411BWBU.cons60.gt90.fasta` & `pytrimal-0.7.0/pytrimal/tests/data/ENOG411BWBU.cons60.gt90.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/pytrimal/tests/data/ENOG411BWBU.fasta` & `pytrimal-0.7.0/pytrimal/tests/data/ENOG411BWBU.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/pytrimal/tests/data/ENOG411BWBU.gappyout.fasta` & `pytrimal-0.7.0/pytrimal/tests/data/ENOG411BWBU.gappyout.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/pytrimal/tests/data/ENOG411BWBU.id50.fasta` & `pytrimal-0.7.0/pytrimal/tests/data/ENOG411BWBU.id50.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/pytrimal/tests/data/ENOG411BWBU.id70.fasta` & `pytrimal-0.7.0/pytrimal/tests/data/ENOG411BWBU.id70.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/pytrimal/tests/data/ENOG411BWBU.maxidentity75.fasta` & `pytrimal-0.7.0/pytrimal/tests/data/ENOG411BWBU.maxidentity75.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/pytrimal/tests/data/ENOG411BWBU.noallgaps.fasta` & `pytrimal-0.7.0/pytrimal/tests/data/ENOG411BWBU.noallgaps.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/pytrimal/tests/data/ENOG411BWBU.noduplicateseqs.fasta` & `pytrimal-0.7.0/pytrimal/tests/data/ENOG411BWBU.noduplicateseqs.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/pytrimal/tests/data/ENOG411BWBU.seq40.res60.fasta` & `pytrimal-0.7.0/pytrimal/tests/data/ENOG411BWBU.seq40.res60.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/pytrimal/tests/data/ENOG411BWBU.seq80.res80.fasta` & `pytrimal-0.7.0/pytrimal/tests/data/ENOG411BWBU.seq80.res80.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/pytrimal/tests/data/ENOG411BWBU.strict.fasta` & `pytrimal-0.7.0/pytrimal/tests/data/ENOG411BWBU.strict.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/pytrimal/tests/data/ENOG411BWBU.strictplus.fasta` & `pytrimal-0.7.0/pytrimal/tests/data/ENOG411BWBU.strictplus.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/pytrimal/tests/data/PF12574.full.afa` & `pytrimal-0.7.0/pytrimal/tests/data/PF12574.full.afa`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/pytrimal/tests/data/halorhodopsin.afa` & `pytrimal-0.7.0/pytrimal/tests/data/halorhodopsin.afa`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/pytrimal/tests/data/pam70.json` & `pytrimal-0.7.0/pytrimal/tests/data/pam70.json`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/pytrimal/tests/test_alignment.py` & `pytrimal-0.7.0/pytrimal/tests/test_alignment.py`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/pytrimal/tests/test_automatic_trimmer.py` & `pytrimal-0.7.0/pytrimal/tests/test_automatic_trimmer.py`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/pytrimal/tests/test_doctest.py` & `pytrimal-0.7.0/pytrimal/tests/test_doctest.py`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/pytrimal/tests/test_manual_trimmer.py` & `pytrimal-0.7.0/pytrimal/tests/test_manual_trimmer.py`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/pytrimal/tests/test_overlap_trimmer.py` & `pytrimal-0.7.0/pytrimal/tests/test_overlap_trimmer.py`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/pytrimal/tests/test_representative_trimmer.py` & `pytrimal-0.7.0/pytrimal/tests/test_representative_trimmer.py`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/pytrimal/tests/test_similarity_matrix.py` & `pytrimal-0.7.0/pytrimal/tests/test_similarity_matrix.py`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/pytrimal.egg-info/PKG-INFO` & `pytrimal-0.7.0/pytrimal.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytrimal
-Version: 0.6.0
+Version: 0.7.0
 Summary: Cython bindings and Python interface to trimAl, a tool for automated alignment trimming.
 Home-page: https://github.com/althonos/pytrimal
 Author: Martin Larralde
 Author-email: martin.larralde@embl.de
 License: GPLv3
 Project-URL: Documentation, https://pytrimal.readthedocs.io/en/stable/
 Project-URL: Bug Tracker, https://github.com/althonos/pytrimal/issues
@@ -50,15 +50,15 @@
 [![Python Versions](https://img.shields.io/pypi/pyversions/pytrimal.svg?style=flat-square&maxAge=600&logo=python)](https://pypi.org/project/pytrimal/#files)
 [![Python Implementations](https://img.shields.io/pypi/implementation/pytrimal.svg?style=flat-square&maxAge=600&label=impl)](https://pypi.org/project/pytrimal/#files)
 [![Source](https://img.shields.io/badge/source-GitHub-303030.svg?maxAge=2678400&style=flat-square)](https://github.com/althonos/pytrimal/)
 [![Mirror](https://img.shields.io/badge/mirror-EMBL-009f4d?style=flat-square&maxAge=2678400)](https://git.embl.de/larralde/pytrimal/)
 [![Issues](https://img.shields.io/github/issues/althonos/pytrimal.svg?style=flat-square&maxAge=600)](https://github.com/althonos/pytrimal/issues)
 [![Docs](https://img.shields.io/readthedocs/pytrimal/latest?style=flat-square&maxAge=600)](https://pytrimal.readthedocs.io)
 [![Changelog](https://img.shields.io/badge/keep%20a-changelog-8A0707.svg?maxAge=2678400&style=flat-square)](https://github.com/althonos/pytrimal/blob/main/CHANGELOG.md)
-[![Downloads](https://img.shields.io/badge/dynamic/json?style=flat-square&color=303f9f&maxAge=86400&label=downloads&query=%24.total_downloads&url=https%3A%2F%2Fapi.pepy.tech%2Fapi%2Fprojects%2Fpytrimal)](https://pepy.tech/project/pytrimal)
+[![Downloads](https://img.shields.io/pypi/dm/pytrimal?style=flat-square&color=303f9f&maxAge=86400&label=downloads)](https://pepy.tech/project/pytrimal)
 
 ***⚠️ This package is based on the release candidate of trimAl 2.0, and results
 may not be consistent across versions or with the trimAl 1.4 results.***
 
 ## 🗺️ Overview
 
 PytrimAl is a Python module that provides bindings to [trimAl](http://trimal.cgenomics.org/)
```

### Comparing `pytrimal-0.6.0/pytrimal.egg-info/SOURCES.txt` & `pytrimal-0.7.0/pytrimal.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 CONTRIBUTING.md
 COPYING
 MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
 setup.py
-include/_unicode.pxd
 include/iostream.pxd
 include/cpu_features/__init__.pxd
 include/cpu_features/aarch64.pxd
 include/cpu_features/arm.pxd
 include/cpu_features/x86.pxd
 include/trimal/__init__.pxd
 include/trimal/alignment.pxd
```

### Comparing `pytrimal-0.6.0/setup.cfg` & `pytrimal-0.7.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 [options]
 zip_safe = false
 packages = pytrimal, pytrimal.tests, pytrimal.tests.data
 include_package_data = false
 python_requires = >=3.5
 setup_requires = 
 	setuptools >=46.4
-	cython ~=0.29.16
+	cython ~=3.0
 install_requires = 
 	archspec ~=0.1
 tests_require = 
 	importlib-resources ; python_version < '3.9'
 
 [options.package_data]
 pytrimal = py.typed, *.pyi
```

### Comparing `pytrimal-0.6.0/setup.py` & `pytrimal-0.7.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -407,14 +407,18 @@
         elif self.compiler.compiler_type == "msvc":
             ext.extra_compile_args.append("/std:c11")
 
         # add Windows flags
         if self.compiler.compiler_type == "msvc":
             ext.define_macros.append(("WIN32", 1))
 
+        # check `PyInterpreterState_GetID` is present
+        if self._check_getid():
+            ext.define_macros.append(("HAS_PYINTERPRETERSTATE_GETID", 1))
+
         # update link and include directories
         for name in ext.libraries:
             lib = self._clib_cmd.get_library(name)
             libfile = self.compiler.library_filename(
                 lib.name, output_dir=self._clib_cmd.build_clib
             )
             ext.depends.append(libfile)
@@ -442,15 +446,14 @@
         cython_args = {
             "include_path": ["include"],
             "compiler_directives": {
                 "cdivision": True,
                 "nonecheck": False,
             },
             "compile_time_env": {
-                "HAS_PYINTERPRETERSTATE_GETID": self._check_getid(),
                 "SYS_IMPLEMENTATION_NAME": sys.implementation.name,
                 "SYS_VERSION_INFO_MAJOR": sys.version_info.major,
                 "SYS_VERSION_INFO_MINOR": sys.version_info.minor,
                 "SYS_VERSION_INFO_MICRO": sys.version_info.micro,
                 "DEFAULT_BUFFER_SIZE": io.DEFAULT_BUFFER_SIZE,
                 "TARGET_CPU": TARGET_CPU,
                 "TARGET_SYSTEM": TARGET_SYSTEM,
```

### Comparing `pytrimal-0.6.0/vendor/trimal/AUTHORS` & `pytrimal-0.7.0/vendor/trimal/AUTHORS`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/CHANGELOG` & `pytrimal-0.7.0/vendor/trimal/CHANGELOG`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/CMakeLists.txt` & `pytrimal-0.7.0/vendor/trimal/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/LICENSE` & `pytrimal-0.7.0/vendor/trimal/LICENSE`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/README.md` & `pytrimal-0.7.0/vendor/trimal/README.md`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/dataset/example.005.AA.fasta` & `pytrimal-0.7.0/vendor/trimal/dataset/example.005.AA.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/dataset/example.006.AA.pir` & `pytrimal-0.7.0/vendor/trimal/dataset/example.006.AA.pir`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/dataset/example.007.AA.fasta` & `pytrimal-0.7.0/vendor/trimal/dataset/example.007.AA.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/dataset/example.007.AA.only_seqs` & `pytrimal-0.7.0/vendor/trimal/dataset/example.007.AA.only_seqs`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/dataset/example.009.AA.fasta` & `pytrimal-0.7.0/vendor/trimal/dataset/example.009.AA.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/dataset/example.010.AA.fasta` & `pytrimal-0.7.0/vendor/trimal/dataset/example.010.AA.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/dataset/example.011.AA.YKL197C.clw` & `pytrimal-0.7.0/vendor/trimal/dataset/example.011.AA.YKL197C.clw`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/dataset/example.011.AA.YKL197C.fasta` & `pytrimal-0.7.0/vendor/trimal/dataset/example.011.AA.YKL197C.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/dataset/example.011.AA.YKL197C.phy` & `pytrimal-0.7.0/vendor/trimal/dataset/example.011.AA.YKL197C.phy`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/dataset/example.012.AA.SuperAlignment.phy` & `pytrimal-0.7.0/vendor/trimal/dataset/example.012.AA.SuperAlignment.phy`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/dataset/example.013.AA.SuperAlignment.phy` & `pytrimal-0.7.0/vendor/trimal/dataset/example.013.AA.SuperAlignment.phy`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/dataset/example.014.AA.EggNOG.COG0591.fasta` & `pytrimal-0.7.0/vendor/trimal/dataset/example.014.AA.EggNOG.COG0591.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/dataset/example.015.AA.bctoNOG.ENOG41099F3.fasta` & `pytrimal-0.7.0/vendor/trimal/dataset/example.015.AA.bctoNOG.ENOG41099F3.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/dataset/example.016.AA.bctoNOG.ENOG41099FB.fasta` & `pytrimal-0.7.0/vendor/trimal/dataset/example.016.AA.bctoNOG.ENOG41099FB.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/dataset/example.017.AA.bctoNOG.ENOG41099FJ.fasta` & `pytrimal-0.7.0/vendor/trimal/dataset/example.017.AA.bctoNOG.ENOG41099FJ.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/dataset/example.018.AA.bctoNOG.ENOG41099FV.fasta` & `pytrimal-0.7.0/vendor/trimal/dataset/example.018.AA.bctoNOG.ENOG41099FV.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/dataset/example.019.AA.bctoNOG.ENOG41099HI.fasta` & `pytrimal-0.7.0/vendor/trimal/dataset/example.019.AA.bctoNOG.ENOG41099HI.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/dataset/example.020.AA.bctoNOG.ENOG41099HN.fasta` & `pytrimal-0.7.0/vendor/trimal/dataset/example.020.AA.bctoNOG.ENOG41099HN.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/dataset/example.021.AA.bctoNOG.ENOG41099I5.fasta` & `pytrimal-0.7.0/vendor/trimal/dataset/example.021.AA.bctoNOG.ENOG41099I5.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/dataset/example.022.AA.bctoNOG.ENOG41099IZ.fasta` & `pytrimal-0.7.0/vendor/trimal/dataset/example.022.AA.bctoNOG.ENOG41099IZ.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/dataset/example.023.AA.bctoNOG.ENOG41099K3.fasta` & `pytrimal-0.7.0/vendor/trimal/dataset/example.023.AA.bctoNOG.ENOG41099K3.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/dataset/example.024.AA.bctoNOG.ENOG41099KM.fasta` & `pytrimal-0.7.0/vendor/trimal/dataset/example.024.AA.bctoNOG.ENOG41099KM.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/dataset/example.025.AA.bctoNOG.ENOG41099KP.fasta` & `pytrimal-0.7.0/vendor/trimal/dataset/example.025.AA.bctoNOG.ENOG41099KP.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/dataset/example.026.AA.bctoNOG.ENOG41099MV.fasta` & `pytrimal-0.7.0/vendor/trimal/dataset/example.026.AA.bctoNOG.ENOG41099MV.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/dataset/example.027.AA.bctoNOG.ENOG41099NY.fasta` & `pytrimal-0.7.0/vendor/trimal/dataset/example.027.AA.bctoNOG.ENOG41099NY.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/dataset/example.028.AA.bctoNOG.ENOG41099PA.fasta` & `pytrimal-0.7.0/vendor/trimal/dataset/example.028.AA.bctoNOG.ENOG41099PA.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/dataset/example.029.AA.bctoNOG.ENOG41099Q3.fasta` & `pytrimal-0.7.0/vendor/trimal/dataset/example.029.AA.bctoNOG.ENOG41099Q3.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/dataset/example.030.AA.bctoNOG.ENOG41099RG.fasta` & `pytrimal-0.7.0/vendor/trimal/dataset/example.030.AA.bctoNOG.ENOG41099RG.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/dataset/example.031.AA.bctoNOG.ENOG41099UK.fasta` & `pytrimal-0.7.0/vendor/trimal/dataset/example.031.AA.bctoNOG.ENOG41099UK.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/dataset/example.032.AA.bctoNOG.ENOG41099UW.fasta` & `pytrimal-0.7.0/vendor/trimal/dataset/example.032.AA.bctoNOG.ENOG41099UW.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/dataset/example.033.AA.bctoNOG.ENOG41099VK.fasta` & `pytrimal-0.7.0/vendor/trimal/dataset/example.033.AA.bctoNOG.ENOG41099VK.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/dataset/example.034.AA.bctoNOG.ENOG41099WA.fasta` & `pytrimal-0.7.0/vendor/trimal/dataset/example.034.AA.bctoNOG.ENOG41099WA.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/dataset/example.035.AA.bctoNOG.ENOG41099WF.fasta` & `pytrimal-0.7.0/vendor/trimal/dataset/example.035.AA.bctoNOG.ENOG41099WF.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/dataset/example.036.AA.bctoNOG.ENOG41099XJ.fasta` & `pytrimal-0.7.0/vendor/trimal/dataset/example.036.AA.bctoNOG.ENOG41099XJ.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/dataset/example.037.AA.bctoNOG.ENOG41099XP.fasta` & `pytrimal-0.7.0/vendor/trimal/dataset/example.037.AA.bctoNOG.ENOG41099XP.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/dataset/example.038.AA.bctoNOG.ENOG41099Y4.fasta` & `pytrimal-0.7.0/vendor/trimal/dataset/example.038.AA.bctoNOG.ENOG41099Y4.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/dataset/example.039.AA.bctoNOG.ENOG41099YD.fasta` & `pytrimal-0.7.0/vendor/trimal/dataset/example.039.AA.bctoNOG.ENOG41099YD.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/dataset/example.040.AA.bctoNOG.ENOG4109A32.fasta` & `pytrimal-0.7.0/vendor/trimal/dataset/example.040.AA.bctoNOG.ENOG4109A32.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/dataset/example.041.AA.bctoNOG.ENOG4109A5T.fasta` & `pytrimal-0.7.0/vendor/trimal/dataset/example.041.AA.bctoNOG.ENOG4109A5T.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/dataset/example.042.AA.bctoNOG.ENOG4109A9M.fasta` & `pytrimal-0.7.0/vendor/trimal/dataset/example.042.AA.bctoNOG.ENOG4109A9M.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/dataset/example.043.AA.bctoNOG.ENOG4109ADN.fasta` & `pytrimal-0.7.0/vendor/trimal/dataset/example.043.AA.bctoNOG.ENOG4109ADN.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/dataset/example.044.AA.bctoNOG.ENOG4109AED.fasta` & `pytrimal-0.7.0/vendor/trimal/dataset/example.044.AA.bctoNOG.ENOG4109AED.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/dataset/example.045.AA.bctoNOG.ENOG4109AGT.fasta` & `pytrimal-0.7.0/vendor/trimal/dataset/example.045.AA.bctoNOG.ENOG4109AGT.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/dataset/example.046.AA.bctoNOG.ENOG4109AGW.fasta` & `pytrimal-0.7.0/vendor/trimal/dataset/example.046.AA.bctoNOG.ENOG4109AGW.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/dataset/example.047.AA.bctoNOG.ENOG4109AIC.fasta` & `pytrimal-0.7.0/vendor/trimal/dataset/example.047.AA.bctoNOG.ENOG4109AIC.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/dataset/example.048.AA.bctoNOG.ENOG4109AJ3.fasta` & `pytrimal-0.7.0/vendor/trimal/dataset/example.048.AA.bctoNOG.ENOG4109AJ3.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/dataset/example.049.AA.bctoNOG.ENOG4109AY5.fasta` & `pytrimal-0.7.0/vendor/trimal/dataset/example.049.AA.bctoNOG.ENOG4109AY5.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/dataset/example.050.AA.bctoNOG.ENOG4109B8Z.fasta` & `pytrimal-0.7.0/vendor/trimal/dataset/example.050.AA.bctoNOG.ENOG4109B8Z.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/dataset/example.051.AA.bctoNOG.ENOG4109BCJ.fasta` & `pytrimal-0.7.0/vendor/trimal/dataset/example.051.AA.bctoNOG.ENOG4109BCJ.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/dataset/example.052.AA.bctoNOG.ENOG4109CTU.fasta` & `pytrimal-0.7.0/vendor/trimal/dataset/example.052.AA.bctoNOG.ENOG4109CTU.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/dataset/example.053.AA.bctoNOG.ENOG4109CVC.fasta` & `pytrimal-0.7.0/vendor/trimal/dataset/example.053.AA.bctoNOG.ENOG4109CVC.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/dataset/example.054.AA.bctoNOG.ENOG4109FIT.fasta` & `pytrimal-0.7.0/vendor/trimal/dataset/example.054.AA.bctoNOG.ENOG4109FIT.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/dataset/example.055.AA.bctoNOG.ENOG4109GY9.fasta` & `pytrimal-0.7.0/vendor/trimal/dataset/example.055.AA.bctoNOG.ENOG4109GY9.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/dataset/example.056.AA.bctoNOG.ENOG4109IPJ.fasta` & `pytrimal-0.7.0/vendor/trimal/dataset/example.056.AA.bctoNOG.ENOG4109IPJ.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/dataset/example.057.AA.bctoNOG.ENOG4109SZ2.fasta` & `pytrimal-0.7.0/vendor/trimal/dataset/example.057.AA.bctoNOG.ENOG4109SZ2.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/dataset/example.058.AA.strNOG.ENOG411BBR6.fasta` & `pytrimal-0.7.0/vendor/trimal/dataset/example.058.AA.strNOG.ENOG411BBR6.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/dataset/example.059.AA.strNOG.ENOG411BBRR.fasta` & `pytrimal-0.7.0/vendor/trimal/dataset/example.059.AA.strNOG.ENOG411BBRR.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/dataset/example.060.AA.strNOG.ENOG411BBWK.fasta` & `pytrimal-0.7.0/vendor/trimal/dataset/example.060.AA.strNOG.ENOG411BBWK.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/dataset/example.061.AA.strNOG.ENOG411BCDZ.fasta` & `pytrimal-0.7.0/vendor/trimal/dataset/example.061.AA.strNOG.ENOG411BCDZ.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/dataset/example.062.AA.strNOG.ENOG411BCX3.fasta` & `pytrimal-0.7.0/vendor/trimal/dataset/example.062.AA.strNOG.ENOG411BCX3.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/dataset/example.063.AA.strNOG.ENOG411BDBU.fasta` & `pytrimal-0.7.0/vendor/trimal/dataset/example.063.AA.strNOG.ENOG411BDBU.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/dataset/example.064.AA.strNOG.ENOG411BDKC.fasta` & `pytrimal-0.7.0/vendor/trimal/dataset/example.064.AA.strNOG.ENOG411BDKC.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/dataset/example.065.AA.strNOG.ENOG411BDSZ.fasta` & `pytrimal-0.7.0/vendor/trimal/dataset/example.065.AA.strNOG.ENOG411BDSZ.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/dataset/example.066.AA.strNOG.ENOG411BDUE.fasta` & `pytrimal-0.7.0/vendor/trimal/dataset/example.066.AA.strNOG.ENOG411BDUE.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/dataset/example.067.AA.strNOG.ENOG411BDX3.fasta` & `pytrimal-0.7.0/vendor/trimal/dataset/example.067.AA.strNOG.ENOG411BDX3.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/dataset/example.068.AA.strNOG.ENOG411BE45.fasta` & `pytrimal-0.7.0/vendor/trimal/dataset/example.068.AA.strNOG.ENOG411BE45.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/dataset/example.069.AA.strNOG.ENOG411BE8B.fasta` & `pytrimal-0.7.0/vendor/trimal/dataset/example.069.AA.strNOG.ENOG411BE8B.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/dataset/example.070.AA.strNOG.ENOG411BEUV.fasta` & `pytrimal-0.7.0/vendor/trimal/dataset/example.070.AA.strNOG.ENOG411BEUV.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/dataset/example.071.AA.strNOG.ENOG411BEZ0.fasta` & `pytrimal-0.7.0/vendor/trimal/dataset/example.071.AA.strNOG.ENOG411BEZ0.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/dataset/example.072.AA.strNOG.ENOG411BF1S.fasta` & `pytrimal-0.7.0/vendor/trimal/dataset/example.072.AA.strNOG.ENOG411BF1S.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/dataset/example.073.AA.strNOG.ENOG411BFCW.fasta` & `pytrimal-0.7.0/vendor/trimal/dataset/example.073.AA.strNOG.ENOG411BFCW.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/dataset/example.074.AA.strNOG.ENOG411BFPF.fasta` & `pytrimal-0.7.0/vendor/trimal/dataset/example.074.AA.strNOG.ENOG411BFPF.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/dataset/example.075.AA.strNOG.ENOG411BFQS.fasta` & `pytrimal-0.7.0/vendor/trimal/dataset/example.075.AA.strNOG.ENOG411BFQS.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/dataset/example.076.AA.strNOG.ENOG411BH75.fasta` & `pytrimal-0.7.0/vendor/trimal/dataset/example.076.AA.strNOG.ENOG411BH75.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/dataset/example.077.AA.strNOG.ENOG411BH79.fasta` & `pytrimal-0.7.0/vendor/trimal/dataset/example.077.AA.strNOG.ENOG411BH79.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/dataset/example.078.AA.strNOG.ENOG411BH99.fasta` & `pytrimal-0.7.0/vendor/trimal/dataset/example.078.AA.strNOG.ENOG411BH99.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/dataset/example.079.AA.strNOG.ENOG411BJDC.fasta` & `pytrimal-0.7.0/vendor/trimal/dataset/example.079.AA.strNOG.ENOG411BJDC.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/dataset/example.080.AA.strNOG.ENOG411BJIF.fasta` & `pytrimal-0.7.0/vendor/trimal/dataset/example.080.AA.strNOG.ENOG411BJIF.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/dataset/example.081.AA.strNOG.ENOG411BK9X.fasta` & `pytrimal-0.7.0/vendor/trimal/dataset/example.081.AA.strNOG.ENOG411BK9X.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/dataset/example.082.AA.strNOG.ENOG411BKC5.fasta` & `pytrimal-0.7.0/vendor/trimal/dataset/example.082.AA.strNOG.ENOG411BKC5.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/dataset/example.083.AA.strNOG.ENOG411BMKC.fasta` & `pytrimal-0.7.0/vendor/trimal/dataset/example.083.AA.strNOG.ENOG411BMKC.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/dataset/example.084.AA.strNOG.ENOG411BNP9.fasta` & `pytrimal-0.7.0/vendor/trimal/dataset/example.084.AA.strNOG.ENOG411BNP9.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/dataset/example.085.AA.strNOG.ENOG411BQTJ.fasta` & `pytrimal-0.7.0/vendor/trimal/dataset/example.085.AA.strNOG.ENOG411BQTJ.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/dataset/example.086.AA.strNOG.ENOG411BR1D.fasta` & `pytrimal-0.7.0/vendor/trimal/dataset/example.086.AA.strNOG.ENOG411BR1D.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/dataset/example.087.AA.strNOG.ENOG411BRCH.fasta` & `pytrimal-0.7.0/vendor/trimal/dataset/example.087.AA.strNOG.ENOG411BRCH.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/dataset/example.088.AA.strNOG.ENOG411BSXF.fasta` & `pytrimal-0.7.0/vendor/trimal/dataset/example.088.AA.strNOG.ENOG411BSXF.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/dataset/example.089.AA.strNOG.ENOG411BV9B.fasta` & `pytrimal-0.7.0/vendor/trimal/dataset/example.089.AA.strNOG.ENOG411BV9B.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/dataset/example.090.AA.strNOG.ENOG411BVKR.fasta` & `pytrimal-0.7.0/vendor/trimal/dataset/example.090.AA.strNOG.ENOG411BVKR.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/dataset/example.091.AA.strNOG.ENOG411BWBU.codon.fa` & `pytrimal-0.7.0/vendor/trimal/dataset/example.091.AA.strNOG.ENOG411BWBU.codon.fa`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/dataset/example.091.AA.strNOG.ENOG411BWBU.fasta` & `pytrimal-0.7.0/vendor/trimal/dataset/example.091.AA.strNOG.ENOG411BWBU.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/dataset/example.092.DNA.fasta` & `pytrimal-0.7.0/vendor/trimal/dataset/example.092.DNA.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/dataset/example.093.DNA.fasta` & `pytrimal-0.7.0/vendor/trimal/dataset/example.093.DNA.fasta`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/dataset/example.094.DNADeg.sequential_phy` & `pytrimal-0.7.0/vendor/trimal/dataset/example.094.DNADeg.sequential_phy`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/dataset/matrix.BLOSUM62` & `pytrimal-0.7.0/vendor/trimal/dataset/matrix.BLOSUM62`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/include/Alignment/Alignment.h` & `pytrimal-0.7.0/vendor/trimal/include/Alignment/Alignment.h`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/include/Alignment/sequencesMatrix.h` & `pytrimal-0.7.0/vendor/trimal/include/Alignment/sequencesMatrix.h`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/include/Cleaner.h` & `pytrimal-0.7.0/vendor/trimal/include/Cleaner.h`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/include/FormatHandling/BaseFormatHandler.h` & `pytrimal-0.7.0/vendor/trimal/include/FormatHandling/BaseFormatHandler.h`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/include/FormatHandling/FormatManager.h` & `pytrimal-0.7.0/vendor/trimal/include/FormatHandling/FormatManager.h`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/include/FormatHandling/clustal_state.h` & `pytrimal-0.7.0/vendor/trimal/include/FormatHandling/clustal_state.h`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/include/FormatHandling/fasta_m10_state.h` & `pytrimal-0.7.0/vendor/trimal/include/FormatHandling/fasta_m10_state.h`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/include/FormatHandling/fasta_state.h` & `pytrimal-0.7.0/vendor/trimal/include/FormatHandling/fasta_state.h`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/include/FormatHandling/formats_header.h` & `pytrimal-0.7.0/vendor/trimal/include/FormatHandling/formats_header.h`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/include/FormatHandling/htmlreport_state.h` & `pytrimal-0.7.0/vendor/trimal/include/FormatHandling/htmlreport_state.h`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/include/FormatHandling/mega_interleaved_state.h` & `pytrimal-0.7.0/vendor/trimal/include/FormatHandling/mega_interleaved_state.h`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/include/FormatHandling/mega_sequential_state.h` & `pytrimal-0.7.0/vendor/trimal/include/FormatHandling/mega_sequential_state.h`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/include/FormatHandling/nexus_m10_state.h` & `pytrimal-0.7.0/vendor/trimal/include/FormatHandling/nexus_m10_state.h`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/include/FormatHandling/nexus_state.h` & `pytrimal-0.7.0/vendor/trimal/include/FormatHandling/nexus_state.h`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/include/FormatHandling/phylip32_m10_state.h` & `pytrimal-0.7.0/vendor/trimal/include/FormatHandling/phylip32_m10_state.h`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/include/FormatHandling/phylip32_state.h` & `pytrimal-0.7.0/vendor/trimal/include/FormatHandling/phylip32_state.h`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/include/FormatHandling/phylip40_m10_state.h` & `pytrimal-0.7.0/vendor/trimal/include/FormatHandling/phylip40_m10_state.h`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/include/FormatHandling/phylip40_state.h` & `pytrimal-0.7.0/vendor/trimal/include/FormatHandling/phylip40_state.h`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/include/FormatHandling/phylip_paml_m10_state.h` & `pytrimal-0.7.0/vendor/trimal/include/FormatHandling/phylip_paml_m10_state.h`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/include/FormatHandling/phylip_paml_state.h` & `pytrimal-0.7.0/vendor/trimal/include/FormatHandling/phylip_paml_state.h`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/include/FormatHandling/pir_state.h` & `pytrimal-0.7.0/vendor/trimal/include/FormatHandling/pir_state.h`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/include/InternalBenchmarker.h` & `pytrimal-0.7.0/vendor/trimal/include/InternalBenchmarker.h`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/include/RawText/examples.txt` & `pytrimal-0.7.0/vendor/trimal/include/RawText/examples.txt`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/include/RawText/legacyMenu.txt` & `pytrimal-0.7.0/vendor/trimal/include/RawText/legacyMenu.txt`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/include/RawText/menu.txt` & `pytrimal-0.7.0/vendor/trimal/include/RawText/menu.txt`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/include/Statistics/Consistency.h` & `pytrimal-0.7.0/vendor/trimal/include/Statistics/Consistency.h`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/include/Statistics/Gaps.h` & `pytrimal-0.7.0/vendor/trimal/include/Statistics/Gaps.h`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/include/Statistics/Manager.h` & `pytrimal-0.7.0/vendor/trimal/include/Statistics/Manager.h`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/include/Statistics/Mold.h` & `pytrimal-0.7.0/vendor/trimal/include/Statistics/Mold.h`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/include/Statistics/Similarity.h` & `pytrimal-0.7.0/vendor/trimal/include/Statistics/Similarity.h`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/include/Statistics/similarityMatrix.h` & `pytrimal-0.7.0/vendor/trimal/include/Statistics/similarityMatrix.h`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/include/VCFHandler.h` & `pytrimal-0.7.0/vendor/trimal/include/VCFHandler.h`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/include/defines.h` & `pytrimal-0.7.0/vendor/trimal/include/defines.h`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/include/reportsystem.h` & `pytrimal-0.7.0/vendor/trimal/include/reportsystem.h`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/include/trimalManager.h` & `pytrimal-0.7.0/vendor/trimal/include/trimalManager.h`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/include/utils.h` & `pytrimal-0.7.0/vendor/trimal/include/utils.h`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/include/values.h` & `pytrimal-0.7.0/vendor/trimal/include/values.h`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/source/Alignment/Alignment.cpp` & `pytrimal-0.7.0/vendor/trimal/source/Alignment/Alignment.cpp`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/source/Alignment/sequencesMatrix.cpp` & `pytrimal-0.7.0/vendor/trimal/source/Alignment/sequencesMatrix.cpp`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/source/Cleaner.cpp` & `pytrimal-0.7.0/vendor/trimal/source/Cleaner.cpp`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/source/FormatHandling/BaseFormatHandler.cpp` & `pytrimal-0.7.0/vendor/trimal/source/FormatHandling/BaseFormatHandler.cpp`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/source/FormatHandling/clustal_state.cpp` & `pytrimal-0.7.0/vendor/trimal/source/FormatHandling/clustal_state.cpp`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/source/FormatHandling/fasta_m10_state.cpp` & `pytrimal-0.7.0/vendor/trimal/source/FormatHandling/fasta_m10_state.cpp`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/source/FormatHandling/fasta_state.cpp` & `pytrimal-0.7.0/vendor/trimal/source/FormatHandling/fasta_state.cpp`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/source/FormatHandling/htmlreport_state.cpp` & `pytrimal-0.7.0/vendor/trimal/source/FormatHandling/htmlreport_state.cpp`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/source/FormatHandling/mega_interleaved_state.cpp` & `pytrimal-0.7.0/vendor/trimal/source/FormatHandling/mega_interleaved_state.cpp`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/source/FormatHandling/mega_sequential_state.cpp` & `pytrimal-0.7.0/vendor/trimal/source/FormatHandling/mega_sequential_state.cpp`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/source/FormatHandling/nexus_m10_state.cpp` & `pytrimal-0.7.0/vendor/trimal/source/FormatHandling/nexus_m10_state.cpp`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/source/FormatHandling/nexus_state.cpp` & `pytrimal-0.7.0/vendor/trimal/source/FormatHandling/nexus_state.cpp`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/source/FormatHandling/phylip32_m10_state.cpp` & `pytrimal-0.7.0/vendor/trimal/source/FormatHandling/phylip32_m10_state.cpp`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/source/FormatHandling/phylip32_state.cpp` & `pytrimal-0.7.0/vendor/trimal/source/FormatHandling/phylip32_state.cpp`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/source/FormatHandling/phylip40_m10_state.cpp` & `pytrimal-0.7.0/vendor/trimal/source/FormatHandling/phylip40_m10_state.cpp`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/source/FormatHandling/phylip40_state.cpp` & `pytrimal-0.7.0/vendor/trimal/source/FormatHandling/phylip40_state.cpp`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/source/FormatHandling/phylip_paml_m10_state.cpp` & `pytrimal-0.7.0/vendor/trimal/source/FormatHandling/phylip_paml_m10_state.cpp`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/source/FormatHandling/phylip_paml_state.cpp` & `pytrimal-0.7.0/vendor/trimal/source/FormatHandling/phylip_paml_state.cpp`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/source/FormatHandling/pir_state.cpp` & `pytrimal-0.7.0/vendor/trimal/source/FormatHandling/pir_state.cpp`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/source/FormatHandling/readAlMain.cpp` & `pytrimal-0.7.0/vendor/trimal/source/FormatHandling/readAlMain.cpp`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/source/InternalBenchmarker.cpp` & `pytrimal-0.7.0/vendor/trimal/source/InternalBenchmarker.cpp`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/source/Statistics/Consistency.cpp` & `pytrimal-0.7.0/vendor/trimal/source/Statistics/Consistency.cpp`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/source/Statistics/Gaps.cpp` & `pytrimal-0.7.0/vendor/trimal/source/Statistics/Gaps.cpp`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/source/Statistics/Manager.cpp` & `pytrimal-0.7.0/vendor/trimal/source/Statistics/Manager.cpp`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/source/Statistics/Mold.cpp` & `pytrimal-0.7.0/vendor/trimal/source/Statistics/Mold.cpp`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/source/Statistics/Similarity.cpp` & `pytrimal-0.7.0/vendor/trimal/source/Statistics/Similarity.cpp`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/source/Statistics/similarityMatrix.cpp` & `pytrimal-0.7.0/vendor/trimal/source/Statistics/similarityMatrix.cpp`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/source/VCFHandler.cpp` & `pytrimal-0.7.0/vendor/trimal/source/VCFHandler.cpp`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/source/alignment.cpp` & `pytrimal-0.7.0/vendor/trimal/source/alignment.cpp`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/source/compareFiles.cpp` & `pytrimal-0.7.0/vendor/trimal/source/compareFiles.cpp`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/source/main.cpp` & `pytrimal-0.7.0/vendor/trimal/source/main.cpp`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/source/reportMessages/errorMessages.cpp` & `pytrimal-0.7.0/vendor/trimal/source/reportMessages/errorMessages.cpp`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/source/reportMessages/infoMessages.cpp` & `pytrimal-0.7.0/vendor/trimal/source/reportMessages/infoMessages.cpp`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/source/reportMessages/warningMessages.cpp` & `pytrimal-0.7.0/vendor/trimal/source/reportMessages/warningMessages.cpp`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/source/reportsystem.cpp` & `pytrimal-0.7.0/vendor/trimal/source/reportsystem.cpp`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/source/rwAlignment.cpp` & `pytrimal-0.7.0/vendor/trimal/source/rwAlignment.cpp`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/source/trimAlMain.cpp` & `pytrimal-0.7.0/vendor/trimal/source/trimAlMain.cpp`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/source/trimalManager.cpp` & `pytrimal-0.7.0/vendor/trimal/source/trimalManager.cpp`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/source/typeHelper.cpp` & `pytrimal-0.7.0/vendor/trimal/source/typeHelper.cpp`

 * *Files identical despite different names*

### Comparing `pytrimal-0.6.0/vendor/trimal/source/utils.cpp` & `pytrimal-0.7.0/vendor/trimal/source/utils.cpp`

 * *Files identical despite different names*

