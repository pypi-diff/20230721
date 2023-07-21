# Comparing `tmp/isal-1.1.0.tar.gz` & `tmp/isal-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "isal-1.1.0.tar", last modified: Wed Oct 12 13:32:58 2022, max compression
+gzip compressed data, was "isal-1.2.0.tar", last modified: Fri Jul 21 12:29:00 2023, max compression
```

## Comparing `isal-1.1.0.tar` & `isal-1.2.0.tar`

### file list

```diff
@@ -1,432 +1,438 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-12 13:32:58.059377 isal-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (121)     2484 2022-10-12 13:21:37.000000 isal-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       42 2022-10-12 13:21:37.000000 isal-1.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     8609 2022-10-12 13:32:58.059377 isal-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     7292 2022-10-12 13:21:37.000000 isal-1.1.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-10-12 13:21:37.000000 isal-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       73 2022-10-12 13:32:58.059377 isal-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     9217 2022-10-12 13:21:37.000000 isal-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-12 13:32:58.007377 isal-1.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-12 13:32:58.011376 isal-1.1.0/src/isal/
--rw-r--r--   0 runner    (1001) docker     (121)      909 2022-10-12 13:21:37.000000 isal-1.1.0/src/isal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      405 2022-10-12 13:21:37.000000 isal-1.1.0/src/isal/_isal.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1284 2022-10-12 13:21:37.000000 isal-1.1.0/src/isal/_isalmodule.c
--rw-r--r--   0 runner    (1001) docker     (121)    22284 2022-10-12 13:21:37.000000 isal-1.1.0/src/isal/igzip.py
--rw-r--r--   0 runner    (1001) docker     (121)     1623 2022-10-12 13:21:37.000000 isal-1.1.0/src/isal/igzip_lib.pyi
--rw-r--r--   0 runner    (1001) docker     (121)    22656 2022-10-12 13:21:37.000000 isal-1.1.0/src/isal/igzip_libmodule.c
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-12 13:32:58.015377 isal-1.1.0/src/isal/isa-l/
--rw-r--r--   0 runner    (1001) docker     (121)       45 2022-10-12 13:21:37.000000 isal-1.1.0/src/isal/isa-l/.git
--rw-r--r--   0 runner    (1001) docker     (121)      233 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     2486 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/.travis.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1378 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (121)     1188 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/Doxyfile
--rw-r--r--   0 runner    (1001) docker     (121)     1559 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     4497 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/Makefile.am
--rw-r--r--   0 runner    (1001) docker     (121)    10136 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/Makefile.nmake
--rw-r--r--   0 runner    (1001) docker     (121)     2313 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/Makefile.unx
--rw-r--r--   0 runner    (1001) docker     (121)     2570 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     9439 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/Release_notes.txt
--rwxr-xr-x   0 runner    (1001) docker     (121)      429 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/autogen.sh
--rw-r--r--   0 runner    (1001) docker     (121)     8871 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/configure.ac
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-12 13:32:58.019377 isal-1.1.0/src/isal/isa-l/crc/
--rw-r--r--   0 runner    (1001) docker     (121)     3434 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/crc/Makefile.am
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-12 13:32:58.023377 isal-1.1.0/src/isal/isa-l/crc/aarch64/
--rw-r--r--   0 runner    (1001) docker     (121)     2628 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/crc/aarch64/Makefile.am
--rw-r--r--   0 runner    (1001) docker     (121)    11478 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/crc/aarch64/crc16_t10dif_copy_pmull.S
--rw-r--r--   0 runner    (1001) docker     (121)    11068 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/crc/aarch64/crc16_t10dif_pmull.S
--rw-r--r--   0 runner    (1001) docker     (121)     7929 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/crc/aarch64/crc32_aarch64_common.h
--rw-r--r--   0 runner    (1001) docker     (121)     3684 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/crc/aarch64/crc32_common_crc_ext_cortex_a72.S
--rw-r--r--   0 runner    (1001) docker     (121)    13330 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/crc/aarch64/crc32_common_mix_neoverse_n1.S
--rw-r--r--   0 runner    (1001) docker     (121)     2996 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/crc/aarch64/crc32_gzip_refl_3crc_fold.S
--rw-r--r--   0 runner    (1001) docker     (121)     2437 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/crc/aarch64/crc32_gzip_refl_crc_ext.S
--rw-r--r--   0 runner    (1001) docker     (121)     1835 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/crc/aarch64/crc32_gzip_refl_pmull.S
--rw-r--r--   0 runner    (1001) docker     (121)     5574 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/crc/aarch64/crc32_gzip_refl_pmull.h
--rw-r--r--   0 runner    (1001) docker     (121)     1835 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/crc/aarch64/crc32_ieee_norm_pmull.S
--rw-r--r--   0 runner    (1001) docker     (121)     5566 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/crc/aarch64/crc32_ieee_norm_pmull.h
--rw-r--r--   0 runner    (1001) docker     (121)     2976 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/crc/aarch64/crc32_iscsi_3crc_fold.S
--rw-r--r--   0 runner    (1001) docker     (121)     2421 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/crc/aarch64/crc32_iscsi_crc_ext.S
--rw-r--r--   0 runner    (1001) docker     (121)     2166 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/crc/aarch64/crc32_iscsi_refl_pmull.S
--rw-r--r--   0 runner    (1001) docker     (121)     5577 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/crc/aarch64/crc32_iscsi_refl_pmull.h
--rw-r--r--   0 runner    (1001) docker     (121)     2852 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/crc/aarch64/crc32_mix_default.S
--rw-r--r--   0 runner    (1001) docker     (121)    14383 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/crc/aarch64/crc32_mix_default_common.S
--rw-r--r--   0 runner    (1001) docker     (121)     2599 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/crc/aarch64/crc32_mix_neoverse_n1.S
--rw-r--r--   0 runner    (1001) docker     (121)     3899 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/crc/aarch64/crc32_norm_common_pmull.h
--rw-r--r--   0 runner    (1001) docker     (121)     3698 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/crc/aarch64/crc32_refl_common_pmull.h
--rw-r--r--   0 runner    (1001) docker     (121)     2895 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/crc/aarch64/crc32c_mix_default.S
--rw-r--r--   0 runner    (1001) docker     (121)     2608 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/crc/aarch64/crc32c_mix_neoverse_n1.S
--rw-r--r--   0 runner    (1001) docker     (121)     1835 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/crc/aarch64/crc64_ecma_norm_pmull.S
--rw-r--r--   0 runner    (1001) docker     (121)     8616 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/crc/aarch64/crc64_ecma_norm_pmull.h
--rw-r--r--   0 runner    (1001) docker     (121)     1835 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/crc/aarch64/crc64_ecma_refl_pmull.S
--rw-r--r--   0 runner    (1001) docker     (121)     8524 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/crc/aarch64/crc64_ecma_refl_pmull.h
--rw-r--r--   0 runner    (1001) docker     (121)     1833 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/crc/aarch64/crc64_iso_norm_pmull.S
--rw-r--r--   0 runner    (1001) docker     (121)     8629 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/crc/aarch64/crc64_iso_norm_pmull.h
--rw-r--r--   0 runner    (1001) docker     (121)     1833 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/crc/aarch64/crc64_iso_refl_pmull.S
--rw-r--r--   0 runner    (1001) docker     (121)     8525 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/crc/aarch64/crc64_iso_refl_pmull.h
--rw-r--r--   0 runner    (1001) docker     (121)     1837 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/crc/aarch64/crc64_jones_norm_pmull.S
--rw-r--r--   0 runner    (1001) docker     (121)     8628 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/crc/aarch64/crc64_jones_norm_pmull.h
--rw-r--r--   0 runner    (1001) docker     (121)     1837 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/crc/aarch64/crc64_jones_refl_pmull.S
--rw-r--r--   0 runner    (1001) docker     (121)     8524 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/crc/aarch64/crc64_jones_refl_pmull.h
--rw-r--r--   0 runner    (1001) docker     (121)     3830 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/crc/aarch64/crc64_norm_common_pmull.h
--rw-r--r--   0 runner    (1001) docker     (121)     3708 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/crc/aarch64/crc64_refl_common_pmull.h
--rw-r--r--   0 runner    (1001) docker     (121)     4787 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/crc/aarch64/crc_aarch64_dispatcher.c
--rw-r--r--   0 runner    (1001) docker     (121)     8408 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/crc/aarch64/crc_common_pmull.h
--rw-r--r--   0 runner    (1001) docker     (121)     2089 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/crc/aarch64/crc_multibinary_arm.S
--rw-r--r--   0 runner    (1001) docker     (121)    16358 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/crc/crc16_t10dif_01.asm
--rw-r--r--   0 runner    (1001) docker     (121)    16470 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/crc/crc16_t10dif_02.asm
--rw-r--r--   0 runner    (1001) docker     (121)    16302 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/crc/crc16_t10dif_by16_10.asm
--rw-r--r--   0 runner    (1001) docker     (121)    13873 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/crc/crc16_t10dif_by4.asm
--rw-r--r--   0 runner    (1001) docker     (121)    14701 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/crc/crc16_t10dif_copy_by4.asm
--rw-r--r--   0 runner    (1001) docker     (121)    14753 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/crc/crc16_t10dif_copy_by4_02.asm
--rw-r--r--   0 runner    (1001) docker     (121)     2893 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/crc/crc16_t10dif_copy_perf.c
--rw-r--r--   0 runner    (1001) docker     (121)     5222 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/crc/crc16_t10dif_copy_test.c
--rw-r--r--   0 runner    (1001) docker     (121)     3823 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/crc/crc16_t10dif_op_perf.c
--rw-r--r--   0 runner    (1001) docker     (121)     2771 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/crc/crc16_t10dif_perf.c
--rw-r--r--   0 runner    (1001) docker     (121)     5646 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/crc/crc16_t10dif_test.c
--rw-r--r--   0 runner    (1001) docker     (121)     9117 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/crc/crc32_funcs_test.c
--rw-r--r--   0 runner    (1001) docker     (121)    15408 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/crc/crc32_gzip_refl_by16_10.asm
--rw-r--r--   0 runner    (1001) docker     (121)    18522 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/crc/crc32_gzip_refl_by8.asm
--rw-r--r--   0 runner    (1001) docker     (121)    15070 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/crc/crc32_gzip_refl_by8_02.asm
--rw-r--r--   0 runner    (1001) docker     (121)     3087 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/crc/crc32_gzip_refl_perf.c
--rw-r--r--   0 runner    (1001) docker     (121)    16265 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/crc/crc32_ieee_01.asm
--rw-r--r--   0 runner    (1001) docker     (121)    16389 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/crc/crc32_ieee_02.asm
--rw-r--r--   0 runner    (1001) docker     (121)    16027 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/crc/crc32_ieee_by16_10.asm
--rw-r--r--   0 runner    (1001) docker     (121)    12342 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/crc/crc32_ieee_by4.asm
--rw-r--r--   0 runner    (1001) docker     (121)     2765 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/crc/crc32_ieee_perf.c
--rw-r--r--   0 runner    (1001) docker     (121)    26502 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/crc/crc32_iscsi_00.asm
--rw-r--r--   0 runner    (1001) docker     (121)    17397 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/crc/crc32_iscsi_01.asm
--rw-r--r--   0 runner    (1001) docker     (121)    15072 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/crc/crc32_iscsi_by16_10.asm
--rw-r--r--   0 runner    (1001) docker     (121)     2768 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/crc/crc32_iscsi_perf.c
--rw-r--r--   0 runner    (1001) docker     (121)    40460 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/crc/crc64_base.c
--rw-r--r--   0 runner    (1001) docker     (121)     2577 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/crc/crc64_ecma_norm_by16_10.asm
--rw-r--r--   0 runner    (1001) docker     (121)    15333 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/crc/crc64_ecma_norm_by8.asm
--rw-r--r--   0 runner    (1001) docker     (121)     2577 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/crc/crc64_ecma_refl_by16_10.asm
--rw-r--r--   0 runner    (1001) docker     (121)    16984 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/crc/crc64_ecma_refl_by8.asm
--rw-r--r--   0 runner    (1001) docker     (121)     2533 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/crc/crc64_example.c
--rw-r--r--   0 runner    (1001) docker     (121)     3550 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/crc/crc64_funcs_perf.c
--rw-r--r--   0 runner    (1001) docker     (121)     9000 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/crc/crc64_funcs_test.c
--rw-r--r--   0 runner    (1001) docker     (121)    14892 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/crc/crc64_iso_norm_by16_10.asm
--rw-r--r--   0 runner    (1001) docker     (121)    15246 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/crc/crc64_iso_norm_by8.asm
--rw-r--r--   0 runner    (1001) docker     (121)    13763 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/crc/crc64_iso_refl_by16_10.asm
--rw-r--r--   0 runner    (1001) docker     (121)    16755 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/crc/crc64_iso_refl_by8.asm
--rw-r--r--   0 runner    (1001) docker     (121)     2578 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/crc/crc64_jones_norm_by16_10.asm
--rw-r--r--   0 runner    (1001) docker     (121)    15254 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/crc/crc64_jones_norm_by8.asm
--rw-r--r--   0 runner    (1001) docker     (121)     2578 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/crc/crc64_jones_refl_by16_10.asm
--rw-r--r--   0 runner    (1001) docker     (121)    16763 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/crc/crc64_jones_refl_by8.asm
--rw-r--r--   0 runner    (1001) docker     (121)     4059 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/crc/crc64_multibinary.asm
--rw-r--r--   0 runner    (1001) docker     (121)     4427 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/crc/crc64_ref.h
--rw-r--r--   0 runner    (1001) docker     (121)    15273 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/crc/crc_base.c
--rw-r--r--   0 runner    (1001) docker     (121)     3207 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/crc/crc_base_aliases.c
--rw-r--r--   0 runner    (1001) docker     (121)     8537 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/crc/crc_multibinary.asm
--rw-r--r--   0 runner    (1001) docker     (121)     4096 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/crc/crc_ref.h
--rw-r--r--   0 runner    (1001) docker     (121)     2463 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/crc/crc_simple_test.c
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-12 13:32:58.023377 isal-1.1.0/src/isal/isa-l/doc/
--rw-r--r--   0 runner    (1001) docker     (121)     1674 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/doc/build.md
--rw-r--r--   0 runner    (1001) docker     (121)     2292 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/doc/test.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-12 13:32:58.035377 isal-1.1.0/src/isal/isa-l/erasure_code/
--rw-r--r--   0 runner    (1001) docker     (121)     6056 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/erasure_code/Makefile.am
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-12 13:32:58.035377 isal-1.1.0/src/isal/isa-l/erasure_code/aarch64/
--rw-r--r--   0 runner    (1001) docker     (121)     2440 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/erasure_code/aarch64/Makefile.am
--rw-r--r--   0 runner    (1001) docker     (121)     2600 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/erasure_code/aarch64/ec_aarch64_dispatcher.c
--rw-r--r--   0 runner    (1001) docker     (121)     4823 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/erasure_code/aarch64/ec_aarch64_highlevel_func.c
--rw-r--r--   0 runner    (1001) docker     (121)     1871 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/erasure_code/aarch64/ec_multibinary_arm.S
--rw-r--r--   0 runner    (1001) docker     (121)    10162 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/erasure_code/aarch64/gf_2vect_dot_prod_neon.S
--rw-r--r--   0 runner    (1001) docker     (121)    10865 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/erasure_code/aarch64/gf_2vect_mad_neon.S
--rw-r--r--   0 runner    (1001) docker     (121)     9087 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/erasure_code/aarch64/gf_3vect_dot_prod_neon.S
--rw-r--r--   0 runner    (1001) docker     (121)    10267 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/erasure_code/aarch64/gf_3vect_mad_neon.S
--rw-r--r--   0 runner    (1001) docker     (121)    10930 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/erasure_code/aarch64/gf_4vect_dot_prod_neon.S
--rw-r--r--   0 runner    (1001) docker     (121)    12303 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/erasure_code/aarch64/gf_4vect_mad_neon.S
--rw-r--r--   0 runner    (1001) docker     (121)    12679 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/erasure_code/aarch64/gf_5vect_dot_prod_neon.S
--rw-r--r--   0 runner    (1001) docker     (121)    14536 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/erasure_code/aarch64/gf_5vect_mad_neon.S
--rw-r--r--   0 runner    (1001) docker     (121)    16767 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/erasure_code/aarch64/gf_6vect_mad_neon.S
--rw-r--r--   0 runner    (1001) docker     (121)     7696 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/erasure_code/aarch64/gf_vect_dot_prod_neon.S
--rw-r--r--   0 runner    (1001) docker     (121)     8356 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/erasure_code/aarch64/gf_vect_mad_neon.S
--rw-r--r--   0 runner    (1001) docker     (121)     6955 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/erasure_code/aarch64/gf_vect_mul_neon.S
--rw-r--r--   0 runner    (1001) docker     (121)     9475 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/erasure_code/ec_base.c
--rw-r--r--   0 runner    (1001) docker     (121)   406502 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/erasure_code/ec_base.h
--rw-r--r--   0 runner    (1001) docker     (121)     2588 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/erasure_code/ec_base_aliases.c
--rw-r--r--   0 runner    (1001) docker     (121)    10380 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/erasure_code/ec_highlevel_func.c
--rw-r--r--   0 runner    (1001) docker     (121)     4147 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/erasure_code/ec_multibinary.asm
--rw-r--r--   0 runner    (1001) docker     (121)     5303 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/erasure_code/erasure_code_base_perf.c
--rw-r--r--   0 runner    (1001) docker     (121)    21974 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/erasure_code/erasure_code_base_test.c
--rw-r--r--   0 runner    (1001) docker     (121)     5341 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/erasure_code/erasure_code_perf.c
--rw-r--r--   0 runner    (1001) docker     (121)    21970 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/erasure_code/erasure_code_test.c
--rw-r--r--   0 runner    (1001) docker     (121)     8645 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/erasure_code/erasure_code_update_perf.c
--rw-r--r--   0 runner    (1001) docker     (121)    27553 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/erasure_code/erasure_code_update_test.c
--rw-r--r--   0 runner    (1001) docker     (121)     2845 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/erasure_code/gen_rs_matrix_limits.c
--rw-r--r--   0 runner    (1001) docker     (121)     8106 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/erasure_code/gf_2vect_dot_prod_avx.asm
--rw-r--r--   0 runner    (1001) docker     (121)     8657 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/erasure_code/gf_2vect_dot_prod_avx2.asm
--rw-r--r--   0 runner    (1001) docker     (121)     6505 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/erasure_code/gf_2vect_dot_prod_avx512.asm
--rw-r--r--   0 runner    (1001) docker     (121)     8114 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/erasure_code/gf_2vect_dot_prod_sse.asm
--rw-r--r--   0 runner    (1001) docker     (121)     6282 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/erasure_code/gf_2vect_mad_avx.asm
--rw-r--r--   0 runner    (1001) docker     (121)     6685 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/erasure_code/gf_2vect_mad_avx2.asm
--rw-r--r--   0 runner    (1001) docker     (121)     6300 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/erasure_code/gf_2vect_mad_avx512.asm
--rw-r--r--   0 runner    (1001) docker     (121)     6391 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/erasure_code/gf_2vect_mad_sse.asm
--rw-r--r--   0 runner    (1001) docker     (121)     9365 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/erasure_code/gf_3vect_dot_prod_avx.asm
--rw-r--r--   0 runner    (1001) docker     (121)    10086 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/erasure_code/gf_3vect_dot_prod_avx2.asm
--rw-r--r--   0 runner    (1001) docker     (121)     7308 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/erasure_code/gf_3vect_dot_prod_avx512.asm
--rw-r--r--   0 runner    (1001) docker     (121)     9314 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/erasure_code/gf_3vect_dot_prod_sse.asm
--rw-r--r--   0 runner    (1001) docker     (121)     8280 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/erasure_code/gf_3vect_mad_avx.asm
--rw-r--r--   0 runner    (1001) docker     (121)     9195 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/erasure_code/gf_3vect_mad_avx2.asm
--rw-r--r--   0 runner    (1001) docker     (121)     7000 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/erasure_code/gf_3vect_mad_avx512.asm
--rw-r--r--   0 runner    (1001) docker     (121)     8306 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/erasure_code/gf_3vect_mad_sse.asm
--rw-r--r--   0 runner    (1001) docker     (121)    11494 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/erasure_code/gf_4vect_dot_prod_avx.asm
--rw-r--r--   0 runner    (1001) docker     (121)    12268 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/erasure_code/gf_4vect_dot_prod_avx2.asm
--rw-r--r--   0 runner    (1001) docker     (121)     8311 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/erasure_code/gf_4vect_dot_prod_avx512.asm
--rw-r--r--   0 runner    (1001) docker     (121)    11487 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/erasure_code/gf_4vect_dot_prod_sse.asm
--rw-r--r--   0 runner    (1001) docker     (121)     9677 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/erasure_code/gf_4vect_mad_avx.asm
--rw-r--r--   0 runner    (1001) docker     (121)    10145 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/erasure_code/gf_4vect_mad_avx2.asm
--rw-r--r--   0 runner    (1001) docker     (121)     7647 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/erasure_code/gf_4vect_mad_avx512.asm
--rw-r--r--   0 runner    (1001) docker     (121)     9468 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/erasure_code/gf_4vect_mad_sse.asm
--rw-r--r--   0 runner    (1001) docker     (121)     8386 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/erasure_code/gf_5vect_dot_prod_avx.asm
--rw-r--r--   0 runner    (1001) docker     (121)     8819 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/erasure_code/gf_5vect_dot_prod_avx2.asm
--rw-r--r--   0 runner    (1001) docker     (121)     9392 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/erasure_code/gf_5vect_dot_prod_avx512.asm
--rw-r--r--   0 runner    (1001) docker     (121)     8318 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/erasure_code/gf_5vect_dot_prod_sse.asm
--rw-r--r--   0 runner    (1001) docker     (121)    10917 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/erasure_code/gf_5vect_mad_avx.asm
--rw-r--r--   0 runner    (1001) docker     (121)    11110 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/erasure_code/gf_5vect_mad_avx2.asm
--rw-r--r--   0 runner    (1001) docker     (121)     8341 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/erasure_code/gf_5vect_mad_avx512.asm
--rw-r--r--   0 runner    (1001) docker     (121)    10727 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/erasure_code/gf_5vect_mad_sse.asm
--rw-r--r--   0 runner    (1001) docker     (121)     8817 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/erasure_code/gf_6vect_dot_prod_avx.asm
--rw-r--r--   0 runner    (1001) docker     (121)     9290 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/erasure_code/gf_6vect_dot_prod_avx2.asm
--rw-r--r--   0 runner    (1001) docker     (121)    10053 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/erasure_code/gf_6vect_dot_prod_avx512.asm
--rw-r--r--   0 runner    (1001) docker     (121)     8740 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/erasure_code/gf_6vect_dot_prod_sse.asm
--rw-r--r--   0 runner    (1001) docker     (121)    11988 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/erasure_code/gf_6vect_mad_avx.asm
--rw-r--r--   0 runner    (1001) docker     (121)    12582 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/erasure_code/gf_6vect_mad_avx2.asm
--rw-r--r--   0 runner    (1001) docker     (121)     9329 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/erasure_code/gf_6vect_mad_avx512.asm
--rw-r--r--   0 runner    (1001) docker     (121)    11959 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/erasure_code/gf_6vect_mad_sse.asm
--rw-r--r--   0 runner    (1001) docker     (121)     5131 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/erasure_code/gf_inverse_test.c
--rw-r--r--   0 runner    (1001) docker     (121)     4424 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/erasure_code/gf_vect_dot_prod_1tbl.c
--rw-r--r--   0 runner    (1001) docker     (121)     6114 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/erasure_code/gf_vect_dot_prod_avx.asm
--rw-r--r--   0 runner    (1001) docker     (121)     6397 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/erasure_code/gf_vect_dot_prod_avx2.asm
--rw-r--r--   0 runner    (1001) docker     (121)     6165 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/erasure_code/gf_vect_dot_prod_avx512.asm
--rw-r--r--   0 runner    (1001) docker     (121)     7380 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/erasure_code/gf_vect_dot_prod_base_test.c
--rw-r--r--   0 runner    (1001) docker     (121)     5054 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/erasure_code/gf_vect_dot_prod_perf.c
--rw-r--r--   0 runner    (1001) docker     (121)     6106 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/erasure_code/gf_vect_dot_prod_sse.asm
--rw-r--r--   0 runner    (1001) docker     (121)    13606 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/erasure_code/gf_vect_dot_prod_test.c
--rw-r--r--   0 runner    (1001) docker     (121)     5156 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/erasure_code/gf_vect_mad_avx.asm
--rw-r--r--   0 runner    (1001) docker     (121)     5400 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/erasure_code/gf_vect_mad_avx2.asm
--rw-r--r--   0 runner    (1001) docker     (121)     5158 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/erasure_code/gf_vect_mad_avx512.asm
--rw-r--r--   0 runner    (1001) docker     (121)     5218 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/erasure_code/gf_vect_mad_sse.asm
--rw-r--r--   0 runner    (1001) docker     (121)    13905 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/erasure_code/gf_vect_mad_test.c
--rw-r--r--   0 runner    (1001) docker     (121)     4673 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/erasure_code/gf_vect_mul_avx.asm
--rw-r--r--   0 runner    (1001) docker     (121)     4145 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/erasure_code/gf_vect_mul_base_test.c
--rw-r--r--   0 runner    (1001) docker     (121)     3118 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/erasure_code/gf_vect_mul_perf.c
--rw-r--r--   0 runner    (1001) docker     (121)     4680 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/erasure_code/gf_vect_mul_sse.asm
--rw-r--r--   0 runner    (1001) docker     (121)     4881 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/erasure_code/gf_vect_mul_test.c
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-12 13:32:58.035377 isal-1.1.0/src/isal/isa-l/erasure_code/ppc64le/
--rw-r--r--   0 runner    (1001) docker     (121)      656 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/erasure_code/ppc64le/Makefile.am
--rw-r--r--   0 runner    (1001) docker     (121)     2106 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/erasure_code/ppc64le/ec_base_vsx.c
--rw-r--r--   0 runner    (1001) docker     (121)    14099 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/erasure_code/ppc64le/ec_base_vsx.h
--rw-r--r--   0 runner    (1001) docker     (121)     2132 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/erasure_code/ppc64le/gf_2vect_dot_prod_vsx.c
--rw-r--r--   0 runner    (1001) docker     (121)     1895 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/erasure_code/ppc64le/gf_2vect_mad_vsx.c
--rw-r--r--   0 runner    (1001) docker     (121)     2844 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/erasure_code/ppc64le/gf_3vect_dot_prod_vsx.c
--rw-r--r--   0 runner    (1001) docker     (121)     2580 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/erasure_code/ppc64le/gf_3vect_mad_vsx.c
--rw-r--r--   0 runner    (1001) docker     (121)     3555 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/erasure_code/ppc64le/gf_4vect_dot_prod_vsx.c
--rw-r--r--   0 runner    (1001) docker     (121)     3265 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/erasure_code/ppc64le/gf_4vect_mad_vsx.c
--rw-r--r--   0 runner    (1001) docker     (121)     4267 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/erasure_code/ppc64le/gf_5vect_dot_prod_vsx.c
--rw-r--r--   0 runner    (1001) docker     (121)     3950 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/erasure_code/ppc64le/gf_5vect_mad_vsx.c
--rw-r--r--   0 runner    (1001) docker     (121)     5024 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/erasure_code/ppc64le/gf_6vect_dot_prod_vsx.c
--rw-r--r--   0 runner    (1001) docker     (121)     4657 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/erasure_code/ppc64le/gf_6vect_mad_vsx.c
--rw-r--r--   0 runner    (1001) docker     (121)     2053 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/erasure_code/ppc64le/gf_vect_dot_prod_vsx.c
--rw-r--r--   0 runner    (1001) docker     (121)     1229 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/erasure_code/ppc64le/gf_vect_mad_vsx.c
--rw-r--r--   0 runner    (1001) docker     (121)     1483 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/erasure_code/ppc64le/gf_vect_mul_vsx.c
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-12 13:32:58.011376 isal-1.1.0/src/isal/isa-l/examples/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-12 13:32:58.039377 isal-1.1.0/src/isal/isa-l/examples/ec/
--rw-r--r--   0 runner    (1001) docker     (121)     1860 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/examples/ec/Makefile.am
--rw-r--r--   0 runner    (1001) docker     (121)      140 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/examples/ec/Makefile.unx
--rw-r--r--   0 runner    (1001) docker     (121)    13870 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/examples/ec/ec_piggyback_example.c
--rw-r--r--   0 runner    (1001) docker     (121)     8026 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/examples/ec/ec_simple_example.c
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-12 13:32:58.047377 isal-1.1.0/src/isal/isa-l/igzip/
--rw-r--r--   0 runner    (1001) docker     (121)     5495 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/igzip/Makefile.am
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-12 13:32:58.051377 isal-1.1.0/src/isal/isa-l/igzip/aarch64/
--rw-r--r--   0 runner    (1001) docker     (121)     2443 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/igzip/aarch64/bitbuf2_aarch64.h
--rw-r--r--   0 runner    (1001) docker     (121)     8483 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/igzip/aarch64/data_struct_aarch64.h
--rw-r--r--   0 runner    (1001) docker     (121)     5500 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/igzip/aarch64/encode_df.S
--rw-r--r--   0 runner    (1001) docker     (121)     7557 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/igzip/aarch64/gen_icf_map.S
--rw-r--r--   0 runner    (1001) docker     (121)     5865 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/igzip/aarch64/huffman_aarch64.h
--rw-r--r--   0 runner    (1001) docker     (121)    21035 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/igzip/aarch64/igzip_decode_huffman_code_block_aarch64.S
--rw-r--r--   0 runner    (1001) docker     (121)     8392 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/igzip/aarch64/igzip_deflate_body_aarch64.S
--rw-r--r--   0 runner    (1001) docker     (121)     8406 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/igzip/aarch64/igzip_deflate_finish_aarch64.S
--rw-r--r--   0 runner    (1001) docker     (121)     3305 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/igzip/aarch64/igzip_deflate_hash_aarch64.S
--rw-r--r--   0 runner    (1001) docker     (121)     1780 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/igzip/aarch64/igzip_inflate_multibinary_arm64.S
--rw-r--r--   0 runner    (1001) docker     (121)     4721 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/igzip/aarch64/igzip_isal_adler32_neon.S
--rw-r--r--   0 runner    (1001) docker     (121)     5722 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/igzip/aarch64/igzip_multibinary_aarch64_dispatcher.c
--rw-r--r--   0 runner    (1001) docker     (121)     2387 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/igzip/aarch64/igzip_multibinary_arm64.S
--rw-r--r--   0 runner    (1001) docker     (121)     5745 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/igzip/aarch64/igzip_set_long_icf_fg.S
--rw-r--r--   0 runner    (1001) docker     (121)    10098 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/igzip/aarch64/isal_deflate_icf_body_hash_hist.S
--rw-r--r--   0 runner    (1001) docker     (121)    10211 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/igzip/aarch64/isal_deflate_icf_finish_hash_hist.S
--rw-r--r--   0 runner    (1001) docker     (121)     9433 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/igzip/aarch64/isal_update_histogram.S
--rw-r--r--   0 runner    (1001) docker     (121)     3037 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/igzip/aarch64/lz0a_const_aarch64.h
--rw-r--r--   0 runner    (1001) docker     (121)     2435 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/igzip/aarch64/options_aarch64.h
--rw-r--r--   0 runner    (1001) docker     (121)     2297 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/igzip/aarch64/stdmac_aarch64.h
--rw-r--r--   0 runner    (1001) docker     (121)     6568 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/igzip/adler32_avx2_4.asm
--rw-r--r--   0 runner    (1001) docker     (121)     2264 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/igzip/adler32_base.c
--rw-r--r--   0 runner    (1001) docker     (121)     2648 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/igzip/adler32_perf.c
--rw-r--r--   0 runner    (1001) docker     (121)     5234 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/igzip/adler32_sse.asm
--rw-r--r--   0 runner    (1001) docker     (121)     2419 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/igzip/bitbuf2.asm
--rw-r--r--   0 runner    (1001) docker     (121)     4149 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/igzip/bitbuf2.h
--rw-r--r--   0 runner    (1001) docker     (121)     8193 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/igzip/checksum32_funcs_test.c
--rw-r--r--   0 runner    (1001) docker     (121)     3849 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/igzip/checksum_test_ref.h
--rw-r--r--   0 runner    (1001) docker     (121)    10738 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/igzip/data_struct2.asm
--rw-r--r--   0 runner    (1001) docker     (121)      963 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/igzip/encode_df.c
--rw-r--r--   0 runner    (1001) docker     (121)      944 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/igzip/encode_df.h
--rw-r--r--   0 runner    (1001) docker     (121)    14839 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/igzip/encode_df_04.asm
--rw-r--r--   0 runner    (1001) docker     (121)    15380 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/igzip/encode_df_06.asm
--rw-r--r--   0 runner    (1001) docker     (121)      798 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/igzip/flatten_ll.c
--rw-r--r--   0 runner    (1001) docker     (121)       57 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/igzip/flatten_ll.h
--rw-r--r--   0 runner    (1001) docker     (121)    15782 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/igzip/generate_custom_hufftables.c
--rw-r--r--   0 runner    (1001) docker     (121)     7484 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/igzip/generate_static_inflate.c
--rw-r--r--   0 runner    (1001) docker     (121)     3431 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/igzip/heap_macros.asm
--rw-r--r--   0 runner    (1001) docker     (121)    64686 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/igzip/huff_codes.c
--rw-r--r--   0 runner    (1001) docker     (121)     5159 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/igzip/huff_codes.h
--rw-r--r--   0 runner    (1001) docker     (121)     7651 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/igzip/huffman.asm
--rw-r--r--   0 runner    (1001) docker     (121)     8316 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/igzip/huffman.h
--rw-r--r--   0 runner    (1001) docker     (121)   379753 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/igzip/hufftables_c.c
--rw-r--r--   0 runner    (1001) docker     (121)    60765 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/igzip/igzip.c
--rw-r--r--   0 runner    (1001) docker     (121)     6154 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/igzip/igzip_base.c
--rw-r--r--   0 runner    (1001) docker     (121)     5839 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/igzip/igzip_base_aliases.c
--rw-r--r--   0 runner    (1001) docker     (121)    19012 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/igzip/igzip_body.asm
--rw-r--r--   0 runner    (1001) docker     (121)      796 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/igzip/igzip_build_hash_table_perf.c
--rw-r--r--   0 runner    (1001) docker     (121)      308 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/igzip/igzip_checksums.h
--rw-r--r--   0 runner    (1001) docker     (121)    10827 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/igzip/igzip_compare_types.asm
--rw-r--r--   0 runner    (1001) docker     (121)    22135 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/igzip/igzip_decode_block_stateless.asm
--rw-r--r--   0 runner    (1001) docker     (121)       61 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/igzip/igzip_decode_block_stateless_01.asm
--rw-r--r--   0 runner    (1001) docker     (121)       79 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/igzip/igzip_decode_block_stateless_04.asm
--rw-r--r--   0 runner    (1001) docker     (121)     3855 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/igzip/igzip_deflate_hash.asm
--rw-r--r--   0 runner    (1001) docker     (121)     3225 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/igzip/igzip_example.c
--rw-r--r--   0 runner    (1001) docker     (121)     9332 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/igzip/igzip_file_perf.c
--rw-r--r--   0 runner    (1001) docker     (121)     9236 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/igzip/igzip_finish.asm
--rw-r--r--   0 runner    (1001) docker     (121)    20586 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/igzip/igzip_gen_icf_map_lh1_04.asm
--rw-r--r--   0 runner    (1001) docker     (121)    15185 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/igzip/igzip_gen_icf_map_lh1_06.asm
--rw-r--r--   0 runner    (1001) docker     (121)     3950 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/igzip/igzip_hist_perf.c
--rw-r--r--   0 runner    (1001) docker     (121)    10312 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/igzip/igzip_icf_base.c
--rw-r--r--   0 runner    (1001) docker     (121)    10360 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/igzip/igzip_icf_body.c
--rw-r--r--   0 runner    (1001) docker     (121)    21600 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/igzip/igzip_icf_body_h1_gr_bt.asm
--rw-r--r--   0 runner    (1001) docker     (121)     8691 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/igzip/igzip_icf_finish.asm
--rw-r--r--   0 runner    (1001) docker     (121)    76698 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/igzip/igzip_inflate.c
--rw-r--r--   0 runner    (1001) docker     (121)     2236 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/igzip/igzip_inflate_multibinary.asm
--rw-r--r--   0 runner    (1001) docker     (121)     8840 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/igzip/igzip_inflate_test.c
--rw-r--r--   0 runner    (1001) docker     (121)     1100 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/igzip/igzip_level_buf_structs.h
--rw-r--r--   0 runner    (1001) docker     (121)     6308 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/igzip/igzip_multibinary.asm
--rw-r--r--   0 runner    (1001) docker     (121)    22446 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/igzip/igzip_perf.c
--rw-r--r--   0 runner    (1001) docker     (121)    80528 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/igzip/igzip_rand_test.c
--rw-r--r--   0 runner    (1001) docker     (121)     9326 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/igzip/igzip_semi_dyn_file_perf.c
--rw-r--r--   0 runner    (1001) docker     (121)     8046 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/igzip/igzip_set_long_icf_fg_04.asm
--rw-r--r--   0 runner    (1001) docker     (121)     9836 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/igzip/igzip_set_long_icf_fg_06.asm
--rw-r--r--   0 runner    (1001) docker     (121)     2981 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/igzip/igzip_sync_flush_example.c
--rw-r--r--   0 runner    (1001) docker     (121)    14353 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/igzip/igzip_update_histogram.asm
--rw-r--r--   0 runner    (1001) docker     (121)      107 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/igzip/igzip_update_histogram_01.asm
--rw-r--r--   0 runner    (1001) docker     (121)      125 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/igzip/igzip_update_histogram_04.asm
--rw-r--r--   0 runner    (1001) docker     (121)     2194 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/igzip/igzip_wrapper.h
--rw-r--r--   0 runner    (1001) docker     (121)    20453 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/igzip/igzip_wrapper_hdr_test.c
--rw-r--r--   0 runner    (1001) docker     (121)     5879 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/igzip/inflate_data_structs.asm
--rw-r--r--   0 runner    (1001) docker     (121)    57015 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/igzip/inflate_std_vects.h
--rw-r--r--   0 runner    (1001) docker     (121)     3011 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/igzip/lz0a_const.asm
--rw-r--r--   0 runner    (1001) docker     (121)     2577 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/igzip/options.asm
--rw-r--r--   0 runner    (1001) docker     (121)     3461 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/igzip/proc_heap.asm
--rw-r--r--   0 runner    (1001) docker     (121)     2912 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/igzip/proc_heap_base.c
--rw-r--r--   0 runner    (1001) docker     (121)     2966 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/igzip/repeated_char_result.h
--rw-r--r--   0 runner    (1001) docker     (121)     5044 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/igzip/rfc1951_lookup.asm
--rw-r--r--   0 runner    (1001) docker     (121)   142279 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/igzip/static_inflate.h
--rw-r--r--   0 runner    (1001) docker     (121)    10063 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/igzip/stdmac.asm
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-12 13:32:58.051377 isal-1.1.0/src/isal/isa-l/include/
--rw-r--r--   0 runner    (1001) docker     (121)     9912 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/include/aarch64_multibinary.h
--rw-r--r--   0 runner    (1001) docker     (121)     7052 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/include/crc.h
--rw-r--r--   0 runner    (1001) docker     (121)     8849 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/include/crc64.h
--rw-r--r--   0 runner    (1001) docker     (121)    38530 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/include/erasure_code.h
--rw-r--r--   0 runner    (1001) docker     (121)     6108 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/include/gf_vect_mul.h
--rw-r--r--   0 runner    (1001) docker     (121)    44454 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/include/igzip_lib.h
--rw-r--r--   0 runner    (1001) docker     (121)     2397 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/include/mem_routines.h
--rw-r--r--   0 runner    (1001) docker     (121)    11018 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/include/multibinary.asm
--rw-r--r--   0 runner    (1001) docker     (121)    10414 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/include/raid.h
--rw-r--r--   0 runner    (1001) docker     (121)     7433 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/include/reg_sizes.asm
--rw-r--r--   0 runner    (1001) docker     (121)     7815 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/include/test.h
--rw-r--r--   0 runner    (1001) docker     (121)     2771 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/include/types.h
--rw-r--r--   0 runner    (1001) docker     (121)     2634 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/include/unaligned.h
--rw-r--r--   0 runner    (1001) docker     (121)     3479 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/isa-l.def
--rw-r--r--   0 runner    (1001) docker     (121)      220 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/libisal.pc.in
--rw-r--r--   0 runner    (1001) docker     (121)    12362 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/make.inc
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-12 13:32:58.051377 isal-1.1.0/src/isal/isa-l/mem/
--rw-r--r--   0 runner    (1001) docker     (121)     2202 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/mem/Makefile.am
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-12 13:32:58.051377 isal-1.1.0/src/isal/isa-l/mem/aarch64/
--rw-r--r--   0 runner    (1001) docker     (121)     1856 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/mem/aarch64/Makefile.am
--rw-r--r--   0 runner    (1001) docker     (121)     1939 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/mem/aarch64/mem_aarch64_dispatcher.c
--rw-r--r--   0 runner    (1001) docker     (121)     1791 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/mem/aarch64/mem_multibinary_arm.S
--rw-r--r--   0 runner    (1001) docker     (121)     5432 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/mem/aarch64/mem_zero_detect_neon.S
--rw-r--r--   0 runner    (1001) docker     (121)     2046 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/mem/mem_multibinary.asm
--rw-r--r--   0 runner    (1001) docker     (121)     4356 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/mem/mem_zero_detect_avx.asm
--rw-r--r--   0 runner    (1001) docker     (121)     2412 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/mem/mem_zero_detect_base.c
--rw-r--r--   0 runner    (1001) docker     (121)     1887 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/mem/mem_zero_detect_base_aliases.c
--rw-r--r--   0 runner    (1001) docker     (121)     2330 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/mem/mem_zero_detect_perf.c
--rw-r--r--   0 runner    (1001) docker     (121)     4142 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/mem/mem_zero_detect_sse.asm
--rw-r--r--   0 runner    (1001) docker     (121)     5984 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/mem/mem_zero_detect_test.c
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-12 13:32:58.051377 isal-1.1.0/src/isal/isa-l/programs/
--rw-r--r--   0 runner    (1001) docker     (121)     2007 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/programs/Makefile.am
--rw-r--r--   0 runner    (1001) docker     (121)     1982 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/programs/igzip.1
--rw-r--r--   0 runner    (1001) docker     (121)      646 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/programs/igzip.1.h2m
--rw-r--r--   0 runner    (1001) docker     (121)    30935 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/programs/igzip_cli.c
--rwxr-xr-x   0 runner    (1001) docker     (121)     7084 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/programs/igzip_cli_check.sh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-12 13:32:58.055377 isal-1.1.0/src/isal/isa-l/raid/
--rw-r--r--   0 runner    (1001) docker     (121)     2689 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/raid/Makefile.am
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-12 13:32:58.055377 isal-1.1.0/src/isal/isa-l/raid/aarch64/
--rw-r--r--   0 runner    (1001) docker     (121)     1953 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/raid/aarch64/Makefile.am
--rw-r--r--   0 runner    (1001) docker     (121)     9158 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/raid/aarch64/pq_check_neon.S
--rw-r--r--   0 runner    (1001) docker     (121)     7847 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/raid/aarch64/pq_gen_neon.S
--rw-r--r--   0 runner    (1001) docker     (121)     2349 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/raid/aarch64/raid_aarch64_dispatcher.c
--rw-r--r--   0 runner    (1001) docker     (121)     1853 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/raid/aarch64/raid_multibinary_arm.S
--rw-r--r--   0 runner    (1001) docker     (121)     7054 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/raid/aarch64/xor_check_neon.S
--rw-r--r--   0 runner    (1001) docker     (121)     7034 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/raid/aarch64/xor_gen_neon.S
--rw-r--r--   0 runner    (1001) docker     (121)     8117 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/raid/pq_check_sse.asm
--rw-r--r--   0 runner    (1001) docker     (121)     7801 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/raid/pq_check_sse_i32.asm
--rw-r--r--   0 runner    (1001) docker     (121)     8407 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/raid/pq_check_test.c
--rw-r--r--   0 runner    (1001) docker     (121)     7640 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/raid/pq_gen_avx.asm
--rw-r--r--   0 runner    (1001) docker     (121)     7724 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/raid/pq_gen_avx2.asm
--rw-r--r--   0 runner    (1001) docker     (121)     6981 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/raid/pq_gen_avx512.asm
--rw-r--r--   0 runner    (1001) docker     (121)     3050 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/raid/pq_gen_perf.c
--rw-r--r--   0 runner    (1001) docker     (121)     7628 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/raid/pq_gen_sse.asm
--rw-r--r--   0 runner    (1001) docker     (121)     7371 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/raid/pq_gen_sse_i32.asm
--rw-r--r--   0 runner    (1001) docker     (121)     5043 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/raid/pq_gen_test.c
--rw-r--r--   0 runner    (1001) docker     (121)     4238 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/raid/raid_base.c
--rw-r--r--   0 runner    (1001) docker     (121)     2094 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/raid/raid_base_aliases.c
--rw-r--r--   0 runner    (1001) docker     (121)     3769 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/raid/raid_multibinary.asm
--rw-r--r--   0 runner    (1001) docker     (121)     2386 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/raid/raid_multibinary_i32.asm
--rw-r--r--   0 runner    (1001) docker     (121)     6911 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/raid/xor_check_sse.asm
--rw-r--r--   0 runner    (1001) docker     (121)     7859 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/raid/xor_check_test.c
--rw-r--r--   0 runner    (1001) docker     (121)     2736 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/raid/xor_example.c
--rw-r--r--   0 runner    (1001) docker     (121)     6012 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/raid/xor_gen_avx.asm
--rw-r--r--   0 runner    (1001) docker     (121)     5787 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/raid/xor_gen_avx512.asm
--rw-r--r--   0 runner    (1001) docker     (121)     3043 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/raid/xor_gen_perf.c
--rw-r--r--   0 runner    (1001) docker     (121)     7110 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/raid/xor_gen_sse.asm
--rw-r--r--   0 runner    (1001) docker     (121)     4404 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/raid/xor_gen_test.c
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-12 13:32:58.011376 isal-1.1.0/src/isal/isa-l/tests/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-12 13:32:58.059377 isal-1.1.0/src/isal/isa-l/tests/fuzz/
--rw-r--r--   0 runner    (1001) docker     (121)     2616 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/tests/fuzz/Makefile.am
--rw-r--r--   0 runner    (1001) docker     (121)      189 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/tests/fuzz/Makefile.unx
--rw-r--r--   0 runner    (1001) docker     (121)     2264 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/tests/fuzz/igzip_checked_inflate_fuzz_test.c
--rw-r--r--   0 runner    (1001) docker     (121)      897 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/tests/fuzz/igzip_dump_inflate_corpus.c
--rw-r--r--   0 runner    (1001) docker     (121)      913 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/tests/fuzz/igzip_fuzz_inflate.c
--rw-r--r--   0 runner    (1001) docker     (121)      489 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/tests/fuzz/igzip_simple_inflate_fuzz_test.c
--rw-r--r--   0 runner    (1001) docker     (121)     3516 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/tests/fuzz/igzip_simple_round_trip_fuzz_test.c
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-12 13:32:58.059377 isal-1.1.0/src/isal/isa-l/tools/
--rwxr-xr-x   0 runner    (1001) docker     (121)     2424 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/tools/check_format.sh
--rw-r--r--   0 runner    (1001) docker     (121)     6408 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/tools/gen_nmake.mk
--rwxr-xr-x   0 runner    (1001) docker     (121)       54 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/tools/iindent
--rwxr-xr-x   0 runner    (1001) docker     (121)      961 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/tools/nasm-cet-filter.sh
--rwxr-xr-x   0 runner    (1001) docker     (121)      917 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/tools/nasm-filter.sh
--rwxr-xr-x   0 runner    (1001) docker     (121)       49 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/tools/remove_trailing_whitespace.sh
--rwxr-xr-x   0 runner    (1001) docker     (121)     1297 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/tools/test_autorun.sh
--rwxr-xr-x   0 runner    (1001) docker     (121)     2989 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/tools/test_checks.sh
--rwxr-xr-x   0 runner    (1001) docker     (121)     5765 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/tools/test_extended.sh
--rwxr-xr-x   0 runner    (1001) docker     (121)     4608 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/tools/test_fuzz.sh
--rwxr-xr-x   0 runner    (1001) docker     (121)      148 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/tools/test_tools.sh
--rwxr-xr-x   0 runner    (1001) docker     (121)      851 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/tools/yasm-cet-filter.sh
--rwxr-xr-x   0 runner    (1001) docker     (121)      807 2022-10-12 13:21:38.000000 isal-1.1.0/src/isal/isa-l/tools/yasm-filter.sh
--rw-r--r--   0 runner    (1001) docker     (121)    12076 2022-10-12 13:21:37.000000 isal-1.1.0/src/isal/isal_shared.h
--rw-r--r--   0 runner    (1001) docker     (121)     1754 2022-10-12 13:21:37.000000 isal-1.1.0/src/isal/isal_zlib.pyi
--rw-r--r--   0 runner    (1001) docker     (121)    38931 2022-10-12 13:21:37.000000 isal-1.1.0/src/isal/isal_zlibmodule.c
--rw-r--r--   0 runner    (1001) docker     (121)       27 2022-10-12 13:21:37.000000 isal-1.1.0/src/isal/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-12 13:32:58.011376 isal-1.1.0/src/isal.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     8609 2022-10-12 13:32:57.000000 isal-1.1.0/src/isal.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    17784 2022-10-12 13:32:58.000000 isal-1.1.0/src/isal.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-12 13:32:57.000000 isal-1.1.0/src/isal.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-12 13:32:57.000000 isal-1.1.0/src/isal.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-10-12 13:32:57.000000 isal-1.1.0/src/isal.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:29:00.935249 isal-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-07-21 12:22:12.000000 isal-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-21 12:22:12.000000 isal-1.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8675 2023-07-21 12:29:00.935249 isal-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7358 2023-07-21 12:22:12.000000 isal-1.2.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-21 12:22:12.000000 isal-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-21 12:29:00.935249 isal-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     7639 2023-07-21 12:22:12.000000 isal-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:29:00.875248 isal-1.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:29:00.879248 isal-1.2.0/src/isal/
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-07-21 12:22:12.000000 isal-1.2.0/src/isal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-21 12:22:12.000000 isal-1.2.0/src/isal/_isal.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-07-21 12:22:12.000000 isal-1.2.0/src/isal/_isalmodule.c
+-rw-r--r--   0 runner    (1001) docker     (123)    23378 2023-07-21 12:22:12.000000 isal-1.2.0/src/isal/igzip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-07-21 12:22:12.000000 isal-1.2.0/src/isal/igzip_lib.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    23610 2023-07-21 12:22:12.000000 isal-1.2.0/src/isal/igzip_libmodule.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:29:00.883248 isal-1.2.0/src/isal/isa-l/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-21 12:22:13.000000 isal-1.2.0/src/isal/isa-l/.git
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/.travis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/Doxyfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4497 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/Makefile.am
+-rw-r--r--   0 runner    (1001) docker     (123)    10136 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/Makefile.nmake
+-rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/Makefile.unx
+-rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     9439 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/Release_notes.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      429 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/autogen.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     8871 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/configure.ac
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:29:00.891248 isal-1.2.0/src/isal/isa-l/crc/
+-rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/crc/Makefile.am
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:29:00.895248 isal-1.2.0/src/isal/isa-l/crc/aarch64/
+-rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/crc/aarch64/Makefile.am
+-rw-r--r--   0 runner    (1001) docker     (123)    11478 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/crc/aarch64/crc16_t10dif_copy_pmull.S
+-rw-r--r--   0 runner    (1001) docker     (123)    11068 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/crc/aarch64/crc16_t10dif_pmull.S
+-rw-r--r--   0 runner    (1001) docker     (123)     7929 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/crc/aarch64/crc32_aarch64_common.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/crc/aarch64/crc32_common_crc_ext_cortex_a72.S
+-rw-r--r--   0 runner    (1001) docker     (123)    13330 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/crc/aarch64/crc32_common_mix_neoverse_n1.S
+-rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/crc/aarch64/crc32_gzip_refl_3crc_fold.S
+-rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/crc/aarch64/crc32_gzip_refl_crc_ext.S
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/crc/aarch64/crc32_gzip_refl_pmull.S
+-rw-r--r--   0 runner    (1001) docker     (123)     5574 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/crc/aarch64/crc32_gzip_refl_pmull.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/crc/aarch64/crc32_ieee_norm_pmull.S
+-rw-r--r--   0 runner    (1001) docker     (123)     5566 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/crc/aarch64/crc32_ieee_norm_pmull.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/crc/aarch64/crc32_iscsi_3crc_fold.S
+-rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/crc/aarch64/crc32_iscsi_crc_ext.S
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/crc/aarch64/crc32_iscsi_refl_pmull.S
+-rw-r--r--   0 runner    (1001) docker     (123)     5577 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/crc/aarch64/crc32_iscsi_refl_pmull.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/crc/aarch64/crc32_mix_default.S
+-rw-r--r--   0 runner    (1001) docker     (123)    14383 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/crc/aarch64/crc32_mix_default_common.S
+-rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/crc/aarch64/crc32_mix_neoverse_n1.S
+-rw-r--r--   0 runner    (1001) docker     (123)     3899 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/crc/aarch64/crc32_norm_common_pmull.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3698 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/crc/aarch64/crc32_refl_common_pmull.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/crc/aarch64/crc32c_mix_default.S
+-rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/crc/aarch64/crc32c_mix_neoverse_n1.S
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/crc/aarch64/crc64_ecma_norm_pmull.S
+-rw-r--r--   0 runner    (1001) docker     (123)     8616 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/crc/aarch64/crc64_ecma_norm_pmull.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/crc/aarch64/crc64_ecma_refl_pmull.S
+-rw-r--r--   0 runner    (1001) docker     (123)     8524 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/crc/aarch64/crc64_ecma_refl_pmull.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/crc/aarch64/crc64_iso_norm_pmull.S
+-rw-r--r--   0 runner    (1001) docker     (123)     8629 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/crc/aarch64/crc64_iso_norm_pmull.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/crc/aarch64/crc64_iso_refl_pmull.S
+-rw-r--r--   0 runner    (1001) docker     (123)     8525 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/crc/aarch64/crc64_iso_refl_pmull.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/crc/aarch64/crc64_jones_norm_pmull.S
+-rw-r--r--   0 runner    (1001) docker     (123)     8628 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/crc/aarch64/crc64_jones_norm_pmull.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/crc/aarch64/crc64_jones_refl_pmull.S
+-rw-r--r--   0 runner    (1001) docker     (123)     8524 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/crc/aarch64/crc64_jones_refl_pmull.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3830 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/crc/aarch64/crc64_norm_common_pmull.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3708 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/crc/aarch64/crc64_refl_common_pmull.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4787 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/crc/aarch64/crc_aarch64_dispatcher.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8408 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/crc/aarch64/crc_common_pmull.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/crc/aarch64/crc_multibinary_arm.S
+-rw-r--r--   0 runner    (1001) docker     (123)    16358 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/crc/crc16_t10dif_01.asm
+-rw-r--r--   0 runner    (1001) docker     (123)    16470 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/crc/crc16_t10dif_02.asm
+-rw-r--r--   0 runner    (1001) docker     (123)    16302 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/crc/crc16_t10dif_by16_10.asm
+-rw-r--r--   0 runner    (1001) docker     (123)    13873 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/crc/crc16_t10dif_by4.asm
+-rw-r--r--   0 runner    (1001) docker     (123)    14701 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/crc/crc16_t10dif_copy_by4.asm
+-rw-r--r--   0 runner    (1001) docker     (123)    14753 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/crc/crc16_t10dif_copy_by4_02.asm
+-rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/crc/crc16_t10dif_copy_perf.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/crc/crc16_t10dif_copy_test.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3823 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/crc/crc16_t10dif_op_perf.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/crc/crc16_t10dif_perf.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5646 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/crc/crc16_t10dif_test.c
+-rw-r--r--   0 runner    (1001) docker     (123)     9117 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/crc/crc32_funcs_test.c
+-rw-r--r--   0 runner    (1001) docker     (123)    15408 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/crc/crc32_gzip_refl_by16_10.asm
+-rw-r--r--   0 runner    (1001) docker     (123)    18522 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/crc/crc32_gzip_refl_by8.asm
+-rw-r--r--   0 runner    (1001) docker     (123)    15070 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/crc/crc32_gzip_refl_by8_02.asm
+-rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/crc/crc32_gzip_refl_perf.c
+-rw-r--r--   0 runner    (1001) docker     (123)    16265 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/crc/crc32_ieee_01.asm
+-rw-r--r--   0 runner    (1001) docker     (123)    16389 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/crc/crc32_ieee_02.asm
+-rw-r--r--   0 runner    (1001) docker     (123)    16027 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/crc/crc32_ieee_by16_10.asm
+-rw-r--r--   0 runner    (1001) docker     (123)    12342 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/crc/crc32_ieee_by4.asm
+-rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/crc/crc32_ieee_perf.c
+-rw-r--r--   0 runner    (1001) docker     (123)    26502 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/crc/crc32_iscsi_00.asm
+-rw-r--r--   0 runner    (1001) docker     (123)    17397 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/crc/crc32_iscsi_01.asm
+-rw-r--r--   0 runner    (1001) docker     (123)    15072 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/crc/crc32_iscsi_by16_10.asm
+-rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/crc/crc32_iscsi_perf.c
+-rw-r--r--   0 runner    (1001) docker     (123)    40460 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/crc/crc64_base.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/crc/crc64_ecma_norm_by16_10.asm
+-rw-r--r--   0 runner    (1001) docker     (123)    15333 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/crc/crc64_ecma_norm_by8.asm
+-rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/crc/crc64_ecma_refl_by16_10.asm
+-rw-r--r--   0 runner    (1001) docker     (123)    16984 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/crc/crc64_ecma_refl_by8.asm
+-rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/crc/crc64_example.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/crc/crc64_funcs_perf.c
+-rw-r--r--   0 runner    (1001) docker     (123)     9000 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/crc/crc64_funcs_test.c
+-rw-r--r--   0 runner    (1001) docker     (123)    14892 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/crc/crc64_iso_norm_by16_10.asm
+-rw-r--r--   0 runner    (1001) docker     (123)    15246 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/crc/crc64_iso_norm_by8.asm
+-rw-r--r--   0 runner    (1001) docker     (123)    13763 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/crc/crc64_iso_refl_by16_10.asm
+-rw-r--r--   0 runner    (1001) docker     (123)    16755 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/crc/crc64_iso_refl_by8.asm
+-rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/crc/crc64_jones_norm_by16_10.asm
+-rw-r--r--   0 runner    (1001) docker     (123)    15254 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/crc/crc64_jones_norm_by8.asm
+-rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/crc/crc64_jones_refl_by16_10.asm
+-rw-r--r--   0 runner    (1001) docker     (123)    16763 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/crc/crc64_jones_refl_by8.asm
+-rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/crc/crc64_multibinary.asm
+-rw-r--r--   0 runner    (1001) docker     (123)     4427 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/crc/crc64_ref.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15273 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/crc/crc_base.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3207 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/crc/crc_base_aliases.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8537 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/crc/crc_multibinary.asm
+-rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/crc/crc_ref.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/crc/crc_simple_test.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:29:00.895248 isal-1.2.0/src/isal/isa-l/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/doc/build.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/doc/test.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:29:00.907248 isal-1.2.0/src/isal/isa-l/erasure_code/
+-rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/erasure_code/Makefile.am
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:29:00.907248 isal-1.2.0/src/isal/isa-l/erasure_code/aarch64/
+-rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/erasure_code/aarch64/Makefile.am
+-rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/erasure_code/aarch64/ec_aarch64_dispatcher.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/erasure_code/aarch64/ec_aarch64_highlevel_func.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/erasure_code/aarch64/ec_multibinary_arm.S
+-rw-r--r--   0 runner    (1001) docker     (123)    10162 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/erasure_code/aarch64/gf_2vect_dot_prod_neon.S
+-rw-r--r--   0 runner    (1001) docker     (123)    10865 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/erasure_code/aarch64/gf_2vect_mad_neon.S
+-rw-r--r--   0 runner    (1001) docker     (123)     9087 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/erasure_code/aarch64/gf_3vect_dot_prod_neon.S
+-rw-r--r--   0 runner    (1001) docker     (123)    10267 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/erasure_code/aarch64/gf_3vect_mad_neon.S
+-rw-r--r--   0 runner    (1001) docker     (123)    10930 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/erasure_code/aarch64/gf_4vect_dot_prod_neon.S
+-rw-r--r--   0 runner    (1001) docker     (123)    12303 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/erasure_code/aarch64/gf_4vect_mad_neon.S
+-rw-r--r--   0 runner    (1001) docker     (123)    12679 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/erasure_code/aarch64/gf_5vect_dot_prod_neon.S
+-rw-r--r--   0 runner    (1001) docker     (123)    14536 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/erasure_code/aarch64/gf_5vect_mad_neon.S
+-rw-r--r--   0 runner    (1001) docker     (123)    16767 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/erasure_code/aarch64/gf_6vect_mad_neon.S
+-rw-r--r--   0 runner    (1001) docker     (123)     7696 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/erasure_code/aarch64/gf_vect_dot_prod_neon.S
+-rw-r--r--   0 runner    (1001) docker     (123)     8356 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/erasure_code/aarch64/gf_vect_mad_neon.S
+-rw-r--r--   0 runner    (1001) docker     (123)     6955 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/erasure_code/aarch64/gf_vect_mul_neon.S
+-rw-r--r--   0 runner    (1001) docker     (123)     9475 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/erasure_code/ec_base.c
+-rw-r--r--   0 runner    (1001) docker     (123)   406502 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/erasure_code/ec_base.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/erasure_code/ec_base_aliases.c
+-rw-r--r--   0 runner    (1001) docker     (123)    10380 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/erasure_code/ec_highlevel_func.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4147 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/erasure_code/ec_multibinary.asm
+-rw-r--r--   0 runner    (1001) docker     (123)     5303 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/erasure_code/erasure_code_base_perf.c
+-rw-r--r--   0 runner    (1001) docker     (123)    21974 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/erasure_code/erasure_code_base_test.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5341 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/erasure_code/erasure_code_perf.c
+-rw-r--r--   0 runner    (1001) docker     (123)    21970 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/erasure_code/erasure_code_test.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8645 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/erasure_code/erasure_code_update_perf.c
+-rw-r--r--   0 runner    (1001) docker     (123)    27553 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/erasure_code/erasure_code_update_test.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/erasure_code/gen_rs_matrix_limits.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8106 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/erasure_code/gf_2vect_dot_prod_avx.asm
+-rw-r--r--   0 runner    (1001) docker     (123)     8657 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/erasure_code/gf_2vect_dot_prod_avx2.asm
+-rw-r--r--   0 runner    (1001) docker     (123)     6505 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/erasure_code/gf_2vect_dot_prod_avx512.asm
+-rw-r--r--   0 runner    (1001) docker     (123)     8114 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/erasure_code/gf_2vect_dot_prod_sse.asm
+-rw-r--r--   0 runner    (1001) docker     (123)     6282 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/erasure_code/gf_2vect_mad_avx.asm
+-rw-r--r--   0 runner    (1001) docker     (123)     6685 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/erasure_code/gf_2vect_mad_avx2.asm
+-rw-r--r--   0 runner    (1001) docker     (123)     6300 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/erasure_code/gf_2vect_mad_avx512.asm
+-rw-r--r--   0 runner    (1001) docker     (123)     6391 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/erasure_code/gf_2vect_mad_sse.asm
+-rw-r--r--   0 runner    (1001) docker     (123)     9365 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/erasure_code/gf_3vect_dot_prod_avx.asm
+-rw-r--r--   0 runner    (1001) docker     (123)    10086 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/erasure_code/gf_3vect_dot_prod_avx2.asm
+-rw-r--r--   0 runner    (1001) docker     (123)     7308 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/erasure_code/gf_3vect_dot_prod_avx512.asm
+-rw-r--r--   0 runner    (1001) docker     (123)     9314 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/erasure_code/gf_3vect_dot_prod_sse.asm
+-rw-r--r--   0 runner    (1001) docker     (123)     8280 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/erasure_code/gf_3vect_mad_avx.asm
+-rw-r--r--   0 runner    (1001) docker     (123)     9195 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/erasure_code/gf_3vect_mad_avx2.asm
+-rw-r--r--   0 runner    (1001) docker     (123)     7000 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/erasure_code/gf_3vect_mad_avx512.asm
+-rw-r--r--   0 runner    (1001) docker     (123)     8306 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/erasure_code/gf_3vect_mad_sse.asm
+-rw-r--r--   0 runner    (1001) docker     (123)    11494 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/erasure_code/gf_4vect_dot_prod_avx.asm
+-rw-r--r--   0 runner    (1001) docker     (123)    12268 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/erasure_code/gf_4vect_dot_prod_avx2.asm
+-rw-r--r--   0 runner    (1001) docker     (123)     8311 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/erasure_code/gf_4vect_dot_prod_avx512.asm
+-rw-r--r--   0 runner    (1001) docker     (123)    11487 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/erasure_code/gf_4vect_dot_prod_sse.asm
+-rw-r--r--   0 runner    (1001) docker     (123)     9677 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/erasure_code/gf_4vect_mad_avx.asm
+-rw-r--r--   0 runner    (1001) docker     (123)    10145 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/erasure_code/gf_4vect_mad_avx2.asm
+-rw-r--r--   0 runner    (1001) docker     (123)     7647 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/erasure_code/gf_4vect_mad_avx512.asm
+-rw-r--r--   0 runner    (1001) docker     (123)     9468 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/erasure_code/gf_4vect_mad_sse.asm
+-rw-r--r--   0 runner    (1001) docker     (123)     8386 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/erasure_code/gf_5vect_dot_prod_avx.asm
+-rw-r--r--   0 runner    (1001) docker     (123)     8819 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/erasure_code/gf_5vect_dot_prod_avx2.asm
+-rw-r--r--   0 runner    (1001) docker     (123)     9392 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/erasure_code/gf_5vect_dot_prod_avx512.asm
+-rw-r--r--   0 runner    (1001) docker     (123)     8318 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/erasure_code/gf_5vect_dot_prod_sse.asm
+-rw-r--r--   0 runner    (1001) docker     (123)    10917 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/erasure_code/gf_5vect_mad_avx.asm
+-rw-r--r--   0 runner    (1001) docker     (123)    11110 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/erasure_code/gf_5vect_mad_avx2.asm
+-rw-r--r--   0 runner    (1001) docker     (123)     8341 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/erasure_code/gf_5vect_mad_avx512.asm
+-rw-r--r--   0 runner    (1001) docker     (123)    10727 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/erasure_code/gf_5vect_mad_sse.asm
+-rw-r--r--   0 runner    (1001) docker     (123)     8817 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/erasure_code/gf_6vect_dot_prod_avx.asm
+-rw-r--r--   0 runner    (1001) docker     (123)     9290 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/erasure_code/gf_6vect_dot_prod_avx2.asm
+-rw-r--r--   0 runner    (1001) docker     (123)    10053 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/erasure_code/gf_6vect_dot_prod_avx512.asm
+-rw-r--r--   0 runner    (1001) docker     (123)     8740 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/erasure_code/gf_6vect_dot_prod_sse.asm
+-rw-r--r--   0 runner    (1001) docker     (123)    11988 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/erasure_code/gf_6vect_mad_avx.asm
+-rw-r--r--   0 runner    (1001) docker     (123)    12582 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/erasure_code/gf_6vect_mad_avx2.asm
+-rw-r--r--   0 runner    (1001) docker     (123)     9329 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/erasure_code/gf_6vect_mad_avx512.asm
+-rw-r--r--   0 runner    (1001) docker     (123)    11959 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/erasure_code/gf_6vect_mad_sse.asm
+-rw-r--r--   0 runner    (1001) docker     (123)     5131 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/erasure_code/gf_inverse_test.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4424 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/erasure_code/gf_vect_dot_prod_1tbl.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6114 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/erasure_code/gf_vect_dot_prod_avx.asm
+-rw-r--r--   0 runner    (1001) docker     (123)     6397 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/erasure_code/gf_vect_dot_prod_avx2.asm
+-rw-r--r--   0 runner    (1001) docker     (123)     6165 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/erasure_code/gf_vect_dot_prod_avx512.asm
+-rw-r--r--   0 runner    (1001) docker     (123)     7380 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/erasure_code/gf_vect_dot_prod_base_test.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5054 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/erasure_code/gf_vect_dot_prod_perf.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6106 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/erasure_code/gf_vect_dot_prod_sse.asm
+-rw-r--r--   0 runner    (1001) docker     (123)    13606 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/erasure_code/gf_vect_dot_prod_test.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5156 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/erasure_code/gf_vect_mad_avx.asm
+-rw-r--r--   0 runner    (1001) docker     (123)     5400 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/erasure_code/gf_vect_mad_avx2.asm
+-rw-r--r--   0 runner    (1001) docker     (123)     5158 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/erasure_code/gf_vect_mad_avx512.asm
+-rw-r--r--   0 runner    (1001) docker     (123)     5218 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/erasure_code/gf_vect_mad_sse.asm
+-rw-r--r--   0 runner    (1001) docker     (123)    13905 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/erasure_code/gf_vect_mad_test.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4673 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/erasure_code/gf_vect_mul_avx.asm
+-rw-r--r--   0 runner    (1001) docker     (123)     4145 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/erasure_code/gf_vect_mul_base_test.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/erasure_code/gf_vect_mul_perf.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4680 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/erasure_code/gf_vect_mul_sse.asm
+-rw-r--r--   0 runner    (1001) docker     (123)     4881 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/erasure_code/gf_vect_mul_test.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:29:00.911248 isal-1.2.0/src/isal/isa-l/erasure_code/ppc64le/
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/erasure_code/ppc64le/Makefile.am
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/erasure_code/ppc64le/ec_base_vsx.c
+-rw-r--r--   0 runner    (1001) docker     (123)    14099 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/erasure_code/ppc64le/ec_base_vsx.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/erasure_code/ppc64le/gf_2vect_dot_prod_vsx.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/erasure_code/ppc64le/gf_2vect_mad_vsx.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/erasure_code/ppc64le/gf_3vect_dot_prod_vsx.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/erasure_code/ppc64le/gf_3vect_mad_vsx.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3555 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/erasure_code/ppc64le/gf_4vect_dot_prod_vsx.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/erasure_code/ppc64le/gf_4vect_mad_vsx.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4267 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/erasure_code/ppc64le/gf_5vect_dot_prod_vsx.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3950 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/erasure_code/ppc64le/gf_5vect_mad_vsx.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5024 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/erasure_code/ppc64le/gf_6vect_dot_prod_vsx.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4657 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/erasure_code/ppc64le/gf_6vect_mad_vsx.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/erasure_code/ppc64le/gf_vect_dot_prod_vsx.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/erasure_code/ppc64le/gf_vect_mad_vsx.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/erasure_code/ppc64le/gf_vect_mul_vsx.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:29:00.879248 isal-1.2.0/src/isal/isa-l/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:29:00.911248 isal-1.2.0/src/isal/isa-l/examples/ec/
+-rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/examples/ec/Makefile.am
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/examples/ec/Makefile.unx
+-rw-r--r--   0 runner    (1001) docker     (123)    13870 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/examples/ec/ec_piggyback_example.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8026 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/examples/ec/ec_simple_example.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:29:00.923249 isal-1.2.0/src/isal/isa-l/igzip/
+-rw-r--r--   0 runner    (1001) docker     (123)     5495 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/igzip/Makefile.am
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:29:00.923249 isal-1.2.0/src/isal/isa-l/igzip/aarch64/
+-rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/igzip/aarch64/bitbuf2_aarch64.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8483 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/igzip/aarch64/data_struct_aarch64.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5500 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/igzip/aarch64/encode_df.S
+-rw-r--r--   0 runner    (1001) docker     (123)     7557 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/igzip/aarch64/gen_icf_map.S
+-rw-r--r--   0 runner    (1001) docker     (123)     5865 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/igzip/aarch64/huffman_aarch64.h
+-rw-r--r--   0 runner    (1001) docker     (123)    21035 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/igzip/aarch64/igzip_decode_huffman_code_block_aarch64.S
+-rw-r--r--   0 runner    (1001) docker     (123)     8392 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/igzip/aarch64/igzip_deflate_body_aarch64.S
+-rw-r--r--   0 runner    (1001) docker     (123)     8406 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/igzip/aarch64/igzip_deflate_finish_aarch64.S
+-rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/igzip/aarch64/igzip_deflate_hash_aarch64.S
+-rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/igzip/aarch64/igzip_inflate_multibinary_arm64.S
+-rw-r--r--   0 runner    (1001) docker     (123)     4721 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/igzip/aarch64/igzip_isal_adler32_neon.S
+-rw-r--r--   0 runner    (1001) docker     (123)     5722 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/igzip/aarch64/igzip_multibinary_aarch64_dispatcher.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/igzip/aarch64/igzip_multibinary_arm64.S
+-rw-r--r--   0 runner    (1001) docker     (123)     5745 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/igzip/aarch64/igzip_set_long_icf_fg.S
+-rw-r--r--   0 runner    (1001) docker     (123)    10098 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/igzip/aarch64/isal_deflate_icf_body_hash_hist.S
+-rw-r--r--   0 runner    (1001) docker     (123)    10211 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/igzip/aarch64/isal_deflate_icf_finish_hash_hist.S
+-rw-r--r--   0 runner    (1001) docker     (123)     9433 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/igzip/aarch64/isal_update_histogram.S
+-rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/igzip/aarch64/lz0a_const_aarch64.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/igzip/aarch64/options_aarch64.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/igzip/aarch64/stdmac_aarch64.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6568 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/igzip/adler32_avx2_4.asm
+-rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/igzip/adler32_base.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/igzip/adler32_perf.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/igzip/adler32_sse.asm
+-rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/igzip/bitbuf2.asm
+-rw-r--r--   0 runner    (1001) docker     (123)     4149 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/igzip/bitbuf2.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8193 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/igzip/checksum32_funcs_test.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3849 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/igzip/checksum_test_ref.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10738 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/igzip/data_struct2.asm
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/igzip/encode_df.c
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/igzip/encode_df.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14839 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/igzip/encode_df_04.asm
+-rw-r--r--   0 runner    (1001) docker     (123)    15380 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/igzip/encode_df_06.asm
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/igzip/flatten_ll.c
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/igzip/flatten_ll.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15782 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/igzip/generate_custom_hufftables.c
+-rw-r--r--   0 runner    (1001) docker     (123)     7484 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/igzip/generate_static_inflate.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/igzip/heap_macros.asm
+-rw-r--r--   0 runner    (1001) docker     (123)    64686 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/igzip/huff_codes.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5159 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/igzip/huff_codes.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/igzip/huffman.asm
+-rw-r--r--   0 runner    (1001) docker     (123)     8316 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/igzip/huffman.h
+-rw-r--r--   0 runner    (1001) docker     (123)   379753 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/igzip/hufftables_c.c
+-rw-r--r--   0 runner    (1001) docker     (123)    60765 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/igzip/igzip.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6154 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/igzip/igzip_base.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5839 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/igzip/igzip_base_aliases.c
+-rw-r--r--   0 runner    (1001) docker     (123)    19012 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/igzip/igzip_body.asm
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/igzip/igzip_build_hash_table_perf.c
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/igzip/igzip_checksums.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10827 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/igzip/igzip_compare_types.asm
+-rw-r--r--   0 runner    (1001) docker     (123)    22135 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/igzip/igzip_decode_block_stateless.asm
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/igzip/igzip_decode_block_stateless_01.asm
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/igzip/igzip_decode_block_stateless_04.asm
+-rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/igzip/igzip_deflate_hash.asm
+-rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/igzip/igzip_example.c
+-rw-r--r--   0 runner    (1001) docker     (123)     9332 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/igzip/igzip_file_perf.c
+-rw-r--r--   0 runner    (1001) docker     (123)     9236 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/igzip/igzip_finish.asm
+-rw-r--r--   0 runner    (1001) docker     (123)    20586 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/igzip/igzip_gen_icf_map_lh1_04.asm
+-rw-r--r--   0 runner    (1001) docker     (123)    15185 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/igzip/igzip_gen_icf_map_lh1_06.asm
+-rw-r--r--   0 runner    (1001) docker     (123)     3950 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/igzip/igzip_hist_perf.c
+-rw-r--r--   0 runner    (1001) docker     (123)    10312 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/igzip/igzip_icf_base.c
+-rw-r--r--   0 runner    (1001) docker     (123)    10360 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/igzip/igzip_icf_body.c
+-rw-r--r--   0 runner    (1001) docker     (123)    21600 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/igzip/igzip_icf_body_h1_gr_bt.asm
+-rw-r--r--   0 runner    (1001) docker     (123)     8691 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/igzip/igzip_icf_finish.asm
+-rw-r--r--   0 runner    (1001) docker     (123)    76698 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/igzip/igzip_inflate.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/igzip/igzip_inflate_multibinary.asm
+-rw-r--r--   0 runner    (1001) docker     (123)     8840 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/igzip/igzip_inflate_test.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/igzip/igzip_level_buf_structs.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6308 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/igzip/igzip_multibinary.asm
+-rw-r--r--   0 runner    (1001) docker     (123)    22446 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/igzip/igzip_perf.c
+-rw-r--r--   0 runner    (1001) docker     (123)    80528 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/igzip/igzip_rand_test.c
+-rw-r--r--   0 runner    (1001) docker     (123)     9326 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/igzip/igzip_semi_dyn_file_perf.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8046 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/igzip/igzip_set_long_icf_fg_04.asm
+-rw-r--r--   0 runner    (1001) docker     (123)     9836 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/igzip/igzip_set_long_icf_fg_06.asm
+-rw-r--r--   0 runner    (1001) docker     (123)     2981 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/igzip/igzip_sync_flush_example.c
+-rw-r--r--   0 runner    (1001) docker     (123)    14353 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/igzip/igzip_update_histogram.asm
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/igzip/igzip_update_histogram_01.asm
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/igzip/igzip_update_histogram_04.asm
+-rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/igzip/igzip_wrapper.h
+-rw-r--r--   0 runner    (1001) docker     (123)    20453 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/igzip/igzip_wrapper_hdr_test.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5879 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/igzip/inflate_data_structs.asm
+-rw-r--r--   0 runner    (1001) docker     (123)    57015 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/igzip/inflate_std_vects.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/igzip/lz0a_const.asm
+-rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/igzip/options.asm
+-rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/igzip/proc_heap.asm
+-rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/igzip/proc_heap_base.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/igzip/repeated_char_result.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5044 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/igzip/rfc1951_lookup.asm
+-rw-r--r--   0 runner    (1001) docker     (123)   142279 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/igzip/static_inflate.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10063 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/igzip/stdmac.asm
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:29:00.927249 isal-1.2.0/src/isal/isa-l/include/
+-rw-r--r--   0 runner    (1001) docker     (123)     9912 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/include/aarch64_multibinary.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7052 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/include/crc.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8849 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/include/crc64.h
+-rw-r--r--   0 runner    (1001) docker     (123)    38530 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/include/erasure_code.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6108 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/include/gf_vect_mul.h
+-rw-r--r--   0 runner    (1001) docker     (123)    44454 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/include/igzip_lib.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/include/mem_routines.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11018 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/include/multibinary.asm
+-rw-r--r--   0 runner    (1001) docker     (123)    10414 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/include/raid.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7433 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/include/reg_sizes.asm
+-rw-r--r--   0 runner    (1001) docker     (123)     7815 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/include/test.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/include/types.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/include/unaligned.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/isa-l.def
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/libisal.pc.in
+-rw-r--r--   0 runner    (1001) docker     (123)    12362 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/make.inc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:29:00.927249 isal-1.2.0/src/isal/isa-l/mem/
+-rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/mem/Makefile.am
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:29:00.927249 isal-1.2.0/src/isal/isa-l/mem/aarch64/
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/mem/aarch64/Makefile.am
+-rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/mem/aarch64/mem_aarch64_dispatcher.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/mem/aarch64/mem_multibinary_arm.S
+-rw-r--r--   0 runner    (1001) docker     (123)     5432 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/mem/aarch64/mem_zero_detect_neon.S
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/mem/mem_multibinary.asm
+-rw-r--r--   0 runner    (1001) docker     (123)     4356 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/mem/mem_zero_detect_avx.asm
+-rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/mem/mem_zero_detect_base.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/mem/mem_zero_detect_base_aliases.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/mem/mem_zero_detect_perf.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/mem/mem_zero_detect_sse.asm
+-rw-r--r--   0 runner    (1001) docker     (123)     5984 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/mem/mem_zero_detect_test.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:29:00.927249 isal-1.2.0/src/isal/isa-l/programs/
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/programs/Makefile.am
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/programs/igzip.1
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/programs/igzip.1.h2m
+-rw-r--r--   0 runner    (1001) docker     (123)    30935 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/programs/igzip_cli.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7084 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/programs/igzip_cli_check.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:29:00.931249 isal-1.2.0/src/isal/isa-l/raid/
+-rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/raid/Makefile.am
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:29:00.931249 isal-1.2.0/src/isal/isa-l/raid/aarch64/
+-rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/raid/aarch64/Makefile.am
+-rw-r--r--   0 runner    (1001) docker     (123)     9158 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/raid/aarch64/pq_check_neon.S
+-rw-r--r--   0 runner    (1001) docker     (123)     7847 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/raid/aarch64/pq_gen_neon.S
+-rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/raid/aarch64/raid_aarch64_dispatcher.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/raid/aarch64/raid_multibinary_arm.S
+-rw-r--r--   0 runner    (1001) docker     (123)     7054 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/raid/aarch64/xor_check_neon.S
+-rw-r--r--   0 runner    (1001) docker     (123)     7034 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/raid/aarch64/xor_gen_neon.S
+-rw-r--r--   0 runner    (1001) docker     (123)     8117 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/raid/pq_check_sse.asm
+-rw-r--r--   0 runner    (1001) docker     (123)     7801 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/raid/pq_check_sse_i32.asm
+-rw-r--r--   0 runner    (1001) docker     (123)     8407 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/raid/pq_check_test.c
+-rw-r--r--   0 runner    (1001) docker     (123)     7640 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/raid/pq_gen_avx.asm
+-rw-r--r--   0 runner    (1001) docker     (123)     7724 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/raid/pq_gen_avx2.asm
+-rw-r--r--   0 runner    (1001) docker     (123)     6981 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/raid/pq_gen_avx512.asm
+-rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/raid/pq_gen_perf.c
+-rw-r--r--   0 runner    (1001) docker     (123)     7628 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/raid/pq_gen_sse.asm
+-rw-r--r--   0 runner    (1001) docker     (123)     7371 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/raid/pq_gen_sse_i32.asm
+-rw-r--r--   0 runner    (1001) docker     (123)     5043 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/raid/pq_gen_test.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/raid/raid_base.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/raid/raid_base_aliases.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/raid/raid_multibinary.asm
+-rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/raid/raid_multibinary_i32.asm
+-rw-r--r--   0 runner    (1001) docker     (123)     6911 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/raid/xor_check_sse.asm
+-rw-r--r--   0 runner    (1001) docker     (123)     7859 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/raid/xor_check_test.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/raid/xor_example.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6012 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/raid/xor_gen_avx.asm
+-rw-r--r--   0 runner    (1001) docker     (123)     5787 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/raid/xor_gen_avx512.asm
+-rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/raid/xor_gen_perf.c
+-rw-r--r--   0 runner    (1001) docker     (123)     7110 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/raid/xor_gen_sse.asm
+-rw-r--r--   0 runner    (1001) docker     (123)     4404 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/raid/xor_gen_test.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:29:00.879248 isal-1.2.0/src/isal/isa-l/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:29:00.935249 isal-1.2.0/src/isal/isa-l/tests/fuzz/
+-rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/tests/fuzz/Makefile.am
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/tests/fuzz/Makefile.unx
+-rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/tests/fuzz/igzip_checked_inflate_fuzz_test.c
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/tests/fuzz/igzip_dump_inflate_corpus.c
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/tests/fuzz/igzip_fuzz_inflate.c
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/tests/fuzz/igzip_simple_inflate_fuzz_test.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3516 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/tests/fuzz/igzip_simple_round_trip_fuzz_test.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:29:00.935249 isal-1.2.0/src/isal/isa-l/tools/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2424 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/tools/check_format.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     6408 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/tools/gen_nmake.mk
+-rwxr-xr-x   0 runner    (1001) docker     (123)       54 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/tools/iindent
+-rwxr-xr-x   0 runner    (1001) docker     (123)      961 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/tools/nasm-cet-filter.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      917 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/tools/nasm-filter.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)       49 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/tools/remove_trailing_whitespace.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1297 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/tools/test_autorun.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2989 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/tools/test_checks.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5765 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/tools/test_extended.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4608 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/tools/test_fuzz.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      148 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/tools/test_tools.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      851 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/tools/yasm-cet-filter.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      807 2023-07-21 12:22:14.000000 isal-1.2.0/src/isal/isa-l/tools/yasm-filter.sh
+-rw-r--r--   0 runner    (1001) docker     (123)    12553 2023-07-21 12:22:12.000000 isal-1.2.0/src/isal/isal_shared.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-07-21 12:22:12.000000 isal-1.2.0/src/isal/isal_zlib.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    41038 2023-07-21 12:22:12.000000 isal-1.2.0/src/isal/isal_zlibmodule.c
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-21 12:22:12.000000 isal-1.2.0/src/isal/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:29:00.879248 isal-1.2.0/src/isal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8675 2023-07-21 12:29:00.000000 isal-1.2.0/src/isal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17909 2023-07-21 12:29:00.000000 isal-1.2.0/src/isal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 12:29:00.000000 isal-1.2.0/src/isal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 12:29:00.000000 isal-1.2.0/src/isal.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-21 12:29:00.000000 isal-1.2.0/src/isal.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:29:00.935249 isal-1.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7318 2023-07-21 12:22:12.000000 isal-1.2.0/tests/test_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34314 2023-07-21 12:22:12.000000 isal-1.2.0/tests/test_gzip_compliance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15131 2023-07-21 12:22:12.000000 isal-1.2.0/tests/test_igzip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9987 2023-07-21 12:22:12.000000 isal-1.2.0/tests/test_igzip_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37116 2023-07-21 12:22:12.000000 isal-1.2.0/tests/test_zlib_compliance.py
```

### Comparing `isal-1.1.0/LICENSE` & `isal-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/PKG-INFO` & `isal-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: isal
-Version: 1.1.0
+Version: 1.2.0
 Summary: Faster zlib and gzip compatible compression and decompression by providing python bindings for the ISA-L library.
 Home-page: https://github.com/pycompression/python-isal
 Author: Leiden University Medical Center
 Author-email: r.h.p.vorderman@lumc.nl
 License: PSF-2.0
 Keywords: isal isa-l compression deflate gzip igzip
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -136,20 +136,20 @@
 Python-isal supports a limited amount of platforms for which wheels have been
 made available. To prevent your users from running into issues when installing
 your project please list a python-isal dependency as follows.
 
 ``setup.cfg``::
 
     install_requires =
