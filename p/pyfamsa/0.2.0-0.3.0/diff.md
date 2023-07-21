# Comparing `tmp/pyfamsa-0.2.0.tar.gz` & `tmp/pyfamsa-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfamsa-0.2.0.tar", last modified: Thu Dec 22 01:30:56 2022, max compression
+gzip compressed data, was "pyfamsa-0.3.0.tar", last modified: Fri Jul 21 17:39:19 2023, max compression
```

## Comparing `pyfamsa-0.2.0.tar` & `pyfamsa-0.3.0.tar`

### file list

```diff
@@ -1,259 +1,259 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 01:30:56.301630 pyfamsa-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2022-12-22 01:30:47.000000 pyfamsa-0.2.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2022-12-22 01:30:47.000000 pyfamsa-0.2.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    35148 2022-12-22 01:30:47.000000 pyfamsa-0.2.0/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)      571 2022-12-22 01:30:47.000000 pyfamsa-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10565 2022-12-22 01:30:56.301630 pyfamsa-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8721 2022-12-22 01:30:47.000000 pyfamsa-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 01:30:56.273630 pyfamsa-0.2.0/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 01:30:56.277630 pyfamsa-0.2.0/include/famsa/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-22 01:30:47.000000 pyfamsa-0.2.0/include/famsa/__init__.pxd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 01:30:56.277630 pyfamsa-0.2.0/include/famsa/core/
--rw-r--r--   0 runner    (1001) docker     (123)      863 2022-12-22 01:30:47.000000 pyfamsa-0.2.0/include/famsa/core/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (123)      696 2022-12-22 01:30:47.000000 pyfamsa-0.2.0/include/famsa/core/io_service.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     2228 2022-12-22 01:30:47.000000 pyfamsa-0.2.0/include/famsa/core/params.pxd
--rw-r--r--   0 runner    (1001) docker     (123)      373 2022-12-22 01:30:47.000000 pyfamsa-0.2.0/include/famsa/core/profile.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     2128 2022-12-22 01:30:47.000000 pyfamsa-0.2.0/include/famsa/core/sequence.pxd
--rw-r--r--   0 runner    (1001) docker     (123)      123 2022-12-22 01:30:47.000000 pyfamsa-0.2.0/include/famsa/core/version.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1602 2022-12-22 01:30:47.000000 pyfamsa-0.2.0/include/famsa/msa.pxd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 01:30:56.277630 pyfamsa-0.2.0/include/famsa/tree/
--rw-r--r--   0 runner    (1001) docker     (123)      498 2022-12-22 01:30:47.000000 pyfamsa-0.2.0/include/famsa/tree/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (123)      441 2022-12-22 01:30:47.000000 pyfamsa-0.2.0/include/famsa/tree/abstract_tree_generator.pxd
--rw-r--r--   0 runner    (1001) docker     (123)      454 2022-12-22 01:30:47.000000 pyfamsa-0.2.0/include/famsa/tree/guide_tree.pxd
--rw-r--r--   0 runner    (1001) docker     (123)      612 2022-12-22 01:30:47.000000 pyfamsa-0.2.0/include/famsa/tree/newick_parser.pxd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 01:30:56.277630 pyfamsa-0.2.0/include/famsa/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-22 01:30:47.000000 pyfamsa-0.2.0/include/famsa/utils/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (123)      363 2022-12-22 01:30:47.000000 pyfamsa-0.2.0/include/famsa/utils/log.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2022-12-22 01:30:47.000000 pyfamsa-0.2.0/include/famsa/utils/memory_monotonic.pxd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 01:30:56.277630 pyfamsa-0.2.0/patches/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2022-12-22 01:30:47.000000 pyfamsa-0.2.0/patches/NewickParser.h.patch
--rw-r--r--   0 runner    (1001) docker     (123)     1730 2022-12-22 01:30:47.000000 pyfamsa-0.2.0/patches/memory_monotonic.h.patch
--rw-r--r--   0 runner    (1001) docker     (123)      304 2022-12-22 01:30:47.000000 pyfamsa-0.2.0/patches/msa.cpp.patch
--rw-r--r--   0 runner    (1001) docker     (123)       41 2022-12-22 01:30:47.000000 pyfamsa-0.2.0/patches/msa.h.patch
--rw-r--r--   0 runner    (1001) docker     (123)     1675 2022-12-22 01:30:47.000000 pyfamsa-0.2.0/patches/sequence.cpp.patch
--rw-r--r--   0 runner    (1001) docker     (123)      695 2022-12-22 01:30:47.000000 pyfamsa-0.2.0/patches/sequence.h.patch
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 01:30:56.281630 pyfamsa-0.2.0/pyfamsa/
--rw-r--r--   0 runner    (1001) docker     (123)      424 2022-12-22 01:30:47.000000 pyfamsa-0.2.0/pyfamsa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2022-12-22 01:30:47.000000 pyfamsa-0.2.0/pyfamsa/_famsa.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2022-12-22 01:30:47.000000 pyfamsa-0.2.0/pyfamsa/_famsa.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    18693 2022-12-22 01:30:47.000000 pyfamsa-0.2.0/pyfamsa/_famsa.pyx
--rw-r--r--   0 runner    (1001) docker     (123)       22 2022-12-22 01:30:47.000000 pyfamsa-0.2.0/pyfamsa/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-22 01:30:47.000000 pyfamsa-0.2.0/pyfamsa/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 01:30:56.281630 pyfamsa-0.2.0/pyfamsa/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      330 2022-12-22 01:30:47.000000 pyfamsa-0.2.0/pyfamsa/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       65 2022-12-22 01:30:47.000000 pyfamsa-0.2.0/pyfamsa/tests/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 01:30:56.289630 pyfamsa-0.2.0/pyfamsa/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-22 01:30:47.000000 pyfamsa-0.2.0/pyfamsa/tests/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    47464 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/pyfamsa/tests/data/adeno_fiber.faa
--rw-r--r--   0 runner    (1001) docker     (123)    68569 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/pyfamsa/tests/data/adeno_fiber.sl.afa
--rw-r--r--   0 runner    (1001) docker     (123)     7333 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/pyfamsa/tests/data/adeno_fiber.sl.nwk
--rw-r--r--   0 runner    (1001) docker     (123)    70021 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/pyfamsa/tests/data/adeno_fiber.upgma.afa
--rw-r--r--   0 runner    (1001) docker     (123)     7333 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/pyfamsa/tests/data/adeno_fiber.upgma.nwk
--rw-r--r--   0 runner    (1001) docker     (123)   287439 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/pyfamsa/tests/data/hemopexin.faa
--rw-r--r--   0 runner    (1001) docker     (123)  2097465 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/pyfamsa/tests/data/hemopexin.medoid-nj.afa
--rw-r--r--   0 runner    (1001) docker     (123)   129095 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/pyfamsa/tests/data/hemopexin.medoid-nj.nwk
--rw-r--r--   0 runner    (1001) docker     (123)  1913193 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/pyfamsa/tests/data/hemopexin.medoid-sl.afa
--rw-r--r--   0 runner    (1001) docker     (123)   129095 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/pyfamsa/tests/data/hemopexin.medoid-sl.nwk
--rw-r--r--   0 runner    (1001) docker     (123)   129095 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/pyfamsa/tests/data/hemopexin.medoid-slink.nwk
--rw-r--r--   0 runner    (1001) docker     (123)  2030457 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/pyfamsa/tests/data/hemopexin.medoid-upgma.afa
--rw-r--r--   0 runner    (1001) docker     (123)   129095 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/pyfamsa/tests/data/hemopexin.medoid-upgma.nwk
--rw-r--r--   0 runner    (1001) docker     (123)      849 2022-12-22 01:30:47.000000 pyfamsa-0.2.0/pyfamsa/tests/fasta.py
--rw-r--r--   0 runner    (1001) docker     (123)       45 2022-12-22 01:30:47.000000 pyfamsa-0.2.0/pyfamsa/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4107 2022-12-22 01:30:47.000000 pyfamsa-0.2.0/pyfamsa/tests/test_aligner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2526 2022-12-22 01:30:47.000000 pyfamsa-0.2.0/pyfamsa/tests/test_doctest.py
--rw-r--r--   0 runner    (1001) docker     (123)      877 2022-12-22 01:30:47.000000 pyfamsa-0.2.0/pyfamsa/tests/test_sequence.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 01:30:56.281630 pyfamsa-0.2.0/pyfamsa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10565 2022-12-22 01:30:56.000000 pyfamsa-0.2.0/pyfamsa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9734 2022-12-22 01:30:56.000000 pyfamsa-0.2.0/pyfamsa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-22 01:30:56.000000 pyfamsa-0.2.0/pyfamsa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-22 01:30:56.000000 pyfamsa-0.2.0/pyfamsa.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        8 2022-12-22 01:30:56.000000 pyfamsa-0.2.0/pyfamsa.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      136 2022-12-22 01:30:56.000000 pyfamsa-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     3056 2022-12-22 01:30:56.301630 pyfamsa-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)    35241 2022-12-22 01:30:47.000000 pyfamsa-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 01:30:56.273630 pyfamsa-0.2.0/vendor/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 01:30:56.289630 pyfamsa-0.2.0/vendor/FAMSA/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13518 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 01:30:56.273630 pyfamsa-0.2.0/vendor/FAMSA/libs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 01:30:56.289630 pyfamsa-0.2.0/vendor/FAMSA/libs/atomic_wait/
--rw-r--r--   0 runner    (1001) docker     (123)    12610 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/libs/atomic_wait/atomic_wait
--rw-r--r--   0 runner    (1001) docker     (123)     9777 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/libs/atomic_wait/barrier
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/libs/atomic_wait/latch
--rw-r--r--   0 runner    (1001) docker     (123)    17651 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/libs/atomic_wait/semaphore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 01:30:56.289630 pyfamsa-0.2.0/vendor/FAMSA/libs/libdeflate/
--rw-r--r--   0 runner    (1001) docker     (123)      163 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/libs/libdeflate/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/libs/libdeflate/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)    13487 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/libs/libdeflate/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     9437 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/libs/libdeflate/NEWS.md
--rw-r--r--   0 runner    (1001) docker     (123)    12146 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/libs/libdeflate/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 01:30:56.289630 pyfamsa-0.2.0/vendor/FAMSA/libs/libdeflate/common/
--rw-r--r--   0 runner    (1001) docker     (123)     9618 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/libs/libdeflate/common/common_defs.h
--rw-r--r--   0 runner    (1001) docker     (123)     8596 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/libs/libdeflate/common/compiler_gcc.h
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/libs/libdeflate/common/compiler_msc.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 01:30:56.293630 pyfamsa-0.2.0/vendor/FAMSA/libs/libdeflate/lib/
--rw-r--r--   0 runner    (1001) docker     (123)     3638 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/libs/libdeflate/lib/adler32.c
--rw-r--r--   0 runner    (1001) docker     (123)     3918 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/libs/libdeflate/lib/adler32_vec_template.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 01:30:56.293630 pyfamsa-0.2.0/vendor/FAMSA/libs/libdeflate/lib/arm/
--rw-r--r--   0 runner    (1001) docker     (123)     4527 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/libs/libdeflate/lib/arm/adler32_impl.h
--rw-r--r--   0 runner    (1001) docker     (123)     3738 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/libs/libdeflate/lib/arm/cpu_features.c
--rw-r--r--   0 runner    (1001) docker     (123)      860 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/libs/libdeflate/lib/arm/cpu_features.h
--rw-r--r--   0 runner    (1001) docker     (123)     7595 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/libs/libdeflate/lib/arm/crc32_impl.h
--rw-r--r--   0 runner    (1001) docker     (123)     2839 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/libs/libdeflate/lib/arm/matchfinder_impl.h
--rw-r--r--   0 runner    (1001) docker     (123)    11537 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/libs/libdeflate/lib/bt_matchfinder.h
--rw-r--r--   0 runner    (1001) docker     (123)     2711 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/libs/libdeflate/lib/cpu_features_common.h
--rw-r--r--   0 runner    (1001) docker     (123)    10495 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/libs/libdeflate/lib/crc32.c
--rw-r--r--   0 runner    (1001) docker     (123)    25448 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/libs/libdeflate/lib/crc32_table.h
--rw-r--r--   0 runner    (1001) docker     (123)     2114 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/libs/libdeflate/lib/crc32_vec_template.h
--rw-r--r--   0 runner    (1001) docker     (123)    12769 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/libs/libdeflate/lib/decompress_template.h
--rw-r--r--   0 runner    (1001) docker     (123)   124274 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/libs/libdeflate/lib/deflate_compress.c
--rw-r--r--   0 runner    (1001) docker     (123)      395 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/libs/libdeflate/lib/deflate_compress.h
--rw-r--r--   0 runner    (1001) docker     (123)     1855 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/libs/libdeflate/lib/deflate_constants.h
--rw-r--r--   0 runner    (1001) docker     (123)    38953 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/libs/libdeflate/lib/deflate_decompress.c
--rw-r--r--   0 runner    (1001) docker     (123)     2744 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/libs/libdeflate/lib/gzip_compress.c
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/libs/libdeflate/lib/gzip_constants.h
--rw-r--r--   0 runner    (1001) docker     (123)     4054 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/libs/libdeflate/lib/gzip_decompress.c
--rw-r--r--   0 runner    (1001) docker     (123)    14042 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/libs/libdeflate/lib/hc_matchfinder.h
--rw-r--r--   0 runner    (1001) docker     (123)     7207 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/libs/libdeflate/lib/ht_matchfinder.h
--rw-r--r--   0 runner    (1001) docker     (123)     2548 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/libs/libdeflate/lib/lib_common.h
--rw-r--r--   0 runner    (1001) docker     (123)     5124 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/libs/libdeflate/lib/matchfinder_common.h
--rw-r--r--   0 runner    (1001) docker     (123)     5645 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/libs/libdeflate/lib/unaligned.h
--rw-r--r--   0 runner    (1001) docker     (123)     3284 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/libs/libdeflate/lib/utils.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 01:30:56.293630 pyfamsa-0.2.0/vendor/FAMSA/libs/libdeflate/lib/x86/
--rw-r--r--   0 runner    (1001) docker     (123)    12149 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/libs/libdeflate/lib/x86/adler32_impl.h
--rw-r--r--   0 runner    (1001) docker     (123)     4567 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/libs/libdeflate/lib/x86/cpu_features.c
--rw-r--r--   0 runner    (1001) docker     (123)      931 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/libs/libdeflate/lib/x86/cpu_features.h
--rw-r--r--   0 runner    (1001) docker     (123)     3233 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/libs/libdeflate/lib/x86/crc32_impl.h
--rw-r--r--   0 runner    (1001) docker     (123)    10451 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/libs/libdeflate/lib/x86/crc32_pclmul_template.h
--rw-r--r--   0 runner    (1001) docker     (123)      734 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/libs/libdeflate/lib/x86/decompress_impl.h
--rw-r--r--   0 runner    (1001) docker     (123)     3742 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/libs/libdeflate/lib/x86/matchfinder_impl.h
--rw-r--r--   0 runner    (1001) docker     (123)     2697 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/libs/libdeflate/lib/zlib_compress.c
--rw-r--r--   0 runner    (1001) docker     (123)      488 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/libs/libdeflate/lib/zlib_constants.h
--rw-r--r--   0 runner    (1001) docker     (123)     3196 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/libs/libdeflate/lib/zlib_decompress.c
--rw-r--r--   0 runner    (1001) docker     (123)    15154 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/libs/libdeflate/libdeflate.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 01:30:56.293630 pyfamsa-0.2.0/vendor/FAMSA/libs/libdeflate/programs/
--rw-r--r--   0 runner    (1001) docker     (123)    17356 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/libs/libdeflate/programs/benchmark.c
--rw-r--r--   0 runner    (1001) docker     (123)     4605 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/libs/libdeflate/programs/checksum.c
--rw-r--r--   0 runner    (1001) docker     (123)    17835 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/libs/libdeflate/programs/gzip.c
--rw-r--r--   0 runner    (1001) docker     (123)    11580 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/libs/libdeflate/programs/prog_util.c
--rw-r--r--   0 runner    (1001) docker     (123)     4845 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/libs/libdeflate/programs/prog_util.h
--rw-r--r--   0 runner    (1001) docker     (123)     5012 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/libs/libdeflate/programs/test_checksums.c
--rw-r--r--   0 runner    (1001) docker     (123)     1753 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/libs/libdeflate/programs/test_custom_malloc.c
--rw-r--r--   0 runner    (1001) docker     (123)    11890 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/libs/libdeflate/programs/test_incomplete_codes.c
--rw-r--r--   0 runner    (1001) docker     (123)     2207 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/libs/libdeflate/programs/test_litrunlen_overflow.c
--rw-r--r--   0 runner    (1001) docker     (123)     2686 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/libs/libdeflate/programs/test_overread.c
--rw-r--r--   0 runner    (1001) docker     (123)    22742 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/libs/libdeflate/programs/test_slow_decompression.c
--rw-r--r--   0 runner    (1001) docker     (123)     5221 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/libs/libdeflate/programs/test_trailing_bytes.c
--rw-r--r--   0 runner    (1001) docker     (123)     5695 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/libs/libdeflate/programs/test_util.c
--rw-r--r--   0 runner    (1001) docker     (123)     2127 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/libs/libdeflate/programs/test_util.h
--rw-r--r--   0 runner    (1001) docker     (123)     3530 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/libs/libdeflate/programs/tgetopt.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 01:30:56.293630 pyfamsa-0.2.0/vendor/FAMSA/libs/libdeflate/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1512 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/libs/libdeflate/scripts/detect.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 01:30:56.293630 pyfamsa-0.2.0/vendor/FAMSA/libs/libdeflate/windows/
--rw-r--r--   0 runner    (1001) docker     (123)    73752 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/libs/libdeflate/windows/libdeflatestatic.lib
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 01:30:56.297630 pyfamsa-0.2.0/vendor/FAMSA/libs/mimalloc/
--rw-r--r--   0 runner    (1001) docker     (123)    12441 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/libs/mimalloc/alloc-aligned.c
--rw-r--r--   0 runner    (1001) docker     (123)    13515 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/libs/mimalloc/alloc-override-osx.c
--rw-r--r--   0 runner    (1001) docker     (123)    14876 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/libs/mimalloc/alloc-override.c
--rw-r--r--   0 runner    (1001) docker     (123)     6227 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/libs/mimalloc/alloc-posix.c
--rw-r--r--   0 runner    (1001) docker     (123)    32874 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/libs/mimalloc/alloc.c
--rw-r--r--   0 runner    (1001) docker     (123)    19573 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/libs/mimalloc/arena.c
--rw-r--r--   0 runner    (1001) docker     (123)    16746 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/libs/mimalloc/bitmap.c
--rw-r--r--   0 runner    (1001) docker     (123)     5328 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/libs/mimalloc/bitmap.h
--rw-r--r--   0 runner    (1001) docker     (123)    20115 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/libs/mimalloc/heap.c
--rw-r--r--   0 runner    (1001) docker     (123)    25391 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/libs/mimalloc/init.c
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/libs/mimalloc/mimalloc-LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15171 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/libs/mimalloc/mimalloc-atomic.h
--rw-r--r--   0 runner    (1001) docker     (123)    40784 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/libs/mimalloc/mimalloc-internal.h
--rw-r--r--   0 runner    (1001) docker     (123)     3441 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/libs/mimalloc/mimalloc-new-delete.h
--rw-r--r--   0 runner    (1001) docker     (123)     3111 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/libs/mimalloc/mimalloc-override.h
--rw-r--r--   0 runner    (1001) docker     (123)    24060 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/libs/mimalloc/mimalloc-types.h
--rw-r--r--   0 runner    (1001) docker     (123)    28550 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/libs/mimalloc/mimalloc.h
--rw-r--r--   0 runner    (1001) docker     (123)    22798 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/libs/mimalloc/options.c
--rw-r--r--   0 runner    (1001) docker     (123)    55869 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/libs/mimalloc/os.c
--rw-r--r--   0 runner    (1001) docker     (123)      964 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/libs/mimalloc/override-new-delete.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    11537 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/libs/mimalloc/page-queue.c
--rw-r--r--   0 runner    (1001) docker     (123)    33440 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/libs/mimalloc/page.c
--rw-r--r--   0 runner    (1001) docker     (123)    12823 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/libs/mimalloc/random.c
--rw-r--r--   0 runner    (1001) docker     (123)    20963 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/libs/mimalloc/region.c
--rw-r--r--   0 runner    (1001) docker     (123)    14137 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/libs/mimalloc/segment-cache.c
--rw-r--r--   0 runner    (1001) docker     (123)    65602 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/libs/mimalloc/segment.c
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/libs/mimalloc/static.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    21607 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/libs/mimalloc/stats.c
--rw-r--r--   0 runner    (1001) docker     (123)     6925 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 01:30:56.297630 pyfamsa-0.2.0/vendor/FAMSA/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 01:30:56.297630 pyfamsa-0.2.0/vendor/FAMSA/src/core/
--rw-r--r--   0 runner    (1001) docker     (123)     3026 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/src/core/defs.h
--rw-r--r--   0 runner    (1001) docker     (123)     3997 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/src/core/io_service.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1535 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/src/core/io_service.h
--rw-r--r--   0 runner    (1001) docker     (123)     9007 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/src/core/params.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3892 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/src/core/params.h
--rw-r--r--   0 runner    (1001) docker     (123)    47408 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/src/core/profile.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    12974 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/src/core/profile.h
--rw-r--r--   0 runner    (1001) docker     (123)    31900 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/src/core/profile_par.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    29543 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/src/core/profile_seq.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5395 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/src/core/queues.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    11739 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/src/core/queues.h
--rw-r--r--   0 runner    (1001) docker     (123)    15198 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/src/core/sequence.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3011 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/src/core/sequence.h
--rw-r--r--   0 runner    (1001) docker     (123)     5184 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/src/core/version.h
--rw-r--r--   0 runner    (1001) docker     (123)     4077 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/src/famsa.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 01:30:56.297630 pyfamsa-0.2.0/vendor/FAMSA/src/lcs/
--rw-r--r--   0 runner    (1001) docker     (123)     5692 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/src/lcs/lcsbp.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      892 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/src/lcs/lcsbp.h
--rw-r--r--   0 runner    (1001) docker     (123)    12467 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/src/lcs/lcsbp_avx2_intr.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    13463 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/src/lcs/lcsbp_avx2_intr.h
--rw-r--r--   0 runner    (1001) docker     (123)     9376 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/src/lcs/lcsbp_avx_intr.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    10800 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/src/lcs/lcsbp_avx_intr.h
--rw-r--r--   0 runner    (1001) docker     (123)     8337 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/src/lcs/lcsbp_classic.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6561 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/src/lcs/lcsbp_classic.h
--rw-r--r--   0 runner    (1001) docker     (123)     9388 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/src/lcs/lcsbp_neon_intr.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    10511 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/src/lcs/lcsbp_neon_intr.h
--rw-r--r--   0 runner    (1001) docker     (123)    25404 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/src/msa.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2826 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/src/msa.h
--rw-r--r--   0 runner    (1001) docker     (123)     5908 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/src/msa_refinement.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 01:30:56.301630 pyfamsa-0.2.0/vendor/FAMSA/src/tree/
--rw-r--r--   0 runner    (1001) docker     (123)     2041 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/src/tree/AbstractTreeGenerator.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/src/tree/AbstractTreeGenerator.h
--rw-r--r--   0 runner    (1001) docker     (123)    12021 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/src/tree/AbstractTreeGenerator.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      605 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/src/tree/Chained.h
--rw-r--r--   0 runner    (1001) docker     (123)     9457 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/src/tree/Clustering.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      881 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/src/tree/Clustering.h
--rw-r--r--   0 runner    (1001) docker     (123)     3393 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/src/tree/DistanceCalculator.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      641 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/src/tree/DistanceCalculator.h
--rw-r--r--   0 runner    (1001) docker     (123)    10325 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/src/tree/FastTree.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/src/tree/FastTree.h
--rw-r--r--   0 runner    (1001) docker     (123)     5665 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/src/tree/GuideTree.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      883 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/src/tree/GuideTree.h
--rw-r--r--   0 runner    (1001) docker     (123)      202 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/src/tree/IPartialGenerator.h
--rw-r--r--   0 runner    (1001) docker     (123)    23238 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/src/tree/MSTPrim.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5505 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/src/tree/MSTPrim.h
--rw-r--r--   0 runner    (1001) docker     (123)     3409 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/src/tree/NeighborJoining.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      578 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/src/tree/NeighborJoining.h
--rw-r--r--   0 runner    (1001) docker     (123)     3856 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/src/tree/NewickParser.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      756 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/src/tree/NewickParser.h
--rw-r--r--   0 runner    (1001) docker     (123)     7809 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/src/tree/SingleLinkage.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/src/tree/SingleLinkage.h
--rw-r--r--   0 runner    (1001) docker     (123)     3474 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/src/tree/SingleLinkageQueue.h
--rw-r--r--   0 runner    (1001) docker     (123)     3371 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/src/tree/TreeDefs.h
--rw-r--r--   0 runner    (1001) docker     (123)     8934 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/src/tree/UPGMA.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2319 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/src/tree/UPGMA.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 01:30:56.301630 pyfamsa-0.2.0/vendor/FAMSA/src/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     8706 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/src/utils/array.h
--rw-r--r--   0 runner    (1001) docker     (123)     3864 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/src/utils/conversion.h
--rw-r--r--   0 runner    (1001) docker     (123)      769 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/src/utils/cpuid.h
--rw-r--r--   0 runner    (1001) docker     (123)     3257 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/src/utils/deterministic_random.h
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/src/utils/log.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4244 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/src/utils/log.h
--rw-r--r--   0 runner    (1001) docker     (123)     4581 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/src/utils/memory_monotonic.h
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/src/utils/meta_oper.h
--rw-r--r--   0 runner    (1001) docker     (123)     3725 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/src/utils/pooled_threads.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      870 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/src/utils/pooled_threads.h
--rw-r--r--   0 runner    (1001) docker     (123)     1787 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/src/utils/statistics.h
--rw-r--r--   0 runner    (1001) docker     (123)     1929 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/src/utils/timer.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/src/utils/timer.h
--rw-r--r--   0 runner    (1001) docker     (123)      313 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/src/utils/utils.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/src/utils/utils.h
--rw-r--r--   0 runner    (1001) docker     (123)      410 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/src/utils/utils_avx.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      393 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/src/utils/utils_avx2.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      371 2022-12-22 01:30:49.000000 pyfamsa-0.2.0/vendor/FAMSA/src/utils/utils_neon.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 17:39:19.066868 pyfamsa-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-07-21 17:39:11.000000 pyfamsa-0.3.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-07-21 17:39:11.000000 pyfamsa-0.3.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-07-21 17:39:11.000000 pyfamsa-0.3.0/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-07-21 17:39:11.000000 pyfamsa-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10428 2023-07-21 17:39:19.066868 pyfamsa-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8634 2023-07-21 17:39:11.000000 pyfamsa-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 17:39:19.034868 pyfamsa-0.3.0/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 17:39:19.042868 pyfamsa-0.3.0/include/famsa/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 17:39:11.000000 pyfamsa-0.3.0/include/famsa/__init__.pxd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 17:39:19.042868 pyfamsa-0.3.0/include/famsa/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-07-21 17:39:11.000000 pyfamsa-0.3.0/include/famsa/core/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-21 17:39:11.000000 pyfamsa-0.3.0/include/famsa/core/io_service.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-07-21 17:39:11.000000 pyfamsa-0.3.0/include/famsa/core/params.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-21 17:39:11.000000 pyfamsa-0.3.0/include/famsa/core/profile.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-07-21 17:39:11.000000 pyfamsa-0.3.0/include/famsa/core/sequence.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-21 17:39:11.000000 pyfamsa-0.3.0/include/famsa/core/version.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-07-21 17:39:11.000000 pyfamsa-0.3.0/include/famsa/msa.pxd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 17:39:19.042868 pyfamsa-0.3.0/include/famsa/tree/
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-21 17:39:11.000000 pyfamsa-0.3.0/include/famsa/tree/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-07-21 17:39:11.000000 pyfamsa-0.3.0/include/famsa/tree/abstract_tree_generator.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-21 17:39:11.000000 pyfamsa-0.3.0/include/famsa/tree/guide_tree.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-21 17:39:11.000000 pyfamsa-0.3.0/include/famsa/tree/newick_parser.pxd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 17:39:19.042868 pyfamsa-0.3.0/include/famsa/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 17:39:11.000000 pyfamsa-0.3.0/include/famsa/utils/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-21 17:39:11.000000 pyfamsa-0.3.0/include/famsa/utils/log.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-07-21 17:39:11.000000 pyfamsa-0.3.0/include/famsa/utils/memory_monotonic.pxd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 17:39:19.042868 pyfamsa-0.3.0/patches/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-21 17:39:11.000000 pyfamsa-0.3.0/patches/NewickParser.h.patch
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-07-21 17:39:11.000000 pyfamsa-0.3.0/patches/memory_monotonic.h.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-07-21 17:39:11.000000 pyfamsa-0.3.0/patches/msa.cpp.patch
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-21 17:39:11.000000 pyfamsa-0.3.0/patches/msa.h.patch
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-07-21 17:39:11.000000 pyfamsa-0.3.0/patches/sequence.cpp.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-07-21 17:39:11.000000 pyfamsa-0.3.0/patches/sequence.h.patch
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 17:39:19.042868 pyfamsa-0.3.0/pyfamsa/
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-07-21 17:39:11.000000 pyfamsa-0.3.0/pyfamsa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-07-21 17:39:11.000000 pyfamsa-0.3.0/pyfamsa/_famsa.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-07-21 17:39:11.000000 pyfamsa-0.3.0/pyfamsa/_famsa.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    18975 2023-07-21 17:39:11.000000 pyfamsa-0.3.0/pyfamsa/_famsa.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-21 17:39:11.000000 pyfamsa-0.3.0/pyfamsa/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 17:39:11.000000 pyfamsa-0.3.0/pyfamsa/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 17:39:19.042868 pyfamsa-0.3.0/pyfamsa/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-07-21 17:39:11.000000 pyfamsa-0.3.0/pyfamsa/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-21 17:39:11.000000 pyfamsa-0.3.0/pyfamsa/tests/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 17:39:19.050868 pyfamsa-0.3.0/pyfamsa/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 17:39:11.000000 pyfamsa-0.3.0/pyfamsa/tests/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47464 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/pyfamsa/tests/data/adeno_fiber.faa
+-rw-r--r--   0 runner    (1001) docker     (123)    68569 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/pyfamsa/tests/data/adeno_fiber.sl.afa
+-rw-r--r--   0 runner    (1001) docker     (123)     7333 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/pyfamsa/tests/data/adeno_fiber.sl.nwk
+-rw-r--r--   0 runner    (1001) docker     (123)    70021 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/pyfamsa/tests/data/adeno_fiber.upgma.afa
+-rw-r--r--   0 runner    (1001) docker     (123)     7333 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/pyfamsa/tests/data/adeno_fiber.upgma.nwk
+-rw-r--r--   0 runner    (1001) docker     (123)   287439 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/pyfamsa/tests/data/hemopexin.faa
+-rw-r--r--   0 runner    (1001) docker     (123)  2097465 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/pyfamsa/tests/data/hemopexin.medoid-nj.afa
+-rw-r--r--   0 runner    (1001) docker     (123)   129095 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/pyfamsa/tests/data/hemopexin.medoid-nj.nwk
+-rw-r--r--   0 runner    (1001) docker     (123)  1913193 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/pyfamsa/tests/data/hemopexin.medoid-sl.afa
+-rw-r--r--   0 runner    (1001) docker     (123)   129095 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/pyfamsa/tests/data/hemopexin.medoid-sl.nwk
+-rw-r--r--   0 runner    (1001) docker     (123)   129095 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/pyfamsa/tests/data/hemopexin.medoid-slink.nwk
+-rw-r--r--   0 runner    (1001) docker     (123)  2030457 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/pyfamsa/tests/data/hemopexin.medoid-upgma.afa
+-rw-r--r--   0 runner    (1001) docker     (123)   129095 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/pyfamsa/tests/data/hemopexin.medoid-upgma.nwk
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-07-21 17:39:11.000000 pyfamsa-0.3.0/pyfamsa/tests/fasta.py
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-21 17:39:11.000000 pyfamsa-0.3.0/pyfamsa/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-07-21 17:39:11.000000 pyfamsa-0.3.0/pyfamsa/tests/test_aligner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-07-21 17:39:11.000000 pyfamsa-0.3.0/pyfamsa/tests/test_doctest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-07-21 17:39:11.000000 pyfamsa-0.3.0/pyfamsa/tests/test_sequence.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 17:39:19.042868 pyfamsa-0.3.0/pyfamsa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10428 2023-07-21 17:39:18.000000 pyfamsa-0.3.0/pyfamsa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9734 2023-07-21 17:39:19.000000 pyfamsa-0.3.0/pyfamsa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 17:39:18.000000 pyfamsa-0.3.0/pyfamsa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 17:39:18.000000 pyfamsa-0.3.0/pyfamsa.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-21 17:39:18.000000 pyfamsa-0.3.0/pyfamsa.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-21 17:39:18.000000 pyfamsa-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-07-21 17:39:19.066868 pyfamsa-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)    36592 2023-07-21 17:39:11.000000 pyfamsa-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 17:39:19.034868 pyfamsa-0.3.0/vendor/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 17:39:19.050868 pyfamsa-0.3.0/vendor/FAMSA/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13518 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 17:39:19.038868 pyfamsa-0.3.0/vendor/FAMSA/libs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 17:39:19.050868 pyfamsa-0.3.0/vendor/FAMSA/libs/atomic_wait/
+-rw-r--r--   0 runner    (1001) docker     (123)    12610 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/libs/atomic_wait/atomic_wait
+-rw-r--r--   0 runner    (1001) docker     (123)     9777 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/libs/atomic_wait/barrier
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/libs/atomic_wait/latch
+-rw-r--r--   0 runner    (1001) docker     (123)    17651 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/libs/atomic_wait/semaphore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 17:39:19.054868 pyfamsa-0.3.0/vendor/FAMSA/libs/libdeflate/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/libs/libdeflate/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/libs/libdeflate/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)    13487 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/libs/libdeflate/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     9437 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/libs/libdeflate/NEWS.md
+-rw-r--r--   0 runner    (1001) docker     (123)    12146 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/libs/libdeflate/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 17:39:19.054868 pyfamsa-0.3.0/vendor/FAMSA/libs/libdeflate/common/
+-rw-r--r--   0 runner    (1001) docker     (123)     9618 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/libs/libdeflate/common/common_defs.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8596 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/libs/libdeflate/common/compiler_gcc.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/libs/libdeflate/common/compiler_msc.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 17:39:19.054868 pyfamsa-0.3.0/vendor/FAMSA/libs/libdeflate/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/libs/libdeflate/lib/adler32.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/libs/libdeflate/lib/adler32_vec_template.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 17:39:19.054868 pyfamsa-0.3.0/vendor/FAMSA/libs/libdeflate/lib/arm/
+-rw-r--r--   0 runner    (1001) docker     (123)     4527 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/libs/libdeflate/lib/arm/adler32_impl.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/libs/libdeflate/lib/arm/cpu_features.c
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/libs/libdeflate/lib/arm/cpu_features.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7595 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/libs/libdeflate/lib/arm/crc32_impl.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/libs/libdeflate/lib/arm/matchfinder_impl.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11537 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/libs/libdeflate/lib/bt_matchfinder.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/libs/libdeflate/lib/cpu_features_common.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10495 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/libs/libdeflate/lib/crc32.c
+-rw-r--r--   0 runner    (1001) docker     (123)    25448 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/libs/libdeflate/lib/crc32_table.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/libs/libdeflate/lib/crc32_vec_template.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12769 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/libs/libdeflate/lib/decompress_template.h
+-rw-r--r--   0 runner    (1001) docker     (123)   124274 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/libs/libdeflate/lib/deflate_compress.c
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/libs/libdeflate/lib/deflate_compress.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/libs/libdeflate/lib/deflate_constants.h
+-rw-r--r--   0 runner    (1001) docker     (123)    38953 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/libs/libdeflate/lib/deflate_decompress.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/libs/libdeflate/lib/gzip_compress.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/libs/libdeflate/lib/gzip_constants.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/libs/libdeflate/lib/gzip_decompress.c
+-rw-r--r--   0 runner    (1001) docker     (123)    14042 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/libs/libdeflate/lib/hc_matchfinder.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7207 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/libs/libdeflate/lib/ht_matchfinder.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/libs/libdeflate/lib/lib_common.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5124 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/libs/libdeflate/lib/matchfinder_common.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5645 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/libs/libdeflate/lib/unaligned.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/libs/libdeflate/lib/utils.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 17:39:19.058868 pyfamsa-0.3.0/vendor/FAMSA/libs/libdeflate/lib/x86/
+-rw-r--r--   0 runner    (1001) docker     (123)    12149 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/libs/libdeflate/lib/x86/adler32_impl.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4567 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/libs/libdeflate/lib/x86/cpu_features.c
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/libs/libdeflate/lib/x86/cpu_features.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/libs/libdeflate/lib/x86/crc32_impl.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10451 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/libs/libdeflate/lib/x86/crc32_pclmul_template.h
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/libs/libdeflate/lib/x86/decompress_impl.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/libs/libdeflate/lib/x86/matchfinder_impl.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/libs/libdeflate/lib/zlib_compress.c
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/libs/libdeflate/lib/zlib_constants.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/libs/libdeflate/lib/zlib_decompress.c
+-rw-r--r--   0 runner    (1001) docker     (123)    15154 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/libs/libdeflate/libdeflate.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 17:39:19.058868 pyfamsa-0.3.0/vendor/FAMSA/libs/libdeflate/programs/
+-rw-r--r--   0 runner    (1001) docker     (123)    17356 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/libs/libdeflate/programs/benchmark.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4605 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/libs/libdeflate/programs/checksum.c
+-rw-r--r--   0 runner    (1001) docker     (123)    17835 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/libs/libdeflate/programs/gzip.c
+-rw-r--r--   0 runner    (1001) docker     (123)    11580 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/libs/libdeflate/programs/prog_util.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4845 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/libs/libdeflate/programs/prog_util.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5012 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/libs/libdeflate/programs/test_checksums.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/libs/libdeflate/programs/test_custom_malloc.c
+-rw-r--r--   0 runner    (1001) docker     (123)    11890 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/libs/libdeflate/programs/test_incomplete_codes.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/libs/libdeflate/programs/test_litrunlen_overflow.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2686 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/libs/libdeflate/programs/test_overread.c
+-rw-r--r--   0 runner    (1001) docker     (123)    22742 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/libs/libdeflate/programs/test_slow_decompression.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5221 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/libs/libdeflate/programs/test_trailing_bytes.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5695 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/libs/libdeflate/programs/test_util.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/libs/libdeflate/programs/test_util.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/libs/libdeflate/programs/tgetopt.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 17:39:19.058868 pyfamsa-0.3.0/vendor/FAMSA/libs/libdeflate/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1512 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/libs/libdeflate/scripts/detect.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 17:39:19.058868 pyfamsa-0.3.0/vendor/FAMSA/libs/libdeflate/windows/
+-rw-r--r--   0 runner    (1001) docker     (123)    73752 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/libs/libdeflate/windows/libdeflatestatic.lib
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 17:39:19.062868 pyfamsa-0.3.0/vendor/FAMSA/libs/mimalloc/
+-rw-r--r--   0 runner    (1001) docker     (123)    12441 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/libs/mimalloc/alloc-aligned.c
+-rw-r--r--   0 runner    (1001) docker     (123)    13515 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/libs/mimalloc/alloc-override-osx.c
+-rw-r--r--   0 runner    (1001) docker     (123)    14876 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/libs/mimalloc/alloc-override.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6227 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/libs/mimalloc/alloc-posix.c
+-rw-r--r--   0 runner    (1001) docker     (123)    32874 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/libs/mimalloc/alloc.c
+-rw-r--r--   0 runner    (1001) docker     (123)    19573 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/libs/mimalloc/arena.c
+-rw-r--r--   0 runner    (1001) docker     (123)    16746 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/libs/mimalloc/bitmap.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5328 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/libs/mimalloc/bitmap.h
+-rw-r--r--   0 runner    (1001) docker     (123)    20115 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/libs/mimalloc/heap.c
+-rw-r--r--   0 runner    (1001) docker     (123)    25391 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/libs/mimalloc/init.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/libs/mimalloc/mimalloc-LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15171 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/libs/mimalloc/mimalloc-atomic.h
+-rw-r--r--   0 runner    (1001) docker     (123)    40784 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/libs/mimalloc/mimalloc-internal.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/libs/mimalloc/mimalloc-new-delete.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/libs/mimalloc/mimalloc-override.h
+-rw-r--r--   0 runner    (1001) docker     (123)    24060 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/libs/mimalloc/mimalloc-types.h
+-rw-r--r--   0 runner    (1001) docker     (123)    28550 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/libs/mimalloc/mimalloc.h
+-rw-r--r--   0 runner    (1001) docker     (123)    22798 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/libs/mimalloc/options.c
+-rw-r--r--   0 runner    (1001) docker     (123)    55869 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/libs/mimalloc/os.c
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/libs/mimalloc/override-new-delete.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11537 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/libs/mimalloc/page-queue.c
+-rw-r--r--   0 runner    (1001) docker     (123)    33440 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/libs/mimalloc/page.c
+-rw-r--r--   0 runner    (1001) docker     (123)    12823 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/libs/mimalloc/random.c
+-rw-r--r--   0 runner    (1001) docker     (123)    20963 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/libs/mimalloc/region.c
+-rw-r--r--   0 runner    (1001) docker     (123)    14137 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/libs/mimalloc/segment-cache.c
+-rw-r--r--   0 runner    (1001) docker     (123)    65602 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/libs/mimalloc/segment.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/libs/mimalloc/static.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    21607 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/libs/mimalloc/stats.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6925 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 17:39:19.062868 pyfamsa-0.3.0/vendor/FAMSA/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 17:39:19.062868 pyfamsa-0.3.0/vendor/FAMSA/src/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/src/core/defs.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3997 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/src/core/io_service.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/src/core/io_service.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9007 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/src/core/params.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3892 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/src/core/params.h
+-rw-r--r--   0 runner    (1001) docker     (123)    47408 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/src/core/profile.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    12974 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/src/core/profile.h
+-rw-r--r--   0 runner    (1001) docker     (123)    31900 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/src/core/profile_par.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    29543 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/src/core/profile_seq.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5395 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/src/core/queues.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11739 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/src/core/queues.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15198 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/src/core/sequence.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/src/core/sequence.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5184 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/src/core/version.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/src/famsa.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 17:39:19.062868 pyfamsa-0.3.0/vendor/FAMSA/src/lcs/
+-rw-r--r--   0 runner    (1001) docker     (123)     5692 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/src/lcs/lcsbp.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/src/lcs/lcsbp.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12467 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/src/lcs/lcsbp_avx2_intr.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    13463 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/src/lcs/lcsbp_avx2_intr.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9376 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/src/lcs/lcsbp_avx_intr.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10800 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/src/lcs/lcsbp_avx_intr.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8337 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/src/lcs/lcsbp_classic.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6561 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/src/lcs/lcsbp_classic.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9388 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/src/lcs/lcsbp_neon_intr.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10511 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/src/lcs/lcsbp_neon_intr.h
+-rw-r--r--   0 runner    (1001) docker     (123)    25404 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/src/msa.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/src/msa.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5908 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/src/msa_refinement.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 17:39:19.062868 pyfamsa-0.3.0/vendor/FAMSA/src/tree/
+-rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/src/tree/AbstractTreeGenerator.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/src/tree/AbstractTreeGenerator.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12021 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/src/tree/AbstractTreeGenerator.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/src/tree/Chained.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9457 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/src/tree/Clustering.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/src/tree/Clustering.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/src/tree/DistanceCalculator.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/src/tree/DistanceCalculator.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10325 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/src/tree/FastTree.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/src/tree/FastTree.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5665 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/src/tree/GuideTree.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/src/tree/GuideTree.h
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/src/tree/IPartialGenerator.h
+-rw-r--r--   0 runner    (1001) docker     (123)    23238 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/src/tree/MSTPrim.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5505 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/src/tree/MSTPrim.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/src/tree/NeighborJoining.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/src/tree/NeighborJoining.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3856 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/src/tree/NewickParser.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/src/tree/NewickParser.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7809 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/src/tree/SingleLinkage.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/src/tree/SingleLinkage.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/src/tree/SingleLinkageQueue.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/src/tree/TreeDefs.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8934 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/src/tree/UPGMA.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/src/tree/UPGMA.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 17:39:19.066868 pyfamsa-0.3.0/vendor/FAMSA/src/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     8706 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/src/utils/array.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3864 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/src/utils/conversion.h
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/src/utils/cpuid.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/src/utils/deterministic_random.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/src/utils/log.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/src/utils/log.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4581 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/src/utils/memory_monotonic.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/src/utils/meta_oper.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3725 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/src/utils/pooled_threads.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/src/utils/pooled_threads.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/src/utils/statistics.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/src/utils/timer.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/src/utils/timer.h
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/src/utils/utils.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/src/utils/utils.h
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/src/utils/utils_avx.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/src/utils/utils_avx2.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-21 17:39:12.000000 pyfamsa-0.3.0/vendor/FAMSA/src/utils/utils_neon.cpp
```

### Comparing `pyfamsa-0.2.0/CHANGELOG.md` & `pyfamsa-0.3.0/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,25 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
 and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).
 
 
 ## [Unreleased]
