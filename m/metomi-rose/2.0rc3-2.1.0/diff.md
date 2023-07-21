# Comparing `tmp/metomi-rose-2.0rc3.tar.gz` & `tmp/metomi-rose-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metomi-rose-2.0rc3.tar", last modified: Fri May 20 12:44:04 2022, max compression
+gzip compressed data, was "metomi-rose-2.1.0.tar", last modified: Fri Jul 21 11:04:05 2023, max compression
```

## Comparing `metomi-rose-2.0rc3.tar` & `metomi-rose-2.1.0.tar`

### file list

```diff
@@ -1,425 +1,393 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.479482 metomi-rose-2.0rc3/
--rw-r--r--   0 runner    (1001) docker     (121)    35147 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/COPYING
--rw-r--r--   0 runner    (1001) docker     (121)      116 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     3190 2022-05-20 12:44:04.479482 metomi-rose-2.0rc3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2204 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.447482 metomi-rose-2.0rc3/metomi/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.455482 metomi-rose-2.0rc3/metomi/rose/
--rw-r--r--   0 runner    (1001) docker     (121)     4031 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    19321 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/app_run.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.455482 metomi-rose-2.0rc3/metomi/rose/apps/
--rw-r--r--   0 runner    (1001) docker     (121)      818 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/apps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.455482 metomi-rose-2.0rc3/metomi/rose/apps/ana_builtin/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/apps/ana_builtin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    21577 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/apps/ana_builtin/grepper.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.455482 metomi-rose-2.0rc3/metomi/rose/apps/comparisons/
--rw-r--r--   0 runner    (1001) docker     (121)     7501 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/apps/comparisons/cumf.py
--rw-r--r--   0 runner    (1001) docker     (121)     3436 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/apps/comparisons/exact.py
--rw-r--r--   0 runner    (1001) docker     (121)     1803 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/apps/comparisons/mandatory.py
--rw-r--r--   0 runner    (1001) docker     (121)     1757 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/apps/comparisons/output_grepper.py
--rw-r--r--   0 runner    (1001) docker     (121)     1816 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/apps/comparisons/prohibited.py
--rw-r--r--   0 runner    (1001) docker     (121)     4929 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/apps/comparisons/within.py
--rw-r--r--   0 runner    (1001) docker     (121)    11819 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/apps/fcm_make.py
--rw-r--r--   0 runner    (1001) docker     (121)    33581 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/apps/rose_ana.py
--rw-r--r--   0 runner    (1001) docker     (121)    21791 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/apps/rose_ana_v1.py
--rw-r--r--   0 runner    (1001) docker     (121)    23070 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/apps/rose_arch.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.455482 metomi-rose-2.0rc3/metomi/rose/apps/rose_arch_compressions/
--rw-r--r--   0 runner    (1001) docker     (121)      818 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/apps/rose_arch_compressions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1827 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/apps/rose_arch_compressions/rose_arch_gzip.py
--rw-r--r--   0 runner    (1001) docker     (121)     2851 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/apps/rose_arch_compressions/rose_arch_tar.py
--rw-r--r--   0 runner    (1001) docker     (121)    20796 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/apps/rose_bunch.py
--rw-r--r--   0 runner    (1001) docker     (121)    12346 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/apps/rose_prune.py
--rw-r--r--   0 runner    (1001) docker     (121)     7988 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/c3.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    12092 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/check_software.py
--rw-r--r--   0 runner    (1001) docker     (121)     5772 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/checksum.py
--rw-r--r--   0 runner    (1001) docker     (121)    64089 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/config.py
--rw-r--r--   0 runner    (1001) docker     (121)     7736 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/config_cli.py
--rw-r--r--   0 runner    (1001) docker     (121)    11281 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/config_diff.py
--rw-r--r--   0 runner    (1001) docker     (121)     3076 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/config_dump.py
--rw-r--r--   0 runner    (1001) docker     (121)     5053 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/config_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.455482 metomi-rose-2.0rc3/metomi/rose/config_processors/
--rw-r--r--   0 runner    (1001) docker     (121)      818 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/config_processors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2150 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/config_processors/env.py
--rw-r--r--   0 runner    (1001) docker     (121)    33931 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/config_processors/fileinstall.py
--rw-r--r--   0 runner    (1001) docker     (121)    15431 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/config_tree.py
--rw-r--r--   0 runner    (1001) docker     (121)    17852 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/date.py
--rw-r--r--   0 runner    (1001) docker     (121)    10193 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/date_cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     5855 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/env.py
--rw-r--r--   0 runner    (1001) docker     (121)     3305 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/env_cat.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.443482 metomi-rose-2.0rc3/metomi/rose/etc/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.443482 metomi-rose-2.0rc3/metomi/rose/etc/lib/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.455482 metomi-rose-2.0rc3/metomi/rose/etc/lib/bash/
--rw-r--r--   0 runner    (1001) docker     (121)     3469 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/lib/bash/rose_log
--rw-r--r--   0 runner    (1001) docker     (121)     2089 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/lib/bash/rose_usage
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.443482 metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.443482 metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/fcm_make/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.455482 metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/fcm_make/HEAD/
--rw-r--r--   0 runner    (1001) docker     (121)     1444 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/fcm_make/HEAD/rose-meta.conf
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.455482 metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose-all/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.443482 metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose-all/etc/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.455482 metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose-all/etc/images/
--rw-r--r--   0 runner    (1001) docker     (121)     1084 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose-all/etc/images/icon.png
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose-all/rose-meta.conf
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.455482 metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose-app-conf/
--rw-r--r--   0 runner    (1001) docker     (121)     3755 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose-app-conf/rose-meta.conf
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.443482 metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose-demo-baked-alaska/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.455482 metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose-demo-baked-alaska/HEAD/
--rw-r--r--   0 runner    (1001) docker     (121)      165 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose-demo-baked-alaska/HEAD/rose-meta.conf
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.455482 metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose-demo-baked-alaska/vn1.0/
--rw-r--r--   0 runner    (1001) docker     (121)      323 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose-demo-baked-alaska/vn1.0/rose-meta.conf
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.455482 metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose-demo-baked-alaska/vn2.0/
--rw-r--r--   0 runner    (1001) docker     (121)      168 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose-demo-baked-alaska/vn2.0/rose-meta.conf
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.443482 metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose-demo-baked-alaska-icecream/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.455482 metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose-demo-baked-alaska-icecream/HEAD/
--rw-r--r--   0 runner    (1001) docker     (121)      104 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose-demo-baked-alaska-icecream/HEAD/rose-meta.conf
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.455482 metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose-demo-baked-alaska-icecream/vn1.0/
--rw-r--r--   0 runner    (1001) docker     (121)      184 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose-demo-baked-alaska-icecream/vn1.0/rose-meta.conf
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.455482 metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose-demo-baked-alaska-icecream/vn2.0/
--rw-r--r--   0 runner    (1001) docker     (121)      101 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose-demo-baked-alaska-icecream/vn2.0/rose-meta.conf
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.443482 metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose-demo-baked-alaska-sponge/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.455482 metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose-demo-baked-alaska-sponge/HEAD/
--rw-r--r--   0 runner    (1001) docker     (121)       87 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose-demo-baked-alaska-sponge/HEAD/rose-meta.conf
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.455482 metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose-demo-baked-alaska-sponge/vn1.0/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.443482 metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose-demo-baked-alaska-sponge/vn1.0/lib/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.443482 metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose-demo-baked-alaska-sponge/vn1.0/lib/python/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.455482 metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose-demo-baked-alaska-sponge/vn1.0/lib/python/macros/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose-demo-baked-alaska-sponge/vn1.0/lib/python/macros/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1555 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose-demo-baked-alaska-sponge/vn1.0/lib/python/macros/desoggy.py
--rw-r--r--   0 runner    (1001) docker     (121)       84 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose-demo-baked-alaska-sponge/vn1.0/rose-meta.conf
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.455482 metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose-demo-baked-alaska-sponge/vn2.0/
--rw-r--r--   0 runner    (1001) docker     (121)       84 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose-demo-baked-alaska-sponge/vn2.0/rose-meta.conf
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.455482 metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose-demo-upgrade/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.459482 metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose-demo-upgrade/HEAD/
--rw-r--r--   0 runner    (1001) docker     (121)      551 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose-demo-upgrade/HEAD/rose-meta.conf
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.443482 metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose-demo-upgrade/etc/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.459482 metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose-demo-upgrade/etc/garden0.4/
--rw-r--r--   0 runner    (1001) docker     (121)       87 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose-demo-upgrade/etc/garden0.4/rose-macro-add.conf
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.459482 metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose-demo-upgrade/garden0.1/
--rw-r--r--   0 runner    (1001) docker     (121)      210 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose-demo-upgrade/garden0.1/rose-meta.conf
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.459482 metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose-demo-upgrade/garden0.2/
--rw-r--r--   0 runner    (1001) docker     (121)      283 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose-demo-upgrade/garden0.2/rose-meta.conf
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.459482 metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose-demo-upgrade/garden0.3/
--rw-r--r--   0 runner    (1001) docker     (121)      328 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose-demo-upgrade/garden0.3/rose-meta.conf
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.459482 metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose-demo-upgrade/garden0.4/
--rw-r--r--   0 runner    (1001) docker     (121)      361 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose-demo-upgrade/garden0.4/rose-meta.conf
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.459482 metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose-demo-upgrade/garden0.9/
--rw-r--r--   0 runner    (1001) docker     (121)      614 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose-demo-upgrade/garden0.9/rose-meta.conf
--rw-r--r--   0 runner    (1001) docker     (121)     3887 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose-demo-upgrade/versions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.459482 metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose-demo-upgrade-null/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.459482 metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose-demo-upgrade-null/0.1/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose-demo-upgrade-null/0.1/rose-meta.conf
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.459482 metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose-demo-upgrade-null/0.2/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose-demo-upgrade-null/0.2/rose-meta.conf
--rw-r--r--   0 runner    (1001) docker     (121)      605 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose-demo-upgrade-null/versions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.459482 metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose-suite-conf/
--rw-r--r--   0 runner    (1001) docker     (121)     2668 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose-suite-conf/rose-meta.conf
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.459482 metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose-suite-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1909 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose-suite-info/rose-meta.conf
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.443482 metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose_bunch/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.459482 metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose_bunch/HEAD/
--rw-r--r--   0 runner    (1001) docker     (121)     2760 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose_bunch/HEAD/rose-meta.conf
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.443482 metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose_prune/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.459482 metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose_prune/HEAD/
--rw-r--r--   0 runner    (1001) docker     (121)     3602 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose_prune/HEAD/rose-meta.conf
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.459482 metomi-rose-2.0rc3/metomi/rose/etc/syntax/
--rw-r--r--   0 runner    (1001) docker     (121)     4866 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/syntax/rose-conf-mode.el
--rw-r--r--   0 runner    (1001) docker     (121)     3260 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/syntax/rose-conf.lang
--rw-r--r--   0 runner    (1001) docker     (121)     1929 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/syntax/rose-conf.vim
--rw-r--r--   0 runner    (1001) docker     (121)     1809 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/syntax/rose-conf.xml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.459482 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/
--rw-r--r--   0 runner    (1001) docker     (121)      111 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/api-keys
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.459482 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/consolidation-tutorial/
--rw-r--r--   0 runner    (1001) docker     (121)       36 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/consolidation-tutorial/.validate
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.459482 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/consolidation-tutorial/bin/
--rwxr-xr-x   0 runner    (1001) docker     (121)     3548 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/consolidation-tutorial/bin/consolidate-observations
--rwxr-xr-x   0 runner    (1001) docker     (121)     8469 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/consolidation-tutorial/bin/forecast
--rwxr-xr-x   0 runner    (1001) docker     (121)     3187 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/consolidation-tutorial/bin/get-observations
--rwxr-xr-x   0 runner    (1001) docker     (121)     5544 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/consolidation-tutorial/bin/get-rainfall
--rwxr-xr-x   0 runner    (1001) docker     (121)     3036 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/consolidation-tutorial/bin/post-process
--rw-r--r--   0 runner    (1001) docker     (121)     4335 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/consolidation-tutorial/flow.cylc
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.443482 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/consolidation-tutorial/lib/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.459482 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/consolidation-tutorial/lib/python/
--rw-r--r--   0 runner    (1001) docker     (121)     2132 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/consolidation-tutorial/lib/python/mecator.py
--rw-r--r--   0 runner    (1001) docker     (121)     9230 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/consolidation-tutorial/lib/python/util.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.459482 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/consolidation-tutorial/lib/template/
--rw-r--r--   0 runner    (1001) docker     (121)     2606 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/consolidation-tutorial/lib/template/map.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.459482 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/cylc-forecasting-suite/
--rw-r--r--   0 runner    (1001) docker     (121)      198 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/cylc-forecasting-suite/.validate
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.459482 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/cylc-forecasting-suite/bin/
--rwxr-xr-x   0 runner    (1001) docker     (121)     3548 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/cylc-forecasting-suite/bin/consolidate-observations
--rwxr-xr-x   0 runner    (1001) docker     (121)     8469 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/cylc-forecasting-suite/bin/forecast
--rwxr-xr-x   0 runner    (1001) docker     (121)     3187 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/cylc-forecasting-suite/bin/get-observations
--rwxr-xr-x   0 runner    (1001) docker     (121)     5544 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/cylc-forecasting-suite/bin/get-rainfall
--rwxr-xr-x   0 runner    (1001) docker     (121)     3036 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/cylc-forecasting-suite/bin/post-process
--rw-r--r--   0 runner    (1001) docker     (121)     3827 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/cylc-forecasting-suite/flow.cylc
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.447482 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/cylc-forecasting-suite/lib/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.459482 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/cylc-forecasting-suite/lib/python/
--rw-r--r--   0 runner    (1001) docker     (121)     2132 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/cylc-forecasting-suite/lib/python/mecator.py
--rw-r--r--   0 runner    (1001) docker     (121)     9230 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/cylc-forecasting-suite/lib/python/util.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.459482 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/cylc-forecasting-suite/lib/template/
--rw-r--r--   0 runner    (1001) docker     (121)     2606 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/cylc-forecasting-suite/lib/template/map.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.459482 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/failif-warnif/
--rw-r--r--   0 runner    (1001) docker     (121)       63 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/failif-warnif/.validate
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.459482 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/failif-warnif/meta/
--rw-r--r--   0 runner    (1001) docker     (121)     2212 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/failif-warnif/meta/rose-meta.conf
--rw-r--r--   0 runner    (1001) docker     (121)      225 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/failif-warnif/rose-app.conf
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.459482 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/forecast-script/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/forecast-script/.validate
--rwxr-xr-x   0 runner    (1001) docker     (121)     8469 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/forecast-script/forecast
--rw-r--r--   0 runner    (1001) docker     (121)     9230 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/forecast-script/util.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.459482 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/inheritance-tutorial/
--rw-r--r--   0 runner    (1001) docker     (121)      911 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/inheritance-tutorial/flow.cylc
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.463482 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/map-template/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/map-template/.validate
--rw-r--r--   0 runner    (1001) docker     (121)     2606 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/map-template/map-template.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.463482 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/metadata-tutorial/
--rw-r--r--   0 runner    (1001) docker     (121)       42 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/metadata-tutorial/.validate
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.463482 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/metadata-tutorial/bin/
--rwxr-xr-x   0 runner    (1001) docker     (121)     8469 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/metadata-tutorial/bin/forecast
--rw-r--r--   0 runner    (1001) docker     (121)     9230 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/metadata-tutorial/bin/util.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.463482 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/metadata-tutorial/file/
--rw-r--r--   0 runner    (1001) docker     (121)     2606 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/metadata-tutorial/file/map-template.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.463482 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/metadata-tutorial/file/test-data/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/metadata-tutorial/file/test-data/.validate
--rw-r--r--   0 runner    (1001) docker     (121)    33085 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/metadata-tutorial/file/test-data/rainfall.csv
--rw-r--r--   0 runner    (1001) docker     (121)    35829 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/metadata-tutorial/file/test-data/wind_20171101T0000Z_x.csv
--rw-r--r--   0 runner    (1001) docker     (121)    38004 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/metadata-tutorial/file/test-data/wind_20171101T0000Z_y.csv
--rw-r--r--   0 runner    (1001) docker     (121)      832 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/metadata-tutorial/rose-app.conf
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.463482 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/queues-tutorial/
--rw-r--r--   0 runner    (1001) docker     (121)      929 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/queues-tutorial/flow.cylc
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.463482 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/retries-tutorial/
--rw-r--r--   0 runner    (1001) docker     (121)      393 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/retries-tutorial/flow.cylc
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.463482 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-stem/
--rw-r--r--   0 runner    (1001) docker     (121)      268 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-stem/.validate
--rw-r--r--   0 runner    (1001) docker     (121)     1304 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-stem/kgo.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.463482 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-stem/rose-stem/
--rw-r--r--   0 runner    (1001) docker     (121)     1973 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-stem/rose-stem/flow.cylc
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-stem/rose-stem/rose-suite.conf
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.463482 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-stem/src/
--rw-r--r--   0 runner    (1001) docker     (121)     1307 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-stem/src/spaceship_command.f90
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.463482 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-suite-tutorial/
--rw-r--r--   0 runner    (1001) docker     (121)      129 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-suite-tutorial/.validate
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.447482 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-suite-tutorial/app/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.463482 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-suite-tutorial/app/forecast/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.463482 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-suite-tutorial/app/forecast/bin/
--rwxr-xr-x   0 runner    (1001) docker     (121)     8469 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-suite-tutorial/app/forecast/bin/forecast
--rw-r--r--   0 runner    (1001) docker     (121)     9230 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-suite-tutorial/app/forecast/bin/util.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.463482 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-suite-tutorial/app/forecast/file/
--rw-r--r--   0 runner    (1001) docker     (121)     2606 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-suite-tutorial/app/forecast/file/map-template.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.463482 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-suite-tutorial/app/forecast/file/test-data/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-suite-tutorial/app/forecast/file/test-data/.validate
--rw-r--r--   0 runner    (1001) docker     (121)    33085 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-suite-tutorial/app/forecast/file/test-data/rainfall.csv
--rw-r--r--   0 runner    (1001) docker     (121)    35829 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-suite-tutorial/app/forecast/file/test-data/wind_20171101T0000Z_x.csv
--rw-r--r--   0 runner    (1001) docker     (121)    38004 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-suite-tutorial/app/forecast/file/test-data/wind_20171101T0000Z_y.csv
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.463482 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-suite-tutorial/app/forecast/meta/
--rw-r--r--   0 runner    (1001) docker     (121)      994 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-suite-tutorial/app/forecast/meta/rose-meta.conf
--rw-r--r--   0 runner    (1001) docker     (121)      333 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-suite-tutorial/app/forecast/rose-app.conf
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.463482 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-suite-tutorial/bin/
--rwxr-xr-x   0 runner    (1001) docker     (121)     3548 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-suite-tutorial/bin/consolidate-observations
--rwxr-xr-x   0 runner    (1001) docker     (121)     3187 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-suite-tutorial/bin/get-observations
--rwxr-xr-x   0 runner    (1001) docker     (121)     5544 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-suite-tutorial/bin/get-rainfall
--rwxr-xr-x   0 runner    (1001) docker     (121)     3036 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-suite-tutorial/bin/post-process
--rw-r--r--   0 runner    (1001) docker     (121)     3827 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-suite-tutorial/flow.cylc
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.447482 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-suite-tutorial/lib/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.463482 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-suite-tutorial/lib/python/
--rw-r--r--   0 runner    (1001) docker     (121)     2132 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-suite-tutorial/lib/python/mecator.py
--rw-r--r--   0 runner    (1001) docker     (121)     9230 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-suite-tutorial/lib/python/util.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.463482 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/
--rw-r--r--   0 runner    (1001) docker     (121)      166 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/.validate
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.447482 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/app/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.463482 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/app/forecast/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.463482 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/app/forecast/bin/
--rwxr-xr-x   0 runner    (1001) docker     (121)     8469 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/app/forecast/bin/forecast
--rw-r--r--   0 runner    (1001) docker     (121)     9230 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/app/forecast/bin/util.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.467482 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/app/forecast/file/
--rw-r--r--   0 runner    (1001) docker     (121)     2606 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/app/forecast/file/map-template.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.467482 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/app/forecast/file/test-data/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/app/forecast/file/test-data/.validate
--rw-r--r--   0 runner    (1001) docker     (121)    33085 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/app/forecast/file/test-data/rainfall.csv
--rw-r--r--   0 runner    (1001) docker     (121)    35829 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/app/forecast/file/test-data/wind_20171101T0000Z_x.csv
--rw-r--r--   0 runner    (1001) docker     (121)    38004 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/app/forecast/file/test-data/wind_20171101T0000Z_y.csv
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.467482 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/app/forecast/meta/
--rw-r--r--   0 runner    (1001) docker     (121)      994 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/app/forecast/meta/rose-meta.conf
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.467482 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/app/forecast/opt/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/app/forecast/opt/rose-app-test.conf
--rw-r--r--   0 runner    (1001) docker     (121)      442 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/app/forecast/rose-app.conf
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.467482 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/bin/
--rwxr-xr-x   0 runner    (1001) docker     (121)     3548 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/bin/consolidate-observations
--rwxr-xr-x   0 runner    (1001) docker     (121)     8469 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/bin/forecast
--rwxr-xr-x   0 runner    (1001) docker     (121)     3187 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/bin/get-observations
--rwxr-xr-x   0 runner    (1001) docker     (121)     5544 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/bin/get-rainfall
--rwxr-xr-x   0 runner    (1001) docker     (121)     3036 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/bin/post-process
--rw-r--r--   0 runner    (1001) docker     (121)     2704 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/flow.cylc
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.447482 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/lib/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.467482 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/lib/python/
--rw-r--r--   0 runner    (1001) docker     (121)     2132 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/lib/python/mecator.py
--rw-r--r--   0 runner    (1001) docker     (121)     9230 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/lib/python/util.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.467482 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/meta/
--rw-r--r--   0 runner    (1001) docker     (121)       99 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/meta/rose-meta.conf
--rw-r--r--   0 runner    (1001) docker     (121)      115 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/rose-suite.conf
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.467482 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/runtime-introduction/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.467482 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/runtime-introduction/bin/
--rwxr-xr-x   0 runner    (1001) docker     (121)      457 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/runtime-introduction/bin/get-observations
--rw-r--r--   0 runner    (1001) docker     (121)     1573 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/runtime-introduction/flow.cylc
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.467482 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/runtime-tutorial/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/runtime-tutorial/.validate
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.467482 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/runtime-tutorial/bin/
--rwxr-xr-x   0 runner    (1001) docker     (121)     3548 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/runtime-tutorial/bin/consolidate-observations
--rwxr-xr-x   0 runner    (1001) docker     (121)     8469 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/runtime-tutorial/bin/forecast
--rwxr-xr-x   0 runner    (1001) docker     (121)     3187 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/runtime-tutorial/bin/get-observations
--rwxr-xr-x   0 runner    (1001) docker     (121)     5544 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/runtime-tutorial/bin/get-rainfall
--rwxr-xr-x   0 runner    (1001) docker     (121)     3036 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/runtime-tutorial/bin/post-process
--rw-r--r--   0 runner    (1001) docker     (121)     1434 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/runtime-tutorial/flow.cylc
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.447482 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/runtime-tutorial/lib/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.467482 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/runtime-tutorial/lib/python/
--rw-r--r--   0 runner    (1001) docker     (121)     2132 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/runtime-tutorial/lib/python/mecator.py
--rw-r--r--   0 runner    (1001) docker     (121)     9230 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/runtime-tutorial/lib/python/util.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.467482 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/runtime-tutorial/lib/template/
--rw-r--r--   0 runner    (1001) docker     (121)     2606 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/runtime-tutorial/lib/template/map.html
--rw-r--r--   0 runner    (1001) docker     (121)     2240 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/runtime-tutorial/runtime
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.467482 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/test-data/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/test-data/.validate
--rw-r--r--   0 runner    (1001) docker     (121)    33085 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/test-data/rainfall.csv
--rw-r--r--   0 runner    (1001) docker     (121)    35829 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/test-data/wind_20171101T0000Z_x.csv
--rw-r--r--   0 runner    (1001) docker     (121)    38004 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/test-data/wind_20171101T0000Z_y.csv
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.467482 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/widget/
--rw-r--r--   0 runner    (1001) docker     (121)       28 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/widget/.validate
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.447482 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/widget/meta/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.447482 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/widget/meta/lib/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.447482 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/widget/meta/lib/python/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.467482 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/widget/meta/lib/python/widget/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/widget/meta/lib/python/widget/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1695 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/widget/meta/lib/python/widget/username.py
--rw-r--r--   0 runner    (1001) docker     (121)       57 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/etc/tutorial/widget/rose-app.conf
--rw-r--r--   0 runner    (1001) docker     (121)     2031 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/external.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.467482 metomi-rose-2.0rc3/metomi/rose/formats/
--rw-r--r--   0 runner    (1001) docker     (121)     1039 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/formats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    14235 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/formats/namelist.py
--rw-r--r--   0 runner    (1001) docker     (121)     5893 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/fs_util.py
--rw-r--r--   0 runner    (1001) docker     (121)    24700 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/host_select.py
--rw-r--r--   0 runner    (1001) docker     (121)     2675 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/host_select_client.py
--rw-r--r--   0 runner    (1001) docker     (121)     9251 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/job_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.471482 metomi-rose-2.0rc3/metomi/rose/loc_handlers/
--rw-r--r--   0 runner    (1001) docker     (121)      856 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/loc_handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2179 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/loc_handlers/fs.py
--rw-r--r--   0 runner    (1001) docker     (121)     3318 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/loc_handlers/namelist.py
--rw-r--r--   0 runner    (1001) docker     (121)     3873 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/loc_handlers/rsync.py
--rw-r--r--   0 runner    (1001) docker     (121)     2415 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/loc_handlers/rsync_remote_check.py
--rw-r--r--   0 runner    (1001) docker     (121)     4116 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/loc_handlers/svn.py
--rw-r--r--   0 runner    (1001) docker     (121)    68500 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/macro.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.471482 metomi-rose-2.0rc3/metomi/rose/macros/
--rw-r--r--   0 runner    (1001) docker     (121)     2444 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/macros/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12374 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/macros/compulsory.py
--rw-r--r--   0 runner    (1001) docker     (121)     3474 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/macros/duplicate.py
--rw-r--r--   0 runner    (1001) docker     (121)     1708 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/macros/format.py
--rw-r--r--   0 runner    (1001) docker     (121)    16940 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/macros/rule.py
--rw-r--r--   0 runner    (1001) docker     (121)    26691 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/macros/trigger.py
--rw-r--r--   0 runner    (1001) docker     (121)    14522 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/macros/value.py
--rw-r--r--   0 runner    (1001) docker     (121)     7060 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/meta_type.py
--rw-r--r--   0 runner    (1001) docker     (121)    16583 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/metadata_check.py
--rw-r--r--   0 runner    (1001) docker     (121)     7432 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/metadata_gen.py
--rw-r--r--   0 runner    (1001) docker     (121)    13680 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/metadata_graph.py
--rw-r--r--   0 runner    (1001) docker     (121)     5436 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/namelist_dump.py
--rw-r--r--   0 runner    (1001) docker     (121)    43854 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/opt_parse.py
--rw-r--r--   0 runner    (1001) docker     (121)    13966 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/popen.py
--rw-r--r--   0 runner    (1001) docker     (121)     9639 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/reporter.py
--rw-r--r--   0 runner    (1001) docker     (121)     9456 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/resource.py
--rw-r--r--   0 runner    (1001) docker     (121)     9088 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/rose.py
--rw-r--r--   0 runner    (1001) docker     (121)     7357 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/run.py
--rw-r--r--   0 runner    (1001) docker     (121)     2844 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/run_source_vc.py
--rw-r--r--   0 runner    (1001) docker     (121)     4982 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/scheme_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.471482 metomi-rose-2.0rc3/metomi/rose/scripts/
--rw-r--r--   0 runner    (1001) docker     (121)      955 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/scripts/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1343 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/scripts/rosa-db-create
--rwxr-xr-x   0 runner    (1001) docker     (121)     1217 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/scripts/rosa-svn-post-commit
--rwxr-xr-x   0 runner    (1001) docker     (121)     1214 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/scripts/rosa-svn-pre-commit
--rwxr-xr-x   0 runner    (1001) docker     (121)     1430 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/scripts/rosa-ws
--rwxr-xr-x   0 runner    (1001) docker     (121)    10543 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/scripts/rose-mpi-launch
--rwxr-xr-x   0 runner    (1001) docker     (121)     2919 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/scripts/rose-tutorial
--rw-r--r--   0 runner    (1001) docker     (121)     3402 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/section.py
--rw-r--r--   0 runner    (1001) docker     (121)    17868 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/suite_engine_proc.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.471482 metomi-rose-2.0rc3/metomi/rose/suite_engine_procs/
--rw-r--r--   0 runner    (1001) docker     (121)      818 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/suite_engine_procs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    19425 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/suite_engine_procs/cylc.py
--rw-r--r--   0 runner    (1001) docker     (121)     8409 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/task_env.py
--rw-r--r--   0 runner    (1001) docker     (121)     6607 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/task_run.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.471482 metomi-rose-2.0rc3/metomi/rose/tests/
--rw-r--r--   0 runner    (1001) docker     (121)     1262 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.471482 metomi-rose-2.0rc3/metomi/rose/tests/suite_engine_procs/
--rw-r--r--   0 runner    (1001) docker     (121)     4265 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/tests/suite_engine_procs/test_cylc.py
--rw-r--r--   0 runner    (1001) docker     (121)     7580 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (121)     1790 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/tests/test_date.py
--rw-r--r--   0 runner    (1001) docker     (121)     8529 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/tests/test_date_cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     2100 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/tests/test_env.py
--rw-r--r--   0 runner    (1001) docker     (121)     2172 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/tests/test_env_cat.py
--rw-r--r--   0 runner    (1001) docker     (121)     2371 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/tests/test_host_select_client.py
--rw-r--r--   0 runner    (1001) docker     (121)     2357 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/tests/test_loc_handlers_rsync_remote_check.py
--rw-r--r--   0 runner    (1001) docker     (121)     1925 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/tests/test_popen.py
--rw-r--r--   0 runner    (1001) docker     (121)     4855 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/tests/test_resource_locator.py
--rw-r--r--   0 runner    (1001) docker     (121)     1520 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/tests/test_trigger_file.py
--rw-r--r--   0 runner    (1001) docker     (121)     1936 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/tests/test_unicode_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     2124 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/unicode_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    35890 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/upgrade.py
--rw-r--r--   0 runner    (1001) docker     (121)    15668 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rose/variable.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.475482 metomi-rose-2.0rc3/metomi/rosie/
--rw-r--r--   0 runner    (1001) docker     (121)      890 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rosie/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    15908 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rosie/db.py
--rw-r--r--   0 runner    (1001) docker     (121)    10011 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rosie/db_create.py
--rw-r--r--   0 runner    (1001) docker     (121)    10322 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rosie/graph.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.447482 metomi-rose-2.0rc3/metomi/rosie/lib/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.447482 metomi-rose-2.0rc3/metomi/rosie/lib/html/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.475482 metomi-rose-2.0rc3/metomi/rosie/lib/html/static/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.475482 metomi-rose-2.0rc3/metomi/rosie/lib/html/static/css/
--rw-r--r--   0 runner    (1001) docker     (121)   121260 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rosie/lib/html/static/css/bootstrap.min.css
--rw-r--r--   0 runner    (1001) docker     (121)     7678 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rosie/lib/html/static/css/dataTables.bootstrap.css
--rw-r--r--   0 runner    (1001) docker     (121)    17203 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rosie/lib/html/static/css/jquery.dataTables.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.475482 metomi-rose-2.0rc3/metomi/rosie/lib/html/static/fonts/
--rw-r--r--   0 runner    (1001) docker     (121)    20127 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rosie/lib/html/static/fonts/glyphicons-halflings-regular.eot
--rw-r--r--   0 runner    (1001) docker     (121)   108738 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rosie/lib/html/static/fonts/glyphicons-halflings-regular.svg
--rw-r--r--   0 runner    (1001) docker     (121)    45404 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rosie/lib/html/static/fonts/glyphicons-halflings-regular.ttf
--rw-r--r--   0 runner    (1001) docker     (121)    23424 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rosie/lib/html/static/fonts/glyphicons-halflings-regular.woff
--rw-r--r--   0 runner    (1001) docker     (121)    18028 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rosie/lib/html/static/fonts/glyphicons-halflings-regular.woff2
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.475482 metomi-rose-2.0rc3/metomi/rosie/lib/html/static/images/
--rw-r--r--   0 runner    (1001) docker     (121)     1118 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rosie/lib/html/static/images/sort_asc.png
--rw-r--r--   0 runner    (1001) docker     (121)     2916 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rosie/lib/html/static/images/sort_asc_disabled.png
--rw-r--r--   0 runner    (1001) docker     (121)     1136 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rosie/lib/html/static/images/sort_both.png
--rw-r--r--   0 runner    (1001) docker     (121)     1127 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rosie/lib/html/static/images/sort_desc.png
--rw-r--r--   0 runner    (1001) docker     (121)     1045 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rosie/lib/html/static/images/sort_desc_disabled.png
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.475482 metomi-rose-2.0rc3/metomi/rosie/lib/html/static/js/
--rw-r--r--   0 runner    (1001) docker     (121)    36868 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rosie/lib/html/static/js/bootstrap.min.js
--rw-r--r--   0 runner    (1001) docker     (121)     4287 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rosie/lib/html/static/js/dataTables.bootstrap.js
--rw-r--r--   0 runner    (1001) docker     (121)   434957 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rosie/lib/html/static/js/jquery.dataTables.js
--rw-r--r--   0 runner    (1001) docker     (121)    78746 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rosie/lib/html/static/js/jquery.dataTables.min.js
--rw-r--r--   0 runner    (1001) docker     (121)    95786 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rosie/lib/html/static/js/jquery.min.js
--rw-r--r--   0 runner    (1001) docker     (121)     1414 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rosie/lib/html/static/js/livestamp.min.js
--rw-r--r--   0 runner    (1001) docker     (121)    18053 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rosie/lib/html/static/js/moment.min.js
--rw-r--r--   0 runner    (1001) docker     (121)     5281 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rosie/lib/html/static/js/rosie-disco.js
--rw-r--r--   0 runner    (1001) docker     (121)     1039 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rosie/lib/html/static/rosie-favicon.png
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.447482 metomi-rose-2.0rc3/metomi/rosie/lib/html/template/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.475482 metomi-rose-2.0rc3/metomi/rosie/lib/html/template/rosie-disco/
--rw-r--r--   0 runner    (1001) docker     (121)      955 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rosie/lib/html/template/rosie-disco/index.html
--rw-r--r--   0 runner    (1001) docker     (121)     9235 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rosie/lib/html/template/rosie-disco/prefix-index.html
--rw-r--r--   0 runner    (1001) docker     (121)    22335 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rosie/suite_id.py
--rw-r--r--   0 runner    (1001) docker     (121)     5892 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rosie/svn_hook.py
--rw-r--r--   0 runner    (1001) docker     (121)    20364 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rosie/svn_post_commit.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    13444 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rosie/svn_pre_commit.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.475482 metomi-rose-2.0rc3/metomi/rosie/tests/
--rw-r--r--   0 runner    (1001) docker     (121)     1541 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rosie/tests/test_suite_id.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.475482 metomi-rose-2.0rc3/metomi/rosie/usertools/
--rw-r--r--   0 runner    (1001) docker     (121)      860 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rosie/usertools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3243 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rosie/usertools/ldaptool.py
--rw-r--r--   0 runner    (1001) docker     (121)     1965 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rosie/usertools/passwdtool.py
--rw-r--r--   0 runner    (1001) docker     (121)    29449 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rosie/vc.py
--rw-r--r--   0 runner    (1001) docker     (121)    21705 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rosie/ws.py
--rw-r--r--   0 runner    (1001) docker     (121)    16254 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rosie/ws_client.py
--rw-r--r--   0 runner    (1001) docker     (121)    19597 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rosie/ws_client_auth.py
--rw-r--r--   0 runner    (1001) docker     (121)    11407 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/metomi/rosie/ws_client_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 12:44:04.479482 metomi-rose-2.0rc3/metomi_rose.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3190 2022-05-20 12:44:04.000000 metomi-rose-2.0rc3/metomi_rose.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    14500 2022-05-20 12:44:04.000000 metomi-rose-2.0rc3/metomi_rose.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-20 12:44:04.000000 metomi-rose-2.0rc3/metomi_rose.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1278 2022-05-20 12:44:04.000000 metomi-rose-2.0rc3/metomi_rose.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      599 2022-05-20 12:44:04.000000 metomi-rose-2.0rc3/metomi_rose.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-05-20 12:44:04.000000 metomi-rose-2.0rc3/metomi_rose.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2852 2022-05-20 12:44:04.479482 metomi-rose-2.0rc3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      803 2022-05-20 12:44:00.000000 metomi-rose-2.0rc3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:04:05.623907 metomi-rose-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-07-21 11:04:05.623907 metomi-rose-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:04:05.591905 metomi-rose-2.1.0/metomi/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:04:05.595905 metomi-rose-2.1.0/metomi/rose/
+-rw-r--r--   0 runner    (1001) docker     (123)     4030 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19321 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/app_run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:04:05.595905 metomi-rose-2.1.0/metomi/rose/apps/
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/apps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:04:05.595905 metomi-rose-2.1.0/metomi/rose/apps/ana_builtin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/apps/ana_builtin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21577 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/apps/ana_builtin/grepper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:04:05.599905 metomi-rose-2.1.0/metomi/rose/apps/comparisons/
+-rw-r--r--   0 runner    (1001) docker     (123)     7501 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/apps/comparisons/cumf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/apps/comparisons/exact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/apps/comparisons/mandatory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/apps/comparisons/output_grepper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/apps/comparisons/prohibited.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4929 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/apps/comparisons/within.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11819 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/apps/fcm_make.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33581 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/apps/rose_ana.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21791 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/apps/rose_ana_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23070 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/apps/rose_arch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:04:05.599905 metomi-rose-2.1.0/metomi/rose/apps/rose_arch_compressions/
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/apps/rose_arch_compressions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/apps/rose_arch_compressions/rose_arch_gzip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/apps/rose_arch_compressions/rose_arch_tar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21012 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/apps/rose_bunch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12346 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/apps/rose_prune.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7988 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/c3.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12093 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/check_software.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5772 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/checksum.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64089 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7736 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/config_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11281 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/config_diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/config_dump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4984 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/config_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:04:05.599905 metomi-rose-2.1.0/metomi/rose/config_processors/
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/config_processors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/config_processors/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33907 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/config_processors/fileinstall.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15431 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/config_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17852 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/date.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10268 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/date_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5855 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/env_cat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:04:05.587905 metomi-rose-2.1.0/metomi/rose/etc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:04:05.583904 metomi-rose-2.1.0/metomi/rose/etc/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:04:05.599905 metomi-rose-2.1.0/metomi/rose/etc/lib/bash/
+-rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/etc/lib/bash/rose_log
+-rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/etc/lib/bash/rose_usage
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:04:05.587905 metomi-rose-2.1.0/metomi/rose/etc/rose-meta/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:04:05.583904 metomi-rose-2.1.0/metomi/rose/etc/rose-meta/fcm_make/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:04:05.599905 metomi-rose-2.1.0/metomi/rose/etc/rose-meta/fcm_make/HEAD/
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/etc/rose-meta/fcm_make/HEAD/rose-meta.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:04:05.599905 metomi-rose-2.1.0/metomi/rose/etc/rose-meta/rose-all/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:04:05.583904 metomi-rose-2.1.0/metomi/rose/etc/rose-meta/rose-all/etc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:04:05.599905 metomi-rose-2.1.0/metomi/rose/etc/rose-meta/rose-all/etc/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/etc/rose-meta/rose-all/etc/images/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/etc/rose-meta/rose-all/rose-meta.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:04:05.599905 metomi-rose-2.1.0/metomi/rose/etc/rose-meta/rose-app-conf/
+-rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/etc/rose-meta/rose-app-conf/rose-meta.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:04:05.587905 metomi-rose-2.1.0/metomi/rose/etc/rose-meta/rose-demo-baked-alaska/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:04:05.599905 metomi-rose-2.1.0/metomi/rose/etc/rose-meta/rose-demo-baked-alaska/HEAD/
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/etc/rose-meta/rose-demo-baked-alaska/HEAD/rose-meta.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:04:05.599905 metomi-rose-2.1.0/metomi/rose/etc/rose-meta/rose-demo-baked-alaska/vn1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/etc/rose-meta/rose-demo-baked-alaska/vn1.0/rose-meta.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:04:05.599905 metomi-rose-2.1.0/metomi/rose/etc/rose-meta/rose-demo-baked-alaska/vn2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/etc/rose-meta/rose-demo-baked-alaska/vn2.0/rose-meta.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:04:05.583904 metomi-rose-2.1.0/metomi/rose/etc/rose-meta/rose-demo-baked-alaska-icecream/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:04:05.599905 metomi-rose-2.1.0/metomi/rose/etc/rose-meta/rose-demo-baked-alaska-icecream/HEAD/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/etc/rose-meta/rose-demo-baked-alaska-icecream/HEAD/rose-meta.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:04:05.599905 metomi-rose-2.1.0/metomi/rose/etc/rose-meta/rose-demo-baked-alaska-icecream/vn1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/etc/rose-meta/rose-demo-baked-alaska-icecream/vn1.0/rose-meta.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:04:05.599905 metomi-rose-2.1.0/metomi/rose/etc/rose-meta/rose-demo-baked-alaska-icecream/vn2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/etc/rose-meta/rose-demo-baked-alaska-icecream/vn2.0/rose-meta.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:04:05.587905 metomi-rose-2.1.0/metomi/rose/etc/rose-meta/rose-demo-baked-alaska-sponge/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:04:05.599905 metomi-rose-2.1.0/metomi/rose/etc/rose-meta/rose-demo-baked-alaska-sponge/HEAD/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/etc/rose-meta/rose-demo-baked-alaska-sponge/HEAD/rose-meta.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:04:05.599905 metomi-rose-2.1.0/metomi/rose/etc/rose-meta/rose-demo-baked-alaska-sponge/vn1.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:04:05.587905 metomi-rose-2.1.0/metomi/rose/etc/rose-meta/rose-demo-baked-alaska-sponge/vn1.0/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:04:05.587905 metomi-rose-2.1.0/metomi/rose/etc/rose-meta/rose-demo-baked-alaska-sponge/vn1.0/lib/python/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:04:05.599905 metomi-rose-2.1.0/metomi/rose/etc/rose-meta/rose-demo-baked-alaska-sponge/vn1.0/lib/python/macros/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/etc/rose-meta/rose-demo-baked-alaska-sponge/vn1.0/lib/python/macros/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/etc/rose-meta/rose-demo-baked-alaska-sponge/vn1.0/lib/python/macros/desoggy.py
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/etc/rose-meta/rose-demo-baked-alaska-sponge/vn1.0/rose-meta.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:04:05.599905 metomi-rose-2.1.0/metomi/rose/etc/rose-meta/rose-demo-baked-alaska-sponge/vn2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/etc/rose-meta/rose-demo-baked-alaska-sponge/vn2.0/rose-meta.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:04:05.599905 metomi-rose-2.1.0/metomi/rose/etc/rose-meta/rose-demo-upgrade/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:04:05.599905 metomi-rose-2.1.0/metomi/rose/etc/rose-meta/rose-demo-upgrade/HEAD/
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/etc/rose-meta/rose-demo-upgrade/HEAD/rose-meta.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:04:05.587905 metomi-rose-2.1.0/metomi/rose/etc/rose-meta/rose-demo-upgrade/etc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:04:05.599905 metomi-rose-2.1.0/metomi/rose/etc/rose-meta/rose-demo-upgrade/etc/garden0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/etc/rose-meta/rose-demo-upgrade/etc/garden0.4/rose-macro-add.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:04:05.599905 metomi-rose-2.1.0/metomi/rose/etc/rose-meta/rose-demo-upgrade/garden0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/etc/rose-meta/rose-demo-upgrade/garden0.1/rose-meta.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:04:05.599905 metomi-rose-2.1.0/metomi/rose/etc/rose-meta/rose-demo-upgrade/garden0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/etc/rose-meta/rose-demo-upgrade/garden0.2/rose-meta.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:04:05.599905 metomi-rose-2.1.0/metomi/rose/etc/rose-meta/rose-demo-upgrade/garden0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/etc/rose-meta/rose-demo-upgrade/garden0.3/rose-meta.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:04:05.599905 metomi-rose-2.1.0/metomi/rose/etc/rose-meta/rose-demo-upgrade/garden0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/etc/rose-meta/rose-demo-upgrade/garden0.4/rose-meta.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:04:05.599905 metomi-rose-2.1.0/metomi/rose/etc/rose-meta/rose-demo-upgrade/garden0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/etc/rose-meta/rose-demo-upgrade/garden0.9/rose-meta.conf
+-rw-r--r--   0 runner    (1001) docker     (123)     3887 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/etc/rose-meta/rose-demo-upgrade/versions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:04:05.599905 metomi-rose-2.1.0/metomi/rose/etc/rose-meta/rose-demo-upgrade-null/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:04:05.599905 metomi-rose-2.1.0/metomi/rose/etc/rose-meta/rose-demo-upgrade-null/0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/etc/rose-meta/rose-demo-upgrade-null/0.1/rose-meta.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:04:05.599905 metomi-rose-2.1.0/metomi/rose/etc/rose-meta/rose-demo-upgrade-null/0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/etc/rose-meta/rose-demo-upgrade-null/0.2/rose-meta.conf
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/etc/rose-meta/rose-demo-upgrade-null/versions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:04:05.599905 metomi-rose-2.1.0/metomi/rose/etc/rose-meta/rose-suite-conf/
+-rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/etc/rose-meta/rose-suite-conf/rose-meta.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:04:05.603906 metomi-rose-2.1.0/metomi/rose/etc/rose-meta/rose-suite-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/etc/rose-meta/rose-suite-info/rose-meta.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:04:05.587905 metomi-rose-2.1.0/metomi/rose/etc/rose-meta/rose_bunch/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:04:05.603906 metomi-rose-2.1.0/metomi/rose/etc/rose-meta/rose_bunch/HEAD/
+-rw-r--r--   0 runner    (1001) docker     (123)     2760 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/etc/rose-meta/rose_bunch/HEAD/rose-meta.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:04:05.587905 metomi-rose-2.1.0/metomi/rose/etc/rose-meta/rose_prune/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:04:05.603906 metomi-rose-2.1.0/metomi/rose/etc/rose-meta/rose_prune/HEAD/
+-rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/etc/rose-meta/rose_prune/HEAD/rose-meta.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:04:05.603906 metomi-rose-2.1.0/metomi/rose/etc/syntax/
+-rw-r--r--   0 runner    (1001) docker     (123)     4866 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/etc/syntax/rose-conf-mode.el
+-rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/etc/syntax/rose-conf.lang
+-rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/etc/syntax/rose-conf.vim
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/etc/syntax/rose-conf.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:04:05.603906 metomi-rose-2.1.0/metomi/rose/etc/tutorial/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/etc/tutorial/api-keys
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:04:05.603906 metomi-rose-2.1.0/metomi/rose/etc/tutorial/cylc-forecasting-workflow/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1139 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/etc/tutorial/cylc-forecasting-workflow/.validate
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:04:05.603906 metomi-rose-2.1.0/metomi/rose/etc/tutorial/cylc-forecasting-workflow/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4248 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/etc/tutorial/cylc-forecasting-workflow/bin/consolidate-observations
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9151 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/etc/tutorial/cylc-forecasting-workflow/bin/forecast
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7216 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/etc/tutorial/cylc-forecasting-workflow/bin/get-observations
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6453 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/etc/tutorial/cylc-forecasting-workflow/bin/get-rainfall
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3721 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/etc/tutorial/cylc-forecasting-workflow/bin/post-process
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:04:05.603906 metomi-rose-2.1.0/metomi/rose/etc/tutorial/cylc-forecasting-workflow/etc/
+-rw-r--r--   0 runner    (1001) docker     (123)     7485 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/etc/tutorial/cylc-forecasting-workflow/etc/met-office-sites.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/etc/tutorial/cylc-forecasting-workflow/etc/python-job.settings
+-rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/etc/tutorial/cylc-forecasting-workflow/flow.cylc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:04:05.587905 metomi-rose-2.1.0/metomi/rose/etc/tutorial/cylc-forecasting-workflow/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:04:05.603906 metomi-rose-2.1.0/metomi/rose/etc/tutorial/cylc-forecasting-workflow/lib/python/
+-rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/etc/tutorial/cylc-forecasting-workflow/lib/python/mercator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10018 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/etc/tutorial/cylc-forecasting-workflow/lib/python/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:04:05.603906 metomi-rose-2.1.0/metomi/rose/etc/tutorial/cylc-forecasting-workflow/lib/template/
+-rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/etc/tutorial/cylc-forecasting-workflow/lib/template/map.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:04:05.603906 metomi-rose-2.1.0/metomi/rose/etc/tutorial/failif-warnif/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/etc/tutorial/failif-warnif/.validate
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:04:05.603906 metomi-rose-2.1.0/metomi/rose/etc/tutorial/failif-warnif/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/etc/tutorial/failif-warnif/meta/rose-meta.conf
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/etc/tutorial/failif-warnif/rose-app.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:04:05.603906 metomi-rose-2.1.0/metomi/rose/etc/tutorial/forecast-script/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9151 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/etc/tutorial/forecast-script/forecast
+-rw-r--r--   0 runner    (1001) docker     (123)    10018 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/etc/tutorial/forecast-script/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:04:05.603906 metomi-rose-2.1.0/metomi/rose/etc/tutorial/map-template/
+-rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/etc/tutorial/map-template/map-template.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:04:05.603906 metomi-rose-2.1.0/metomi/rose/etc/tutorial/metadata-tutorial/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/etc/tutorial/metadata-tutorial/.validate
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:04:05.603906 metomi-rose-2.1.0/metomi/rose/etc/tutorial/metadata-tutorial/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9151 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/etc/tutorial/metadata-tutorial/bin/forecast
+-rw-r--r--   0 runner    (1001) docker     (123)    10018 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/etc/tutorial/metadata-tutorial/bin/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:04:05.603906 metomi-rose-2.1.0/metomi/rose/etc/tutorial/metadata-tutorial/file/
+-rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/etc/tutorial/metadata-tutorial/file/map-template.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:04:05.603906 metomi-rose-2.1.0/metomi/rose/etc/tutorial/metadata-tutorial/file/test-data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/etc/tutorial/metadata-tutorial/file/test-data/.validate
+-rw-r--r--   0 runner    (1001) docker     (123)    33085 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/etc/tutorial/metadata-tutorial/file/test-data/rainfall.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    35829 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/etc/tutorial/metadata-tutorial/file/test-data/wind_20171101T0000Z_x.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    38004 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/etc/tutorial/metadata-tutorial/file/test-data/wind_20171101T0000Z_y.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/etc/tutorial/metadata-tutorial/rose-app.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:04:05.603906 metomi-rose-2.1.0/metomi/rose/etc/tutorial/rose-stem/
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/etc/tutorial/rose-stem/.validate
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/etc/tutorial/rose-stem/kgo.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:04:05.607906 metomi-rose-2.1.0/metomi/rose/etc/tutorial/rose-stem/rose-stem/
+-rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/etc/tutorial/rose-stem/rose-stem/flow.cylc
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/etc/tutorial/rose-stem/rose-stem/rose-suite.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:04:05.607906 metomi-rose-2.1.0/metomi/rose/etc/tutorial/rose-stem/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/etc/tutorial/rose-stem/src/spaceship_command.f90
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:04:05.607906 metomi-rose-2.1.0/metomi/rose/etc/tutorial/rose-suite-tutorial/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/etc/tutorial/rose-suite-tutorial/.validate
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:04:05.587905 metomi-rose-2.1.0/metomi/rose/etc/tutorial/rose-suite-tutorial/app/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:04:05.607906 metomi-rose-2.1.0/metomi/rose/etc/tutorial/rose-suite-tutorial/app/forecast/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:04:05.607906 metomi-rose-2.1.0/metomi/rose/etc/tutorial/rose-suite-tutorial/app/forecast/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9151 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/etc/tutorial/rose-suite-tutorial/app/forecast/bin/forecast
+-rw-r--r--   0 runner    (1001) docker     (123)    10018 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/etc/tutorial/rose-suite-tutorial/app/forecast/bin/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:04:05.607906 metomi-rose-2.1.0/metomi/rose/etc/tutorial/rose-suite-tutorial/app/forecast/file/
+-rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/etc/tutorial/rose-suite-tutorial/app/forecast/file/map-template.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:04:05.607906 metomi-rose-2.1.0/metomi/rose/etc/tutorial/rose-suite-tutorial/app/forecast/file/test-data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/etc/tutorial/rose-suite-tutorial/app/forecast/file/test-data/.validate
+-rw-r--r--   0 runner    (1001) docker     (123)    33085 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/etc/tutorial/rose-suite-tutorial/app/forecast/file/test-data/rainfall.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    35829 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/etc/tutorial/rose-suite-tutorial/app/forecast/file/test-data/wind_20171101T0000Z_x.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    38004 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/etc/tutorial/rose-suite-tutorial/app/forecast/file/test-data/wind_20171101T0000Z_y.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:04:05.607906 metomi-rose-2.1.0/metomi/rose/etc/tutorial/rose-suite-tutorial/app/forecast/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/etc/tutorial/rose-suite-tutorial/app/forecast/meta/rose-meta.conf
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/etc/tutorial/rose-suite-tutorial/app/forecast/rose-app.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:04:05.607906 metomi-rose-2.1.0/metomi/rose/etc/tutorial/rose-suite-tutorial/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4248 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/etc/tutorial/rose-suite-tutorial/bin/consolidate-observations
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7216 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/etc/tutorial/rose-suite-tutorial/bin/get-observations
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6453 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/etc/tutorial/rose-suite-tutorial/bin/get-rainfall
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3721 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/etc/tutorial/rose-suite-tutorial/bin/post-process
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:04:05.607906 metomi-rose-2.1.0/metomi/rose/etc/tutorial/rose-suite-tutorial/etc/
+-rw-r--r--   0 runner    (1001) docker     (123)     7485 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/etc/tutorial/rose-suite-tutorial/etc/met-office-sites.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/etc/tutorial/rose-suite-tutorial/etc/python-job.settings
+-rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/etc/tutorial/rose-suite-tutorial/flow.cylc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:04:05.587905 metomi-rose-2.1.0/metomi/rose/etc/tutorial/rose-suite-tutorial/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:04:05.607906 metomi-rose-2.1.0/metomi/rose/etc/tutorial/rose-suite-tutorial/lib/python/
+-rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/etc/tutorial/rose-suite-tutorial/lib/python/mercator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10018 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/etc/tutorial/rose-suite-tutorial/lib/python/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:04:05.607906 metomi-rose-2.1.0/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/.validate
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:04:05.587905 metomi-rose-2.1.0/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/app/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:04:05.607906 metomi-rose-2.1.0/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/app/forecast/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:04:05.607906 metomi-rose-2.1.0/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/app/forecast/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9151 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/app/forecast/bin/forecast
+-rw-r--r--   0 runner    (1001) docker     (123)    10018 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/app/forecast/bin/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:04:05.607906 metomi-rose-2.1.0/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/app/forecast/file/
+-rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/app/forecast/file/map-template.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:04:05.607906 metomi-rose-2.1.0/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/app/forecast/file/test-data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/app/forecast/file/test-data/.validate
+-rw-r--r--   0 runner    (1001) docker     (123)    33085 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/app/forecast/file/test-data/rainfall.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    35829 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/app/forecast/file/test-data/wind_20171101T0000Z_x.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    38004 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/app/forecast/file/test-data/wind_20171101T0000Z_y.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:04:05.611906 metomi-rose-2.1.0/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/app/forecast/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/app/forecast/meta/rose-meta.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:04:05.611906 metomi-rose-2.1.0/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/app/forecast/opt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/app/forecast/opt/rose-app-test.conf
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/app/forecast/rose-app.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:04:05.611906 metomi-rose-2.1.0/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4248 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/bin/consolidate-observations
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9151 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/bin/forecast
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7216 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/bin/get-observations
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6453 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/bin/get-rainfall
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3721 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/bin/post-process
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:04:05.611906 metomi-rose-2.1.0/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/etc/
+-rw-r--r--   0 runner    (1001) docker     (123)     7485 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/etc/met-office-sites.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/etc/python-job.settings
+-rw-r--r--   0 runner    (1001) docker     (123)     2940 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/flow.cylc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:04:05.591905 metomi-rose-2.1.0/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:04:05.611906 metomi-rose-2.1.0/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/lib/python/
+-rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/lib/python/mercator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10018 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/lib/python/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:04:05.611906 metomi-rose-2.1.0/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/meta/rose-meta.conf
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/rose-suite.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:04:05.611906 metomi-rose-2.1.0/metomi/rose/etc/tutorial/test-data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/etc/tutorial/test-data/.validate
+-rw-r--r--   0 runner    (1001) docker     (123)    33085 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/etc/tutorial/test-data/rainfall.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    35829 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/etc/tutorial/test-data/wind_20171101T0000Z_x.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    38004 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/etc/tutorial/test-data/wind_20171101T0000Z_y.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:04:05.611906 metomi-rose-2.1.0/metomi/rose/etc/tutorial/widget/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/etc/tutorial/widget/.validate
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:04:05.591905 metomi-rose-2.1.0/metomi/rose/etc/tutorial/widget/meta/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:04:05.591905 metomi-rose-2.1.0/metomi/rose/etc/tutorial/widget/meta/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:04:05.591905 metomi-rose-2.1.0/metomi/rose/etc/tutorial/widget/meta/lib/python/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:04:05.611906 metomi-rose-2.1.0/metomi/rose/etc/tutorial/widget/meta/lib/python/widget/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/etc/tutorial/widget/meta/lib/python/widget/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/etc/tutorial/widget/meta/lib/python/widget/username.py
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/etc/tutorial/widget/rose-app.conf
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/external.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:04:05.611906 metomi-rose-2.1.0/metomi/rose/formats/
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/formats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14235 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/formats/namelist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5893 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/fs_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24700 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/host_select.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/host_select_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9301 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/job_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:04:05.611906 metomi-rose-2.1.0/metomi/rose/loc_handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/loc_handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/loc_handlers/fs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/loc_handlers/namelist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3872 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/loc_handlers/rsync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/loc_handlers/rsync_remote_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4116 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/loc_handlers/svn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68500 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/macro.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:04:05.611906 metomi-rose-2.1.0/metomi/rose/macros/
+-rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/macros/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12374 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/macros/compulsory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/macros/duplicate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/macros/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20514 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/macros/rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26691 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/macros/trigger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14522 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/macros/value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7060 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/meta_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16583 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/metadata_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7432 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/metadata_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13680 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/metadata_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5436 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/namelist_dump.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43854 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/opt_parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13966 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/popen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9639 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/reporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9456 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9271 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/rose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7357 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/run_source_vc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5437 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/scheme_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:04:05.615906 metomi-rose-2.1.0/metomi/rose/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/scripts/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1343 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/scripts/rosa-db-create
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1217 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/scripts/rosa-svn-post-commit
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1214 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/scripts/rosa-svn-pre-commit
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1430 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/scripts/rosa-ws
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10543 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/scripts/rose-mpi-launch
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2919 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/scripts/rose-tutorial
+-rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/section.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17868 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/suite_engine_proc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:04:05.615906 metomi-rose-2.1.0/metomi/rose/suite_engine_procs/
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/suite_engine_procs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19435 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/suite_engine_procs/cylc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8409 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/task_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6607 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/task_run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:04:05.615906 metomi-rose-2.1.0/metomi/rose/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:04:05.615906 metomi-rose-2.1.0/metomi/rose/tests/macros/
+-rw-r--r--   0 runner    (1001) docker     (123)     7561 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/tests/macros/test_py2_compat_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:04:05.615906 metomi-rose-2.1.0/metomi/rose/tests/suite_engine_procs/
+-rw-r--r--   0 runner    (1001) docker     (123)     4265 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/tests/suite_engine_procs/test_cylc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7580 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/tests/test_date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9381 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/tests/test_date_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/tests/test_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/tests/test_env_cat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/tests/test_host_select_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/tests/test_loc_handlers_rsync_remote_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/tests/test_popen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4855 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/tests/test_resource_locator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/tests/test_trigger_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/tests/test_unicode_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/unicode_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35890 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/upgrade.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15668 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rose/variable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:04:05.615906 metomi-rose-2.1.0/metomi/rosie/
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rosie/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15908 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rosie/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10011 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rosie/db_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10322 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rosie/graph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:04:05.591905 metomi-rose-2.1.0/metomi/rosie/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:04:05.591905 metomi-rose-2.1.0/metomi/rosie/lib/html/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:04:05.619907 metomi-rose-2.1.0/metomi/rosie/lib/html/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:04:05.619907 metomi-rose-2.1.0/metomi/rosie/lib/html/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)   121260 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rosie/lib/html/static/css/bootstrap.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)     7678 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rosie/lib/html/static/css/dataTables.bootstrap.css
+-rw-r--r--   0 runner    (1001) docker     (123)    17203 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rosie/lib/html/static/css/jquery.dataTables.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:04:05.619907 metomi-rose-2.1.0/metomi/rosie/lib/html/static/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)    20127 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rosie/lib/html/static/fonts/glyphicons-halflings-regular.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   108738 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rosie/lib/html/static/fonts/glyphicons-halflings-regular.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    45404 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rosie/lib/html/static/fonts/glyphicons-halflings-regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    23424 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rosie/lib/html/static/fonts/glyphicons-halflings-regular.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    18028 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rosie/lib/html/static/fonts/glyphicons-halflings-regular.woff2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:04:05.619907 metomi-rose-2.1.0/metomi/rosie/lib/html/static/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rosie/lib/html/static/images/sort_asc.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rosie/lib/html/static/images/sort_asc_disabled.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rosie/lib/html/static/images/sort_both.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rosie/lib/html/static/images/sort_desc.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rosie/lib/html/static/images/sort_desc_disabled.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:04:05.619907 metomi-rose-2.1.0/metomi/rosie/lib/html/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    36868 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rosie/lib/html/static/js/bootstrap.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rosie/lib/html/static/js/dataTables.bootstrap.js
+-rw-r--r--   0 runner    (1001) docker     (123)   434957 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rosie/lib/html/static/js/jquery.dataTables.js
+-rw-r--r--   0 runner    (1001) docker     (123)    78746 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rosie/lib/html/static/js/jquery.dataTables.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    95786 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rosie/lib/html/static/js/jquery.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rosie/lib/html/static/js/livestamp.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    18053 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rosie/lib/html/static/js/moment.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5281 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rosie/lib/html/static/js/rosie-disco.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rosie/lib/html/static/rosie-favicon.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:04:05.591905 metomi-rose-2.1.0/metomi/rosie/lib/html/template/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:04:05.619907 metomi-rose-2.1.0/metomi/rosie/lib/html/template/rosie-disco/
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rosie/lib/html/template/rosie-disco/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     9235 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rosie/lib/html/template/rosie-disco/prefix-index.html
+-rw-r--r--   0 runner    (1001) docker     (123)    22335 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rosie/suite_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5892 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rosie/svn_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20364 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rosie/svn_post_commit.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13444 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rosie/svn_pre_commit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:04:05.619907 metomi-rose-2.1.0/metomi/rosie/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rosie/tests/test_suite_id.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:04:05.623907 metomi-rose-2.1.0/metomi/rosie/usertools/
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rosie/usertools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rosie/usertools/ldaptool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rosie/usertools/passwdtool.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29449 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rosie/vc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21705 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rosie/ws.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16254 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rosie/ws_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16380 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rosie/ws_client_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11407 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/metomi/rosie/ws_client_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:04:05.623907 metomi-rose-2.1.0/metomi_rose.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-07-21 11:04:05.000000 metomi-rose-2.1.0/metomi_rose.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13343 2023-07-21 11:04:05.000000 metomi-rose-2.1.0/metomi_rose.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 11:04:05.000000 metomi-rose-2.1.0/metomi_rose.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-07-21 11:04:05.000000 metomi-rose-2.1.0/metomi_rose.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-21 11:04:05.000000 metomi-rose-2.1.0/metomi_rose.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-21 11:04:05.000000 metomi-rose-2.1.0/metomi_rose.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-07-21 11:04:05.623907 metomi-rose-2.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-07-21 11:04:01.000000 metomi-rose-2.1.0/setup.py
```

### Comparing `metomi-rose-2.0rc3/COPYING` & `metomi-rose-2.1.0/COPYING`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/PKG-INFO` & `metomi-rose-2.1.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metomi-rose
-Version: 2.0rc3
+Version: 2.1.0
 Summary: Rose, a framework for meteorological suites.
 Home-page: https://metomi.github.io/rose/doc/html/index.html
 Author: British Crown (Met Office) & Contributors
 Author-email: metomi@metoffice.gov.uk
 License: GPL
 Keywords: hpc,weather-modelling,weather-model,meteorological-suites,meteorological-modelling,meteorological-models
 Platform: any
@@ -23,45 +23,41 @@
 Provides-Extra: rosa
 Provides-Extra: tests
 Provides-Extra: all
 License-File: COPYING
 
 # Rose
 
-[![Build Status](https://travis-ci.org/metomi/rose.svg?branch=master)](https://travis-ci.org/metomi/rose)
-[![Codacy Badge](https://api.codacy.com/project/badge/Grade/ad021a33e7a64b398f792305dd901795)](https://www.codacy.com/app/metomi/rose?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=metomi/rose&amp;utm_campaign=Badge_Grade)
+[![test](https://github.com/metomi/rose/actions/workflows/test.yml/badge.svg)](https://github.com/metomi/rose/actions/workflows/test.yml)
 [![DOI](https://zenodo.org/badge/6223866.svg)](https://zenodo.org/badge/latestdoi/6223866)
-[![codecov](https://codecov.io/gh/metomi/rose/branch/master/graph/badge.svg)](https://codecov.io/gh/metomi/rose)
 
 Rose: a framework for managing and running meteorological suites.
 
 ### Python 2 or Python 3 ?
 
 #### Rose 2019
 
-- Production ready
 - Python 2
 - PyGTK GUI
 - `2019.01.x` branch in the source code
 
 #### Rose 2
 
-- Release candidate
 - Python 3
 - No GUIs
 - Web-based GUIs will follow in later Rose 2 releases
 - `master` branch in the source code
 
 [Installation](http://metomi.github.io/rose/doc/html/installation.html) |
 [User Guide](http://metomi.github.io/rose/) |
 [How to Contribute](https://github.com/metomi/rose/blob/master/CONTRIBUTING.md)
 
 ## Copyright and Terms of Use
 
-Copyright (C) 2012-<span actions:bind='current-year'>2022</span> British Crown (Met Office) &amp; Contributors
+Copyright (C) 2012-<span actions:bind='current-year'>2023</span> British Crown (Met Office) &amp; Contributors
 
 Rose is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 Rose is distributed in the hope that it will be useful,
```

### Comparing `metomi-rose-2.0rc3/README.md` & `metomi-rose-2.1.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,40 +1,36 @@
 # Rose
 
-[![Build Status](https://travis-ci.org/metomi/rose.svg?branch=master)](https://travis-ci.org/metomi/rose)
-[![Codacy Badge](https://api.codacy.com/project/badge/Grade/ad021a33e7a64b398f792305dd901795)](https://www.codacy.com/app/metomi/rose?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=metomi/rose&amp;utm_campaign=Badge_Grade)
+[![test](https://github.com/metomi/rose/actions/workflows/test.yml/badge.svg)](https://github.com/metomi/rose/actions/workflows/test.yml)
 [![DOI](https://zenodo.org/badge/6223866.svg)](https://zenodo.org/badge/latestdoi/6223866)
-[![codecov](https://codecov.io/gh/metomi/rose/branch/master/graph/badge.svg)](https://codecov.io/gh/metomi/rose)
 
 Rose: a framework for managing and running meteorological suites.
 
 ### Python 2 or Python 3 ?
 
 #### Rose 2019
 
-- Production ready
 - Python 2
 - PyGTK GUI
 - `2019.01.x` branch in the source code
 
 #### Rose 2
 
-- Release candidate
 - Python 3
 - No GUIs
 - Web-based GUIs will follow in later Rose 2 releases
 - `master` branch in the source code
 
 [Installation](http://metomi.github.io/rose/doc/html/installation.html) |
 [User Guide](http://metomi.github.io/rose/) |
 [How to Contribute](https://github.com/metomi/rose/blob/master/CONTRIBUTING.md)
 
 ## Copyright and Terms of Use
 
-Copyright (C) 2012-<span actions:bind='current-year'>2022</span> British Crown (Met Office) &amp; Contributors
+Copyright (C) 2012-<span actions:bind='current-year'>2023</span> British Crown (Met Office) &amp; Contributors
 
 Rose is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 Rose is distributed in the hope that it will be useful,
```

### Comparing `metomi-rose-2.0rc3/metomi/rose/__init__.py` & `metomi-rose-2.1.0/metomi/rose/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -140,8 +140,8 @@
 FILE_VAR_CHECKSUM = "checksum"
 FILE_VAR_MODE = "mode"
 FILE_VAR_SOURCE = "source"
 
 # Paths in the Rose distribution.
 FILEPATH_README = "README.md"
 
-__version__ = "2.0rc3"
+__version__ = "2.1.0"
```

### Comparing `metomi-rose-2.0rc3/metomi/rose/app_run.py` & `metomi-rose-2.1.0/metomi/rose/app_run.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rose/apps/__init__.py` & `metomi-rose-2.1.0/metomi/rose/apps/__init__.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rose/apps/ana_builtin/grepper.py` & `metomi-rose-2.1.0/metomi/rose/apps/ana_builtin/grepper.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rose/apps/comparisons/cumf.py` & `metomi-rose-2.1.0/metomi/rose/apps/comparisons/cumf.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rose/apps/comparisons/exact.py` & `metomi-rose-2.1.0/metomi/rose/apps/comparisons/exact.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rose/apps/comparisons/mandatory.py` & `metomi-rose-2.1.0/metomi/rose/apps/comparisons/mandatory.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rose/apps/comparisons/output_grepper.py` & `metomi-rose-2.1.0/metomi/rose/apps/comparisons/output_grepper.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rose/apps/comparisons/prohibited.py` & `metomi-rose-2.1.0/metomi/rose/apps/comparisons/prohibited.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rose/apps/comparisons/within.py` & `metomi-rose-2.1.0/metomi/rose/apps/comparisons/within.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rose/apps/fcm_make.py` & `metomi-rose-2.1.0/metomi/rose/apps/fcm_make.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rose/apps/rose_ana.py` & `metomi-rose-2.1.0/metomi/rose/apps/rose_ana.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rose/apps/rose_ana_v1.py` & `metomi-rose-2.1.0/metomi/rose/apps/rose_ana_v1.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rose/apps/rose_arch.py` & `metomi-rose-2.1.0/metomi/rose/apps/rose_arch.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rose/apps/rose_arch_compressions/__init__.py` & `metomi-rose-2.1.0/metomi/rose/apps/rose_arch_compressions/__init__.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rose/apps/rose_arch_compressions/rose_arch_gzip.py` & `metomi-rose-2.1.0/metomi/rose/apps/rose_arch_compressions/rose_arch_gzip.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rose/apps/rose_arch_compressions/rose_arch_tar.py` & `metomi-rose-2.1.0/metomi/rose/apps/rose_arch_compressions/rose_arch_tar.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rose/apps/rose_bunch.py` & `metomi-rose-2.1.0/metomi/rose/apps/rose_bunch.py`

 * *Files 2% similar despite different names*

```diff
@@ -287,14 +287,18 @@
                 instances,
                 "inconsistent arg lengths",
             )
 
         # Set max number of processes to run at once
         max_procs = conf_tree.node.get_value([self.BUNCH_SECTION, "pool-size"])
 
+        # Add CYLC_TASK_FLOW_NUMBERS to configuration:
+        cylc_task_flow_numbers = os.environ.get('CYLC_TASK_FLOW_NUMBERS', "0")
+        conf_tree.node.set(['CYLC_TASK_FLOW_NUMBERS'], cylc_task_flow_numbers)
+
         if max_procs:
             max_procs = int(metomi.rose.env.env_var_process(max_procs))
         else:
             max_procs = arglength
 
         if self.incremental == "true":
             self.dao = RoseBunchDAO(conf_tree)
@@ -471,15 +475,15 @@
         if self.conn is None:
             self.conn = sqlite3.connect(self.db_file_name, self.CONN_TIMEOUT)
         return
 
     def create_tables(self):
         """Create tables as appropriate"""
         existing = []
-        first_run = os.environ.get("CYLC_TASK_TRY_NUMBER") == "1"
+        first_run = os.environ.get("CYLC_TASK_SUBMIT_NUMBER") == "1"
 
         for row in self.conn.execute(
             "SELECT name FROM sqlite_master " + "WHERE type=='table'"
         ):
             existing.append(row[0])
 
         if first_run:
@@ -562,15 +566,14 @@
             if not isinstance(node.value, dict):
                 if not node.is_ignored():
                     flat["_".join(keys)] = node.value
         return flat
 
     def record_config(self, config, clear_db=False):
         """Take in a conf_tree object and record the entries"""
-
         if clear_db:
             d_stmt = "DELETE FROM " + self.TABLE_CONFIG
             self.conn.execute(d_stmt)
             self.conn.commit()
 
         res = self.flatten_config(config)
```

### Comparing `metomi-rose-2.0rc3/metomi/rose/apps/rose_prune.py` & `metomi-rose-2.1.0/metomi/rose/apps/rose_prune.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rose/c3.py` & `metomi-rose-2.1.0/metomi/rose/c3.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rose/check_software.py` & `metomi-rose-2.1.0/metomi/rose/check_software.py`

 * *Files 0% similar despite different names*

```diff
@@ -230,15 +230,15 @@
         if min_version:
             return (line + 'not ok (unknown version)', False)
         return (line + 'ok (unknown version)', True)
 
     # Check version < min_incompat_version.
     version = version_tuple(version_string)
     if min_incompat_version and version > min_incompat_version:
-        return(line + 'not ok (%s > %s)' % (
+        return (line + 'not ok (%s > %s)' % (
             version_string, version_str(min_incompat_version)), False)
 
     # Check version >= min_version.
     if min_version:
         if version >= min_version:
             return (line + 'ok (%s)' % version_string, True)
         else:
```

### Comparing `metomi-rose-2.0rc3/metomi/rose/checksum.py` & `metomi-rose-2.1.0/metomi/rose/checksum.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rose/config.py` & `metomi-rose-2.1.0/metomi/rose/config.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rose/config_cli.py` & `metomi-rose-2.1.0/metomi/rose/config_cli.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rose/config_diff.py` & `metomi-rose-2.1.0/metomi/rose/config_diff.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rose/config_dump.py` & `metomi-rose-2.1.0/metomi/rose/config_dump.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rose/config_processor.py` & `metomi-rose-2.1.0/metomi/rose/config_processor.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,16 +12,14 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with Rose. If not, see <http://www.gnu.org/licenses/>.
 # -----------------------------------------------------------------------------
 """Process named settings in metomi.rose.config.ConfigTree."""
 
-import os
-import sys
 from typing import Optional
 
 from metomi.rose.env import UnboundEnvironmentVariableError
 from metomi.rose.fs_util import FileSystemUtil
 from metomi.rose.popen import RosePopener
 from metomi.rose.scheme_handler import SchemeHandlersManager
 
@@ -104,19 +102,19 @@
         self.event_handler = event_handler
         if popen is None:
             popen = RosePopener(event_handler)
         self.popen = popen
         if fs_util is None:
             fs_util = FileSystemUtil(event_handler)
         self.fs_util = fs_util
-        path = os.path.dirname(
-            os.path.dirname(sys.modules["metomi.rose"].__file__)
-        )
         SchemeHandlersManager.__init__(
-            self, [path], "rose.config_processors", ["process"]
+            self,
+            [self.get_rose_path()],
+            "metomi.rose.config_processors",
+            ["process"]
         )
 
     def handle_event(self, *args, **kwargs):
         """Report an event."""
         if callable(self.event_handler):
             return self.event_handler(*args, **kwargs)
```

### Comparing `metomi-rose-2.0rc3/metomi/rose/config_processors/__init__.py` & `metomi-rose-2.1.0/metomi/rose/config_processors/__init__.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rose/config_processors/env.py` & `metomi-rose-2.1.0/metomi/rose/config_processors/env.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rose/config_processors/fileinstall.py` & `metomi-rose-2.1.0/metomi/rose/config_processors/fileinstall.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 from fnmatch import fnmatch
 from glob import glob
 from io import BytesIO
 import os
 import shlex
 from shutil import rmtree
 import sqlite3
-import sys
 from tempfile import mkdtemp
 from typing import Any, Optional
 from urllib.parse import urlparse
 
 import aiofiles
 from metomi.rose.checksum import (
     get_checksum,
@@ -621,18 +620,23 @@
             Path name.
         checksum:
             Computed checksum value.
         access_mode:
             File type and mode bits (see os.stat_result:st_mode).
     """
 
-    def __init__(self, name, checksum=None, access_mode=None):
-        self.name: str = name
-        self.checksum: Any = checksum
-        self.access_mode: Optional[int] = access_mode
+    def __init__(
+        self,
+        name: str,
+        checksum: Any = None,
+        access_mode: Optional[int] = None
+    ):
+        self.name = name
+        self.checksum = checksum
+        self.access_mode = access_mode
 
     def __lt__(self, other):
         return (self.name, self.checksum, self.access_mode) < (
             other.name,
             other.checksum,
             other.access_mode,
         )
@@ -820,19 +824,18 @@
         self.event_handler = event_handler
         if popen is None:
             popen = RosePopener(event_handler)
         self.popen = popen
         if fs_util is None:
             fs_util = FileSystemUtil(event_handler)
         self.fs_util = fs_util
-        path = os.path.dirname(os.path.dirname(sys.modules["rose"].__file__))
         SchemeHandlersManager.__init__(
             self,
-            [path],
-            ns="rose.loc_handlers",
+            [self.get_rose_path()],
+            ns="metomi.rose.loc_handlers",
             attrs=["parse", "pull"],
             can_handle="can_pull",
         )
 
     def handle_event(self, *args, **kwargs):
         """Call self.event_handler with given arguments if possible."""
         if callable(self.event_handler):
```

### Comparing `metomi-rose-2.0rc3/metomi/rose/config_tree.py` & `metomi-rose-2.1.0/metomi/rose/config_tree.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rose/date.py` & `metomi-rose-2.1.0/metomi/rose/date.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rose/date_cli.py` & `metomi-rose-2.1.0/metomi/rose/date_cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -234,42 +234,50 @@
             if CYLC5_FORMAT.match(arg):
                 args[i] = upgrade_cylc5_datetime(arg)
             elif UNIX_FORMAT.match(arg):
                 args[i] = upgrade_unix_datetime(arg)
     return args
 
 
-def main():
+def _main(argv):
     """Implement rose date."""
     if sys.stdin.isatty():
         print(
             'WARNING: "rose date" is deprecated, use the "isodatetime" '
             'command.',
             file=sys.stderr
         )
 
-    if '--help' in sys.argv:
+    if '--help' in argv:
         print('\n' + __doc__)
-        sys.exit()
+        return 0
 
-    sys.argv = _handle_old_datetimes(sys.argv)
-    sys.argv = _handle_old_offsets(sys.argv)
+    argv = _handle_old_datetimes(argv)
+    argv = _handle_old_offsets(argv)
 
     # Handle Legacy Rose-date -c functionality
-    if '-c' in sys.argv or '--use-task-cycle-time' in sys.argv:
+    if '-c' in argv or '--use-task-cycle-time' in argv:
         if os.getenv('ROSE_TASK_CYCLE_TIME'):
             os.environ['ISODATETIMEREF'] = os.getenv('ROSE_TASK_CYCLE_TIME')
         elif not os.getenv('ISODATETIMEREF'):
-            sys.exit(
-                "[FAIL] [UNDEFINED ENVIRONMENT VARIABLE] ROSE_TASK_CYCLE_TIME")
+            return (
+                "[FAIL] [UNDEFINED ENVIRONMENT VARIABLE] ROSE_TASK_CYCLE_TIME"
+            )
 
         for opt in ('-c', '--use-task-cycle-time'):
-            if opt in sys.argv:
+            if opt in argv:
                 sys.argv.remove(opt)
-        if 'ref' not in sys.argv:
-            sys.argv.append('ref')
+        if 'ref' not in argv:
+            argv.append('ref')
 
     # Convert ROSE_CYCLING_MODE to ISODATETIMECALENDAR
-    if os.getenv('ROSE_CYCLING_MODE'):
+    if os.getenv('ROSE_CYCLING_MODE') not in ['integer', None]:
         os.environ['ISODATETIMECALENDAR'] = os.getenv('ROSE_CYCLING_MODE')
 
-    sys.exit(iso_main())
+    sys.argv = argv
+    return iso_main()
+
+
+def main():
+    sys.exit(
+        _main(sys.argv)
+    )
```

### Comparing `metomi-rose-2.0rc3/metomi/rose/env.py` & `metomi-rose-2.1.0/metomi/rose/env.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rose/env_cat.py` & `metomi-rose-2.1.0/metomi/rose/env_cat.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rose/etc/lib/bash/rose_log` & `metomi-rose-2.1.0/metomi/rose/etc/lib/bash/rose_log`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rose/etc/lib/bash/rose_usage` & `metomi-rose-2.1.0/metomi/rose/etc/lib/bash/rose_usage`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/fcm_make/HEAD/rose-meta.conf` & `metomi-rose-2.1.0/metomi/rose/etc/rose-meta/fcm_make/HEAD/rose-meta.conf`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose-all/etc/images/icon.png` & `metomi-rose-2.1.0/metomi/rose/etc/rose-meta/rose-all/etc/images/icon.png`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose-app-conf/rose-meta.conf` & `metomi-rose-2.1.0/metomi/rose/etc/rose-meta/rose-app-conf/rose-meta.conf`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose-demo-baked-alaska-sponge/vn1.0/lib/python/macros/desoggy.py` & `metomi-rose-2.1.0/metomi/rose/etc/rose-meta/rose-demo-baked-alaska-sponge/vn1.0/lib/python/macros/desoggy.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose-demo-upgrade/HEAD/rose-meta.conf` & `metomi-rose-2.1.0/metomi/rose/etc/rose-meta/rose-demo-upgrade/HEAD/rose-meta.conf`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose-demo-upgrade/garden0.9/rose-meta.conf` & `metomi-rose-2.1.0/metomi/rose/etc/rose-meta/rose-demo-upgrade/garden0.9/rose-meta.conf`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose-demo-upgrade/versions.py` & `metomi-rose-2.1.0/metomi/rose/etc/rose-meta/rose-demo-upgrade/versions.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose-demo-upgrade-null/versions.py` & `metomi-rose-2.1.0/metomi/rose/etc/rose-meta/rose-demo-upgrade-null/versions.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose-suite-conf/rose-meta.conf` & `metomi-rose-2.1.0/metomi/rose/etc/rose-meta/rose-suite-conf/rose-meta.conf`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose-suite-info/rose-meta.conf` & `metomi-rose-2.1.0/metomi/rose/etc/rose-meta/rose-suite-info/rose-meta.conf`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose_bunch/HEAD/rose-meta.conf` & `metomi-rose-2.1.0/metomi/rose/etc/rose-meta/rose_bunch/HEAD/rose-meta.conf`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rose/etc/rose-meta/rose_prune/HEAD/rose-meta.conf` & `metomi-rose-2.1.0/metomi/rose/etc/rose-meta/rose_prune/HEAD/rose-meta.conf`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rose/etc/syntax/rose-conf-mode.el` & `metomi-rose-2.1.0/metomi/rose/etc/syntax/rose-conf-mode.el`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rose/etc/syntax/rose-conf.lang` & `metomi-rose-2.1.0/metomi/rose/etc/syntax/rose-conf.lang`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rose/etc/syntax/rose-conf.vim` & `metomi-rose-2.1.0/metomi/rose/etc/syntax/rose-conf.vim`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rose/etc/syntax/rose-conf.xml` & `metomi-rose-2.1.0/metomi/rose/etc/syntax/rose-conf.xml`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rose/etc/tutorial/consolidation-tutorial/bin/forecast` & `metomi-rose-2.1.0/metomi/rose/etc/tutorial/cylc-forecasting-workflow/bin/forecast`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,28 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 # -----------------------------------------------------------------------------
-# Copyright (C) British Crown (Met Office) & Contributors - GNU V3+.
+# THIS FILE IS PART OF THE CYLC WORKFLOW ENGINE.
+# Copyright (C) NIWA & British Crown (Met Office) & Contributors.
+#
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU General Public License as published by
+# the Free Software Foundation, either version 3 of the License, or
+# (at your option) any later version.
+#
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU General Public License for more details.
+#
+# You should have received a copy of the GNU General Public License
+# along with this program.  If not, see <http://www.gnu.org/licenses/>.
+# -----------------------------------------------------------------------------
 # This is illustrative code developed for tutorial purposes, it is not
 # intended for scientific use and is not guarantied to be accurate or correct.
-# -----------------------------------------------------------------------------
 """
 Usage:
     forecast INTERVAL ITERATIONS
 
 Arguments:
     INTERVAL: The period between forecasts in minutes.
     ITERATIONS: The number of forecasts to produce.
@@ -43,15 +57,15 @@
         wind_file_path (str): Template for the path to a wind data file.
             The template should contain substitutions for `{cycles}`
             (i.e. the cycle point) and `{xy}` (i.e. the value 'x' or 'y').
         wind_cycles (list): List of cycle points to get wind data for
             as strings.
 
     Return:
-            list - A list 2-tuples containing wind field matricies i.e.
+            list - A list 2-tuples containing wind field matrices i.e.
             [(wind_x, wind_y), ...]
 
     """
     wind_fields = []
     for cycle in wind_cycles:
         wind_x = util.read_csv(wind_file_path.format(cycle=cycle, xy='x'))
         wind_y = util.read_csv(wind_file_path.format(cycle=cycle, xy='y'))
@@ -176,16 +190,16 @@
     """
     return Popen(
         ['cylc', 'cyclepoint', '--offset-hours', str(int(offset_hours))],
         stdout=PIPE
     ).communicate()[0].strip().decode()
 
 
-def main(forecast_interval, forecast_itterations):
-    # Get suite settings.
+def main(forecast_interval, forecast_iterations):
+    # Get workflow settings.
     domain = util.parse_domain(os.environ['DOMAIN'])
     resolution = float(os.environ['RESOLUTION'])
 
     # Get science settings.
     spline_level = int(os.environ.get('SPLINE_LEVEL', 0))
     weighting = list(map(float, os.environ.get('WEIGHTING', '1').split(',')))
 
@@ -208,15 +222,15 @@
 
     # Initiate the forecaster.
     generator = push_rainfall(rainfall, weighted_wind_data, forecast_interval,
                               resolution, spline_level)
 
     # Generate forecasts.
     forecasts = {}
-    for lead_minutes in range(0, forecast_interval * (forecast_itterations + 1),
+    for lead_minutes in range(0, forecast_interval * (forecast_iterations + 1),
                               forecast_interval):
         forecast_name = '+PT%02dH%02dM' % (lead_minutes // 60,
                                            lead_minutes % 60)
         # Generate forecast.
         forecast = next(generator)
         forecasts[forecast_name] = forecast
         # Output forecast data.
```

### Comparing `metomi-rose-2.0rc3/metomi/rose/etc/tutorial/consolidation-tutorial/bin/get-rainfall` & `metomi-rose-2.1.0/metomi/rose/etc/tutorial/cylc-forecasting-workflow/bin/get-rainfall`

 * *Files 14% similar despite different names*

```diff
@@ -1,44 +1,64 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 # -----------------------------------------------------------------------------
-# Copyright (C) British Crown (Met Office) & Contributors - GNU V3+.
+# THIS FILE IS PART OF THE CYLC WORKFLOW ENGINE.
+# Copyright (C) NIWA & British Crown (Met Office) & Contributors.
+#
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU General Public License as published by
+# the Free Software Foundation, either version 3 of the License, or
+# (at your option) any later version.
+#
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU General Public License for more details.
+#
+# You should have received a copy of the GNU General Public License
+# along with this program.  If not, see <http://www.gnu.org/licenses/>.
+# -----------------------------------------------------------------------------
 # This is illustrative code developed for tutorial purposes, it is not
 # intended for scientific use and is not guarantied to be accurate or correct.
-# -----------------------------------------------------------------------------
 """
 Usage:
     get-rainfall
 
 Environment Variables:
     API_KEY: The DataPoint API key, required for getting live weather data.
         If un-specified then get-observations will fall back to archive data
-        from the suite directory.
-    DOMIAN: The area in which to generate forecasts for in the format
+        from the workflow directory.
+    DOMAIN: The area in which to generate forecasts for in the format
         (lng1, lat1, lng2, lat2).
     RESOLUTION: The length/width of each grid cell in degrees.
 
 """
 
 from datetime import datetime
 import math
 import os
 import shutil
-import urllib.request
 
-import PIL.Image
-from mecator import get_offset, get_scale, coord_to_pos, pos_to_coord
+import requests
+
+try:
+    from PIL import Image
+except ModuleNotFoundError:
+    # not all PIL installations are created equal
+    # sometimes we must import like this
+    import Image
+from mercator import get_offset, get_scale, pos_to_coord
 import util
 
 
 URL = ('http://datapoint.metoffice.gov.uk/public/data/layer/wxobs/'
        'RADAR_UK_Composite_Highres/png?TIME={time}&key={api_key}')
 
 
-class Rainfall:
+class Rainfall(object):
     """Class for holding rainfall data.
 
     Args:
         domain (dict): Domain as returned by util.parse_domain()
         resolution (float): The length of each grid cell in degrees.
 
     """
@@ -52,30 +72,32 @@
         (254, 0, 254, 255): 7
     }
 
     def __init__(self, domain, resolution):
         self.resolution = resolution
         self.domain = domain
 
-        rows = int(math.ceil(abs(domain['lat1'] - domain['lat2']) / resolution))
-        cols = int(math.ceil(abs(domain['lng1'] - domain['lng2']) / resolution))
+        rows = int(
+            math.ceil(abs(domain['lat1'] - domain['lat2']) / resolution))
+        cols = int(
+            math.ceil(abs(domain['lng1'] - domain['lng2']) / resolution))
 
         self.data = []
         for itt_y in range(rows):
             self.data.append([])
             for _ in range(cols):
                 self.data[itt_y].append([])
 
     def add(self, lng, lat, value):
         """Add a data point to this data set.
 
         Args:
             lng (float): The longitude for this reading.
             lat (float): The latitude fo this reading.
-            value (float): The value of the reading.
+            value (tuple): The value of the reading.
 
         """
         itt_x, itt_y = util.get_grid_coordinates(lng, lat, self.domain,
                                                  self.resolution)
         try:
             self.data[itt_y][itt_x].append(self.VALUE_MAP[value])
         except KeyError:
@@ -93,56 +115,58 @@
 
 
 def get_datapoint_radar_image(filename, time, api_key):
     """Retrieve a png image of rainfall from the DataPoint service.
 
     Args:
         filename (str): The path to write the image file to.
-        time (str): The date-time of the image to reteieve in ISO8601 format.
+        time (str): The datetime of the image to retrieve in ISO8601 format.
         api_key (str): Datapoint API key.
 
     """
-    time = datetime.strptime(time, '%Y%m%dT%H%MZ'
-                            ).strftime('%Y-%m-%dT%H:%M:%SZ')
+    time = datetime.strptime(time, '%Y%m%dT%H%MZ').strftime(
+        '%Y-%m-%dT%H:%M:%SZ')
     url = URL.format(time=time, api_key=api_key)
-    print('Opening URL: %s' % url)
-    out = urllib.request.urlopen(url).read()
-    with open(filename, 'bw+') as png_file:
-        png_file.write(out)
+    req = requests.get(url)
+    if req.status_code != 200:
+        raise Exception(f'{url} returned exit code {req.status_code}')
+    with open(filename, 'bw') as png_file:
+        png_file.write(req.content)
 
 
 def get_archived_radar_image(filename, time):
-    """Retrieve a png image from the archived data in the suite directory.
+    """Retrieve a png image from the archived data in the workflow directory.
 
     Args:
         filename (str): The path to write the image file to.
-        time (str): The date-time of the image to reteieve in ISO8601 format.
+        time (str): The datetime of the image to retrieve in ISO8601 format.
 
     """
     shutil.copyfile(
-        os.path.join(os.environ['CYLC_SUITE_DEF_PATH'], 'data', time, filename),
+        os.path.join(os.environ['CYLC_WORKFLOW_RUN_DIR'], 'data', time,
+                     filename),
         filename)
 
 
 def process_rainfall_data(filename, resolution, domain):
-    """Generate a 2D matric of data from the rainfall data in the image.
+    """Generate a 2D matrix of data from the rainfall data in the image.
 
     Args:
         filename (str): Path to the png image to process.
-        resolution (float): The length/wieght of each grid cell in degrees.
+        resolution (float): The length/weight of each grid cell in degrees.
         domain (dict): The bounds of the domain as returned by
             util.parse_domain.
 
     Return:
         list - A 2D matrix of rainfall data.
 
     """
     rainfall = Rainfall(domain, resolution)
 
-    image = PIL.Image.open(filename)
+    image = Image.open(filename)
     scale = get_scale(domain, image.width)
     offset = get_offset(domain, scale)
 
     for itt_x in range(image.width):
         for itt_y in range(image.height):
             lng, lat = pos_to_coord(
                 itt_x,
@@ -159,15 +183,15 @@
     domain = util.parse_domain(os.environ['DOMAIN'])
     api_key = os.environ.get('API_KEY')
 
     if api_key:
         print('Attempting to get weather data from the DataPoint service.')
         get_datapoint_radar_image('rainfall-radar.png', time, api_key)
     else:
-        print('No API key provided, falling back to arhived data')
+        print('No API key provided, falling back to archived data')
         get_archived_radar_image('rainfall-radar.png', time)
 
     data = process_rainfall_data('rainfall-radar.png', resolution, domain)
     util.write_csv('rainfall.csv', data)
 
 
 if __name__ == '__main__':
```

### Comparing `metomi-rose-2.0rc3/metomi/rose/etc/tutorial/consolidation-tutorial/bin/post-process` & `metomi-rose-2.1.0/metomi/rose/etc/tutorial/cylc-forecasting-workflow/bin/post-process`

 * *Files 27% similar despite different names*

```diff
@@ -1,25 +1,39 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 # -----------------------------------------------------------------------------
-# Copyright (C) British Crown (Met Office) & Contributors - GNU V3+.
+# THIS FILE IS PART OF THE CYLC WORKFLOW ENGINE.
+# Copyright (C) NIWA & British Crown (Met Office) & Contributors.
+#
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU General Public License as published by
+# the Free Software Foundation, either version 3 of the License, or
+# (at your option) any later version.
+#
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU General Public License for more details.
+#
+# You should have received a copy of the GNU General Public License
+# along with this program.  If not, see <http://www.gnu.org/licenses/>.
+# -----------------------------------------------------------------------------
 # This is illustrative code developed for tutorial purposes, it is not
 # intended for scientific use and is not guarantied to be accurate or correct.
-# -----------------------------------------------------------------------------
 """
 Usage:
     post-process SITE TIME
 
 Arguments:
     SITE: The name of the location to process data for.
     TIME: The time ahead of the cycle point to produce the forecast for in
           minutes.
 
 Environment Variables:
-    DOMIAN: The area in which to generate forecasts for in the format
+    DOMAIN: The area in which to generate forecasts for in the format
         (lng1, lat1, lng2, lat2).
     RESOLUTION: The length/width of each grid cell in degrees.
 
 """
 
 from datetime import datetime, timedelta
 import os
@@ -43,15 +57,15 @@
     lng, lat = SITE_LOCATIONS[site_name]
 
     # Load forecast data.
     filename = '+PT%02dH%02dM.csv' % (time // 60, time % 60)
     try:
         # The path to the forecast data file.
         forecast = util.read_csv(os.path.join(
-            os.environ['CYLC_SUITE_WORK_DIR'],
+            os.environ['CYLC_WORKFLOW_WORK_DIR'],
             os.environ['CYLC_TASK_CYCLE_POINT'],
             'forecast',
             filename
         ))
     except IOError:
         sys.exit('Could not find forecast "%s".' % filename)
```

### Comparing `metomi-rose-2.0rc3/metomi/rose/etc/tutorial/consolidation-tutorial/flow.cylc` & `metomi-rose-2.1.0/metomi/rose/etc/tutorial/cylc-forecasting-workflow/flow.cylc`

 * *Files 25% similar despite different names*

```diff
@@ -1,105 +1,96 @@
+#!jinja2
 [scheduler]
     UTC mode = True
+[task parameters]
+    # A list of the weather stations we will be fetching observations from.
+    station = camborne, heathrow, shetland, aldergrove
+    # A list of the sites we will be generating forecasts for.
+    site = exeter
 
 [scheduling]
-    # Start the suite 7 hours before now ignoring minutes and seconds
+    # Start the workflow 7 hours before now ignoring minutes and seconds
     # * previous(T-00) takes the current time ignoring minutes and seconds.
     # * - PT7H subtracts 7 hours from the time.
     initial cycle point = previous(T-00) - PT7H
-    # Stop the suite 6 hours after the initial cycle point.
+    # Stop the workflow 6 hours after the initial cycle point.
     final cycle point = +PT6H
-    [[dependencies]]
-        [[[PT3H]]]
-            # Repeat every three hours starting at the initial cycle point.
-            graph = """
-                get_observations_belmullet => consolidate_observations
-                get_observations_camborne => consolidate_observations
-                get_observations_heathrow => consolidate_observations
-                get_observations_shetland => consolidate_observations
-            """
-
-        [[[+PT6H/PT6H]]]
-            # Repeat every six hours starting six hours after the initial
-            # cycle point.
-            graph = """
-                consolidate_observations => forecast
-                consolidate_observations[-PT3H] => forecast
-                consolidate_observations[-PT6H] => forecast
-                get_rainfall => forecast => post_process_exeter
-            """
-
-        [[[+PT12H/PT6H]]]
-            # Repeat every six hours starting twelve hours after the initial
-            # cycle point.
-            graph = """
-                forecast[-PT6H] => forecast
-            """
+    [[graph]]
+        # Repeat every three hours starting at the initial cycle point.
+        PT3H = """
+            get_observations<station> => consolidate_observations
+        """
+
+        # Repeat every six hours starting six hours after the initial
+        # cycle point.
+        +PT6H/PT6H = """
+            consolidate_observations => forecast
+            consolidate_observations[-PT3H] => forecast
+            consolidate_observations[-PT6H] => forecast
+            get_rainfall => forecast => post_process<site>
+        """
+
+        # Repeat every six hours starting twelve hours after the initial
+        # cycle point.
+        +PT12H/PT6H = """
+            forecast[-PT6H] => forecast
+        """
+
 [runtime]
-    [[get_observations_belmullet]]
+    [[root]]
+        # These environment variables will be available to all tasks.
+        [[[environment]]]
+            # The dimensions of each grid cell in degrees.
+            RESOLUTION = 0.2
+            # The area to generate forecasts for (lng1, lat1, lng2, lat2)
+            DOMAIN = -12,48,5,61  # Do not change!
+
+    [[get_observations<station>]]
         script = get-observations
         [[[environment]]]
-            SITE_ID = 3976
+            # The key required to get weather data from the DataPoint service.
+            # To use archived data comment this line out.
             API_KEY = DATAPOINT_API_KEY
-    [[get_observations_camborne]]
-        script = get-observations
+
+    [[get_observations<station=aldergrove>]]
+        [[[environment]]]
+            SITE_ID = 3917
+    [[get_observations<station=camborne>]]
         [[[environment]]]
             SITE_ID = 3808
-            API_KEY = DATAPOINT_API_KEY
-    [[get_observations_heathrow]]
-        script = get-observations
+    [[get_observations<station=heathrow>]]
         [[[environment]]]
             SITE_ID = 3772
-            API_KEY = DATAPOINT_API_KEY
-    [[get_observations_shetland]]
-        script = get-observations
+    [[get_observations<station=shetland>]]
         [[[environment]]]
             SITE_ID = 3005
-            API_KEY = DATAPOINT_API_KEY
-
 
     [[consolidate_observations]]
         script = consolidate-observations
-        [[[environment]]]
-            # The dimensions of each grid cell in degrees.
-            RESOLUTION = 0.2
-            # The area to generate forecasts for (lng1, lat1, lng2, lat2)
-            DOMAIN = -12,48,5,61  # Do not change!
 
     [[get_rainfall]]
         script = get-rainfall
         [[[environment]]]
             # The key required to get weather data from the DataPoint service.
             # To use archived data comment this line out.
             API_KEY = DATAPOINT_API_KEY
-            # The dimensions of each grid cell in degrees.
-            RESOLUTION = 0.2
-            # The area to generate forecasts for (lng1, lat1, lng2, lat2)
-            DOMAIN = -12,48,5,61  # Do not change!
 
     [[forecast]]
         script = forecast 60 5  # Generate 5 forecasts at 60 minute intervals.
         [[[environment]]]
-            # The dimensions of each grid cell in degrees.
-            RESOLUTION = 0.2
-            # The area to generate forecasts for (lng1, lat1, lng2, lat2)
-            DOMAIN = -12,48,5,61  # Do not change!
             # The path to the files containing wind data (the {variables} will
             # get substituted in the forecast script).
-            WIND_FILE_TEMPLATE = $CYLC_SUITE_WORK_DIR/{cycle}/consolidate_observations/wind_{xy}.csv
+            WIND_FILE_TEMPLATE = $CYLC_WORKFLOW_WORK_DIR/{cycle}/consolidate_observations/wind_{xy}.csv
             # Offset in hours to cycles to process wind data from.
             WIND_CYCLES = 0, -3, -6
             # The path to the rainfall file.
-            RAINFALL_FILE = $CYLC_SUITE_WORK_DIR/$CYLC_TASK_CYCLE_POINT/get_rainfall/rainfall.csv
+            RAINFALL_FILE = $CYLC_WORKFLOW_WORK_DIR/$CYLC_TASK_CYCLE_POINT/get_rainfall/rainfall.csv
             # Create the html map file in the task's log directory.
             MAP_FILE = "${CYLC_TASK_LOG_ROOT}-map.html"
             # The path to the template file used to generate the html map.
-            MAP_TEMPLATE = "$CYLC_SUITE_RUN_DIR/lib/template/map.html"
+            MAP_TEMPLATE = "$CYLC_WORKFLOW_RUN_DIR/lib/template/map.html"
 
-    [[post_process_exeter]]
-        # Generate a forecast for Exeter 60 minutes in the future.
-        script = post-process exeter 60
-        [[[environment]]]
-            # The dimensions of each grid cell in degrees.
-            RESOLUTION = 0.2
-            # The area to generate forecasts for (lng1, lat1, lng2, lat2)
-            DOMAIN = -12,48,5,61  # Do not change!
+    [[post_process<site>]]
+        # Generate a forecast for the location <site> 60 minutes in the future.
+        script = post-process $CYLC_TASK_PARAM_site 60
+
+{% include 'etc/python-job.settings' %}
```

### Comparing `metomi-rose-2.0rc3/metomi/rose/etc/tutorial/consolidation-tutorial/lib/python/mecator.py` & `metomi-rose-2.1.0/metomi/rose/etc/tutorial/cylc-forecasting-workflow/lib/python/mercator.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,34 @@
-# Copyright (C) British Crown (Met Office) & Contributors - GNU V3+.
+# -*- coding: utf-8 -*-
+# -----------------------------------------------------------------------------
+# THIS FILE IS PART OF THE CYLC WORKFLOW ENGINE.
+# Copyright (C) NIWA & British Crown (Met Office) & Contributors.
+#
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU General Public License as published by
+# the Free Software Foundation, either version 3 of the License, or
+# (at your option) any later version.
+#
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU General Public License for more details.
+#
+# You should have received a copy of the GNU General Public License
+# along with this program.  If not, see <http://www.gnu.org/licenses/>.
+# -----------------------------------------------------------------------------
 # This is illustrative code developed for tutorial purposes, it is not
 # intended for scientific use and is not guarantied to be accurate or correct.
-# -----------------------------------------------------------------------------
 import math
 
+
 R_0 = 6356752.3
 
 
-def get_offset(bbox, scale=(1.0, 1.0)):
+def get_offset(bbox, scale=(1., 1.)):
     """Define an offset from the origin using the provided bbox.
 
     Args:
         bbox: The coordinates of the domain as a dictionary {'lat1', 'lng1',
             'lat2', 'lng2'}
         scale: The x, y scale factor as returned by get_scale().
 
@@ -24,50 +41,49 @@
 
     Args:
         bbox: The coordinates of the domain as a dictionary {'lat1', 'lng1',
             'lat2', 'lng2'}
         width: The width of the projection.
 
     """
-    scale = width * (180.0 / abs(bbox['lng2'] - bbox['lng1']))
+    scale = width * (180. / abs(bbox['lng2'] - bbox['lng1']))
     return (
         (math.pi * R_0) / scale,
-        (math.pi * R_0 * 2.0) / scale,
-    )
+        (math.pi * R_0 * 2.) / scale)
 
 
-def coord_to_pos(lng, lat, offset=(0.0, 0.0), scale=(1.0, 1.0)):
-    """Convert a lng, lat coord to an x, y position in a mecator projection.
+def coord_to_pos(lng, lat, offset=(0., 0.), scale=(1., 1.)):
+    """Convert a lng, lat coord to an x, y position in a mercator projection.
 
     proj equivalent:
         $ echo <lng> <lat> | proj +proj=merc
         # Divide by scale.
         # Subtract offset.
 
     """
     lng = math.radians(lng)
     lat = math.radians(lat)
     pos_x = R_0 * lng
-    pos_y = R_0 * math.log(math.tan((math.pi / 4.0) + (lat / 2.0)))
+    pos_y = R_0 * math.log(math.tan((math.pi / 4.) + (lat / 2.)))
     pos_x /= scale[0]
     pos_y /= scale[1]
     pos_x -= offset[0]
     pos_y -= offset[1]
     return pos_x, pos_y
 
 
-def pos_to_coord(pos_x, pos_y, offset=(0.0, 0.0), scale=(1.0, 1.0)):
-    """Convert an x, y coordinate in a mecator projection to a lng, lat coord.
+def pos_to_coord(pos_x, pos_y, offset=(0., 0.), scale=(1., 1.)):
+    """Convert an x, y coordinate in a mercator projection to a lng, lat coord.
 
     proj equivalent:
         # Add offset
         # Multiply by scale.
         $ echo <pos_x> <pos_y> | proj -I +proj=merc
 
     """
     pos_x += offset[0]
     pos_y += offset[1]
     pos_x *= scale[0]
     pos_y *= scale[1]
     lng = pos_x / R_0
-    lat = 2 * math.atan(math.exp(pos_y / R_0)) - (math.pi / 2.0)
+    lat = 2 * math.atan(math.exp(pos_y / R_0)) - (math.pi / 2.)
     return math.degrees(lng), math.degrees(lat)
```

### Comparing `metomi-rose-2.0rc3/metomi/rose/etc/tutorial/consolidation-tutorial/lib/python/util.py` & `metomi-rose-2.1.0/metomi/rose/etc/tutorial/cylc-forecasting-workflow/lib/python/util.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,35 @@
-# Copyright (C) British Crown (Met Office) & Contributors - GNU V3+.
+# -*- coding: utf-8 -*-
+# -----------------------------------------------------------------------------
+# THIS FILE IS PART OF THE CYLC WORKFLOW ENGINE.
+# Copyright (C) NIWA & British Crown (Met Office) & Contributors.
+#
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU General Public License as published by
+# the Free Software Foundation, either version 3 of the License, or
+# (at your option) any later version.
+#
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU General Public License for more details.
+#
+# You should have received a copy of the GNU General Public License
+# along with this program.  If not, see <http://www.gnu.org/licenses/>.
+# -----------------------------------------------------------------------------
 # This is illustrative code developed for tutorial purposes, it is not
 # intended for scientific use and is not guarantied to be accurate or correct.
-# -----------------------------------------------------------------------------
 from copy import copy
+from contextlib import suppress
 import math
+import jinja2
 import sys
 
-import jinja2
 
-R_0 = 6371.0  # Radius of the Earth (km).
+R_0 = 6371.  # Radius of the Earth (km).
 
 
 def frange(start, stop, step):
     """Implementation of python's xrange which works with floats."""
     while start < stop:
         yield start
         start += step
@@ -48,27 +65,26 @@
 
     Args:
         filename (str): The path of the csv file to write to.
         field (function): A function of the form f(x, y) -> z.
         x_range (list): List of the x coordinates of the extrapolated grid.
             These are the extrapolation coordinates, the length of this list
             defines the size of the grid.
-        x_range (list): List of the y coordinates of the extrapolated grid.
+        y_range (list): List of the y coordinates of the extrapolated grid.
             These are the extrapolation coordinates, the length of this list
             defines the size of the grid.
 
     """
     with open(filename, 'w+') as csv_file:
         for itt_y in y_range:
-            csv_file.write(
-                ', '.join('%.2f' % field(x, itt_y) for x in x_range) + '\n'
-            )
+            csv_file.write(', '.join('%.2f' % field(x, itt_y) for
+                                     x in x_range) + '\n')
 
 
-def generate_matrix(dim_x, dim_y, value=0.0):
+def generate_matrix(dim_x, dim_y, value=0.):
     """Generates a 2D list with the desired dimensions.
 
     Args:
         dim_x (int): The x-dimension of the matrix.
         dim_y (int): The y-dimension of the matrix.
         value: The default value for each cell of the matrix.
 
@@ -99,23 +115,20 @@
     (lng_1, lat_1) = coordinate_1
     (lng_2, lat_2) = coordinate_2
     lng_1 = math.radians(lng_1)
     lat_1 = math.radians(lat_1)
     lng_2 = math.radians(lng_2)
     lat_2 = math.radians(lat_2)
     return (
-        2
-        * R_0
-        * math.asin(
+        2 * R_0 * math.asin(
             math.sqrt(
-                (math.sin((lat_2 - lat_1) / 2.0) ** 2)
-                + (
-                    math.cos(lat_1)
-                    * math.cos(lat_2)
-                    * (math.sin((lng_2 - lng_1) / 2.0) ** 2)
+                (math.sin((lat_2 - lat_1) / 2.) ** 2) + (
+                    math.cos(lat_1) *
+                    math.cos(lat_2) *
+                    (math.sin((lng_2 - lng_1) / 2.) ** 2)
                 )
             )
         )
     )
 
 
 def interpolate_grid(points, dim_x, dim_y, d_x, d_y, spline_order=0):
@@ -132,61 +145,57 @@
             interpolation (0 = nearset).
 
     Return:
         list - 2D matrix of dimensions dim_x, dim_y containing the interpolated
         data.
 
     """
-
     def spline_0(pos_x, pos_y, z_val):
         """Zeroth order beta spline (i.e. nearest point)."""
         return [(int(round(pos_x)), int(round(pos_y)), z_val)]  # [(x, y, z)]
 
     def spline_1(pos_x, pos_y, z_val):
-        """First order beta spline (weight spread about four nearest ponts)."""
+        """First order beta spline (weight spread about four nearest
+        points)."""
         x_0 = int(math.floor(pos_x))
         y_0 = int(math.floor(pos_y))
         x_1 = x_0 + 1
         y_1 = y_0 + 1
         return [
             # (x, y, z), ...
             (x_0, y_0, (x_0 + d_x - pos_x) * (y_0 + d_y - pos_y) * z_val),
             (x_1, y_0, (pos_x - x_0) * (y_0 + d_y - pos_y) * z_val),
             (x_0, y_1, (x_0 + d_x - pos_x) * (pos_y - y_0) * z_val),
-            (x_1, y_1, (pos_x - x_0) * (pos_y - y_0) * z_val),
+            (x_1, y_1, (pos_x - x_0) * (pos_y - y_0) * z_val)
         ]
 
     if spline_order == 0:
         spline = spline_0
-    elif spline_order == 1:
+    elif spline_order == 1:  # noqa: SIM106 (case type matching)
         spline = spline_1
     else:
-        raise ValueError(
-            'Invalid spline order "%d" must be in (0, 1).' % spline_order
-        )
+        raise ValueError('Invalid spline order "%d" must be in (0, 1).' %
+                         spline_order)
 
-    grid = generate_matrix(dim_x, dim_y, 0.0)
+    grid = generate_matrix(dim_x, dim_y, 0.)
 
     for x_val, y_val, z_val in points:
         x_coord = x_val / d_x
         y_coord = y_val / d_y
         for grid_x, grid_y, grid_z in spline(x_coord, y_coord, z_val):
-            try:
+            with suppress(IndexError):
                 grid[grid_y][grid_x] += grid_z
-            except IndexError:
-                # Grid point out of bounds => skip.
-                pass
+                # skip grid point out of bounds
 
     return grid
 
 
 def plot_vector_grid(filename, x_grid, y_grid):
     try:
         import matplotlib
-
         matplotlib.use('Agg')
         import matplotlib.pyplot as plt
     except ImportError:
         print('Plotting disabled', file=sys.stderr)
         return
 
     fig = plt.figure()
@@ -195,34 +204,31 @@
     z_coords = []
     for itt_x in range(len(x_grid[0])):
         for itt_y in range(len(x_grid)):
             x_coords.append(itt_x)
             y_coords.append(itt_y)
             z_coords.append((
                 x_grid[itt_y][itt_x],
-                y_grid[itt_y][itt_x],
+                y_grid[itt_y][itt_x]
             ))
 
-    plt.quiver(
-        x_coords,
-        y_coords,
-        [x[0] for x in z_coords],
-        [y[1] for y in z_coords],
-    )
+    plt.quiver(x_coords,
+               y_coords,
+               [x[0] for x in z_coords],
+               [y[1] for y in z_coords])
     fig.savefig(filename)
 
 
 def get_grid_coordinates(lng, lat, domain, resolution):
     """Return the grid coordinates for a lat, long coordinate pair."""
     # NOTE: Grid coordinates run from *top* left to bottom right.
     length_y = int(abs(domain['lat2'] - domain['lat1']) // resolution)
     return (
         int((abs(lng - domain['lng1'])) // resolution),
-        length_y - int((abs(lat - domain['lat1'])) // resolution),
-    )
+        length_y - int((abs(lat - domain['lat1'])) // resolution))
 
 
 class SurfaceFitter:
     """A 2D interpolation for random points.
 
     A standin for scipy.interpolate.interp2d
 
@@ -239,19 +245,19 @@
 
     """
 
     def __init__(self, x_points, y_points, z_points, kind='linear'):
         self.points = list(zip(x_points, y_points, z_points))
 
         if kind == 'linear':
-            self.power = 1.0
+            self.power = 1.
         elif kind == 'quadratic':
-            self.power = 2.0
-        elif kind == 'cubic':
-            self.power = 3.0
+            self.power = 2.
+        elif kind == 'cubic':  # noqa: SIM106 (case type matching)
+            self.power = 3.
         else:
             raise ValueError('"%s" is not a valid interpolation method' % kind)
 
     def __call__(self, grid_x, grid_y):
         sum_value = 0.0
         sum_weight = 0.0
         z_val = None
@@ -260,15 +266,15 @@
             d_y = grid_y - y_point
             if d_x == 0 and d_y == 0:
                 # This point is exactly at the grid location we are
                 # interpolating for, return this value.
                 z_val = z_point
                 break
             else:
-                weight = 1.0 / ((math.sqrt(d_x ** 2 + d_y ** 2)) ** self.power)
+                weight = 1. / ((math.sqrt(d_x ** 2 + d_y ** 2)) ** self.power)
                 sum_weight += weight
                 sum_value += weight * z_point
 
         if z_val is None:
             z_val = sum_value / sum_weight
 
         return z_val
@@ -276,24 +282,22 @@
 
 def parse_domain(domain):
     bbox = list(map(float, domain.split(',')))
     return {
         'lng1': bbox[0],
         'lat1': bbox[1],
         'lng2': bbox[2],
-        'lat2': bbox[3],
+        'lat2': bbox[3]
     }
 
 
 def generate_html_map(filename, template_file, data, domain, resolution):
-    with open(template_file, 'r') as template:
+    with open(template_file, 'r') as template:  # noqa: SIM117
         with open(filename, 'w+') as html_file:
-            html_file.write(
-                jinja2.Template(template.read()).render(
-                    resolution=resolution,
-                    lng1=domain['lng1'],
-                    lng2=domain['lng2'],
-                    lat1=domain['lat1'],
-                    lat2=domain['lat2'],
-                    data=data,
-                )
-            )
+            html_file.write(jinja2.Template(template.read()).render(
+                resolution=resolution,
+                lng1=domain['lng1'],
+                lng2=domain['lng2'],
+                lat1=domain['lat1'],
+                lat2=domain['lat2'],
+                data=data
+            ))
```

### Comparing `metomi-rose-2.0rc3/metomi/rose/etc/tutorial/consolidation-tutorial/lib/template/map.html` & `metomi-rose-2.1.0/metomi/rose/etc/tutorial/cylc-forecasting-workflow/lib/template/map.html`

 * *Files 10% similar despite different names*

```diff
@@ -1,82 +1,93 @@
 <html>
-  <head>
-    <link rel="stylesheet"
-          href="https://unpkg.com/leaflet@1.2.0/dist/leaflet.css" />
+
+<head>
+    <link rel="stylesheet" href="https://unpkg.com/leaflet@1.2.0/dist/leaflet.css" />
     <script src="https://unpkg.com/leaflet@1.2.0/dist/leaflet.js"></script>
-  </head>
-  <body>
+</head>
+
+<body>
     <div id="map" style="width:100%;height:100%"></div>
 
     <script type="text/javascript">
-      // Define the colours to display for the different rainfall values.
-      // NOTE: Rainfall values range from 0 to 6+.
-      function get_colour(value) {
-          if (value < 0.1)
-              return '#ffffff88';
-          if (value < 0.5)
-              return '#00F7FF';
-          if (value < 1)
-              return '#00AAFF';
-          else if (value < 2)
-              return '#0051FF';
-          else if (value < 3)
-              return '#6600FF';
-          else if (value < 4)
-              return '#AE00FF';
-          else if (value < 5)
-              return '#FF00EA';
-          else
-              return '#FF0055';
-      }
-
-      // Forecast data as dict {'lead_time': [2d data matrix]}.
-      var data = {{ data }};
-
-      // Annotate map with data.
-      var lng;
-      var lat;
-      var rects;
-      var times = [];
-      var layers = [];
-      for (let time in data) {
-          rects = L.layerGroup();
-          for (let pos_y in data[time]) {
-              for (let pos_x in data[time][0]) {
-                  lng = (pos_x * {{ resolution }}) + {{ lng1 }};
-                  lat = {{ lat2 }} - (pos_y * {{ resolution }});
-                  L.rectangle(
-                      [[lat, lng],
-                      [lat + {{ resolution }}, lng + {{ resolution }}]],
-                      {color: get_colour(data[time][pos_y][pos_x]),
-                       weight: 0, fillOpacity: 0.5}).addTo(rects);
-              }
-          }
-          layers.push(rects);
-          times.push(time);
-      }
-
-      // Sort map layers lexicographically.
-      var sorted_times = times.slice(0);  // Copy the times list.
-      var fcsts = {};  // {'lead_time': L.LayerGroup}  Note dicts are ordered.
-      sorted_times.sort();
-      var ind;
-      for (let time of sorted_times) {
-          ind = times.indexOf(time);
-          fcsts[times[ind]] = layers[ind];
-      }
-
-      // Create map.
-      var map = L.map('map', {layers: [fcsts[sorted_times[0]]]});
-
-      // Zoom / center map to fit domain.
-      map.fitBounds([[{{ lat1 }}, {{ lng1 }}], [{{ lat2 }}, {{ lng2 }}]]);
-
-      // Add mapp tiles.
-      map.addLayer(
-          L.tileLayer('http://{s}.tile.openstreetmap.org/{z}/{x}/{y}.png'));
+        // Define the colours to display for the different rainfall values.
+        // NOTE: Rainfall values range from 0 to 6+.
+        function get_colour(value) {
+            if (value < 0.1)
+                return '#ffffff88';
+            if (value < 0.5)
+                return '#00F7FF';
+            if (value < 1)
+                return '#00AAFF';
+            else if (value < 2)
+                return '#0051FF';
+            else if (value < 3)
+                return '#6600FF';
+            else if (value < 4)
+                return '#AE00FF';
+            else if (value < 5)
+                return '#FF00EA';
+            else
+                return '#FF0055';
+        }
+
+        // Forecast data as dict {'lead_time': [2d data matrix]}.
+        var data = {{ data }};
+
+        // Annotate map with data.
+        var lng;
+        var lat;
+        var rects;
+        var times = [];
+        var layers = [];
+        for (let time in data) {
+            rects = L.layerGroup();
+            for (let pos_y in data[time]) {
+                for (let pos_x in data[time][0]) {
+                    lng = (pos_x * {{ resolution }}) + {{ lng1 }};
+                    lat = {{ lat2 }} - (pos_y * {{ resolution }});
+                    L.rectangle(
+                        [
+                            [lat, lng],
+                            [lat + {{ resolution }}, lng + {{ resolution }}]
+                        ], {
+                            color: get_colour(data[time][pos_y][pos_x]),
+                            weight: 0,
+                            fillOpacity: 0.5
+                        }).addTo(rects);
+                }
+            }
+            layers.push(rects);
+            times.push(time);
+        }
+
+        // Sort map layers lexicographically.
+        var sorted_times = times.slice(0); // Copy the times list.
+        var fcsts = {}; // {'lead_time': L.LayerGroup}  Note dicts are ordered.
+        sorted_times.sort();
+        var ind;
+        for (let time of sorted_times) {
+            ind = times.indexOf(time);
+            fcsts[times[ind]] = layers[ind];
+        }
+
+        // Create map.
+        var map = L.map('map', {
+            layers: [fcsts[sorted_times[0]]]
+        });
+
+        // Zoom / center map to fit domain.
+        map.fitBounds([
+            [{{ lat1 }}, {{ lng1 }}],
+            [{{ lat2 }}, {{ lng2 }}]
+        ]);
+
+        // Add map tiles.
+        map.addLayer(
+            L.tileLayer('http://{s}.tile.openstreetmap.org/{z}/{x}/{y}.png'));
 
-      // Add layer selector.
-      L.control.layers(fcsts).addTo(map);
+        // Add layer selector.
+        L.control.layers(fcsts).addTo(map);
     </script>
-  </body>
+</body>
+
 </html>
```

### Comparing `metomi-rose-2.0rc3/metomi/rose/etc/tutorial/cylc-forecasting-suite/bin/forecast` & `metomi-rose-2.1.0/metomi/rose/etc/tutorial/forecast-script/forecast`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,28 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 # -----------------------------------------------------------------------------
-# Copyright (C) British Crown (Met Office) & Contributors - GNU V3+.
+# THIS FILE IS PART OF THE CYLC WORKFLOW ENGINE.
+# Copyright (C) NIWA & British Crown (Met Office) & Contributors.
+#
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU General Public License as published by
+# the Free Software Foundation, either version 3 of the License, or
+# (at your option) any later version.
+#
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU General Public License for more details.
+#
+# You should have received a copy of the GNU General Public License
+# along with this program.  If not, see <http://www.gnu.org/licenses/>.
+# -----------------------------------------------------------------------------
 # This is illustrative code developed for tutorial purposes, it is not
 # intended for scientific use and is not guarantied to be accurate or correct.
-# -----------------------------------------------------------------------------
 """
 Usage:
     forecast INTERVAL ITERATIONS
 
 Arguments:
     INTERVAL: The period between forecasts in minutes.
     ITERATIONS: The number of forecasts to produce.
@@ -43,15 +57,15 @@
         wind_file_path (str): Template for the path to a wind data file.
             The template should contain substitutions for `{cycles}`
             (i.e. the cycle point) and `{xy}` (i.e. the value 'x' or 'y').
         wind_cycles (list): List of cycle points to get wind data for
             as strings.
 
     Return:
-            list - A list 2-tuples containing wind field matricies i.e.
+            list - A list 2-tuples containing wind field matrices i.e.
             [(wind_x, wind_y), ...]
 
     """
     wind_fields = []
     for cycle in wind_cycles:
         wind_x = util.read_csv(wind_file_path.format(cycle=cycle, xy='x'))
         wind_y = util.read_csv(wind_file_path.format(cycle=cycle, xy='y'))
@@ -176,16 +190,16 @@
     """
     return Popen(
         ['cylc', 'cyclepoint', '--offset-hours', str(int(offset_hours))],
         stdout=PIPE
     ).communicate()[0].strip().decode()
 
 
-def main(forecast_interval, forecast_itterations):
-    # Get suite settings.
+def main(forecast_interval, forecast_iterations):
+    # Get workflow settings.
     domain = util.parse_domain(os.environ['DOMAIN'])
     resolution = float(os.environ['RESOLUTION'])
 
     # Get science settings.
     spline_level = int(os.environ.get('SPLINE_LEVEL', 0))
     weighting = list(map(float, os.environ.get('WEIGHTING', '1').split(',')))
 
@@ -208,15 +222,15 @@
 
     # Initiate the forecaster.
     generator = push_rainfall(rainfall, weighted_wind_data, forecast_interval,
                               resolution, spline_level)
 
     # Generate forecasts.
     forecasts = {}
-    for lead_minutes in range(0, forecast_interval * (forecast_itterations + 1),
+    for lead_minutes in range(0, forecast_interval * (forecast_iterations + 1),
                               forecast_interval):
         forecast_name = '+PT%02dH%02dM' % (lead_minutes // 60,
                                            lead_minutes % 60)
         # Generate forecast.
         forecast = next(generator)
         forecasts[forecast_name] = forecast
         # Output forecast data.
```

### Comparing `metomi-rose-2.0rc3/metomi/rose/etc/tutorial/cylc-forecasting-suite/bin/get-rainfall` & `metomi-rose-2.1.0/metomi/rose/etc/tutorial/rose-suite-tutorial/bin/get-rainfall`

 * *Files 14% similar despite different names*

```diff
@@ -1,44 +1,64 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 # -----------------------------------------------------------------------------
-# Copyright (C) British Crown (Met Office) & Contributors - GNU V3+.
+# THIS FILE IS PART OF THE CYLC WORKFLOW ENGINE.
+# Copyright (C) NIWA & British Crown (Met Office) & Contributors.
+#
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU General Public License as published by
+# the Free Software Foundation, either version 3 of the License, or
+# (at your option) any later version.
+#
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU General Public License for more details.
+#
+# You should have received a copy of the GNU General Public License
+# along with this program.  If not, see <http://www.gnu.org/licenses/>.
+# -----------------------------------------------------------------------------
 # This is illustrative code developed for tutorial purposes, it is not
 # intended for scientific use and is not guarantied to be accurate or correct.
-# -----------------------------------------------------------------------------
 """
 Usage:
     get-rainfall
 
 Environment Variables:
     API_KEY: The DataPoint API key, required for getting live weather data.
         If un-specified then get-observations will fall back to archive data
-        from the suite directory.
-    DOMIAN: The area in which to generate forecasts for in the format
+        from the workflow directory.
+    DOMAIN: The area in which to generate forecasts for in the format
         (lng1, lat1, lng2, lat2).
     RESOLUTION: The length/width of each grid cell in degrees.
 
 """
 
 from datetime import datetime
 import math
 import os
 import shutil
-import urllib.request
 
-import PIL.Image
-from mecator import get_offset, get_scale, coord_to_pos, pos_to_coord
+import requests
+
+try:
+    from PIL import Image
+except ModuleNotFoundError:
+    # not all PIL installations are created equal
+    # sometimes we must import like this
+    import Image
+from mercator import get_offset, get_scale, pos_to_coord
 import util
 
 
 URL = ('http://datapoint.metoffice.gov.uk/public/data/layer/wxobs/'
        'RADAR_UK_Composite_Highres/png?TIME={time}&key={api_key}')
 
 
-class Rainfall:
+class Rainfall(object):
     """Class for holding rainfall data.
 
     Args:
         domain (dict): Domain as returned by util.parse_domain()
         resolution (float): The length of each grid cell in degrees.
 
     """
@@ -52,30 +72,32 @@
         (254, 0, 254, 255): 7
     }
 
     def __init__(self, domain, resolution):
         self.resolution = resolution
         self.domain = domain
 
-        rows = int(math.ceil(abs(domain['lat1'] - domain['lat2']) / resolution))
-        cols = int(math.ceil(abs(domain['lng1'] - domain['lng2']) / resolution))
+        rows = int(
+            math.ceil(abs(domain['lat1'] - domain['lat2']) / resolution))
+        cols = int(
+            math.ceil(abs(domain['lng1'] - domain['lng2']) / resolution))
 
         self.data = []
         for itt_y in range(rows):
             self.data.append([])
             for _ in range(cols):
                 self.data[itt_y].append([])
 
     def add(self, lng, lat, value):
         """Add a data point to this data set.
 
         Args:
             lng (float): The longitude for this reading.
             lat (float): The latitude fo this reading.
-            value (float): The value of the reading.
+            value (tuple): The value of the reading.
 
         """
         itt_x, itt_y = util.get_grid_coordinates(lng, lat, self.domain,
                                                  self.resolution)
         try:
             self.data[itt_y][itt_x].append(self.VALUE_MAP[value])
         except KeyError:
@@ -93,56 +115,58 @@
 
 
 def get_datapoint_radar_image(filename, time, api_key):
     """Retrieve a png image of rainfall from the DataPoint service.
 
     Args:
         filename (str): The path to write the image file to.
-        time (str): The date-time of the image to reteieve in ISO8601 format.
+        time (str): The datetime of the image to retrieve in ISO8601 format.
         api_key (str): Datapoint API key.
 
     """
-    time = datetime.strptime(time, '%Y%m%dT%H%MZ'
-                            ).strftime('%Y-%m-%dT%H:%M:%SZ')
+    time = datetime.strptime(time, '%Y%m%dT%H%MZ').strftime(
+        '%Y-%m-%dT%H:%M:%SZ')
     url = URL.format(time=time, api_key=api_key)
-    print('Opening URL: %s' % url)
-    out = urllib.request.urlopen(url).read()
-    with open(filename, 'bw+') as png_file:
-        png_file.write(out)
+    req = requests.get(url)
+    if req.status_code != 200:
+        raise Exception(f'{url} returned exit code {req.status_code}')
+    with open(filename, 'bw') as png_file:
+        png_file.write(req.content)
 
 
 def get_archived_radar_image(filename, time):
-    """Retrieve a png image from the archived data in the suite directory.
+    """Retrieve a png image from the archived data in the workflow directory.
 
     Args:
         filename (str): The path to write the image file to.
-        time (str): The date-time of the image to reteieve in ISO8601 format.
+        time (str): The datetime of the image to retrieve in ISO8601 format.
 
     """
     shutil.copyfile(
-        os.path.join(os.environ['CYLC_SUITE_DEF_PATH'], 'data', time, filename),
+        os.path.join(os.environ['CYLC_WORKFLOW_RUN_DIR'], 'data', time,
+                     filename),
         filename)
 
 
 def process_rainfall_data(filename, resolution, domain):
-    """Generate a 2D matric of data from the rainfall data in the image.
+    """Generate a 2D matrix of data from the rainfall data in the image.
 
     Args:
         filename (str): Path to the png image to process.
-        resolution (float): The length/wieght of each grid cell in degrees.
+        resolution (float): The length/weight of each grid cell in degrees.
         domain (dict): The bounds of the domain as returned by
             util.parse_domain.
 
     Return:
         list - A 2D matrix of rainfall data.
 
     """
     rainfall = Rainfall(domain, resolution)
 
-    image = PIL.Image.open(filename)
+    image = Image.open(filename)
     scale = get_scale(domain, image.width)
     offset = get_offset(domain, scale)
 
     for itt_x in range(image.width):
         for itt_y in range(image.height):
             lng, lat = pos_to_coord(
                 itt_x,
@@ -159,15 +183,15 @@
     domain = util.parse_domain(os.environ['DOMAIN'])
     api_key = os.environ.get('API_KEY')
 
     if api_key:
         print('Attempting to get weather data from the DataPoint service.')
         get_datapoint_radar_image('rainfall-radar.png', time, api_key)
     else:
-        print('No API key provided, falling back to arhived data')
+        print('No API key provided, falling back to archived data')
         get_archived_radar_image('rainfall-radar.png', time)
 
     data = process_rainfall_data('rainfall-radar.png', resolution, domain)
     util.write_csv('rainfall.csv', data)
 
 
 if __name__ == '__main__':
```

### Comparing `metomi-rose-2.0rc3/metomi/rose/etc/tutorial/cylc-forecasting-suite/bin/post-process` & `metomi-rose-2.1.0/metomi/rose/etc/tutorial/rose-suite-tutorial/bin/post-process`

 * *Files 27% similar despite different names*

```diff
@@ -1,25 +1,39 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 # -----------------------------------------------------------------------------
-# Copyright (C) British Crown (Met Office) & Contributors - GNU V3+.
+# THIS FILE IS PART OF THE CYLC WORKFLOW ENGINE.
+# Copyright (C) NIWA & British Crown (Met Office) & Contributors.
+#
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU General Public License as published by
+# the Free Software Foundation, either version 3 of the License, or
+# (at your option) any later version.
+#
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU General Public License for more details.
+#
+# You should have received a copy of the GNU General Public License
+# along with this program.  If not, see <http://www.gnu.org/licenses/>.
+# -----------------------------------------------------------------------------
 # This is illustrative code developed for tutorial purposes, it is not
 # intended for scientific use and is not guarantied to be accurate or correct.
-# -----------------------------------------------------------------------------
 """
 Usage:
     post-process SITE TIME
 
 Arguments:
     SITE: The name of the location to process data for.
     TIME: The time ahead of the cycle point to produce the forecast for in
           minutes.
 
 Environment Variables:
-    DOMIAN: The area in which to generate forecasts for in the format
+    DOMAIN: The area in which to generate forecasts for in the format
         (lng1, lat1, lng2, lat2).
     RESOLUTION: The length/width of each grid cell in degrees.
 
 """
 
 from datetime import datetime, timedelta
 import os
@@ -43,15 +57,15 @@
     lng, lat = SITE_LOCATIONS[site_name]
 
     # Load forecast data.
     filename = '+PT%02dH%02dM.csv' % (time // 60, time % 60)
     try:
         # The path to the forecast data file.
         forecast = util.read_csv(os.path.join(
-            os.environ['CYLC_SUITE_WORK_DIR'],
+            os.environ['CYLC_WORKFLOW_WORK_DIR'],
             os.environ['CYLC_TASK_CYCLE_POINT'],
             'forecast',
             filename
         ))
     except IOError:
         sys.exit('Could not find forecast "%s".' % filename)
```

### Comparing `metomi-rose-2.0rc3/metomi/rose/etc/tutorial/cylc-forecasting-suite/flow.cylc` & `metomi-rose-2.1.0/metomi/rose/etc/tutorial/rose-suite-tutorial/flow.cylc`

 * *Files 4% similar despite different names*

```diff
@@ -1,45 +1,43 @@
+#!jinja2
 [scheduler]
     UTC mode = True
-    [[parameters]]
-        # A list of the weather stations we will be fetching observations from.
-        station = camborne, heathrow, shetland, belmullet
-        # A list of the sites we will be generating forecasts for.
-        site = exeter
+[task parameters]
+    # A list of the weather stations we will be fetching observations from.
+    station = camborne, heathrow, shetland, aldergrove
+    # A list of the sites we will be generating forecasts for.
+    site = exeter
 
 [scheduling]
-    # Start the suite 7 hours before now ignoring minutes and seconds
+    # Start the workflow 7 hours before now ignoring minutes and seconds
     # * previous(T-00) takes the current time ignoring minutes and seconds.
     # * - PT7H subtracts 7 hours from the time.
     initial cycle point = previous(T-00) - PT7H
-    # Stop the suite 6 hours after the initial cycle point.
+    # Stop the workflow 6 hours after the initial cycle point.
     final cycle point = +PT6H
-    [[dependencies]]
-        [[[PT3H]]]
-            # Repeat every three hours starting at the initial cycle point.
-            graph = """
-                get_observations<station> => consolidate_observations
-            """
-
-        [[[+PT6H/PT6H]]]
-            # Repeat every six hours starting six hours after the initial
-            # cycle point.
-            graph = """
-                consolidate_observations => forecast
-                consolidate_observations[-PT3H] => forecast
-                consolidate_observations[-PT6H] => forecast
-                get_rainfall => forecast => post_process<site>
-            """
-
-        [[[+PT12H/PT6H]]]
-            # Repeat every six hours starting twelve hours after the initial
-            # cycle point.
-            graph = """
-                forecast[-PT6H] => forecast
-            """
+    [[graph]]
+        # Repeat every three hours starting at the initial cycle point.
+        PT3H = """
+            get_observations<station> => consolidate_observations
+        """
+
+        # Repeat every six hours starting six hours after the initial
+        # cycle point.
+        +PT6H/PT6H = """
+            consolidate_observations => forecast
+            consolidate_observations[-PT3H] => forecast
+            consolidate_observations[-PT6H] => forecast
+            get_rainfall => forecast => post_process<site>
+        """
+
+        # Repeat every six hours starting twelve hours after the initial
+        # cycle point.
+        +PT12H/PT6H = """
+            forecast[-PT6H] => forecast
+        """
 
 [runtime]
     [[root]]
         # These environment variables will be available to all tasks.
         [[[environment]]]
             # The dimensions of each grid cell in degrees.
             RESOLUTION = 0.2
@@ -49,17 +47,17 @@
     [[get_observations<station>]]
         script = get-observations
         [[[environment]]]
             # The key required to get weather data from the DataPoint service.
             # To use archived data comment this line out.
             API_KEY = DATAPOINT_API_KEY
 
-    [[get_observations<station=belmullet>]]
+    [[get_observations<station=aldergrove>]]
         [[[environment]]]
-            SITE_ID = 3976
+            SITE_ID = 3917
     [[get_observations<station=camborne>]]
         [[[environment]]]
             SITE_ID = 3808
     [[get_observations<station=heathrow>]]
         [[[environment]]]
             SITE_ID = 3772
     [[get_observations<station=shetland>]]
@@ -77,20 +75,22 @@
             API_KEY = DATAPOINT_API_KEY
 
     [[forecast]]
         script = forecast 60 5  # Generate 5 forecasts at 60 minute intervals.
         [[[environment]]]
             # The path to the files containing wind data (the {variables} will
             # get substituted in the forecast script).
-            WIND_FILE_TEMPLATE = $CYLC_SUITE_WORK_DIR/{cycle}/consolidate_observations/wind_{xy}.csv
+            WIND_FILE_TEMPLATE = $CYLC_WORKFLOW_WORK_DIR/{cycle}/consolidate_observations/wind_{xy}.csv
             # Offset in hours to cycles to process wind data from.
             WIND_CYCLES = 0, -3, -6
             # The path to the rainfall file.
-            RAINFALL_FILE = $CYLC_SUITE_WORK_DIR/$CYLC_TASK_CYCLE_POINT/get_rainfall/rainfall.csv
+            RAINFALL_FILE = $CYLC_WORKFLOW_WORK_DIR/$CYLC_TASK_CYCLE_POINT/get_rainfall/rainfall.csv
             # Create the html map file in the task's log directory.
             MAP_FILE = "${CYLC_TASK_LOG_ROOT}-map.html"
             # The path to the template file used to generate the html map.
-            MAP_TEMPLATE = "$CYLC_SUITE_RUN_DIR/lib/template/map.html"
+            MAP_TEMPLATE = "$CYLC_WORKFLOW_RUN_DIR/lib/template/map.html"
 
     [[post_process<site>]]
         # Generate a forecast for the location <site> 60 minutes in the future.
         script = post-process $CYLC_TASK_PARAM_site 60
+
+{% include 'etc/python-job.settings' %}
```

### Comparing `metomi-rose-2.0rc3/metomi/rose/etc/tutorial/cylc-forecasting-suite/lib/python/mecator.py` & `metomi-rose-2.1.0/metomi/rose/etc/tutorial/rose-suite-tutorial/lib/python/mercator.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,34 @@
-# Copyright (C) British Crown (Met Office) & Contributors - GNU V3+.
+# -*- coding: utf-8 -*-
+# -----------------------------------------------------------------------------
+# THIS FILE IS PART OF THE CYLC WORKFLOW ENGINE.
+# Copyright (C) NIWA & British Crown (Met Office) & Contributors.
+#
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU General Public License as published by
+# the Free Software Foundation, either version 3 of the License, or
+# (at your option) any later version.
+#
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU General Public License for more details.
+#
+# You should have received a copy of the GNU General Public License
+# along with this program.  If not, see <http://www.gnu.org/licenses/>.
+# -----------------------------------------------------------------------------
 # This is illustrative code developed for tutorial purposes, it is not
 # intended for scientific use and is not guarantied to be accurate or correct.
-# -----------------------------------------------------------------------------
 import math
 
+
 R_0 = 6356752.3
 
 
-def get_offset(bbox, scale=(1.0, 1.0)):
+def get_offset(bbox, scale=(1., 1.)):
     """Define an offset from the origin using the provided bbox.
 
     Args:
         bbox: The coordinates of the domain as a dictionary {'lat1', 'lng1',
             'lat2', 'lng2'}
         scale: The x, y scale factor as returned by get_scale().
 
@@ -24,50 +41,49 @@
 
     Args:
         bbox: The coordinates of the domain as a dictionary {'lat1', 'lng1',
             'lat2', 'lng2'}
         width: The width of the projection.
 
     """
-    scale = width * (180.0 / abs(bbox['lng2'] - bbox['lng1']))
+    scale = width * (180. / abs(bbox['lng2'] - bbox['lng1']))
     return (
         (math.pi * R_0) / scale,
-        (math.pi * R_0 * 2.0) / scale,
-    )
+        (math.pi * R_0 * 2.) / scale)
 
 
-def coord_to_pos(lng, lat, offset=(0.0, 0.0), scale=(1.0, 1.0)):
-    """Convert a lng, lat coord to an x, y position in a mecator projection.
+def coord_to_pos(lng, lat, offset=(0., 0.), scale=(1., 1.)):
+    """Convert a lng, lat coord to an x, y position in a mercator projection.
 
     proj equivalent:
         $ echo <lng> <lat> | proj +proj=merc
         # Divide by scale.
         # Subtract offset.
 
     """
     lng = math.radians(lng)
     lat = math.radians(lat)
     pos_x = R_0 * lng
-    pos_y = R_0 * math.log(math.tan((math.pi / 4.0) + (lat / 2.0)))
+    pos_y = R_0 * math.log(math.tan((math.pi / 4.) + (lat / 2.)))
     pos_x /= scale[0]
     pos_y /= scale[1]
     pos_x -= offset[0]
     pos_y -= offset[1]
     return pos_x, pos_y
 
 
-def pos_to_coord(pos_x, pos_y, offset=(0.0, 0.0), scale=(1.0, 1.0)):
-    """Convert an x, y coordinate in a mecator projection to a lng, lat coord.
+def pos_to_coord(pos_x, pos_y, offset=(0., 0.), scale=(1., 1.)):
+    """Convert an x, y coordinate in a mercator projection to a lng, lat coord.
 
     proj equivalent:
         # Add offset
         # Multiply by scale.
         $ echo <pos_x> <pos_y> | proj -I +proj=merc
 
     """
     pos_x += offset[0]
     pos_y += offset[1]
     pos_x *= scale[0]
     pos_y *= scale[1]
     lng = pos_x / R_0
-    lat = 2 * math.atan(math.exp(pos_y / R_0)) - (math.pi / 2.0)
+    lat = 2 * math.atan(math.exp(pos_y / R_0)) - (math.pi / 2.)
     return math.degrees(lng), math.degrees(lat)
```

### Comparing `metomi-rose-2.0rc3/metomi/rose/etc/tutorial/cylc-forecasting-suite/lib/python/util.py` & `metomi-rose-2.1.0/metomi/rose/etc/tutorial/forecast-script/util.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,35 @@
-# Copyright (C) British Crown (Met Office) & Contributors - GNU V3+.
+# -*- coding: utf-8 -*-
+# -----------------------------------------------------------------------------
+# THIS FILE IS PART OF THE CYLC WORKFLOW ENGINE.
+# Copyright (C) NIWA & British Crown (Met Office) & Contributors.
+#
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU General Public License as published by
+# the Free Software Foundation, either version 3 of the License, or
+# (at your option) any later version.
+#
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU General Public License for more details.
+#
+# You should have received a copy of the GNU General Public License
+# along with this program.  If not, see <http://www.gnu.org/licenses/>.
+# -----------------------------------------------------------------------------
 # This is illustrative code developed for tutorial purposes, it is not
 # intended for scientific use and is not guarantied to be accurate or correct.
-# -----------------------------------------------------------------------------
 from copy import copy
+from contextlib import suppress
 import math
+import jinja2
 import sys
 
-import jinja2
 
-R_0 = 6371.0  # Radius of the Earth (km).
+R_0 = 6371.  # Radius of the Earth (km).
 
 
 def frange(start, stop, step):
     """Implementation of python's xrange which works with floats."""
     while start < stop:
         yield start
         start += step
@@ -48,27 +65,26 @@
 
     Args:
         filename (str): The path of the csv file to write to.
         field (function): A function of the form f(x, y) -> z.
         x_range (list): List of the x coordinates of the extrapolated grid.
             These are the extrapolation coordinates, the length of this list
             defines the size of the grid.
-        x_range (list): List of the y coordinates of the extrapolated grid.
+        y_range (list): List of the y coordinates of the extrapolated grid.
             These are the extrapolation coordinates, the length of this list
             defines the size of the grid.
 
     """
     with open(filename, 'w+') as csv_file:
         for itt_y in y_range:
-            csv_file.write(
-                ', '.join('%.2f' % field(x, itt_y) for x in x_range) + '\n'
-            )
+            csv_file.write(', '.join('%.2f' % field(x, itt_y) for
+                                     x in x_range) + '\n')
 
 
-def generate_matrix(dim_x, dim_y, value=0.0):
+def generate_matrix(dim_x, dim_y, value=0.):
     """Generates a 2D list with the desired dimensions.
 
     Args:
         dim_x (int): The x-dimension of the matrix.
         dim_y (int): The y-dimension of the matrix.
         value: The default value for each cell of the matrix.
 
@@ -99,23 +115,20 @@
     (lng_1, lat_1) = coordinate_1
     (lng_2, lat_2) = coordinate_2
     lng_1 = math.radians(lng_1)
     lat_1 = math.radians(lat_1)
     lng_2 = math.radians(lng_2)
     lat_2 = math.radians(lat_2)
     return (
-        2
-        * R_0
-        * math.asin(
+        2 * R_0 * math.asin(
             math.sqrt(
-                (math.sin((lat_2 - lat_1) / 2.0) ** 2)
-                + (
-                    math.cos(lat_1)
-                    * math.cos(lat_2)
-                    * (math.sin((lng_2 - lng_1) / 2.0) ** 2)
+                (math.sin((lat_2 - lat_1) / 2.) ** 2) + (
+                    math.cos(lat_1) *
+                    math.cos(lat_2) *
+                    (math.sin((lng_2 - lng_1) / 2.) ** 2)
                 )
             )
         )
     )
 
 
 def interpolate_grid(points, dim_x, dim_y, d_x, d_y, spline_order=0):
@@ -132,61 +145,57 @@
             interpolation (0 = nearset).
 
     Return:
         list - 2D matrix of dimensions dim_x, dim_y containing the interpolated
         data.
 
     """
-
     def spline_0(pos_x, pos_y, z_val):
         """Zeroth order beta spline (i.e. nearest point)."""
         return [(int(round(pos_x)), int(round(pos_y)), z_val)]  # [(x, y, z)]
 
     def spline_1(pos_x, pos_y, z_val):
-        """First order beta spline (weight spread about four nearest ponts)."""
+        """First order beta spline (weight spread about four nearest
+        points)."""
         x_0 = int(math.floor(pos_x))
         y_0 = int(math.floor(pos_y))
         x_1 = x_0 + 1
         y_1 = y_0 + 1
         return [
             # (x, y, z), ...
             (x_0, y_0, (x_0 + d_x - pos_x) * (y_0 + d_y - pos_y) * z_val),
             (x_1, y_0, (pos_x - x_0) * (y_0 + d_y - pos_y) * z_val),
             (x_0, y_1, (x_0 + d_x - pos_x) * (pos_y - y_0) * z_val),
-            (x_1, y_1, (pos_x - x_0) * (pos_y - y_0) * z_val),
+            (x_1, y_1, (pos_x - x_0) * (pos_y - y_0) * z_val)
         ]
 
     if spline_order == 0:
         spline = spline_0
-    elif spline_order == 1:
+    elif spline_order == 1:  # noqa: SIM106 (case type matching)
         spline = spline_1
     else:
-        raise ValueError(
-            'Invalid spline order "%d" must be in (0, 1).' % spline_order
-        )
+        raise ValueError('Invalid spline order "%d" must be in (0, 1).' %
+                         spline_order)
 
-    grid = generate_matrix(dim_x, dim_y, 0.0)
+    grid = generate_matrix(dim_x, dim_y, 0.)
 
     for x_val, y_val, z_val in points:
         x_coord = x_val / d_x
         y_coord = y_val / d_y
         for grid_x, grid_y, grid_z in spline(x_coord, y_coord, z_val):
-            try:
+            with suppress(IndexError):
                 grid[grid_y][grid_x] += grid_z
-            except IndexError:
-                # Grid point out of bounds => skip.
-                pass
+                # skip grid point out of bounds
 
     return grid
 
 
 def plot_vector_grid(filename, x_grid, y_grid):
     try:
         import matplotlib
-
         matplotlib.use('Agg')
         import matplotlib.pyplot as plt
     except ImportError:
         print('Plotting disabled', file=sys.stderr)
         return
 
     fig = plt.figure()
@@ -195,34 +204,31 @@
     z_coords = []
     for itt_x in range(len(x_grid[0])):
         for itt_y in range(len(x_grid)):
             x_coords.append(itt_x)
             y_coords.append(itt_y)
             z_coords.append((
                 x_grid[itt_y][itt_x],
-                y_grid[itt_y][itt_x],
+                y_grid[itt_y][itt_x]
             ))
 
-    plt.quiver(
-        x_coords,
-        y_coords,
-        [x[0] for x in z_coords],
-        [y[1] for y in z_coords],
-    )
+    plt.quiver(x_coords,
+               y_coords,
+               [x[0] for x in z_coords],
+               [y[1] for y in z_coords])
     fig.savefig(filename)
 
 
 def get_grid_coordinates(lng, lat, domain, resolution):
     """Return the grid coordinates for a lat, long coordinate pair."""
     # NOTE: Grid coordinates run from *top* left to bottom right.
     length_y = int(abs(domain['lat2'] - domain['lat1']) // resolution)
     return (
         int((abs(lng - domain['lng1'])) // resolution),
-        length_y - int((abs(lat - domain['lat1'])) // resolution),
-    )
+        length_y - int((abs(lat - domain['lat1'])) // resolution))
 
 
 class SurfaceFitter:
     """A 2D interpolation for random points.
 
     A standin for scipy.interpolate.interp2d
 
@@ -239,19 +245,19 @@
 
     """
 
     def __init__(self, x_points, y_points, z_points, kind='linear'):
         self.points = list(zip(x_points, y_points, z_points))
 
         if kind == 'linear':
-            self.power = 1.0
+            self.power = 1.
         elif kind == 'quadratic':
-            self.power = 2.0
-        elif kind == 'cubic':
-            self.power = 3.0
+            self.power = 2.
+        elif kind == 'cubic':  # noqa: SIM106 (case type matching)
+            self.power = 3.
         else:
             raise ValueError('"%s" is not a valid interpolation method' % kind)
 
     def __call__(self, grid_x, grid_y):
         sum_value = 0.0
         sum_weight = 0.0
         z_val = None
@@ -260,15 +266,15 @@
             d_y = grid_y - y_point
             if d_x == 0 and d_y == 0:
                 # This point is exactly at the grid location we are
                 # interpolating for, return this value.
                 z_val = z_point
                 break
             else:
-                weight = 1.0 / ((math.sqrt(d_x ** 2 + d_y ** 2)) ** self.power)
+                weight = 1. / ((math.sqrt(d_x ** 2 + d_y ** 2)) ** self.power)
                 sum_weight += weight
                 sum_value += weight * z_point
 
         if z_val is None:
             z_val = sum_value / sum_weight
 
         return z_val
@@ -276,24 +282,22 @@
 
 def parse_domain(domain):
     bbox = list(map(float, domain.split(',')))
     return {
         'lng1': bbox[0],
         'lat1': bbox[1],
         'lng2': bbox[2],
-        'lat2': bbox[3],
+        'lat2': bbox[3]
     }
 
 
 def generate_html_map(filename, template_file, data, domain, resolution):
-    with open(template_file, 'r') as template:
+    with open(template_file, 'r') as template:  # noqa: SIM117
         with open(filename, 'w+') as html_file:
-            html_file.write(
-                jinja2.Template(template.read()).render(
-                    resolution=resolution,
-                    lng1=domain['lng1'],
-                    lng2=domain['lng2'],
-                    lat1=domain['lat1'],
-                    lat2=domain['lat2'],
-                    data=data,
-                )
-            )
+            html_file.write(jinja2.Template(template.read()).render(
+                resolution=resolution,
+                lng1=domain['lng1'],
+                lng2=domain['lng2'],
+                lat1=domain['lat1'],
+                lat2=domain['lat2'],
+                data=data
+            ))
```

### Comparing `metomi-rose-2.0rc3/metomi/rose/etc/tutorial/cylc-forecasting-suite/lib/template/map.html` & `metomi-rose-2.1.0/metomi/rose/etc/tutorial/map-template/map-template.html`

 * *Files 10% similar despite different names*

```diff
@@ -1,82 +1,93 @@
 <html>
-  <head>
-    <link rel="stylesheet"
-          href="https://unpkg.com/leaflet@1.2.0/dist/leaflet.css" />
+
+<head>
+    <link rel="stylesheet" href="https://unpkg.com/leaflet@1.2.0/dist/leaflet.css" />
     <script src="https://unpkg.com/leaflet@1.2.0/dist/leaflet.js"></script>
-  </head>
-  <body>
+</head>
+
+<body>
     <div id="map" style="width:100%;height:100%"></div>
 
     <script type="text/javascript">
-      // Define the colours to display for the different rainfall values.
-      // NOTE: Rainfall values range from 0 to 6+.
-      function get_colour(value) {
-          if (value < 0.1)
-              return '#ffffff88';
-          if (value < 0.5)
-              return '#00F7FF';
-          if (value < 1)
-              return '#00AAFF';
-          else if (value < 2)
-              return '#0051FF';
-          else if (value < 3)
-              return '#6600FF';
-          else if (value < 4)
-              return '#AE00FF';
-          else if (value < 5)
-              return '#FF00EA';
-          else
-              return '#FF0055';
-      }
-
-      // Forecast data as dict {'lead_time': [2d data matrix]}.
-      var data = {{ data }};
-
-      // Annotate map with data.
-      var lng;
-      var lat;
-      var rects;
-      var times = [];
-      var layers = [];
-      for (let time in data) {
-          rects = L.layerGroup();
-          for (let pos_y in data[time]) {
-              for (let pos_x in data[time][0]) {
-                  lng = (pos_x * {{ resolution }}) + {{ lng1 }};
-                  lat = {{ lat2 }} - (pos_y * {{ resolution }});
-                  L.rectangle(
-                      [[lat, lng],
-                      [lat + {{ resolution }}, lng + {{ resolution }}]],
-                      {color: get_colour(data[time][pos_y][pos_x]),
-                       weight: 0, fillOpacity: 0.5}).addTo(rects);
-              }
-          }
-          layers.push(rects);
-          times.push(time);
-      }
-
-      // Sort map layers lexicographically.
-      var sorted_times = times.slice(0);  // Copy the times list.
-      var fcsts = {};  // {'lead_time': L.LayerGroup}  Note dicts are ordered.
-      sorted_times.sort();
-      var ind;
-      for (let time of sorted_times) {
-          ind = times.indexOf(time);
-          fcsts[times[ind]] = layers[ind];
-      }
-
-      // Create map.
-      var map = L.map('map', {layers: [fcsts[sorted_times[0]]]});
-
-      // Zoom / center map to fit domain.
-      map.fitBounds([[{{ lat1 }}, {{ lng1 }}], [{{ lat2 }}, {{ lng2 }}]]);
-
-      // Add mapp tiles.
-      map.addLayer(
-          L.tileLayer('http://{s}.tile.openstreetmap.org/{z}/{x}/{y}.png'));
+        // Define the colours to display for the different rainfall values.
+        // NOTE: Rainfall values range from 0 to 6+.
+        function get_colour(value) {
+            if (value < 0.1)
+                return '#ffffff88';
+            if (value < 0.5)
+                return '#00F7FF';
+            if (value < 1)
+                return '#00AAFF';
+            else if (value < 2)
+                return '#0051FF';
+            else if (value < 3)
+                return '#6600FF';
+            else if (value < 4)
+                return '#AE00FF';
+            else if (value < 5)
+                return '#FF00EA';
+            else
+                return '#FF0055';
+        }
+
+        // Forecast data as dict {'lead_time': [2d data matrix]}.
+        var data = {{ data }};
+
+        // Annotate map with data.
+        var lng;
+        var lat;
+        var rects;
+        var times = [];
+        var layers = [];
+        for (let time in data) {
+            rects = L.layerGroup();
+            for (let pos_y in data[time]) {
+                for (let pos_x in data[time][0]) {
+                    lng = (pos_x * {{ resolution }}) + {{ lng1 }};
+                    lat = {{ lat2 }} - (pos_y * {{ resolution }});
+                    L.rectangle(
+                        [
+                            [lat, lng],
+                            [lat + {{ resolution }}, lng + {{ resolution }}]
+                        ], {
+                            color: get_colour(data[time][pos_y][pos_x]),
+                            weight: 0,
+                            fillOpacity: 0.5
+                        }).addTo(rects);
+                }
+            }
+            layers.push(rects);
+            times.push(time);
+        }
+
+        // Sort map layers lexicographically.
+        var sorted_times = times.slice(0); // Copy the times list.
+        var fcsts = {}; // {'lead_time': L.LayerGroup}  Note dicts are ordered.
+        sorted_times.sort();
+        var ind;
+        for (let time of sorted_times) {
+            ind = times.indexOf(time);
+            fcsts[times[ind]] = layers[ind];
+        }
+
+        // Create map.
+        var map = L.map('map', {
+            layers: [fcsts[sorted_times[0]]]
+        });
+
+        // Zoom / center map to fit domain.
+        map.fitBounds([
+            [{{ lat1 }}, {{ lng1 }}],
+            [{{ lat2 }}, {{ lng2 }}]
+        ]);
+
+        // Add map tiles.
+        map.addLayer(
+            L.tileLayer('http://{s}.tile.openstreetmap.org/{z}/{x}/{y}.png'));
 
-      // Add layer selector.
-      L.control.layers(fcsts).addTo(map);
+        // Add layer selector.
+        L.control.layers(fcsts).addTo(map);
     </script>
-  </body>
+</body>
+
 </html>
```

### Comparing `metomi-rose-2.0rc3/metomi/rose/etc/tutorial/failif-warnif/meta/rose-meta.conf` & `metomi-rose-2.1.0/metomi/rose/etc/tutorial/failif-warnif/meta/rose-meta.conf`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rose/etc/tutorial/forecast-script/forecast` & `metomi-rose-2.1.0/metomi/rose/etc/tutorial/metadata-tutorial/bin/forecast`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,28 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 # -----------------------------------------------------------------------------
-# Copyright (C) British Crown (Met Office) & Contributors - GNU V3+.
+# THIS FILE IS PART OF THE CYLC WORKFLOW ENGINE.
+# Copyright (C) NIWA & British Crown (Met Office) & Contributors.
+#
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU General Public License as published by
+# the Free Software Foundation, either version 3 of the License, or
+# (at your option) any later version.
+#
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU General Public License for more details.
+#
+# You should have received a copy of the GNU General Public License
+# along with this program.  If not, see <http://www.gnu.org/licenses/>.
+# -----------------------------------------------------------------------------
 # This is illustrative code developed for tutorial purposes, it is not
 # intended for scientific use and is not guarantied to be accurate or correct.
-# -----------------------------------------------------------------------------
 """
 Usage:
     forecast INTERVAL ITERATIONS
 
 Arguments:
     INTERVAL: The period between forecasts in minutes.
     ITERATIONS: The number of forecasts to produce.
@@ -43,15 +57,15 @@
         wind_file_path (str): Template for the path to a wind data file.
             The template should contain substitutions for `{cycles}`
             (i.e. the cycle point) and `{xy}` (i.e. the value 'x' or 'y').
         wind_cycles (list): List of cycle points to get wind data for
             as strings.
 
     Return:
-            list - A list 2-tuples containing wind field matricies i.e.
+            list - A list 2-tuples containing wind field matrices i.e.
             [(wind_x, wind_y), ...]
 
     """
     wind_fields = []
     for cycle in wind_cycles:
         wind_x = util.read_csv(wind_file_path.format(cycle=cycle, xy='x'))
         wind_y = util.read_csv(wind_file_path.format(cycle=cycle, xy='y'))
@@ -176,16 +190,16 @@
     """
     return Popen(
         ['cylc', 'cyclepoint', '--offset-hours', str(int(offset_hours))],
         stdout=PIPE
     ).communicate()[0].strip().decode()
 
 
-def main(forecast_interval, forecast_itterations):
-    # Get suite settings.
+def main(forecast_interval, forecast_iterations):
+    # Get workflow settings.
     domain = util.parse_domain(os.environ['DOMAIN'])
     resolution = float(os.environ['RESOLUTION'])
 
     # Get science settings.
     spline_level = int(os.environ.get('SPLINE_LEVEL', 0))
     weighting = list(map(float, os.environ.get('WEIGHTING', '1').split(',')))
 
@@ -208,15 +222,15 @@
 
     # Initiate the forecaster.
     generator = push_rainfall(rainfall, weighted_wind_data, forecast_interval,
                               resolution, spline_level)
 
     # Generate forecasts.
     forecasts = {}
-    for lead_minutes in range(0, forecast_interval * (forecast_itterations + 1),
+    for lead_minutes in range(0, forecast_interval * (forecast_iterations + 1),
                               forecast_interval):
         forecast_name = '+PT%02dH%02dM' % (lead_minutes // 60,
                                            lead_minutes % 60)
         # Generate forecast.
         forecast = next(generator)
         forecasts[forecast_name] = forecast
         # Output forecast data.
```

### Comparing `metomi-rose-2.0rc3/metomi/rose/etc/tutorial/forecast-script/util.py` & `metomi-rose-2.1.0/metomi/rose/etc/tutorial/metadata-tutorial/bin/util.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,35 @@
-# Copyright (C) British Crown (Met Office) & Contributors - GNU V3+.
+# -*- coding: utf-8 -*-
+# -----------------------------------------------------------------------------
+# THIS FILE IS PART OF THE CYLC WORKFLOW ENGINE.
+# Copyright (C) NIWA & British Crown (Met Office) & Contributors.
+#
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU General Public License as published by
+# the Free Software Foundation, either version 3 of the License, or
+# (at your option) any later version.
+#
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU General Public License for more details.
+#
+# You should have received a copy of the GNU General Public License
+# along with this program.  If not, see <http://www.gnu.org/licenses/>.
+# -----------------------------------------------------------------------------
 # This is illustrative code developed for tutorial purposes, it is not
 # intended for scientific use and is not guarantied to be accurate or correct.
-# -----------------------------------------------------------------------------
 from copy import copy
+from contextlib import suppress
 import math
+import jinja2
 import sys
 
-import jinja2
 
-R_0 = 6371.0  # Radius of the Earth (km).
+R_0 = 6371.  # Radius of the Earth (km).
 
 
 def frange(start, stop, step):
     """Implementation of python's xrange which works with floats."""
     while start < stop:
         yield start
         start += step
@@ -48,27 +65,26 @@
 
     Args:
         filename (str): The path of the csv file to write to.
         field (function): A function of the form f(x, y) -> z.
         x_range (list): List of the x coordinates of the extrapolated grid.
             These are the extrapolation coordinates, the length of this list
             defines the size of the grid.
-        x_range (list): List of the y coordinates of the extrapolated grid.
+        y_range (list): List of the y coordinates of the extrapolated grid.
             These are the extrapolation coordinates, the length of this list
             defines the size of the grid.
 
     """
     with open(filename, 'w+') as csv_file:
         for itt_y in y_range:
-            csv_file.write(
-                ', '.join('%.2f' % field(x, itt_y) for x in x_range) + '\n'
-            )
+            csv_file.write(', '.join('%.2f' % field(x, itt_y) for
+                                     x in x_range) + '\n')
 
 
-def generate_matrix(dim_x, dim_y, value=0.0):
+def generate_matrix(dim_x, dim_y, value=0.):
     """Generates a 2D list with the desired dimensions.
 
     Args:
         dim_x (int): The x-dimension of the matrix.
         dim_y (int): The y-dimension of the matrix.
         value: The default value for each cell of the matrix.
 
@@ -99,23 +115,20 @@
     (lng_1, lat_1) = coordinate_1
     (lng_2, lat_2) = coordinate_2
     lng_1 = math.radians(lng_1)
     lat_1 = math.radians(lat_1)
     lng_2 = math.radians(lng_2)
     lat_2 = math.radians(lat_2)
     return (
-        2
-        * R_0
-        * math.asin(
+        2 * R_0 * math.asin(
             math.sqrt(
-                (math.sin((lat_2 - lat_1) / 2.0) ** 2)
-                + (
-                    math.cos(lat_1)
-                    * math.cos(lat_2)
-                    * (math.sin((lng_2 - lng_1) / 2.0) ** 2)
+                (math.sin((lat_2 - lat_1) / 2.) ** 2) + (
+                    math.cos(lat_1) *
+                    math.cos(lat_2) *
+                    (math.sin((lng_2 - lng_1) / 2.) ** 2)
                 )
             )
         )
     )
 
 
 def interpolate_grid(points, dim_x, dim_y, d_x, d_y, spline_order=0):
@@ -132,61 +145,57 @@
             interpolation (0 = nearset).
 
     Return:
         list - 2D matrix of dimensions dim_x, dim_y containing the interpolated
         data.
 
     """
-
     def spline_0(pos_x, pos_y, z_val):
         """Zeroth order beta spline (i.e. nearest point)."""
         return [(int(round(pos_x)), int(round(pos_y)), z_val)]  # [(x, y, z)]
 
     def spline_1(pos_x, pos_y, z_val):
-        """First order beta spline (weight spread about four nearest ponts)."""
+        """First order beta spline (weight spread about four nearest
+        points)."""
         x_0 = int(math.floor(pos_x))
         y_0 = int(math.floor(pos_y))
         x_1 = x_0 + 1
         y_1 = y_0 + 1
         return [
             # (x, y, z), ...
             (x_0, y_0, (x_0 + d_x - pos_x) * (y_0 + d_y - pos_y) * z_val),
             (x_1, y_0, (pos_x - x_0) * (y_0 + d_y - pos_y) * z_val),
             (x_0, y_1, (x_0 + d_x - pos_x) * (pos_y - y_0) * z_val),
-            (x_1, y_1, (pos_x - x_0) * (pos_y - y_0) * z_val),
+            (x_1, y_1, (pos_x - x_0) * (pos_y - y_0) * z_val)
         ]
 
     if spline_order == 0:
         spline = spline_0
-    elif spline_order == 1:
+    elif spline_order == 1:  # noqa: SIM106 (case type matching)
         spline = spline_1
     else:
-        raise ValueError(
-            'Invalid spline order "%d" must be in (0, 1).' % spline_order
-        )
+        raise ValueError('Invalid spline order "%d" must be in (0, 1).' %
+                         spline_order)
 
-    grid = generate_matrix(dim_x, dim_y, 0.0)
+    grid = generate_matrix(dim_x, dim_y, 0.)
 
     for x_val, y_val, z_val in points:
         x_coord = x_val / d_x
         y_coord = y_val / d_y
         for grid_x, grid_y, grid_z in spline(x_coord, y_coord, z_val):
-            try:
+            with suppress(IndexError):
                 grid[grid_y][grid_x] += grid_z
-            except IndexError:
-                # Grid point out of bounds => skip.
-                pass
+                # skip grid point out of bounds
 
     return grid
 
 
 def plot_vector_grid(filename, x_grid, y_grid):
     try:
         import matplotlib
-
         matplotlib.use('Agg')
         import matplotlib.pyplot as plt
     except ImportError:
         print('Plotting disabled', file=sys.stderr)
         return
 
     fig = plt.figure()
@@ -195,34 +204,31 @@
     z_coords = []
     for itt_x in range(len(x_grid[0])):
         for itt_y in range(len(x_grid)):
             x_coords.append(itt_x)
             y_coords.append(itt_y)
             z_coords.append((
                 x_grid[itt_y][itt_x],
-                y_grid[itt_y][itt_x],
+                y_grid[itt_y][itt_x]
             ))
 
-    plt.quiver(
-        x_coords,
-        y_coords,
-        [x[0] for x in z_coords],
-        [y[1] for y in z_coords],
-    )
+    plt.quiver(x_coords,
+               y_coords,
+               [x[0] for x in z_coords],
+               [y[1] for y in z_coords])
     fig.savefig(filename)
 
 
 def get_grid_coordinates(lng, lat, domain, resolution):
     """Return the grid coordinates for a lat, long coordinate pair."""
     # NOTE: Grid coordinates run from *top* left to bottom right.
     length_y = int(abs(domain['lat2'] - domain['lat1']) // resolution)
     return (
         int((abs(lng - domain['lng1'])) // resolution),
-        length_y - int((abs(lat - domain['lat1'])) // resolution),
-    )
+        length_y - int((abs(lat - domain['lat1'])) // resolution))
 
 
 class SurfaceFitter:
     """A 2D interpolation for random points.
 
     A standin for scipy.interpolate.interp2d
 
@@ -239,19 +245,19 @@
 
     """
 
     def __init__(self, x_points, y_points, z_points, kind='linear'):
         self.points = list(zip(x_points, y_points, z_points))
 
         if kind == 'linear':
-            self.power = 1.0
+            self.power = 1.
         elif kind == 'quadratic':
-            self.power = 2.0
-        elif kind == 'cubic':
-            self.power = 3.0
+            self.power = 2.
+        elif kind == 'cubic':  # noqa: SIM106 (case type matching)
+            self.power = 3.
         else:
             raise ValueError('"%s" is not a valid interpolation method' % kind)
 
     def __call__(self, grid_x, grid_y):
         sum_value = 0.0
         sum_weight = 0.0
         z_val = None
@@ -260,15 +266,15 @@
             d_y = grid_y - y_point
             if d_x == 0 and d_y == 0:
                 # This point is exactly at the grid location we are
                 # interpolating for, return this value.
                 z_val = z_point
                 break
             else:
-                weight = 1.0 / ((math.sqrt(d_x ** 2 + d_y ** 2)) ** self.power)
+                weight = 1. / ((math.sqrt(d_x ** 2 + d_y ** 2)) ** self.power)
                 sum_weight += weight
                 sum_value += weight * z_point
 
         if z_val is None:
             z_val = sum_value / sum_weight
 
         return z_val
@@ -276,24 +282,22 @@
 
 def parse_domain(domain):
     bbox = list(map(float, domain.split(',')))
     return {
         'lng1': bbox[0],
         'lat1': bbox[1],
         'lng2': bbox[2],
-        'lat2': bbox[3],
+        'lat2': bbox[3]
     }
 
 
 def generate_html_map(filename, template_file, data, domain, resolution):
-    with open(template_file, 'r') as template:
+    with open(template_file, 'r') as template:  # noqa: SIM117
         with open(filename, 'w+') as html_file:
-            html_file.write(
-                jinja2.Template(template.read()).render(
-                    resolution=resolution,
-                    lng1=domain['lng1'],
-                    lng2=domain['lng2'],
-                    lat1=domain['lat1'],
-                    lat2=domain['lat2'],
-                    data=data,
-                )
-            )
+            html_file.write(jinja2.Template(template.read()).render(
+                resolution=resolution,
+                lng1=domain['lng1'],
+                lng2=domain['lng2'],
+                lat1=domain['lat1'],
+                lat2=domain['lat2'],
+                data=data
+            ))
```

### Comparing `metomi-rose-2.0rc3/metomi/rose/etc/tutorial/map-template/map-template.html` & `metomi-rose-2.1.0/metomi/rose/etc/tutorial/metadata-tutorial/file/map-template.html`

 * *Files 10% similar despite different names*

```diff
@@ -1,82 +1,93 @@
 <html>
-  <head>
-    <link rel="stylesheet"
-          href="https://unpkg.com/leaflet@1.2.0/dist/leaflet.css" />
+
+<head>
+    <link rel="stylesheet" href="https://unpkg.com/leaflet@1.2.0/dist/leaflet.css" />
     <script src="https://unpkg.com/leaflet@1.2.0/dist/leaflet.js"></script>
-  </head>
-  <body>
+</head>
+
+<body>
     <div id="map" style="width:100%;height:100%"></div>
 
     <script type="text/javascript">
-      // Define the colours to display for the different rainfall values.
-      // NOTE: Rainfall values range from 0 to 6+.
-      function get_colour(value) {
-          if (value < 0.1)
-              return '#ffffff88';
-          if (value < 0.5)
-              return '#00F7FF';
-          if (value < 1)
-              return '#00AAFF';
-          else if (value < 2)
-              return '#0051FF';
-          else if (value < 3)
-              return '#6600FF';
-          else if (value < 4)
-              return '#AE00FF';
-          else if (value < 5)
-              return '#FF00EA';
-          else
-              return '#FF0055';
-      }
-
-      // Forecast data as dict {'lead_time': [2d data matrix]}.
-      var data = {{ data }};
-
-      // Annotate map with data.
-      var lng;
-      var lat;
-      var rects;
-      var times = [];
-      var layers = [];
-      for (let time in data) {
-          rects = L.layerGroup();
-          for (let pos_y in data[time]) {
-              for (let pos_x in data[time][0]) {
-                  lng = (pos_x * {{ resolution }}) + {{ lng1 }};
-                  lat = {{ lat2 }} - (pos_y * {{ resolution }});
-                  L.rectangle(
-                      [[lat, lng],
-                      [lat + {{ resolution }}, lng + {{ resolution }}]],
-                      {color: get_colour(data[time][pos_y][pos_x]),
-                       weight: 0, fillOpacity: 0.5}).addTo(rects);
-              }
-          }
-          layers.push(rects);
-          times.push(time);
-      }
-
-      // Sort map layers lexicographically.
-      var sorted_times = times.slice(0);  // Copy the times list.
-      var fcsts = {};  // {'lead_time': L.LayerGroup}  Note dicts are ordered.
-      sorted_times.sort();
-      var ind;
-      for (let time of sorted_times) {
-          ind = times.indexOf(time);
-          fcsts[times[ind]] = layers[ind];
-      }
-
-      // Create map.
-      var map = L.map('map', {layers: [fcsts[sorted_times[0]]]});
-
-      // Zoom / center map to fit domain.
-      map.fitBounds([[{{ lat1 }}, {{ lng1 }}], [{{ lat2 }}, {{ lng2 }}]]);
-
-      // Add mapp tiles.
-      map.addLayer(
-          L.tileLayer('http://{s}.tile.openstreetmap.org/{z}/{x}/{y}.png'));
+        // Define the colours to display for the different rainfall values.
+        // NOTE: Rainfall values range from 0 to 6+.
+        function get_colour(value) {
+            if (value < 0.1)
+                return '#ffffff88';
+            if (value < 0.5)
+                return '#00F7FF';
+            if (value < 1)
+                return '#00AAFF';
+            else if (value < 2)
+                return '#0051FF';
+            else if (value < 3)
+                return '#6600FF';
+            else if (value < 4)
+                return '#AE00FF';
+            else if (value < 5)
+                return '#FF00EA';
+            else
+                return '#FF0055';
+        }
+
+        // Forecast data as dict {'lead_time': [2d data matrix]}.
+        var data = {{ data }};
+
+        // Annotate map with data.
+        var lng;
+        var lat;
+        var rects;
+        var times = [];
+        var layers = [];
+        for (let time in data) {
+            rects = L.layerGroup();
+            for (let pos_y in data[time]) {
+                for (let pos_x in data[time][0]) {
+                    lng = (pos_x * {{ resolution }}) + {{ lng1 }};
+                    lat = {{ lat2 }} - (pos_y * {{ resolution }});
+                    L.rectangle(
+                        [
+                            [lat, lng],
+                            [lat + {{ resolution }}, lng + {{ resolution }}]
+                        ], {
+                            color: get_colour(data[time][pos_y][pos_x]),
+                            weight: 0,
+                            fillOpacity: 0.5
+                        }).addTo(rects);
+                }
+            }
+            layers.push(rects);
+            times.push(time);
+        }
+
+        // Sort map layers lexicographically.
+        var sorted_times = times.slice(0); // Copy the times list.
+        var fcsts = {}; // {'lead_time': L.LayerGroup}  Note dicts are ordered.
+        sorted_times.sort();
+        var ind;
+        for (let time of sorted_times) {
+            ind = times.indexOf(time);
+            fcsts[times[ind]] = layers[ind];
+        }
+
+        // Create map.
+        var map = L.map('map', {
+            layers: [fcsts[sorted_times[0]]]
+        });
+
+        // Zoom / center map to fit domain.
+        map.fitBounds([
+            [{{ lat1 }}, {{ lng1 }}],
+            [{{ lat2 }}, {{ lng2 }}]
+        ]);
+
+        // Add map tiles.
+        map.addLayer(
+            L.tileLayer('http://{s}.tile.openstreetmap.org/{z}/{x}/{y}.png'));
 
-      // Add layer selector.
-      L.control.layers(fcsts).addTo(map);
+        // Add layer selector.
+        L.control.layers(fcsts).addTo(map);
     </script>
-  </body>
+</body>
+
 </html>
```

### Comparing `metomi-rose-2.0rc3/metomi/rose/etc/tutorial/metadata-tutorial/bin/forecast` & `metomi-rose-2.1.0/metomi/rose/etc/tutorial/rose-suite-tutorial/app/forecast/bin/forecast`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,28 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 # -----------------------------------------------------------------------------
-# Copyright (C) British Crown (Met Office) & Contributors - GNU V3+.
+# THIS FILE IS PART OF THE CYLC WORKFLOW ENGINE.
+# Copyright (C) NIWA & British Crown (Met Office) & Contributors.
+#
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU General Public License as published by
+# the Free Software Foundation, either version 3 of the License, or
+# (at your option) any later version.
+#
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU General Public License for more details.
+#
+# You should have received a copy of the GNU General Public License
+# along with this program.  If not, see <http://www.gnu.org/licenses/>.
+# -----------------------------------------------------------------------------
 # This is illustrative code developed for tutorial purposes, it is not
 # intended for scientific use and is not guarantied to be accurate or correct.
-# -----------------------------------------------------------------------------
 """
 Usage:
     forecast INTERVAL ITERATIONS
 
 Arguments:
     INTERVAL: The period between forecasts in minutes.
     ITERATIONS: The number of forecasts to produce.
@@ -43,15 +57,15 @@
         wind_file_path (str): Template for the path to a wind data file.
             The template should contain substitutions for `{cycles}`
             (i.e. the cycle point) and `{xy}` (i.e. the value 'x' or 'y').
         wind_cycles (list): List of cycle points to get wind data for
             as strings.
 
     Return:
-            list - A list 2-tuples containing wind field matricies i.e.
+            list - A list 2-tuples containing wind field matrices i.e.
             [(wind_x, wind_y), ...]
 
     """
     wind_fields = []
     for cycle in wind_cycles:
         wind_x = util.read_csv(wind_file_path.format(cycle=cycle, xy='x'))
         wind_y = util.read_csv(wind_file_path.format(cycle=cycle, xy='y'))
@@ -176,16 +190,16 @@
     """
     return Popen(
         ['cylc', 'cyclepoint', '--offset-hours', str(int(offset_hours))],
         stdout=PIPE
     ).communicate()[0].strip().decode()
 
 
-def main(forecast_interval, forecast_itterations):
-    # Get suite settings.
+def main(forecast_interval, forecast_iterations):
+    # Get workflow settings.
     domain = util.parse_domain(os.environ['DOMAIN'])
     resolution = float(os.environ['RESOLUTION'])
 
     # Get science settings.
     spline_level = int(os.environ.get('SPLINE_LEVEL', 0))
     weighting = list(map(float, os.environ.get('WEIGHTING', '1').split(',')))
 
@@ -208,15 +222,15 @@
 
     # Initiate the forecaster.
     generator = push_rainfall(rainfall, weighted_wind_data, forecast_interval,
                               resolution, spline_level)
 
     # Generate forecasts.
     forecasts = {}
-    for lead_minutes in range(0, forecast_interval * (forecast_itterations + 1),
+    for lead_minutes in range(0, forecast_interval * (forecast_iterations + 1),
                               forecast_interval):
         forecast_name = '+PT%02dH%02dM' % (lead_minutes // 60,
                                            lead_minutes % 60)
         # Generate forecast.
         forecast = next(generator)
         forecasts[forecast_name] = forecast
         # Output forecast data.
```

### Comparing `metomi-rose-2.0rc3/metomi/rose/etc/tutorial/metadata-tutorial/bin/util.py` & `metomi-rose-2.1.0/metomi/rose/etc/tutorial/rose-suite-tutorial/app/forecast/bin/util.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,35 @@
-# Copyright (C) British Crown (Met Office) & Contributors - GNU V3+.
+# -*- coding: utf-8 -*-
+# -----------------------------------------------------------------------------
+# THIS FILE IS PART OF THE CYLC WORKFLOW ENGINE.
+# Copyright (C) NIWA & British Crown (Met Office) & Contributors.
+#
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU General Public License as published by
+# the Free Software Foundation, either version 3 of the License, or
+# (at your option) any later version.
+#
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU General Public License for more details.
+#
+# You should have received a copy of the GNU General Public License
+# along with this program.  If not, see <http://www.gnu.org/licenses/>.
+# -----------------------------------------------------------------------------
 # This is illustrative code developed for tutorial purposes, it is not
 # intended for scientific use and is not guarantied to be accurate or correct.
-# -----------------------------------------------------------------------------
 from copy import copy
+from contextlib import suppress
 import math
+import jinja2
 import sys
 
-import jinja2
 
-R_0 = 6371.0  # Radius of the Earth (km).
+R_0 = 6371.  # Radius of the Earth (km).
 
 
 def frange(start, stop, step):
     """Implementation of python's xrange which works with floats."""
     while start < stop:
         yield start
         start += step
@@ -48,27 +65,26 @@
 
     Args:
         filename (str): The path of the csv file to write to.
         field (function): A function of the form f(x, y) -> z.
         x_range (list): List of the x coordinates of the extrapolated grid.
             These are the extrapolation coordinates, the length of this list
             defines the size of the grid.
-        x_range (list): List of the y coordinates of the extrapolated grid.
+        y_range (list): List of the y coordinates of the extrapolated grid.
             These are the extrapolation coordinates, the length of this list
             defines the size of the grid.
 
     """
     with open(filename, 'w+') as csv_file:
         for itt_y in y_range:
-            csv_file.write(
-                ', '.join('%.2f' % field(x, itt_y) for x in x_range) + '\n'
-            )
+            csv_file.write(', '.join('%.2f' % field(x, itt_y) for
+                                     x in x_range) + '\n')
 
 
-def generate_matrix(dim_x, dim_y, value=0.0):
+def generate_matrix(dim_x, dim_y, value=0.):
     """Generates a 2D list with the desired dimensions.
 
     Args:
         dim_x (int): The x-dimension of the matrix.
         dim_y (int): The y-dimension of the matrix.
         value: The default value for each cell of the matrix.
 
@@ -99,23 +115,20 @@
     (lng_1, lat_1) = coordinate_1
     (lng_2, lat_2) = coordinate_2
     lng_1 = math.radians(lng_1)
     lat_1 = math.radians(lat_1)
     lng_2 = math.radians(lng_2)
     lat_2 = math.radians(lat_2)
     return (
-        2
-        * R_0
-        * math.asin(
+        2 * R_0 * math.asin(
             math.sqrt(
-                (math.sin((lat_2 - lat_1) / 2.0) ** 2)
-                + (
-                    math.cos(lat_1)
-                    * math.cos(lat_2)
-                    * (math.sin((lng_2 - lng_1) / 2.0) ** 2)
+                (math.sin((lat_2 - lat_1) / 2.) ** 2) + (
+                    math.cos(lat_1) *
+                    math.cos(lat_2) *
+                    (math.sin((lng_2 - lng_1) / 2.) ** 2)
                 )
             )
         )
     )
 
 
 def interpolate_grid(points, dim_x, dim_y, d_x, d_y, spline_order=0):
@@ -132,61 +145,57 @@
             interpolation (0 = nearset).
 
     Return:
         list - 2D matrix of dimensions dim_x, dim_y containing the interpolated
         data.
 
     """
-
     def spline_0(pos_x, pos_y, z_val):
         """Zeroth order beta spline (i.e. nearest point)."""
         return [(int(round(pos_x)), int(round(pos_y)), z_val)]  # [(x, y, z)]
 
     def spline_1(pos_x, pos_y, z_val):
-        """First order beta spline (weight spread about four nearest ponts)."""
+        """First order beta spline (weight spread about four nearest
+        points)."""
         x_0 = int(math.floor(pos_x))
         y_0 = int(math.floor(pos_y))
         x_1 = x_0 + 1
         y_1 = y_0 + 1
         return [
             # (x, y, z), ...
             (x_0, y_0, (x_0 + d_x - pos_x) * (y_0 + d_y - pos_y) * z_val),
             (x_1, y_0, (pos_x - x_0) * (y_0 + d_y - pos_y) * z_val),
             (x_0, y_1, (x_0 + d_x - pos_x) * (pos_y - y_0) * z_val),
-            (x_1, y_1, (pos_x - x_0) * (pos_y - y_0) * z_val),
+            (x_1, y_1, (pos_x - x_0) * (pos_y - y_0) * z_val)
         ]
 
     if spline_order == 0:
         spline = spline_0
-    elif spline_order == 1:
+    elif spline_order == 1:  # noqa: SIM106 (case type matching)
         spline = spline_1
     else:
-        raise ValueError(
-            'Invalid spline order "%d" must be in (0, 1).' % spline_order
-        )
+        raise ValueError('Invalid spline order "%d" must be in (0, 1).' %
+                         spline_order)
 
-    grid = generate_matrix(dim_x, dim_y, 0.0)
+    grid = generate_matrix(dim_x, dim_y, 0.)
 
     for x_val, y_val, z_val in points:
         x_coord = x_val / d_x
         y_coord = y_val / d_y
         for grid_x, grid_y, grid_z in spline(x_coord, y_coord, z_val):
-            try:
+            with suppress(IndexError):
                 grid[grid_y][grid_x] += grid_z
-            except IndexError:
-                # Grid point out of bounds => skip.
-                pass
+                # skip grid point out of bounds
 
     return grid
 
 
 def plot_vector_grid(filename, x_grid, y_grid):
     try:
         import matplotlib
-
         matplotlib.use('Agg')
         import matplotlib.pyplot as plt
     except ImportError:
         print('Plotting disabled', file=sys.stderr)
         return
 
     fig = plt.figure()
@@ -195,34 +204,31 @@
     z_coords = []
     for itt_x in range(len(x_grid[0])):
         for itt_y in range(len(x_grid)):
             x_coords.append(itt_x)
             y_coords.append(itt_y)
             z_coords.append((
                 x_grid[itt_y][itt_x],
-                y_grid[itt_y][itt_x],
+                y_grid[itt_y][itt_x]
             ))
 
-    plt.quiver(
-        x_coords,
-        y_coords,
-        [x[0] for x in z_coords],
-        [y[1] for y in z_coords],
-    )
+    plt.quiver(x_coords,
+               y_coords,
+               [x[0] for x in z_coords],
+               [y[1] for y in z_coords])
     fig.savefig(filename)
 
 
 def get_grid_coordinates(lng, lat, domain, resolution):
     """Return the grid coordinates for a lat, long coordinate pair."""
     # NOTE: Grid coordinates run from *top* left to bottom right.
     length_y = int(abs(domain['lat2'] - domain['lat1']) // resolution)
     return (
         int((abs(lng - domain['lng1'])) // resolution),
-        length_y - int((abs(lat - domain['lat1'])) // resolution),
-    )
+        length_y - int((abs(lat - domain['lat1'])) // resolution))
 
 
 class SurfaceFitter:
     """A 2D interpolation for random points.
 
     A standin for scipy.interpolate.interp2d
 
@@ -239,19 +245,19 @@
 
     """
 
     def __init__(self, x_points, y_points, z_points, kind='linear'):
         self.points = list(zip(x_points, y_points, z_points))
 
         if kind == 'linear':
-            self.power = 1.0
+            self.power = 1.
         elif kind == 'quadratic':
-            self.power = 2.0
-        elif kind == 'cubic':
-            self.power = 3.0
+            self.power = 2.
+        elif kind == 'cubic':  # noqa: SIM106 (case type matching)
+            self.power = 3.
         else:
             raise ValueError('"%s" is not a valid interpolation method' % kind)
 
     def __call__(self, grid_x, grid_y):
         sum_value = 0.0
         sum_weight = 0.0
         z_val = None
@@ -260,15 +266,15 @@
             d_y = grid_y - y_point
             if d_x == 0 and d_y == 0:
                 # This point is exactly at the grid location we are
                 # interpolating for, return this value.
                 z_val = z_point
                 break
             else:
-                weight = 1.0 / ((math.sqrt(d_x ** 2 + d_y ** 2)) ** self.power)
+                weight = 1. / ((math.sqrt(d_x ** 2 + d_y ** 2)) ** self.power)
                 sum_weight += weight
                 sum_value += weight * z_point
 
         if z_val is None:
             z_val = sum_value / sum_weight
 
         return z_val
@@ -276,24 +282,22 @@
 
 def parse_domain(domain):
     bbox = list(map(float, domain.split(',')))
     return {
         'lng1': bbox[0],
         'lat1': bbox[1],
         'lng2': bbox[2],
-        'lat2': bbox[3],
+        'lat2': bbox[3]
     }
 
 
 def generate_html_map(filename, template_file, data, domain, resolution):
-    with open(template_file, 'r') as template:
+    with open(template_file, 'r') as template:  # noqa: SIM117
         with open(filename, 'w+') as html_file:
-            html_file.write(
-                jinja2.Template(template.read()).render(
-                    resolution=resolution,
-                    lng1=domain['lng1'],
-                    lng2=domain['lng2'],
-                    lat1=domain['lat1'],
-                    lat2=domain['lat2'],
-                    data=data,
-                )
-            )
+            html_file.write(jinja2.Template(template.read()).render(
+                resolution=resolution,
+                lng1=domain['lng1'],
+                lng2=domain['lng2'],
+                lat1=domain['lat1'],
+                lat2=domain['lat2'],
+                data=data
+            ))
```

### Comparing `metomi-rose-2.0rc3/metomi/rose/etc/tutorial/metadata-tutorial/file/map-template.html` & `metomi-rose-2.1.0/metomi/rose/etc/tutorial/rose-suite-tutorial/app/forecast/file/map-template.html`

 * *Files 10% similar despite different names*

```diff
@@ -1,82 +1,93 @@
 <html>
-  <head>
-    <link rel="stylesheet"
-          href="https://unpkg.com/leaflet@1.2.0/dist/leaflet.css" />
+
+<head>
+    <link rel="stylesheet" href="https://unpkg.com/leaflet@1.2.0/dist/leaflet.css" />
     <script src="https://unpkg.com/leaflet@1.2.0/dist/leaflet.js"></script>
-  </head>
-  <body>
+</head>
+
+<body>
     <div id="map" style="width:100%;height:100%"></div>
 
     <script type="text/javascript">
-      // Define the colours to display for the different rainfall values.
-      // NOTE: Rainfall values range from 0 to 6+.
-      function get_colour(value) {
-          if (value < 0.1)
-              return '#ffffff88';
-          if (value < 0.5)
-              return '#00F7FF';
-          if (value < 1)
-              return '#00AAFF';
-          else if (value < 2)
-              return '#0051FF';
-          else if (value < 3)
-              return '#6600FF';
-          else if (value < 4)
-              return '#AE00FF';
-          else if (value < 5)
-              return '#FF00EA';
-          else
-              return '#FF0055';
-      }
-
-      // Forecast data as dict {'lead_time': [2d data matrix]}.
-      var data = {{ data }};
-
-      // Annotate map with data.
-      var lng;
-      var lat;
-      var rects;
-      var times = [];
-      var layers = [];
-      for (let time in data) {
-          rects = L.layerGroup();
-          for (let pos_y in data[time]) {
-              for (let pos_x in data[time][0]) {
-                  lng = (pos_x * {{ resolution }}) + {{ lng1 }};
-                  lat = {{ lat2 }} - (pos_y * {{ resolution }});
-                  L.rectangle(
-                      [[lat, lng],
-                      [lat + {{ resolution }}, lng + {{ resolution }}]],
-                      {color: get_colour(data[time][pos_y][pos_x]),
-                       weight: 0, fillOpacity: 0.5}).addTo(rects);
-              }
-          }
-          layers.push(rects);
-          times.push(time);
-      }
-
-      // Sort map layers lexicographically.
-      var sorted_times = times.slice(0);  // Copy the times list.
-      var fcsts = {};  // {'lead_time': L.LayerGroup}  Note dicts are ordered.
-      sorted_times.sort();
-      var ind;
-      for (let time of sorted_times) {
-          ind = times.indexOf(time);
-          fcsts[times[ind]] = layers[ind];
-      }
-
-      // Create map.
-      var map = L.map('map', {layers: [fcsts[sorted_times[0]]]});
-
-      // Zoom / center map to fit domain.
-      map.fitBounds([[{{ lat1 }}, {{ lng1 }}], [{{ lat2 }}, {{ lng2 }}]]);
-
-      // Add mapp tiles.
-      map.addLayer(
-          L.tileLayer('http://{s}.tile.openstreetmap.org/{z}/{x}/{y}.png'));
+        // Define the colours to display for the different rainfall values.
+        // NOTE: Rainfall values range from 0 to 6+.
+        function get_colour(value) {
+            if (value < 0.1)
+                return '#ffffff88';
+            if (value < 0.5)
+                return '#00F7FF';
+            if (value < 1)
+                return '#00AAFF';
+            else if (value < 2)
+                return '#0051FF';
+            else if (value < 3)
+                return '#6600FF';
+            else if (value < 4)
+                return '#AE00FF';
+            else if (value < 5)
+                return '#FF00EA';
+            else
+                return '#FF0055';
+        }
+
+        // Forecast data as dict {'lead_time': [2d data matrix]}.
+        var data = {{ data }};
+
+        // Annotate map with data.
+        var lng;
+        var lat;
+        var rects;
+        var times = [];
+        var layers = [];
+        for (let time in data) {
+            rects = L.layerGroup();
+            for (let pos_y in data[time]) {
+                for (let pos_x in data[time][0]) {
+                    lng = (pos_x * {{ resolution }}) + {{ lng1 }};
+                    lat = {{ lat2 }} - (pos_y * {{ resolution }});
+                    L.rectangle(
+                        [
+                            [lat, lng],
+                            [lat + {{ resolution }}, lng + {{ resolution }}]
+                        ], {
+                            color: get_colour(data[time][pos_y][pos_x]),
+                            weight: 0,
+                            fillOpacity: 0.5
+                        }).addTo(rects);
+                }
+            }
+            layers.push(rects);
+            times.push(time);
+        }
+
+        // Sort map layers lexicographically.
+        var sorted_times = times.slice(0); // Copy the times list.
+        var fcsts = {}; // {'lead_time': L.LayerGroup}  Note dicts are ordered.
+        sorted_times.sort();
+        var ind;
+        for (let time of sorted_times) {
+            ind = times.indexOf(time);
+            fcsts[times[ind]] = layers[ind];
+        }
+
+        // Create map.
+        var map = L.map('map', {
+            layers: [fcsts[sorted_times[0]]]
+        });
+
+        // Zoom / center map to fit domain.
+        map.fitBounds([
+            [{{ lat1 }}, {{ lng1 }}],
+            [{{ lat2 }}, {{ lng2 }}]
+        ]);
+
+        // Add map tiles.
+        map.addLayer(
+            L.tileLayer('http://{s}.tile.openstreetmap.org/{z}/{x}/{y}.png'));
 
-      // Add layer selector.
-      L.control.layers(fcsts).addTo(map);
+        // Add layer selector.
+        L.control.layers(fcsts).addTo(map);
     </script>
-  </body>
+</body>
+
 </html>
```

### Comparing `metomi-rose-2.0rc3/metomi/rose/etc/tutorial/metadata-tutorial/file/test-data/rainfall.csv` & `metomi-rose-2.1.0/metomi/rose/etc/tutorial/metadata-tutorial/file/test-data/rainfall.csv`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rose/etc/tutorial/metadata-tutorial/file/test-data/wind_20171101T0000Z_x.csv` & `metomi-rose-2.1.0/metomi/rose/etc/tutorial/metadata-tutorial/file/test-data/wind_20171101T0000Z_x.csv`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rose/etc/tutorial/metadata-tutorial/file/test-data/wind_20171101T0000Z_y.csv` & `metomi-rose-2.1.0/metomi/rose/etc/tutorial/metadata-tutorial/file/test-data/wind_20171101T0000Z_y.csv`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rose/etc/tutorial/metadata-tutorial/rose-app.conf` & `metomi-rose-2.1.0/metomi/rose/etc/tutorial/metadata-tutorial/rose-app.conf`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-stem/kgo.txt` & `metomi-rose-2.1.0/metomi/rose/etc/tutorial/rose-stem/kgo.txt`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-stem/rose-stem/flow.cylc` & `metomi-rose-2.1.0/metomi/rose/etc/tutorial/rose-stem/rose-stem/flow.cylc`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-stem/src/spaceship_command.f90` & `metomi-rose-2.1.0/metomi/rose/etc/tutorial/rose-stem/src/spaceship_command.f90`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-suite-tutorial/app/forecast/bin/forecast` & `metomi-rose-2.1.0/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/app/forecast/bin/forecast`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,28 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 # -----------------------------------------------------------------------------
-# Copyright (C) British Crown (Met Office) & Contributors - GNU V3+.
+# THIS FILE IS PART OF THE CYLC WORKFLOW ENGINE.
+# Copyright (C) NIWA & British Crown (Met Office) & Contributors.
+#
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU General Public License as published by
+# the Free Software Foundation, either version 3 of the License, or
+# (at your option) any later version.
+#
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU General Public License for more details.
+#
+# You should have received a copy of the GNU General Public License
+# along with this program.  If not, see <http://www.gnu.org/licenses/>.
+# -----------------------------------------------------------------------------
 # This is illustrative code developed for tutorial purposes, it is not
 # intended for scientific use and is not guarantied to be accurate or correct.
-# -----------------------------------------------------------------------------
 """
 Usage:
     forecast INTERVAL ITERATIONS
 
 Arguments:
     INTERVAL: The period between forecasts in minutes.
     ITERATIONS: The number of forecasts to produce.
@@ -43,15 +57,15 @@
         wind_file_path (str): Template for the path to a wind data file.
             The template should contain substitutions for `{cycles}`
             (i.e. the cycle point) and `{xy}` (i.e. the value 'x' or 'y').
         wind_cycles (list): List of cycle points to get wind data for
             as strings.
 
     Return:
-            list - A list 2-tuples containing wind field matricies i.e.
+            list - A list 2-tuples containing wind field matrices i.e.
             [(wind_x, wind_y), ...]
 
     """
     wind_fields = []
     for cycle in wind_cycles:
         wind_x = util.read_csv(wind_file_path.format(cycle=cycle, xy='x'))
         wind_y = util.read_csv(wind_file_path.format(cycle=cycle, xy='y'))
@@ -176,16 +190,16 @@
     """
     return Popen(
         ['cylc', 'cyclepoint', '--offset-hours', str(int(offset_hours))],
         stdout=PIPE
     ).communicate()[0].strip().decode()
 
 
-def main(forecast_interval, forecast_itterations):
-    # Get suite settings.
+def main(forecast_interval, forecast_iterations):
+    # Get workflow settings.
     domain = util.parse_domain(os.environ['DOMAIN'])
     resolution = float(os.environ['RESOLUTION'])
 
     # Get science settings.
     spline_level = int(os.environ.get('SPLINE_LEVEL', 0))
     weighting = list(map(float, os.environ.get('WEIGHTING', '1').split(',')))
 
@@ -208,15 +222,15 @@
 
     # Initiate the forecaster.
     generator = push_rainfall(rainfall, weighted_wind_data, forecast_interval,
                               resolution, spline_level)
 
     # Generate forecasts.
     forecasts = {}
-    for lead_minutes in range(0, forecast_interval * (forecast_itterations + 1),
+    for lead_minutes in range(0, forecast_interval * (forecast_iterations + 1),
                               forecast_interval):
         forecast_name = '+PT%02dH%02dM' % (lead_minutes // 60,
                                            lead_minutes % 60)
         # Generate forecast.
         forecast = next(generator)
         forecasts[forecast_name] = forecast
         # Output forecast data.
```

### Comparing `metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-suite-tutorial/app/forecast/bin/util.py` & `metomi-rose-2.1.0/metomi/rose/etc/tutorial/rose-suite-tutorial/lib/python/util.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,35 @@
-# Copyright (C) British Crown (Met Office) & Contributors - GNU V3+.
+# -*- coding: utf-8 -*-
+# -----------------------------------------------------------------------------
+# THIS FILE IS PART OF THE CYLC WORKFLOW ENGINE.
+# Copyright (C) NIWA & British Crown (Met Office) & Contributors.
+#
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU General Public License as published by
+# the Free Software Foundation, either version 3 of the License, or
+# (at your option) any later version.
+#
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU General Public License for more details.
+#
+# You should have received a copy of the GNU General Public License
+# along with this program.  If not, see <http://www.gnu.org/licenses/>.
+# -----------------------------------------------------------------------------
 # This is illustrative code developed for tutorial purposes, it is not
 # intended for scientific use and is not guarantied to be accurate or correct.
-# -----------------------------------------------------------------------------
 from copy import copy
+from contextlib import suppress
 import math
+import jinja2
 import sys
 
-import jinja2
 
-R_0 = 6371.0  # Radius of the Earth (km).
+R_0 = 6371.  # Radius of the Earth (km).
 
 
 def frange(start, stop, step):
     """Implementation of python's xrange which works with floats."""
     while start < stop:
         yield start
         start += step
@@ -48,27 +65,26 @@
 
     Args:
         filename (str): The path of the csv file to write to.
         field (function): A function of the form f(x, y) -> z.
         x_range (list): List of the x coordinates of the extrapolated grid.
             These are the extrapolation coordinates, the length of this list
             defines the size of the grid.
-        x_range (list): List of the y coordinates of the extrapolated grid.
+        y_range (list): List of the y coordinates of the extrapolated grid.
             These are the extrapolation coordinates, the length of this list
             defines the size of the grid.
 
     """
     with open(filename, 'w+') as csv_file:
         for itt_y in y_range:
-            csv_file.write(
-                ', '.join('%.2f' % field(x, itt_y) for x in x_range) + '\n'
-            )
+            csv_file.write(', '.join('%.2f' % field(x, itt_y) for
+                                     x in x_range) + '\n')
 
 
-def generate_matrix(dim_x, dim_y, value=0.0):
+def generate_matrix(dim_x, dim_y, value=0.):
     """Generates a 2D list with the desired dimensions.
 
     Args:
         dim_x (int): The x-dimension of the matrix.
         dim_y (int): The y-dimension of the matrix.
         value: The default value for each cell of the matrix.
 
@@ -99,23 +115,20 @@
     (lng_1, lat_1) = coordinate_1
     (lng_2, lat_2) = coordinate_2
     lng_1 = math.radians(lng_1)
     lat_1 = math.radians(lat_1)
     lng_2 = math.radians(lng_2)
     lat_2 = math.radians(lat_2)
     return (
-        2
-        * R_0
-        * math.asin(
+        2 * R_0 * math.asin(
             math.sqrt(
-                (math.sin((lat_2 - lat_1) / 2.0) ** 2)
-                + (
-                    math.cos(lat_1)
-                    * math.cos(lat_2)
-                    * (math.sin((lng_2 - lng_1) / 2.0) ** 2)
+                (math.sin((lat_2 - lat_1) / 2.) ** 2) + (
+                    math.cos(lat_1) *
+                    math.cos(lat_2) *
+                    (math.sin((lng_2 - lng_1) / 2.) ** 2)
                 )
             )
         )
     )
 
 
 def interpolate_grid(points, dim_x, dim_y, d_x, d_y, spline_order=0):
@@ -132,61 +145,57 @@
             interpolation (0 = nearset).
 
     Return:
         list - 2D matrix of dimensions dim_x, dim_y containing the interpolated
         data.
 
     """
-
     def spline_0(pos_x, pos_y, z_val):
         """Zeroth order beta spline (i.e. nearest point)."""
         return [(int(round(pos_x)), int(round(pos_y)), z_val)]  # [(x, y, z)]
 
     def spline_1(pos_x, pos_y, z_val):
-        """First order beta spline (weight spread about four nearest ponts)."""
+        """First order beta spline (weight spread about four nearest
+        points)."""
         x_0 = int(math.floor(pos_x))
         y_0 = int(math.floor(pos_y))
         x_1 = x_0 + 1
         y_1 = y_0 + 1
         return [
             # (x, y, z), ...
             (x_0, y_0, (x_0 + d_x - pos_x) * (y_0 + d_y - pos_y) * z_val),
             (x_1, y_0, (pos_x - x_0) * (y_0 + d_y - pos_y) * z_val),
             (x_0, y_1, (x_0 + d_x - pos_x) * (pos_y - y_0) * z_val),
-            (x_1, y_1, (pos_x - x_0) * (pos_y - y_0) * z_val),
+            (x_1, y_1, (pos_x - x_0) * (pos_y - y_0) * z_val)
         ]
 
     if spline_order == 0:
         spline = spline_0
-    elif spline_order == 1:
+    elif spline_order == 1:  # noqa: SIM106 (case type matching)
         spline = spline_1
     else:
-        raise ValueError(
-            'Invalid spline order "%d" must be in (0, 1).' % spline_order
-        )
+        raise ValueError('Invalid spline order "%d" must be in (0, 1).' %
+                         spline_order)
 
-    grid = generate_matrix(dim_x, dim_y, 0.0)
+    grid = generate_matrix(dim_x, dim_y, 0.)
 
     for x_val, y_val, z_val in points:
         x_coord = x_val / d_x
         y_coord = y_val / d_y
         for grid_x, grid_y, grid_z in spline(x_coord, y_coord, z_val):
-            try:
+            with suppress(IndexError):
                 grid[grid_y][grid_x] += grid_z
-            except IndexError:
-                # Grid point out of bounds => skip.
-                pass
+                # skip grid point out of bounds
 
     return grid
 
 
 def plot_vector_grid(filename, x_grid, y_grid):
     try:
         import matplotlib
-
         matplotlib.use('Agg')
         import matplotlib.pyplot as plt
     except ImportError:
         print('Plotting disabled', file=sys.stderr)
         return
 
     fig = plt.figure()
@@ -195,34 +204,31 @@
     z_coords = []
     for itt_x in range(len(x_grid[0])):
         for itt_y in range(len(x_grid)):
             x_coords.append(itt_x)
             y_coords.append(itt_y)
             z_coords.append((
                 x_grid[itt_y][itt_x],
-                y_grid[itt_y][itt_x],
+                y_grid[itt_y][itt_x]
             ))
 
-    plt.quiver(
-        x_coords,
-        y_coords,
-        [x[0] for x in z_coords],
-        [y[1] for y in z_coords],
-    )
+    plt.quiver(x_coords,
+               y_coords,
+               [x[0] for x in z_coords],
+               [y[1] for y in z_coords])
     fig.savefig(filename)
 
 
 def get_grid_coordinates(lng, lat, domain, resolution):
     """Return the grid coordinates for a lat, long coordinate pair."""
     # NOTE: Grid coordinates run from *top* left to bottom right.
     length_y = int(abs(domain['lat2'] - domain['lat1']) // resolution)
     return (
         int((abs(lng - domain['lng1'])) // resolution),
-        length_y - int((abs(lat - domain['lat1'])) // resolution),
-    )
+        length_y - int((abs(lat - domain['lat1'])) // resolution))
 
 
 class SurfaceFitter:
     """A 2D interpolation for random points.
 
     A standin for scipy.interpolate.interp2d
 
@@ -239,19 +245,19 @@
 
     """
 
     def __init__(self, x_points, y_points, z_points, kind='linear'):
         self.points = list(zip(x_points, y_points, z_points))
 
         if kind == 'linear':
-            self.power = 1.0
+            self.power = 1.
         elif kind == 'quadratic':
-            self.power = 2.0
-        elif kind == 'cubic':
-            self.power = 3.0
+            self.power = 2.
+        elif kind == 'cubic':  # noqa: SIM106 (case type matching)
+            self.power = 3.
         else:
             raise ValueError('"%s" is not a valid interpolation method' % kind)
 
     def __call__(self, grid_x, grid_y):
         sum_value = 0.0
         sum_weight = 0.0
         z_val = None
@@ -260,15 +266,15 @@
             d_y = grid_y - y_point
             if d_x == 0 and d_y == 0:
                 # This point is exactly at the grid location we are
                 # interpolating for, return this value.
                 z_val = z_point
                 break
             else:
-                weight = 1.0 / ((math.sqrt(d_x ** 2 + d_y ** 2)) ** self.power)
+                weight = 1. / ((math.sqrt(d_x ** 2 + d_y ** 2)) ** self.power)
                 sum_weight += weight
                 sum_value += weight * z_point
 
         if z_val is None:
             z_val = sum_value / sum_weight
 
         return z_val
@@ -276,24 +282,22 @@
 
 def parse_domain(domain):
     bbox = list(map(float, domain.split(',')))
     return {
         'lng1': bbox[0],
         'lat1': bbox[1],
         'lng2': bbox[2],
-        'lat2': bbox[3],
+        'lat2': bbox[3]
     }
 
 
 def generate_html_map(filename, template_file, data, domain, resolution):
-    with open(template_file, 'r') as template:
+    with open(template_file, 'r') as template:  # noqa: SIM117
         with open(filename, 'w+') as html_file:
-            html_file.write(
-                jinja2.Template(template.read()).render(
-                    resolution=resolution,
-                    lng1=domain['lng1'],
-                    lng2=domain['lng2'],
-                    lat1=domain['lat1'],
-                    lat2=domain['lat2'],
-                    data=data,
-                )
-            )
+            html_file.write(jinja2.Template(template.read()).render(
+                resolution=resolution,
+                lng1=domain['lng1'],
+                lng2=domain['lng2'],
+                lat1=domain['lat1'],
+                lat2=domain['lat2'],
+                data=data
+            ))
```

### Comparing `metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-suite-tutorial/app/forecast/file/map-template.html` & `metomi-rose-2.1.0/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/app/forecast/file/map-template.html`

 * *Files 10% similar despite different names*

```diff
@@ -1,82 +1,93 @@
 <html>
-  <head>
-    <link rel="stylesheet"
-          href="https://unpkg.com/leaflet@1.2.0/dist/leaflet.css" />
+
+<head>
+    <link rel="stylesheet" href="https://unpkg.com/leaflet@1.2.0/dist/leaflet.css" />
     <script src="https://unpkg.com/leaflet@1.2.0/dist/leaflet.js"></script>
-  </head>
-  <body>
+</head>
+
+<body>
     <div id="map" style="width:100%;height:100%"></div>
 
     <script type="text/javascript">
-      // Define the colours to display for the different rainfall values.
-      // NOTE: Rainfall values range from 0 to 6+.
-      function get_colour(value) {
-          if (value < 0.1)
-              return '#ffffff88';
-          if (value < 0.5)
-              return '#00F7FF';
-          if (value < 1)
-              return '#00AAFF';
-          else if (value < 2)
-              return '#0051FF';
-          else if (value < 3)
-              return '#6600FF';
-          else if (value < 4)
-              return '#AE00FF';
-          else if (value < 5)
-              return '#FF00EA';
-          else
-              return '#FF0055';
-      }
-
-      // Forecast data as dict {'lead_time': [2d data matrix]}.
-      var data = {{ data }};
-
-      // Annotate map with data.
-      var lng;
-      var lat;
-      var rects;
-      var times = [];
-      var layers = [];
-      for (let time in data) {
-          rects = L.layerGroup();
-          for (let pos_y in data[time]) {
-              for (let pos_x in data[time][0]) {
-                  lng = (pos_x * {{ resolution }}) + {{ lng1 }};
-                  lat = {{ lat2 }} - (pos_y * {{ resolution }});
-                  L.rectangle(
-                      [[lat, lng],
-                      [lat + {{ resolution }}, lng + {{ resolution }}]],
-                      {color: get_colour(data[time][pos_y][pos_x]),
-                       weight: 0, fillOpacity: 0.5}).addTo(rects);
-              }
-          }
-          layers.push(rects);
-          times.push(time);
-      }
-
-      // Sort map layers lexicographically.
-      var sorted_times = times.slice(0);  // Copy the times list.
-      var fcsts = {};  // {'lead_time': L.LayerGroup}  Note dicts are ordered.
-      sorted_times.sort();
-      var ind;
-      for (let time of sorted_times) {
-          ind = times.indexOf(time);
-          fcsts[times[ind]] = layers[ind];
-      }
-
-      // Create map.
-      var map = L.map('map', {layers: [fcsts[sorted_times[0]]]});
-
-      // Zoom / center map to fit domain.
-      map.fitBounds([[{{ lat1 }}, {{ lng1 }}], [{{ lat2 }}, {{ lng2 }}]]);
-
-      // Add mapp tiles.
-      map.addLayer(
-          L.tileLayer('http://{s}.tile.openstreetmap.org/{z}/{x}/{y}.png'));
+        // Define the colours to display for the different rainfall values.
+        // NOTE: Rainfall values range from 0 to 6+.
+        function get_colour(value) {
+            if (value < 0.1)
+                return '#ffffff88';
+            if (value < 0.5)
+                return '#00F7FF';
+            if (value < 1)
+                return '#00AAFF';
+            else if (value < 2)
+                return '#0051FF';
+            else if (value < 3)
+                return '#6600FF';
+            else if (value < 4)
+                return '#AE00FF';
+            else if (value < 5)
+                return '#FF00EA';
+            else
+                return '#FF0055';
+        }
+
+        // Forecast data as dict {'lead_time': [2d data matrix]}.
+        var data = {{ data }};
+
+        // Annotate map with data.
+        var lng;
+        var lat;
+        var rects;
+        var times = [];
+        var layers = [];
+        for (let time in data) {
+            rects = L.layerGroup();
+            for (let pos_y in data[time]) {
+                for (let pos_x in data[time][0]) {
+                    lng = (pos_x * {{ resolution }}) + {{ lng1 }};
+                    lat = {{ lat2 }} - (pos_y * {{ resolution }});
+                    L.rectangle(
+                        [
+                            [lat, lng],
+                            [lat + {{ resolution }}, lng + {{ resolution }}]
+                        ], {
+                            color: get_colour(data[time][pos_y][pos_x]),
+                            weight: 0,
+                            fillOpacity: 0.5
+                        }).addTo(rects);
+                }
+            }
+            layers.push(rects);
+            times.push(time);
+        }
+
+        // Sort map layers lexicographically.
+        var sorted_times = times.slice(0); // Copy the times list.
+        var fcsts = {}; // {'lead_time': L.LayerGroup}  Note dicts are ordered.
+        sorted_times.sort();
+        var ind;
+        for (let time of sorted_times) {
+            ind = times.indexOf(time);
+            fcsts[times[ind]] = layers[ind];
+        }
+
+        // Create map.
+        var map = L.map('map', {
+            layers: [fcsts[sorted_times[0]]]
+        });
+
+        // Zoom / center map to fit domain.
+        map.fitBounds([
+            [{{ lat1 }}, {{ lng1 }}],
+            [{{ lat2 }}, {{ lng2 }}]
+        ]);
+
+        // Add map tiles.
+        map.addLayer(
+            L.tileLayer('http://{s}.tile.openstreetmap.org/{z}/{x}/{y}.png'));
 
-      // Add layer selector.
-      L.control.layers(fcsts).addTo(map);
+        // Add layer selector.
+        L.control.layers(fcsts).addTo(map);
     </script>
-  </body>
+</body>
+
 </html>
```

### Comparing `metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-suite-tutorial/app/forecast/file/test-data/rainfall.csv` & `metomi-rose-2.1.0/metomi/rose/etc/tutorial/rose-suite-tutorial/app/forecast/file/test-data/rainfall.csv`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-suite-tutorial/app/forecast/file/test-data/wind_20171101T0000Z_x.csv` & `metomi-rose-2.1.0/metomi/rose/etc/tutorial/rose-suite-tutorial/app/forecast/file/test-data/wind_20171101T0000Z_x.csv`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-suite-tutorial/app/forecast/file/test-data/wind_20171101T0000Z_y.csv` & `metomi-rose-2.1.0/metomi/rose/etc/tutorial/rose-suite-tutorial/app/forecast/file/test-data/wind_20171101T0000Z_y.csv`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-suite-tutorial/app/forecast/meta/rose-meta.conf` & `metomi-rose-2.1.0/metomi/rose/etc/tutorial/rose-suite-tutorial/app/forecast/meta/rose-meta.conf`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-suite-tutorial/bin/get-rainfall` & `metomi-rose-2.1.0/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/bin/get-rainfall`

 * *Files 14% similar despite different names*

```diff
@@ -1,44 +1,64 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 # -----------------------------------------------------------------------------
-# Copyright (C) British Crown (Met Office) & Contributors - GNU V3+.
+# THIS FILE IS PART OF THE CYLC WORKFLOW ENGINE.
+# Copyright (C) NIWA & British Crown (Met Office) & Contributors.
+#
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU General Public License as published by
+# the Free Software Foundation, either version 3 of the License, or
+# (at your option) any later version.
+#
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU General Public License for more details.
+#
+# You should have received a copy of the GNU General Public License
+# along with this program.  If not, see <http://www.gnu.org/licenses/>.
+# -----------------------------------------------------------------------------
 # This is illustrative code developed for tutorial purposes, it is not
 # intended for scientific use and is not guarantied to be accurate or correct.
-# -----------------------------------------------------------------------------
 """
 Usage:
     get-rainfall
 
 Environment Variables:
     API_KEY: The DataPoint API key, required for getting live weather data.
         If un-specified then get-observations will fall back to archive data
-        from the suite directory.
-    DOMIAN: The area in which to generate forecasts for in the format
+        from the workflow directory.
+    DOMAIN: The area in which to generate forecasts for in the format
         (lng1, lat1, lng2, lat2).
     RESOLUTION: The length/width of each grid cell in degrees.
 
 """
 
 from datetime import datetime
 import math
 import os
 import shutil
-import urllib.request
 
-import PIL.Image
-from mecator import get_offset, get_scale, coord_to_pos, pos_to_coord
+import requests
+
+try:
+    from PIL import Image
+except ModuleNotFoundError:
+    # not all PIL installations are created equal
+    # sometimes we must import like this
+    import Image
+from mercator import get_offset, get_scale, pos_to_coord
 import util
 
 
 URL = ('http://datapoint.metoffice.gov.uk/public/data/layer/wxobs/'
        'RADAR_UK_Composite_Highres/png?TIME={time}&key={api_key}')
 
 
-class Rainfall:
+class Rainfall(object):
     """Class for holding rainfall data.
 
     Args:
         domain (dict): Domain as returned by util.parse_domain()
         resolution (float): The length of each grid cell in degrees.
 
     """
@@ -52,30 +72,32 @@
         (254, 0, 254, 255): 7
     }
 
     def __init__(self, domain, resolution):
         self.resolution = resolution
         self.domain = domain
 
-        rows = int(math.ceil(abs(domain['lat1'] - domain['lat2']) / resolution))
-        cols = int(math.ceil(abs(domain['lng1'] - domain['lng2']) / resolution))
+        rows = int(
+            math.ceil(abs(domain['lat1'] - domain['lat2']) / resolution))
+        cols = int(
+            math.ceil(abs(domain['lng1'] - domain['lng2']) / resolution))
 
         self.data = []
         for itt_y in range(rows):
             self.data.append([])
             for _ in range(cols):
                 self.data[itt_y].append([])
 
     def add(self, lng, lat, value):
         """Add a data point to this data set.
 
         Args:
             lng (float): The longitude for this reading.
             lat (float): The latitude fo this reading.
-            value (float): The value of the reading.
+            value (tuple): The value of the reading.
 
         """
         itt_x, itt_y = util.get_grid_coordinates(lng, lat, self.domain,
                                                  self.resolution)
         try:
             self.data[itt_y][itt_x].append(self.VALUE_MAP[value])
         except KeyError:
@@ -93,56 +115,58 @@
 
 
 def get_datapoint_radar_image(filename, time, api_key):
     """Retrieve a png image of rainfall from the DataPoint service.
 
     Args:
         filename (str): The path to write the image file to.
-        time (str): The date-time of the image to reteieve in ISO8601 format.
+        time (str): The datetime of the image to retrieve in ISO8601 format.
         api_key (str): Datapoint API key.
 
     """
-    time = datetime.strptime(time, '%Y%m%dT%H%MZ'
-                            ).strftime('%Y-%m-%dT%H:%M:%SZ')
+    time = datetime.strptime(time, '%Y%m%dT%H%MZ').strftime(
+        '%Y-%m-%dT%H:%M:%SZ')
     url = URL.format(time=time, api_key=api_key)
-    print('Opening URL: %s' % url)
-    out = urllib.request.urlopen(url).read()
-    with open(filename, 'bw+') as png_file:
-        png_file.write(out)
+    req = requests.get(url)
+    if req.status_code != 200:
+        raise Exception(f'{url} returned exit code {req.status_code}')
+    with open(filename, 'bw') as png_file:
+        png_file.write(req.content)
 
 
 def get_archived_radar_image(filename, time):
-    """Retrieve a png image from the archived data in the suite directory.
+    """Retrieve a png image from the archived data in the workflow directory.
 
     Args:
         filename (str): The path to write the image file to.
-        time (str): The date-time of the image to reteieve in ISO8601 format.
+        time (str): The datetime of the image to retrieve in ISO8601 format.
 
     """
     shutil.copyfile(
-        os.path.join(os.environ['CYLC_SUITE_DEF_PATH'], 'data', time, filename),
+        os.path.join(os.environ['CYLC_WORKFLOW_RUN_DIR'], 'data', time,
+                     filename),
         filename)
 
 
 def process_rainfall_data(filename, resolution, domain):
-    """Generate a 2D matric of data from the rainfall data in the image.
+    """Generate a 2D matrix of data from the rainfall data in the image.
 
     Args:
         filename (str): Path to the png image to process.
-        resolution (float): The length/wieght of each grid cell in degrees.
+        resolution (float): The length/weight of each grid cell in degrees.
         domain (dict): The bounds of the domain as returned by
             util.parse_domain.
 
     Return:
         list - A 2D matrix of rainfall data.
 
     """
     rainfall = Rainfall(domain, resolution)
 
-    image = PIL.Image.open(filename)
+    image = Image.open(filename)
     scale = get_scale(domain, image.width)
     offset = get_offset(domain, scale)
 
     for itt_x in range(image.width):
         for itt_y in range(image.height):
             lng, lat = pos_to_coord(
                 itt_x,
@@ -159,15 +183,15 @@
     domain = util.parse_domain(os.environ['DOMAIN'])
     api_key = os.environ.get('API_KEY')
 
     if api_key:
         print('Attempting to get weather data from the DataPoint service.')
         get_datapoint_radar_image('rainfall-radar.png', time, api_key)
     else:
-        print('No API key provided, falling back to arhived data')
+        print('No API key provided, falling back to archived data')
         get_archived_radar_image('rainfall-radar.png', time)
 
     data = process_rainfall_data('rainfall-radar.png', resolution, domain)
     util.write_csv('rainfall.csv', data)
 
 
 if __name__ == '__main__':
```

### Comparing `metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-suite-tutorial/bin/post-process` & `metomi-rose-2.1.0/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/bin/post-process`

 * *Files 27% similar despite different names*

```diff
@@ -1,25 +1,39 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 # -----------------------------------------------------------------------------
-# Copyright (C) British Crown (Met Office) & Contributors - GNU V3+.
+# THIS FILE IS PART OF THE CYLC WORKFLOW ENGINE.
+# Copyright (C) NIWA & British Crown (Met Office) & Contributors.
+#
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU General Public License as published by
+# the Free Software Foundation, either version 3 of the License, or
+# (at your option) any later version.
+#
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU General Public License for more details.
+#
+# You should have received a copy of the GNU General Public License
+# along with this program.  If not, see <http://www.gnu.org/licenses/>.
+# -----------------------------------------------------------------------------
 # This is illustrative code developed for tutorial purposes, it is not
 # intended for scientific use and is not guarantied to be accurate or correct.
-# -----------------------------------------------------------------------------
 """
 Usage:
     post-process SITE TIME
 
 Arguments:
     SITE: The name of the location to process data for.
     TIME: The time ahead of the cycle point to produce the forecast for in
           minutes.
 
 Environment Variables:
-    DOMIAN: The area in which to generate forecasts for in the format
+    DOMAIN: The area in which to generate forecasts for in the format
         (lng1, lat1, lng2, lat2).
     RESOLUTION: The length/width of each grid cell in degrees.
 
 """
 
 from datetime import datetime, timedelta
 import os
@@ -43,15 +57,15 @@
     lng, lat = SITE_LOCATIONS[site_name]
 
     # Load forecast data.
     filename = '+PT%02dH%02dM.csv' % (time // 60, time % 60)
     try:
         # The path to the forecast data file.
         forecast = util.read_csv(os.path.join(
-            os.environ['CYLC_SUITE_WORK_DIR'],
+            os.environ['CYLC_WORKFLOW_WORK_DIR'],
             os.environ['CYLC_TASK_CYCLE_POINT'],
             'forecast',
             filename
         ))
     except IOError:
         sys.exit('Could not find forecast "%s".' % filename)
```

### Comparing `metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-suite-tutorial/flow.cylc` & `metomi-rose-2.1.0/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/flow.cylc`

 * *Files 21% similar despite different names*

```diff
@@ -1,65 +1,63 @@
+#!jinja2
 [scheduler]
     UTC mode = True
-    [[parameters]]
-        # A list of the weather stations we will be fetching observations from.
-        station = camborne, heathrow, shetland, belmullet
-        # A list of the sites we will be generating forecasts for.
-        site = exeter
+[task parameters]
+    # A list of the weather stations we will be fetching observations from.
+    station = {{ station | join(", ") }}
+    # A list of the sites we will be generating forecasts for.
+    site = exeter
 
 [scheduling]
-    # Start the suite 7 hours before now ignoring minutes and seconds
+    # Start the workflow 7 hours before now ignoring minutes and seconds
     # * previous(T-00) takes the current time ignoring minutes and seconds.
     # * - PT7H subtracts 7 hours from the time.
     initial cycle point = previous(T-00) - PT7H
-    # Stop the suite 6 hours after the initial cycle point.
+    # Stop the workflow 6 hours after the initial cycle point.
     final cycle point = +PT6H
-    [[dependencies]]
-        [[[PT3H]]]
-            # Repeat every three hours starting at the initial cycle point.
-            graph = """
-                get_observations<station> => consolidate_observations
-            """
-
-        [[[+PT6H/PT6H]]]
-            # Repeat every six hours starting six hours after the initial
-            # cycle point.
-            graph = """
-                consolidate_observations => forecast
-                consolidate_observations[-PT3H] => forecast
-                consolidate_observations[-PT6H] => forecast
-                get_rainfall => forecast => post_process<site>
-            """
-
-        [[[+PT12H/PT6H]]]
-            # Repeat every six hours starting twelve hours after the initial
-            # cycle point.
-            graph = """
-                forecast[-PT6H] => forecast
-            """
+    [[graph]]
+        # Repeat every three hours starting at the initial cycle point.
+        PT3H = """
+            get_observations<station> => consolidate_observations
+        """
+
+        # Repeat every six hours starting six hours after the initial
+        # cycle point.
+        +PT6H/PT6H = """
+            consolidate_observations => forecast
+            consolidate_observations[-PT3H] => forecast
+            consolidate_observations[-PT6H] => forecast
+            get_rainfall => forecast => post_process<site>
+        """
+
+        # Repeat every six hours starting twelve hours after the initial
+        # cycle point.
+        +PT12H/PT6H = """
+            forecast[-PT6H] => forecast
+        """
 
 [runtime]
     [[root]]
         # These environment variables will be available to all tasks.
         [[[environment]]]
             # The dimensions of each grid cell in degrees.
-            RESOLUTION = 0.2
+            RESOLUTION = {{ RESOLUTION }}
             # The area to generate forecasts for (lng1, lat1, lng2, lat2)
-            DOMAIN = -12,48,5,61  # Do not change!
+            DOMAIN = {{ DOMAIN | join(", ")}}
 
     [[get_observations<station>]]
         script = get-observations
         [[[environment]]]
             # The key required to get weather data from the DataPoint service.
             # To use archived data comment this line out.
-            API_KEY = DATAPOINT_API_KEY
+            API_KEY = 3b627bb4-f8aa-4ed5-b486-09c606a475ef
 
-    [[get_observations<station=belmullet>]]
+    [[get_observations<station=aldergrove>]]
         [[[environment]]]
-            SITE_ID = 3976
+            SITE_ID = 3917
     [[get_observations<station=camborne>]]
         [[[environment]]]
             SITE_ID = 3808
     [[get_observations<station=heathrow>]]
         [[[environment]]]
             SITE_ID = 3772
     [[get_observations<station=shetland>]]
@@ -70,27 +68,17 @@
         script = consolidate-observations
 
     [[get_rainfall]]
         script = get-rainfall
         [[[environment]]]
             # The key required to get weather data from the DataPoint service.
             # To use archived data comment this line out.
-            API_KEY = DATAPOINT_API_KEY
+            API_KEY = 3b627bb4-f8aa-4ed5-b486-09c606a475ef
 
     [[forecast]]
-        script = forecast 60 5  # Generate 5 forecasts at 60 minute intervals.
-        [[[environment]]]
-            # The path to the files containing wind data (the {variables} will
-            # get substituted in the forecast script).
-            WIND_FILE_TEMPLATE = $CYLC_SUITE_WORK_DIR/{cycle}/consolidate_observations/wind_{xy}.csv
-            # Offset in hours to cycles to process wind data from.
-            WIND_CYCLES = 0, -3, -6
-            # The path to the rainfall file.
-            RAINFALL_FILE = $CYLC_SUITE_WORK_DIR/$CYLC_TASK_CYCLE_POINT/get_rainfall/rainfall.csv
-            # Create the html map file in the task's log directory.
-            MAP_FILE = "${CYLC_TASK_LOG_ROOT}-map.html"
-            # The path to the template file used to generate the html map.
-            MAP_TEMPLATE = "$CYLC_SUITE_RUN_DIR/lib/template/map.html"
+        script = rose task-run
 
     [[post_process<site>]]
         # Generate a forecast for the location <site> 60 minutes in the future.
         script = post-process $CYLC_TASK_PARAM_site 60
+
+{% include 'etc/python-job.settings' %}
```

### Comparing `metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-suite-tutorial/lib/python/mecator.py` & `metomi-rose-2.1.0/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/lib/python/mercator.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,34 @@
-# Copyright (C) British Crown (Met Office) & Contributors - GNU V3+.
+# -*- coding: utf-8 -*-
+# -----------------------------------------------------------------------------
+# THIS FILE IS PART OF THE CYLC WORKFLOW ENGINE.
+# Copyright (C) NIWA & British Crown (Met Office) & Contributors.
+#
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU General Public License as published by
+# the Free Software Foundation, either version 3 of the License, or
+# (at your option) any later version.
+#
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU General Public License for more details.
+#
+# You should have received a copy of the GNU General Public License
+# along with this program.  If not, see <http://www.gnu.org/licenses/>.
+# -----------------------------------------------------------------------------
 # This is illustrative code developed for tutorial purposes, it is not
 # intended for scientific use and is not guarantied to be accurate or correct.
-# -----------------------------------------------------------------------------
 import math
 
+
 R_0 = 6356752.3
 
 
-def get_offset(bbox, scale=(1.0, 1.0)):
+def get_offset(bbox, scale=(1., 1.)):
     """Define an offset from the origin using the provided bbox.
 
     Args:
         bbox: The coordinates of the domain as a dictionary {'lat1', 'lng1',
             'lat2', 'lng2'}
         scale: The x, y scale factor as returned by get_scale().
 
@@ -24,50 +41,49 @@
 
     Args:
         bbox: The coordinates of the domain as a dictionary {'lat1', 'lng1',
             'lat2', 'lng2'}
         width: The width of the projection.
 
     """
-    scale = width * (180.0 / abs(bbox['lng2'] - bbox['lng1']))
+    scale = width * (180. / abs(bbox['lng2'] - bbox['lng1']))
     return (
         (math.pi * R_0) / scale,
-        (math.pi * R_0 * 2.0) / scale,
-    )
+        (math.pi * R_0 * 2.) / scale)
 
 
-def coord_to_pos(lng, lat, offset=(0.0, 0.0), scale=(1.0, 1.0)):
-    """Convert a lng, lat coord to an x, y position in a mecator projection.
+def coord_to_pos(lng, lat, offset=(0., 0.), scale=(1., 1.)):
+    """Convert a lng, lat coord to an x, y position in a mercator projection.
 
     proj equivalent:
         $ echo <lng> <lat> | proj +proj=merc
         # Divide by scale.
         # Subtract offset.
 
     """
     lng = math.radians(lng)
     lat = math.radians(lat)
     pos_x = R_0 * lng
-    pos_y = R_0 * math.log(math.tan((math.pi / 4.0) + (lat / 2.0)))
+    pos_y = R_0 * math.log(math.tan((math.pi / 4.) + (lat / 2.)))
     pos_x /= scale[0]
     pos_y /= scale[1]
     pos_x -= offset[0]
     pos_y -= offset[1]
     return pos_x, pos_y
 
 
-def pos_to_coord(pos_x, pos_y, offset=(0.0, 0.0), scale=(1.0, 1.0)):
-    """Convert an x, y coordinate in a mecator projection to a lng, lat coord.
+def pos_to_coord(pos_x, pos_y, offset=(0., 0.), scale=(1., 1.)):
+    """Convert an x, y coordinate in a mercator projection to a lng, lat coord.
 
     proj equivalent:
         # Add offset
         # Multiply by scale.
         $ echo <pos_x> <pos_y> | proj -I +proj=merc
 
     """
     pos_x += offset[0]
     pos_y += offset[1]
     pos_x *= scale[0]
     pos_y *= scale[1]
     lng = pos_x / R_0
-    lat = 2 * math.atan(math.exp(pos_y / R_0)) - (math.pi / 2.0)
+    lat = 2 * math.atan(math.exp(pos_y / R_0)) - (math.pi / 2.)
     return math.degrees(lng), math.degrees(lat)
```

### Comparing `metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-suite-tutorial/lib/python/util.py` & `metomi-rose-2.1.0/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/app/forecast/bin/util.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,35 @@
-# Copyright (C) British Crown (Met Office) & Contributors - GNU V3+.
+# -*- coding: utf-8 -*-
+# -----------------------------------------------------------------------------
+# THIS FILE IS PART OF THE CYLC WORKFLOW ENGINE.
+# Copyright (C) NIWA & British Crown (Met Office) & Contributors.
+#
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU General Public License as published by
+# the Free Software Foundation, either version 3 of the License, or
+# (at your option) any later version.
+#
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU General Public License for more details.
+#
+# You should have received a copy of the GNU General Public License
+# along with this program.  If not, see <http://www.gnu.org/licenses/>.
+# -----------------------------------------------------------------------------
 # This is illustrative code developed for tutorial purposes, it is not
 # intended for scientific use and is not guarantied to be accurate or correct.
-# -----------------------------------------------------------------------------
 from copy import copy
+from contextlib import suppress
 import math
+import jinja2
 import sys
 
-import jinja2
 
-R_0 = 6371.0  # Radius of the Earth (km).
+R_0 = 6371.  # Radius of the Earth (km).
 
 
 def frange(start, stop, step):
     """Implementation of python's xrange which works with floats."""
     while start < stop:
         yield start
         start += step
@@ -48,27 +65,26 @@
 
     Args:
         filename (str): The path of the csv file to write to.
         field (function): A function of the form f(x, y) -> z.
         x_range (list): List of the x coordinates of the extrapolated grid.
             These are the extrapolation coordinates, the length of this list
             defines the size of the grid.
-        x_range (list): List of the y coordinates of the extrapolated grid.
+        y_range (list): List of the y coordinates of the extrapolated grid.
             These are the extrapolation coordinates, the length of this list
             defines the size of the grid.
 
     """
     with open(filename, 'w+') as csv_file:
         for itt_y in y_range:
-            csv_file.write(
-                ', '.join('%.2f' % field(x, itt_y) for x in x_range) + '\n'
-            )
+            csv_file.write(', '.join('%.2f' % field(x, itt_y) for
+                                     x in x_range) + '\n')
 
 
-def generate_matrix(dim_x, dim_y, value=0.0):
+def generate_matrix(dim_x, dim_y, value=0.):
     """Generates a 2D list with the desired dimensions.
 
     Args:
         dim_x (int): The x-dimension of the matrix.
         dim_y (int): The y-dimension of the matrix.
         value: The default value for each cell of the matrix.
 
@@ -99,23 +115,20 @@
     (lng_1, lat_1) = coordinate_1
     (lng_2, lat_2) = coordinate_2
     lng_1 = math.radians(lng_1)
     lat_1 = math.radians(lat_1)
     lng_2 = math.radians(lng_2)
     lat_2 = math.radians(lat_2)
     return (
-        2
-        * R_0
-        * math.asin(
+        2 * R_0 * math.asin(
             math.sqrt(
-                (math.sin((lat_2 - lat_1) / 2.0) ** 2)
-                + (
-                    math.cos(lat_1)
-                    * math.cos(lat_2)
-                    * (math.sin((lng_2 - lng_1) / 2.0) ** 2)
+                (math.sin((lat_2 - lat_1) / 2.) ** 2) + (
+                    math.cos(lat_1) *
+                    math.cos(lat_2) *
+                    (math.sin((lng_2 - lng_1) / 2.) ** 2)
                 )
             )
         )
     )
 
 
 def interpolate_grid(points, dim_x, dim_y, d_x, d_y, spline_order=0):
@@ -132,61 +145,57 @@
             interpolation (0 = nearset).
 
     Return:
         list - 2D matrix of dimensions dim_x, dim_y containing the interpolated
         data.
 
     """
-
     def spline_0(pos_x, pos_y, z_val):
         """Zeroth order beta spline (i.e. nearest point)."""
         return [(int(round(pos_x)), int(round(pos_y)), z_val)]  # [(x, y, z)]
 
     def spline_1(pos_x, pos_y, z_val):
-        """First order beta spline (weight spread about four nearest ponts)."""
+        """First order beta spline (weight spread about four nearest
+        points)."""
         x_0 = int(math.floor(pos_x))
         y_0 = int(math.floor(pos_y))
         x_1 = x_0 + 1
         y_1 = y_0 + 1
         return [
             # (x, y, z), ...
             (x_0, y_0, (x_0 + d_x - pos_x) * (y_0 + d_y - pos_y) * z_val),
             (x_1, y_0, (pos_x - x_0) * (y_0 + d_y - pos_y) * z_val),
             (x_0, y_1, (x_0 + d_x - pos_x) * (pos_y - y_0) * z_val),
-            (x_1, y_1, (pos_x - x_0) * (pos_y - y_0) * z_val),
+            (x_1, y_1, (pos_x - x_0) * (pos_y - y_0) * z_val)
         ]
 
     if spline_order == 0:
         spline = spline_0
-    elif spline_order == 1:
+    elif spline_order == 1:  # noqa: SIM106 (case type matching)
         spline = spline_1
     else:
-        raise ValueError(
-            'Invalid spline order "%d" must be in (0, 1).' % spline_order
-        )
+        raise ValueError('Invalid spline order "%d" must be in (0, 1).' %
+                         spline_order)
 
-    grid = generate_matrix(dim_x, dim_y, 0.0)
+    grid = generate_matrix(dim_x, dim_y, 0.)
 
     for x_val, y_val, z_val in points:
         x_coord = x_val / d_x
         y_coord = y_val / d_y
         for grid_x, grid_y, grid_z in spline(x_coord, y_coord, z_val):
-            try:
+            with suppress(IndexError):
                 grid[grid_y][grid_x] += grid_z
-            except IndexError:
-                # Grid point out of bounds => skip.
-                pass
+                # skip grid point out of bounds
 
     return grid
 
 
 def plot_vector_grid(filename, x_grid, y_grid):
     try:
         import matplotlib
-
         matplotlib.use('Agg')
         import matplotlib.pyplot as plt
     except ImportError:
         print('Plotting disabled', file=sys.stderr)
         return
 
     fig = plt.figure()
@@ -195,34 +204,31 @@
     z_coords = []
     for itt_x in range(len(x_grid[0])):
         for itt_y in range(len(x_grid)):
             x_coords.append(itt_x)
             y_coords.append(itt_y)
             z_coords.append((
                 x_grid[itt_y][itt_x],
-                y_grid[itt_y][itt_x],
+                y_grid[itt_y][itt_x]
             ))
 
-    plt.quiver(
-        x_coords,
-        y_coords,
-        [x[0] for x in z_coords],
-        [y[1] for y in z_coords],
-    )
+    plt.quiver(x_coords,
+               y_coords,
+               [x[0] for x in z_coords],
+               [y[1] for y in z_coords])
     fig.savefig(filename)
 
 
 def get_grid_coordinates(lng, lat, domain, resolution):
     """Return the grid coordinates for a lat, long coordinate pair."""
     # NOTE: Grid coordinates run from *top* left to bottom right.
     length_y = int(abs(domain['lat2'] - domain['lat1']) // resolution)
     return (
         int((abs(lng - domain['lng1'])) // resolution),
-        length_y - int((abs(lat - domain['lat1'])) // resolution),
-    )
+        length_y - int((abs(lat - domain['lat1'])) // resolution))
 
 
 class SurfaceFitter:
     """A 2D interpolation for random points.
 
     A standin for scipy.interpolate.interp2d
 
@@ -239,19 +245,19 @@
 
     """
 
     def __init__(self, x_points, y_points, z_points, kind='linear'):
         self.points = list(zip(x_points, y_points, z_points))
 
         if kind == 'linear':
-            self.power = 1.0
+            self.power = 1.
         elif kind == 'quadratic':
-            self.power = 2.0
-        elif kind == 'cubic':
-            self.power = 3.0
+            self.power = 2.
+        elif kind == 'cubic':  # noqa: SIM106 (case type matching)
+            self.power = 3.
         else:
             raise ValueError('"%s" is not a valid interpolation method' % kind)
 
     def __call__(self, grid_x, grid_y):
         sum_value = 0.0
         sum_weight = 0.0
         z_val = None
@@ -260,15 +266,15 @@
             d_y = grid_y - y_point
             if d_x == 0 and d_y == 0:
                 # This point is exactly at the grid location we are
                 # interpolating for, return this value.
                 z_val = z_point
                 break
             else:
-                weight = 1.0 / ((math.sqrt(d_x ** 2 + d_y ** 2)) ** self.power)
+                weight = 1. / ((math.sqrt(d_x ** 2 + d_y ** 2)) ** self.power)
                 sum_weight += weight
                 sum_value += weight * z_point
 
         if z_val is None:
             z_val = sum_value / sum_weight
 
         return z_val
@@ -276,24 +282,22 @@
 
 def parse_domain(domain):
     bbox = list(map(float, domain.split(',')))
     return {
         'lng1': bbox[0],
         'lat1': bbox[1],
         'lng2': bbox[2],
-        'lat2': bbox[3],
+        'lat2': bbox[3]
     }
 
 
 def generate_html_map(filename, template_file, data, domain, resolution):
-    with open(template_file, 'r') as template:
+    with open(template_file, 'r') as template:  # noqa: SIM117
         with open(filename, 'w+') as html_file:
-            html_file.write(
-                jinja2.Template(template.read()).render(
-                    resolution=resolution,
-                    lng1=domain['lng1'],
-                    lng2=domain['lng2'],
-                    lat1=domain['lat1'],
-                    lat2=domain['lat2'],
-                    data=data,
-                )
-            )
+            html_file.write(jinja2.Template(template.read()).render(
+                resolution=resolution,
+                lng1=domain['lng1'],
+                lng2=domain['lng2'],
+                lat1=domain['lat1'],
+                lat2=domain['lat2'],
+                data=data
+            ))
```

### Comparing `metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/app/forecast/bin/forecast` & `metomi-rose-2.1.0/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/bin/forecast`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,28 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 # -----------------------------------------------------------------------------
-# Copyright (C) British Crown (Met Office) & Contributors - GNU V3+.
+# THIS FILE IS PART OF THE CYLC WORKFLOW ENGINE.
+# Copyright (C) NIWA & British Crown (Met Office) & Contributors.
+#
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU General Public License as published by
+# the Free Software Foundation, either version 3 of the License, or
+# (at your option) any later version.
+#
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU General Public License for more details.
+#
+# You should have received a copy of the GNU General Public License
+# along with this program.  If not, see <http://www.gnu.org/licenses/>.
+# -----------------------------------------------------------------------------
 # This is illustrative code developed for tutorial purposes, it is not
 # intended for scientific use and is not guarantied to be accurate or correct.
-# -----------------------------------------------------------------------------
 """
 Usage:
     forecast INTERVAL ITERATIONS
 
 Arguments:
     INTERVAL: The period between forecasts in minutes.
     ITERATIONS: The number of forecasts to produce.
@@ -43,15 +57,15 @@
         wind_file_path (str): Template for the path to a wind data file.
             The template should contain substitutions for `{cycles}`
             (i.e. the cycle point) and `{xy}` (i.e. the value 'x' or 'y').
         wind_cycles (list): List of cycle points to get wind data for
             as strings.
 
     Return:
-            list - A list 2-tuples containing wind field matricies i.e.
+            list - A list 2-tuples containing wind field matrices i.e.
             [(wind_x, wind_y), ...]
 
     """
     wind_fields = []
     for cycle in wind_cycles:
         wind_x = util.read_csv(wind_file_path.format(cycle=cycle, xy='x'))
         wind_y = util.read_csv(wind_file_path.format(cycle=cycle, xy='y'))
@@ -176,16 +190,16 @@
     """
     return Popen(
         ['cylc', 'cyclepoint', '--offset-hours', str(int(offset_hours))],
         stdout=PIPE
     ).communicate()[0].strip().decode()
 
 
-def main(forecast_interval, forecast_itterations):
-    # Get suite settings.
+def main(forecast_interval, forecast_iterations):
+    # Get workflow settings.
     domain = util.parse_domain(os.environ['DOMAIN'])
     resolution = float(os.environ['RESOLUTION'])
 
     # Get science settings.
     spline_level = int(os.environ.get('SPLINE_LEVEL', 0))
     weighting = list(map(float, os.environ.get('WEIGHTING', '1').split(',')))
 
@@ -208,15 +222,15 @@
 
     # Initiate the forecaster.
     generator = push_rainfall(rainfall, weighted_wind_data, forecast_interval,
                               resolution, spline_level)
 
     # Generate forecasts.
     forecasts = {}
-    for lead_minutes in range(0, forecast_interval * (forecast_itterations + 1),
+    for lead_minutes in range(0, forecast_interval * (forecast_iterations + 1),
                               forecast_interval):
         forecast_name = '+PT%02dH%02dM' % (lead_minutes // 60,
                                            lead_minutes % 60)
         # Generate forecast.
         forecast = next(generator)
         forecasts[forecast_name] = forecast
         # Output forecast data.
```

### Comparing `metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/app/forecast/bin/util.py` & `metomi-rose-2.1.0/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/lib/python/util.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,35 @@
-# Copyright (C) British Crown (Met Office) & Contributors - GNU V3+.
+# -*- coding: utf-8 -*-
+# -----------------------------------------------------------------------------
+# THIS FILE IS PART OF THE CYLC WORKFLOW ENGINE.
+# Copyright (C) NIWA & British Crown (Met Office) & Contributors.
+#
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU General Public License as published by
+# the Free Software Foundation, either version 3 of the License, or
+# (at your option) any later version.
+#
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU General Public License for more details.
+#
+# You should have received a copy of the GNU General Public License
+# along with this program.  If not, see <http://www.gnu.org/licenses/>.
+# -----------------------------------------------------------------------------
 # This is illustrative code developed for tutorial purposes, it is not
 # intended for scientific use and is not guarantied to be accurate or correct.
-# -----------------------------------------------------------------------------
 from copy import copy
+from contextlib import suppress
 import math
+import jinja2
 import sys
 
-import jinja2
 
-R_0 = 6371.0  # Radius of the Earth (km).
+R_0 = 6371.  # Radius of the Earth (km).
 
 
 def frange(start, stop, step):
     """Implementation of python's xrange which works with floats."""
     while start < stop:
         yield start
         start += step
@@ -48,27 +65,26 @@
 
     Args:
         filename (str): The path of the csv file to write to.
         field (function): A function of the form f(x, y) -> z.
         x_range (list): List of the x coordinates of the extrapolated grid.
             These are the extrapolation coordinates, the length of this list
             defines the size of the grid.
-        x_range (list): List of the y coordinates of the extrapolated grid.
+        y_range (list): List of the y coordinates of the extrapolated grid.
             These are the extrapolation coordinates, the length of this list
             defines the size of the grid.
 
     """
     with open(filename, 'w+') as csv_file:
         for itt_y in y_range:
-            csv_file.write(
-                ', '.join('%.2f' % field(x, itt_y) for x in x_range) + '\n'
-            )
+            csv_file.write(', '.join('%.2f' % field(x, itt_y) for
+                                     x in x_range) + '\n')
 
 
-def generate_matrix(dim_x, dim_y, value=0.0):
+def generate_matrix(dim_x, dim_y, value=0.):
     """Generates a 2D list with the desired dimensions.
 
     Args:
         dim_x (int): The x-dimension of the matrix.
         dim_y (int): The y-dimension of the matrix.
         value: The default value for each cell of the matrix.
 
@@ -99,23 +115,20 @@
     (lng_1, lat_1) = coordinate_1
     (lng_2, lat_2) = coordinate_2
     lng_1 = math.radians(lng_1)
     lat_1 = math.radians(lat_1)
     lng_2 = math.radians(lng_2)
     lat_2 = math.radians(lat_2)
     return (
-        2
-        * R_0
-        * math.asin(
+        2 * R_0 * math.asin(
             math.sqrt(
-                (math.sin((lat_2 - lat_1) / 2.0) ** 2)
-                + (
-                    math.cos(lat_1)
-                    * math.cos(lat_2)
-                    * (math.sin((lng_2 - lng_1) / 2.0) ** 2)
+                (math.sin((lat_2 - lat_1) / 2.) ** 2) + (
+                    math.cos(lat_1) *
+                    math.cos(lat_2) *
+                    (math.sin((lng_2 - lng_1) / 2.) ** 2)
                 )
             )
         )
     )
 
 
 def interpolate_grid(points, dim_x, dim_y, d_x, d_y, spline_order=0):
@@ -132,61 +145,57 @@
             interpolation (0 = nearset).
 
     Return:
         list - 2D matrix of dimensions dim_x, dim_y containing the interpolated
         data.
 
     """
-
     def spline_0(pos_x, pos_y, z_val):
         """Zeroth order beta spline (i.e. nearest point)."""
         return [(int(round(pos_x)), int(round(pos_y)), z_val)]  # [(x, y, z)]
 
     def spline_1(pos_x, pos_y, z_val):
-        """First order beta spline (weight spread about four nearest ponts)."""
+        """First order beta spline (weight spread about four nearest
+        points)."""
         x_0 = int(math.floor(pos_x))
         y_0 = int(math.floor(pos_y))
         x_1 = x_0 + 1
         y_1 = y_0 + 1
         return [
             # (x, y, z), ...
             (x_0, y_0, (x_0 + d_x - pos_x) * (y_0 + d_y - pos_y) * z_val),
             (x_1, y_0, (pos_x - x_0) * (y_0 + d_y - pos_y) * z_val),
             (x_0, y_1, (x_0 + d_x - pos_x) * (pos_y - y_0) * z_val),
-            (x_1, y_1, (pos_x - x_0) * (pos_y - y_0) * z_val),
+            (x_1, y_1, (pos_x - x_0) * (pos_y - y_0) * z_val)
         ]
 
     if spline_order == 0:
         spline = spline_0
-    elif spline_order == 1:
+    elif spline_order == 1:  # noqa: SIM106 (case type matching)
         spline = spline_1
     else:
-        raise ValueError(
-            'Invalid spline order "%d" must be in (0, 1).' % spline_order
-        )
+        raise ValueError('Invalid spline order "%d" must be in (0, 1).' %
+                         spline_order)
 
-    grid = generate_matrix(dim_x, dim_y, 0.0)
+    grid = generate_matrix(dim_x, dim_y, 0.)
 
     for x_val, y_val, z_val in points:
         x_coord = x_val / d_x
         y_coord = y_val / d_y
         for grid_x, grid_y, grid_z in spline(x_coord, y_coord, z_val):
-            try:
+            with suppress(IndexError):
                 grid[grid_y][grid_x] += grid_z
-            except IndexError:
-                # Grid point out of bounds => skip.
-                pass
+                # skip grid point out of bounds
 
     return grid
 
 
 def plot_vector_grid(filename, x_grid, y_grid):
     try:
         import matplotlib
-
         matplotlib.use('Agg')
         import matplotlib.pyplot as plt
     except ImportError:
         print('Plotting disabled', file=sys.stderr)
         return
 
     fig = plt.figure()
@@ -195,34 +204,31 @@
     z_coords = []
     for itt_x in range(len(x_grid[0])):
         for itt_y in range(len(x_grid)):
             x_coords.append(itt_x)
             y_coords.append(itt_y)
             z_coords.append((
                 x_grid[itt_y][itt_x],
-                y_grid[itt_y][itt_x],
+                y_grid[itt_y][itt_x]
             ))
 
-    plt.quiver(
-        x_coords,
-        y_coords,
-        [x[0] for x in z_coords],
-        [y[1] for y in z_coords],
-    )
+    plt.quiver(x_coords,
+               y_coords,
+               [x[0] for x in z_coords],
+               [y[1] for y in z_coords])
     fig.savefig(filename)
 
 
 def get_grid_coordinates(lng, lat, domain, resolution):
     """Return the grid coordinates for a lat, long coordinate pair."""
     # NOTE: Grid coordinates run from *top* left to bottom right.
     length_y = int(abs(domain['lat2'] - domain['lat1']) // resolution)
     return (
         int((abs(lng - domain['lng1'])) // resolution),
-        length_y - int((abs(lat - domain['lat1'])) // resolution),
-    )
+        length_y - int((abs(lat - domain['lat1'])) // resolution))
 
 
 class SurfaceFitter:
     """A 2D interpolation for random points.
 
     A standin for scipy.interpolate.interp2d
 
@@ -239,19 +245,19 @@
 
     """
 
     def __init__(self, x_points, y_points, z_points, kind='linear'):
         self.points = list(zip(x_points, y_points, z_points))
 
         if kind == 'linear':
-            self.power = 1.0
+            self.power = 1.
         elif kind == 'quadratic':
-            self.power = 2.0
-        elif kind == 'cubic':
-            self.power = 3.0
+            self.power = 2.
+        elif kind == 'cubic':  # noqa: SIM106 (case type matching)
+            self.power = 3.
         else:
             raise ValueError('"%s" is not a valid interpolation method' % kind)
 
     def __call__(self, grid_x, grid_y):
         sum_value = 0.0
         sum_weight = 0.0
         z_val = None
@@ -260,15 +266,15 @@
             d_y = grid_y - y_point
             if d_x == 0 and d_y == 0:
                 # This point is exactly at the grid location we are
                 # interpolating for, return this value.
                 z_val = z_point
                 break
             else:
-                weight = 1.0 / ((math.sqrt(d_x ** 2 + d_y ** 2)) ** self.power)
+                weight = 1. / ((math.sqrt(d_x ** 2 + d_y ** 2)) ** self.power)
                 sum_weight += weight
                 sum_value += weight * z_point
 
         if z_val is None:
             z_val = sum_value / sum_weight
 
         return z_val
@@ -276,24 +282,22 @@
 
 def parse_domain(domain):
     bbox = list(map(float, domain.split(',')))
     return {
         'lng1': bbox[0],
         'lat1': bbox[1],
         'lng2': bbox[2],
-        'lat2': bbox[3],
+        'lat2': bbox[3]
     }
 
 
 def generate_html_map(filename, template_file, data, domain, resolution):
-    with open(template_file, 'r') as template:
+    with open(template_file, 'r') as template:  # noqa: SIM117
         with open(filename, 'w+') as html_file:
-            html_file.write(
-                jinja2.Template(template.read()).render(
-                    resolution=resolution,
-                    lng1=domain['lng1'],
-                    lng2=domain['lng2'],
-                    lat1=domain['lat1'],
-                    lat2=domain['lat2'],
-                    data=data,
-                )
-            )
+            html_file.write(jinja2.Template(template.read()).render(
+                resolution=resolution,
+                lng1=domain['lng1'],
+                lng2=domain['lng2'],
+                lat1=domain['lat1'],
+                lat2=domain['lat2'],
+                data=data
+            ))
```

### Comparing `metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/app/forecast/file/test-data/rainfall.csv` & `metomi-rose-2.1.0/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/app/forecast/file/test-data/rainfall.csv`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/app/forecast/file/test-data/wind_20171101T0000Z_x.csv` & `metomi-rose-2.1.0/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/app/forecast/file/test-data/wind_20171101T0000Z_x.csv`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/app/forecast/file/test-data/wind_20171101T0000Z_y.csv` & `metomi-rose-2.1.0/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/app/forecast/file/test-data/wind_20171101T0000Z_y.csv`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/app/forecast/meta/rose-meta.conf` & `metomi-rose-2.1.0/metomi/rose/etc/tutorial/rose-weather-forecasting-suite/app/forecast/meta/rose-meta.conf`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rose/etc/tutorial/test-data/rainfall.csv` & `metomi-rose-2.1.0/metomi/rose/etc/tutorial/test-data/rainfall.csv`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rose/etc/tutorial/test-data/wind_20171101T0000Z_x.csv` & `metomi-rose-2.1.0/metomi/rose/etc/tutorial/test-data/wind_20171101T0000Z_x.csv`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rose/etc/tutorial/test-data/wind_20171101T0000Z_y.csv` & `metomi-rose-2.1.0/metomi/rose/etc/tutorial/test-data/wind_20171101T0000Z_y.csv`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rose/etc/tutorial/widget/meta/lib/python/widget/username.py` & `metomi-rose-2.1.0/metomi/rose/etc/tutorial/widget/meta/lib/python/widget/username.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rose/external.py` & `metomi-rose-2.1.0/metomi/rose/external.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rose/formats/__init__.py` & `metomi-rose-2.1.0/metomi/rose/formats/__init__.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rose/formats/namelist.py` & `metomi-rose-2.1.0/metomi/rose/formats/namelist.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rose/fs_util.py` & `metomi-rose-2.1.0/metomi/rose/fs_util.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rose/host_select.py` & `metomi-rose-2.1.0/metomi/rose/host_select.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rose/host_select_client.py` & `metomi-rose-2.1.0/metomi/rose/host_select_client.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rose/job_runner.py` & `metomi-rose-2.1.0/metomi/rose/job_runner.py`

 * *Files 12% similar despite different names*

```diff
@@ -144,108 +144,119 @@
         """Update self.contextwith the values of "other.context"."""
         self.context.update(other.context)
 
 
 class JobRunner:
     """Runs JobProxy objects with pool of workers."""
 
+    ASYNC_SLEEP_TIME = 0.1
+
     def __init__(self, job_processor, nproc=None):
         """
         Initialise a job runner.
 
         job_processor: the processor of a job. Must implement a process_job()
         and a post_process_job() methods. See the run() method for detail.
 
         nproc: maximum number of processes in the pool. If None or not
         specified, use self.NPROC.
 
         """
         self.job_processor = job_processor
 
-    def run(self, job_manager, *args):
-        """
-        Start the job runner with an instance of JobManager.
+    def run(self, job_manager, *args, concurrency=6):
+        """Start the job runner with an instance of JobManager.
 
         Args:
             job_manager (JobManager):
                 A JobManager object used to handle the list of jobs to be done
-
-        Outline:
-                 +------------------+
-            +---->  job_manager.    +------------>  FINISH
-            |    |  has_jobs ?      |   No
-            |    +------------------+
-            |        |Yes
-            |    +---v--------------+
-            |    |Post-process any  |
-            |    |finished jobs     |
-            |    +---+--------------+
-            |        |
-            |    +---v--------------------------------+
-            |    |   Check for ready jobs             |
-            |    |   Add ready jobs to "awaiting"     |
-            |    +---+-------------------------^------+
-            |        |                         |
-            |    +---v---------------+         |
-            +----+ Are there any jobs|         |
-            No   | in "awaiting"?    |         |
-                 +-------------------+         |
-                     |Yes                      |
-                 +-------------------+         |
-                 | Add jobs to event |         |
-                 | loop - wait until |         |
-                 | asyncio returns   |         |
-                 | first result.     +---------+
-                 +-------------------+
+            args:
+                Arguments to pass through to jobs / post-processing.
+            concurrency:
+                The maximum number of jobs to run concurrently.
 
         """
+        running = []
         loop = asyncio.get_event_loop()
         loop.set_exception_handler(self.job_processor.handle_event)
-        results = {}
+        loop.run_until_complete(
+            asyncio.gather(
+                self._run_jobs(running, job_manager, args, concurrency),
+                self._post_process_jobs(running, job_manager, args),
+            )
+        )
+        dead_jobs = job_manager.get_dead_jobs()
+        if dead_jobs:
+            raise JobRunnerNotCompletedError(dead_jobs)
 
-        while job_manager.has_jobs():
-            # Post-process all finished jobs and handle exceptions.
-            for job_proxy, result in list(results.items()):
-                results.pop(job_proxy)
-                job_proxy.exc = result.exception()
-                job_manager.put_job(job_proxy)
-                if not job_proxy.exc:
-                    self.job_processor.post_process_job(job_proxy, *args)
-                    self.job_processor.handle_event(JobEvent(job_proxy))
-                else:
-                    self.job_processor.handle_event(job_proxy.exc)
+    async def _run_jobs(self, running, job_manager, args, concurrency):
+        """Run pending jobs subject to the concurrency limit.
+
+        This coroutine exits when there are no more jobs left to run.
 
-            awaiting = set()
+        Args:
+            running:
+                Jobs will be added to this list when run.
+            job_manager:
+                A JobManager object used to handle the list of jobs to be done
+            args:
+                Arguments to pass through to jobs / post-processing.
+            concurrency:
+                The maximum number of jobs to run concurrently.
 
-            def get_ready_jobs():
-                """Get list of jobs with satisfied dependencies"""
-                while job_manager.has_ready_jobs():
-                    job = job_manager.get_job()
-                    if job is None:
-                        break
-                    task = loop.create_task(
-                        self.job_processor.process_job(job, *args)
-                    )
-                    task.job = job
-                    awaiting.add(task)
-
-            get_ready_jobs()
-            while awaiting:
-                # Submit all tasks in awaiting to event loop, then wait until
-                # one of them completes, at which point check whether any more
-                # jobs have become ready and submit those.
-                just_completed, awaiting = loop.run_until_complete(
-                    asyncio.wait(awaiting, return_when=asyncio.FIRST_COMPLETED)
+        """
+        while job_manager.has_jobs():
+            while len(running) < concurrency:
+                # run jobs
+                job = job_manager.get_job()
+                if job is None:
+                    # we've run out of jobs for now
+                    break
+                task = asyncio.create_task(
+                    self.job_processor.process_job(job, *args)
                 )
-                results.update({task.job: task for task in just_completed})
-                get_ready_jobs()
+                task.job = job
+                running.append(task)
+            # we've hit the concurrency limit => wait
+            await asyncio.sleep(self.ASYNC_SLEEP_TIME)
 
-        dead_jobs = job_manager.get_dead_jobs()
-        if dead_jobs:
-            raise JobRunnerNotCompletedError(dead_jobs)
+    async def _post_process_jobs(self, running, job_manager, args):
+        """Post process completed jobs.
+
+        This coroutine exits when there are not more jobs left to run / post
+        process.
+
+        Args:
+            running:
+                Jobs will be added to this list when run.
+            job_manager:
+                A JobManager object used to handle the list of jobs to be done
+            args:
+                Arguments to pass through to jobs / post-processing.
+
+        """
+        while running or job_manager.has_jobs():
+            if not running:
+                # wait for more tasks to be queued
+                await asyncio.sleep(self.ASYNC_SLEEP_TIME)
+                continue
+            done, _running = await asyncio.wait(
+                running,
+                return_when=asyncio.FIRST_COMPLETED
+            )
+            for task in done:
+                running.remove(task)
+                job = task.job
+                job.exc = task.exception()
+                job_manager.put_job(job)
+                if not job.exc:
+                    self.job_processor.post_process_job(job, *args)
+                    self.job_processor.handle_event(JobEvent(job))
+                else:
+                    self.job_processor.handle_event(job.exc)
 
     __call__ = run
 
 
 class JobRunnerNotCompletedError(Exception):
     """Error raised when there are no ready/working jobs but pending ones."""
```

### Comparing `metomi-rose-2.0rc3/metomi/rose/loc_handlers/__init__.py` & `metomi-rose-2.1.0/metomi/rose/loc_handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rose/loc_handlers/fs.py` & `metomi-rose-2.1.0/metomi/rose/loc_handlers/fs.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rose/loc_handlers/namelist.py` & `metomi-rose-2.1.0/metomi/rose/loc_handlers/namelist.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rose/loc_handlers/rsync.py` & `metomi-rose-2.1.0/metomi/rose/loc_handlers/rsync.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 
     def parse(self, loc, _):
         """Set loc.scheme, loc.loc_type, loc.paths."""
         loc.scheme = "rsync"
         # Attempt to obtain the checksum(s) via "ssh"
         host, path = loc.name.split(":", 1)
         cmd = self.manager.popen.get_cmd(
-            "ssh", host, "python3", "-", path, loc.TYPE_BLOB, loc.TYPE_TREE
+            "ssh", host, "python", "-", path, loc.TYPE_BLOB, loc.TYPE_TREE
         )
         with open(rsync_remote_check_file, 'r') as stdin:
             out = self.manager.popen(*cmd, stdin=stdin)[0]
         lines = out.splitlines()
         if not lines or lines[0] not in [loc.TYPE_BLOB, loc.TYPE_TREE]:
             raise ValueError(loc.name)
         loc.loc_type = lines.pop(0)
```

### Comparing `metomi-rose-2.0rc3/metomi/rose/loc_handlers/rsync_remote_check.py` & `metomi-rose-2.1.0/metomi/rose/loc_handlers/rsync_remote_check.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,28 +21,35 @@
 
 This is a Python file but we read it and pass it to stdin
 to avoid reliance on remote platforms having rose installed.
 
 Warning:
     This script will not necessarily be run in the Rose Python environment.
     It should not have any dependencies outside of the stdlib and should be
-    compatible with as wide a range of Python3 versions as possible.
+    compatible with as wide a range of Python versions as possible.
 
 """
+from __future__ import print_function
 import os
 import sys
 
 
 def main(path, str_blob, str_tree):
     """Check file exists and print some info:
 
-    1. Octal protection bits.
-    2. Last modified time.
-    3. Filesize.
-    4. Path, which has been checked.
+    Args:
+        path (str): Path to a file or directory.
+        str_blob: return this string if path is a file. Default='blob'
+        str_tree: return this string if path is a directory. Default='tree'
+
+    Prints:
+        1. Access Mode information.
+        2. Last modified time.
+        3. Filesize.
+        4. Path, which has been checked.
     """
     if os.path.isdir(path):
         print(str_tree)
         os.chdir(path)
         for dirpath, dirnames, filenames in os.walk(path):
             good_dirnames = []
             for dirname in dirnames:
```

### Comparing `metomi-rose-2.0rc3/metomi/rose/loc_handlers/svn.py` & `metomi-rose-2.1.0/metomi/rose/loc_handlers/svn.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rose/macro.py` & `metomi-rose-2.1.0/metomi/rose/macro.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rose/macros/__init__.py` & `metomi-rose-2.1.0/metomi/rose/macros/__init__.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rose/macros/compulsory.py` & `metomi-rose-2.1.0/metomi/rose/macros/compulsory.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rose/macros/duplicate.py` & `metomi-rose-2.1.0/metomi/rose/macros/duplicate.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rose/macros/format.py` & `metomi-rose-2.1.0/metomi/rose/macros/format.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rose/macros/rule.py` & `metomi-rose-2.1.0/metomi/rose/macros/rule.py`

 * *Files 16% similar despite different names*

```diff
@@ -46,14 +46,147 @@
            .*              (?# anything)
            $               (?# the end)
          )""",
     re.X,
 )
 
 
+class Int(int):
+    """Override integer to maintain Python2 style interface
+    """
+    def __lt__(self, other):
+        """
+        Examples:
+            >>> Int(4) < Int(6)
+            True
+            >>> Int(4) < Float(6.1)
+            True
+            >>> Int(4) < Str('Zaphod Beeblebrox')
+            True
+            >>> Int(99999) < Str('Zaphod Beeblebrox')
+            True
+            >>> Int(4) < Float(-5.5)
+            False
+            >>> Int(42) < 42
+            False
+            >>> Int(77) < ''
+            False
+        """
+        try:
+            return int(self) < other
+        except TypeError:
+            return False
+
+    def __gt__(self, other):
+        """
+        Examples:
+            >>> Int(2) > Float(2.0)
+            False
+            >>> Int(3) > Float(2.0)
+            True
+        """
+        try:
+            return int(self) > other
+        except TypeError:
+            return True
+
+    def __le__(self, other):
+        return not self.__gt__(other)
+
+    def __ge__(self, other):
+        return not self.__lt__(other)
+
+
+class Float(float):
+    def __lt__(self, other):
+        """
+        Examples:
+            >>> Int(4) < Int(6)
+            True
+            >>> Int(4) < Float(6.1)
+            True
+            >>> Int(4) < Str('Zaphod Beeblebrox')
+            True
+            >>> Int(99999) < Str('Zaphod Beeblebrox')
+            True
+            >>> Int(4) < Float(-5.5)
+            False
+            >>> Int(1199) < 1199
+            False
+        """
+        try:
+            return float(self) < float(other)
+        except (TypeError, ValueError):
+            return True
+
+    def __gt__(self, other):
+        """
+        Examples:
+            >>> Int(2) > Float(2.0)
+            False
+            >>> Int(3) > Float(2.0)
+            True
+        """
+        try:
+            return float(self) > float(other)
+        except (TypeError, ValueError):
+            return False
+
+    def __le__(self, other):
+        return not self.__gt__(other)
+
+    def __ge__(self, other):
+        return not self.__lt__(other)
+
+
+class Str(str):
+    def __lt__(self, other):
+        """
+        Examples:
+            >>> Str('aardvaark') < Str('zebra')
+            True
+            >>> Str('alligator') < Int(400)
+            False
+            >>> Str('pink fairy armadillo') < 'syrian hamster'
+            True
+        """
+        if isinstance(other, (int, float, Float, Int)):
+            return False
+        elif isinstance(other, Str):
+            return str(self) < str(other)
+        else:
+            return str(self) < other
+
+    def __gt__(self, other):
+        """
+        Examples:
+            >>> Str('aardvaark') > Str('zebra')
+            False
+            >>> Str('alligator') > Int(400)
+            True
+            >>> Str('pink fairy armadillo') > 'syrian hamster'
+            False
+        """
+        if isinstance(other, (int, float, Float, Int)):
+            return True
+        elif isinstance(other, Str):
+            return str(self) > str(other)
+        else:
+            return str(self) > other
+
+    def __le__(self, other):
+        return not self.__gt__(other)
+
+    def __ge__(self, other):
+        return not self.__lt__(other)
+
+
+MYTYPES = {str: Str, int: Int, bool: Int, float: Float}
+
+
 class RuleValueError(Exception):
     def __init__(self, *args):
         self.args = args
 
     def __str__(self):
         arg_string = " ".join([str(a) for a in self.args])
         return "{0} - could not retrieve value. ".format(arg_string)
@@ -207,20 +340,28 @@
 
     def evaluate_rule(self, rule, setting_id, config, meta_config):
         """Evaluate the logic in the provided rule based on config values."""
         rule_template_str, rule_id_values = self._process_rule(
             rule, setting_id, config, meta_config
         )
         template = jinja2.Template(rule_template_str)
+
+        # Recast to our own implementations of base types to maintain
+        # Python 2 behaviour
+        for key, value in rule_id_values.items():
+            for basetype, mytype in MYTYPES.items():
+                if isinstance(value, basetype):
+                    rule_id_values[key] = mytype(rule_id_values[key])
+
         return_string = template.render(rule_id_values)
         return ast.literal_eval(return_string)
 
     def evaluate_rule_id_usage(self, rule, setting_id, meta_config):
         """Return a set of setting ids referenced in the provided rule."""
-        log_ids = set([])
+        log_ids = set()
         self._process_rule(
             rule, setting_id, None, meta_config, log_ids=log_ids
         )
         return log_ids
 
     def _process_rule(
         self, rule, setting_id, config, meta_config, log_ids=None
```

### Comparing `metomi-rose-2.0rc3/metomi/rose/macros/trigger.py` & `metomi-rose-2.1.0/metomi/rose/macros/trigger.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rose/macros/value.py` & `metomi-rose-2.1.0/metomi/rose/macros/value.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rose/meta_type.py` & `metomi-rose-2.1.0/metomi/rose/meta_type.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rose/metadata_check.py` & `metomi-rose-2.1.0/metomi/rose/metadata_check.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rose/metadata_gen.py` & `metomi-rose-2.1.0/metomi/rose/metadata_gen.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rose/metadata_graph.py` & `metomi-rose-2.1.0/metomi/rose/metadata_graph.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rose/namelist_dump.py` & `metomi-rose-2.1.0/metomi/rose/namelist_dump.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rose/opt_parse.py` & `metomi-rose-2.1.0/metomi/rose/opt_parse.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rose/popen.py` & `metomi-rose-2.1.0/metomi/rose/popen.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rose/reporter.py` & `metomi-rose-2.1.0/metomi/rose/reporter.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rose/resource.py` & `metomi-rose-2.1.0/metomi/rose/resource.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rose/rose.py` & `metomi-rose-2.1.0/metomi/rose/rose.py`

 * *Files 8% similar despite different names*

```diff
@@ -43,48 +43,52 @@
 
 # fmt: off
 DEAD_ENDS = {
     # messages to show for commands which have been removed or renamed
     # (ns, sub_cmd): message
     ('rosa', 'rpmbuild'):
         'Rosa RPM Builder has been removed.',
-    ('rose', 'config-edit'):
-        'The Rose configuration editor has been removed, use the Cylc GUI.',
-    ('rose', 'edit'):
-        'The Rose configuration editor has been removed, use the Cylc GUI.',
+    ('rose', 'config-edit'): (
+        'The Rose configuration editor has been removed. The old '
+        'Rose 2019 GUI remains compatible with Rose 2 configurations.'
+    ),
+    ('rose', 'edit'): (
+        'The Rose configuration editor has been removed. The old '
+        'Rose 2019 GUI remains compatible with Rose 2 configurations.'
+    ),
     ('rose', 'metadata-graph'):
         'This command has been removed pending re-implementation',
     ('rose', 'suite-clean'):
-        'This command has been replaced by): "cylc clean".',
+        'This command has been replaced by: "cylc clean".',
     ('rose', 'suite-cmp-vc'):
-        'This command is awaiting re-implementation in Cylc8',
+        'This command is awaiting re-implementation in Cylc 8',
     ('rose', 'suite-gcontrol'):
-        'This command has been removed): use the Cylc GUI.',
+        'This command has been removed: use the Cylc GUI.',
     ('rose', 'sgc'):
-        'This command has been removed): use the Cylc GUI.',
+        'This command has been removed: use the Cylc GUI.',
     ('rose', 'suite-hook'):
         'Command obsolete, use Cylc event handlers',
     ('rose', 'task-hook'):
         'Command obsolete, use Cylc event handlers',
     ('rose', 'suite-log-view'):
-        'This command has been removed): use the Cylc GUI.',
+        'This command has been removed: use cylc review at Cylc 7 instead.',
     ('rose', 'suite-log'):
-        'This command has been removed): use the Cylc GUI',
+        'This command has been removed: use cylc review at Cylc 7 instead.',
     ('rose', 'slv'):
-        'This command has been removed): use the Cylc GUI',
+        'This command has been removed: use cylc review at Cylc 7 instead.',
     ('rose', 'suite-restart'):
-        'This command has been replaced by): "cylc restart".',
+        'This command has been replaced by: "cylc restart".',
     ('rose', 'suite-run'):
-        'This command has been replaced by): "cylc install".',
+        'This command has been replaced by: "cylc install".',
     ('rose', 'suite-init'):
-        'This command has been replaced by): "cylc install".',
+        'This command has been replaced by: "cylc install".',
     ('rose', 'suite-scan'):
-        'This command has been replaced by): "cylc scan".',
+        'This command has been replaced by: "cylc scan".',
     ('rose', 'suite-shutdown'):
-        'This command has been replaced by): "cylc stop".',
+        'This command has been replaced by: "cylc stop".',
     ('rose', 'suite-stop'):
         'This command has been replaced by: "cylc stop".',
     ('rosie', 'disco'):
         'Rosie Disco has been disabled pending fixes at a later release.',
     ('rosie', 'go'):
         'This command has been removed pending re-implementation',
 }
```

### Comparing `metomi-rose-2.0rc3/metomi/rose/run.py` & `metomi-rose-2.1.0/metomi/rose/run.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rose/run_source_vc.py` & `metomi-rose-2.1.0/metomi/rose/run_source_vc.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rose/scheme_handler.py` & `metomi-rose-2.1.0/metomi/rose/scheme_handler.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 # -----------------------------------------------------------------------------
 """Load and select from a group of related functional classes."""
 
 
 from glob import glob
 import inspect
 import os
+from pathlib import Path
 import sys
 
 
 class SchemeHandlersManager:
     """Load and select from a group of related functional classes."""
 
     CAN_HANDLE = "can_handle"
@@ -120,7 +121,19 @@
         handler = self.get_handler(item)
         if handler:
             return handler
         for handler in self.handlers.values():
             can_handle = getattr(handler, self.can_handle, None)
             if callable(can_handle) and can_handle(item):
                 return handler
+
+    @staticmethod
+    def get_rose_path():
+        """Get path where rose handlers can be found.
+
+        n.b. At Python 3 there is no requirement to have a __init__ file
+        in a module, and therefore we need to get metomi.rose's path (where
+        there is an __init__.py) and not just metomi.
+        """
+        path = str(
+            Path(sys.modules["metomi.rose"].__file__).parent.parent.parent)
+        return path
```

### Comparing `metomi-rose-2.0rc3/metomi/rose/scripts/__init__.py` & `metomi-rose-2.1.0/metomi/rose/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rose/scripts/rosa-db-create` & `metomi-rose-2.1.0/metomi/rose/scripts/rosa-db-create`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rose/scripts/rosa-svn-post-commit` & `metomi-rose-2.1.0/metomi/rose/scripts/rosa-svn-post-commit`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rose/scripts/rosa-svn-pre-commit` & `metomi-rose-2.1.0/metomi/rose/scripts/rosa-svn-pre-commit`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rose/scripts/rosa-ws` & `metomi-rose-2.1.0/metomi/rose/scripts/rosa-ws`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rose/scripts/rose-mpi-launch` & `metomi-rose-2.1.0/metomi/rose/scripts/rose-mpi-launch`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rose/scripts/rose-tutorial` & `metomi-rose-2.1.0/metomi/rose/scripts/rose-tutorial`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rose/section.py` & `metomi-rose-2.1.0/metomi/rose/section.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rose/suite_engine_proc.py` & `metomi-rose-2.1.0/metomi/rose/suite_engine_proc.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rose/suite_engine_procs/__init__.py` & `metomi-rose-2.1.0/metomi/rose/suite_engine_procs/__init__.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rose/suite_engine_procs/cylc.py` & `metomi-rose-2.1.0/metomi/rose/suite_engine_procs/cylc.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import pwd
 from random import shuffle
 import re
 import socket
 import sqlite3
 import tarfile
 from time import sleep
-from typing import Any, List, Tuple, Union
+from typing import Any, List, Optional, Tuple
 from uuid import uuid4
 
 from metomi.rose.fs_util import FileSystemEvent
 from metomi.rose.popen import WorkflowFileNotFoundError, RosePopenError
 from metomi.rose.reporter import Reporter
 from metomi.rose.suite_engine_proc import (
     SuiteEngineProcessor,
@@ -64,15 +64,15 @@
 
         paths -- if specified, are added to the end of the path.
 
         """
         return os.path.join(cls.SUITE_DIR_REL_ROOT, suite_name, *paths)
 
     def get_suite_jobs_auths(
-        self, suite_name: str, cycle_name_tuples: Tuple[Any] = None
+        self, suite_name: str, cycle_name_tuples: Optional[Tuple[Any]] = None
     ) -> List[str]:
         """Get hosts of jobs from a Cylc workflow database.
 
         returns: list of hostname strings.
         """
         # n.b. Imports inside function to avoid dependency on Cylc and
         # Cylc-Rose is Rose is being used with a different workflow engine.
@@ -91,15 +91,15 @@
             for platform in tasks.values():
                 hosts.append(get_host_from_platform(platform))
         hosts = list(set(hosts))
         return hosts
 
     def get_task_auth(
         self, suite_name: str, task_name: str
-    ) -> Union[str, None]:
+    ) -> Optional[str]:
         """Get host for a remote task from a Cylc workflow definition.
 
         Returns: Hostname, or None if:
           - task does not run remotely.
           - task has not been defined.
           - cylc-rose is not installed(*)
```

### Comparing `metomi-rose-2.0rc3/metomi/rose/task_env.py` & `metomi-rose-2.1.0/metomi/rose/task_env.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rose/task_run.py` & `metomi-rose-2.1.0/metomi/rose/task_run.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rose/tests/conftest.py` & `metomi-rose-2.1.0/metomi/rose/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rose/tests/suite_engine_procs/test_cylc.py` & `metomi-rose-2.1.0/metomi/rose/tests/suite_engine_procs/test_cylc.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rose/tests/test_config.py` & `metomi-rose-2.1.0/metomi/rose/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rose/tests/test_date.py` & `metomi-rose-2.1.0/metomi/rose/tests/test_date.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rose/tests/test_date_cli.py` & `metomi-rose-2.1.0/metomi/rose/tests/test_date_cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,15 +16,18 @@
 # -----------------------------------------------------------------------------
 """Test the CLI for Rose Date
 """
 import pytest
 import sys
 
 from metomi.rose.date_cli import (
-    _handle_old_offsets, _handle_old_datetimes, main
+    _handle_old_offsets,
+    _handle_old_datetimes,
+    _main,
+    main,
 )
 
 
 param = pytest.param
 
 
 @pytest.mark.parametrize(
@@ -251,7 +254,30 @@
     def fake_exit(myfunc):
         return myfunc
 
     monkeypatch.setattr(sys, 'argv', args)
     monkeypatch.setattr(sys, 'exit', fake_exit)
     main()
     assert capsys.readouterr().out.split('\n')[-2] == expect
+
+
+def test_cycling_mode(monkeypatch, capsys):
+    # it should default to the gregorian calendar
+    monkeypatch.setenv('ROSE_CYCLING_MODE', '')
+    _main(['rose-date', '2000', '--offset=P360D'])
+    out, _ = capsys.readouterr()
+    # 2000 + P360D = 20001226
+    assert out.splitlines()[0] == '2000'
+
+    # it should ignore the integer cycling mode
+    monkeypatch.setenv('ROSE_CYCLING_MODE', 'integer')
+    _main(['rose-date', '2000', '--offset=P360D'])
+    out, _ = capsys.readouterr()
+    # 2000 + P360D = 20001226
+    assert out.splitlines()[0] == '2000'
+
+    # but it should switch to alternative calendars as appropriate
+    monkeypatch.setenv('ROSE_CYCLING_MODE', '360_day')
+    _main(['rose-date', '2000', '--offset=P360D'])
+    out, _ = capsys.readouterr()
+    # 2000 + P360D = 2001
+    assert out.splitlines()[0] == '2001'
```

### Comparing `metomi-rose-2.0rc3/metomi/rose/tests/test_env.py` & `metomi-rose-2.1.0/metomi/rose/tests/test_env.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rose/tests/test_env_cat.py` & `metomi-rose-2.1.0/metomi/rose/tests/test_env_cat.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rose/tests/test_host_select_client.py` & `metomi-rose-2.1.0/metomi/rose/tests/test_host_select_client.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rose/tests/test_loc_handlers_rsync_remote_check.py` & `metomi-rose-2.1.0/metomi/rose/tests/test_loc_handlers_rsync_remote_check.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rose/tests/test_popen.py` & `metomi-rose-2.1.0/metomi/rose/tests/test_popen.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rose/tests/test_resource_locator.py` & `metomi-rose-2.1.0/metomi/rose/tests/test_resource_locator.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rose/tests/test_trigger_file.py` & `metomi-rose-2.1.0/metomi/rose/tests/test_trigger_file.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rose/tests/test_unicode_utils.py` & `metomi-rose-2.1.0/metomi/rose/tests/test_unicode_utils.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rose/unicode_utils.py` & `metomi-rose-2.1.0/metomi/rose/unicode_utils.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rose/upgrade.py` & `metomi-rose-2.1.0/metomi/rose/upgrade.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rose/variable.py` & `metomi-rose-2.1.0/metomi/rose/variable.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rosie/__init__.py` & `metomi-rose-2.1.0/metomi/rosie/__init__.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rosie/db.py` & `metomi-rose-2.1.0/metomi/rosie/db.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rosie/db_create.py` & `metomi-rose-2.1.0/metomi/rosie/db_create.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rosie/graph.py` & `metomi-rose-2.1.0/metomi/rosie/graph.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rosie/lib/html/static/css/bootstrap.min.css` & `metomi-rose-2.1.0/metomi/rosie/lib/html/static/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rosie/lib/html/static/css/dataTables.bootstrap.css` & `metomi-rose-2.1.0/metomi/rosie/lib/html/static/css/dataTables.bootstrap.css`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rosie/lib/html/static/css/jquery.dataTables.css` & `metomi-rose-2.1.0/metomi/rosie/lib/html/static/css/jquery.dataTables.css`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rosie/lib/html/static/fonts/glyphicons-halflings-regular.eot` & `metomi-rose-2.1.0/metomi/rosie/lib/html/static/fonts/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rosie/lib/html/static/fonts/glyphicons-halflings-regular.svg` & `metomi-rose-2.1.0/metomi/rosie/lib/html/static/fonts/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rosie/lib/html/static/fonts/glyphicons-halflings-regular.ttf` & `metomi-rose-2.1.0/metomi/rosie/lib/html/static/fonts/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rosie/lib/html/static/fonts/glyphicons-halflings-regular.woff` & `metomi-rose-2.1.0/metomi/rosie/lib/html/static/fonts/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rosie/lib/html/static/fonts/glyphicons-halflings-regular.woff2` & `metomi-rose-2.1.0/metomi/rosie/lib/html/static/fonts/glyphicons-halflings-regular.woff2`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rosie/lib/html/static/images/sort_asc.png` & `metomi-rose-2.1.0/metomi/rosie/lib/html/static/images/sort_asc.png`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rosie/lib/html/static/images/sort_asc_disabled.png` & `metomi-rose-2.1.0/metomi/rosie/lib/html/static/images/sort_asc_disabled.png`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rosie/lib/html/static/images/sort_both.png` & `metomi-rose-2.1.0/metomi/rosie/lib/html/static/images/sort_both.png`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rosie/lib/html/static/images/sort_desc.png` & `metomi-rose-2.1.0/metomi/rosie/lib/html/static/images/sort_desc.png`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rosie/lib/html/static/images/sort_desc_disabled.png` & `metomi-rose-2.1.0/metomi/rosie/lib/html/static/images/sort_desc_disabled.png`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rosie/lib/html/static/js/bootstrap.min.js` & `metomi-rose-2.1.0/metomi/rosie/lib/html/static/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rosie/lib/html/static/js/dataTables.bootstrap.js` & `metomi-rose-2.1.0/metomi/rosie/lib/html/static/js/dataTables.bootstrap.js`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rosie/lib/html/static/js/jquery.dataTables.js` & `metomi-rose-2.1.0/metomi/rosie/lib/html/static/js/jquery.dataTables.js`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rosie/lib/html/static/js/jquery.dataTables.min.js` & `metomi-rose-2.1.0/metomi/rosie/lib/html/static/js/jquery.dataTables.min.js`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rosie/lib/html/static/js/jquery.min.js` & `metomi-rose-2.1.0/metomi/rosie/lib/html/static/js/jquery.min.js`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rosie/lib/html/static/js/livestamp.min.js` & `metomi-rose-2.1.0/metomi/rosie/lib/html/static/js/livestamp.min.js`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rosie/lib/html/static/js/moment.min.js` & `metomi-rose-2.1.0/metomi/rosie/lib/html/static/js/moment.min.js`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rosie/lib/html/static/js/rosie-disco.js` & `metomi-rose-2.1.0/metomi/rosie/lib/html/static/js/rosie-disco.js`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rosie/lib/html/static/rosie-favicon.png` & `metomi-rose-2.1.0/metomi/rosie/lib/html/static/rosie-favicon.png`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rosie/lib/html/template/rosie-disco/index.html` & `metomi-rose-2.1.0/metomi/rosie/lib/html/template/rosie-disco/index.html`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rosie/lib/html/template/rosie-disco/prefix-index.html` & `metomi-rose-2.1.0/metomi/rosie/lib/html/template/rosie-disco/prefix-index.html`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rosie/suite_id.py` & `metomi-rose-2.1.0/metomi/rosie/suite_id.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rosie/svn_hook.py` & `metomi-rose-2.1.0/metomi/rosie/svn_hook.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rosie/svn_post_commit.py` & `metomi-rose-2.1.0/metomi/rosie/svn_post_commit.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rosie/svn_pre_commit.py` & `metomi-rose-2.1.0/metomi/rosie/svn_pre_commit.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rosie/tests/test_suite_id.py` & `metomi-rose-2.1.0/metomi/rosie/tests/test_suite_id.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rosie/usertools/__init__.py` & `metomi-rose-2.1.0/metomi/rosie/usertools/__init__.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rosie/usertools/ldaptool.py` & `metomi-rose-2.1.0/metomi/rosie/usertools/ldaptool.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rosie/usertools/passwdtool.py` & `metomi-rose-2.1.0/metomi/rosie/usertools/passwdtool.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rosie/vc.py` & `metomi-rose-2.1.0/metomi/rosie/vc.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rosie/ws.py` & `metomi-rose-2.1.0/metomi/rosie/ws.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rosie/ws_client.py` & `metomi-rose-2.1.0/metomi/rosie/ws_client.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi/rosie/ws_client_auth.py` & `metomi-rose-2.1.0/metomi/rosie/ws_client_auth.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,48 +12,41 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with Rose. If not, see <http://www.gnu.org/licenses/>.
 # -----------------------------------------------------------------------------
 """The authentication manager for the Rosie web service client."""
 
+from abc import ABC, abstractmethod
 import ast
 from getpass import getpass
 import os
 import re
 import shlex
 import socket
 import sys
+from typing import Optional
 from urllib.parse import urlparse
-import warnings
 
 import metomi.rose.config
 from metomi.rose.env import env_var_process
 from metomi.rose.popen import RosePopener
 from metomi.rose.reporter import Reporter
 from metomi.rose.resource import ResourceLocator
 
 try:
-    from gi import require_version, pygtkcompat
-
-    require_version('Gtk', '3.0')  # For GTK+ >=v3 use PyGObject; v2 use PyGTK
-    require_version('Secret', '1')
-    from gi.repository import Secret
-
-    del pygtkcompat
-    GI_FLAG = True
-except (ImportError, ValueError):
-    GI_FLAG = False
-try:
-    with warnings.catch_warnings():
-        warnings.simplefilter('ignore')
-        import gtk
-    import gnomekeyring
+    import keyring
+    KEYRING_FLAG = True
 except ImportError:
-    pass
+    KEYRING_FLAG = False
+else:
+    import keyring.errors
+    # Fallback non-functional keyring - used to check if keyring.get_keyring()
+    # gives us a usable keyring:
+    from keyring.backends.fail import Keyring as NoAvailableKeyring
 
 
 class UndefinedRosiePrefixWS(Exception):
     """Raised if a prefix has no config."""
 
     def __str__(self):
         return "[rosie-id]prefix-ws.%s: configuration not defined" % self.args
@@ -74,258 +67,209 @@
     def __str__(self):
         message = "Cannot retrieve username/password: %s" % self.args[0]
         if self.args[1]:
             message += ": %s" % self.args[1]
         return message
 
 
-class GnomekeyringStore:
-
-    """Password management with gnomekeyring."""
+class BaseStore(ABC):
+    """Abstract base class for password management."""
 
     @classmethod
-    def usable(cls):
+    @abstractmethod
+    def usable(cls) -> bool:
         """Can this store be used?"""
-        if "gnomekeyring" in globals() and gnomekeyring.is_available():
-            if "gtk" in globals() and not hasattr(gtk, "application_name"):
-                gtk.application_name = "rosie.ws_client"
-            return True
-        return False
-
-    def __init__(self):
-        self.item_ids = {}
-
-    def clear_password(self, scheme, host, username):
-        """Remove the password from the cache."""
-        try:
-            if (scheme, host, username) in self.item_ids:
-                ring_id, item_id = self.item_ids[(scheme, host, username)]
-                gnomekeyring.item_delete_sync(ring_id, item_id)
-        except gnomekeyring.NoKeyringDaemonError:
-            pass
+        ...
 
-    def find_password(self, scheme, host, username):
+    @abstractmethod
+    def store_password(
+        self, scheme: str, host: str, username: str, password: str
+    ) -> None:
+        """Store the password of username@root."""
+        ...
+
+    @abstractmethod
+    def find_password(
+        self, scheme: str, host: str, username: str
+    ) -> Optional[str]:
         """Return the password of username@root."""
-        try:
-            res = gnomekeyring.find_network_password_sync(
-                username, None, host, None, scheme
-            )
-            ring_id = res[0]["keyring"]
-            item_id = res[0]["item_id"]
-            self.item_ids[(scheme, host, username)] = (ring_id, item_id)
-            return res[0]["password"]
-        except (gnomekeyring.NoMatchError, gnomekeyring.NoKeyringDaemonError):
-            return
-        except gnomekeyring.Error as exc:
-            exc_type = "gnomekeyring." + type(exc).__name__
-            exc_string = str(exc)
-            raise RosieStoreRetrievalError(exc_type, exc_string)
+        ...
 
-    def store_password(self, scheme, host, username, password):
-        """Return the password of username@root."""
-        self.clear_password(scheme, host, username)
-        try:
-            item_id = gnomekeyring.item_create_sync(
-                None,
-                gnomekeyring.ITEM_NETWORK_PASSWORD,
-                host,
-                {"user": username, "protocol": scheme, "server": host},
-                password,
-                True,
-            )
-        except (
-            gnomekeyring.CancelledError,
-            gnomekeyring.NoKeyringDaemonError,
-        ):
-            pass
-        self.item_ids[(scheme, host, username)] = (None, item_id)
+    @abstractmethod
+    def clear_password(
+        self, scheme: str, host: str, username: str
+    ) -> None:
+        """Remove the password from the cache."""
+        ...
 
 
-class GPGAgentStore:
+class GPGAgentStore(BaseStore):
 
     """Password management with gpg-agent."""
 
     RECV_BUFSIZE = 4096
 
     @classmethod
-    def usable(cls):
+    def usable(cls) -> bool:
         """Can this store be used?"""
         try:
             cls.get_socket()
         except GPGAgentStoreConnectionError:
             return False
         return True
 
     @classmethod
-    def get_socket(cls):
+    def get_socket(cls) -> socket.socket:
         """Get a connected, ready-to-use socket for gpg-agent."""
         agent_info = os.environ.get("GPG_AGENT_INFO")
         if agent_info is None:
             raise GPGAgentStoreConnectionError("no $GPG_AGENT_INFO env var")
         socket_address = agent_info.split(":")[0]
         gpg_socket = socket.socket(socket.AF_UNIX)
         try:
             gpg_socket.connect(socket_address)
         except socket.error as exc:
-            raise GPGAgentStoreConnectionError("socket error: %s" % exc)
+            raise GPGAgentStoreConnectionError(f"socket error: {exc}")
         cls._socket_receive(gpg_socket, b"^OK .*\n")
         gpg_socket.send(b"GETINFO socket_name\n")
         reply = cls._socket_receive(gpg_socket, b"^(?!OK)[^ ]+ .*\n")
         if not reply.startswith(b"D"):
-            raise GPGAgentStoreConnectionError("socket: bad reply: %r" % reply)
+            raise GPGAgentStoreConnectionError(f"socket: bad reply: {reply}")
         reply_socket_address = reply.split()[1]
-        if reply_socket_address != socket_address:
+        if reply_socket_address.decode() != socket_address:
             # The gpg-agent documentation advises making this check.
             raise GPGAgentStoreConnectionError("daemon socket mismatch")
         tty = os.environ.get("GPG_TTY")
         if tty is None:
             if not sys.stdin.isatty():
                 raise GPGAgentStoreConnectionError(
                     "no $GPG_TTY env var and failed to extrapolate it"
                 )
             tty = os.ttyname(sys.stdin.fileno())
-        gpg_socket.send(b"OPTION putenv=GPG_TTY=%s\n" % tty)
+        gpg_socket.send(f"OPTION putenv=GPG_TTY={tty}\n".encode())
         cls._socket_receive(gpg_socket, b"^OK\n")
         for name in ("TERM", "LANG", "LC_ALL", "DISPLAY"):
             val = os.environ.get(name)
             if val is not None:
-                gpg_socket.send(b"OPTION putenv=%s=%s\n" % (name, val))
+                gpg_socket.send(f"OPTION putenv={name}={val}\n".encode())
                 cls._socket_receive(gpg_socket, b"^OK\n")
         return gpg_socket
 
     @classmethod
     def _socket_receive(cls, gpg_socket, pattern):
         reply = b""
         while not reply or not re.search(pattern, reply, re.M):
             reply += gpg_socket.recv(cls.RECV_BUFSIZE)
         return reply
 
-    def __init__(self):
-        pass
-
-    def clear_password(self, scheme, host, username):
+    def clear_password(self, scheme: str, host: str, username: str) -> None:
         """Remove the password from the cache."""
         gpg_socket = self.get_socket()
-        gpg_socket.send("CLEAR_PASSPHRASE rosie:%s:%s\n" % (scheme, host))
+        gpg_socket.send(f"CLEAR_PASSPHRASE rosie:{scheme}:{host}\n".encode())
         # This command always returns 'OK', even when the cache id is invalid.
         self._socket_receive(gpg_socket, b"^OK")
 
     def find_password(self, scheme, host, username):
         """Return the password of username@root."""
         return self.get_password(scheme, host, username, no_ask=True)
 
-    def get_password(self, scheme, host, username, no_ask=False, prompt=None):
+    def get_password(
+        self,
+        scheme: str,
+        host: str,
+        username: str,
+        no_ask: bool = False,
+        prompt: Optional[str] = None
+    ) -> Optional[str]:
         """Store and retrieve the password."""
         gpg_socket = self.get_socket()
-        no_ask_option = ""
-        if no_ask:
-            no_ask_option = "--no-ask"
-        if prompt is None:
-            prompt = "X"
-        else:
-            prompt = prompt.replace(" ", "+")
+        no_ask_option = "--no-ask" if no_ask else ""
+        prompt = "X" if prompt is None else prompt.replace(" ", "+")
         gpg_socket.send(
-            "GET_PASSPHRASE --data %s rosie:%s:%s X X %s\n"
-            % (no_ask_option, scheme, host, prompt)
+            f"GET_PASSPHRASE --data {no_ask_option} "
+            f"rosie:{scheme}:{host} X X {prompt}\n"
+            .encode()
         )
         reply = self._socket_receive(gpg_socket, b"^(?!OK)[^ ]+ .*\n")
         replylines = reply.splitlines()
         for line in replylines:
-            if line.startswith("D"):
-                return line.split(None, 1)[1]
+            if line.startswith(b"D"):
+                return line.split(None, 1)[1].decode()
         if not no_ask:
             # We want gpg-agent to prompt for a password.
             for line in replylines:
                 if (
-                    line.startswith("INQUIRE ")
-                    or "Operation cancelled" in line
+                    line.startswith(b"INQUIRE ")
+                    or b"Operation cancelled" in line
                 ):
                     # Prompt was launched, or a launched prompt was cancelled.
                     return None
             # Prompt couldn't be launched.
             raise RosieStoreRetrievalError(
-                "gpg-agent", reply.replace("OK\n", "").replace("\n", " ")
+                "gpg-agent", reply.replace(b"OK\n", b"").replace(b"\n", b" ")
             )
         return None
 
     def prompt_password(self, prompt, scheme, host, username):
         """Prompt for the password of username@root."""
         return self.get_password(scheme, host, username, prompt=prompt)
 
     def store_password(self, scheme, host, username, password):
         """Store the password of username@root... but it's already stored."""
         pass
 
 
-class LibsecretStore:
+class KeyringStore(BaseStore):
+    """Password management with keyring.
 
-    """Password management with libsecret."""
+    Supports GNOME keyring & MacOS keychain among others."""
 
     @classmethod
-    def usable(cls):
-        """Can this store be used?"""
-        return bool(GI_FLAG)
-
-    def __init__(self):
-        # Attributes must be explicitly defined; not managed by the schema
-        self.category = ("protocol", "server", "user")
-        self.attributes = dict(
-            (key, Secret.SchemaAttributeType.STRING) for key in self.category
+    def usable(cls) -> bool:
+        return KEYRING_FLAG and not isinstance(
+            keyring.get_keyring(), NoAvailableKeyring
         )
-        self.schema = Secret.Schema.new(
-            "org.rosie.disco.Store", Secret.SchemaFlags.NONE, self.attributes
-        )
-
-    def clear_password(self, scheme, host, username):
-        """Remove the password from the cache."""
-        template = dict(zip(self.category, (scheme, host, username)))
-        Secret.password_clear_sync(self.schema, template, None)
 
-    def find_password(self, scheme, host, username):
-        """Return the password of username@root."""
-        template = dict(zip(self.category, (scheme, host, username)))
+    def store_password(
+        self, scheme: str, host: str, username: str, password: str
+    ) -> None:
+        keyring.set_password(host, username, password)
+
+    def find_password(
+        self, scheme: str, host: str, username: str
+    ) -> Optional[str]:
+        return keyring.get_password(host, username)
+
+    def clear_password(
+        self, scheme: str, host: str, username: str
+    ) -> None:
         try:
-            password = Secret.password_lookup_sync(self.schema, template, None)
-        except Secret.SECRET_ERROR_PROTOCOL:
-            return
-        return password
-
-    def store_password(self, scheme, host, username, password):
-        """Return the password of username@root."""
-        template = dict(zip(self.category, (scheme, host, username)))
-        self.clear_password(scheme, host, username)
-        try:
-            Secret.password_store_sync(
-                self.schema,
-                template,
-                Secret.COLLECTION_DEFAULT,
-                host,
-                password,
-                None,
-            )
-        except Secret.SECRET_ERROR_PROTOCOL:
+            keyring.delete_password(host, username)
+        except keyring.errors.PasswordDeleteError:
+            # No such password
             pass
 
 
 class RosieWSClientAuthManager:
 
     """Manage authentication info for a Rosie web service client."""
 
     ST_UNC = "UNC"  # Item is unchanged
     ST_MOD = "MOD"  # Item is modified
-    PASSWORD_STORES_STR = "gpgagent gnomekeyring libsecret"
+    PASSWORD_STORES_STR = "gpgagent keyring"
     PASSWORD_STORE_CLASSES = {
         "gpgagent": GPGAgentStore,
-        "gnomekeyring": GnomekeyringStore,
-        "libsecret": LibsecretStore,
+        "keyring": KeyringStore,
     }
     PROMPT_USERNAME = "Username for %(prefix)r - %(root)r: "
     PROMPT_PASSWORD = "Password for %(username)s at %(prefix)r - %(root)r: "
     STR_CANCELLED = "cancelled by user"
 
+    password_store: Optional[BaseStore]
+
     def __init__(
         self, prefix, popen=None, prompt_func=None, event_handler=None
     ):
         self.prefix = prefix
         root = self._get_conf_value("ws")
         if root is None:
             raise UndefinedRosiePrefixWS(self.prefix)
@@ -462,43 +406,33 @@
             )
             if self.password_orig is None:
                 self.password_orig = self.password
 
     def _prompt(self, is_retry=False):
         """Prompt for the username and password, where necessary.
 
-        Prompt with zenity or raw_input/getpass.
+        Prompt with raw_input/getpass.
 
         """
         if callable(self.prompt_func) and not hasattr(
             self.password_store, "prompt_password"
         ):
             self.username, self.password = self.prompt_func(
                 self.username, self.password, is_retry
             )
             return
 
-        icon_path = ResourceLocator.default().locate("images/rosie-icon.png")
         if is_retry:
             username = ""
 
             prompt = self.PROMPT_USERNAME % {
                 "prefix": self.prefix,
                 "root": self.root,
             }
-            if self.popen.which("zenity") and os.getenv("DISPLAY"):
-                username = self.popen.run(
-                    "zenity",
-                    "--entry",
-                    "--title=Rosie",
-                    "--window-icon=" + icon_path,
-                    "--text=" + prompt,
-                )[1].strip()
-            else:
-                username = input(prompt)
+            username = input(prompt)
             if not username:
                 raise KeyboardInterrupt(self.STR_CANCELLED)
             if username and username != self.username:
                 self.username = username
                 self._load_password(is_retry)
                 if self.password:
                     return
@@ -518,22 +452,12 @@
                     )
                 except RosieStoreRetrievalError as exc:
                     self.event_handler(exc)
                 else:
                     need_prompting = False
 
             if not password and need_prompting:
-                if self.popen.which("zenity") and os.getenv("DISPLAY"):
-                    password = self.popen.run(
-                        "zenity",
-                        "--entry",
-                        "--hide-text",
-                        "--title=Rosie",
-                        "--window-icon=" + icon_path,
-                        "--text=" + prompt,
-                    )[1].strip()
-                else:
-                    password = getpass(prompt)
+                password = getpass(prompt)
             if not password:
                 raise KeyboardInterrupt(self.STR_CANCELLED)
             if password and password != self.password:
                 self.password = password
```

### Comparing `metomi-rose-2.0rc3/metomi/rosie/ws_client_cli.py` & `metomi-rose-2.1.0/metomi/rosie/ws_client_cli.py`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi_rose.egg-info/PKG-INFO` & `metomi-rose-2.1.0/metomi_rose.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metomi-rose
-Version: 2.0rc3
+Version: 2.1.0
 Summary: Rose, a framework for meteorological suites.
 Home-page: https://metomi.github.io/rose/doc/html/index.html
 Author: British Crown (Met Office) & Contributors
 Author-email: metomi@metoffice.gov.uk
 License: GPL
 Keywords: hpc,weather-modelling,weather-model,meteorological-suites,meteorological-modelling,meteorological-models
 Platform: any
@@ -23,45 +23,41 @@
 Provides-Extra: rosa
 Provides-Extra: tests
 Provides-Extra: all
 License-File: COPYING
 
 # Rose
 
-[![Build Status](https://travis-ci.org/metomi/rose.svg?branch=master)](https://travis-ci.org/metomi/rose)
-[![Codacy Badge](https://api.codacy.com/project/badge/Grade/ad021a33e7a64b398f792305dd901795)](https://www.codacy.com/app/metomi/rose?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=metomi/rose&amp;utm_campaign=Badge_Grade)
+[![test](https://github.com/metomi/rose/actions/workflows/test.yml/badge.svg)](https://github.com/metomi/rose/actions/workflows/test.yml)
 [![DOI](https://zenodo.org/badge/6223866.svg)](https://zenodo.org/badge/latestdoi/6223866)
-[![codecov](https://codecov.io/gh/metomi/rose/branch/master/graph/badge.svg)](https://codecov.io/gh/metomi/rose)
 
 Rose: a framework for managing and running meteorological suites.
 
 ### Python 2 or Python 3 ?
 
 #### Rose 2019
 
-- Production ready
 - Python 2
 - PyGTK GUI
 - `2019.01.x` branch in the source code
 
 #### Rose 2
 
-- Release candidate
 - Python 3
 - No GUIs
 - Web-based GUIs will follow in later Rose 2 releases
 - `master` branch in the source code
 
 [Installation](http://metomi.github.io/rose/doc/html/installation.html) |
 [User Guide](http://metomi.github.io/rose/) |
 [How to Contribute](https://github.com/metomi/rose/blob/master/CONTRIBUTING.md)
 
 ## Copyright and Terms of Use
 
-Copyright (C) 2012-<span actions:bind='current-year'>2022</span> British Crown (Met Office) &amp; Contributors
+Copyright (C) 2012-<span actions:bind='current-year'>2023</span> British Crown (Met Office) &amp; Contributors
 
 Rose is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 Rose is distributed in the hope that it will be useful,
```

### Comparing `metomi-rose-2.0rc3/metomi_rose.egg-info/SOURCES.txt` & `metomi-rose-2.1.0/metomi_rose.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -98,54 +98,41 @@
 metomi/rose/etc/rose-meta/rose_bunch/HEAD/rose-meta.conf
 metomi/rose/etc/rose-meta/rose_prune/HEAD/rose-meta.conf
 metomi/rose/etc/syntax/rose-conf-mode.el
 metomi/rose/etc/syntax/rose-conf.lang
 metomi/rose/etc/syntax/rose-conf.vim
 metomi/rose/etc/syntax/rose-conf.xml
 metomi/rose/etc/tutorial/api-keys
-metomi/rose/etc/tutorial/consolidation-tutorial/.validate
-metomi/rose/etc/tutorial/consolidation-tutorial/flow.cylc
-metomi/rose/etc/tutorial/consolidation-tutorial/bin/consolidate-observations
-metomi/rose/etc/tutorial/consolidation-tutorial/bin/forecast
-metomi/rose/etc/tutorial/consolidation-tutorial/bin/get-observations
-metomi/rose/etc/tutorial/consolidation-tutorial/bin/get-rainfall
-metomi/rose/etc/tutorial/consolidation-tutorial/bin/post-process
-metomi/rose/etc/tutorial/consolidation-tutorial/lib/python/mecator.py
-metomi/rose/etc/tutorial/consolidation-tutorial/lib/python/util.py
-metomi/rose/etc/tutorial/consolidation-tutorial/lib/template/map.html
-metomi/rose/etc/tutorial/cylc-forecasting-suite/.validate
-metomi/rose/etc/tutorial/cylc-forecasting-suite/flow.cylc
-metomi/rose/etc/tutorial/cylc-forecasting-suite/bin/consolidate-observations
-metomi/rose/etc/tutorial/cylc-forecasting-suite/bin/forecast
-metomi/rose/etc/tutorial/cylc-forecasting-suite/bin/get-observations
-metomi/rose/etc/tutorial/cylc-forecasting-suite/bin/get-rainfall
-metomi/rose/etc/tutorial/cylc-forecasting-suite/bin/post-process
-metomi/rose/etc/tutorial/cylc-forecasting-suite/lib/python/mecator.py
-metomi/rose/etc/tutorial/cylc-forecasting-suite/lib/python/util.py
-metomi/rose/etc/tutorial/cylc-forecasting-suite/lib/template/map.html
+metomi/rose/etc/tutorial/cylc-forecasting-workflow/.validate
+metomi/rose/etc/tutorial/cylc-forecasting-workflow/flow.cylc
+metomi/rose/etc/tutorial/cylc-forecasting-workflow/bin/consolidate-observations
+metomi/rose/etc/tutorial/cylc-forecasting-workflow/bin/forecast
+metomi/rose/etc/tutorial/cylc-forecasting-workflow/bin/get-observations
+metomi/rose/etc/tutorial/cylc-forecasting-workflow/bin/get-rainfall
+metomi/rose/etc/tutorial/cylc-forecasting-workflow/bin/post-process
+metomi/rose/etc/tutorial/cylc-forecasting-workflow/etc/met-office-sites.dat
+metomi/rose/etc/tutorial/cylc-forecasting-workflow/etc/python-job.settings
+metomi/rose/etc/tutorial/cylc-forecasting-workflow/lib/python/mercator.py
+metomi/rose/etc/tutorial/cylc-forecasting-workflow/lib/python/util.py
+metomi/rose/etc/tutorial/cylc-forecasting-workflow/lib/template/map.html
 metomi/rose/etc/tutorial/failif-warnif/.validate
 metomi/rose/etc/tutorial/failif-warnif/rose-app.conf
 metomi/rose/etc/tutorial/failif-warnif/meta/rose-meta.conf
-metomi/rose/etc/tutorial/forecast-script/.validate
 metomi/rose/etc/tutorial/forecast-script/forecast
 metomi/rose/etc/tutorial/forecast-script/util.py
-metomi/rose/etc/tutorial/inheritance-tutorial/flow.cylc
-metomi/rose/etc/tutorial/map-template/.validate
 metomi/rose/etc/tutorial/map-template/map-template.html
 metomi/rose/etc/tutorial/metadata-tutorial/.validate
 metomi/rose/etc/tutorial/metadata-tutorial/rose-app.conf
 metomi/rose/etc/tutorial/metadata-tutorial/bin/forecast
 metomi/rose/etc/tutorial/metadata-tutorial/bin/util.py
 metomi/rose/etc/tutorial/metadata-tutorial/file/map-template.html
 metomi/rose/etc/tutorial/metadata-tutorial/file/test-data/.validate
 metomi/rose/etc/tutorial/metadata-tutorial/file/test-data/rainfall.csv
 metomi/rose/etc/tutorial/metadata-tutorial/file/test-data/wind_20171101T0000Z_x.csv
 metomi/rose/etc/tutorial/metadata-tutorial/file/test-data/wind_20171101T0000Z_y.csv
-metomi/rose/etc/tutorial/queues-tutorial/flow.cylc
-metomi/rose/etc/tutorial/retries-tutorial/flow.cylc
 metomi/rose/etc/tutorial/rose-stem/.validate
 metomi/rose/etc/tutorial/rose-stem/kgo.txt
 metomi/rose/etc/tutorial/rose-stem/rose-stem/flow.cylc
 metomi/rose/etc/tutorial/rose-stem/rose-stem/rose-suite.conf
 metomi/rose/etc/tutorial/rose-stem/src/spaceship_command.f90
 metomi/rose/etc/tutorial/rose-suite-tutorial/.validate
 metomi/rose/etc/tutorial/rose-suite-tutorial/flow.cylc
@@ -158,15 +145,17 @@
 metomi/rose/etc/tutorial/rose-suite-tutorial/app/forecast/file/test-data/wind_20171101T0000Z_x.csv
 metomi/rose/etc/tutorial/rose-suite-tutorial/app/forecast/file/test-data/wind_20171101T0000Z_y.csv
 metomi/rose/etc/tutorial/rose-suite-tutorial/app/forecast/meta/rose-meta.conf
 metomi/rose/etc/tutorial/rose-suite-tutorial/bin/consolidate-observations
 metomi/rose/etc/tutorial/rose-suite-tutorial/bin/get-observations
 metomi/rose/etc/tutorial/rose-suite-tutorial/bin/get-rainfall
 metomi/rose/etc/tutorial/rose-suite-tutorial/bin/post-process
-metomi/rose/etc/tutorial/rose-suite-tutorial/lib/python/mecator.py
+metomi/rose/etc/tutorial/rose-suite-tutorial/etc/met-office-sites.dat
+metomi/rose/etc/tutorial/rose-suite-tutorial/etc/python-job.settings
+metomi/rose/etc/tutorial/rose-suite-tutorial/lib/python/mercator.py
 metomi/rose/etc/tutorial/rose-suite-tutorial/lib/python/util.py
 metomi/rose/etc/tutorial/rose-weather-forecasting-suite/.validate
 metomi/rose/etc/tutorial/rose-weather-forecasting-suite/flow.cylc
 metomi/rose/etc/tutorial/rose-weather-forecasting-suite/rose-suite.conf
 metomi/rose/etc/tutorial/rose-weather-forecasting-suite/app/forecast/rose-app.conf
 metomi/rose/etc/tutorial/rose-weather-forecasting-suite/app/forecast/bin/forecast
 metomi/rose/etc/tutorial/rose-weather-forecasting-suite/app/forecast/bin/util.py
@@ -178,30 +167,19 @@
 metomi/rose/etc/tutorial/rose-weather-forecasting-suite/app/forecast/meta/rose-meta.conf
 metomi/rose/etc/tutorial/rose-weather-forecasting-suite/app/forecast/opt/rose-app-test.conf
 metomi/rose/etc/tutorial/rose-weather-forecasting-suite/bin/consolidate-observations
 metomi/rose/etc/tutorial/rose-weather-forecasting-suite/bin/forecast
 metomi/rose/etc/tutorial/rose-weather-forecasting-suite/bin/get-observations
 metomi/rose/etc/tutorial/rose-weather-forecasting-suite/bin/get-rainfall
 metomi/rose/etc/tutorial/rose-weather-forecasting-suite/bin/post-process
-metomi/rose/etc/tutorial/rose-weather-forecasting-suite/lib/python/mecator.py
+metomi/rose/etc/tutorial/rose-weather-forecasting-suite/etc/met-office-sites.dat
+metomi/rose/etc/tutorial/rose-weather-forecasting-suite/etc/python-job.settings
+metomi/rose/etc/tutorial/rose-weather-forecasting-suite/lib/python/mercator.py
 metomi/rose/etc/tutorial/rose-weather-forecasting-suite/lib/python/util.py
 metomi/rose/etc/tutorial/rose-weather-forecasting-suite/meta/rose-meta.conf
-metomi/rose/etc/tutorial/runtime-introduction/flow.cylc
-metomi/rose/etc/tutorial/runtime-introduction/bin/get-observations
-metomi/rose/etc/tutorial/runtime-tutorial/.validate
-metomi/rose/etc/tutorial/runtime-tutorial/flow.cylc
-metomi/rose/etc/tutorial/runtime-tutorial/runtime
-metomi/rose/etc/tutorial/runtime-tutorial/bin/consolidate-observations
-metomi/rose/etc/tutorial/runtime-tutorial/bin/forecast
-metomi/rose/etc/tutorial/runtime-tutorial/bin/get-observations
-metomi/rose/etc/tutorial/runtime-tutorial/bin/get-rainfall
-metomi/rose/etc/tutorial/runtime-tutorial/bin/post-process
-metomi/rose/etc/tutorial/runtime-tutorial/lib/python/mecator.py
-metomi/rose/etc/tutorial/runtime-tutorial/lib/python/util.py
-metomi/rose/etc/tutorial/runtime-tutorial/lib/template/map.html
 metomi/rose/etc/tutorial/test-data/.validate
 metomi/rose/etc/tutorial/test-data/rainfall.csv
 metomi/rose/etc/tutorial/test-data/wind_20171101T0000Z_x.csv
 metomi/rose/etc/tutorial/test-data/wind_20171101T0000Z_y.csv
 metomi/rose/etc/tutorial/widget/.validate
 metomi/rose/etc/tutorial/widget/rose-app.conf
 metomi/rose/etc/tutorial/widget/meta/lib/python/widget/__init__.py
@@ -238,14 +216,15 @@
 metomi/rose/tests/test_env_cat.py
 metomi/rose/tests/test_host_select_client.py
 metomi/rose/tests/test_loc_handlers_rsync_remote_check.py
 metomi/rose/tests/test_popen.py
 metomi/rose/tests/test_resource_locator.py
 metomi/rose/tests/test_trigger_file.py
 metomi/rose/tests/test_unicode_utils.py
+metomi/rose/tests/macros/test_py2_compat_types.py
 metomi/rose/tests/suite_engine_procs/test_cylc.py
 metomi/rosie/__init__.py
 metomi/rosie/db.py
 metomi/rosie/db_create.py
 metomi/rosie/graph.py
 metomi/rosie/suite_id.py
 metomi/rosie/svn_hook.py
```

### Comparing `metomi-rose-2.0rc3/metomi_rose.egg-info/entry_points.txt` & `metomi-rose-2.1.0/metomi_rose.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `metomi-rose-2.0rc3/metomi_rose.egg-info/requires.txt` & `metomi-rose-2.1.0/metomi_rose.egg-info/requires.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 aiofiles
 jinja2>=2.10.1
+keyring==23.*
 ldap3
 metomi-isodatetime==1!3.*
 psutil>=5.6.0
 requests
-sqlalchemy
+sqlalchemy==1.*
 
 [all]
 cylc-sphinx-extensions[all]>=1.2.0
 hieroglyph>=2.1.0
 setuptools>=49
 sphinx
 sphinx_rtd_theme
 sphinxcontrib-httpdomain
 sphinxcontrib-svg2pdfconverter
 pygraphviz!=1.8,>1.0
-flake8>=3.0.0
+flake8>=4.0.0
 mypy>=0.800
 pytest
 types-aiofiles
 types-setuptools
 
 [docs]
 cylc-sphinx-extensions[all]>=1.2.0
@@ -32,12 +33,12 @@
 
 [graph]
 pygraphviz!=1.8,>1.0
 
 [rosa]
 
 [tests]
-flake8>=3.0.0
+flake8>=4.0.0
 mypy>=0.800
 pytest
 types-aiofiles
 types-setuptools
```

### Comparing `metomi-rose-2.0rc3/setup.cfg` & `metomi-rose-2.1.0/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -31,19 +31,20 @@
 [options]
 packages = find_namespace:
 include_package_data = True
 python_requires = >=3.7
 install_requires = 
 	aiofiles
 	jinja2>=2.10.1
+	keyring==23.*
 	ldap3
 	metomi-isodatetime==1!3.*
 	psutil>=5.6.0
 	requests
-	sqlalchemy
+	sqlalchemy==1.*
 
 [options.packages.find]
 include = metomi*
 
 [options.extras_require]
 docs = 
 	cylc-sphinx-extensions[all]>=1.2.0
@@ -53,15 +54,15 @@
 	sphinx_rtd_theme
 	sphinxcontrib-httpdomain
 	sphinxcontrib-svg2pdfconverter
 graph = 
 	pygraphviz>1.0,!=1.8
 rosa = 
 tests = 
-	flake8>=3.0.0
+	flake8>=4.0.0
 	mypy>=0.800
 	pytest
 	types-aiofiles
 	types-setuptools
 all = 
 	%(docs)s
 	%(graph)s
```

### Comparing `metomi-rose-2.0rc3/setup.py` & `metomi-rose-2.1.0/setup.py`

 * *Files identical despite different names*