-        isal; platform.machine == "x86_64" or platform.machine == "AMD64"
+        isal; platform.machine == "x86_64" or platform.machine == "AMD64" or platform.machine == "aarch64"
 
 ``setup.py``::
 
     extras_require={
-        ":platform.machine == 'x86_64' or platform.machine == 'AMD64'": ['isal']
+        ":platform.machine == 'x86_64' or platform.machine == 'AMD64' or platform.machine == 'aarch64'": ['isal']
     },
 
 .. dependency end
 
 Differences with zlib and gzip modules
 --------------------------------------
```

### Comparing `isal-1.1.0/README.rst` & `isal-1.2.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -107,20 +107,20 @@
 Python-isal supports a limited amount of platforms for which wheels have been
 made available. To prevent your users from running into issues when installing
 your project please list a python-isal dependency as follows.
 
 ``setup.cfg``::
 
     install_requires =
-        isal; platform.machine == "x86_64" or platform.machine == "AMD64"
+        isal; platform.machine == "x86_64" or platform.machine == "AMD64" or platform.machine == "aarch64"
 
 ``setup.py``::
 
     extras_require={
-        ":platform.machine == 'x86_64' or platform.machine == 'AMD64'": ['isal']
+        ":platform.machine == 'x86_64' or platform.machine == 'AMD64' or platform.machine == 'aarch64'": ['isal']
     },
 
 .. dependency end
 
 Differences with zlib and gzip modules
 --------------------------------------