-[Unreleased]: https://github.com/althonos/pyfamsa/compare/v0.2.0...HEAD
+[Unreleased]: https://github.com/althonos/pyfamsa/compare/v0.3.0...HEAD
+
+
+## [v0.3.0] - 2023-07-21
+[v0.3.0]: https://github.com/althonos/pyfamsa/compare/v0.2.0...v0.3.0
+
+### Changed
+- Bumped Cython dependency to `v3.0`.
+
+### Fixed
+- PyPy builds failing on missing `PyInterpreterState_GetID`.
 
 
 ## [v0.2.0] - 2022-11-22
 [v0.2.0]: https://github.com/althonos/pyfamsa/compare/v0.1.1...v0.2.0
 
 ### Added
 - `pyfamsa.famsa_info` function to get version information about the embedded FAMSA version.
```

### Comparing `pyfamsa-0.2.0/CONTRIBUTING.md` & `pyfamsa-0.3.0/CONTRIBUTING.md`

 * *Files 10% similar despite different names*

```diff
@@ -22,22 +22,20 @@
 ```console
 $ python setup.py build_ext --debug --inplace
 $ python -m unittest discover -vv
 ```
 
 ## Coding guidelines
 
-This project targets Python 3.5 or later.
+This project targets Python 3.6 or later.
 
 Python objects should be typed; since it is not supported by Cython,
 you must manually declare types in type stubs (`.pyi` files). In Python
 files, you can add type annotations to function signatures (supported in
-Python 3.5) but not in variable assignments (supported only from Python
-3.6 onward). However, Cython allows you to use
-[f-strings](https://www.python.org/dev/peps/pep-0498/)
-even when compiling the code for Python 3.5.
+Python 3.5) and in variable assignments (supported from Python
+3.6 onward). 
 
 ### Interfacing with C/C++
 
 When interfacing with C or C++, and in particular with pointers, use
 assertions everywhere you assume the pointer to be non-NULL. Also consider
 using assertions when accessing raw C arrays, if applicable.