```

### Comparing `isal-1.1.0/setup.py` & `isal-1.2.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 # Copyright (c) 2001, 2002, 2003, 2004, 2005, 2006, 2007, 2008, 2009, 2010,
 # 2011, 2012, 2013, 2014, 2015, 2016, 2017, 2018, 2019, 2020, 2021, 2022
 # Python Software Foundation; All Rights Reserved
 
 # This file is part of python-isal which is distributed under the
 # PYTHON SOFTWARE FOUNDATION LICENSE VERSION 2.
 
-import copy
 import functools
 import os
+import platform
 import shutil
 import subprocess
 import sys
 import tempfile
 from pathlib import Path
 
 from setuptools import Extension, find_packages, setup
@@ -68,104 +68,78 @@
                 ext.libraries = ["isal"]  # libisal.so*
             elif SYSTEM_IS_WINDOWS:
                 ext.libraries = ["isa-l"]  # isa-l.dll
             else:
                 raise NotImplementedError(
                     f"Unsupported platform: {sys.platform}")
         else:
-            if self.compiler.compiler_type == "msvc":
-                compiler = copy.deepcopy(self.compiler)
-                if not compiler.initialized:
-                    compiler.initialize()
-                compiler_command = f'"{compiler.cc}"'
-                compiler_args = compiler.compile_options
-            elif self.compiler.compiler_type == "unix":
-                compiler_command = self.compiler.compiler[0]
-                compiler_args = self.compiler.compiler[1:]
-            else:
-                raise NotImplementedError("Unknown compiler")
-            isa_l_prefix_dir = build_isa_l(compiler_command,
-                                           " ".join(compiler_args))
+            isa_l_build_dir = build_isa_l()
             if SYSTEM_IS_UNIX:
                 ext.extra_objects = [
-                    os.path.join(isa_l_prefix_dir, "lib", "libisal.a")]
+                    os.path.join(isa_l_build_dir, "bin", "isa-l.a")]
             elif SYSTEM_IS_WINDOWS:
                 ext.extra_objects = [
-                    os.path.join(isa_l_prefix_dir, "isa-l_static.lib")]
+                    os.path.join(isa_l_build_dir, "isa-l_static.lib")]
             else:
                 raise NotImplementedError(
                     f"Unsupported platform: {sys.platform}")
-            ext.include_dirs = [os.path.join(isa_l_prefix_dir,
-                                             "include")]
-            # -fPIC needed for proper static linking
-            ext.extra_compile_args = ["-fPIC"]
+            ext.include_dirs = [isa_l_build_dir]
         super().build_extension(ext)
 
 
 # Use a cache to prevent isa-l from being build twice. According to the
 # functools docs lru_cache with maxsize None is faster. The shortcut called
 # 'cache' is only available from python 3.9 onwards.
 # see: https://docs.python.org/3/library/functools.html#functools.cache
 @functools.lru_cache(maxsize=None)
-def build_isa_l(compiler_command: str, compiler_options: str):
+def build_isa_l():
     # Check for cache
     if BUILD_CACHE:
         if BUILD_CACHE_FILE.exists():
             cache_path = Path(BUILD_CACHE_FILE.read_text())
-            if (cache_path / "include" / "isa-l").exists():
+            if (cache_path / "isa-l.h").exists():
                 return str(cache_path)
 
     # Creating temporary directories
     build_dir = tempfile.mktemp()
-    temp_prefix = tempfile.mkdtemp()
     shutil.copytree(ISA_L_SOURCE, build_dir)
 
     # Build environment is a copy of OS environment to allow user to influence
     # it.
     build_env = os.environ.copy()