```

### Comparing `pyfamsa-0.2.0/COPYING` & `pyfamsa-0.3.0/COPYING`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/MANIFEST.in` & `pyfamsa-0.3.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/PKG-INFO` & `pyfamsa-0.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfamsa
-Version: 0.2.0
+Version: 0.3.0
 Summary: Cython bindings and Python interface to FAMSA, an algorithm for ultra-scale multiple sequence alignments.
 Home-page: https://github.com/althonos/pyfamsa
 Author: Martin Larralde
 Author-email: martin.larralde@embl.de
 License: GPLv3
 Project-URL: Documentation, https://pyfamsa.readthedocs.io/en/stable/
 Project-URL: Bug Tracker, https://github.com/althonos/pyfamsa/issues
@@ -17,27 +17,26 @@
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Cython
-Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Classifier: Typing :: Typed
-Requires-Python: >=3.5
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: COPYING
 
 # 🐍🧮 PyFAMSA [![Stars](https://img.shields.io/github/stars/althonos/pyfamsa.svg?style=social&maxAge=3600&label=Star)](https://github.com/althonos/pyfamsa/stargazers)
 
 *[Cython](https://cython.org/) bindings and Python interface to [FAMSA](https://github.com/refresh-bio/FAMSA), an algorithm for ultra-scale multiple sequence alignments.*
 
@@ -51,15 +50,16 @@
 [![Python Versions](https://img.shields.io/pypi/pyversions/pyfamsa.svg?style=flat-square&maxAge=600&logo=python)](https://pypi.org/project/pyfamsa/#files)
 [![Python Implementations](https://img.shields.io/pypi/implementation/pyfamsa.svg?style=flat-square&maxAge=600&label=impl)](https://pypi.org/project/pyfamsa/#files)
 [![Source](https://img.shields.io/badge/source-GitHub-303030.svg?maxAge=2678400&style=flat-square)](https://github.com/althonos/pyfamsa/)
 [![Mirror](https://img.shields.io/badge/mirror-EMBL-009f4d?style=flat-square&maxAge=2678400)](https://git.embl.de/larralde/pyfamsa/)
 [![Issues](https://img.shields.io/github/issues/althonos/pyfamsa.svg?style=flat-square&maxAge=600)](https://github.com/althonos/pyfamsa/issues)
 [![Docs](https://img.shields.io/readthedocs/pyfamsa/latest?style=flat-square&maxAge=600)](https://pyfamsa.readthedocs.io)
 [![Changelog](https://img.shields.io/badge/keep%20a-changelog-8A0707.svg?maxAge=2678400&style=flat-square)](https://github.com/althonos/pyfamsa/blob/main/CHANGELOG.md)
-[![Downloads](https://img.shields.io/badge/dynamic/json?style=flat-square&color=303f9f&maxAge=86400&label=downloads&query=%24.total_downloads&url=https%3A%2F%2Fapi.pepy.tech%2Fapi%2Fprojects%2Fpyfamsa)](https://pepy.tech/project/pyfamsa)
+[![Downloads](https://img.shields.io/pypi/dm/pyfamsa?style=flat-square&color=303f9f&maxAge=86400&label=downloads)](https://pepy.tech/project/pyfamsa)
+
 
 ***⚠️ This package is based on FAMSA 2.***
 
 ## 🗺️ Overview
 
 [FAMSA](https://github.com/refresh-bio/FAMSA) is a method published in
 2016 by Deorowicz *et al.* for large-scale multiple sequence alignments.
```