-    # Add -fPIC flag to allow static compilation
-    build_env["CC"] = compiler_command
     if SYSTEM_IS_UNIX:
-        build_env["CFLAGS"] = compiler_options + " -fPIC"
-    elif SYSTEM_IS_WINDOWS:
-        # The nmake file has CLFAGS_REL for all the compiler options.
-        # This is added to CFLAGS with all the necessary include options.
-        build_env["CFLAGS_REL"] = compiler_options
+        build_env["CFLAGS"] = build_env.get("CFLAGS", "") + " -fPIC"
     if hasattr(os, "sched_getaffinity"):
         cpu_count = len(os.sched_getaffinity(0))
     else:  # sched_getaffinity not available on all platforms
         cpu_count = os.cpu_count() or 1  # os.cpu_count() can return None
     run_args = dict(cwd=build_dir, env=build_env)
     if SYSTEM_IS_UNIX:
-        subprocess.run(os.path.join(build_dir, "autogen.sh"), **run_args)
-        subprocess.run([os.path.join(build_dir, "configure"),
-                        "--prefix", temp_prefix], **run_args)
-        subprocess.run(["make", "-j", str(cpu_count)], **run_args)
-        subprocess.run(["make", "-j", str(cpu_count), "install"], **run_args)
+        if platform.machine() == "aarch64":
+            cflags_param = "CFLAGS_aarch64"
+        else:
+            cflags_param = "CFLAGS_"
+        subprocess.run(["make", "-j", str(cpu_count), "-f", "Makefile.unx",
+                        "isa-l.h", "bin/isa-l.a",
+                        f"{cflags_param}={build_env.get('CFLAGS', '')}"],
+                       **run_args)
     elif SYSTEM_IS_WINDOWS:
-        subprocess.run(["nmake", "/E", "/f", "Makefile.nmake"], **run_args)
-        Path(temp_prefix, "include").mkdir()
-        print(temp_prefix, file=sys.stderr)
-        shutil.copytree(os.path.join(build_dir, "include"),
-                        Path(temp_prefix, "include", "isa-l"))
-        shutil.copy(os.path.join(build_dir, "isa-l_static.lib"),
-                    os.path.join(temp_prefix, "isa-l_static.lib"))
-        shutil.copy(os.path.join(build_dir, "isa-l.h"),
-                    os.path.join(temp_prefix, "include", "isa-l.h"))
+        subprocess.run(["nmake", "/f", "Makefile.nmake"], **run_args)
     else:
         raise NotImplementedError(f"Unsupported platform: {sys.platform}")
-    shutil.rmtree(build_dir)
+    shutil.copytree(os.path.join(build_dir, "include"),
+                    os.path.join(build_dir, "isa-l"))
     if BUILD_CACHE:
-        BUILD_CACHE_FILE.write_text(temp_prefix)
-    return temp_prefix
+        BUILD_CACHE_FILE.write_text(build_dir)
+    return build_dir
 
 
 setup(
     name="isal",
-    version="1.1.0",
+    version="1.2.0",
     description="Faster zlib and gzip compatible compression and "
                 "decompression by providing python bindings for the ISA-L "
                 "library.",
     author="Leiden University Medical Center",
     author_email="r.h.p.vorderman@lumc.nl",  # A placeholder for now
     long_description=Path("README.rst").read_text(),
     long_description_content_type="text/x-rst",
```

### Comparing `isal-1.1.0/src/isal/__init__.py` & `isal-1.2.0/src/isal/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,8 +23,8 @@
     "ISAL_MAJOR_VERSION",
     "ISAL_MINOR_VERSION",
     "ISAL_PATCH_VERSION",
     "ISAL_VERSION",
     "__version__"
 ]
 
-__version__ = "1.1.0"
+__version__ = "1.2.0"
```

### Comparing `isal-1.1.0/src/isal/_isalmodule.c` & `isal-1.2.0/src/isal/_isalmodule.c`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/igzip.py` & `isal-1.2.0/src/isal/igzip.py`

 * *Files 2% similar despite different names*

```diff
@@ -216,14 +216,30 @@
             self.fileobj.write(self.compress.compress(data))
             self.size += length
             self.crc = isal_zlib.crc32(data, self.crc)
             self.offset += length
         return length
 
 
+def detect_bgzip(header: bytes) -> bool:
+    if len(header) < 18:
+        return False
+    magic, method, flags, mtime, xfl, os, xlen, si1, si2, slen, bsize = \
+        struct.unpack("<HBBIBBHBBHH", header[:18])
+    return (
+            method == 8 and  # Deflate method used
+            flags & 4 and    # There are extra fields
+            xlen == 6 and    # The extra field should be of length 6
+            si1 == 66 and    # BGZIP magic number one
+            si2 == 67 and    # BGZIP magic number two
+            slen == 2        # The length of the 16 bit integer that stores
+                             # the size of the block
+    )
+
+
 class _PaddedFile(gzip._PaddedFile):
     # Overwrite _PaddedFile from gzip as its prepend method assumes that
     # the prepended data is always read from its _buffer. Unfortunately in
     # isal_zlib.decompressobj there is a bitbuffer as well which may be added.
     # So an extra check is added to prepend to ensure no extra data in front
     # of the buffer was present. (Negative self._read).
     def prepend(self, prepend=b''):
@@ -245,14 +261,23 @@
         # It is not very invasive and allows us to override _PaddedFile
         _compression.DecompressReader.__init__(
             self, _PaddedFile(fp), igzip_lib.IgzipDecompressor,
             hist_bits=igzip_lib.MAX_HIST_BITS, flag=igzip_lib.DECOMP_DEFLATE)
         # Set flag indicating start of a new member
         self._new_member = True
         self._last_mtime = None
+        self._read_buffer_size = READ_BUFFER_SIZE
+        if hasattr(fp, "peek") and detect_bgzip(fp.peek(18)):
+            # bgzip consists of puny little blocks of max 64K uncompressed data
+            # so in practice probably more around 16K in compressed size. A
+            # 128K buffer is a massive overshoot and slows down the
+            # decompression.
+            # bgzip stores the block size, so it can be unpacked more
+            # efficiently but this is outside scope for python-isal.
+            self._read_buffer_size = 16 * 1024
 
     def read(self, size=-1):
         if size < 0:
             return self.readall()
         # size=0 is special because decompress(max_length=0) is not supported
         if not size:
             return b""
@@ -278,15 +303,15 @@
                 if not self._read_gzip_header():
                     self._size = self._pos
                     return b""
                 self._new_member = False
 
             # Read a chunk of data from the file
             if self._decompressor.needs_input:
-                buf = self._fp.read(READ_BUFFER_SIZE)
+                buf = self._fp.read(self._read_buffer_size)
                 uncompress = self._decompressor.decompress(buf, size)
             else:
                 uncompress = self._decompressor.decompress(b"", size)
             if self._decompressor.unused_data != b"":
                 # Prepend the already read bytes to the fileobj so they can
                 # be seen by _read_eof() and _read_gzip_header()
                 self._fp.prepend(self._decompressor.unused_data)
@@ -445,17 +470,15 @@
                               help="Write to this output file")
     parser.add_argument("-n", "--no-name", action="store_true",
                         dest="reproducible",
                         help="do not save or restore the original name and "
                              "timestamp")
     parser.add_argument("-f", "--force", action="store_true",
                         help="Overwrite output without prompting")
-    # -b flag not taken by either gzip or igzip. Hidden attribute. Above 32K
-    # diminishing returns hit. _compression.BUFFER_SIZE = 8k. But 32K is about
-    # ~6% faster.
+    # -b flag not taken by either gzip or igzip. Hidden attribute.
     parser.add_argument("-b", "--buffer-size",
                         default=READ_BUFFER_SIZE, type=int,
                         help=argparse.SUPPRESS)
     return parser
 
 
 def main():
```

### Comparing `isal-1.1.0/src/isal/igzip_lib.pyi` & `isal-1.2.0/src/isal/igzip_lib.pyi`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/igzip_libmodule.c` & `isal-1.2.0/src/isal/igzip_libmodule.c`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,16 @@
   clinic.
 */
 
 #include "isal_shared.h"
 
 typedef struct {
     PyObject_HEAD
-    PyObject *unused_data;
+    PyObject *unused_data;    
+    PyThread_type_lock lock;
     PyObject *zdict;
     uint8_t *input_buffer;
     Py_ssize_t input_buffer_size;
     /* inflate_state>avail_in is only 32 bit, so we store the true length
        separately. Conversion and looping is encapsulated in
        decompress_buf() */
     Py_ssize_t avail_in_real;
@@ -37,20 +38,47 @@
        the end of the IgzipDecompressor so members can be accessed easily. */
     struct inflate_state state;
 } IgzipDecompressor;
 
 static void
 IgzipDecompressor_dealloc(IgzipDecompressor *self)
 {
+    PyThread_free_lock(self->lock);
     PyMem_Free(self->input_buffer);
     Py_CLEAR(self->unused_data);
     Py_CLEAR(self->zdict);
     Py_TYPE(self)->tp_free((PyObject *)self);
 }
 
+
+static int
+set_inflate_zdict_IgzipDecompressor(IgzipDecompressor *self)
+{
+    Py_buffer zdict_buf;
+    if (PyObject_GetBuffer(self->zdict, &zdict_buf, PyBUF_SIMPLE) == -1) {
+        return -1;
+    }
+    if ((size_t)zdict_buf.len > UINT32_MAX) {
+        PyErr_SetString(PyExc_OverflowError,
+                        "zdict length does not fit in an unsigned 32-bit integer");
+        PyBuffer_Release(&zdict_buf);
+        return -1;
+    }
+    int err;
+    err = isal_inflate_set_dict(&self->state,
+                                zdict_buf.buf, (uint32_t)zdict_buf.len);
+    PyBuffer_Release(&zdict_buf);
+    if (err != ISAL_DECOMP_OK) {
+        isal_inflate_error(err);
+        return -1;
+    }
+    return 0;
+}
+
+
 /* Decompress data of length d->bzs_avail_in_real in d->state.next_in.  The output
    buffer is allocated dynamically and returned.  At most max_length bytes are
    returned, so some of the input may not be consumed. d->state.next_in and
    d->bzs_avail_in_real are updated to reflect the consumed input. */
 static PyObject*
 decompress_buf(IgzipDecompressor *self, Py_ssize_t max_length)
 {
@@ -95,21 +123,40 @@
                 PyErr_SetString(PyExc_MemoryError, 
                                 "Unsufficient memory for buffer allocation");
                 goto error;
             }
             else if (obuflen == -2)
                 break;
         
+            Py_BEGIN_ALLOW_THREADS;
             err = isal_inflate(&(self->state));
-            if (err != ISAL_DECOMP_OK){
-                isal_inflate_error(err);
-                goto error;
+            Py_END_ALLOW_THREADS;
+
+            switch(err) {
+                case ISAL_DECOMP_OK:
+                    break;
+                case ISAL_NEED_DICT:                
+                    if  (self->zdict != NULL) {
+                        if (set_inflate_zdict_IgzipDecompressor(self) < 0) {
+                            goto error;
+                        }
+                        else 
+                            break;
+                    }
+                    else {
+                        isal_inflate_error(err);
+                        goto error;
+                    }
+                default:
+                    isal_inflate_error(err);
+                    goto error;
             }
-        } while (self->state.avail_out == 0 && 
-                 self->state.block_state != ISAL_BLOCK_FINISH);
+
+        } while (self->state.avail_out == 0 || err == ISAL_NEED_DICT);
+    
     } while(self->avail_in_real != 0 && 
             self->state.block_state != ISAL_BLOCK_FINISH);
 
     if (self->state.block_state == ISAL_BLOCK_FINISH)
         self->eof = 1;
 
     self->avail_in_real += self->state.avail_in;
@@ -353,26 +400,31 @@
 static PyObject *
 igzip_lib_IgzipDecompressor_decompress(IgzipDecompressor *self, 
                                        PyObject *args, 
                                        PyObject *kwargs)
 {
     static char *keywords[] = {"", "max_length", NULL};
     static char *format = "y*|n:decompress";
+
+    PyObject *result = NULL;
     Py_buffer data = {NULL, NULL};
     Py_ssize_t max_length = -1;
 
     if (!PyArg_ParseTupleAndKeywords(
             args, kwargs, format, keywords, &data, &max_length)) {
         return NULL;
     }
-    PyObject *result = NULL;
-    if (self->eof)
+    ENTER_ZLIB(self);
+    if (self->eof) {
         PyErr_SetString(PyExc_EOFError, "End of stream already reached");
-    else
+    }
+    else {
         result = decompress(self, data.buf, data.len, max_length);
+    }
+    LEAVE_ZLIB(self);
     PyBuffer_Release(&data);
     return result;
 }
 
 PyDoc_STRVAR(igzip_lib_IgzipDecompressor___init____doc__,
 "IgzipDecompressor(flag=0, hist_bits=15, zdict=b\'\')\n"
 "--\n"
@@ -400,50 +452,39 @@
     PyObject *zdict = NULL;
 
     if (!PyArg_ParseTupleAndKeywords(
             args, kwargs, format, keywords, &flag, &hist_bits, &zdict)) {
         return NULL;
     }
     IgzipDecompressor *self = PyObject_New(IgzipDecompressor, type); 
-    int err;
     self->eof = 0;
     self->needs_input = 1;
     self->avail_in_real = 0;
     self->input_buffer = NULL;
     self->input_buffer_size = 0;
     self->zdict = zdict;
     self->unused_data = PyBytes_FromStringAndSize(NULL, 0);
     if (self->unused_data == NULL) {
         Py_CLEAR(self);
         return NULL;
     }
+    self->lock = PyThread_allocate_lock();
+    if (self->lock == NULL) {
+        Py_DECREF(self);
+        PyErr_SetString(PyExc_MemoryError, "Unable to allocate lock");
+        return NULL;
+    }
     isal_inflate_init(&(self->state));
     self->state.hist_bits = hist_bits;
     self->state.crc_flag = flag;
     if (self->zdict != NULL){
-        Py_buffer zdict_buf;
-        if (PyObject_GetBuffer(self->zdict, &zdict_buf, PyBUF_SIMPLE) == -1) {
-                Py_CLEAR(self);
-                return NULL;
-        }
-        if ((size_t)zdict_buf.len > UINT32_MAX) {
-            PyErr_SetString(PyExc_OverflowError,
-                           "zdict length does not fit in an unsigned 32-bits int");
-            PyBuffer_Release(&zdict_buf);
+        if (set_inflate_zdict_IgzipDecompressor(self) < 0) {
             Py_CLEAR(self);
             return NULL;
         }
-        err = isal_inflate_set_dict(&(self->state), zdict_buf.buf, 
-                                    (uint32_t)zdict_buf.len);
-        PyBuffer_Release(&zdict_buf);
-        if (err != ISAL_DECOMP_OK) {
-            isal_inflate_error(err);
-            Py_CLEAR(self);
-            return NULL;
-        }        
     }
     return (PyObject *)self;
 }
 
 static PyMethodDef IgzipDecompressor_methods[] = {
     IGZIP_LIB_IGZIPDECOMPRESSOR_DECOMPRESS_METHODDEF,
     {NULL}
```

### Comparing `isal-1.1.0/src/isal/isa-l/.travis.yml` & `isal-1.2.0/src/isal/isa-l/.travis.yml`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/CONTRIBUTING.md` & `isal-1.2.0/src/isal/isa-l/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/Doxyfile` & `isal-1.2.0/src/isal/isa-l/Doxyfile`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/LICENSE` & `isal-1.2.0/src/isal/isa-l/LICENSE`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/Makefile.am` & `isal-1.2.0/src/isal/isa-l/Makefile.am`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/Makefile.nmake` & `isal-1.2.0/src/isal/isa-l/Makefile.nmake`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/Makefile.unx` & `isal-1.2.0/src/isal/isa-l/Makefile.unx`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/README.md` & `isal-1.2.0/src/isal/isa-l/README.md`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/Release_notes.txt` & `isal-1.2.0/src/isal/isa-l/Release_notes.txt`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/configure.ac` & `isal-1.2.0/src/isal/isa-l/configure.ac`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/crc/Makefile.am` & `isal-1.2.0/src/isal/isa-l/crc/Makefile.am`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/crc/aarch64/Makefile.am` & `isal-1.2.0/src/isal/isa-l/crc/aarch64/Makefile.am`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/crc/aarch64/crc16_t10dif_copy_pmull.S` & `isal-1.2.0/src/isal/isa-l/crc/aarch64/crc16_t10dif_copy_pmull.S`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/crc/aarch64/crc16_t10dif_pmull.S` & `isal-1.2.0/src/isal/isa-l/crc/aarch64/crc16_t10dif_pmull.S`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/crc/aarch64/crc32_aarch64_common.h` & `isal-1.2.0/src/isal/isa-l/crc/aarch64/crc32_aarch64_common.h`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/crc/aarch64/crc32_common_crc_ext_cortex_a72.S` & `isal-1.2.0/src/isal/isa-l/crc/aarch64/crc32_common_crc_ext_cortex_a72.S`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/crc/aarch64/crc32_common_mix_neoverse_n1.S` & `isal-1.2.0/src/isal/isa-l/crc/aarch64/crc32_common_mix_neoverse_n1.S`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/crc/aarch64/crc32_gzip_refl_3crc_fold.S` & `isal-1.2.0/src/isal/isa-l/crc/aarch64/crc32_gzip_refl_3crc_fold.S`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/crc/aarch64/crc32_gzip_refl_crc_ext.S` & `isal-1.2.0/src/isal/isa-l/crc/aarch64/crc32_gzip_refl_crc_ext.S`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/crc/aarch64/crc32_gzip_refl_pmull.S` & `isal-1.2.0/src/isal/isa-l/crc/aarch64/crc32_gzip_refl_pmull.S`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/crc/aarch64/crc32_gzip_refl_pmull.h` & `isal-1.2.0/src/isal/isa-l/crc/aarch64/crc32_gzip_refl_pmull.h`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/crc/aarch64/crc32_ieee_norm_pmull.S` & `isal-1.2.0/src/isal/isa-l/crc/aarch64/crc32_ieee_norm_pmull.S`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/crc/aarch64/crc32_ieee_norm_pmull.h` & `isal-1.2.0/src/isal/isa-l/crc/aarch64/crc32_ieee_norm_pmull.h`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/crc/aarch64/crc32_iscsi_3crc_fold.S` & `isal-1.2.0/src/isal/isa-l/crc/aarch64/crc32_iscsi_3crc_fold.S`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/crc/aarch64/crc32_iscsi_crc_ext.S` & `isal-1.2.0/src/isal/isa-l/crc/aarch64/crc32_iscsi_crc_ext.S`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/crc/aarch64/crc32_iscsi_refl_pmull.S` & `isal-1.2.0/src/isal/isa-l/crc/aarch64/crc32_iscsi_refl_pmull.S`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/crc/aarch64/crc32_iscsi_refl_pmull.h` & `isal-1.2.0/src/isal/isa-l/crc/aarch64/crc32_iscsi_refl_pmull.h`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/crc/aarch64/crc32_mix_default.S` & `isal-1.2.0/src/isal/isa-l/crc/aarch64/crc32_mix_default.S`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/crc/aarch64/crc32_mix_default_common.S` & `isal-1.2.0/src/isal/isa-l/crc/aarch64/crc32_mix_default_common.S`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/crc/aarch64/crc32_mix_neoverse_n1.S` & `isal-1.2.0/src/isal/isa-l/crc/aarch64/crc32_mix_neoverse_n1.S`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/crc/aarch64/crc32_norm_common_pmull.h` & `isal-1.2.0/src/isal/isa-l/crc/aarch64/crc32_norm_common_pmull.h`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/crc/aarch64/crc32_refl_common_pmull.h` & `isal-1.2.0/src/isal/isa-l/crc/aarch64/crc32_refl_common_pmull.h`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/crc/aarch64/crc32c_mix_default.S` & `isal-1.2.0/src/isal/isa-l/crc/aarch64/crc32c_mix_default.S`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/crc/aarch64/crc32c_mix_neoverse_n1.S` & `isal-1.2.0/src/isal/isa-l/crc/aarch64/crc32c_mix_neoverse_n1.S`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/crc/aarch64/crc64_ecma_norm_pmull.S` & `isal-1.2.0/src/isal/isa-l/crc/aarch64/crc64_ecma_norm_pmull.S`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/crc/aarch64/crc64_ecma_norm_pmull.h` & `isal-1.2.0/src/isal/isa-l/crc/aarch64/crc64_ecma_norm_pmull.h`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/crc/aarch64/crc64_ecma_refl_pmull.S` & `isal-1.2.0/src/isal/isa-l/crc/aarch64/crc64_ecma_refl_pmull.S`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/crc/aarch64/crc64_ecma_refl_pmull.h` & `isal-1.2.0/src/isal/isa-l/crc/aarch64/crc64_ecma_refl_pmull.h`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/crc/aarch64/crc64_iso_norm_pmull.S` & `isal-1.2.0/src/isal/isa-l/crc/aarch64/crc64_iso_norm_pmull.S`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/crc/aarch64/crc64_iso_norm_pmull.h` & `isal-1.2.0/src/isal/isa-l/crc/aarch64/crc64_iso_norm_pmull.h`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/crc/aarch64/crc64_iso_refl_pmull.S` & `isal-1.2.0/src/isal/isa-l/crc/aarch64/crc64_iso_refl_pmull.S`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/crc/aarch64/crc64_iso_refl_pmull.h` & `isal-1.2.0/src/isal/isa-l/crc/aarch64/crc64_iso_refl_pmull.h`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/crc/aarch64/crc64_jones_norm_pmull.S` & `isal-1.2.0/src/isal/isa-l/crc/aarch64/crc64_jones_norm_pmull.S`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/crc/aarch64/crc64_jones_norm_pmull.h` & `isal-1.2.0/src/isal/isa-l/crc/aarch64/crc64_jones_norm_pmull.h`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/crc/aarch64/crc64_jones_refl_pmull.S` & `isal-1.2.0/src/isal/isa-l/crc/aarch64/crc64_jones_refl_pmull.S`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/crc/aarch64/crc64_jones_refl_pmull.h` & `isal-1.2.0/src/isal/isa-l/crc/aarch64/crc64_jones_refl_pmull.h`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/crc/aarch64/crc64_norm_common_pmull.h` & `isal-1.2.0/src/isal/isa-l/crc/aarch64/crc64_norm_common_pmull.h`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/crc/aarch64/crc64_refl_common_pmull.h` & `isal-1.2.0/src/isal/isa-l/crc/aarch64/crc64_refl_common_pmull.h`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/crc/aarch64/crc_aarch64_dispatcher.c` & `isal-1.2.0/src/isal/isa-l/crc/aarch64/crc_aarch64_dispatcher.c`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/crc/aarch64/crc_common_pmull.h` & `isal-1.2.0/src/isal/isa-l/crc/aarch64/crc_common_pmull.h`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/crc/aarch64/crc_multibinary_arm.S` & `isal-1.2.0/src/isal/isa-l/crc/aarch64/crc_multibinary_arm.S`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/crc/crc16_t10dif_01.asm` & `isal-1.2.0/src/isal/isa-l/crc/crc16_t10dif_01.asm`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/crc/crc16_t10dif_02.asm` & `isal-1.2.0/src/isal/isa-l/crc/crc16_t10dif_02.asm`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/crc/crc16_t10dif_by16_10.asm` & `isal-1.2.0/src/isal/isa-l/crc/crc16_t10dif_by16_10.asm`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/crc/crc16_t10dif_by4.asm` & `isal-1.2.0/src/isal/isa-l/crc/crc16_t10dif_by4.asm`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/crc/crc16_t10dif_copy_by4.asm` & `isal-1.2.0/src/isal/isa-l/crc/crc16_t10dif_copy_by4.asm`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/crc/crc16_t10dif_copy_by4_02.asm` & `isal-1.2.0/src/isal/isa-l/crc/crc16_t10dif_copy_by4_02.asm`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/crc/crc16_t10dif_copy_perf.c` & `isal-1.2.0/src/isal/isa-l/crc/crc16_t10dif_copy_perf.c`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/crc/crc16_t10dif_copy_test.c` & `isal-1.2.0/src/isal/isa-l/crc/crc16_t10dif_copy_test.c`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/crc/crc16_t10dif_op_perf.c` & `isal-1.2.0/src/isal/isa-l/crc/crc16_t10dif_op_perf.c`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/crc/crc16_t10dif_perf.c` & `isal-1.2.0/src/isal/isa-l/crc/crc16_t10dif_perf.c`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/crc/crc16_t10dif_test.c` & `isal-1.2.0/src/isal/isa-l/crc/crc16_t10dif_test.c`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/crc/crc32_funcs_test.c` & `isal-1.2.0/src/isal/isa-l/crc/crc32_funcs_test.c`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/crc/crc32_gzip_refl_by16_10.asm` & `isal-1.2.0/src/isal/isa-l/crc/crc32_gzip_refl_by16_10.asm`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/crc/crc32_gzip_refl_by8.asm` & `isal-1.2.0/src/isal/isa-l/crc/crc32_gzip_refl_by8.asm`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/crc/crc32_gzip_refl_by8_02.asm` & `isal-1.2.0/src/isal/isa-l/crc/crc32_gzip_refl_by8_02.asm`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/crc/crc32_gzip_refl_perf.c` & `isal-1.2.0/src/isal/isa-l/crc/crc32_gzip_refl_perf.c`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/crc/crc32_ieee_01.asm` & `isal-1.2.0/src/isal/isa-l/crc/crc32_ieee_01.asm`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/crc/crc32_ieee_02.asm` & `isal-1.2.0/src/isal/isa-l/crc/crc32_ieee_02.asm`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/crc/crc32_ieee_by16_10.asm` & `isal-1.2.0/src/isal/isa-l/crc/crc32_ieee_by16_10.asm`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/crc/crc32_ieee_by4.asm` & `isal-1.2.0/src/isal/isa-l/crc/crc32_ieee_by4.asm`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/crc/crc32_ieee_perf.c` & `isal-1.2.0/src/isal/isa-l/crc/crc32_ieee_perf.c`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/crc/crc32_iscsi_00.asm` & `isal-1.2.0/src/isal/isa-l/crc/crc32_iscsi_00.asm`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/crc/crc32_iscsi_01.asm` & `isal-1.2.0/src/isal/isa-l/crc/crc32_iscsi_01.asm`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/crc/crc32_iscsi_by16_10.asm` & `isal-1.2.0/src/isal/isa-l/crc/crc32_iscsi_by16_10.asm`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/crc/crc32_iscsi_perf.c` & `isal-1.2.0/src/isal/isa-l/crc/crc32_iscsi_perf.c`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/crc/crc64_base.c` & `isal-1.2.0/src/isal/isa-l/crc/crc64_base.c`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/crc/crc64_ecma_norm_by16_10.asm` & `isal-1.2.0/src/isal/isa-l/crc/crc64_ecma_norm_by16_10.asm`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/crc/crc64_ecma_norm_by8.asm` & `isal-1.2.0/src/isal/isa-l/crc/crc64_ecma_norm_by8.asm`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/crc/crc64_ecma_refl_by16_10.asm` & `isal-1.2.0/src/isal/isa-l/crc/crc64_ecma_refl_by16_10.asm`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/crc/crc64_ecma_refl_by8.asm` & `isal-1.2.0/src/isal/isa-l/crc/crc64_ecma_refl_by8.asm`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/crc/crc64_example.c` & `isal-1.2.0/src/isal/isa-l/crc/crc64_example.c`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/crc/crc64_funcs_perf.c` & `isal-1.2.0/src/isal/isa-l/crc/crc64_funcs_perf.c`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/crc/crc64_funcs_test.c` & `isal-1.2.0/src/isal/isa-l/crc/crc64_funcs_test.c`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/crc/crc64_iso_norm_by16_10.asm` & `isal-1.2.0/src/isal/isa-l/crc/crc64_iso_norm_by16_10.asm`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/crc/crc64_iso_norm_by8.asm` & `isal-1.2.0/src/isal/isa-l/crc/crc64_iso_norm_by8.asm`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/crc/crc64_iso_refl_by16_10.asm` & `isal-1.2.0/src/isal/isa-l/crc/crc64_iso_refl_by16_10.asm`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/crc/crc64_iso_refl_by8.asm` & `isal-1.2.0/src/isal/isa-l/crc/crc64_iso_refl_by8.asm`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/crc/crc64_jones_norm_by16_10.asm` & `isal-1.2.0/src/isal/isa-l/crc/crc64_jones_norm_by16_10.asm`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/crc/crc64_jones_norm_by8.asm` & `isal-1.2.0/src/isal/isa-l/crc/crc64_jones_norm_by8.asm`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/crc/crc64_jones_refl_by16_10.asm` & `isal-1.2.0/src/isal/isa-l/crc/crc64_jones_refl_by16_10.asm`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/crc/crc64_jones_refl_by8.asm` & `isal-1.2.0/src/isal/isa-l/crc/crc64_jones_refl_by8.asm`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/crc/crc64_multibinary.asm` & `isal-1.2.0/src/isal/isa-l/crc/crc64_multibinary.asm`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/crc/crc64_ref.h` & `isal-1.2.0/src/isal/isa-l/crc/crc64_ref.h`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/crc/crc_base.c` & `isal-1.2.0/src/isal/isa-l/crc/crc_base.c`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/crc/crc_base_aliases.c` & `isal-1.2.0/src/isal/isa-l/crc/crc_base_aliases.c`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/crc/crc_multibinary.asm` & `isal-1.2.0/src/isal/isa-l/crc/crc_multibinary.asm`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/crc/crc_ref.h` & `isal-1.2.0/src/isal/isa-l/crc/crc_ref.h`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/crc/crc_simple_test.c` & `isal-1.2.0/src/isal/isa-l/crc/crc_simple_test.c`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/doc/build.md` & `isal-1.2.0/src/isal/isa-l/doc/build.md`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/doc/test.md` & `isal-1.2.0/src/isal/isa-l/doc/test.md`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/erasure_code/Makefile.am` & `isal-1.2.0/src/isal/isa-l/erasure_code/Makefile.am`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/erasure_code/aarch64/Makefile.am` & `isal-1.2.0/src/isal/isa-l/erasure_code/aarch64/Makefile.am`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/erasure_code/aarch64/ec_aarch64_dispatcher.c` & `isal-1.2.0/src/isal/isa-l/erasure_code/aarch64/ec_aarch64_dispatcher.c`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/erasure_code/aarch64/ec_aarch64_highlevel_func.c` & `isal-1.2.0/src/isal/isa-l/erasure_code/aarch64/ec_aarch64_highlevel_func.c`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/erasure_code/aarch64/ec_multibinary_arm.S` & `isal-1.2.0/src/isal/isa-l/erasure_code/aarch64/ec_multibinary_arm.S`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/erasure_code/aarch64/gf_2vect_dot_prod_neon.S` & `isal-1.2.0/src/isal/isa-l/erasure_code/aarch64/gf_2vect_dot_prod_neon.S`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/erasure_code/aarch64/gf_2vect_mad_neon.S` & `isal-1.2.0/src/isal/isa-l/erasure_code/aarch64/gf_2vect_mad_neon.S`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/erasure_code/aarch64/gf_3vect_dot_prod_neon.S` & `isal-1.2.0/src/isal/isa-l/erasure_code/aarch64/gf_3vect_dot_prod_neon.S`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/erasure_code/aarch64/gf_3vect_mad_neon.S` & `isal-1.2.0/src/isal/isa-l/erasure_code/aarch64/gf_3vect_mad_neon.S`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/erasure_code/aarch64/gf_4vect_dot_prod_neon.S` & `isal-1.2.0/src/isal/isa-l/erasure_code/aarch64/gf_4vect_dot_prod_neon.S`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/erasure_code/aarch64/gf_4vect_mad_neon.S` & `isal-1.2.0/src/isal/isa-l/erasure_code/aarch64/gf_4vect_mad_neon.S`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/erasure_code/aarch64/gf_5vect_dot_prod_neon.S` & `isal-1.2.0/src/isal/isa-l/erasure_code/aarch64/gf_5vect_dot_prod_neon.S`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/erasure_code/aarch64/gf_5vect_mad_neon.S` & `isal-1.2.0/src/isal/isa-l/erasure_code/aarch64/gf_5vect_mad_neon.S`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/erasure_code/aarch64/gf_6vect_mad_neon.S` & `isal-1.2.0/src/isal/isa-l/erasure_code/aarch64/gf_6vect_mad_neon.S`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/erasure_code/aarch64/gf_vect_dot_prod_neon.S` & `isal-1.2.0/src/isal/isa-l/erasure_code/aarch64/gf_vect_dot_prod_neon.S`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/erasure_code/aarch64/gf_vect_mad_neon.S` & `isal-1.2.0/src/isal/isa-l/erasure_code/aarch64/gf_vect_mad_neon.S`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/erasure_code/aarch64/gf_vect_mul_neon.S` & `isal-1.2.0/src/isal/isa-l/erasure_code/aarch64/gf_vect_mul_neon.S`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/erasure_code/ec_base.c` & `isal-1.2.0/src/isal/isa-l/erasure_code/ec_base.c`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/erasure_code/ec_base.h` & `isal-1.2.0/src/isal/isa-l/erasure_code/ec_base.h`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/erasure_code/ec_base_aliases.c` & `isal-1.2.0/src/isal/isa-l/erasure_code/ec_base_aliases.c`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/erasure_code/ec_highlevel_func.c` & `isal-1.2.0/src/isal/isa-l/erasure_code/ec_highlevel_func.c`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/erasure_code/ec_multibinary.asm` & `isal-1.2.0/src/isal/isa-l/erasure_code/ec_multibinary.asm`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/erasure_code/erasure_code_base_perf.c` & `isal-1.2.0/src/isal/isa-l/erasure_code/erasure_code_base_perf.c`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/erasure_code/erasure_code_base_test.c` & `isal-1.2.0/src/isal/isa-l/erasure_code/erasure_code_base_test.c`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/erasure_code/erasure_code_perf.c` & `isal-1.2.0/src/isal/isa-l/erasure_code/erasure_code_perf.c`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/erasure_code/erasure_code_test.c` & `isal-1.2.0/src/isal/isa-l/erasure_code/erasure_code_test.c`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/erasure_code/erasure_code_update_perf.c` & `isal-1.2.0/src/isal/isa-l/erasure_code/erasure_code_update_perf.c`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/erasure_code/erasure_code_update_test.c` & `isal-1.2.0/src/isal/isa-l/erasure_code/erasure_code_update_test.c`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/erasure_code/gen_rs_matrix_limits.c` & `isal-1.2.0/src/isal/isa-l/erasure_code/gen_rs_matrix_limits.c`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/erasure_code/gf_2vect_dot_prod_avx.asm` & `isal-1.2.0/src/isal/isa-l/erasure_code/gf_2vect_dot_prod_avx.asm`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/erasure_code/gf_2vect_dot_prod_avx2.asm` & `isal-1.2.0/src/isal/isa-l/erasure_code/gf_2vect_dot_prod_avx2.asm`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/erasure_code/gf_2vect_dot_prod_avx512.asm` & `isal-1.2.0/src/isal/isa-l/erasure_code/gf_2vect_dot_prod_avx512.asm`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/erasure_code/gf_2vect_dot_prod_sse.asm` & `isal-1.2.0/src/isal/isa-l/erasure_code/gf_2vect_dot_prod_sse.asm`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/erasure_code/gf_2vect_mad_avx.asm` & `isal-1.2.0/src/isal/isa-l/erasure_code/gf_2vect_mad_avx.asm`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/erasure_code/gf_2vect_mad_avx2.asm` & `isal-1.2.0/src/isal/isa-l/erasure_code/gf_2vect_mad_avx2.asm`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/erasure_code/gf_2vect_mad_avx512.asm` & `isal-1.2.0/src/isal/isa-l/erasure_code/gf_2vect_mad_avx512.asm`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/erasure_code/gf_2vect_mad_sse.asm` & `isal-1.2.0/src/isal/isa-l/erasure_code/gf_2vect_mad_sse.asm`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/erasure_code/gf_3vect_dot_prod_avx.asm` & `isal-1.2.0/src/isal/isa-l/erasure_code/gf_3vect_dot_prod_avx.asm`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/erasure_code/gf_3vect_dot_prod_avx2.asm` & `isal-1.2.0/src/isal/isa-l/erasure_code/gf_3vect_dot_prod_avx2.asm`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/erasure_code/gf_3vect_dot_prod_avx512.asm` & `isal-1.2.0/src/isal/isa-l/erasure_code/gf_3vect_dot_prod_avx512.asm`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/erasure_code/gf_3vect_dot_prod_sse.asm` & `isal-1.2.0/src/isal/isa-l/erasure_code/gf_3vect_dot_prod_sse.asm`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/erasure_code/gf_3vect_mad_avx.asm` & `isal-1.2.0/src/isal/isa-l/erasure_code/gf_3vect_mad_avx.asm`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/erasure_code/gf_3vect_mad_avx2.asm` & `isal-1.2.0/src/isal/isa-l/erasure_code/gf_3vect_mad_avx2.asm`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/erasure_code/gf_3vect_mad_avx512.asm` & `isal-1.2.0/src/isal/isa-l/erasure_code/gf_3vect_mad_avx512.asm`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/erasure_code/gf_3vect_mad_sse.asm` & `isal-1.2.0/src/isal/isa-l/erasure_code/gf_3vect_mad_sse.asm`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/erasure_code/gf_4vect_dot_prod_avx.asm` & `isal-1.2.0/src/isal/isa-l/erasure_code/gf_4vect_dot_prod_avx.asm`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/erasure_code/gf_4vect_dot_prod_avx2.asm` & `isal-1.2.0/src/isal/isa-l/erasure_code/gf_4vect_dot_prod_avx2.asm`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/erasure_code/gf_4vect_dot_prod_avx512.asm` & `isal-1.2.0/src/isal/isa-l/erasure_code/gf_4vect_dot_prod_avx512.asm`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/erasure_code/gf_4vect_dot_prod_sse.asm` & `isal-1.2.0/src/isal/isa-l/erasure_code/gf_4vect_dot_prod_sse.asm`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/erasure_code/gf_4vect_mad_avx.asm` & `isal-1.2.0/src/isal/isa-l/erasure_code/gf_4vect_mad_avx.asm`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/erasure_code/gf_4vect_mad_avx2.asm` & `isal-1.2.0/src/isal/isa-l/erasure_code/gf_4vect_mad_avx2.asm`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/erasure_code/gf_4vect_mad_avx512.asm` & `isal-1.2.0/src/isal/isa-l/erasure_code/gf_4vect_mad_avx512.asm`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/erasure_code/gf_4vect_mad_sse.asm` & `isal-1.2.0/src/isal/isa-l/erasure_code/gf_4vect_mad_sse.asm`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/erasure_code/gf_5vect_dot_prod_avx.asm` & `isal-1.2.0/src/isal/isa-l/erasure_code/gf_5vect_dot_prod_avx.asm`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/erasure_code/gf_5vect_dot_prod_avx2.asm` & `isal-1.2.0/src/isal/isa-l/erasure_code/gf_5vect_dot_prod_avx2.asm`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/erasure_code/gf_5vect_dot_prod_avx512.asm` & `isal-1.2.0/src/isal/isa-l/erasure_code/gf_5vect_dot_prod_avx512.asm`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/erasure_code/gf_5vect_dot_prod_sse.asm` & `isal-1.2.0/src/isal/isa-l/erasure_code/gf_5vect_dot_prod_sse.asm`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/erasure_code/gf_5vect_mad_avx.asm` & `isal-1.2.0/src/isal/isa-l/erasure_code/gf_5vect_mad_avx.asm`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/erasure_code/gf_5vect_mad_avx2.asm` & `isal-1.2.0/src/isal/isa-l/erasure_code/gf_5vect_mad_avx2.asm`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/erasure_code/gf_5vect_mad_avx512.asm` & `isal-1.2.0/src/isal/isa-l/erasure_code/gf_5vect_mad_avx512.asm`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/erasure_code/gf_5vect_mad_sse.asm` & `isal-1.2.0/src/isal/isa-l/erasure_code/gf_5vect_mad_sse.asm`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/erasure_code/gf_6vect_dot_prod_avx.asm` & `isal-1.2.0/src/isal/isa-l/erasure_code/gf_6vect_dot_prod_avx.asm`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/erasure_code/gf_6vect_dot_prod_avx2.asm` & `isal-1.2.0/src/isal/isa-l/erasure_code/gf_6vect_dot_prod_avx2.asm`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/erasure_code/gf_6vect_dot_prod_avx512.asm` & `isal-1.2.0/src/isal/isa-l/erasure_code/gf_6vect_dot_prod_avx512.asm`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/erasure_code/gf_6vect_dot_prod_sse.asm` & `isal-1.2.0/src/isal/isa-l/erasure_code/gf_6vect_dot_prod_sse.asm`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/erasure_code/gf_6vect_mad_avx.asm` & `isal-1.2.0/src/isal/isa-l/erasure_code/gf_6vect_mad_avx.asm`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/erasure_code/gf_6vect_mad_avx2.asm` & `isal-1.2.0/src/isal/isa-l/erasure_code/gf_6vect_mad_avx2.asm`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/erasure_code/gf_6vect_mad_avx512.asm` & `isal-1.2.0/src/isal/isa-l/erasure_code/gf_6vect_mad_avx512.asm`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/erasure_code/gf_6vect_mad_sse.asm` & `isal-1.2.0/src/isal/isa-l/erasure_code/gf_6vect_mad_sse.asm`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/erasure_code/gf_inverse_test.c` & `isal-1.2.0/src/isal/isa-l/erasure_code/gf_inverse_test.c`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/erasure_code/gf_vect_dot_prod_1tbl.c` & `isal-1.2.0/src/isal/isa-l/erasure_code/gf_vect_dot_prod_1tbl.c`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/erasure_code/gf_vect_dot_prod_avx.asm` & `isal-1.2.0/src/isal/isa-l/erasure_code/gf_vect_dot_prod_avx.asm`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/erasure_code/gf_vect_dot_prod_avx2.asm` & `isal-1.2.0/src/isal/isa-l/erasure_code/gf_vect_dot_prod_avx2.asm`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/erasure_code/gf_vect_dot_prod_avx512.asm` & `isal-1.2.0/src/isal/isa-l/erasure_code/gf_vect_dot_prod_avx512.asm`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/erasure_code/gf_vect_dot_prod_base_test.c` & `isal-1.2.0/src/isal/isa-l/erasure_code/gf_vect_dot_prod_base_test.c`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/erasure_code/gf_vect_dot_prod_perf.c` & `isal-1.2.0/src/isal/isa-l/erasure_code/gf_vect_dot_prod_perf.c`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/erasure_code/gf_vect_dot_prod_sse.asm` & `isal-1.2.0/src/isal/isa-l/erasure_code/gf_vect_dot_prod_sse.asm`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/erasure_code/gf_vect_dot_prod_test.c` & `isal-1.2.0/src/isal/isa-l/erasure_code/gf_vect_dot_prod_test.c`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/erasure_code/gf_vect_mad_avx.asm` & `isal-1.2.0/src/isal/isa-l/erasure_code/gf_vect_mad_avx.asm`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/erasure_code/gf_vect_mad_avx2.asm` & `isal-1.2.0/src/isal/isa-l/erasure_code/gf_vect_mad_avx2.asm`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/erasure_code/gf_vect_mad_avx512.asm` & `isal-1.2.0/src/isal/isa-l/erasure_code/gf_vect_mad_avx512.asm`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/erasure_code/gf_vect_mad_sse.asm` & `isal-1.2.0/src/isal/isa-l/erasure_code/gf_vect_mad_sse.asm`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/erasure_code/gf_vect_mad_test.c` & `isal-1.2.0/src/isal/isa-l/erasure_code/gf_vect_mad_test.c`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/erasure_code/gf_vect_mul_avx.asm` & `isal-1.2.0/src/isal/isa-l/erasure_code/gf_vect_mul_avx.asm`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/erasure_code/gf_vect_mul_base_test.c` & `isal-1.2.0/src/isal/isa-l/erasure_code/gf_vect_mul_base_test.c`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/erasure_code/gf_vect_mul_perf.c` & `isal-1.2.0/src/isal/isa-l/erasure_code/gf_vect_mul_perf.c`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/erasure_code/gf_vect_mul_sse.asm` & `isal-1.2.0/src/isal/isa-l/erasure_code/gf_vect_mul_sse.asm`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/erasure_code/gf_vect_mul_test.c` & `isal-1.2.0/src/isal/isa-l/erasure_code/gf_vect_mul_test.c`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/erasure_code/ppc64le/Makefile.am` & `isal-1.2.0/src/isal/isa-l/erasure_code/ppc64le/Makefile.am`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/erasure_code/ppc64le/ec_base_vsx.c` & `isal-1.2.0/src/isal/isa-l/erasure_code/ppc64le/ec_base_vsx.c`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/erasure_code/ppc64le/ec_base_vsx.h` & `isal-1.2.0/src/isal/isa-l/erasure_code/ppc64le/ec_base_vsx.h`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/erasure_code/ppc64le/gf_2vect_dot_prod_vsx.c` & `isal-1.2.0/src/isal/isa-l/erasure_code/ppc64le/gf_2vect_dot_prod_vsx.c`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/erasure_code/ppc64le/gf_2vect_mad_vsx.c` & `isal-1.2.0/src/isal/isa-l/erasure_code/ppc64le/gf_2vect_mad_vsx.c`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/erasure_code/ppc64le/gf_3vect_dot_prod_vsx.c` & `isal-1.2.0/src/isal/isa-l/erasure_code/ppc64le/gf_3vect_dot_prod_vsx.c`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/erasure_code/ppc64le/gf_3vect_mad_vsx.c` & `isal-1.2.0/src/isal/isa-l/erasure_code/ppc64le/gf_3vect_mad_vsx.c`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/erasure_code/ppc64le/gf_4vect_dot_prod_vsx.c` & `isal-1.2.0/src/isal/isa-l/erasure_code/ppc64le/gf_4vect_dot_prod_vsx.c`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/erasure_code/ppc64le/gf_4vect_mad_vsx.c` & `isal-1.2.0/src/isal/isa-l/erasure_code/ppc64le/gf_4vect_mad_vsx.c`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/erasure_code/ppc64le/gf_5vect_dot_prod_vsx.c` & `isal-1.2.0/src/isal/isa-l/erasure_code/ppc64le/gf_5vect_dot_prod_vsx.c`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/erasure_code/ppc64le/gf_5vect_mad_vsx.c` & `isal-1.2.0/src/isal/isa-l/erasure_code/ppc64le/gf_5vect_mad_vsx.c`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/erasure_code/ppc64le/gf_6vect_dot_prod_vsx.c` & `isal-1.2.0/src/isal/isa-l/erasure_code/ppc64le/gf_6vect_dot_prod_vsx.c`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/erasure_code/ppc64le/gf_6vect_mad_vsx.c` & `isal-1.2.0/src/isal/isa-l/erasure_code/ppc64le/gf_6vect_mad_vsx.c`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/erasure_code/ppc64le/gf_vect_dot_prod_vsx.c` & `isal-1.2.0/src/isal/isa-l/erasure_code/ppc64le/gf_vect_dot_prod_vsx.c`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/erasure_code/ppc64le/gf_vect_mad_vsx.c` & `isal-1.2.0/src/isal/isa-l/erasure_code/ppc64le/gf_vect_mad_vsx.c`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/erasure_code/ppc64le/gf_vect_mul_vsx.c` & `isal-1.2.0/src/isal/isa-l/erasure_code/ppc64le/gf_vect_mul_vsx.c`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/examples/ec/Makefile.am` & `isal-1.2.0/src/isal/isa-l/examples/ec/Makefile.am`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/examples/ec/ec_piggyback_example.c` & `isal-1.2.0/src/isal/isa-l/examples/ec/ec_piggyback_example.c`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/examples/ec/ec_simple_example.c` & `isal-1.2.0/src/isal/isa-l/examples/ec/ec_simple_example.c`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/igzip/Makefile.am` & `isal-1.2.0/src/isal/isa-l/igzip/Makefile.am`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/igzip/aarch64/bitbuf2_aarch64.h` & `isal-1.2.0/src/isal/isa-l/igzip/aarch64/bitbuf2_aarch64.h`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/igzip/aarch64/data_struct_aarch64.h` & `isal-1.2.0/src/isal/isa-l/igzip/aarch64/data_struct_aarch64.h`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/igzip/aarch64/encode_df.S` & `isal-1.2.0/src/isal/isa-l/igzip/aarch64/encode_df.S`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/igzip/aarch64/gen_icf_map.S` & `isal-1.2.0/src/isal/isa-l/igzip/aarch64/gen_icf_map.S`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/igzip/aarch64/huffman_aarch64.h` & `isal-1.2.0/src/isal/isa-l/igzip/aarch64/huffman_aarch64.h`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/igzip/aarch64/igzip_decode_huffman_code_block_aarch64.S` & `isal-1.2.0/src/isal/isa-l/igzip/aarch64/igzip_decode_huffman_code_block_aarch64.S`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/igzip/aarch64/igzip_deflate_body_aarch64.S` & `isal-1.2.0/src/isal/isa-l/igzip/aarch64/igzip_deflate_body_aarch64.S`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/igzip/aarch64/igzip_deflate_finish_aarch64.S` & `isal-1.2.0/src/isal/isa-l/igzip/aarch64/igzip_deflate_finish_aarch64.S`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/igzip/aarch64/igzip_deflate_hash_aarch64.S` & `isal-1.2.0/src/isal/isa-l/igzip/aarch64/igzip_deflate_hash_aarch64.S`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/igzip/aarch64/igzip_inflate_multibinary_arm64.S` & `isal-1.2.0/src/isal/isa-l/igzip/aarch64/igzip_inflate_multibinary_arm64.S`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/igzip/aarch64/igzip_isal_adler32_neon.S` & `isal-1.2.0/src/isal/isa-l/igzip/aarch64/igzip_isal_adler32_neon.S`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/igzip/aarch64/igzip_multibinary_aarch64_dispatcher.c` & `isal-1.2.0/src/isal/isa-l/igzip/aarch64/igzip_multibinary_aarch64_dispatcher.c`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/igzip/aarch64/igzip_multibinary_arm64.S` & `isal-1.2.0/src/isal/isa-l/igzip/aarch64/igzip_multibinary_arm64.S`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/igzip/aarch64/igzip_set_long_icf_fg.S` & `isal-1.2.0/src/isal/isa-l/igzip/aarch64/igzip_set_long_icf_fg.S`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/igzip/aarch64/isal_deflate_icf_body_hash_hist.S` & `isal-1.2.0/src/isal/isa-l/igzip/aarch64/isal_deflate_icf_body_hash_hist.S`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/igzip/aarch64/isal_deflate_icf_finish_hash_hist.S` & `isal-1.2.0/src/isal/isa-l/igzip/aarch64/isal_deflate_icf_finish_hash_hist.S`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/igzip/aarch64/isal_update_histogram.S` & `isal-1.2.0/src/isal/isa-l/igzip/aarch64/isal_update_histogram.S`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/igzip/aarch64/lz0a_const_aarch64.h` & `isal-1.2.0/src/isal/isa-l/igzip/aarch64/lz0a_const_aarch64.h`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/igzip/aarch64/options_aarch64.h` & `isal-1.2.0/src/isal/isa-l/igzip/aarch64/options_aarch64.h`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/igzip/aarch64/stdmac_aarch64.h` & `isal-1.2.0/src/isal/isa-l/igzip/aarch64/stdmac_aarch64.h`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/igzip/adler32_avx2_4.asm` & `isal-1.2.0/src/isal/isa-l/igzip/adler32_avx2_4.asm`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/igzip/adler32_base.c` & `isal-1.2.0/src/isal/isa-l/igzip/adler32_base.c`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/igzip/adler32_perf.c` & `isal-1.2.0/src/isal/isa-l/igzip/adler32_perf.c`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/igzip/adler32_sse.asm` & `isal-1.2.0/src/isal/isa-l/igzip/adler32_sse.asm`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/igzip/bitbuf2.asm` & `isal-1.2.0/src/isal/isa-l/igzip/bitbuf2.asm`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/igzip/bitbuf2.h` & `isal-1.2.0/src/isal/isa-l/igzip/bitbuf2.h`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/igzip/checksum32_funcs_test.c` & `isal-1.2.0/src/isal/isa-l/igzip/checksum32_funcs_test.c`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/igzip/checksum_test_ref.h` & `isal-1.2.0/src/isal/isa-l/igzip/checksum_test_ref.h`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/igzip/data_struct2.asm` & `isal-1.2.0/src/isal/isa-l/igzip/data_struct2.asm`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/igzip/encode_df.c` & `isal-1.2.0/src/isal/isa-l/igzip/encode_df.c`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/igzip/encode_df.h` & `isal-1.2.0/src/isal/isa-l/igzip/encode_df.h`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/igzip/encode_df_04.asm` & `isal-1.2.0/src/isal/isa-l/igzip/encode_df_04.asm`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/igzip/encode_df_06.asm` & `isal-1.2.0/src/isal/isa-l/igzip/encode_df_06.asm`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/igzip/flatten_ll.c` & `isal-1.2.0/src/isal/isa-l/igzip/flatten_ll.c`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/igzip/generate_custom_hufftables.c` & `isal-1.2.0/src/isal/isa-l/igzip/generate_custom_hufftables.c`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/igzip/generate_static_inflate.c` & `isal-1.2.0/src/isal/isa-l/igzip/generate_static_inflate.c`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/igzip/heap_macros.asm` & `isal-1.2.0/src/isal/isa-l/igzip/heap_macros.asm`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/igzip/huff_codes.c` & `isal-1.2.0/src/isal/isa-l/igzip/huff_codes.c`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/igzip/huff_codes.h` & `isal-1.2.0/src/isal/isa-l/igzip/huff_codes.h`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/igzip/huffman.asm` & `isal-1.2.0/src/isal/isa-l/igzip/huffman.asm`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/igzip/huffman.h` & `isal-1.2.0/src/isal/isa-l/igzip/huffman.h`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/igzip/hufftables_c.c` & `isal-1.2.0/src/isal/isa-l/igzip/hufftables_c.c`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/igzip/igzip.c` & `isal-1.2.0/src/isal/isa-l/igzip/igzip.c`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/igzip/igzip_base.c` & `isal-1.2.0/src/isal/isa-l/igzip/igzip_base.c`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/igzip/igzip_base_aliases.c` & `isal-1.2.0/src/isal/isa-l/igzip/igzip_base_aliases.c`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/igzip/igzip_body.asm` & `isal-1.2.0/src/isal/isa-l/igzip/igzip_body.asm`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/igzip/igzip_build_hash_table_perf.c` & `isal-1.2.0/src/isal/isa-l/igzip/igzip_build_hash_table_perf.c`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/igzip/igzip_compare_types.asm` & `isal-1.2.0/src/isal/isa-l/igzip/igzip_compare_types.asm`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/igzip/igzip_decode_block_stateless.asm` & `isal-1.2.0/src/isal/isa-l/igzip/igzip_decode_block_stateless.asm`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/igzip/igzip_deflate_hash.asm` & `isal-1.2.0/src/isal/isa-l/igzip/igzip_deflate_hash.asm`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/igzip/igzip_example.c` & `isal-1.2.0/src/isal/isa-l/igzip/igzip_example.c`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/igzip/igzip_file_perf.c` & `isal-1.2.0/src/isal/isa-l/igzip/igzip_file_perf.c`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/igzip/igzip_finish.asm` & `isal-1.2.0/src/isal/isa-l/igzip/igzip_finish.asm`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/igzip/igzip_gen_icf_map_lh1_04.asm` & `isal-1.2.0/src/isal/isa-l/igzip/igzip_gen_icf_map_lh1_04.asm`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/igzip/igzip_gen_icf_map_lh1_06.asm` & `isal-1.2.0/src/isal/isa-l/igzip/igzip_gen_icf_map_lh1_06.asm`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/igzip/igzip_hist_perf.c` & `isal-1.2.0/src/isal/isa-l/igzip/igzip_hist_perf.c`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/igzip/igzip_icf_base.c` & `isal-1.2.0/src/isal/isa-l/igzip/igzip_icf_base.c`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/igzip/igzip_icf_body.c` & `isal-1.2.0/src/isal/isa-l/igzip/igzip_icf_body.c`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/igzip/igzip_icf_body_h1_gr_bt.asm` & `isal-1.2.0/src/isal/isa-l/igzip/igzip_icf_body_h1_gr_bt.asm`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/igzip/igzip_icf_finish.asm` & `isal-1.2.0/src/isal/isa-l/igzip/igzip_icf_finish.asm`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/igzip/igzip_inflate.c` & `isal-1.2.0/src/isal/isa-l/igzip/igzip_inflate.c`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/igzip/igzip_inflate_multibinary.asm` & `isal-1.2.0/src/isal/isa-l/igzip/igzip_inflate_multibinary.asm`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/igzip/igzip_inflate_test.c` & `isal-1.2.0/src/isal/isa-l/igzip/igzip_inflate_test.c`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/igzip/igzip_level_buf_structs.h` & `isal-1.2.0/src/isal/isa-l/igzip/igzip_level_buf_structs.h`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/igzip/igzip_multibinary.asm` & `isal-1.2.0/src/isal/isa-l/igzip/igzip_multibinary.asm`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/igzip/igzip_perf.c` & `isal-1.2.0/src/isal/isa-l/igzip/igzip_perf.c`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/igzip/igzip_rand_test.c` & `isal-1.2.0/src/isal/isa-l/igzip/igzip_rand_test.c`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/igzip/igzip_semi_dyn_file_perf.c` & `isal-1.2.0/src/isal/isa-l/igzip/igzip_semi_dyn_file_perf.c`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/igzip/igzip_set_long_icf_fg_04.asm` & `isal-1.2.0/src/isal/isa-l/igzip/igzip_set_long_icf_fg_04.asm`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/igzip/igzip_set_long_icf_fg_06.asm` & `isal-1.2.0/src/isal/isa-l/igzip/igzip_set_long_icf_fg_06.asm`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/igzip/igzip_sync_flush_example.c` & `isal-1.2.0/src/isal/isa-l/igzip/igzip_sync_flush_example.c`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/igzip/igzip_update_histogram.asm` & `isal-1.2.0/src/isal/isa-l/igzip/igzip_update_histogram.asm`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/igzip/igzip_wrapper.h` & `isal-1.2.0/src/isal/isa-l/igzip/igzip_wrapper.h`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/igzip/igzip_wrapper_hdr_test.c` & `isal-1.2.0/src/isal/isa-l/igzip/igzip_wrapper_hdr_test.c`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/igzip/inflate_data_structs.asm` & `isal-1.2.0/src/isal/isa-l/igzip/inflate_data_structs.asm`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/igzip/inflate_std_vects.h` & `isal-1.2.0/src/isal/isa-l/igzip/inflate_std_vects.h`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/igzip/lz0a_const.asm` & `isal-1.2.0/src/isal/isa-l/igzip/lz0a_const.asm`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/igzip/options.asm` & `isal-1.2.0/src/isal/isa-l/igzip/options.asm`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/igzip/proc_heap.asm` & `isal-1.2.0/src/isal/isa-l/igzip/proc_heap.asm`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/igzip/proc_heap_base.c` & `isal-1.2.0/src/isal/isa-l/igzip/proc_heap_base.c`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/igzip/repeated_char_result.h` & `isal-1.2.0/src/isal/isa-l/igzip/repeated_char_result.h`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/igzip/rfc1951_lookup.asm` & `isal-1.2.0/src/isal/isa-l/igzip/rfc1951_lookup.asm`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/igzip/static_inflate.h` & `isal-1.2.0/src/isal/isa-l/igzip/static_inflate.h`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/igzip/stdmac.asm` & `isal-1.2.0/src/isal/isa-l/igzip/stdmac.asm`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/include/aarch64_multibinary.h` & `isal-1.2.0/src/isal/isa-l/include/aarch64_multibinary.h`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/include/crc.h` & `isal-1.2.0/src/isal/isa-l/include/crc.h`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/include/crc64.h` & `isal-1.2.0/src/isal/isa-l/include/crc64.h`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/include/erasure_code.h` & `isal-1.2.0/src/isal/isa-l/include/erasure_code.h`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/include/gf_vect_mul.h` & `isal-1.2.0/src/isal/isa-l/include/gf_vect_mul.h`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/include/igzip_lib.h` & `isal-1.2.0/src/isal/isa-l/include/igzip_lib.h`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/include/mem_routines.h` & `isal-1.2.0/src/isal/isa-l/include/mem_routines.h`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/include/multibinary.asm` & `isal-1.2.0/src/isal/isa-l/include/multibinary.asm`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/include/raid.h` & `isal-1.2.0/src/isal/isa-l/include/raid.h`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/include/reg_sizes.asm` & `isal-1.2.0/src/isal/isa-l/include/reg_sizes.asm`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/include/test.h` & `isal-1.2.0/src/isal/isa-l/include/test.h`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/include/types.h` & `isal-1.2.0/src/isal/isa-l/include/types.h`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/include/unaligned.h` & `isal-1.2.0/src/isal/isa-l/include/unaligned.h`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/isa-l.def` & `isal-1.2.0/src/isal/isa-l/isa-l.def`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/make.inc` & `isal-1.2.0/src/isal/isa-l/make.inc`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/mem/Makefile.am` & `isal-1.2.0/src/isal/isa-l/mem/Makefile.am`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/mem/aarch64/Makefile.am` & `isal-1.2.0/src/isal/isa-l/mem/aarch64/Makefile.am`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/mem/aarch64/mem_aarch64_dispatcher.c` & `isal-1.2.0/src/isal/isa-l/mem/aarch64/mem_aarch64_dispatcher.c`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/mem/aarch64/mem_multibinary_arm.S` & `isal-1.2.0/src/isal/isa-l/mem/aarch64/mem_multibinary_arm.S`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/mem/aarch64/mem_zero_detect_neon.S` & `isal-1.2.0/src/isal/isa-l/mem/aarch64/mem_zero_detect_neon.S`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/mem/mem_multibinary.asm` & `isal-1.2.0/src/isal/isa-l/mem/mem_multibinary.asm`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/mem/mem_zero_detect_avx.asm` & `isal-1.2.0/src/isal/isa-l/mem/mem_zero_detect_avx.asm`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/mem/mem_zero_detect_base.c` & `isal-1.2.0/src/isal/isa-l/mem/mem_zero_detect_base.c`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/mem/mem_zero_detect_base_aliases.c` & `isal-1.2.0/src/isal/isa-l/mem/mem_zero_detect_base_aliases.c`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/mem/mem_zero_detect_perf.c` & `isal-1.2.0/src/isal/isa-l/mem/mem_zero_detect_perf.c`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/mem/mem_zero_detect_sse.asm` & `isal-1.2.0/src/isal/isa-l/mem/mem_zero_detect_sse.asm`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/mem/mem_zero_detect_test.c` & `isal-1.2.0/src/isal/isa-l/mem/mem_zero_detect_test.c`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/programs/Makefile.am` & `isal-1.2.0/src/isal/isa-l/programs/Makefile.am`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/programs/igzip.1` & `isal-1.2.0/src/isal/isa-l/programs/igzip.1`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/programs/igzip.1.h2m` & `isal-1.2.0/src/isal/isa-l/programs/igzip.1.h2m`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/programs/igzip_cli.c` & `isal-1.2.0/src/isal/isa-l/programs/igzip_cli.c`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/programs/igzip_cli_check.sh` & `isal-1.2.0/src/isal/isa-l/programs/igzip_cli_check.sh`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/raid/Makefile.am` & `isal-1.2.0/src/isal/isa-l/raid/Makefile.am`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/raid/aarch64/Makefile.am` & `isal-1.2.0/src/isal/isa-l/raid/aarch64/Makefile.am`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/raid/aarch64/pq_check_neon.S` & `isal-1.2.0/src/isal/isa-l/raid/aarch64/pq_check_neon.S`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/raid/aarch64/pq_gen_neon.S` & `isal-1.2.0/src/isal/isa-l/raid/aarch64/pq_gen_neon.S`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/raid/aarch64/raid_aarch64_dispatcher.c` & `isal-1.2.0/src/isal/isa-l/raid/aarch64/raid_aarch64_dispatcher.c`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/raid/aarch64/raid_multibinary_arm.S` & `isal-1.2.0/src/isal/isa-l/raid/aarch64/raid_multibinary_arm.S`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/raid/aarch64/xor_check_neon.S` & `isal-1.2.0/src/isal/isa-l/raid/aarch64/xor_check_neon.S`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/raid/aarch64/xor_gen_neon.S` & `isal-1.2.0/src/isal/isa-l/raid/aarch64/xor_gen_neon.S`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/raid/pq_check_sse.asm` & `isal-1.2.0/src/isal/isa-l/raid/pq_check_sse.asm`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/raid/pq_check_sse_i32.asm` & `isal-1.2.0/src/isal/isa-l/raid/pq_check_sse_i32.asm`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/raid/pq_check_test.c` & `isal-1.2.0/src/isal/isa-l/raid/pq_check_test.c`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/raid/pq_gen_avx.asm` & `isal-1.2.0/src/isal/isa-l/raid/pq_gen_avx.asm`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/raid/pq_gen_avx2.asm` & `isal-1.2.0/src/isal/isa-l/raid/pq_gen_avx2.asm`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/raid/pq_gen_avx512.asm` & `isal-1.2.0/src/isal/isa-l/raid/pq_gen_avx512.asm`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/raid/pq_gen_perf.c` & `isal-1.2.0/src/isal/isa-l/raid/pq_gen_perf.c`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/raid/pq_gen_sse.asm` & `isal-1.2.0/src/isal/isa-l/raid/pq_gen_sse.asm`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/raid/pq_gen_sse_i32.asm` & `isal-1.2.0/src/isal/isa-l/raid/pq_gen_sse_i32.asm`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/raid/pq_gen_test.c` & `isal-1.2.0/src/isal/isa-l/raid/pq_gen_test.c`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/raid/raid_base.c` & `isal-1.2.0/src/isal/isa-l/raid/raid_base.c`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/raid/raid_base_aliases.c` & `isal-1.2.0/src/isal/isa-l/raid/raid_base_aliases.c`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/raid/raid_multibinary.asm` & `isal-1.2.0/src/isal/isa-l/raid/raid_multibinary.asm`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/raid/raid_multibinary_i32.asm` & `isal-1.2.0/src/isal/isa-l/raid/raid_multibinary_i32.asm`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/raid/xor_check_sse.asm` & `isal-1.2.0/src/isal/isa-l/raid/xor_check_sse.asm`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/raid/xor_check_test.c` & `isal-1.2.0/src/isal/isa-l/raid/xor_check_test.c`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/raid/xor_example.c` & `isal-1.2.0/src/isal/isa-l/raid/xor_example.c`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/raid/xor_gen_avx.asm` & `isal-1.2.0/src/isal/isa-l/raid/xor_gen_avx.asm`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/raid/xor_gen_avx512.asm` & `isal-1.2.0/src/isal/isa-l/raid/xor_gen_avx512.asm`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/raid/xor_gen_perf.c` & `isal-1.2.0/src/isal/isa-l/raid/xor_gen_perf.c`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/raid/xor_gen_sse.asm` & `isal-1.2.0/src/isal/isa-l/raid/xor_gen_sse.asm`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/raid/xor_gen_test.c` & `isal-1.2.0/src/isal/isa-l/raid/xor_gen_test.c`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/tests/fuzz/Makefile.am` & `isal-1.2.0/src/isal/isa-l/tests/fuzz/Makefile.am`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/tests/fuzz/igzip_checked_inflate_fuzz_test.c` & `isal-1.2.0/src/isal/isa-l/tests/fuzz/igzip_checked_inflate_fuzz_test.c`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/tests/fuzz/igzip_dump_inflate_corpus.c` & `isal-1.2.0/src/isal/isa-l/tests/fuzz/igzip_dump_inflate_corpus.c`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/tests/fuzz/igzip_fuzz_inflate.c` & `isal-1.2.0/src/isal/isa-l/tests/fuzz/igzip_fuzz_inflate.c`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/tests/fuzz/igzip_simple_round_trip_fuzz_test.c` & `isal-1.2.0/src/isal/isa-l/tests/fuzz/igzip_simple_round_trip_fuzz_test.c`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/tools/check_format.sh` & `isal-1.2.0/src/isal/isa-l/tools/check_format.sh`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/tools/gen_nmake.mk` & `isal-1.2.0/src/isal/isa-l/tools/gen_nmake.mk`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/tools/nasm-cet-filter.sh` & `isal-1.2.0/src/isal/isa-l/tools/nasm-cet-filter.sh`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/tools/nasm-filter.sh` & `isal-1.2.0/src/isal/isa-l/tools/nasm-filter.sh`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/tools/test_autorun.sh` & `isal-1.2.0/src/isal/isa-l/tools/test_autorun.sh`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/tools/test_checks.sh` & `isal-1.2.0/src/isal/isa-l/tools/test_checks.sh`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/tools/test_extended.sh` & `isal-1.2.0/src/isal/isa-l/tools/test_extended.sh`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/tools/test_fuzz.sh` & `isal-1.2.0/src/isal/isa-l/tools/test_fuzz.sh`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/tools/yasm-cet-filter.sh` & `isal-1.2.0/src/isal/isa-l/tools/yasm-cet-filter.sh`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isa-l/tools/yasm-filter.sh` & `isal-1.2.0/src/isal/isa-l/tools/yasm-filter.sh`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isal_shared.h` & `isal-1.2.0/src/isal/isal_shared.h`

 * *Files 4% similar despite different names*

```diff
@@ -24,14 +24,22 @@
 #include "structmember.h"         // PyMemberDef
 
 #include <isa-l/igzip_lib.h>
 #include <stdint.h>
 
 static PyObject *IsalError;
 
+#define ENTER_ZLIB(obj) do {                      \
+    if (!PyThread_acquire_lock((obj)->lock, 0)) { \
+        Py_BEGIN_ALLOW_THREADS                    \
+        PyThread_acquire_lock((obj)->lock, 1);    \
+        Py_END_ALLOW_THREADS                      \
+    } } while (0)
+#define LEAVE_ZLIB(obj) PyThread_release_lock((obj)->lock);
+
 /* Initial buffer size. */
 #define DEF_BUF_SIZE (16*1024)
 #define DEF_MAX_INITIAL_BUF_SIZE (16 * 1024 * 1024)
 #define ISAL_BEST_SPEED ISAL_DEF_MIN_LEVEL
 #define ISAL_BEST_COMPRESSION ISAL_DEF_MAX_LEVEL
 #define ISAL_DEFAULT_COMPRESSION 2
 #define COMP_DEFLATE IGZIP_DEFLATE
@@ -313,15 +321,18 @@
             obuflen = arrange_output_buffer(&(zst.avail_out), &(zst.next_out), 
                                             &RetVal, obuflen);
             if (obuflen < 0) {
                 PyErr_SetString(PyExc_MemoryError,
                         "Unsufficient memory for buffer allocation");
                 goto error;
             }
+
+            Py_BEGIN_ALLOW_THREADS
             err = isal_deflate(&zst);
+            Py_END_ALLOW_THREADS
 
             if (err != COMP_OK) {
                 isal_deflate_error(err);
                 goto error;
             }
 
         } while (zst.avail_out == 0);
@@ -372,15 +383,18 @@
         do {
             bufsize = arrange_output_buffer(&(zst.avail_out), &(zst.next_out),
                                             &RetVal, bufsize);
             if (bufsize < 0) {
                 goto error;
             }
 
+            Py_BEGIN_ALLOW_THREADS
             err = isal_inflate(&zst);
+            Py_END_ALLOW_THREADS
+
             if (err != ISAL_DECOMP_OK) {
                 isal_inflate_error(err);
                 goto error;
             }
         } while (zst.avail_out == 0);
 
     } while (zst.block_state != ISAL_BLOCK_FINISH && ibuflen != 0);
```

### Comparing `isal-1.1.0/src/isal/isal_zlib.pyi` & `isal-1.2.0/src/isal/isal_zlib.pyi`

 * *Files identical despite different names*

### Comparing `isal-1.1.0/src/isal/isal_zlibmodule.c` & `isal-1.2.0/src/isal/isal_zlibmodule.c`

 * *Files 1% similar despite different names*

```diff
@@ -170,15 +170,23 @@
     if (nargs > 1) {
         value = (uint32_t)PyLong_AsUnsignedLongMask(args[1]);
         if (value == (uint32_t)-1 && PyErr_Occurred()) {
             PyBuffer_Release(&data);
             return NULL;
         }
     }
-    value = isal_adler32(value, data.buf, (uint64_t)data.len);
+    uint64_t buffer_length = (uint64_t)data.len;
+    /* Do not drop GIL for small values as it is too much overhead */
+    if (buffer_length > 5 * 1024) {
+        Py_BEGIN_ALLOW_THREADS
+        value = isal_adler32(value, data.buf, buffer_length);
+        Py_END_ALLOW_THREADS
+    } else {
+        value = isal_adler32(value, data.buf, buffer_length);
+    }
     return_value = PyLong_FromUnsignedLong(value & 0xffffffffU);
     PyBuffer_Release(&data);
     return return_value;
 }
 
 PyDoc_STRVAR(zlib_crc32__doc__,
 "crc32($module, data, value=0, /)\n"
@@ -215,15 +223,23 @@
     if (nargs > 1) {
         value = (uint32_t)PyLong_AsUnsignedLongMask(args[1]);
         if (value == (uint32_t)-1 && PyErr_Occurred()) {
             PyBuffer_Release(&data);
             return NULL;
         }
     }
-    value = crc32_gzip_refl(value, data.buf, (uint64_t)data.len);
+    uint64_t buffer_length = (uint64_t)data.len;
+    /* Do not drop GIL for small values as it is too much overhead */
+    if (buffer_length > 5 * 1024) {
+        Py_BEGIN_ALLOW_THREADS
+        value = crc32_gzip_refl(value, data.buf, buffer_length);
+        Py_END_ALLOW_THREADS
+    } else {
+        value = crc32_gzip_refl(value, data.buf, buffer_length);
+    }
     return_value = PyLong_FromUnsignedLong(value & 0xffffffffU);
     PyBuffer_Release(&data);
     return return_value;
 }
 PyDoc_STRVAR(zlib_compress__doc__,
 "compress($module, data, /, level=ISAL_DEFAULT_COMPRESSION, wbits=MAX_WBITS)\n"
 "--\n"
@@ -321,57 +337,67 @@
 
 typedef struct
 {
     PyObject_HEAD
     uint8_t *level_buf;
     PyObject *zdict;
     int is_initialised;
+    PyThread_type_lock lock;
     // isal_zstream should be at the bottom as it contains buffers inside the struct.
     struct isal_zstream zst;
 } compobject;
 
 static void
 Comp_dealloc(compobject *self)
 {
     if (self->is_initialised && self->level_buf != NULL)
         PyMem_Free(self->level_buf);
+    PyThread_free_lock(self->lock);
     Py_XDECREF(self->zdict);
     Py_TYPE(self)->tp_free((PyObject *)self);
 }
 
 static compobject *
 newcompobject()
 {
     compobject *self;
     self = PyObject_New(compobject, &IsalZlibCompType);
     if (self == NULL)
         return NULL;
     self->is_initialised = 0;
     self->zdict = NULL;
     self->level_buf = NULL;
+    self->lock = PyThread_allocate_lock();
+    if (self->lock == NULL) {
+        Py_DECREF(self);
+        PyErr_SetString(PyExc_MemoryError, "Unable to allocate lock");
+        return NULL;
+    }
     return self;
 }
 
 
 typedef struct
 {
     PyObject_HEAD
     PyObject *unused_data;
     PyObject *unconsumed_tail;
     PyObject *zdict;
     int is_initialised;
     int method_set;
     char eof;
+    PyThread_type_lock lock;
     // inflate_state should be at the bottom as it contains buffers inside the struct.
     struct inflate_state zst;
 } decompobject;
 
 static void
 Decomp_dealloc(decompobject *self)
 {
+    PyThread_free_lock(self->lock);
     Py_XDECREF(self->unused_data);
     Py_XDECREF(self->unconsumed_tail);
     Py_XDECREF(self->zdict);
     Py_TYPE(self)->tp_free((PyObject *)self);
 }
 
 static int
@@ -416,14 +442,20 @@
         return NULL;
     }
     self->unconsumed_tail = PyBytes_FromStringAndSize("", 0);
     if (self->unconsumed_tail == NULL) {
         Py_DECREF(self);
         return NULL;
     }
+        self->lock = PyThread_allocate_lock();
+    if (self->lock == NULL) {
+        Py_DECREF(self);
+        PyErr_SetString(PyExc_MemoryError, "Unable to allocate lock");
+        return NULL;
+    }
     return self;
 }
 
 static PyObject *
 isal_zlib_compressobj_impl(PyObject *module, int level, int method, int wbits,
                            int memLevel, int strategy, Py_buffer *zdict)
 {
@@ -558,26 +590,30 @@
 isal_zlib_Compress_compress_impl(compobject *self, Py_buffer *data)
 /*[clinic end generated code: output=5d5cd791cbc6a7f4 input=0d95908d6e64fab8]*/
 {
     PyObject *RetVal = NULL;
     Py_ssize_t ibuflen, obuflen = DEF_BUF_SIZE;
     int err;
 
+    ENTER_ZLIB(self);
+
     self->zst.next_in = data->buf;
     ibuflen = data->len;
 
     do {
         arrange_input_buffer(&(self->zst.avail_in), &ibuflen);
         do {
             obuflen = arrange_output_buffer(&(self->zst.avail_out),
                                             &(self->zst.next_out), &RetVal, obuflen);
             if (obuflen < 0)
                 goto error;
 
+            Py_BEGIN_ALLOW_THREADS
             err = isal_deflate(&self->zst);
+            Py_END_ALLOW_THREADS
 
             if (err != COMP_OK) {
                 isal_deflate_error(err);
                 goto error;
             }
         } while (self->zst.avail_out == 0);
         assert(self->zst.avail_in == 0);
@@ -587,14 +623,15 @@
     if (_PyBytes_Resize(&RetVal, self->zst.next_out -
                         (uint8_t *)PyBytes_AS_STRING(RetVal)) == 0)
         goto success;
 
  error:
     Py_CLEAR(RetVal);
  success:
+    LEAVE_ZLIB(self);
     return RetVal;
 }
 
 /* Helper for objdecompress() and flush(). Saves any unconsumed input data in
    self->unused_data or self->unconsumed_tail, as appropriate. */
 static int
 save_unconsumed_input(decompobject *self, Py_buffer *data, int err)
@@ -664,21 +701,24 @@
             self->zst.crc_flag = ISAL_GZIP;
         }
         else {
             self->zst.crc_flag = ISAL_ZLIB;
         }
         self->method_set = 1;
     }
-    self->zst.next_in = data->buf;
-    ibuflen = data->len;
 
     /* limit amount of data allocated to max_length */
     if (max_length && obuflen > max_length)
         obuflen = max_length;
 
+    ENTER_ZLIB(self);
+
+    self->zst.next_in = data->buf;
+    ibuflen = data->len;
+
     do {
         arrange_input_buffer(&(self->zst.avail_in), &ibuflen);
 
         do {
             obuflen = arrange_output_buffer_with_maximum(&(self->zst.avail_out),
                                                          &(self->zst.next_out), 
                                                          &RetVal,
@@ -689,22 +729,39 @@
                 }
                 PyErr_NoMemory();
             }
             if (obuflen < 0) {
                 goto abort;
             }
 
+            Py_BEGIN_ALLOW_THREADS
             err = isal_inflate(&self->zst);
-            if (err != ISAL_DECOMP_OK){
-                isal_inflate_error(err);
-                goto abort;
+            Py_END_ALLOW_THREADS
+            
+            switch(err) {
+                case ISAL_DECOMP_OK:
+                    break;
+                case ISAL_NEED_DICT:                
+                    if  (self->zdict != NULL) {
+                        if (set_inflate_zdict(self) < 0) {
+                            goto abort;
+                        }
+                        else 
+                            break;
+                    }
+                    else {
+                        isal_inflate_error(err);
+                        goto abort;
+                    }
+                default:
+                    isal_inflate_error(err);
+                    goto abort;
             }
 
-        } while (self->zst.avail_out == 0 && 
-                 self->zst.block_state != ISAL_BLOCK_FINISH);
+        } while (self->zst.avail_out == 0 || err == ISAL_NEED_DICT);
 
     } while (self->zst.block_state != ISAL_BLOCK_FINISH && ibuflen != 0);
 
  save:
     if (save_unconsumed_input(self, data, err) < 0)
         goto abort;
 
@@ -715,29 +772,34 @@
     if (_PyBytes_Resize(&RetVal, self->zst.next_out -
                         (uint8_t *)PyBytes_AS_STRING(RetVal)) == 0)
         goto success;
 
  abort:
     Py_CLEAR(RetVal);
  success:
+    LEAVE_ZLIB(self);
     return RetVal;
 }
 
 static PyObject *
 isal_zlib_Compress_flush_impl(compobject *self, int mode)
 {
     int err;
     Py_ssize_t length = DEF_BUF_SIZE;
     PyObject *RetVal = NULL;
 
     /* Flushing with Z_NO_FLUSH is a no-op, so there's no point in
        doing any work at all; just return an empty string. */
     if (mode == Z_NO_FLUSH) {
-        return PyBytes_FromStringAndSize(NULL, 0);
-    } else if (mode == Z_FINISH) {
+        return PyBytes_FromStringAndSize(NULL, 0);        
+    } 
+    
+    ENTER_ZLIB(self);
+
+    if (mode == Z_FINISH) {
         self->zst.flush = FULL_FLUSH;
         self->zst.end_of_stream = 1;
     } else if (mode == Z_FULL_FLUSH){
         self->zst.flush = FULL_FLUSH;
     } else if (mode == Z_SYNC_FLUSH) {
         self->zst.flush = SYNC_FLUSH;
     } else {
@@ -752,15 +814,17 @@
         length = arrange_output_buffer(&(self->zst.avail_out), 
                                        &(self->zst.next_out), &RetVal, length);
         if (length < 0) {
             Py_CLEAR(RetVal);
             goto error;
         }
 
+        Py_BEGIN_ALLOW_THREADS
         err = isal_deflate(&self->zst);
+        Py_END_ALLOW_THREADS
 
         if (err != COMP_OK) {
             isal_deflate_error(err);
             Py_CLEAR(RetVal);
             goto error;
         }
     } while (self->zst.avail_out == 0);
@@ -780,14 +844,15 @@
     }
 
     if (_PyBytes_Resize(&RetVal, self->zst.next_out -
                         (uint8_t *)PyBytes_AS_STRING(RetVal)) < 0)
         Py_CLEAR(RetVal);
 
  error:
+    LEAVE_ZLIB(self);
     return RetVal;
 }
 
 static PyObject *
 isal_zlib_Decompress_flush_impl(decompobject *self, Py_ssize_t length)
 {
     int err;
@@ -796,15 +861,18 @@
     Py_ssize_t ibuflen;
 
     if (length <= 0) {
         PyErr_SetString(PyExc_ValueError, "length must be greater than zero");
         return NULL;
     }
 
+    ENTER_ZLIB(self);
+
     if (PyObject_GetBuffer(self->unconsumed_tail, &data, PyBUF_SIMPLE) == -1) {
+        LEAVE_ZLIB(self);
         return NULL;
     }
 
     self->zst.next_in = data.buf;
     ibuflen = data.len;
 
     do {
@@ -813,15 +881,17 @@
         do {
             length = arrange_output_buffer(&(self->zst.avail_out),
                                            &(self->zst.next_out), 
                                            &RetVal, length);
             if (length < 0)
                 goto abort;
 
+            Py_BEGIN_ALLOW_THREADS
             err = isal_inflate(&self->zst);
+            Py_END_ALLOW_THREADS
 
             if (err != ISAL_DECOMP_OK) {
                 isal_inflate_error(err);
                 goto abort;
             }
 
         } while (self->zst.avail_out == 0 && 
@@ -842,14 +912,15 @@
                         (uint8_t *)PyBytes_AS_STRING(RetVal)) == 0)
         goto success;
 
  abort:
     Py_CLEAR(RetVal);
  success:
     PyBuffer_Release(&data);
+    LEAVE_ZLIB(self);
     return RetVal;
 }
 
 PyDoc_STRVAR(isal_zlib_compressobj__doc__,
 "compressobj($module, /, level=ISAL_DEFAULT_COMPRESSION, method=DEFLATED,\n"
 "            wbits=MAX_WBITS, memLevel=DEF_MEM_LEVEL,\n"
 "            strategy=Z_DEFAULT_STRATEGY, zdict=None)\n"
```

### Comparing `isal-1.1.0/src/isal.egg-info/PKG-INFO` & `isal-1.2.0/src/isal.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: isal
-Version: 1.1.0
+Version: 1.2.0
 Summary: Faster zlib and gzip compatible compression and decompression by providing python bindings for the ISA-L library.
 Home-page: https://github.com/pycompression/python-isal
 Author: Leiden University Medical Center
 Author-email: r.h.p.vorderman@lumc.nl
 License: PSF-2.0
 Keywords: isal isa-l compression deflate gzip igzip
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -136,20 +136,20 @@
 Python-isal supports a limited amount of platforms for which wheels have been
 made available. To prevent your users from running into issues when installing
 your project please list a python-isal dependency as follows.
 
 ``setup.cfg``::
 
     install_requires =
-        isal; platform.machine == "x86_64" or platform.machine == "AMD64"
+        isal; platform.machine == "x86_64" or platform.machine == "AMD64" or platform.machine == "aarch64"
 
 ``setup.py``::
 
     extras_require={
-        ":platform.machine == 'x86_64' or platform.machine == 'AMD64'": ['isal']
+        ":platform.machine == 'x86_64' or platform.machine == 'AMD64' or platform.machine == 'aarch64'": ['isal']
     },
 
 .. dependency end
 
 Differences with zlib and gzip modules
 --------------------------------------
```

### Comparing `isal-1.1.0/src/isal.egg-info/SOURCES.txt` & `isal-1.2.0/src/isal.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -400,8 +400,13 @@
 src/isal/isa-l/tools/remove_trailing_whitespace.sh
 src/isal/isa-l/tools/test_autorun.sh
 src/isal/isa-l/tools/test_checks.sh
 src/isal/isa-l/tools/test_extended.sh
 src/isal/isa-l/tools/test_fuzz.sh
 src/isal/isa-l/tools/test_tools.sh
 src/isal/isa-l/tools/yasm-cet-filter.sh
-src/isal/isa-l/tools/yasm-filter.sh
+src/isal/isa-l/tools/yasm-filter.sh
+tests/test_compat.py
+tests/test_gzip_compliance.py
+tests/test_igzip.py
+tests/test_igzip_lib.py
+tests/test_zlib_compliance.py
```