### Comparing `pyfamsa-0.2.0/README.md` & `pyfamsa-0.3.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,16 @@
 [![Python Versions](https://img.shields.io/pypi/pyversions/pyfamsa.svg?style=flat-square&maxAge=600&logo=python)](https://pypi.org/project/pyfamsa/#files)
 [![Python Implementations](https://img.shields.io/pypi/implementation/pyfamsa.svg?style=flat-square&maxAge=600&label=impl)](https://pypi.org/project/pyfamsa/#files)
 [![Source](https://img.shields.io/badge/source-GitHub-303030.svg?maxAge=2678400&style=flat-square)](https://github.com/althonos/pyfamsa/)
 [![Mirror](https://img.shields.io/badge/mirror-EMBL-009f4d?style=flat-square&maxAge=2678400)](https://git.embl.de/larralde/pyfamsa/)
 [![Issues](https://img.shields.io/github/issues/althonos/pyfamsa.svg?style=flat-square&maxAge=600)](https://github.com/althonos/pyfamsa/issues)
 [![Docs](https://img.shields.io/readthedocs/pyfamsa/latest?style=flat-square&maxAge=600)](https://pyfamsa.readthedocs.io)
 [![Changelog](https://img.shields.io/badge/keep%20a-changelog-8A0707.svg?maxAge=2678400&style=flat-square)](https://github.com/althonos/pyfamsa/blob/main/CHANGELOG.md)
-[![Downloads](https://img.shields.io/badge/dynamic/json?style=flat-square&color=303f9f&maxAge=86400&label=downloads&query=%24.total_downloads&url=https%3A%2F%2Fapi.pepy.tech%2Fapi%2Fprojects%2Fpyfamsa)](https://pepy.tech/project/pyfamsa)
+[![Downloads](https://img.shields.io/pypi/dm/pyfamsa?style=flat-square&color=303f9f&maxAge=86400&label=downloads)](https://pepy.tech/project/pyfamsa)
+
 
 ***⚠️ This package is based on FAMSA 2.***
 
 ## 🗺️ Overview
 
 [FAMSA](https://github.com/refresh-bio/FAMSA) is a method published in
 2016 by Deorowicz *et al.* for large-scale multiple sequence alignments.
```

### Comparing `pyfamsa-0.2.0/include/famsa/core/__init__.pxd` & `pyfamsa-0.3.0/include/famsa/core/__init__.pxd`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/include/famsa/core/io_service.pxd` & `pyfamsa-0.3.0/include/famsa/core/io_service.pxd`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/include/famsa/core/params.pxd` & `pyfamsa-0.3.0/include/famsa/core/params.pxd`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/include/famsa/core/sequence.pxd` & `pyfamsa-0.3.0/include/famsa/core/sequence.pxd`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/include/famsa/msa.pxd` & `pyfamsa-0.3.0/include/famsa/msa.pxd`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/include/famsa/tree/newick_parser.pxd` & `pyfamsa-0.3.0/include/famsa/tree/newick_parser.pxd`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/include/famsa/utils/memory_monotonic.pxd` & `pyfamsa-0.3.0/include/famsa/utils/memory_monotonic.pxd`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/patches/memory_monotonic.h.patch` & `pyfamsa-0.3.0/patches/memory_monotonic.h.patch`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/patches/sequence.cpp.patch` & `pyfamsa-0.3.0/patches/sequence.cpp.patch`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/patches/sequence.h.patch` & `pyfamsa-0.3.0/patches/sequence.h.patch`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/pyfamsa/_famsa.pxd` & `pyfamsa-0.3.0/pyfamsa/_famsa.pxd`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/pyfamsa/_famsa.pyi` & `pyfamsa-0.3.0/pyfamsa/_famsa.pyi`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/pyfamsa/_famsa.pyx` & `pyfamsa-0.3.0/pyfamsa/_famsa.pyx`

 * *Files 4% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 
 # --- Python imports ---------------------------------------------------------
 
 import datetime
 import collections
 import os
 
+include "_version.py"
 
 # --- Constants --------------------------------------------------------------
 
 cdef memory_monotonic_safe* MMA = new memory_monotonic_safe()
 
 cdef char SYMBOLS[25]
 for i, x in enumerate(b"ARNDCQEGHILKMFPSTWYVBZX*"):
@@ -85,14 +86,24 @@
         std::mt19937 mt(shuffle);
         std::shuffle(sequences.begin(), sequences.end(), mt);
     }
     """
     void sort_sequences(vector[CSequence*]& sequences)
     void shuffle_sequences(vector[CSequence*]& sequences, int shuffle)
 
+# --- PyPI patch --------------------------------------------------------------
+
+cdef extern from *:
+    """
+    #ifndef HAS_PYINTERPRETERSTATE_GETID
+    int64_t PyInterpreterState_GetID(PyInterpreterState *interp) {
+        return 0;
+    }
+    #endif
+    """
 
 # --- Classes ----------------------------------------------------------------
 
 cdef class Sequence:
     """A digitized sequence.
     """
```

### Comparing `pyfamsa-0.2.0/pyfamsa/tests/data/adeno_fiber.faa` & `pyfamsa-0.3.0/pyfamsa/tests/data/adeno_fiber.faa`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/pyfamsa/tests/data/adeno_fiber.sl.afa` & `pyfamsa-0.3.0/pyfamsa/tests/data/adeno_fiber.sl.afa`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/pyfamsa/tests/data/adeno_fiber.sl.nwk` & `pyfamsa-0.3.0/pyfamsa/tests/data/adeno_fiber.sl.nwk`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/pyfamsa/tests/data/adeno_fiber.upgma.afa` & `pyfamsa-0.3.0/pyfamsa/tests/data/adeno_fiber.upgma.afa`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/pyfamsa/tests/data/adeno_fiber.upgma.nwk` & `pyfamsa-0.3.0/pyfamsa/tests/data/adeno_fiber.upgma.nwk`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/pyfamsa/tests/data/hemopexin.faa` & `pyfamsa-0.3.0/pyfamsa/tests/data/hemopexin.faa`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/pyfamsa/tests/data/hemopexin.medoid-nj.afa` & `pyfamsa-0.3.0/pyfamsa/tests/data/hemopexin.medoid-nj.afa`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/pyfamsa/tests/data/hemopexin.medoid-nj.nwk` & `pyfamsa-0.3.0/pyfamsa/tests/data/hemopexin.medoid-nj.nwk`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/pyfamsa/tests/data/hemopexin.medoid-sl.afa` & `pyfamsa-0.3.0/pyfamsa/tests/data/hemopexin.medoid-sl.afa`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/pyfamsa/tests/data/hemopexin.medoid-sl.nwk` & `pyfamsa-0.3.0/pyfamsa/tests/data/hemopexin.medoid-sl.nwk`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/pyfamsa/tests/data/hemopexin.medoid-slink.nwk` & `pyfamsa-0.3.0/pyfamsa/tests/data/hemopexin.medoid-slink.nwk`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/pyfamsa/tests/data/hemopexin.medoid-upgma.afa` & `pyfamsa-0.3.0/pyfamsa/tests/data/hemopexin.medoid-upgma.afa`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/pyfamsa/tests/data/hemopexin.medoid-upgma.nwk` & `pyfamsa-0.3.0/pyfamsa/tests/data/hemopexin.medoid-upgma.nwk`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/pyfamsa/tests/fasta.py` & `pyfamsa-0.3.0/pyfamsa/tests/fasta.py`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/pyfamsa/tests/test_aligner.py` & `pyfamsa-0.3.0/pyfamsa/tests/test_aligner.py`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/pyfamsa/tests/test_doctest.py` & `pyfamsa-0.3.0/pyfamsa/tests/test_doctest.py`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/pyfamsa/tests/test_sequence.py` & `pyfamsa-0.3.0/pyfamsa/tests/test_sequence.py`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/pyfamsa.egg-info/PKG-INFO` & `pyfamsa-0.3.0/pyfamsa.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfamsa
-Version: 0.2.0
+Version: 0.3.0
 Summary: Cython bindings and Python interface to FAMSA, an algorithm for ultra-scale multiple sequence alignments.
 Home-page: https://github.com/althonos/pyfamsa
 Author: Martin Larralde
 Author-email: martin.larralde@embl.de
 License: GPLv3
 Project-URL: Documentation, https://pyfamsa.readthedocs.io/en/stable/
 Project-URL: Bug Tracker, https://github.com/althonos/pyfamsa/issues
@@ -17,27 +17,26 @@
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Cython
-Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Classifier: Typing :: Typed
-Requires-Python: >=3.5
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: COPYING
 
 # 🐍🧮 PyFAMSA [![Stars](https://img.shields.io/github/stars/althonos/pyfamsa.svg?style=social&maxAge=3600&label=Star)](https://github.com/althonos/pyfamsa/stargazers)
 
 *[Cython](https://cython.org/) bindings and Python interface to [FAMSA](https://github.com/refresh-bio/FAMSA), an algorithm for ultra-scale multiple sequence alignments.*
 
@@ -51,15 +50,16 @@
 [![Python Versions](https://img.shields.io/pypi/pyversions/pyfamsa.svg?style=flat-square&maxAge=600&logo=python)](https://pypi.org/project/pyfamsa/#files)
 [![Python Implementations](https://img.shields.io/pypi/implementation/pyfamsa.svg?style=flat-square&maxAge=600&label=impl)](https://pypi.org/project/pyfamsa/#files)
 [![Source](https://img.shields.io/badge/source-GitHub-303030.svg?maxAge=2678400&style=flat-square)](https://github.com/althonos/pyfamsa/)
 [![Mirror](https://img.shields.io/badge/mirror-EMBL-009f4d?style=flat-square&maxAge=2678400)](https://git.embl.de/larralde/pyfamsa/)
 [![Issues](https://img.shields.io/github/issues/althonos/pyfamsa.svg?style=flat-square&maxAge=600)](https://github.com/althonos/pyfamsa/issues)
 [![Docs](https://img.shields.io/readthedocs/pyfamsa/latest?style=flat-square&maxAge=600)](https://pyfamsa.readthedocs.io)
 [![Changelog](https://img.shields.io/badge/keep%20a-changelog-8A0707.svg?maxAge=2678400&style=flat-square)](https://github.com/althonos/pyfamsa/blob/main/CHANGELOG.md)
-[![Downloads](https://img.shields.io/badge/dynamic/json?style=flat-square&color=303f9f&maxAge=86400&label=downloads&query=%24.total_downloads&url=https%3A%2F%2Fapi.pepy.tech%2Fapi%2Fprojects%2Fpyfamsa)](https://pepy.tech/project/pyfamsa)
+[![Downloads](https://img.shields.io/pypi/dm/pyfamsa?style=flat-square&color=303f9f&maxAge=86400&label=downloads)](https://pepy.tech/project/pyfamsa)
+
 
 ***⚠️ This package is based on FAMSA 2.***
 
 ## 🗺️ Overview
 
 [FAMSA](https://github.com/refresh-bio/FAMSA) is a method published in
 2016 by Deorowicz *et al.* for large-scale multiple sequence alignments.
```

### Comparing `pyfamsa-0.2.0/pyfamsa.egg-info/SOURCES.txt` & `pyfamsa-0.3.0/pyfamsa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/setup.cfg` & `pyfamsa-0.3.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 	Development Status :: 3 - Alpha
 	Intended Audience :: Developers
 	Intended Audience :: Science/Research
 	License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 	Operating System :: OS Independent
 	Programming Language :: C
 	Programming Language :: Cython
-	Programming Language :: Python :: 3.5
 	Programming Language :: Python :: 3.6
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 	Programming Language :: Python :: Implementation :: CPython
@@ -38,18 +37,18 @@
 	Builds = https://github.com/althonos/pyfamsa/actions
 	PyPI = https://pypi.org/project/pyfamsa
 
 [options]
 zip_safe = false
 packages = pyfamsa, pyfamsa.tests, pyfamsa.tests.data
 include_package_data = false
-python_requires = >=3.5
+python_requires = >=3.6
 setup_requires = 
 	setuptools >=46.4
-	cython ~=0.29.16
+	cython ~=3.0
 	semantic-version ~=2.10
 tests_require = 
 	importlib-resources ; python_version < '3.7'
 
 [options.package_data]
 pyfamsa = py.typed, *.pyi
 pyfamsa.tests = requirements.txt
@@ -89,19 +88,19 @@
 warn_return_any = true
 exclude = pyfamsa/tests/*
 
 [mypy-pyfamsa.tests]
 disallow_untyped_defs = false
 
 [isort]
-known_first_party = pyfamsa, trimal
+known_first_party = pyfamsa, famsa
 known_standard_library = cpython, cython, _unicode
 known_third_party = libc, libcpp
 line_length = 88
 profile = black
 skip_gitignore = true
-skip_glob = vendor/trimal/*
+skip_glob = vendor/FAMSA/*
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `pyfamsa-0.2.0/setup.py` & `pyfamsa-0.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -268,14 +268,55 @@
         self._clib_cmd.disable_avx2 = self.disable_avx2
         self._clib_cmd.disable_neon = self.disable_neon
         self._clib_cmd.plat_name = self.plat_name
         self._clib_cmd.target_machine = self.target_machine
         self._clib_cmd.target_system = self.target_system
         self._clib_cmd.target_cpu = self.target_cpu
 
+    # --- Autotools-like helpers ---
+
+    def _check_getid(self):
+        _eprint('checking whether `PyInterpreterState_GetID` is available')
+
+        base = "have_getid"
+        testfile = os.path.join(self.build_temp, "{}.c".format(base))
+        objects = []
+
+        self.mkpath(self.build_temp)
+        with open(testfile, "w") as f:
+            f.write("""
+            #include <stdint.h>
+            #include <stdlib.h>
+            #include <Python.h>
+
+            int main(int argc, char *argv[]) {{
+                PyInterpreterState_GetID(NULL);
+                return 0;
+            }}
+            """)
+
+        if self.compiler.compiler_type == "msvc":
+            flags = ["/WX"]
+        else:
+            flags = ["-Werror=implicit-function-declaration"]
+
+        try:
+            self.mkpath(self.build_temp)
+            objects = self.compiler.compile([testfile], extra_postargs=flags)
+        except CompileError:
+            _eprint("no")
+            return False
+        else:
+            _eprint("yes")
+            return True
+        finally:
+            os.remove(testfile)
+            for obj in filter(os.path.isfile, objects):
+                os.remove(obj)
+
     # --- Build code ---
 
     def build_extension(self, ext):
         # show the compiler being used
         _eprint("building", ext.name, "with", self.compiler.compiler_type, "compiler")
 
         # add debug symbols if we are building in debug mode
@@ -301,14 +342,18 @@
                     lib.name, output_dir=self._clib_cmd.build_clib
                 )
                 ext.depends.append(libfile)
                 ext.extra_objects.append(libfile)
                 ext.extra_objects.extend(lib.extra_objects)
                 ext.define_macros.extend(lib.define_macros)
 
+        # make sure `PyInterpreterState_GetID` is available
+        if self._check_getid():
+            ext.define_macros.append(("HAS_PYINTERPRETERSTATE_GETID", 1))
+
         # build the rest of the extension as normal
         ext._needs_stub = False
         _build_ext.build_extension(self, ext)
 
     def build_extensions(self):
         # check `cythonize` is available
         if isinstance(cythonize, ImportError):
```

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/LICENSE` & `pyfamsa-0.3.0/vendor/FAMSA/LICENSE`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/README.md` & `pyfamsa-0.3.0/vendor/FAMSA/README.md`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/libs/atomic_wait/atomic_wait` & `pyfamsa-0.3.0/vendor/FAMSA/libs/atomic_wait/atomic_wait`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/libs/atomic_wait/barrier` & `pyfamsa-0.3.0/vendor/FAMSA/libs/atomic_wait/barrier`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/libs/atomic_wait/latch` & `pyfamsa-0.3.0/vendor/FAMSA/libs/atomic_wait/latch`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/libs/atomic_wait/semaphore` & `pyfamsa-0.3.0/vendor/FAMSA/libs/atomic_wait/semaphore`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/libs/libdeflate/COPYING` & `pyfamsa-0.3.0/vendor/FAMSA/libs/libdeflate/COPYING`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/libs/libdeflate/Makefile` & `pyfamsa-0.3.0/vendor/FAMSA/libs/libdeflate/Makefile`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/libs/libdeflate/NEWS.md` & `pyfamsa-0.3.0/vendor/FAMSA/libs/libdeflate/NEWS.md`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/libs/libdeflate/README.md` & `pyfamsa-0.3.0/vendor/FAMSA/libs/libdeflate/README.md`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/libs/libdeflate/common/common_defs.h` & `pyfamsa-0.3.0/vendor/FAMSA/libs/libdeflate/common/common_defs.h`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/libs/libdeflate/common/compiler_gcc.h` & `pyfamsa-0.3.0/vendor/FAMSA/libs/libdeflate/common/compiler_gcc.h`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/libs/libdeflate/common/compiler_msc.h` & `pyfamsa-0.3.0/vendor/FAMSA/libs/libdeflate/common/compiler_msc.h`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/libs/libdeflate/lib/adler32.c` & `pyfamsa-0.3.0/vendor/FAMSA/libs/libdeflate/lib/adler32.c`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/libs/libdeflate/lib/adler32_vec_template.h` & `pyfamsa-0.3.0/vendor/FAMSA/libs/libdeflate/lib/adler32_vec_template.h`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/libs/libdeflate/lib/arm/adler32_impl.h` & `pyfamsa-0.3.0/vendor/FAMSA/libs/libdeflate/lib/arm/adler32_impl.h`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/libs/libdeflate/lib/arm/cpu_features.c` & `pyfamsa-0.3.0/vendor/FAMSA/libs/libdeflate/lib/arm/cpu_features.c`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/libs/libdeflate/lib/arm/cpu_features.h` & `pyfamsa-0.3.0/vendor/FAMSA/libs/libdeflate/lib/arm/cpu_features.h`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/libs/libdeflate/lib/arm/crc32_impl.h` & `pyfamsa-0.3.0/vendor/FAMSA/libs/libdeflate/lib/arm/crc32_impl.h`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/libs/libdeflate/lib/arm/matchfinder_impl.h` & `pyfamsa-0.3.0/vendor/FAMSA/libs/libdeflate/lib/arm/matchfinder_impl.h`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/libs/libdeflate/lib/bt_matchfinder.h` & `pyfamsa-0.3.0/vendor/FAMSA/libs/libdeflate/lib/bt_matchfinder.h`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/libs/libdeflate/lib/cpu_features_common.h` & `pyfamsa-0.3.0/vendor/FAMSA/libs/libdeflate/lib/cpu_features_common.h`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/libs/libdeflate/lib/crc32.c` & `pyfamsa-0.3.0/vendor/FAMSA/libs/libdeflate/lib/crc32.c`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/libs/libdeflate/lib/crc32_table.h` & `pyfamsa-0.3.0/vendor/FAMSA/libs/libdeflate/lib/crc32_table.h`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/libs/libdeflate/lib/crc32_vec_template.h` & `pyfamsa-0.3.0/vendor/FAMSA/libs/libdeflate/lib/crc32_vec_template.h`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/libs/libdeflate/lib/decompress_template.h` & `pyfamsa-0.3.0/vendor/FAMSA/libs/libdeflate/lib/decompress_template.h`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/libs/libdeflate/lib/deflate_compress.c` & `pyfamsa-0.3.0/vendor/FAMSA/libs/libdeflate/lib/deflate_compress.c`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/libs/libdeflate/lib/deflate_constants.h` & `pyfamsa-0.3.0/vendor/FAMSA/libs/libdeflate/lib/deflate_constants.h`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/libs/libdeflate/lib/deflate_decompress.c` & `pyfamsa-0.3.0/vendor/FAMSA/libs/libdeflate/lib/deflate_decompress.c`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/libs/libdeflate/lib/gzip_compress.c` & `pyfamsa-0.3.0/vendor/FAMSA/libs/libdeflate/lib/gzip_compress.c`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/libs/libdeflate/lib/gzip_constants.h` & `pyfamsa-0.3.0/vendor/FAMSA/libs/libdeflate/lib/gzip_constants.h`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/libs/libdeflate/lib/gzip_decompress.c` & `pyfamsa-0.3.0/vendor/FAMSA/libs/libdeflate/lib/gzip_decompress.c`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/libs/libdeflate/lib/hc_matchfinder.h` & `pyfamsa-0.3.0/vendor/FAMSA/libs/libdeflate/lib/hc_matchfinder.h`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/libs/libdeflate/lib/ht_matchfinder.h` & `pyfamsa-0.3.0/vendor/FAMSA/libs/libdeflate/lib/ht_matchfinder.h`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/libs/libdeflate/lib/lib_common.h` & `pyfamsa-0.3.0/vendor/FAMSA/libs/libdeflate/lib/lib_common.h`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/libs/libdeflate/lib/matchfinder_common.h` & `pyfamsa-0.3.0/vendor/FAMSA/libs/libdeflate/lib/matchfinder_common.h`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/libs/libdeflate/lib/unaligned.h` & `pyfamsa-0.3.0/vendor/FAMSA/libs/libdeflate/lib/unaligned.h`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/libs/libdeflate/lib/utils.c` & `pyfamsa-0.3.0/vendor/FAMSA/libs/libdeflate/lib/utils.c`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/libs/libdeflate/lib/x86/adler32_impl.h` & `pyfamsa-0.3.0/vendor/FAMSA/libs/libdeflate/lib/x86/adler32_impl.h`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/libs/libdeflate/lib/x86/cpu_features.c` & `pyfamsa-0.3.0/vendor/FAMSA/libs/libdeflate/lib/x86/cpu_features.c`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/libs/libdeflate/lib/x86/cpu_features.h` & `pyfamsa-0.3.0/vendor/FAMSA/libs/libdeflate/lib/x86/cpu_features.h`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/libs/libdeflate/lib/x86/crc32_impl.h` & `pyfamsa-0.3.0/vendor/FAMSA/libs/libdeflate/lib/x86/crc32_impl.h`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/libs/libdeflate/lib/x86/crc32_pclmul_template.h` & `pyfamsa-0.3.0/vendor/FAMSA/libs/libdeflate/lib/x86/crc32_pclmul_template.h`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/libs/libdeflate/lib/x86/decompress_impl.h` & `pyfamsa-0.3.0/vendor/FAMSA/libs/libdeflate/lib/x86/decompress_impl.h`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/libs/libdeflate/lib/x86/matchfinder_impl.h` & `pyfamsa-0.3.0/vendor/FAMSA/libs/libdeflate/lib/x86/matchfinder_impl.h`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/libs/libdeflate/lib/zlib_compress.c` & `pyfamsa-0.3.0/vendor/FAMSA/libs/libdeflate/lib/zlib_compress.c`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/libs/libdeflate/lib/zlib_decompress.c` & `pyfamsa-0.3.0/vendor/FAMSA/libs/libdeflate/lib/zlib_decompress.c`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/libs/libdeflate/libdeflate.h` & `pyfamsa-0.3.0/vendor/FAMSA/libs/libdeflate/libdeflate.h`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/libs/libdeflate/programs/benchmark.c` & `pyfamsa-0.3.0/vendor/FAMSA/libs/libdeflate/programs/benchmark.c`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/libs/libdeflate/programs/checksum.c` & `pyfamsa-0.3.0/vendor/FAMSA/libs/libdeflate/programs/checksum.c`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/libs/libdeflate/programs/gzip.c` & `pyfamsa-0.3.0/vendor/FAMSA/libs/libdeflate/programs/gzip.c`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/libs/libdeflate/programs/prog_util.c` & `pyfamsa-0.3.0/vendor/FAMSA/libs/libdeflate/programs/prog_util.c`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/libs/libdeflate/programs/prog_util.h` & `pyfamsa-0.3.0/vendor/FAMSA/libs/libdeflate/programs/prog_util.h`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/libs/libdeflate/programs/test_checksums.c` & `pyfamsa-0.3.0/vendor/FAMSA/libs/libdeflate/programs/test_checksums.c`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/libs/libdeflate/programs/test_custom_malloc.c` & `pyfamsa-0.3.0/vendor/FAMSA/libs/libdeflate/programs/test_custom_malloc.c`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/libs/libdeflate/programs/test_incomplete_codes.c` & `pyfamsa-0.3.0/vendor/FAMSA/libs/libdeflate/programs/test_incomplete_codes.c`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/libs/libdeflate/programs/test_litrunlen_overflow.c` & `pyfamsa-0.3.0/vendor/FAMSA/libs/libdeflate/programs/test_litrunlen_overflow.c`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/libs/libdeflate/programs/test_overread.c` & `pyfamsa-0.3.0/vendor/FAMSA/libs/libdeflate/programs/test_overread.c`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/libs/libdeflate/programs/test_slow_decompression.c` & `pyfamsa-0.3.0/vendor/FAMSA/libs/libdeflate/programs/test_slow_decompression.c`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/libs/libdeflate/programs/test_trailing_bytes.c` & `pyfamsa-0.3.0/vendor/FAMSA/libs/libdeflate/programs/test_trailing_bytes.c`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/libs/libdeflate/programs/test_util.c` & `pyfamsa-0.3.0/vendor/FAMSA/libs/libdeflate/programs/test_util.c`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/libs/libdeflate/programs/test_util.h` & `pyfamsa-0.3.0/vendor/FAMSA/libs/libdeflate/programs/test_util.h`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/libs/libdeflate/programs/tgetopt.c` & `pyfamsa-0.3.0/vendor/FAMSA/libs/libdeflate/programs/tgetopt.c`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/libs/libdeflate/scripts/detect.sh` & `pyfamsa-0.3.0/vendor/FAMSA/libs/libdeflate/scripts/detect.sh`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/libs/libdeflate/windows/libdeflatestatic.lib` & `pyfamsa-0.3.0/vendor/FAMSA/libs/libdeflate/windows/libdeflatestatic.lib`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/libs/mimalloc/alloc-aligned.c` & `pyfamsa-0.3.0/vendor/FAMSA/libs/mimalloc/alloc-aligned.c`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/libs/mimalloc/alloc-override-osx.c` & `pyfamsa-0.3.0/vendor/FAMSA/libs/mimalloc/alloc-override-osx.c`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/libs/mimalloc/alloc-override.c` & `pyfamsa-0.3.0/vendor/FAMSA/libs/mimalloc/alloc-override.c`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/libs/mimalloc/alloc-posix.c` & `pyfamsa-0.3.0/vendor/FAMSA/libs/mimalloc/alloc-posix.c`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/libs/mimalloc/alloc.c` & `pyfamsa-0.3.0/vendor/FAMSA/libs/mimalloc/alloc.c`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/libs/mimalloc/arena.c` & `pyfamsa-0.3.0/vendor/FAMSA/libs/mimalloc/arena.c`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/libs/mimalloc/bitmap.c` & `pyfamsa-0.3.0/vendor/FAMSA/libs/mimalloc/bitmap.c`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/libs/mimalloc/bitmap.h` & `pyfamsa-0.3.0/vendor/FAMSA/libs/mimalloc/bitmap.h`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/libs/mimalloc/heap.c` & `pyfamsa-0.3.0/vendor/FAMSA/libs/mimalloc/heap.c`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/libs/mimalloc/init.c` & `pyfamsa-0.3.0/vendor/FAMSA/libs/mimalloc/init.c`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/libs/mimalloc/mimalloc-LICENSE` & `pyfamsa-0.3.0/vendor/FAMSA/libs/mimalloc/mimalloc-LICENSE`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/libs/mimalloc/mimalloc-atomic.h` & `pyfamsa-0.3.0/vendor/FAMSA/libs/mimalloc/mimalloc-atomic.h`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/libs/mimalloc/mimalloc-internal.h` & `pyfamsa-0.3.0/vendor/FAMSA/libs/mimalloc/mimalloc-internal.h`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/libs/mimalloc/mimalloc-new-delete.h` & `pyfamsa-0.3.0/vendor/FAMSA/libs/mimalloc/mimalloc-new-delete.h`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/libs/mimalloc/mimalloc-override.h` & `pyfamsa-0.3.0/vendor/FAMSA/libs/mimalloc/mimalloc-override.h`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/libs/mimalloc/mimalloc-types.h` & `pyfamsa-0.3.0/vendor/FAMSA/libs/mimalloc/mimalloc-types.h`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/libs/mimalloc/mimalloc.h` & `pyfamsa-0.3.0/vendor/FAMSA/libs/mimalloc/mimalloc.h`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/libs/mimalloc/options.c` & `pyfamsa-0.3.0/vendor/FAMSA/libs/mimalloc/options.c`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/libs/mimalloc/os.c` & `pyfamsa-0.3.0/vendor/FAMSA/libs/mimalloc/os.c`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/libs/mimalloc/override-new-delete.cpp` & `pyfamsa-0.3.0/vendor/FAMSA/libs/mimalloc/override-new-delete.cpp`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/libs/mimalloc/page-queue.c` & `pyfamsa-0.3.0/vendor/FAMSA/libs/mimalloc/page-queue.c`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/libs/mimalloc/page.c` & `pyfamsa-0.3.0/vendor/FAMSA/libs/mimalloc/page.c`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/libs/mimalloc/random.c` & `pyfamsa-0.3.0/vendor/FAMSA/libs/mimalloc/random.c`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/libs/mimalloc/region.c` & `pyfamsa-0.3.0/vendor/FAMSA/libs/mimalloc/region.c`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/libs/mimalloc/segment-cache.c` & `pyfamsa-0.3.0/vendor/FAMSA/libs/mimalloc/segment-cache.c`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/libs/mimalloc/segment.c` & `pyfamsa-0.3.0/vendor/FAMSA/libs/mimalloc/segment.c`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/libs/mimalloc/static.cpp` & `pyfamsa-0.3.0/vendor/FAMSA/libs/mimalloc/static.cpp`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/libs/mimalloc/stats.c` & `pyfamsa-0.3.0/vendor/FAMSA/libs/mimalloc/stats.c`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/makefile` & `pyfamsa-0.3.0/vendor/FAMSA/makefile`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/src/core/defs.h` & `pyfamsa-0.3.0/vendor/FAMSA/src/core/defs.h`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/src/core/io_service.cpp` & `pyfamsa-0.3.0/vendor/FAMSA/src/core/io_service.cpp`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/src/core/io_service.h` & `pyfamsa-0.3.0/vendor/FAMSA/src/core/io_service.h`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/src/core/params.cpp` & `pyfamsa-0.3.0/vendor/FAMSA/src/core/params.cpp`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/src/core/params.h` & `pyfamsa-0.3.0/vendor/FAMSA/src/core/params.h`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/src/core/profile.cpp` & `pyfamsa-0.3.0/vendor/FAMSA/src/core/profile.cpp`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/src/core/profile.h` & `pyfamsa-0.3.0/vendor/FAMSA/src/core/profile.h`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/src/core/profile_par.cpp` & `pyfamsa-0.3.0/vendor/FAMSA/src/core/profile_par.cpp`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/src/core/profile_seq.cpp` & `pyfamsa-0.3.0/vendor/FAMSA/src/core/profile_seq.cpp`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/src/core/queues.cpp` & `pyfamsa-0.3.0/vendor/FAMSA/src/core/queues.cpp`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/src/core/queues.h` & `pyfamsa-0.3.0/vendor/FAMSA/src/core/queues.h`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/src/core/sequence.cpp` & `pyfamsa-0.3.0/vendor/FAMSA/src/core/sequence.cpp`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/src/core/sequence.h` & `pyfamsa-0.3.0/vendor/FAMSA/src/core/sequence.h`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/src/core/version.h` & `pyfamsa-0.3.0/vendor/FAMSA/src/core/version.h`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/src/famsa.cpp` & `pyfamsa-0.3.0/vendor/FAMSA/src/famsa.cpp`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/src/lcs/lcsbp.cpp` & `pyfamsa-0.3.0/vendor/FAMSA/src/lcs/lcsbp.cpp`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/src/lcs/lcsbp.h` & `pyfamsa-0.3.0/vendor/FAMSA/src/lcs/lcsbp.h`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/src/lcs/lcsbp_avx2_intr.cpp` & `pyfamsa-0.3.0/vendor/FAMSA/src/lcs/lcsbp_avx2_intr.cpp`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/src/lcs/lcsbp_avx2_intr.h` & `pyfamsa-0.3.0/vendor/FAMSA/src/lcs/lcsbp_avx2_intr.h`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/src/lcs/lcsbp_avx_intr.cpp` & `pyfamsa-0.3.0/vendor/FAMSA/src/lcs/lcsbp_avx_intr.cpp`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/src/lcs/lcsbp_avx_intr.h` & `pyfamsa-0.3.0/vendor/FAMSA/src/lcs/lcsbp_avx_intr.h`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/src/lcs/lcsbp_classic.cpp` & `pyfamsa-0.3.0/vendor/FAMSA/src/lcs/lcsbp_classic.cpp`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/src/lcs/lcsbp_classic.h` & `pyfamsa-0.3.0/vendor/FAMSA/src/lcs/lcsbp_classic.h`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/src/lcs/lcsbp_neon_intr.cpp` & `pyfamsa-0.3.0/vendor/FAMSA/src/lcs/lcsbp_neon_intr.cpp`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/src/lcs/lcsbp_neon_intr.h` & `pyfamsa-0.3.0/vendor/FAMSA/src/lcs/lcsbp_neon_intr.h`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/src/msa.cpp` & `pyfamsa-0.3.0/vendor/FAMSA/src/msa.cpp`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/src/msa.h` & `pyfamsa-0.3.0/vendor/FAMSA/src/msa.h`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/src/msa_refinement.cpp` & `pyfamsa-0.3.0/vendor/FAMSA/src/msa_refinement.cpp`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/src/tree/AbstractTreeGenerator.cpp` & `pyfamsa-0.3.0/vendor/FAMSA/src/tree/AbstractTreeGenerator.cpp`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/src/tree/AbstractTreeGenerator.h` & `pyfamsa-0.3.0/vendor/FAMSA/src/tree/AbstractTreeGenerator.h`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/src/tree/AbstractTreeGenerator.hpp` & `pyfamsa-0.3.0/vendor/FAMSA/src/tree/AbstractTreeGenerator.hpp`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/src/tree/Chained.h` & `pyfamsa-0.3.0/vendor/FAMSA/src/tree/Chained.h`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/src/tree/Clustering.cpp` & `pyfamsa-0.3.0/vendor/FAMSA/src/tree/Clustering.cpp`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/src/tree/Clustering.h` & `pyfamsa-0.3.0/vendor/FAMSA/src/tree/Clustering.h`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/src/tree/DistanceCalculator.cpp` & `pyfamsa-0.3.0/vendor/FAMSA/src/tree/DistanceCalculator.cpp`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/src/tree/DistanceCalculator.h` & `pyfamsa-0.3.0/vendor/FAMSA/src/tree/DistanceCalculator.h`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/src/tree/FastTree.cpp` & `pyfamsa-0.3.0/vendor/FAMSA/src/tree/FastTree.cpp`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/src/tree/FastTree.h` & `pyfamsa-0.3.0/vendor/FAMSA/src/tree/FastTree.h`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/src/tree/GuideTree.cpp` & `pyfamsa-0.3.0/vendor/FAMSA/src/tree/GuideTree.cpp`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/src/tree/GuideTree.h` & `pyfamsa-0.3.0/vendor/FAMSA/src/tree/GuideTree.h`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/src/tree/MSTPrim.cpp` & `pyfamsa-0.3.0/vendor/FAMSA/src/tree/MSTPrim.cpp`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/src/tree/MSTPrim.h` & `pyfamsa-0.3.0/vendor/FAMSA/src/tree/MSTPrim.h`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/src/tree/NeighborJoining.cpp` & `pyfamsa-0.3.0/vendor/FAMSA/src/tree/NeighborJoining.cpp`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/src/tree/NeighborJoining.h` & `pyfamsa-0.3.0/vendor/FAMSA/src/tree/NeighborJoining.h`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/src/tree/NewickParser.cpp` & `pyfamsa-0.3.0/vendor/FAMSA/src/tree/NewickParser.cpp`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/src/tree/NewickParser.h` & `pyfamsa-0.3.0/vendor/FAMSA/src/tree/NewickParser.h`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/src/tree/SingleLinkage.cpp` & `pyfamsa-0.3.0/vendor/FAMSA/src/tree/SingleLinkage.cpp`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/src/tree/SingleLinkage.h` & `pyfamsa-0.3.0/vendor/FAMSA/src/tree/SingleLinkage.h`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/src/tree/SingleLinkageQueue.h` & `pyfamsa-0.3.0/vendor/FAMSA/src/tree/SingleLinkageQueue.h`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/src/tree/TreeDefs.h` & `pyfamsa-0.3.0/vendor/FAMSA/src/tree/TreeDefs.h`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/src/tree/UPGMA.cpp` & `pyfamsa-0.3.0/vendor/FAMSA/src/tree/UPGMA.cpp`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/src/tree/UPGMA.h` & `pyfamsa-0.3.0/vendor/FAMSA/src/tree/UPGMA.h`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/src/utils/array.h` & `pyfamsa-0.3.0/vendor/FAMSA/src/utils/array.h`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/src/utils/conversion.h` & `pyfamsa-0.3.0/vendor/FAMSA/src/utils/conversion.h`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/src/utils/cpuid.h` & `pyfamsa-0.3.0/vendor/FAMSA/src/utils/cpuid.h`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/src/utils/deterministic_random.h` & `pyfamsa-0.3.0/vendor/FAMSA/src/utils/deterministic_random.h`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/src/utils/log.cpp` & `pyfamsa-0.3.0/vendor/FAMSA/src/utils/log.cpp`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/src/utils/log.h` & `pyfamsa-0.3.0/vendor/FAMSA/src/utils/log.h`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/src/utils/memory_monotonic.h` & `pyfamsa-0.3.0/vendor/FAMSA/src/utils/memory_monotonic.h`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/src/utils/meta_oper.h` & `pyfamsa-0.3.0/vendor/FAMSA/src/utils/meta_oper.h`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/src/utils/pooled_threads.cpp` & `pyfamsa-0.3.0/vendor/FAMSA/src/utils/pooled_threads.cpp`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/src/utils/pooled_threads.h` & `pyfamsa-0.3.0/vendor/FAMSA/src/utils/pooled_threads.h`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/src/utils/statistics.h` & `pyfamsa-0.3.0/vendor/FAMSA/src/utils/statistics.h`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/src/utils/timer.cpp` & `pyfamsa-0.3.0/vendor/FAMSA/src/utils/timer.cpp`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/src/utils/timer.h` & `pyfamsa-0.3.0/vendor/FAMSA/src/utils/timer.h`

 * *Files identical despite different names*

### Comparing `pyfamsa-0.2.0/vendor/FAMSA/src/utils/utils.h` & `pyfamsa-0.3.0/vendor/FAMSA/src/utils/utils.h`

 * *Files identical despite different names*

