# Comparing `tmp/blis-0.9.1.dev0.tar.gz` & `tmp/blis-0.9.1.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blis-0.9.1.dev0.tar", last modified: Thu Jul 21 18:16:00 2022, max compression
+gzip compressed data, was "blis-0.9.1.dev1.tar", last modified: Mon Aug  1 16:04:04 2022, max compression
```

## Comparing `blis-0.9.1.dev0.tar` & `blis-0.9.1.dev1.tar`

### file list

```diff
@@ -1,1761 +1,1761 @@
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.816227 blis-0.9.1.dev0/
--rw-r--r--   0 vsts      (1001) docker     (121)     2033 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (121)      170 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (121)     7728 2022-07-21 18:16:00.812227 blis-0.9.1.dev0/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (121)     6696 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.504226 blis-0.9.1.dev0/blis/
--rw-r--r--   0 vsts      (1001) docker     (121)        0 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/__init__.pxd
--rw-r--r--   0 vsts      (1001) docker     (121)       79 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.504226 blis-0.9.1.dev0/blis/_src/
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.492226 blis-0.9.1.dev0/blis/_src/config/
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.508226 blis-0.9.1.dev0/blis/_src/config/a64fx/
--rw-r--r--   0 vsts      (1001) docker     (121)     4399 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/config/a64fx/bli_a64fx_sector_cache.h
--rw-r--r--   0 vsts      (1001) docker     (121)     5804 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/config/a64fx/bli_cntx_init_a64fx.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2179 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/config/a64fx/bli_family_a64fx.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.508226 blis-0.9.1.dev0/blis/_src/config/amd64/
--rw-r--r--   0 vsts      (1001) docker     (121)     1754 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/config/amd64/bli_family_amd64.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.508226 blis-0.9.1.dev0/blis/_src/config/amd64_legacy/
--rw-r--r--   0 vsts      (1001) docker     (121)     1867 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/config/amd64_legacy/bli_family_amd64_legacy.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.508226 blis-0.9.1.dev0/blis/_src/config/arm32/
--rw-r--r--   0 vsts      (1001) docker     (121)     1850 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/config/arm32/bli_family_arm32.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.508226 blis-0.9.1.dev0/blis/_src/config/arm64/
--rw-r--r--   0 vsts      (1001) docker     (121)     2172 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/config/arm64/bli_family_arm64.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.508226 blis-0.9.1.dev0/blis/_src/config/armsve/
--rw-r--r--   0 vsts      (1001) docker     (121)     6174 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/config/armsve/bli_cntx_init_armsve.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2179 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/config/armsve/bli_family_armsve.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.508226 blis-0.9.1.dev0/blis/_src/config/bgq/
--rw-r--r--   0 vsts      (1001) docker     (121)     3097 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/config/bgq/bli_cntx_init_bgq.c
--rw-r--r--   0 vsts      (1001) docker     (121)     3211 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/config/bgq/bli_family_bgq.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.508226 blis-0.9.1.dev0/blis/_src/config/bulldozer/
--rw-r--r--   0 vsts      (1001) docker     (121)     3279 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/config/bulldozer/bli_cntx_init_bulldozer.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2835 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/config/bulldozer/bli_family_bulldozer.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.508226 blis-0.9.1.dev0/blis/_src/config/cortexa15/
--rw-r--r--   0 vsts      (1001) docker     (121)     3494 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/config/cortexa15/bli_cntx_init_cortexa15.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2938 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/config/cortexa15/bli_family_cortexa15.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.508226 blis-0.9.1.dev0/blis/_src/config/cortexa53/
--rw-r--r--   0 vsts      (1001) docker     (121)     3117 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/config/cortexa53/bli_cntx_init_cortexa53.c
--rw-r--r--   0 vsts      (1001) docker     (121)     1800 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/config/cortexa53/bli_family_cortexa53.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.508226 blis-0.9.1.dev0/blis/_src/config/cortexa57/
--rw-r--r--   0 vsts      (1001) docker     (121)     3117 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/config/cortexa57/bli_cntx_init_cortexa57.c
--rw-r--r--   0 vsts      (1001) docker     (121)     3092 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/config/cortexa57/bli_family_cortexa57.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.508226 blis-0.9.1.dev0/blis/_src/config/cortexa9/
--rw-r--r--   0 vsts      (1001) docker     (121)     3113 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/config/cortexa9/bli_cntx_init_cortexa9.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2934 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/config/cortexa9/bli_family_cortexa9.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.508226 blis-0.9.1.dev0/blis/_src/config/excavator/
--rw-r--r--   0 vsts      (1001) docker     (121)     3267 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/config/excavator/bli_cntx_init_excavator.c
--rw-r--r--   0 vsts      (1001) docker     (121)     3037 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/config/excavator/bli_family_excavator.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.508226 blis-0.9.1.dev0/blis/_src/config/firestorm/
--rw-r--r--   0 vsts      (1001) docker     (121)     5618 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/config/firestorm/bli_cntx_init_firestorm.c
--rw-r--r--   0 vsts      (1001) docker     (121)     3092 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/config/firestorm/bli_family_firestorm.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.508226 blis-0.9.1.dev0/blis/_src/config/generic/
--rw-r--r--   0 vsts      (1001) docker     (121)     1826 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/config/generic/bli_cntx_init_generic.c
--rw-r--r--   0 vsts      (1001) docker     (121)     1735 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/config/generic/bli_family_generic.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.508226 blis-0.9.1.dev0/blis/_src/config/haswell/
--rw-r--r--   0 vsts      (1001) docker     (121)     9868 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/config/haswell/bli_cntx_init_haswell.c
--rw-r--r--   0 vsts      (1001) docker     (121)     4881 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/config/haswell/bli_family_haswell.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.508226 blis-0.9.1.dev0/blis/_src/config/intel64/
--rw-r--r--   0 vsts      (1001) docker     (121)     1734 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/config/intel64/bli_family_intel64.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.508226 blis-0.9.1.dev0/blis/_src/config/intel64_no_skx/
--rw-r--r--   0 vsts      (1001) docker     (121)     1734 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/config/intel64_no_skx/bli_family_intel64.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1734 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/config/intel64_no_skx/bli_family_intel64_no_skx.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.508226 blis-0.9.1.dev0/blis/_src/config/knc/
--rw-r--r--   0 vsts      (1001) docker     (121)     3176 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/config/knc/bli_cntx_init_knc.c
--rw-r--r--   0 vsts      (1001) docker     (121)     3540 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/config/knc/bli_family_knc.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.508226 blis-0.9.1.dev0/blis/_src/config/knl/
--rw-r--r--   0 vsts      (1001) docker     (121)     5048 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/config/knl/bli_cntx_init_knl.c
--rw-r--r--   0 vsts      (1001) docker     (121)     5007 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/config/knl/bli_family_knl.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.492226 blis-0.9.1.dev0/blis/_src/config/old/
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.512226 blis-0.9.1.dev0/blis/_src/config/old/armv7a/
--rw-r--r--   0 vsts      (1001) docker     (121)     3235 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/config/old/armv7a/bli_cntx_init_armv7a.c
--rw-r--r--   0 vsts      (1001) docker     (121)     3064 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/config/old/armv7a/bli_family_armv7a.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.512226 blis-0.9.1.dev0/blis/_src/config/old/emscripten/
--rw-r--r--   0 vsts      (1001) docker     (121)     6542 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/config/old/emscripten/bli_kernel.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.512226 blis-0.9.1.dev0/blis/_src/config/old/haswellbb/
--rw-r--r--   0 vsts      (1001) docker     (121)    11201 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/config/old/haswellbb/bli_cntx_init_haswell.c
--rw-r--r--   0 vsts      (1001) docker     (121)     5296 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/config/old/haswellbb/bli_family_haswell.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.512226 blis-0.9.1.dev0/blis/_src/config/old/loongson3a/
--rw-r--r--   0 vsts      (1001) docker     (121)     6547 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/config/old/loongson3a/bli_kernel.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.512226 blis-0.9.1.dev0/blis/_src/config/old/newarch/
--rw-r--r--   0 vsts      (1001) docker     (121)     1728 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/config/old/newarch/bli_kernel.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.512226 blis-0.9.1.dev0/blis/_src/config/old/pnacl/
--rw-r--r--   0 vsts      (1001) docker     (121)     7821 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/config/old/pnacl/bli_kernel.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.512226 blis-0.9.1.dev0/blis/_src/config/penryn/
--rw-r--r--   0 vsts      (1001) docker     (121)     3401 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/config/penryn/bli_cntx_init_penryn.c
--rw-r--r--   0 vsts      (1001) docker     (121)     3162 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/config/penryn/bli_family_penryn.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.512226 blis-0.9.1.dev0/blis/_src/config/piledriver/
--rw-r--r--   0 vsts      (1001) docker     (121)     3269 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/config/piledriver/bli_cntx_init_piledriver.c
--rw-r--r--   0 vsts      (1001) docker     (121)     3023 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/config/piledriver/bli_family_piledriver.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.512226 blis-0.9.1.dev0/blis/_src/config/power10/
--rw-r--r--   0 vsts      (1001) docker     (121)     6104 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/config/power10/bli_cntx_init_power10.c
--rw-r--r--   0 vsts      (1001) docker     (121)     1838 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/config/power10/bli_family_power10.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.512226 blis-0.9.1.dev0/blis/_src/config/power7/
--rw-r--r--   0 vsts      (1001) docker     (121)     3044 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/config/power7/bli_cntx_init_power7.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2098 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/config/power7/bli_family_power7.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.512226 blis-0.9.1.dev0/blis/_src/config/power9/
--rw-r--r--   0 vsts      (1001) docker     (121)     6056 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/config/power9/bli_cntx_init_power9.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2089 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/config/power9/bli_family_power9.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.512226 blis-0.9.1.dev0/blis/_src/config/sandybridge/
--rw-r--r--   0 vsts      (1001) docker     (121)     3271 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/config/sandybridge/bli_cntx_init_sandybridge.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2812 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/config/sandybridge/bli_family_sandybridge.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.512226 blis-0.9.1.dev0/blis/_src/config/skx/
--rw-r--r--   0 vsts      (1001) docker     (121)     4776 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/config/skx/bli_cntx_init_skx.c
--rw-r--r--   0 vsts      (1001) docker     (121)     4815 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/config/skx/bli_family_skx.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.512226 blis-0.9.1.dev0/blis/_src/config/steamroller/
--rw-r--r--   0 vsts      (1001) docker     (121)     3271 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/config/steamroller/bli_cntx_init_steamroller.c
--rw-r--r--   0 vsts      (1001) docker     (121)     1861 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/config/steamroller/bli_family_steamroller.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.512226 blis-0.9.1.dev0/blis/_src/config/template/
--rw-r--r--   0 vsts      (1001) docker     (121)     4015 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/config/template/bli_cntx_init_template.c
--rw-r--r--   0 vsts      (1001) docker     (121)     1735 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/config/template/bli_family_template.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.492226 blis-0.9.1.dev0/blis/_src/config/template/kernels/
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.512226 blis-0.9.1.dev0/blis/_src/config/template/kernels/1/
--rw-r--r--   0 vsts      (1001) docker     (121)     6920 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/config/template/kernels/1/bli_axpyv_template_noopt_var1.c
--rw-r--r--   0 vsts      (1001) docker     (121)     7848 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/config/template/kernels/1/bli_dotv_template_noopt_var1.c
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.512226 blis-0.9.1.dev0/blis/_src/config/template/kernels/1f/
--rw-r--r--   0 vsts      (1001) docker     (121)    10294 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/config/template/kernels/1f/bli_axpy2v_template_noopt_var1.c
--rw-r--r--   0 vsts      (1001) docker     (121)     9443 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/config/template/kernels/1f/bli_axpyf_template_noopt_var1.c
--rw-r--r--   0 vsts      (1001) docker     (121)    11296 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/config/template/kernels/1f/bli_dotaxpyv_template_noopt_var1.c
--rw-r--r--   0 vsts      (1001) docker     (121)    14336 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/config/template/kernels/1f/bli_dotxaxpyf_template_noopt_var1.c
--rw-r--r--   0 vsts      (1001) docker     (121)    10133 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/config/template/kernels/1f/bli_dotxf_template_noopt_var1.c
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.516226 blis-0.9.1.dev0/blis/_src/config/template/kernels/3/
--rw-r--r--   0 vsts      (1001) docker     (121)     4662 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/config/template/kernels/3/bli_gemm_template_noopt_mxn.c
--rw-r--r--   0 vsts      (1001) docker     (121)     3454 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/config/template/kernels/3/bli_gemmtrsm_l_template_noopt_mxn.c
--rw-r--r--   0 vsts      (1001) docker     (121)     3453 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/config/template/kernels/3/bli_gemmtrsm_u_template_noopt_mxn.c
--rw-r--r--   0 vsts      (1001) docker     (121)     4698 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/config/template/kernels/3/bli_trsm_l_template_noopt_mxn.c
--rw-r--r--   0 vsts      (1001) docker     (121)     4709 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/config/template/kernels/3/bli_trsm_u_template_noopt_mxn.c
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.516226 blis-0.9.1.dev0/blis/_src/config/thunderx2/
--rw-r--r--   0 vsts      (1001) docker     (121)     3117 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/config/thunderx2/bli_cntx_init_thunderx2.c
--rw-r--r--   0 vsts      (1001) docker     (121)     1848 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/config/thunderx2/bli_family_thunderx2.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.516226 blis-0.9.1.dev0/blis/_src/config/x86_64/
--rw-r--r--   0 vsts      (1001) docker     (121)     1734 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/config/x86_64/bli_family_x86_64.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.516226 blis-0.9.1.dev0/blis/_src/config/x86_64_no_skx/
--rw-r--r--   0 vsts      (1001) docker     (121)     1734 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/config/x86_64_no_skx/bli_family_x86_64_no_skx.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.516226 blis-0.9.1.dev0/blis/_src/config/x86_64_no_zen2/
--rw-r--r--   0 vsts      (1001) docker     (121)     1734 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/config/x86_64_no_zen2/bli_family_x86_64_no_zen2.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.516226 blis-0.9.1.dev0/blis/_src/config/x86_64_no_zen3/
--rw-r--r--   0 vsts      (1001) docker     (121)     1734 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/config/x86_64_no_zen3/bli_family_x86_64_no_zen3.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.516226 blis-0.9.1.dev0/blis/_src/config/zen/
--rw-r--r--   0 vsts      (1001) docker     (121)    12183 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/config/zen/bli_cntx_init_zen.c
--rw-r--r--   0 vsts      (1001) docker     (121)     3328 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/config/zen/bli_family_zen.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.516226 blis-0.9.1.dev0/blis/_src/config/zen/old/
--rw-r--r--   0 vsts      (1001) docker     (121)     7542 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/config/zen/old/bli_kernel.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.516226 blis-0.9.1.dev0/blis/_src/config/zen2/
--rw-r--r--   0 vsts      (1001) docker     (121)    10835 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/config/zen2/bli_cntx_init_zen2.c
--rw-r--r--   0 vsts      (1001) docker     (121)     3827 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/config/zen2/bli_family_zen2.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.516226 blis-0.9.1.dev0/blis/_src/config/zen3/
--rw-r--r--   0 vsts      (1001) docker     (121)    11375 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/config/zen3/bli_cntx_init_zen3.c
--rw-r--r--   0 vsts      (1001) docker     (121)     3888 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/config/zen3/bli_family_zen3.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.496226 blis-0.9.1.dev0/blis/_src/frame/
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.516226 blis-0.9.1.dev0/blis/_src/frame/0/
--rw-r--r--   0 vsts      (1001) docker     (121)     1889 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/0/bli_l0.h
--rw-r--r--   0 vsts      (1001) docker     (121)     8713 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/0/bli_l0_check.c
--rw-r--r--   0 vsts      (1001) docker     (121)     3458 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/0/bli_l0_check.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2374 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/0/bli_l0_fpa.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2047 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/0/bli_l0_fpa.h
--rw-r--r--   0 vsts      (1001) docker     (121)     4120 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/0/bli_l0_ft.h
--rw-r--r--   0 vsts      (1001) docker     (121)     8572 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/0/bli_l0_oapi.c
--rw-r--r--   0 vsts      (1001) docker     (121)     3086 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/0/bli_l0_oapi.h
--rw-r--r--   0 vsts      (1001) docker     (121)     5895 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/0/bli_l0_tapi.c
--rw-r--r--   0 vsts      (1001) docker     (121)     3977 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/0/bli_l0_tapi.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.516226 blis-0.9.1.dev0/blis/_src/frame/0/copysc/
--rw-r--r--   0 vsts      (1001) docker     (121)     3760 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/0/copysc/bli_copysc.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2284 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/0/copysc/bli_copysc.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.520226 blis-0.9.1.dev0/blis/_src/frame/1/
--rw-r--r--   0 vsts      (1001) docker     (121)     2604 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/1/bli_l1v.h
--rw-r--r--   0 vsts      (1001) docker     (121)    11714 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/1/bli_l1v_check.c
--rw-r--r--   0 vsts      (1001) docker     (121)     4215 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/1/bli_l1v_check.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2314 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/1/bli_l1v_fpa.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2107 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/1/bli_l1v_fpa.h
--rw-r--r--   0 vsts      (1001) docker     (121)     5044 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/1/bli_l1v_ft.h
--rw-r--r--   0 vsts      (1001) docker     (121)     5463 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/1/bli_l1v_ft_ker.h
--rw-r--r--   0 vsts      (1001) docker     (121)     3276 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/1/bli_l1v_ker.h
--rw-r--r--   0 vsts      (1001) docker     (121)     5755 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/1/bli_l1v_ker_prot.h
--rw-r--r--   0 vsts      (1001) docker     (121)    14345 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/1/bli_l1v_oapi.c
--rw-r--r--   0 vsts      (1001) docker     (121)     4010 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/1/bli_l1v_oapi.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1976 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/1/bli_l1v_oapi_ba.c
--rw-r--r--   0 vsts      (1001) docker     (121)     1974 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/1/bli_l1v_oapi_ex.c
--rw-r--r--   0 vsts      (1001) docker     (121)     9014 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/1/bli_l1v_tapi.c
--rw-r--r--   0 vsts      (1001) docker     (121)     5014 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/1/bli_l1v_tapi.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1974 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/1/bli_l1v_tapi_ba.c
--rw-r--r--   0 vsts      (1001) docker     (121)     1972 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/1/bli_l1v_tapi_ex.c
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.492226 blis-0.9.1.dev0/blis/_src/frame/1/other/
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.520226 blis-0.9.1.dev0/blis/_src/frame/1/other/packv/
--rw-r--r--   0 vsts      (1001) docker     (121)     1692 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/1/other/packv/bli_packv.c
--rw-r--r--   0 vsts      (1001) docker     (121)     1819 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/1/other/packv/bli_packv.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2041 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/1/other/packv/bli_packv_check.c
--rw-r--r--   0 vsts      (1001) docker     (121)     1765 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/1/other/packv/bli_packv_check.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2606 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/1/other/packv/bli_packv_cntl.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2420 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/1/other/packv/bli_packv_cntl.h
--rw-r--r--   0 vsts      (1001) docker     (121)     6495 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/1/other/packv/bli_packv_init.c
--rw-r--r--   0 vsts      (1001) docker     (121)     1946 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/1/other/packv/bli_packv_init.h
--rw-r--r--   0 vsts      (1001) docker     (121)     4380 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/1/other/packv/bli_packv_int.c
--rw-r--r--   0 vsts      (1001) docker     (121)     1789 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/1/other/packv/bli_packv_int.h
--rw-r--r--   0 vsts      (1001) docker     (121)     3151 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/1/other/packv/bli_packv_unb_var1.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2084 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/1/other/packv/bli_packv_unb_var1.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.520226 blis-0.9.1.dev0/blis/_src/frame/1/other/scalv/
--rw-r--r--   0 vsts      (1001) docker     (121)     2421 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/1/other/scalv/bli_scalv_cntl.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2187 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/1/other/scalv/bli_scalv_cntl.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2812 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/1/other/scalv/bli_scalv_int.c
--rw-r--r--   0 vsts      (1001) docker     (121)     1814 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/1/other/scalv/bli_scalv_int.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.524226 blis-0.9.1.dev0/blis/_src/frame/1/other/unpackv/
--rw-r--r--   0 vsts      (1001) docker     (121)     1692 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/1/other/unpackv/bli_unpackv.c
--rw-r--r--   0 vsts      (1001) docker     (121)     1800 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/1/other/unpackv/bli_unpackv.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2199 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/1/other/unpackv/bli_unpackv_check.c
--rw-r--r--   0 vsts      (1001) docker     (121)     1767 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/1/other/unpackv/bli_unpackv_check.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2458 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/1/other/unpackv/bli_unpackv_cntl.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2463 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/1/other/unpackv/bli_unpackv_cntl.h
--rw-r--r--   0 vsts      (1001) docker     (121)     7960 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/1/other/unpackv/bli_unpackv_int.c
--rw-r--r--   0 vsts      (1001) docker     (121)     1951 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/1/other/unpackv/bli_unpackv_int.h
--rw-r--r--   0 vsts      (1001) docker     (121)     3173 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/1/other/unpackv/bli_unpackv_unb_var1.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2102 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/1/other/unpackv/bli_unpackv_unb_var1.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.524226 blis-0.9.1.dev0/blis/_src/frame/1d/
--rw-r--r--   0 vsts      (1001) docker     (121)     2264 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/1d/bli_l1d.h
--rw-r--r--   0 vsts      (1001) docker     (121)     5909 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/1d/bli_l1d_check.c
--rw-r--r--   0 vsts      (1001) docker     (121)     3030 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/1d/bli_l1d_check.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2260 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/1d/bli_l1d_fpa.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2057 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/1d/bli_l1d_fpa.h
--rw-r--r--   0 vsts      (1001) docker     (121)     4485 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/1d/bli_l1d_ft.h
--rw-r--r--   0 vsts      (1001) docker     (121)    11491 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/1d/bli_l1d_oapi.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2882 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/1d/bli_l1d_oapi.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1976 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/1d/bli_l1d_oapi_ba.c
--rw-r--r--   0 vsts      (1001) docker     (121)     1974 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/1d/bli_l1d_oapi_ex.c
--rw-r--r--   0 vsts      (1001) docker     (121)    13381 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/1d/bli_l1d_tapi.c
--rw-r--r--   0 vsts      (1001) docker     (121)     4440 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/1d/bli_l1d_tapi.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1974 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/1d/bli_l1d_tapi_ba.c
--rw-r--r--   0 vsts      (1001) docker     (121)     1972 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/1d/bli_l1d_tapi_ex.c
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.524226 blis-0.9.1.dev0/blis/_src/frame/1f/
--rw-r--r--   0 vsts      (1001) docker     (121)     2326 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/1f/bli_l1f.h
--rw-r--r--   0 vsts      (1001) docker     (121)    12540 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/1f/bli_l1f_check.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2907 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/1f/bli_l1f_check.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2159 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/1f/bli_l1f_fpa.c
--rw-r--r--   0 vsts      (1001) docker     (121)     1962 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/1f/bli_l1f_fpa.h
--rw-r--r--   0 vsts      (1001) docker     (121)     4031 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/1f/bli_l1f_ft.h
--rw-r--r--   0 vsts      (1001) docker     (121)     4464 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/1f/bli_l1f_ft_ker.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2455 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/1f/bli_l1f_ker.h
--rw-r--r--   0 vsts      (1001) docker     (121)     4065 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/1f/bli_l1f_ker_prot.h
--rw-r--r--   0 vsts      (1001) docker     (121)    12137 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/1f/bli_l1f_oapi.c
--rw-r--r--   0 vsts      (1001) docker     (121)     3142 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/1f/bli_l1f_oapi.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1976 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/1f/bli_l1f_oapi_ba.c
--rw-r--r--   0 vsts      (1001) docker     (121)     1974 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/1f/bli_l1f_oapi_ex.c
--rw-r--r--   0 vsts      (1001) docker     (121)     6386 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/1f/bli_l1f_tapi.c
--rw-r--r--   0 vsts      (1001) docker     (121)     3980 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/1f/bli_l1f_tapi.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1974 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/1f/bli_l1f_tapi_ba.c
--rw-r--r--   0 vsts      (1001) docker     (121)     1972 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/1f/bli_l1f_tapi_ex.c
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.528226 blis-0.9.1.dev0/blis/_src/frame/1m/
--rw-r--r--   0 vsts      (1001) docker     (121)     2537 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/1m/bli_l1m.h
--rw-r--r--   0 vsts      (1001) docker     (121)     5411 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/1m/bli_l1m_check.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2784 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/1m/bli_l1m_check.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2645 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/1m/bli_l1m_fpa.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2178 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/1m/bli_l1m_fpa.h
--rw-r--r--   0 vsts      (1001) docker     (121)     4045 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/1m/bli_l1m_ft.h
--rw-r--r--   0 vsts      (1001) docker     (121)     4301 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/1m/bli_l1m_ft_ker.h
--rw-r--r--   0 vsts      (1001) docker     (121)     3443 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/1m/bli_l1m_ker.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2993 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/1m/bli_l1m_ker_prot.h
--rw-r--r--   0 vsts      (1001) docker     (121)    12092 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/1m/bli_l1m_oapi.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2659 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/1m/bli_l1m_oapi.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1976 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/1m/bli_l1m_oapi_ba.c
--rw-r--r--   0 vsts      (1001) docker     (121)     1974 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/1m/bli_l1m_oapi_ex.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2256 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/1m/bli_l1m_oft_var.h
--rw-r--r--   0 vsts      (1001) docker     (121)    11871 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/1m/bli_l1m_tapi.c
--rw-r--r--   0 vsts      (1001) docker     (121)     4092 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/1m/bli_l1m_tapi.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1974 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/1m/bli_l1m_tapi_ba.c
--rw-r--r--   0 vsts      (1001) docker     (121)     1972 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/1m/bli_l1m_tapi_ex.c
--rw-r--r--   0 vsts      (1001) docker     (121)    15140 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/1m/bli_l1m_unb_var1.c
--rw-r--r--   0 vsts      (1001) docker     (121)     4104 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/1m/bli_l1m_unb_var1.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.528226 blis-0.9.1.dev0/blis/_src/frame/1m/other/
--rw-r--r--   0 vsts      (1001) docker     (121)     1702 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/1m/other/bli_scalm.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2181 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/1m/other/bli_scalm_cntl.c
--rw-r--r--   0 vsts      (1001) docker     (121)     1773 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/1m/other/bli_scalm_cntl.h
--rw-r--r--   0 vsts      (1001) docker     (121)     3356 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/1m/other/bli_scalm_int.c
--rw-r--r--   0 vsts      (1001) docker     (121)     1814 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/1m/other/bli_scalm_int.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.532226 blis-0.9.1.dev0/blis/_src/frame/1m/packm/
--rw-r--r--   0 vsts      (1001) docker     (121)     2194 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/1m/packm/bli_packm.h
--rw-r--r--   0 vsts      (1001) docker     (121)     3556 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/1m/packm/bli_packm_alloc.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2027 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/1m/packm/bli_packm_alloc.h
--rw-r--r--   0 vsts      (1001) docker     (121)    11518 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/1m/packm/bli_packm_blk_var1.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2151 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/1m/packm/bli_packm_blk_var1.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2818 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/1m/packm/bli_packm_check.c
--rw-r--r--   0 vsts      (1001) docker     (121)     1868 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/1m/packm/bli_packm_check.h
--rw-r--r--   0 vsts      (1001) docker     (121)     3221 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/1m/packm/bli_packm_cntl.c
--rw-r--r--   0 vsts      (1001) docker     (121)     3608 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/1m/packm/bli_packm_cntl.h
--rw-r--r--   0 vsts      (1001) docker     (121)     7012 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/1m/packm/bli_packm_cxk.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2119 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/1m/packm/bli_packm_cxk.h
--rw-r--r--   0 vsts      (1001) docker     (121)     4308 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/1m/packm/bli_packm_cxk_1er.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2143 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/1m/packm/bli_packm_cxk_1er.h
--rw-r--r--   0 vsts      (1001) docker     (121)     7708 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/1m/packm/bli_packm_init.c
--rw-r--r--   0 vsts      (1001) docker     (121)     1850 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/1m/packm/bli_packm_init.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2312 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/1m/packm/bli_packm_int.c
--rw-r--r--   0 vsts      (1001) docker     (121)     1831 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/1m/packm/bli_packm_int.h
--rw-r--r--   0 vsts      (1001) docker     (121)     9249 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/1m/packm/bli_packm_part.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2606 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/1m/packm/bli_packm_part.h
--rw-r--r--   0 vsts      (1001) docker     (121)     3203 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/1m/packm/bli_packm_scalar.c
--rw-r--r--   0 vsts      (1001) docker     (121)     1741 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/1m/packm/bli_packm_scalar.h
--rw-r--r--   0 vsts      (1001) docker     (121)    14125 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/1m/packm/bli_packm_struc_cxk.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2536 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/1m/packm/bli_packm_struc_cxk.h
--rw-r--r--   0 vsts      (1001) docker     (121)    15130 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/1m/packm/bli_packm_struc_cxk_1er.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2604 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/1m/packm/bli_packm_struc_cxk_1er.h
--rw-r--r--   0 vsts      (1001) docker     (121)    13475 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/1m/packm/bli_packm_struc_cxk_md.c
--rw-r--r--   0 vsts      (1001) docker     (121)     3136 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/1m/packm/bli_packm_struc_cxk_md.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2278 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/1m/packm/bli_packm_thrinfo.c
--rw-r--r--   0 vsts      (1001) docker     (121)     3058 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/1m/packm/bli_packm_thrinfo.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.532226 blis-0.9.1.dev0/blis/_src/frame/1m/unpackm/
--rw-r--r--   0 vsts      (1001) docker     (121)     1828 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/1m/unpackm/bli_unpackm.h
--rw-r--r--   0 vsts      (1001) docker     (121)     8579 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/1m/unpackm/bli_unpackm_blk_var1.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2341 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/1m/unpackm/bli_unpackm_blk_var1.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2458 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/1m/unpackm/bli_unpackm_check.c
--rw-r--r--   0 vsts      (1001) docker     (121)     1772 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/1m/unpackm/bli_unpackm_check.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2770 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/1m/unpackm/bli_unpackm_cntl.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2261 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/1m/unpackm/bli_unpackm_cntl.h
--rw-r--r--   0 vsts      (1001) docker     (121)     3079 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/1m/unpackm/bli_unpackm_cxk.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2032 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/1m/unpackm/bli_unpackm_cxk.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2559 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/1m/unpackm/bli_unpackm_int.c
--rw-r--r--   0 vsts      (1001) docker     (121)     1813 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/1m/unpackm/bli_unpackm_int.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.536226 blis-0.9.1.dev0/blis/_src/frame/2/
--rw-r--r--   0 vsts      (1001) docker     (121)     2558 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/2/bli_l2.h
--rw-r--r--   0 vsts      (1001) docker     (121)    10509 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/2/bli_l2_check.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2909 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/2/bli_l2_check.h
--rw-r--r--   0 vsts      (1001) docker     (121)     3511 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/2/bli_l2_fpa.c
--rw-r--r--   0 vsts      (1001) docker     (121)     3161 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/2/bli_l2_fpa.h
--rw-r--r--   0 vsts      (1001) docker     (121)     4694 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/2/bli_l2_ft.h
--rw-r--r--   0 vsts      (1001) docker     (121)     4447 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/2/bli_l2_ft_unb.h
--rw-r--r--   0 vsts      (1001) docker     (121)    12392 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/2/bli_l2_oapi.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2770 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/2/bli_l2_oapi.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1975 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/2/bli_l2_oapi_ba.c
--rw-r--r--   0 vsts      (1001) docker     (121)     1973 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/2/bli_l2_oapi_ex.c
--rw-r--r--   0 vsts      (1001) docker     (121)    13995 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/2/bli_l2_tapi.c
--rw-r--r--   0 vsts      (1001) docker     (121)     4661 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/2/bli_l2_tapi.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1973 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/2/bli_l2_tapi_ba.c
--rw-r--r--   0 vsts      (1001) docker     (121)     1971 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/2/bli_l2_tapi_ex.c
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.536226 blis-0.9.1.dev0/blis/_src/frame/2/gemv/
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.536226 blis-0.9.1.dev0/blis/_src/frame/2/gemv/amd/
--rw-r--r--   0 vsts      (1001) docker     (121)     5941 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/2/gemv/amd/bli_gemv_unf_var2_amd.c
--rw-r--r--   0 vsts      (1001) docker     (121)     1848 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/2/gemv/bli_gemv.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2996 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/2/gemv/bli_gemv_unb_var1.c
--rw-r--r--   0 vsts      (1001) docker     (121)     3571 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/2/gemv/bli_gemv_unb_var2.c
--rw-r--r--   0 vsts      (1001) docker     (121)     3173 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/2/gemv/bli_gemv_unf_var1.c
--rw-r--r--   0 vsts      (1001) docker     (121)     3641 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/2/gemv/bli_gemv_unf_var2.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2712 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/2/gemv/bli_gemv_var.h
--rw-r--r--   0 vsts      (1001) docker     (121)     3200 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/2/gemv/bli_gemv_var_oapi.c
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.536226 blis-0.9.1.dev0/blis/_src/frame/2/gemv/other/
--rw-r--r--   0 vsts      (1001) docker     (121)     3846 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/2/gemv/other/bli_gemv_blk_var1.c
--rw-r--r--   0 vsts      (1001) docker     (121)     3841 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/2/gemv/other/bli_gemv_blk_var2.c
--rw-r--r--   0 vsts      (1001) docker     (121)     8532 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/2/gemv/other/bli_gemv_cntl.c
--rw-r--r--   0 vsts      (1001) docker     (121)     3514 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/2/gemv/other/bli_gemv_cntl.h
--rw-r--r--   0 vsts      (1001) docker     (121)     7610 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/2/gemv/other/bli_gemv_front.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2234 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/2/gemv/other/bli_gemv_front.h
--rw-r--r--   0 vsts      (1001) docker     (121)     3611 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/2/gemv/other/bli_gemv_int.c
--rw-r--r--   0 vsts      (1001) docker     (121)     1889 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/2/gemv/other/bli_gemv_int.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.536226 blis-0.9.1.dev0/blis/_src/frame/2/ger/
--rw-r--r--   0 vsts      (1001) docker     (121)     1843 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/2/ger/bli_ger.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2769 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/2/ger/bli_ger_unb_var1.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2764 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/2/ger/bli_ger_unb_var2.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2527 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/2/ger/bli_ger_var.h
--rw-r--r--   0 vsts      (1001) docker     (121)     3026 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/2/ger/bli_ger_var_oapi.c
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.540226 blis-0.9.1.dev0/blis/_src/frame/2/ger/other/
--rw-r--r--   0 vsts      (1001) docker     (121)     3813 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/2/ger/other/bli_ger_blk_var1.c
--rw-r--r--   0 vsts      (1001) docker     (121)     3812 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/2/ger/other/bli_ger_blk_var2.c
--rw-r--r--   0 vsts      (1001) docker     (121)     7748 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/2/ger/other/bli_ger_cntl.c
--rw-r--r--   0 vsts      (1001) docker     (121)     3093 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/2/ger/other/bli_ger_cntl.h
--rw-r--r--   0 vsts      (1001) docker     (121)     5782 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/2/ger/other/bli_ger_front.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2187 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/2/ger/other/bli_ger_front.h
--rw-r--r--   0 vsts      (1001) docker     (121)     4430 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/2/ger/other/bli_ger_int.c
--rw-r--r--   0 vsts      (1001) docker     (121)     1926 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/2/ger/other/bli_ger_int.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.540226 blis-0.9.1.dev0/blis/_src/frame/2/hemv/
--rw-r--r--   0 vsts      (1001) docker     (121)     1848 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/2/hemv/bli_hemv.h
--rw-r--r--   0 vsts      (1001) docker     (121)     4873 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/2/hemv/bli_hemv_unb_var1.c
--rw-r--r--   0 vsts      (1001) docker     (121)     4923 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/2/hemv/bli_hemv_unb_var2.c
--rw-r--r--   0 vsts      (1001) docker     (121)     4869 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/2/hemv/bli_hemv_unb_var3.c
--rw-r--r--   0 vsts      (1001) docker     (121)     4802 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/2/hemv/bli_hemv_unb_var4.c
--rw-r--r--   0 vsts      (1001) docker     (121)     6147 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/2/hemv/bli_hemv_unf_var1.c
--rw-r--r--   0 vsts      (1001) docker     (121)     4727 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/2/hemv/bli_hemv_unf_var1a.c
--rw-r--r--   0 vsts      (1001) docker     (121)     6153 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/2/hemv/bli_hemv_unf_var3.c
--rw-r--r--   0 vsts      (1001) docker     (121)     4723 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/2/hemv/bli_hemv_unf_var3a.c
--rw-r--r--   0 vsts      (1001) docker     (121)     3076 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/2/hemv/bli_hemv_var.h
--rw-r--r--   0 vsts      (1001) docker     (121)     3362 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/2/hemv/bli_hemv_var_oapi.c
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.540226 blis-0.9.1.dev0/blis/_src/frame/2/hemv/other/
--rw-r--r--   0 vsts      (1001) docker     (121)     5832 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/2/hemv/other/bli_hemv_blk_var1.c
--rw-r--r--   0 vsts      (1001) docker     (121)     5947 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/2/hemv/other/bli_hemv_blk_var2.c
--rw-r--r--   0 vsts      (1001) docker     (121)     5832 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/2/hemv/other/bli_hemv_blk_var3.c
--rw-r--r--   0 vsts      (1001) docker     (121)     5943 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/2/hemv/other/bli_hemv_blk_var4.c
--rw-r--r--   0 vsts      (1001) docker     (121)     7588 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/2/hemv/other/bli_hemv_cntl.c
--rw-r--r--   0 vsts      (1001) docker     (121)     3772 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/2/hemv/other/bli_hemv_cntl.h
--rw-r--r--   0 vsts      (1001) docker     (121)     7341 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/2/hemv/other/bli_hemv_front.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2312 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/2/hemv/other/bli_hemv_front.h
--rw-r--r--   0 vsts      (1001) docker     (121)     4260 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/2/hemv/other/bli_hemv_int.c
--rw-r--r--   0 vsts      (1001) docker     (121)     1932 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/2/hemv/other/bli_hemv_int.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.544226 blis-0.9.1.dev0/blis/_src/frame/2/her/
--rw-r--r--   0 vsts      (1001) docker     (121)     1843 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/2/her/bli_her.h
--rw-r--r--   0 vsts      (1001) docker     (121)     4843 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/2/her/bli_her_unb_var1.c
--rw-r--r--   0 vsts      (1001) docker     (121)     4845 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/2/her/bli_her_unb_var2.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2581 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/2/her/bli_her_var.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2858 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/2/her/bli_her_var_oapi.c
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.544226 blis-0.9.1.dev0/blis/_src/frame/2/her/other/
--rw-r--r--   0 vsts      (1001) docker     (121)     4773 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/2/her/other/bli_her_blk_var1.c
--rw-r--r--   0 vsts      (1001) docker     (121)     4773 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/2/her/other/bli_her_blk_var2.c
--rw-r--r--   0 vsts      (1001) docker     (121)     5599 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/2/her/other/bli_her_cntl.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2986 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/2/her/other/bli_her_cntl.h
--rw-r--r--   0 vsts      (1001) docker     (121)     5883 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/2/her/other/bli_her_front.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2141 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/2/her/other/bli_her_front.h
--rw-r--r--   0 vsts      (1001) docker     (121)     3696 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/2/her/other/bli_her_int.c
--rw-r--r--   0 vsts      (1001) docker     (121)     1864 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/2/her/other/bli_her_int.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.544226 blis-0.9.1.dev0/blis/_src/frame/2/her2/
--rw-r--r--   0 vsts      (1001) docker     (121)     1847 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/2/her2/bli_her2.h
--rw-r--r--   0 vsts      (1001) docker     (121)     5417 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/2/her2/bli_her2_unb_var1.c
--rw-r--r--   0 vsts      (1001) docker     (121)     5655 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/2/her2/bli_her2_unb_var2.c
--rw-r--r--   0 vsts      (1001) docker     (121)     5653 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/2/her2/bli_her2_unb_var3.c
--rw-r--r--   0 vsts      (1001) docker     (121)     5623 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/2/her2/bli_her2_unb_var4.c
--rw-r--r--   0 vsts      (1001) docker     (121)     5352 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/2/her2/bli_her2_unf_var1.c
--rw-r--r--   0 vsts      (1001) docker     (121)     5560 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/2/her2/bli_her2_unf_var4.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2925 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/2/her2/bli_her2_var.h
--rw-r--r--   0 vsts      (1001) docker     (121)     3226 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/2/her2/bli_her2_var_oapi.c
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.544226 blis-0.9.1.dev0/blis/_src/frame/2/her2/other/
--rw-r--r--   0 vsts      (1001) docker     (121)     5699 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/2/her2/other/bli_her2_blk_var1.c
--rw-r--r--   0 vsts      (1001) docker     (121)     5810 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/2/her2/other/bli_her2_blk_var2.c
--rw-r--r--   0 vsts      (1001) docker     (121)     5810 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/2/her2/other/bli_her2_blk_var3.c
--rw-r--r--   0 vsts      (1001) docker     (121)     5699 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/2/her2/other/bli_her2_blk_var4.c
--rw-r--r--   0 vsts      (1001) docker     (121)     6294 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/2/her2/other/bli_her2_cntl.c
--rw-r--r--   0 vsts      (1001) docker     (121)     3320 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/2/her2/other/bli_her2_cntl.h
--rw-r--r--   0 vsts      (1001) docker     (121)     6795 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/2/her2/other/bli_her2_front.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2202 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/2/her2/other/bli_her2_front.h
--rw-r--r--   0 vsts      (1001) docker     (121)     4572 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/2/her2/other/bli_her2_int.c
--rw-r--r--   0 vsts      (1001) docker     (121)     1939 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/2/her2/other/bli_her2_int.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.544226 blis-0.9.1.dev0/blis/_src/frame/2/symv/
--rw-r--r--   0 vsts      (1001) docker     (121)     1764 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/2/symv/bli_symv.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.544226 blis-0.9.1.dev0/blis/_src/frame/2/symv/other/
--rw-r--r--   0 vsts      (1001) docker     (121)     7348 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/2/symv/other/bli_symv_front.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2238 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/2/symv/other/bli_symv_front.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.544226 blis-0.9.1.dev0/blis/_src/frame/2/syr/
--rw-r--r--   0 vsts      (1001) docker     (121)     1763 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/2/syr/bli_syr.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.544226 blis-0.9.1.dev0/blis/_src/frame/2/syr/other/
--rw-r--r--   0 vsts      (1001) docker     (121)     6000 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/2/syr/other/bli_syr_front.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2124 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/2/syr/other/bli_syr_front.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.548226 blis-0.9.1.dev0/blis/_src/frame/2/syr2/
--rw-r--r--   0 vsts      (1001) docker     (121)     1764 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/2/syr2/bli_syr2.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.548226 blis-0.9.1.dev0/blis/_src/frame/2/syr2/other/
--rw-r--r--   0 vsts      (1001) docker     (121)     6514 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/2/syr2/other/bli_syr2_front.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2202 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/2/syr2/other/bli_syr2_front.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.548226 blis-0.9.1.dev0/blis/_src/frame/2/trmv/
--rw-r--r--   0 vsts      (1001) docker     (121)     1848 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/2/trmv/bli_trmv.h
--rw-r--r--   0 vsts      (1001) docker     (121)     4522 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/2/trmv/bli_trmv_unb_var1.c
--rw-r--r--   0 vsts      (1001) docker     (121)     4492 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/2/trmv/bli_trmv_unb_var2.c
--rw-r--r--   0 vsts      (1001) docker     (121)     6383 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/2/trmv/bli_trmv_unf_var1.c
--rw-r--r--   0 vsts      (1001) docker     (121)     6286 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/2/trmv/bli_trmv_unf_var2.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2676 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/2/trmv/bli_trmv_var.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2954 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/2/trmv/bli_trmv_var_oapi.c
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.548226 blis-0.9.1.dev0/blis/_src/frame/2/trmv/other/
--rw-r--r--   0 vsts      (1001) docker     (121)     6176 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/2/trmv/other/bli_trmv_cntl.c
--rw-r--r--   0 vsts      (1001) docker     (121)     3176 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/2/trmv/other/bli_trmv_cntl.h
--rw-r--r--   0 vsts      (1001) docker     (121)     5970 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/2/trmv/other/bli_trmv_front.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2152 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/2/trmv/other/bli_trmv_front.h
--rw-r--r--   0 vsts      (1001) docker     (121)     5135 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/2/trmv/other/bli_trmv_int.c
--rw-r--r--   0 vsts      (1001) docker     (121)     1836 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/2/trmv/other/bli_trmv_int.h
--rw-r--r--   0 vsts      (1001) docker     (121)     4157 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/2/trmv/other/bli_trmv_l_blk_var1.c
--rw-r--r--   0 vsts      (1001) docker     (121)     4157 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/2/trmv/other/bli_trmv_l_blk_var2.c
--rw-r--r--   0 vsts      (1001) docker     (121)     4157 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/2/trmv/other/bli_trmv_u_blk_var1.c
--rw-r--r--   0 vsts      (1001) docker     (121)     4157 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/2/trmv/other/bli_trmv_u_blk_var2.c
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.548226 blis-0.9.1.dev0/blis/_src/frame/2/trsv/
--rw-r--r--   0 vsts      (1001) docker     (121)     1848 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/2/trsv/bli_trsv.h
--rw-r--r--   0 vsts      (1001) docker     (121)     4520 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/2/trsv/bli_trsv_unb_var1.c
--rw-r--r--   0 vsts      (1001) docker     (121)     4500 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/2/trsv/bli_trsv_unb_var2.c
--rw-r--r--   0 vsts      (1001) docker     (121)     6413 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/2/trsv/bli_trsv_unf_var1.c
--rw-r--r--   0 vsts      (1001) docker     (121)     6332 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/2/trsv/bli_trsv_unf_var2.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2676 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/2/trsv/bli_trsv_var.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2954 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/2/trsv/bli_trsv_var_oapi.c
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.552226 blis-0.9.1.dev0/blis/_src/frame/2/trsv/other/
--rw-r--r--   0 vsts      (1001) docker     (121)     6639 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/2/trsv/other/bli_trsv_cntl.c
--rw-r--r--   0 vsts      (1001) docker     (121)     3314 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/2/trsv/other/bli_trsv_cntl.h
--rw-r--r--   0 vsts      (1001) docker     (121)     5694 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/2/trsv/other/bli_trsv_front.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2151 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/2/trsv/other/bli_trsv_front.h
--rw-r--r--   0 vsts      (1001) docker     (121)     5136 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/2/trsv/other/bli_trsv_int.c
--rw-r--r--   0 vsts      (1001) docker     (121)     1836 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/2/trsv/other/bli_trsv_int.h
--rw-r--r--   0 vsts      (1001) docker     (121)     4269 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/2/trsv/other/bli_trsv_l_blk_var1.c
--rw-r--r--   0 vsts      (1001) docker     (121)     4269 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/2/trsv/other/bli_trsv_l_blk_var2.c
--rw-r--r--   0 vsts      (1001) docker     (121)     4269 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/2/trsv/other/bli_trsv_u_blk_var1.c
--rw-r--r--   0 vsts      (1001) docker     (121)     4269 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/2/trsv/other/bli_trsv_u_blk_var2.c
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.556226 blis-0.9.1.dev0/blis/_src/frame/3/
--rw-r--r--   0 vsts      (1001) docker     (121)     3216 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/3/bli_l3.h
--rw-r--r--   0 vsts      (1001) docker     (121)    10637 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/3/bli_l3_blocksize.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2752 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/3/bli_l3_blocksize.h
--rw-r--r--   0 vsts      (1001) docker     (121)    13347 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/3/bli_l3_check.c
--rw-r--r--   0 vsts      (1001) docker     (121)     3886 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/3/bli_l3_check.h
--rw-r--r--   0 vsts      (1001) docker     (121)     3673 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/3/bli_l3_cntl.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2163 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/3/bli_l3_cntl.h
--rw-r--r--   0 vsts      (1001) docker     (121)     3860 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/3/bli_l3_direct.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2117 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/3/bli_l3_direct.h
--rw-r--r--   0 vsts      (1001) docker     (121)     3271 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/3/bli_l3_ft_ukr.h
--rw-r--r--   0 vsts      (1001) docker     (121)     7843 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/3/bli_l3_ind.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2803 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/3/bli_l3_ind.h
--rw-r--r--   0 vsts      (1001) docker     (121)     3245 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/3/bli_l3_ind_ukr.h
--rw-r--r--   0 vsts      (1001) docker     (121)     4697 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/3/bli_l3_int.c
--rw-r--r--   0 vsts      (1001) docker     (121)     1890 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/3/bli_l3_int.h
--rw-r--r--   0 vsts      (1001) docker     (121)     3339 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/3/bli_l3_oapi.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2801 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/3/bli_l3_oapi.h
--rw-r--r--   0 vsts      (1001) docker     (121)    17009 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/3/bli_l3_oapi_ex.c
--rw-r--r--   0 vsts      (1001) docker     (121)     3050 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/3/bli_l3_oapi_ex.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2949 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/3/bli_l3_oft.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2059 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/3/bli_l3_oft_var.h
--rw-r--r--   0 vsts      (1001) docker     (121)     3329 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/3/bli_l3_packab.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2025 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/3/bli_l3_packab.h
--rw-r--r--   0 vsts      (1001) docker     (121)     6159 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/3/bli_l3_prune.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2398 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/3/bli_l3_prune.h
--rw-r--r--   0 vsts      (1001) docker     (121)     3207 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/3/bli_l3_schema.c
--rw-r--r--   0 vsts      (1001) docker     (121)     1786 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/3/bli_l3_schema.h
--rw-r--r--   0 vsts      (1001) docker     (121)     7134 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/3/bli_l3_sup.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2020 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/3/bli_l3_sup.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2470 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/3/bli_l3_sup_ft_ker.h
--rw-r--r--   0 vsts      (1001) docker     (121)    14424 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/3/bli_l3_sup_int.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2079 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/3/bli_l3_sup_int.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2371 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/3/bli_l3_sup_ker.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2325 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/3/bli_l3_sup_ker_prot.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2081 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/3/bli_l3_sup_oft.h
--rw-r--r--   0 vsts      (1001) docker     (121)    12622 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/3/bli_l3_sup_packm_a.c
--rw-r--r--   0 vsts      (1001) docker     (121)     4037 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/3/bli_l3_sup_packm_a.h
--rw-r--r--   0 vsts      (1001) docker     (121)    12643 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/3/bli_l3_sup_packm_b.c
--rw-r--r--   0 vsts      (1001) docker     (121)     4037 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/3/bli_l3_sup_packm_b.h
--rw-r--r--   0 vsts      (1001) docker     (121)    15254 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/3/bli_l3_sup_packm_var.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2866 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/3/bli_l3_sup_packm_var.h
--rw-r--r--   0 vsts      (1001) docker     (121)     5512 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/3/bli_l3_sup_ref.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2028 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/3/bli_l3_sup_ref.h
--rw-r--r--   0 vsts      (1001) docker     (121)    22400 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/3/bli_l3_sup_var12.c
--rw-r--r--   0 vsts      (1001) docker     (121)    46064 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/3/bli_l3_sup_var1n2m.c
--rw-r--r--   0 vsts      (1001) docker     (121)     6284 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/3/bli_l3_sup_vars.h
--rw-r--r--   0 vsts      (1001) docker     (121)     8312 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/3/bli_l3_tapi.c
--rw-r--r--   0 vsts      (1001) docker     (121)     5401 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/3/bli_l3_tapi.h
--rw-r--r--   0 vsts      (1001) docker     (121)    15114 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/3/bli_l3_tapi_ex.c
--rw-r--r--   0 vsts      (1001) docker     (121)     5918 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/3/bli_l3_tapi_ex.h
--rw-r--r--   0 vsts      (1001) docker     (121)    22929 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/3/bli_l3_thrinfo.c
--rw-r--r--   0 vsts      (1001) docker     (121)     4287 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/3/bli_l3_thrinfo.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2350 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/3/bli_l3_ukr.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2171 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/3/bli_l3_ukr_fpa.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2031 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/3/bli_l3_ukr_fpa.h
--rw-r--r--   0 vsts      (1001) docker     (121)     7006 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/3/bli_l3_ukr_oapi.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2488 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/3/bli_l3_ukr_oapi.h
--rw-r--r--   0 vsts      (1001) docker     (121)     3062 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/3/bli_l3_ukr_prot.h
--rw-r--r--   0 vsts      (1001) docker     (121)     4595 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/3/bli_l3_ukr_tapi.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2165 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/3/bli_l3_ukr_tapi.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.560226 blis-0.9.1.dev0/blis/_src/frame/3/gemm/
--rw-r--r--   0 vsts      (1001) docker     (121)     1873 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/3/gemm/bli_gemm.h
--rw-r--r--   0 vsts      (1001) docker     (121)     3075 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/3/gemm/bli_gemm_blk_var1.c
--rw-r--r--   0 vsts      (1001) docker     (121)     3075 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/3/gemm/bli_gemm_blk_var2.c
--rw-r--r--   0 vsts      (1001) docker     (121)     4386 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/3/gemm/bli_gemm_blk_var3.c
--rw-r--r--   0 vsts      (1001) docker     (121)     7864 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/3/gemm/bli_gemm_cntl.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2656 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/3/gemm/bli_gemm_cntl.h
--rw-r--r--   0 vsts      (1001) docker     (121)     9834 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/3/gemm/bli_gemm_front.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2082 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/3/gemm/bli_gemm_front.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2226 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/3/gemm/bli_gemm_ker_var1.c
--rw-r--r--   0 vsts      (1001) docker     (121)    11371 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/3/gemm/bli_gemm_ker_var2.c
--rw-r--r--   0 vsts      (1001) docker     (121)    21475 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/3/gemm/bli_gemm_md.c
--rw-r--r--   0 vsts      (1001) docker     (121)     9304 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/3/gemm/bli_gemm_md.h
--rw-r--r--   0 vsts      (1001) docker     (121)     8532 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/3/gemm/bli_gemm_md_c2r_ref.c
--rw-r--r--   0 vsts      (1001) docker     (121)     1891 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/3/gemm/bli_gemm_md_c2r_ref.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2250 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/3/gemm/bli_gemm_var.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.560226 blis-0.9.1.dev0/blis/_src/frame/3/gemm/ind/
--rw-r--r--   0 vsts      (1001) docker     (121)     2759 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/3/gemm/ind/bli_gemm_ind_opt.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.560226 blis-0.9.1.dev0/blis/_src/frame/3/gemm/other/
--rw-r--r--   0 vsts      (1001) docker     (121)    10817 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/3/gemm/other/bli_gemm_ker_var2.c
--rw-r--r--   0 vsts      (1001) docker     (121)    11414 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/3/gemm/other/bli_gemm_ker_var2rr.c
--rw-r--r--   0 vsts      (1001) docker     (121)    11408 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/3/gemm/other/bli_gemm_ker_var2sl.c
--rw-r--r--   0 vsts      (1001) docker     (121)    10206 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/3/gemm/other/bli_gemm_ker_var5.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2619 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/3/gemm/other/bli_gemm_ker_var5.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.560226 blis-0.9.1.dev0/blis/_src/frame/3/gemmt/
--rw-r--r--   0 vsts      (1001) docker     (121)     1726 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/3/gemmt/bli_gemmt.h
--rw-r--r--   0 vsts      (1001) docker     (121)     4173 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/3/gemmt/bli_gemmt_front.c
--rw-r--r--   0 vsts      (1001) docker     (121)     1920 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/3/gemmt/bli_gemmt_front.h
--rw-r--r--   0 vsts      (1001) docker     (121)    16264 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/3/gemmt/bli_gemmt_l_ker_var2.c
--rw-r--r--   0 vsts      (1001) docker     (121)    16500 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/3/gemmt/bli_gemmt_u_ker_var2.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2856 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/3/gemmt/bli_gemmt_var.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2386 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/3/gemmt/bli_gemmt_x_ker_var2.c
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.560226 blis-0.9.1.dev0/blis/_src/frame/3/gemmt/other/
--rw-r--r--   0 vsts      (1001) docker     (121)    12337 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/3/gemmt/other/bli_gemmt_l_ker_var2.c
--rw-r--r--   0 vsts      (1001) docker     (121)    12339 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/3/gemmt/other/bli_gemmt_u_ker_var2.c
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.560226 blis-0.9.1.dev0/blis/_src/frame/3/hemm/
--rw-r--r--   0 vsts      (1001) docker     (121)     1702 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/3/hemm/bli_hemm.h
--rw-r--r--   0 vsts      (1001) docker     (121)     6134 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/3/hemm/bli_hemm_front.c
--rw-r--r--   0 vsts      (1001) docker     (121)     1888 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/3/hemm/bli_hemm_front.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.568226 blis-0.9.1.dev0/blis/_src/frame/3/old/
--rw-r--r--   0 vsts      (1001) docker     (121)     5944 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/3/old/bli_l3_ft_ex.h
--rw-r--r--   0 vsts      (1001) docker     (121)     4010 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/3/old/bli_l3_sup_edge.h
--rw-r--r--   0 vsts      (1001) docker     (121)    24752 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/3/old/bli_l3_sup_var1n2m.c
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.568226 blis-0.9.1.dev0/blis/_src/frame/3/symm/
--rw-r--r--   0 vsts      (1001) docker     (121)     1702 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/3/symm/bli_symm.h
--rw-r--r--   0 vsts      (1001) docker     (121)     6098 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/3/symm/bli_symm_front.c
--rw-r--r--   0 vsts      (1001) docker     (121)     1888 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/3/symm/bli_symm_front.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.568226 blis-0.9.1.dev0/blis/_src/frame/3/trmm/
--rw-r--r--   0 vsts      (1001) docker     (121)     1729 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/3/trmm/bli_trmm.h
--rw-r--r--   0 vsts      (1001) docker     (121)     7019 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/3/trmm/bli_trmm_front.c
--rw-r--r--   0 vsts      (1001) docker     (121)     1849 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/3/trmm/bli_trmm_front.h
--rw-r--r--   0 vsts      (1001) docker     (121)    13048 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/3/trmm/bli_trmm_ll_ker_var2.c
--rw-r--r--   0 vsts      (1001) docker     (121)    13206 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/3/trmm/bli_trmm_lu_ker_var2.c
--rw-r--r--   0 vsts      (1001) docker     (121)    15154 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/3/trmm/bli_trmm_rl_ker_var2.c
--rw-r--r--   0 vsts      (1001) docker     (121)    16080 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/3/trmm/bli_trmm_ru_ker_var2.c
--rw-r--r--   0 vsts      (1001) docker     (121)     3054 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/3/trmm/bli_trmm_var.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2835 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/3/trmm/bli_trmm_xx_ker_var2.c
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.568226 blis-0.9.1.dev0/blis/_src/frame/3/trmm/other/
--rw-r--r--   0 vsts      (1001) docker     (121)    16003 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/3/trmm/other/bli_trmm_ll_ker_var2.c
--rw-r--r--   0 vsts      (1001) docker     (121)    16941 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/3/trmm/other/bli_trmm_ll_ker_var2rr.c
--rw-r--r--   0 vsts      (1001) docker     (121)    16933 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/3/trmm/other/bli_trmm_ll_ker_var2sl.c
--rw-r--r--   0 vsts      (1001) docker     (121)    16175 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/3/trmm/other/bli_trmm_lu_ker_var2.c
--rw-r--r--   0 vsts      (1001) docker     (121)    17053 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/3/trmm/other/bli_trmm_lu_ker_var2rr.c
--rw-r--r--   0 vsts      (1001) docker     (121)    17046 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/3/trmm/other/bli_trmm_lu_ker_var2sl.c
--rw-r--r--   0 vsts      (1001) docker     (121)    16489 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/3/trmm/other/bli_trmm_rl_ker_var2.c
--rw-r--r--   0 vsts      (1001) docker     (121)    18922 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/3/trmm/other/bli_trmm_rl_ker_var2rr.c
--rw-r--r--   0 vsts      (1001) docker     (121)    18915 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/3/trmm/other/bli_trmm_rl_ker_var2sl.c
--rw-r--r--   0 vsts      (1001) docker     (121)    16500 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/3/trmm/other/bli_trmm_ru_ker_var2.c
--rw-r--r--   0 vsts      (1001) docker     (121)    19844 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/3/trmm/other/bli_trmm_ru_ker_var2rr.c
--rw-r--r--   0 vsts      (1001) docker     (121)    19837 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/3/trmm/other/bli_trmm_ru_ker_var2sl.c
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.568226 blis-0.9.1.dev0/blis/_src/frame/3/trmm3/
--rw-r--r--   0 vsts      (1001) docker     (121)     1703 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/3/trmm3/bli_trmm3.h
--rw-r--r--   0 vsts      (1001) docker     (121)     6378 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/3/trmm3/bli_trmm3_front.c
--rw-r--r--   0 vsts      (1001) docker     (121)     1889 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/3/trmm3/bli_trmm3_front.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.572226 blis-0.9.1.dev0/blis/_src/frame/3/trsm/
--rw-r--r--   0 vsts      (1001) docker     (121)     1755 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/3/trsm/bli_trsm.h
--rw-r--r--   0 vsts      (1001) docker     (121)     6318 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/3/trsm/bli_trsm_blk_var1.c
--rw-r--r--   0 vsts      (1001) docker     (121)     3075 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/3/trsm/bli_trsm_blk_var2.c
--rw-r--r--   0 vsts      (1001) docker     (121)     3331 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/3/trsm/bli_trsm_blk_var3.c
--rw-r--r--   0 vsts      (1001) docker     (121)     8562 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/3/trsm/bli_trsm_cntl.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2522 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/3/trsm/bli_trsm_cntl.h
--rw-r--r--   0 vsts      (1001) docker     (121)     5204 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/3/trsm/bli_trsm_front.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2105 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/3/trsm/bli_trsm_front.h
--rw-r--r--   0 vsts      (1001) docker     (121)    15924 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/3/trsm/bli_trsm_ll_ker_var2.c
--rw-r--r--   0 vsts      (1001) docker     (121)    16411 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/3/trsm/bli_trsm_lu_ker_var2.c
--rw-r--r--   0 vsts      (1001) docker     (121)    16640 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/3/trsm/bli_trsm_rl_ker_var2.c
--rw-r--r--   0 vsts      (1001) docker     (121)    16270 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/3/trsm/bli_trsm_ru_ker_var2.c
--rw-r--r--   0 vsts      (1001) docker     (121)     3051 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/3/trsm/bli_trsm_var.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2835 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/3/trsm/bli_trsm_xx_ker_var2.c
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.572226 blis-0.9.1.dev0/blis/_src/frame/3/trsm/other/
--rw-r--r--   0 vsts      (1001) docker     (121)    19746 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/3/trsm/other/bli_trsm_ll_ker_var2.c
--rw-r--r--   0 vsts      (1001) docker     (121)    20427 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/3/trsm/other/bli_trsm_ll_ker_var2rr.c
--rw-r--r--   0 vsts      (1001) docker     (121)    20420 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/3/trsm/other/bli_trsm_ll_ker_var2sl.c
--rw-r--r--   0 vsts      (1001) docker     (121)    18777 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/3/trsm/other/bli_trsm_lu_ker_var2.c
--rw-r--r--   0 vsts      (1001) docker     (121)    19458 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/3/trsm/other/bli_trsm_lu_ker_var2rr.c
--rw-r--r--   0 vsts      (1001) docker     (121)    19451 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/3/trsm/other/bli_trsm_lu_ker_var2sl.c
--rw-r--r--   0 vsts      (1001) docker     (121)    19921 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/3/trsm/other/bli_trsm_rl_ker_var2.c
--rw-r--r--   0 vsts      (1001) docker     (121)    19537 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/3/trsm/other/bli_trsm_ru_ker_var2.c
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.584226 blis-0.9.1.dev0/blis/_src/frame/base/
--rw-r--r--   0 vsts      (1001) docker     (121)    18338 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/base/bli_apool.c
--rw-r--r--   0 vsts      (1001) docker     (121)     3579 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/base/bli_apool.h
--rw-r--r--   0 vsts      (1001) docker     (121)     9301 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/base/bli_arch.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2005 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/base/bli_arch.h
--rw-r--r--   0 vsts      (1001) docker     (121)     6732 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/base/bli_array.c
--rw-r--r--   0 vsts      (1001) docker     (121)     3086 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/base/bli_array.h
--rw-r--r--   0 vsts      (1001) docker     (121)     3623 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/base/bli_auxinfo.h
--rw-r--r--   0 vsts      (1001) docker     (121)    10571 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/base/bli_blksz.c
--rw-r--r--   0 vsts      (1001) docker     (121)     7214 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/base/bli_blksz.h
--rw-r--r--   0 vsts      (1001) docker     (121)    22154 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/base/bli_check.c
--rw-r--r--   0 vsts      (1001) docker     (121)     5144 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/base/bli_check.h
--rw-r--r--   0 vsts      (1001) docker     (121)     4618 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/base/bli_clock.c
--rw-r--r--   0 vsts      (1001) docker     (121)     1833 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/base/bli_clock.h
--rw-r--r--   0 vsts      (1001) docker     (121)    11136 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/base/bli_cntl.c
--rw-r--r--   0 vsts      (1001) docker     (121)     5458 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/base/bli_cntl.h
--rw-r--r--   0 vsts      (1001) docker     (121)    51655 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/base/bli_cntx.c
--rw-r--r--   0 vsts      (1001) docker     (121)    21693 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/base/bli_cntx.h
--rw-r--r--   0 vsts      (1001) docker     (121)     3336 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/base/bli_const.c
--rw-r--r--   0 vsts      (1001) docker     (121)     1736 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/base/bli_const.h
--rw-r--r--   0 vsts      (1001) docker     (121)    40207 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/base/bli_cpuid.c
--rw-r--r--   0 vsts      (1001) docker     (121)     6867 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/base/bli_cpuid.h
--rw-r--r--   0 vsts      (1001) docker     (121)     4491 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/base/bli_env.c
--rw-r--r--   0 vsts      (1001) docker     (121)     1955 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/base/bli_env.h
--rw-r--r--   0 vsts      (1001) docker     (121)     8639 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/base/bli_error.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2126 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/base/bli_error.h
--rw-r--r--   0 vsts      (1001) docker     (121)     3170 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/base/bli_func.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2914 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/base/bli_func.h
--rw-r--r--   0 vsts      (1001) docker     (121)     6220 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/base/bli_getopt.c
--rw-r--r--   0 vsts      (1001) docker     (121)     1954 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/base/bli_getopt.h
--rw-r--r--   0 vsts      (1001) docker     (121)    28407 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/base/bli_gks.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2689 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/base/bli_gks.h
--rw-r--r--   0 vsts      (1001) docker     (121)     6060 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/base/bli_ind.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2642 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/base/bli_ind.h
--rw-r--r--   0 vsts      (1001) docker     (121)     7720 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/base/bli_info.c
--rw-r--r--   0 vsts      (1001) docker     (121)     5455 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/base/bli_info.h
--rw-r--r--   0 vsts      (1001) docker     (121)     4444 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/base/bli_init.c
--rw-r--r--   0 vsts      (1001) docker     (121)     1941 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/base/bli_init.h
--rw-r--r--   0 vsts      (1001) docker     (121)     3549 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/base/bli_machval.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2123 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/base/bli_machval.h
--rw-r--r--   0 vsts      (1001) docker     (121)     7665 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/base/bli_malloc.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2804 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/base/bli_malloc.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2347 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/base/bli_mbool.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2354 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/base/bli_mbool.h
--rw-r--r--   0 vsts      (1001) docker     (121)     4266 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/base/bli_mem.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2637 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/base/bli_memsys.c
--rw-r--r--   0 vsts      (1001) docker     (121)     1998 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/base/bli_memsys.h
--rw-r--r--   0 vsts      (1001) docker     (121)    20018 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/base/bli_obj.c
--rw-r--r--   0 vsts      (1001) docker     (121)     3572 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/base/bli_obj.h
--rw-r--r--   0 vsts      (1001) docker     (121)     7575 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/base/bli_obj_scalar.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2599 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/base/bli_obj_scalar.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1798 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/base/bli_opid.h
--rw-r--r--   0 vsts      (1001) docker     (121)     5047 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/base/bli_pack.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2072 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/base/bli_pack.h
--rw-r--r--   0 vsts      (1001) docker     (121)     7681 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/base/bli_param_map.c
--rw-r--r--   0 vsts      (1001) docker     (121)     5701 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/base/bli_param_map.h
--rw-r--r--   0 vsts      (1001) docker     (121)    24778 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/base/bli_part.c
--rw-r--r--   0 vsts      (1001) docker     (121)     3447 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/base/bli_part.h
--rw-r--r--   0 vsts      (1001) docker     (121)    17574 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/base/bli_pba.c
--rw-r--r--   0 vsts      (1001) docker     (121)     4486 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/base/bli_pba.h
--rw-r--r--   0 vsts      (1001) docker     (121)    22049 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/base/bli_pool.c
--rw-r--r--   0 vsts      (1001) docker     (121)     6726 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/base/bli_pool.h
--rw-r--r--   0 vsts      (1001) docker     (121)     5700 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/base/bli_prune.c
--rw-r--r--   0 vsts      (1001) docker     (121)     1783 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/base/bli_prune.h
--rw-r--r--   0 vsts      (1001) docker     (121)     5928 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/base/bli_query.c
--rw-r--r--   0 vsts      (1001) docker     (121)     1856 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/base/bli_query.h
--rw-r--r--   0 vsts      (1001) docker     (121)    14720 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/base/bli_rntm.c
--rw-r--r--   0 vsts      (1001) docker     (121)    10592 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/base/bli_rntm.h
--rw-r--r--   0 vsts      (1001) docker     (121)     5914 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/base/bli_sba.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2382 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/base/bli_sba.h
--rw-r--r--   0 vsts      (1001) docker     (121)     4823 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/base/bli_setgetijm.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2668 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/base/bli_setgetijm.h
--rw-r--r--   0 vsts      (1001) docker     (121)     4380 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/base/bli_setgetijv.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2561 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/base/bli_setgetijv.h
--rw-r--r--   0 vsts      (1001) docker     (121)     4830 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/base/bli_setri.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2177 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/base/bli_setri.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1906 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/base/bli_string.c
--rw-r--r--   0 vsts      (1001) docker     (121)     1709 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/base/bli_string.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2377 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/base/bli_winsys.c
--rw-r--r--   0 vsts      (1001) docker     (121)     1801 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/base/bli_winsys.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.584226 blis-0.9.1.dev0/blis/_src/frame/base/cast/
--rw-r--r--   0 vsts      (1001) docker     (121)     6855 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/base/cast/bli_castm.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2362 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/base/cast/bli_castm.h
--rw-r--r--   0 vsts      (1001) docker     (121)     6875 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/base/cast/bli_castnzm.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2370 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/base/cast/bli_castnzm.h
--rw-r--r--   0 vsts      (1001) docker     (121)     5161 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/base/cast/bli_castv.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2317 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/base/cast/bli_castv.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.584226 blis-0.9.1.dev0/blis/_src/frame/base/cast/old/
--rw-r--r--   0 vsts      (1001) docker     (121)     3350 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/base/cast/old/bli_cast_check.c
--rw-r--r--   0 vsts      (1001) docker     (121)     1812 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/base/cast/old/bli_cast_check.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.584226 blis-0.9.1.dev0/blis/_src/frame/base/check/
--rw-r--r--   0 vsts      (1001) docker     (121)     5732 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/base/check/bli_obj_check.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2965 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/base/check/bli_obj_check.h
--rw-r--r--   0 vsts      (1001) docker     (121)     3263 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/base/check/bli_part_check.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2476 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/base/check/bli_part_check.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.584226 blis-0.9.1.dev0/blis/_src/frame/base/noopt/
--rw-r--r--   0 vsts      (1001) docker     (121)    29298 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/base/noopt/bli_dlamch.c
--rw-r--r--   0 vsts      (1001) docker     (121)     1738 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/base/noopt/bli_dlamch.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2797 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/base/noopt/bli_lsame.c
--rw-r--r--   0 vsts      (1001) docker     (121)     1766 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/base/noopt/bli_lsame.h
--rw-r--r--   0 vsts      (1001) docker     (121)    29227 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/base/noopt/bli_slamch.c
--rw-r--r--   0 vsts      (1001) docker     (121)     1736 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/base/noopt/bli_slamch.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.584226 blis-0.9.1.dev0/blis/_src/frame/base/proj/
--rw-r--r--   0 vsts      (1001) docker     (121)     3662 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/base/proj/bli_projm.c
--rw-r--r--   0 vsts      (1001) docker     (121)     1824 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/base/proj/bli_projm.h
--rw-r--r--   0 vsts      (1001) docker     (121)     3668 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/base/proj/bli_projv.c
--rw-r--r--   0 vsts      (1001) docker     (121)     1824 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/base/proj/bli_projv.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.584226 blis-0.9.1.dev0/blis/_src/frame/base/proj/old/
--rw-r--r--   0 vsts      (1001) docker     (121)     3286 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/base/proj/old/bli_proj_check.c
--rw-r--r--   0 vsts      (1001) docker     (121)     1812 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/base/proj/old/bli_proj_check.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.592226 blis-0.9.1.dev0/blis/_src/frame/compat/
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.592226 blis-0.9.1.dev0/blis/_src/frame/compat/amd/
--rw-r--r--   0 vsts      (1001) docker     (121)     4686 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/amd/bla_copy_amd.c
--rw-r--r--   0 vsts      (1001) docker     (121)     5686 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/amd/bla_gemv_amd.c
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.596226 blis-0.9.1.dev0/blis/_src/frame/compat/attic/
--rw-r--r--   0 vsts      (1001) docker     (121)     3273 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/attic/bla_gbmv.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2405 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/attic/bla_gbmv.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2971 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/attic/bla_hbmv.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2336 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/attic/bla_hbmv.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2914 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/attic/bla_hpmv.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2279 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/attic/bla_hpmv.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2722 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/attic/bla_hpr.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2174 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/attic/bla_hpr.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2868 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/attic/bla_hpr2.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2233 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/attic/bla_hpr2.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2725 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/attic/bla_rot.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2235 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/attic/bla_rot.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2215 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/attic/bla_rotg.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2133 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/attic/bla_rotg.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2602 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/attic/bla_rotm.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2126 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/attic/bla_rotm.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2219 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/attic/bla_rotmg.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2136 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/attic/bla_rotmg.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2957 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/attic/bla_sbmv.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2322 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/attic/bla_sbmv.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2900 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/attic/bla_spmv.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2265 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/attic/bla_spmv.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2708 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/attic/bla_spr.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2160 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/attic/bla_spr.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2854 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/attic/bla_spr2.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2219 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/attic/bla_spr2.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2981 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/attic/bla_tbmv.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2260 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/attic/bla_tbmv.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2981 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/attic/bla_tbsv.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2260 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/attic/bla_tbsv.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2924 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/attic/bla_tpmv.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2203 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/attic/bla_tpmv.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2924 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/attic/bla_tpsv.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2203 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/attic/bla_tpsv.h
--rw-r--r--   0 vsts      (1001) docker     (121)     3167 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/bla_amax.c
--rw-r--r--   0 vsts      (1001) docker     (121)     1989 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/bla_amax.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2638 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/bla_asum.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2011 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/bla_asum.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2780 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/bla_axpy.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2057 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/bla_axpy.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2729 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/bla_copy.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2026 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/bla_copy.h
--rw-r--r--   0 vsts      (1001) docker     (121)     5756 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/bla_dot.c
--rw-r--r--   0 vsts      (1001) docker     (121)     3010 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/bla_dot.h
--rw-r--r--   0 vsts      (1001) docker     (121)     7103 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/bla_gemm.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2261 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/bla_gemm.h
--rw-r--r--   0 vsts      (1001) docker     (121)     4788 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/bla_gemv.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2202 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/bla_gemv.h
--rw-r--r--   0 vsts      (1001) docker     (121)     3272 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/bla_ger.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2154 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/bla_ger.h
--rw-r--r--   0 vsts      (1001) docker     (121)     6206 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/bla_hemm.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2250 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/bla_hemm.h
--rw-r--r--   0 vsts      (1001) docker     (121)     3440 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/bla_hemv.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2193 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/bla_hemv.h
--rw-r--r--   0 vsts      (1001) docker     (121)     3196 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/bla_her.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2112 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/bla_her.h
--rw-r--r--   0 vsts      (1001) docker     (121)     3390 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/bla_her2.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2162 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/bla_her2.h
--rw-r--r--   0 vsts      (1001) docker     (121)     7171 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/bla_her2k.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2253 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/bla_her2k.h
--rw-r--r--   0 vsts      (1001) docker     (121)     6602 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/bla_herk.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2204 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/bla_herk.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2639 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/bla_nrm2.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2011 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/bla_nrm2.h
--rw-r--r--   0 vsts      (1001) docker     (121)     3012 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/bla_scal.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2039 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/bla_scal.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2693 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/bla_swap.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2014 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/bla_swap.h
--rw-r--r--   0 vsts      (1001) docker     (121)     6168 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/bla_symm.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2230 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/bla_symm.h
--rw-r--r--   0 vsts      (1001) docker     (121)     3426 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/bla_symv.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2179 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/bla_symv.h
--rw-r--r--   0 vsts      (1001) docker     (121)     3180 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/bla_syr.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2098 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/bla_syr.h
--rw-r--r--   0 vsts      (1001) docker     (121)     3378 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/bla_syr2.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2148 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/bla_syr2.h
--rw-r--r--   0 vsts      (1001) docker     (121)     6799 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/bla_syr2k.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2233 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/bla_syr2k.h
--rw-r--r--   0 vsts      (1001) docker     (121)     6224 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/bla_syrk.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2184 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/bla_syrk.h
--rw-r--r--   0 vsts      (1001) docker     (121)     5926 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/bla_trmm.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2216 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/bla_trmm.h
--rw-r--r--   0 vsts      (1001) docker     (121)     3523 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/bla_trmv.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2126 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/bla_trmv.h
--rw-r--r--   0 vsts      (1001) docker     (121)     5926 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/bla_trsm.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2216 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/bla_trsm.h
--rw-r--r--   0 vsts      (1001) docker     (121)     3523 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/bla_trsv.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2126 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/bla_trsv.h
--rw-r--r--   0 vsts      (1001) docker     (121)     5539 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/bli_blas.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.496226 blis-0.9.1.dev0/blis/_src/frame/compat/blis/
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.596226 blis-0.9.1.dev0/blis/_src/frame/compat/blis/thread/
--rw-r--r--   0 vsts      (1001) docker     (121)     2754 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/blis/thread/b77_thread.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2029 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/blis/thread/b77_thread.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.596226 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/
--rw-r--r--   0 vsts      (1001) docker     (121)     2157 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/bli_cblas.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.600226 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/f77_sub/
--rw-r--r--   0 vsts      (1001) docker     (121)     2149 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/f77_sub/f77_amax_sub.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2032 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/f77_sub/f77_amax_sub.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2173 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/f77_sub/f77_asum_sub.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2054 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/f77_sub/f77_asum_sub.h
--rw-r--r--   0 vsts      (1001) docker     (121)     3760 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/f77_sub/f77_dot_sub.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2582 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/f77_sub/f77_dot_sub.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2173 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/f77_sub/f77_nrm2_sub.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2054 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/f77_sub/f77_nrm2_sub.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.616227 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/
--rw-r--r--   0 vsts      (1001) docker     (121)    37101 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas.h
--rw-r--r--   0 vsts      (1001) docker     (121)      576 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_caxpy.c
--rw-r--r--   0 vsts      (1001) docker     (121)      537 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_ccopy.c
--rw-r--r--   0 vsts      (1001) docker     (121)      635 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_cdotc_sub.c
--rw-r--r--   0 vsts      (1001) docker     (121)      637 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_cdotu_sub.c
--rw-r--r--   0 vsts      (1001) docker     (121)     4350 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_cgbmv.c
--rw-r--r--   0 vsts      (1001) docker     (121)     3116 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_cgemm.c
--rw-r--r--   0 vsts      (1001) docker     (121)     4255 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_cgemv.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2037 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_cgerc.c
--rw-r--r--   0 vsts      (1001) docker     (121)     1251 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_cgeru.c
--rw-r--r--   0 vsts      (1001) docker     (121)     3659 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_chbmv.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2798 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_chemm.c
--rw-r--r--   0 vsts      (1001) docker     (121)     3617 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_chemv.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2635 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_cher.c
--rw-r--r--   0 vsts      (1001) docker     (121)     3506 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_cher2.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2981 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_cher2k.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2739 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_cherk.c
--rw-r--r--   0 vsts      (1001) docker     (121)     3543 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_chpmv.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2562 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_chpr.c
--rw-r--r--   0 vsts      (1001) docker     (121)     3375 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_chpr2.c
--rw-r--r--   0 vsts      (1001) docker     (121)      484 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_cscal.c
--rw-r--r--   0 vsts      (1001) docker     (121)      469 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_csscal.c
--rw-r--r--   0 vsts      (1001) docker     (121)      532 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_cswap.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2793 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_csymm.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2919 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_csyr2k.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2790 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_csyrk.c
--rw-r--r--   0 vsts      (1001) docker     (121)     4032 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_ctbmv.c
--rw-r--r--   0 vsts      (1001) docker     (121)     4041 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_ctbsv.c
--rw-r--r--   0 vsts      (1001) docker     (121)     3848 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_ctpmv.c
--rw-r--r--   0 vsts      (1001) docker     (121)     3858 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_ctpsv.c
--rw-r--r--   0 vsts      (1001) docker     (121)     3986 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_ctrmm.c
--rw-r--r--   0 vsts      (1001) docker     (121)     3965 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_ctrmv.c
--rw-r--r--   0 vsts      (1001) docker     (121)     4044 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_ctrsm.c
--rw-r--r--   0 vsts      (1001) docker     (121)     3981 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_ctrsv.c
--rw-r--r--   0 vsts      (1001) docker     (121)      518 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_dasum.c
--rw-r--r--   0 vsts      (1001) docker     (121)      543 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_daxpy.c
--rw-r--r--   0 vsts      (1001) docker     (121)      519 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_dcopy.c
--rw-r--r--   0 vsts      (1001) docker     (121)      619 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_ddot.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2296 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_dgbmv.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2989 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_dgemm.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2145 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_dgemv.c
--rw-r--r--   0 vsts      (1001) docker     (121)     1179 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_dger.c
--rw-r--r--   0 vsts      (1001) docker     (121)      517 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_dnrm2.c
--rw-r--r--   0 vsts      (1001) docker     (121)      541 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_drot.c
--rw-r--r--   0 vsts      (1001) docker     (121)      303 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_drotg.c
--rw-r--r--   0 vsts      (1001) docker     (121)      420 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_drotm.c
--rw-r--r--   0 vsts      (1001) docker     (121)      354 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_drotmg.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2028 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_dsbmv.c
--rw-r--r--   0 vsts      (1001) docker     (121)      458 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_dscal.c
--rw-r--r--   0 vsts      (1001) docker     (121)      624 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_dsdot.c
--rw-r--r--   0 vsts      (1001) docker     (121)     1909 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_dspmv.c
--rw-r--r--   0 vsts      (1001) docker     (121)     1688 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_dspr.c
--rw-r--r--   0 vsts      (1001) docker     (121)     1788 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_dspr2.c
--rw-r--r--   0 vsts      (1001) docker     (121)      514 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_dswap.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2686 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_dsymm.c
--rw-r--r--   0 vsts      (1001) docker     (121)     1973 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_dsymv.c
--rw-r--r--   0 vsts      (1001) docker     (121)     1765 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_dsyr.c
--rw-r--r--   0 vsts      (1001) docker     (121)     1932 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_dsyr2.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2825 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_dsyr2k.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2700 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_dsyrk.c
--rw-r--r--   0 vsts      (1001) docker     (121)     3308 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_dtbmv.c
--rw-r--r--   0 vsts      (1001) docker     (121)     3318 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_dtbsv.c
--rw-r--r--   0 vsts      (1001) docker     (121)     3135 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_dtpmv.c
--rw-r--r--   0 vsts      (1001) docker     (121)     3136 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_dtpsv.c
--rw-r--r--   0 vsts      (1001) docker     (121)     3981 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_dtrmm.c
--rw-r--r--   0 vsts      (1001) docker     (121)     3277 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_dtrmv.c
--rw-r--r--   0 vsts      (1001) docker     (121)     4061 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_dtrsm.c
--rw-r--r--   0 vsts      (1001) docker     (121)     3263 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_dtrsv.c
--rw-r--r--   0 vsts      (1001) docker     (121)      521 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_dzasum.c
--rw-r--r--   0 vsts      (1001) docker     (121)      521 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_dznrm2.c
--rw-r--r--   0 vsts      (1001) docker     (121)     6368 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_f77.h
--rw-r--r--   0 vsts      (1001) docker     (121)       93 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_globals.c
--rw-r--r--   0 vsts      (1001) docker     (121)      550 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_icamax.c
--rw-r--r--   0 vsts      (1001) docker     (121)      541 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_idamax.c
--rw-r--r--   0 vsts      (1001) docker     (121)      540 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_isamax.c
--rw-r--r--   0 vsts      (1001) docker     (121)      552 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_izamax.c
--rw-r--r--   0 vsts      (1001) docker     (121)      515 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_sasum.c
--rw-r--r--   0 vsts      (1001) docker     (121)      594 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_saxpy.c
--rw-r--r--   0 vsts      (1001) docker     (121)      519 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_scasum.c
--rw-r--r--   0 vsts      (1001) docker     (121)      519 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_scnrm2.c
--rw-r--r--   0 vsts      (1001) docker     (121)      517 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_scopy.c
--rw-r--r--   0 vsts      (1001) docker     (121)      615 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_sdot.c
--rw-r--r--   0 vsts      (1001) docker     (121)      646 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_sdsdot.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2303 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_sgbmv.c
--rw-r--r--   0 vsts      (1001) docker     (121)     3129 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_sgemm.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2126 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_sgemv.c
--rw-r--r--   0 vsts      (1001) docker     (121)     1151 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_sger.c
--rw-r--r--   0 vsts      (1001) docker     (121)      515 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_snrm2.c
--rw-r--r--   0 vsts      (1001) docker     (121)      548 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_srot.c
--rw-r--r--   0 vsts      (1001) docker     (121)      299 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_srotg.c
--rw-r--r--   0 vsts      (1001) docker     (121)      534 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_srotm.c
--rw-r--r--   0 vsts      (1001) docker     (121)      349 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_srotmg.c
--rw-r--r--   0 vsts      (1001) docker     (121)     1953 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_ssbmv.c
--rw-r--r--   0 vsts      (1001) docker     (121)      456 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_sscal.c
--rw-r--r--   0 vsts      (1001) docker     (121)     1890 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_sspmv.c
--rw-r--r--   0 vsts      (1001) docker     (121)     1694 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_sspr.c
--rw-r--r--   0 vsts      (1001) docker     (121)     1789 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_sspr2.c
--rw-r--r--   0 vsts      (1001) docker     (121)      512 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_sswap.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2760 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_ssymm.c
--rw-r--r--   0 vsts      (1001) docker     (121)     1968 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_ssymv.c
--rw-r--r--   0 vsts      (1001) docker     (121)     1761 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_ssyr.c
--rw-r--r--   0 vsts      (1001) docker     (121)     1928 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_ssyr2.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2900 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_ssyr2k.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2778 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_ssyrk.c
--rw-r--r--   0 vsts      (1001) docker     (121)     3333 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_stbmv.c
--rw-r--r--   0 vsts      (1001) docker     (121)     3317 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_stbsv.c
--rw-r--r--   0 vsts      (1001) docker     (121)     3148 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_stpmv.c
--rw-r--r--   0 vsts      (1001) docker     (121)     3134 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_stpsv.c
--rw-r--r--   0 vsts      (1001) docker     (121)     3953 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_strmm.c
--rw-r--r--   0 vsts      (1001) docker     (121)     3276 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_strmv.c
--rw-r--r--   0 vsts      (1001) docker     (121)     3975 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_strsm.c
--rw-r--r--   0 vsts      (1001) docker     (121)     3261 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_strsv.c
--rw-r--r--   0 vsts      (1001) docker     (121)     1982 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_xerbla.c
--rw-r--r--   0 vsts      (1001) docker     (121)      576 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_zaxpy.c
--rw-r--r--   0 vsts      (1001) docker     (121)      537 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_zcopy.c
--rw-r--r--   0 vsts      (1001) docker     (121)      647 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_zdotc_sub.c
--rw-r--r--   0 vsts      (1001) docker     (121)      649 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_zdotu_sub.c
--rw-r--r--   0 vsts      (1001) docker     (121)      471 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_zdscal.c
--rw-r--r--   0 vsts      (1001) docker     (121)     4367 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_zgbmv.c
--rw-r--r--   0 vsts      (1001) docker     (121)     3112 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_zgemm.c
--rw-r--r--   0 vsts      (1001) docker     (121)     4219 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_zgemv.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2042 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_zgerc.c
--rw-r--r--   0 vsts      (1001) docker     (121)     1251 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_zgeru.c
--rw-r--r--   0 vsts      (1001) docker     (121)     3669 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_zhbmv.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2799 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_zhemm.c
--rw-r--r--   0 vsts      (1001) docker     (121)     3625 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_zhemv.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2560 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_zher.c
--rw-r--r--   0 vsts      (1001) docker     (121)     3522 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_zher2.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2981 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_zher2k.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2741 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_zherk.c
--rw-r--r--   0 vsts      (1001) docker     (121)     3553 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_zhpmv.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2568 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_zhpr.c
--rw-r--r--   0 vsts      (1001) docker     (121)     3399 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_zhpr2.c
--rw-r--r--   0 vsts      (1001) docker     (121)      482 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_zscal.c
--rw-r--r--   0 vsts      (1001) docker     (121)      534 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_zswap.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2794 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_zsymm.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2919 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_zsyr2k.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2790 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_zsyrk.c
--rw-r--r--   0 vsts      (1001) docker     (121)     4034 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_ztbmv.c
--rw-r--r--   0 vsts      (1001) docker     (121)     4043 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_ztbsv.c
--rw-r--r--   0 vsts      (1001) docker     (121)     3850 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_ztpmv.c
--rw-r--r--   0 vsts      (1001) docker     (121)     3860 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_ztpsv.c
--rw-r--r--   0 vsts      (1001) docker     (121)     4062 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_ztrmm.c
--rw-r--r--   0 vsts      (1001) docker     (121)     3981 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_ztrmv.c
--rw-r--r--   0 vsts      (1001) docker     (121)     4078 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_ztrsm.c
--rw-r--r--   0 vsts      (1001) docker     (121)     3983 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_ztrsv.c
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.616227 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/extra/
--rw-r--r--   0 vsts      (1001) docker     (121)      646 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/extra/cblas_caxpby.c
--rw-r--r--   0 vsts      (1001) docker     (121)     3181 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/extra/cblas_cgemm3m.c
--rw-r--r--   0 vsts      (1001) docker     (121)     5593 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/extra/cblas_cgemm_batch.c
--rw-r--r--   0 vsts      (1001) docker     (121)     5349 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/extra/cblas_cgemmt.c
--rw-r--r--   0 vsts      (1001) docker     (121)      594 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/extra/cblas_daxpby.c
--rw-r--r--   0 vsts      (1001) docker     (121)     5439 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/extra/cblas_dgemm_batch.c
--rw-r--r--   0 vsts      (1001) docker     (121)     5239 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/extra/cblas_dgemmt.c
--rw-r--r--   0 vsts      (1001) docker     (121)      647 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/extra/cblas_saxpby.c
--rw-r--r--   0 vsts      (1001) docker     (121)     5435 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/extra/cblas_sgemm_batch.c
--rw-r--r--   0 vsts      (1001) docker     (121)     5234 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/extra/cblas_sgemmt.c
--rw-r--r--   0 vsts      (1001) docker     (121)      648 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/extra/cblas_zaxpby.c
--rw-r--r--   0 vsts      (1001) docker     (121)     3179 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/extra/cblas_zgemm3m.c
--rw-r--r--   0 vsts      (1001) docker     (121)     5593 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/extra/cblas_zgemm_batch.c
--rw-r--r--   0 vsts      (1001) docker     (121)     5349 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/extra/cblas_zgemmt.c
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.620226 blis-0.9.1.dev0/blis/_src/frame/compat/check/
--rw-r--r--   0 vsts      (1001) docker     (121)     3139 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/check/bla_gemm3m_check.h
--rw-r--r--   0 vsts      (1001) docker     (121)     3064 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/check/bla_gemm_check.h
--rw-r--r--   0 vsts      (1001) docker     (121)     3228 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/check/bla_gemmt_check.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2539 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/check/bla_gemv_check.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2370 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/check/bla_ger_check.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2782 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/check/bla_hemm_check.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2422 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/check/bla_hemv_check.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2421 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/check/bla_her2_check.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2783 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/check/bla_her2k_check.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2374 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/check/bla_her_check.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2726 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/check/bla_herk_check.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1744 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/check/bla_symm_check.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1744 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/check/bla_symv_check.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1744 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/check/bla_syr2_check.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2973 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/check/bla_syr2k_check.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1742 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/check/bla_syr_check.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2917 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/check/bla_syrk_check.h
--rw-r--r--   0 vsts      (1001) docker     (121)     3221 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/check/bla_trmm_check.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2873 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/check/bla_trmv_check.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1744 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/check/bla_trsm_check.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1744 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/check/bla_trsv_check.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.620226 blis-0.9.1.dev0/blis/_src/frame/compat/extra/
--rw-r--r--   0 vsts      (1001) docker     (121)     2829 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/extra/bla_axpby.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2083 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/extra/bla_axpby.h
--rw-r--r--   0 vsts      (1001) docker     (121)     7544 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/extra/bla_gemm3m.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2299 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/extra/bla_gemm3m.h
--rw-r--r--   0 vsts      (1001) docker     (121)     7296 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/extra/bla_gemm_batch.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2415 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/extra/bla_gemm_batch.h
--rw-r--r--   0 vsts      (1001) docker     (121)     6351 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/extra/bla_gemmt.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2318 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/extra/bla_gemmt.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.628227 blis-0.9.1.dev0/blis/_src/frame/compat/f2c/
--rw-r--r--   0 vsts      (1001) docker     (121)     2347 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/f2c/bla_cabs1.c
--rw-r--r--   0 vsts      (1001) docker     (121)     1834 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/f2c/bla_cabs1.h
--rw-r--r--   0 vsts      (1001) docker     (121)    51775 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/f2c/bla_gbmv.c
--rw-r--r--   0 vsts      (1001) docker     (121)     3066 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/f2c/bla_gbmv.h
--rw-r--r--   0 vsts      (1001) docker     (121)    36539 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/f2c/bla_hbmv.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2306 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/f2c/bla_hbmv.h
--rw-r--r--   0 vsts      (1001) docker     (121)    32318 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/f2c/bla_hpmv.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2216 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/f2c/bla_hpmv.h
--rw-r--r--   0 vsts      (1001) docker     (121)    22952 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/f2c/bla_hpr.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2060 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/f2c/bla_hpr.h
--rw-r--r--   0 vsts      (1001) docker     (121)    33391 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/f2c/bla_hpr2.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2164 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/f2c/bla_hpr2.h
--rw-r--r--   0 vsts      (1001) docker     (121)     4594 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/f2c/bla_lsame.c
--rw-r--r--   0 vsts      (1001) docker     (121)     1915 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/f2c/bla_lsame.h
--rw-r--r--   0 vsts      (1001) docker     (121)    10542 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/f2c/bla_rot.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2448 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/f2c/bla_rot.h
--rw-r--r--   0 vsts      (1001) docker     (121)     8027 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/f2c/bla_rotg.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2120 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/f2c/bla_rotg.h
--rw-r--r--   0 vsts      (1001) docker     (121)     9056 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/f2c/bla_rotm.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2038 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/f2c/bla_rotm.h
--rw-r--r--   0 vsts      (1001) docker     (121)    11542 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/f2c/bla_rotmg.c
--rw-r--r--   0 vsts      (1001) docker     (121)     1964 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/f2c/bla_rotmg.h
--rw-r--r--   0 vsts      (1001) docker     (121)    21669 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/f2c/bla_sbmv.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2276 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/f2c/bla_sbmv.h
--rw-r--r--   0 vsts      (1001) docker     (121)    17321 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/f2c/bla_spmv.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2186 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/f2c/bla_spmv.h
--rw-r--r--   0 vsts      (1001) docker     (121)    13888 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/f2c/bla_spr.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2048 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/f2c/bla_spr.h
--rw-r--r--   0 vsts      (1001) docker     (121)    16058 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/f2c/bla_spr2.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2140 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/f2c/bla_spr2.h
--rw-r--r--   0 vsts      (1001) docker     (121)    67667 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/f2c/bla_tbmv.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2710 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/f2c/bla_tbmv.h
--rw-r--r--   0 vsts      (1001) docker     (121)    64601 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/f2c/bla_tbsv.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2710 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/f2c/bla_tbsv.h
--rw-r--r--   0 vsts      (1001) docker     (121)    55833 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/f2c/bla_tpmv.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2530 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/f2c/bla_tpmv.h
--rw-r--r--   0 vsts      (1001) docker     (121)    52801 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/f2c/bla_tpsv.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2530 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/f2c/bla_tpsv.h
--rw-r--r--   0 vsts      (1001) docker     (121)     3215 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/f2c/bla_xerbla.c
--rw-r--r--   0 vsts      (1001) docker     (121)     1836 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/f2c/bla_xerbla.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2599 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/f2c/bla_xerbla_array.c
--rw-r--r--   0 vsts      (1001) docker     (121)     1836 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/f2c/bla_xerbla_array.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.632227 blis-0.9.1.dev0/blis/_src/frame/compat/f2c/util/
--rw-r--r--   0 vsts      (1001) docker     (121)     1852 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/f2c/util/bla_c_abs.c
--rw-r--r--   0 vsts      (1001) docker     (121)     1748 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/f2c/util/bla_c_abs.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1864 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/f2c/util/bla_c_div.c
--rw-r--r--   0 vsts      (1001) docker     (121)     1789 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/f2c/util/bla_c_div.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1813 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/f2c/util/bla_d_abs.c
--rw-r--r--   0 vsts      (1001) docker     (121)     1746 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/f2c/util/bla_d_abs.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1820 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/f2c/util/bla_d_cnjg.c
--rw-r--r--   0 vsts      (1001) docker     (121)     1769 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/f2c/util/bla_d_cnjg.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1796 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/f2c/util/bla_d_imag.c
--rw-r--r--   0 vsts      (1001) docker     (121)     1749 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/f2c/util/bla_d_imag.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1857 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/f2c/util/bla_d_sign.c
--rw-r--r--   0 vsts      (1001) docker     (121)     1768 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/f2c/util/bla_d_sign.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2116 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/f2c/util/bla_f__cabs.c
--rw-r--r--   0 vsts      (1001) docker     (121)     1753 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/f2c/util/bla_f__cabs.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1811 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/f2c/util/bla_r_abs.c
--rw-r--r--   0 vsts      (1001) docker     (121)     1744 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/f2c/util/bla_r_abs.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1820 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/f2c/util/bla_r_cnjg.c
--rw-r--r--   0 vsts      (1001) docker     (121)     1769 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/f2c/util/bla_r_cnjg.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1798 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/f2c/util/bla_r_imag.c
--rw-r--r--   0 vsts      (1001) docker     (121)     1751 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/f2c/util/bla_r_imag.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1853 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/f2c/util/bla_r_sign.c
--rw-r--r--   0 vsts      (1001) docker     (121)     1764 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/f2c/util/bla_r_sign.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1852 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/f2c/util/bla_z_abs.c
--rw-r--r--   0 vsts      (1001) docker     (121)     1748 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/f2c/util/bla_z_abs.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1864 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/f2c/util/bla_z_div.c
--rw-r--r--   0 vsts      (1001) docker     (121)     1789 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/compat/f2c/util/bla_z_div.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.636227 blis-0.9.1.dev0/blis/_src/frame/include/
--rw-r--r--   0 vsts      (1001) docker     (121)     7804 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/bli_arch_config.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2808 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/bli_arch_config_pre.h
--rw-r--r--   0 vsts      (1001) docker     (121)     3176 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/bli_blas_macro_defs.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2052 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/bli_builtin_macro_defs.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2337 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/bli_complex_macro_defs.h
--rw-r--r--   0 vsts      (1001) docker     (121)    10343 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/bli_config_macro_defs.h
--rw-r--r--   0 vsts      (1001) docker     (121)     7737 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/bli_edge_case_macro_defs.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1922 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/bli_error_macro_defs.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2225 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/bli_extern_defs.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2301 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/bli_f2c.h
--rw-r--r--   0 vsts      (1001) docker     (121)    10772 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/bli_genarray_macro_defs.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2871 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/bli_gentdef_macro_defs.h
--rw-r--r--   0 vsts      (1001) docker     (121)    54463 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/bli_gentfunc_macro_defs.h
--rw-r--r--   0 vsts      (1001) docker     (121)    27414 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/bli_gentprot_macro_defs.h
--rw-r--r--   0 vsts      (1001) docker     (121)     8415 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/bli_kernel_macro_defs.h
--rw-r--r--   0 vsts      (1001) docker     (121)     4043 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/bli_lang_defs.h
--rw-r--r--   0 vsts      (1001) docker     (121)     4527 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/bli_macro_defs.h
--rw-r--r--   0 vsts      (1001) docker     (121)     4435 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/bli_misc_macro_defs.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2547 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/bli_oapi_ba.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2469 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/bli_oapi_ex.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1808 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/bli_oapi_macro_defs.h
--rw-r--r--   0 vsts      (1001) docker     (121)    40527 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/bli_obj_macro_defs.h
--rw-r--r--   0 vsts      (1001) docker     (121)    33815 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/bli_param_macro_defs.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2687 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/bli_pragma_macro_defs.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2035 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/bli_sbox.h
--rw-r--r--   0 vsts      (1001) docker     (121)     5762 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/bli_scalar_macro_defs.h
--rw-r--r--   0 vsts      (1001) docker     (121)     4131 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/bli_system.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2546 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/bli_tapi_ba.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2468 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/bli_tapi_ex.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1807 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/bli_tapi_macro_defs.h
--rw-r--r--   0 vsts      (1001) docker     (121)    43725 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/bli_type_defs.h
--rw-r--r--   0 vsts      (1001) docker     (121)    46891 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/bli_x86_asm_macros.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2425 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/bli_xapi_undef.h
--rw-r--r--   0 vsts      (1001) docker     (121)     5488 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/blis.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.640227 blis-0.9.1.dev0/blis/_src/frame/include/level0/
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.640227 blis-0.9.1.dev0/blis/_src/frame/include/level0/1e/
--rw-r--r--   0 vsts      (1001) docker     (121)     3282 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/level0/1e/bli_copy1es.h
--rw-r--r--   0 vsts      (1001) docker     (121)     3305 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/level0/1e/bli_copyj1es.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2108 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/level0/1e/bli_invert1es.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2166 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/level0/1e/bli_scal1es.h
--rw-r--r--   0 vsts      (1001) docker     (121)    10659 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/level0/1e/bli_scal21es.h
--rw-r--r--   0 vsts      (1001) docker     (121)    10730 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/level0/1e/bli_scal2j1es.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.644227 blis-0.9.1.dev0/blis/_src/frame/include/level0/1m/
--rw-r--r--   0 vsts      (1001) docker     (121)     4503 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/level0/1m/bli_invert1ms_mxn_diag.h
--rw-r--r--   0 vsts      (1001) docker     (121)     3942 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/level0/1m/bli_scal1ms_mxn.h
--rw-r--r--   0 vsts      (1001) docker     (121)     5933 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/level0/1m/bli_scal21ms_mxn.h
--rw-r--r--   0 vsts      (1001) docker     (121)     4280 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/level0/1m/bli_scal21ms_mxn_diag.h
--rw-r--r--   0 vsts      (1001) docker     (121)     8706 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/level0/1m/bli_scal21ms_mxn_uplo.h
--rw-r--r--   0 vsts      (1001) docker     (121)     6489 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/level0/1m/bli_set1ms_mxn.h
--rw-r--r--   0 vsts      (1001) docker     (121)     4578 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/level0/1m/bli_set1ms_mxn_diag.h
--rw-r--r--   0 vsts      (1001) docker     (121)     6132 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/level0/1m/bli_set1ms_mxn_uplo.h
--rw-r--r--   0 vsts      (1001) docker     (121)     3702 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/level0/1m/bli_seti01ms_mxn_diag.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.644227 blis-0.9.1.dev0/blis/_src/frame/include/level0/1r/
--rw-r--r--   0 vsts      (1001) docker     (121)     1936 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/level0/1r/bli_copy1rs.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1943 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/level0/1r/bli_copyj1rs.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1864 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/level0/1r/bli_invert1rs.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2136 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/level0/1r/bli_scal1rs.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2421 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/level0/1r/bli_scal21rs.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2432 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/level0/1r/bli_scal2j1rs.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.644227 blis-0.9.1.dev0/blis/_src/frame/include/level0/bb/
--rw-r--r--   0 vsts      (1001) docker     (121)     2480 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/level0/bb/bli_bcastbbs_mxn.h
--rw-r--r--   0 vsts      (1001) docker     (121)     6341 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/level0/bb/bli_scal2bbs_mxn.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2468 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/level0/bb/bli_set0bbs_mxn.h
--rw-r--r--   0 vsts      (1001) docker     (121)     4986 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/level0/bli_absq2s.h
--rw-r--r--   0 vsts      (1001) docker     (121)     5104 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/level0/bli_abval2s.h
--rw-r--r--   0 vsts      (1001) docker     (121)    12899 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/level0/bli_add3s.h
--rw-r--r--   0 vsts      (1001) docker     (121)     4141 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/level0/bli_addjs.h
--rw-r--r--   0 vsts      (1001) docker     (121)     4050 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/level0/bli_adds.h
--rw-r--r--   0 vsts      (1001) docker     (121)    16133 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/level0/bli_adds_mxn.h
--rw-r--r--   0 vsts      (1001) docker     (121)     5651 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/level0/bli_adds_mxn_uplo.h
--rw-r--r--   0 vsts      (1001) docker     (121)    12947 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/level0/bli_axmys.h
--rw-r--r--   0 vsts      (1001) docker     (121)    55936 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/level0/bli_axpbyjs.h
--rw-r--r--   0 vsts      (1001) docker     (121)    54645 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/level0/bli_axpbys.h
--rw-r--r--   0 vsts      (1001) docker     (121)    13190 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/level0/bli_axpyjs.h
--rw-r--r--   0 vsts      (1001) docker     (121)    12947 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/level0/bli_axpys.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2208 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/level0/bli_conjs.h
--rw-r--r--   0 vsts      (1001) docker     (121)     3205 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/level0/bli_constants.h
--rw-r--r--   0 vsts      (1001) docker     (121)     4815 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/level0/bli_copycjs.h
--rw-r--r--   0 vsts      (1001) docker     (121)     4072 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/level0/bli_copyjnzs.h
--rw-r--r--   0 vsts      (1001) docker     (121)     4292 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/level0/bli_copyjs.h
--rw-r--r--   0 vsts      (1001) docker     (121)     3942 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/level0/bli_copynzs.h
--rw-r--r--   0 vsts      (1001) docker     (121)     3912 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/level0/bli_copys.h
--rw-r--r--   0 vsts      (1001) docker     (121)    16273 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/level0/bli_copys_mxn.h
--rw-r--r--   0 vsts      (1001) docker     (121)     5870 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/level0/bli_dotjs.h
--rw-r--r--   0 vsts      (1001) docker     (121)     5697 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/level0/bli_dots.h
--rw-r--r--   0 vsts      (1001) docker     (121)     4078 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/level0/bli_eq.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2327 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/level0/bli_fprints.h
--rw-r--r--   0 vsts      (1001) docker     (121)     4005 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/level0/bli_gets.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2292 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/level0/bli_inverts.h
--rw-r--r--   0 vsts      (1001) docker     (121)     4353 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/level0/bli_invscaljs.h
--rw-r--r--   0 vsts      (1001) docker     (121)     4262 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/level0/bli_invscals.h
--rw-r--r--   0 vsts      (1001) docker     (121)     4101 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/level0/bli_neg2s.h
--rw-r--r--   0 vsts      (1001) docker     (121)     5379 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/level0/bli_randnp2s.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2302 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/level0/bli_rands.h
--rw-r--r--   0 vsts      (1001) docker     (121)    13377 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/level0/bli_scal2js.h
--rw-r--r--   0 vsts      (1001) docker     (121)    13133 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/level0/bli_scal2s.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2891 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/level0/bli_scal2s_mxn.h
--rw-r--r--   0 vsts      (1001) docker     (121)     4699 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/level0/bli_scalcjs.h
--rw-r--r--   0 vsts      (1001) docker     (121)     4200 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/level0/bli_scaljs.h
--rw-r--r--   0 vsts      (1001) docker     (121)     4109 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/level0/bli_scals.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1941 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/level0/bli_set0s.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2883 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/level0/bli_set0s_mxn.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1941 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/level0/bli_set1s.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1927 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/level0/bli_seti0s.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2781 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/level0/bli_setis.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2821 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/level0/bli_setrs.h
--rw-r--r--   0 vsts      (1001) docker     (121)     4279 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/level0/bli_sets.h
--rw-r--r--   0 vsts      (1001) docker     (121)     5073 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/level0/bli_sqrt2s.h
--rw-r--r--   0 vsts      (1001) docker     (121)     4141 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/level0/bli_subjs.h
--rw-r--r--   0 vsts      (1001) docker     (121)     4050 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/level0/bli_subs.h
--rw-r--r--   0 vsts      (1001) docker     (121)     4194 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/level0/bli_swaps.h
--rw-r--r--   0 vsts      (1001) docker     (121)    13325 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/level0/bli_xpbyjs.h
--rw-r--r--   0 vsts      (1001) docker     (121)    13154 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/level0/bli_xpbys.h
--rw-r--r--   0 vsts      (1001) docker     (121)    21503 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/level0/bli_xpbys_mxn.h
--rw-r--r--   0 vsts      (1001) docker     (121)     8639 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/level0/bli_xpbys_mxn_uplo.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.644227 blis-0.9.1.dev0/blis/_src/frame/include/level0/old/
--rw-r--r--   0 vsts      (1001) docker     (121)     4610 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/level0/old/bli_cast.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1672 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/level0/old/bli_castfrom.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1672 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/level0/old/bli_castto.h
--rw-r--r--   0 vsts      (1001) docker     (121)     3590 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/level0/old/bli_copynzjs.h
--rw-r--r--   0 vsts      (1001) docker     (121)     3518 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/level0/old/bli_copynzs.h
--rw-r--r--   0 vsts      (1001) docker     (121)     5273 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/level0/old/bli_invscalcjs.h
--rw-r--r--   0 vsts      (1001) docker     (121)     4707 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/level0/old/bli_scalcjs.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2692 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/level0/old/bli_set0ris_mxn.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.644227 blis-0.9.1.dev0/blis/_src/frame/include/level0/old/io/
--rw-r--r--   0 vsts      (1001) docker     (121)     2133 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/level0/old/io/bli_scal2ios.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1973 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/level0/old/io/bli_scal2jios.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.644227 blis-0.9.1.dev0/blis/_src/frame/include/level0/old/ri3/
--rw-r--r--   0 vsts      (1001) docker     (121)     2127 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/level0/old/ri3/bli_copyjri3s.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2107 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/level0/old/ri3/bli_copyri3s.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2521 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/level0/old/ri3/bli_scal2jri3s.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2508 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/level0/old/ri3/bli_scal2ri3s.h
--rw-r--r--   0 vsts      (1001) docker     (121)     5780 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/level0/old/ri3/bli_scal2ri3s_mxn.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.648227 blis-0.9.1.dev0/blis/_src/frame/include/level0/old/rih/
--rw-r--r--   0 vsts      (1001) docker     (121)     6836 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/level0/old/rih/bli_scal2rihs_mxn.h
--rw-r--r--   0 vsts      (1001) docker     (121)     3540 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/level0/old/rih/bli_scal2rihs_mxn_diag.h
--rw-r--r--   0 vsts      (1001) docker     (121)     9612 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/level0/old/rih/bli_scal2rihs_mxn_uplo.h
--rw-r--r--   0 vsts      (1001) docker     (121)     3410 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/level0/old/rih/bli_setrihs_mxn_diag.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.648227 blis-0.9.1.dev0/blis/_src/frame/include/level0/old/ro/
--rw-r--r--   0 vsts      (1001) docker     (121)     1972 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/level0/old/ro/bli_scal2jros.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2134 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/level0/old/ro/bli_scal2ros.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.648227 blis-0.9.1.dev0/blis/_src/frame/include/level0/old/rpi/
--rw-r--r--   0 vsts      (1001) docker     (121)     2073 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/level0/old/rpi/bli_scal2jrpis.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2325 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/level0/old/rpi/bli_scal2rpis.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.656227 blis-0.9.1.dev0/blis/_src/frame/include/level0/ri/
--rw-r--r--   0 vsts      (1001) docker     (121)     2090 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/level0/ri/bli_absq2ris.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2498 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/level0/ri/bli_abval2ris.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2102 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/level0/ri/bli_add3ris.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2057 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/level0/ri/bli_addjris.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2063 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/level0/ri/bli_addris.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2374 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/level0/ri/bli_axmyris.h
--rw-r--r--   0 vsts      (1001) docker     (121)     3396 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/level0/ri/bli_axpbyjris.h
--rw-r--r--   0 vsts      (1001) docker     (121)     3350 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/level0/ri/bli_axpbyris.h
--rw-r--r--   0 vsts      (1001) docker     (121)     5481 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/level0/ri/bli_axpyjris.h
--rw-r--r--   0 vsts      (1001) docker     (121)     5335 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/level0/ri/bli_axpyris.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1944 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/level0/ri/bli_conjris.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2402 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/level0/ri/bli_copycjris.h
--rw-r--r--   0 vsts      (1001) docker     (121)     3288 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/level0/ri/bli_copyjris.h
--rw-r--r--   0 vsts      (1001) docker     (121)     3215 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/level0/ri/bli_copyris.h
--rw-r--r--   0 vsts      (1001) docker     (121)     3132 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/level0/ri/bli_eqris.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2375 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/level0/ri/bli_invertris.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2280 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/level0/ri/bli_invscaljris.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2738 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/level0/ri/bli_invscalris.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2034 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/level0/ri/bli_neg2ris.h
--rw-r--r--   0 vsts      (1001) docker     (121)     9077 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/level0/ri/bli_scal2jris.h
--rw-r--r--   0 vsts      (1001) docker     (121)     5471 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/level0/ri/bli_scal2ris.h
--rw-r--r--   0 vsts      (1001) docker     (121)     5265 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/level0/ri/bli_scal2ris_mxn.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2656 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/level0/ri/bli_scalcjris.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2235 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/level0/ri/bli_scaljris.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2422 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/level0/ri/bli_scalris.h
--rw-r--r--   0 vsts      (1001) docker     (121)     3309 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/level0/ri/bli_scalris_mxn_uplo.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2005 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/level0/ri/bli_set0ris.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2811 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/level0/ri/bli_sqrt2ris.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2057 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/level0/ri/bli_subjris.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2063 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/level0/ri/bli_subris.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2531 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/level0/ri/bli_swapris.h
--rw-r--r--   0 vsts      (1001) docker     (121)     5459 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/level0/ri/bli_xpbyjris.h
--rw-r--r--   0 vsts      (1001) docker     (121)     5313 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/include/level0/ri/bli_xpbyris.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.656227 blis-0.9.1.dev0/blis/_src/frame/thread/
--rw-r--r--   0 vsts      (1001) docker     (121)     2636 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/thread/bli_l3_decor.h
--rw-r--r--   0 vsts      (1001) docker     (121)     8790 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/thread/bli_l3_decor_openmp.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2065 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/thread/bli_l3_decor_openmp.h
--rw-r--r--   0 vsts      (1001) docker     (121)     8650 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/thread/bli_l3_decor_pthreads.c
--rw-r--r--   0 vsts      (1001) docker     (121)     1941 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/thread/bli_l3_decor_pthreads.h
--rw-r--r--   0 vsts      (1001) docker     (121)     5533 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/thread/bli_l3_decor_single.c
--rw-r--r--   0 vsts      (1001) docker     (121)     1859 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/thread/bli_l3_decor_single.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2646 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/thread/bli_l3_sup_decor.h
--rw-r--r--   0 vsts      (1001) docker     (121)     5123 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/thread/bli_l3_sup_decor_openmp.c
--rw-r--r--   0 vsts      (1001) docker     (121)     1864 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/thread/bli_l3_sup_decor_openmp.h
--rw-r--r--   0 vsts      (1001) docker     (121)     7091 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/thread/bli_l3_sup_decor_pthreads.c
--rw-r--r--   0 vsts      (1001) docker     (121)     1953 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/thread/bli_l3_sup_decor_pthreads.h
--rw-r--r--   0 vsts      (1001) docker     (121)     4905 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/thread/bli_l3_sup_decor_single.c
--rw-r--r--   0 vsts      (1001) docker     (121)     1867 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/thread/bli_l3_sup_decor_single.h
--rw-r--r--   0 vsts      (1001) docker     (121)    15102 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/thread/bli_pthread.c
--rw-r--r--   0 vsts      (1001) docker     (121)     7875 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/thread/bli_pthread.h
--rw-r--r--   0 vsts      (1001) docker     (121)     4729 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/thread/bli_thrcomm.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2627 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/thread/bli_thrcomm.h
--rw-r--r--   0 vsts      (1001) docker     (121)     5596 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/thread/bli_thrcomm_openmp.c
--rw-r--r--   0 vsts      (1001) docker     (121)     3203 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/thread/bli_thrcomm_openmp.h
--rw-r--r--   0 vsts      (1001) docker     (121)     3535 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/thread/bli_thrcomm_pthreads.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2629 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/thread/bli_thrcomm_pthreads.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2733 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/thread/bli_thrcomm_single.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2785 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/thread/bli_thrcomm_single.h
--rw-r--r--   0 vsts      (1001) docker     (121)    49078 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/thread/bli_thread.c
--rw-r--r--   0 vsts      (1001) docker     (121)     8482 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/thread/bli_thread.h
--rw-r--r--   0 vsts      (1001) docker     (121)    20289 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/thread/bli_thrinfo.c
--rw-r--r--   0 vsts      (1001) docker     (121)     6814 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/thread/bli_thrinfo.h
--rw-r--r--   0 vsts      (1001) docker     (121)    10397 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/thread/bli_thrinfo_sup.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2300 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/thread/bli_thrinfo_sup.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.668227 blis-0.9.1.dev0/blis/_src/frame/thread/old/
--rw-r--r--   0 vsts      (1001) docker     (121)     2054 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/thread/old/bli_mutex.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2421 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/thread/old/bli_mutex_openmp.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2469 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/thread/old/bli_mutex_pthreads.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2256 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/thread/old/bli_mutex_single.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.668227 blis-0.9.1.dev0/blis/_src/frame/util/
--rw-r--r--   0 vsts      (1001) docker     (121)     2343 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/util/bli_util.h
--rw-r--r--   0 vsts      (1001) docker     (121)     9068 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/util/bli_util_check.c
--rw-r--r--   0 vsts      (1001) docker     (121)     4264 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/util/bli_util_check.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2873 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/util/bli_util_fpa.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2447 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/util/bli_util_fpa.h
--rw-r--r--   0 vsts      (1001) docker     (121)     5973 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/util/bli_util_ft.h
--rw-r--r--   0 vsts      (1001) docker     (121)    16310 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/util/bli_util_oapi.c
--rw-r--r--   0 vsts      (1001) docker     (121)     4522 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/util/bli_util_oapi.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1977 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/util/bli_util_oapi_ba.c
--rw-r--r--   0 vsts      (1001) docker     (121)     1975 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/util/bli_util_oapi_ex.c
--rw-r--r--   0 vsts      (1001) docker     (121)    12097 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/util/bli_util_tapi.c
--rw-r--r--   0 vsts      (1001) docker     (121)     5854 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/util/bli_util_tapi.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1975 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/util/bli_util_tapi_ba.c
--rw-r--r--   0 vsts      (1001) docker     (121)     1973 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/util/bli_util_tapi_ex.c
--rw-r--r--   0 vsts      (1001) docker     (121)    33286 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/util/bli_util_unb_var1.c
--rw-r--r--   0 vsts      (1001) docker     (121)     5577 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/frame/util/bli_util_unb_var1.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.500226 blis-0.9.1.dev0/blis/_src/include/
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.668227 blis-0.9.1.dev0/blis/_src/include/darwin-firestorm/
--rw-r--r--   0 vsts      (1001) docker     (121)  1241655 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/include/darwin-firestorm/blis.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.672227 blis-0.9.1.dev0/blis/_src/include/darwin-generic/
--rw-r--r--   0 vsts      (1001) docker     (121)  1239020 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/include/darwin-generic/blis.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.672227 blis-0.9.1.dev0/blis/_src/include/darwin-x86_64/
--rw-r--r--   0 vsts      (1001) docker     (121)  1282614 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/include/darwin-x86_64/blis.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.680227 blis-0.9.1.dev0/blis/_src/include/darwin-x86_64_no_skx/
--rw-r--r--   0 vsts      (1001) docker     (121)  1269093 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/include/darwin-x86_64_no_skx/blis.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.680227 blis-0.9.1.dev0/blis/_src/include/darwin-x86_64_no_zen2/
--rw-r--r--   0 vsts      (1001) docker     (121)  1274228 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/include/darwin-x86_64_no_zen2/blis.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.684227 blis-0.9.1.dev0/blis/_src/include/darwin-x86_64_no_zen3/
--rw-r--r--   0 vsts      (1001) docker     (121)  1280323 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/include/darwin-x86_64_no_zen3/blis.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.684227 blis-0.9.1.dev0/blis/_src/include/linux-arm64/
--rw-r--r--   0 vsts      (1001) docker     (121)  1246399 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/include/linux-arm64/blis.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.684227 blis-0.9.1.dev0/blis/_src/include/linux-arm64_no_sve/
--rw-r--r--   0 vsts      (1001) docker     (121)  1243881 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/include/linux-arm64_no_sve/blis.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.688227 blis-0.9.1.dev0/blis/_src/include/linux-generic/
--rw-r--r--   0 vsts      (1001) docker     (121)  1239020 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/include/linux-generic/blis.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.688227 blis-0.9.1.dev0/blis/_src/include/linux-power9/
--rw-r--r--   0 vsts      (1001) docker     (121)  1239472 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/include/linux-power9/blis.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.692227 blis-0.9.1.dev0/blis/_src/include/linux-x86_64/
--rw-r--r--   0 vsts      (1001) docker     (121)  1282614 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/include/linux-x86_64/blis.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.692227 blis-0.9.1.dev0/blis/_src/include/linux-x86_64_no_skx/
--rw-r--r--   0 vsts      (1001) docker     (121)  1269093 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/include/linux-x86_64_no_skx/blis.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.696227 blis-0.9.1.dev0/blis/_src/include/linux-x86_64_no_zen2/
--rw-r--r--   0 vsts      (1001) docker     (121)  1274228 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/include/linux-x86_64_no_zen2/blis.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.696227 blis-0.9.1.dev0/blis/_src/include/linux-x86_64_no_zen3/
--rw-r--r--   0 vsts      (1001) docker     (121)  1280323 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/include/linux-x86_64_no_zen3/blis.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.700227 blis-0.9.1.dev0/blis/_src/include/windows-generic/
--rw-r--r--   0 vsts      (1001) docker     (121)  1281621 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/include/windows-generic/blis.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.700227 blis-0.9.1.dev0/blis/_src/include/windows-x86_64/
--rw-r--r--   0 vsts      (1001) docker     (121)  1326521 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/include/windows-x86_64/blis.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.504226 blis-0.9.1.dev0/blis/_src/kernels/
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.700227 blis-0.9.1.dev0/blis/_src/kernels/armsve/
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.704227 blis-0.9.1.dev0/blis/_src/kernels/armsve/1m/
--rw-r--r--   0 vsts      (1001) docker     (121)     2260 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/armsve/1m/armsve512_asm_transpose_d8x2.h
--rw-r--r--   0 vsts      (1001) docker     (121)     4853 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/armsve/1m/armsve512_asm_transpose_d8x8.h
--rw-r--r--   0 vsts      (1001) docker     (121)     7979 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/armsve/1m/bli_dpackm_armsve256_int_8xk.c
--rw-r--r--   0 vsts      (1001) docker     (121)    13414 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/armsve/1m/bli_dpackm_armsve512_asm_10xk.c
--rw-r--r--   0 vsts      (1001) docker     (121)    13673 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/armsve/1m/bli_dpackm_armsve512_asm_16xk.c
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.704227 blis-0.9.1.dev0/blis/_src/kernels/armsve/1m/old/
--rw-r--r--   0 vsts      (1001) docker     (121)    13739 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/armsve/1m/old/bli_dpackm_armsve512_int_12xk.c
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.712227 blis-0.9.1.dev0/blis/_src/kernels/armsve/3/
--rw-r--r--   0 vsts      (1001) docker     (121)    13068 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/armsve/3/armsve_asm_2vx10.h
--rw-r--r--   0 vsts      (1001) docker     (121)     7360 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/armsve/3/armsve_asm_2vx10cmplx.h
--rw-r--r--   0 vsts      (1001) docker     (121)     6236 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/armsve/3/armsve_asm_macros.h
--rw-r--r--   0 vsts      (1001) docker     (121)     4155 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/armsve/3/armsve_asm_macros_cmplx.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1999 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/armsve/3/armsve_asm_macros_dcomplex.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1951 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/armsve/3/armsve_asm_macros_double.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2000 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/armsve/3/armsve_asm_macros_scomplex.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1952 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/armsve/3/armsve_asm_macros_single.h
--rw-r--r--   0 vsts      (1001) docker     (121)     3760 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/armsve/3/bli_armsve_utils.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2181 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/armsve/3/bli_armsve_utils.h
--rw-r--r--   0 vsts      (1001) docker     (121)    16175 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/armsve/3/bli_gemm_armsve_asm_c2vx10_unindexed.c
--rw-r--r--   0 vsts      (1001) docker     (121)    16261 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/armsve/3/bli_gemm_armsve_asm_d2vx10_unindexed.c
--rw-r--r--   0 vsts      (1001) docker     (121)    15390 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/armsve/3/bli_gemm_armsve_asm_s2vx10_unindexed.c
--rw-r--r--   0 vsts      (1001) docker     (121)    16121 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/armsve/3/bli_gemm_armsve_asm_z2vx10_unindexed.c
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.712227 blis-0.9.1.dev0/blis/_src/kernels/armsve/3/old/
--rw-r--r--   0 vsts      (1001) docker     (121)     7945 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/armsve/3/old/armsve_asm_2vx7cmplx.h
--rw-r--r--   0 vsts      (1001) docker     (121)     6909 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/armsve/3/old/armsve_asm_2vx8cmplx.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1954 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/armsve/3/old/armsve_asm_macros_half.h
--rw-r--r--   0 vsts      (1001) docker     (121)    52816 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/armsve/3/old/bli_gemm_armsve256_asm_d8x8.c
--rw-r--r--   0 vsts      (1001) docker     (121)    18788 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/armsve/3/old/bli_gemm_armsve_asm_sh2vx10_unindexed.c
--rw-r--r--   0 vsts      (1001) docker     (121)    14679 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/armsve/3/old/bli_gemm_armsve_asm_z2vx7_unindexed.c
--rw-r--r--   0 vsts      (1001) docker     (121)    16041 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/armsve/3/old/bli_gemm_armsve_asm_z2vx8_unindexed.c
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.712227 blis-0.9.1.dev0/blis/_src/kernels/armsve/3/old/sup/
--rw-r--r--   0 vsts      (1001) docker     (121)    12900 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/armsve/3/old/sup/bli_gemmsup_armsve_ref.c
--rw-r--r--   0 vsts      (1001) docker     (121)    25880 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/armsve/3/old/sup/bli_gemmsup_cv_armsve_asm_d2vx10_unindexed.c
--rw-r--r--   0 vsts      (1001) docker     (121)    20498 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/armsve/3/old/sup/bli_gemmsup_rv_armsve_asm_d2vx10_unindexed.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2656 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/armsve/bli_kernels_armsve.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.712227 blis-0.9.1.dev0/blis/_src/kernels/armv7a/
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.712227 blis-0.9.1.dev0/blis/_src/kernels/armv7a/3/
--rw-r--r--   0 vsts      (1001) docker     (121)     5506 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/armv7a/3/bli_gemm_armv7a_asm_d4x4.c
--rw-r--r--   0 vsts      (1001) docker     (121)    12462 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/armv7a/3/bli_gemm_armv7a_int_d4x4.c
--rw-r--r--   0 vsts      (1001) docker     (121)     1974 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/armv7a/bli_kernels_armv7a.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.716227 blis-0.9.1.dev0/blis/_src/kernels/armv8a/
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.716227 blis-0.9.1.dev0/blis/_src/kernels/armv8a/1m/
--rw-r--r--   0 vsts      (1001) docker     (121)    10641 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/armv8a/1m/bli_packm_armv8a_int_d6xk.c
--rw-r--r--   0 vsts      (1001) docker     (121)    12067 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/armv8a/1m/bli_packm_armv8a_int_d8xk.c
--rw-r--r--   0 vsts      (1001) docker     (121)    15957 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/armv8a/1m/bli_packm_armv8a_int_s12xk.c
--rw-r--r--   0 vsts      (1001) docker     (121)    12799 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/armv8a/1m/bli_packm_armv8a_int_s8xk.c
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.716227 blis-0.9.1.dev0/blis/_src/kernels/armv8a/3/
--rw-r--r--   0 vsts      (1001) docker     (121)     2195 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/armv8a/3/armv8a_asm_d2x2.h
--rw-r--r--   0 vsts      (1001) docker     (121)     4187 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/armv8a/3/armv8a_asm_utils.h
--rw-r--r--   0 vsts      (1001) docker     (121)    85781 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/armv8a/3/bli_gemm_armv8a_asm_d6x8.c
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.716227 blis-0.9.1.dev0/blis/_src/kernels/armv8a/3/old/
--rw-r--r--   0 vsts      (1001) docker     (121)    11291 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/armv8a/3/old/bli_gemm_armv8a_asm_d4x4.c
--rw-r--r--   0 vsts      (1001) docker     (121)    14722 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/armv8a/3/old/bli_gemm_armv8a_asm_d6x8r.c
--rw-r--r--   0 vsts      (1001) docker     (121)    12051 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/armv8a/3/old/bli_gemm_armv8a_asm_d8x4.c
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.716227 blis-0.9.1.dev0/blis/_src/kernels/armv8a/3/sup/
--rw-r--r--   0 vsts      (1001) docker     (121)    12901 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/armv8a/3/sup/bli_gemmsup_armv8a_ref.c
--rw-r--r--   0 vsts      (1001) docker     (121)    20091 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/armv8a/3/sup/bli_gemmsup_rd_armv8a_asm_d6x8m.c
--rw-r--r--   0 vsts      (1001) docker     (121)    22063 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/armv8a/3/sup/bli_gemmsup_rd_armv8a_asm_d6x8n.c
--rw-r--r--   0 vsts      (1001) docker     (121)    18537 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/armv8a/3/sup/bli_gemmsup_rv_armv8a_asm_d4x8m.c
--rw-r--r--   0 vsts      (1001) docker     (121)    18689 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/armv8a/3/sup/bli_gemmsup_rv_armv8a_asm_d4x8n.c
--rw-r--r--   0 vsts      (1001) docker     (121)    21409 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/armv8a/3/sup/bli_gemmsup_rv_armv8a_asm_d6x8m.c
--rw-r--r--   0 vsts      (1001) docker     (121)    20655 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/armv8a/3/sup/bli_gemmsup_rv_armv8a_asm_d6x8n.c
--rw-r--r--   0 vsts      (1001) docker     (121)    17688 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/armv8a/3/sup/bli_gemmsup_rv_armv8a_asm_d8x4m.c
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.720227 blis-0.9.1.dev0/blis/_src/kernels/armv8a/3/sup/d3x4/
--rw-r--r--   0 vsts      (1001) docker     (121)    13051 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/armv8a/3/sup/d3x4/bli_gemmsup_rd_armv8a_asm_d3x4.c
--rw-r--r--   0 vsts      (1001) docker     (121)    15813 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/armv8a/3/sup/d3x4/bli_gemmsup_rd_armv8a_asm_d6x3.c
--rw-r--r--   0 vsts      (1001) docker     (121)    14963 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/armv8a/3/sup/d3x4/bli_gemmsup_rd_armv8a_int_d2x8.c
--rw-r--r--   0 vsts      (1001) docker     (121)    12124 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/armv8a/3/sup/d3x4/bli_gemmsup_rd_armv8a_int_d3x4.c
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.720227 blis-0.9.1.dev0/blis/_src/kernels/armv8a/3/sup/d6x4/
--rw-r--r--   0 vsts      (1001) docker     (121)    16425 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/armv8a/3/sup/d6x4/bli_gemmsup_rv_armv8a_int_d3x8mn.c
--rw-r--r--   0 vsts      (1001) docker     (121)    18893 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/armv8a/3/sup/d6x4/bli_gemmsup_rv_armv8a_int_d6x4mn.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2926 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/armv8a/bli_kernels_armv8a.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.720227 blis-0.9.1.dev0/blis/_src/kernels/bgq/
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.720227 blis-0.9.1.dev0/blis/_src/kernels/bgq/1/
--rw-r--r--   0 vsts      (1001) docker     (121)     2960 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/bgq/1/bli_axpyv_bgq_int.c
--rw-r--r--   0 vsts      (1001) docker     (121)     3380 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/bgq/1/bli_dotv_bgq_int.c
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.720227 blis-0.9.1.dev0/blis/_src/kernels/bgq/1f/
--rw-r--r--   0 vsts      (1001) docker     (121)     5553 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/bgq/1f/bli_axpyf_bgq_int.c
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.720227 blis-0.9.1.dev0/blis/_src/kernels/bgq/3/
--rw-r--r--   0 vsts      (1001) docker     (121)    13754 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/bgq/3/bli_gemm_bgq_int_8x8.c
--rw-r--r--   0 vsts      (1001) docker     (121)     1902 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/bgq/bli_kernels_bgq.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.720227 blis-0.9.1.dev0/blis/_src/kernels/bulldozer/
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.720227 blis-0.9.1.dev0/blis/_src/kernels/bulldozer/3/
--rw-r--r--   0 vsts      (1001) docker     (121)    51743 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/bulldozer/3/bli_gemm_bulldozer_asm_d4x6_fma4.c
--rw-r--r--   0 vsts      (1001) docker     (121)     1906 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/bulldozer/bli_kernels_bulldozer.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.720227 blis-0.9.1.dev0/blis/_src/kernels/haswell/
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.720227 blis-0.9.1.dev0/blis/_src/kernels/haswell/1m/
--rw-r--r--   0 vsts      (1001) docker     (121)    12085 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/haswell/1m/bli_packm_haswell_asm_c3xk.c
--rw-r--r--   0 vsts      (1001) docker     (121)    12657 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/haswell/1m/bli_packm_haswell_asm_c8xk.c
--rw-r--r--   0 vsts      (1001) docker     (121)    11930 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/haswell/1m/bli_packm_haswell_asm_d6xk.c
--rw-r--r--   0 vsts      (1001) docker     (121)    12196 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/haswell/1m/bli_packm_haswell_asm_d8xk.c
--rw-r--r--   0 vsts      (1001) docker     (121)    17802 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/haswell/1m/bli_packm_haswell_asm_s16xk.c
--rw-r--r--   0 vsts      (1001) docker     (121)    13674 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/haswell/1m/bli_packm_haswell_asm_s6xk.c
--rw-r--r--   0 vsts      (1001) docker     (121)    12174 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/haswell/1m/bli_packm_haswell_asm_z3xk.c
--rw-r--r--   0 vsts      (1001) docker     (121)    12556 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/haswell/1m/bli_packm_haswell_asm_z4xk.c
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.724227 blis-0.9.1.dev0/blis/_src/kernels/haswell/3/
--rw-r--r--   0 vsts      (1001) docker     (121)    56813 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/haswell/3/bli_gemm_haswell_asm_d6x8.c
--rw-r--r--   0 vsts      (1001) docker     (121)    40396 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/haswell/3/bli_gemm_haswell_asm_d8x6.c
--rw-r--r--   0 vsts      (1001) docker     (121)    41819 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/haswell/3/bli_gemmtrsm_l_haswell_asm_d6x8.c
--rw-r--r--   0 vsts      (1001) docker     (121)    42186 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/haswell/3/bli_gemmtrsm_u_haswell_asm_d6x8.c
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.724227 blis-0.9.1.dev0/blis/_src/kernels/haswell/3/old/
--rw-r--r--   0 vsts      (1001) docker     (121)    68808 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/haswell/3/old/bli_gemm_haswell_asm_d12x4.c
--rw-r--r--   0 vsts      (1001) docker     (121)    64360 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/haswell/3/old/bli_gemm_haswell_asm_d4x12.c
--rw-r--r--   0 vsts      (1001) docker     (121)   115770 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/haswell/3/old/bli_gemm_haswell_asm_d6x8.c
--rw-r--r--   0 vsts      (1001) docker     (121)   116155 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/haswell/3/old/bli_gemm_haswell_asm_d8x6.c
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.728227 blis-0.9.1.dev0/blis/_src/kernels/haswell/3/sup/
--rw-r--r--   0 vsts      (1001) docker     (121)    52381 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/haswell/3/sup/bli_gemmsup_rd_haswell_asm_d6x8m.c
--rw-r--r--   0 vsts      (1001) docker     (121)    63958 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/haswell/3/sup/bli_gemmsup_rd_haswell_asm_d6x8n.c
--rw-r--r--   0 vsts      (1001) docker     (121)    87529 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/haswell/3/sup/bli_gemmsup_rd_haswell_asm_s6x16m.c
--rw-r--r--   0 vsts      (1001) docker     (121)    64915 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/haswell/3/sup/bli_gemmsup_rd_haswell_asm_s6x16n.c
--rw-r--r--   0 vsts      (1001) docker     (121)    82422 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/haswell/3/sup/bli_gemmsup_rv_haswell_asm_d6x8m.c
--rw-r--r--   0 vsts      (1001) docker     (121)   113882 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/haswell/3/sup/bli_gemmsup_rv_haswell_asm_d6x8n.c
--rw-r--r--   0 vsts      (1001) docker     (121)   135283 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/haswell/3/sup/bli_gemmsup_rv_haswell_asm_s6x16m.c
--rw-r--r--   0 vsts      (1001) docker     (121)   145184 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/haswell/3/sup/bli_gemmsup_rv_haswell_asm_s6x16n.c
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.728227 blis-0.9.1.dev0/blis/_src/kernels/haswell/3/sup/d6x8/
--rw-r--r--   0 vsts      (1001) docker     (121)     5859 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/haswell/3/sup/d6x8/bli_gemmsup_r_haswell_ref_dMx1.c
--rw-r--r--   0 vsts      (1001) docker     (121)    45366 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/haswell/3/sup/d6x8/bli_gemmsup_rd_haswell_asm_dMx1.c
--rw-r--r--   0 vsts      (1001) docker     (121)    49003 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/haswell/3/sup/d6x8/bli_gemmsup_rd_haswell_asm_dMx2.c
--rw-r--r--   0 vsts      (1001) docker     (121)    38513 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/haswell/3/sup/d6x8/bli_gemmsup_rd_haswell_asm_dMx4.c
--rw-r--r--   0 vsts      (1001) docker     (121)    44125 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/haswell/3/sup/d6x8/bli_gemmsup_rd_haswell_asm_dMx8.c
--rw-r--r--   0 vsts      (1001) docker     (121)    66482 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/haswell/3/sup/d6x8/bli_gemmsup_rv_haswell_asm_dMx2.c
--rw-r--r--   0 vsts      (1001) docker     (121)    70571 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/haswell/3/sup/d6x8/bli_gemmsup_rv_haswell_asm_dMx4.c
--rw-r--r--   0 vsts      (1001) docker     (121)    84809 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/haswell/3/sup/d6x8/bli_gemmsup_rv_haswell_asm_dMx6.c
--rw-r--r--   0 vsts      (1001) docker     (121)    91255 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/haswell/3/sup/d6x8/bli_gemmsup_rv_haswell_asm_dMx8.c
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.728227 blis-0.9.1.dev0/blis/_src/kernels/haswell/3/sup/d6x8/old/
--rw-r--r--   0 vsts      (1001) docker     (121)   123287 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/haswell/3/sup/d6x8/old/bli_gemmsup_rd_haswell_asm_d6x8.c
--rw-r--r--   0 vsts      (1001) docker     (121)   304617 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/haswell/3/sup/d6x8/old/bli_gemmsup_rv_haswell_asm_d6x8.c
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.732227 blis-0.9.1.dev0/blis/_src/kernels/haswell/3/sup/old/
--rw-r--r--   0 vsts      (1001) docker     (121)   141528 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/haswell/3/sup/old/bli_gemmsup_rd_haswell_asm_d6x8.c
--rw-r--r--   0 vsts      (1001) docker     (121)   149744 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/haswell/3/sup/old/bli_gemmsup_rd_haswell_asm_d6x8m.c
--rw-r--r--   0 vsts      (1001) docker     (121)   156805 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/haswell/3/sup/old/bli_gemmsup_rd_haswell_asm_d6x8n.c
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.740227 blis-0.9.1.dev0/blis/_src/kernels/haswell/3/sup/s6x16/
--rw-r--r--   0 vsts      (1001) docker     (121)     7643 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/haswell/3/sup/s6x16/bli_gemmsup_r_haswell_ref_sMx1.c
--rw-r--r--   0 vsts      (1001) docker     (121)    46512 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/haswell/3/sup/s6x16/bli_gemmsup_rd_haswell_asm_sMx1.c
--rw-r--r--   0 vsts      (1001) docker     (121)    42106 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/haswell/3/sup/s6x16/bli_gemmsup_rd_haswell_asm_sMx12.c
--rw-r--r--   0 vsts      (1001) docker     (121)    45181 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/haswell/3/sup/s6x16/bli_gemmsup_rd_haswell_asm_sMx16.c
--rw-r--r--   0 vsts      (1001) docker     (121)    49994 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/haswell/3/sup/s6x16/bli_gemmsup_rd_haswell_asm_sMx2.c
--rw-r--r--   0 vsts      (1001) docker     (121)    39761 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/haswell/3/sup/s6x16/bli_gemmsup_rd_haswell_asm_sMx4.c
--rw-r--r--   0 vsts      (1001) docker     (121)    42097 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/haswell/3/sup/s6x16/bli_gemmsup_rd_haswell_asm_sMx8.c
--rw-r--r--   0 vsts      (1001) docker     (121)   105003 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/haswell/3/sup/s6x16/bli_gemmsup_rv_haswell_asm_sMx12.c
--rw-r--r--   0 vsts      (1001) docker     (121)   118893 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/haswell/3/sup/s6x16/bli_gemmsup_rv_haswell_asm_sMx16.c
--rw-r--r--   0 vsts      (1001) docker     (121)    68445 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/haswell/3/sup/s6x16/bli_gemmsup_rv_haswell_asm_sMx2.c
--rw-r--r--   0 vsts      (1001) docker     (121)    74065 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/haswell/3/sup/s6x16/bli_gemmsup_rv_haswell_asm_sMx4.c
--rw-r--r--   0 vsts      (1001) docker     (121)    96722 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/haswell/3/sup/s6x16/bli_gemmsup_rv_haswell_asm_sMx6.c
--rw-r--r--   0 vsts      (1001) docker     (121)    84611 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/haswell/3/sup/s6x16/bli_gemmsup_rv_haswell_asm_sMx8.c
--rw-r--r--   0 vsts      (1001) docker     (121)    12533 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/haswell/bli_kernels_haswell.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.740227 blis-0.9.1.dev0/blis/_src/kernels/knc/
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.740227 blis-0.9.1.dev0/blis/_src/kernels/knc/3/
--rw-r--r--   0 vsts      (1001) docker     (121)    21055 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/knc/3/bli_dgemm_knc_asm_30x8.c
--rw-r--r--   0 vsts      (1001) docker     (121)    21252 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/knc/3/bli_sgemm_knc_asm_30x16.c
--rw-r--r--   0 vsts      (1001) docker     (121)     1771 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/knc/bli_kernels_knc.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.740227 blis-0.9.1.dev0/blis/_src/kernels/knl/
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.740227 blis-0.9.1.dev0/blis/_src/kernels/knl/1m/
--rw-r--r--   0 vsts      (1001) docker     (121)    19685 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/knl/1m/bli_dpackm_knl_asm_24x8.c
--rw-r--r--   0 vsts      (1001) docker     (121)    20632 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/knl/1m/bli_spackm_knl_asm_24x16.c
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.740227 blis-0.9.1.dev0/blis/_src/kernels/knl/1m/old/
--rw-r--r--   0 vsts      (1001) docker     (121)    15691 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/knl/1m/old/bli_packm_knl_asm_30x8.c
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.740227 blis-0.9.1.dev0/blis/_src/kernels/knl/3/
--rw-r--r--   0 vsts      (1001) docker     (121)    19570 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/knl/3/bli_dgemm_knl_asm_24x8.c
--rw-r--r--   0 vsts      (1001) docker     (121)    19430 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/knl/3/bli_sgemm_knl_asm_24x16.c
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.744227 blis-0.9.1.dev0/blis/_src/kernels/knl/3/other/
--rw-r--r--   0 vsts      (1001) docker     (121)    24893 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/knl/3/other/bli_dgemm_knl_asm_12x16.c
--rw-r--r--   0 vsts      (1001) docker     (121)    23763 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/knl/3/other/bli_dgemm_knl_asm_30x8.c
--rw-r--r--   0 vsts      (1001) docker     (121)    15936 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/knl/3/other/bli_dgemm_knl_asm_30x8_knc.c
--rw-r--r--   0 vsts      (1001) docker     (121)    22049 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/knl/3/other/bli_dgemm_knl_asm_8x24.c
--rw-r--r--   0 vsts      (1001) docker     (121)    16389 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/knl/3/other/bli_sgemm_knl_asm_30x16_knc.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2181 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/knl/bli_kernels_knl.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.500226 blis-0.9.1.dev0/blis/_src/kernels/old/
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.744227 blis-0.9.1.dev0/blis/_src/kernels/old/c99/
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.744227 blis-0.9.1.dev0/blis/_src/kernels/old/c99/3/
--rw-r--r--   0 vsts      (1001) docker     (121)     6327 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/old/c99/3/bli_gemm_c99_4x4.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2808 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/old/c99/3/bli_gemmtrsm_l_c99_4x4.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2808 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/old/c99/3/bli_gemmtrsm_u_c99_4x4.c
--rw-r--r--   0 vsts      (1001) docker     (121)     5971 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/old/c99/3/bli_trsm_l_c99_4x4.c
--rw-r--r--   0 vsts      (1001) docker     (121)     6001 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/old/c99/3/bli_trsm_u_c99_4x4.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2374 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/old/c99/bli_kernels_c99.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.500226 blis-0.9.1.dev0/blis/_src/kernels/old/loongson3a/
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.744227 blis-0.9.1.dev0/blis/_src/kernels/old/loongson3a/3/
--rw-r--r--   0 vsts      (1001) docker     (121)    23051 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/old/loongson3a/3/bli_gemm_loongson3a_opt_d4x4.c
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.500226 blis-0.9.1.dev0/blis/_src/kernels/old/nacl/
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.500226 blis-0.9.1.dev0/blis/_src/kernels/old/nacl/pnacl/
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.748227 blis-0.9.1.dev0/blis/_src/kernels/old/nacl/pnacl/1/
--rw-r--r--   0 vsts      (1001) docker     (121)     4948 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/old/nacl/pnacl/1/bli_axpyv_opt.c
--rw-r--r--   0 vsts      (1001) docker     (121)    14220 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/old/nacl/pnacl/1/bli_dotv_opt.c
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.748227 blis-0.9.1.dev0/blis/_src/kernels/old/nacl/pnacl/3/
--rw-r--r--   0 vsts      (1001) docker     (121)    14195 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/old/nacl/pnacl/3/bli_gemm_opt.c
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.500226 blis-0.9.1.dev0/blis/_src/kernels/old/x86/
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.748227 blis-0.9.1.dev0/blis/_src/kernels/old/x86/1m/
--rw-r--r--   0 vsts      (1001) docker     (121)    10427 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/old/x86/1m/bli_packm_2xk.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2056 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/old/x86/1m/bli_packm_2xk.h
--rw-r--r--   0 vsts      (1001) docker     (121)    11378 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/old/x86/1m/bli_packm_4xk.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2056 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/old/x86/1m/bli_packm_4xk.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.748227 blis-0.9.1.dev0/blis/_src/kernels/old/x86/3/
--rw-r--r--   0 vsts      (1001) docker     (121)    16862 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/old/x86/3/bli_gemm_opt_d2x4.c
--rw-r--r--   0 vsts      (1001) docker     (121)    15273 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/old/x86/3/bli_gemm_opt_d4x2.c
--rw-r--r--   0 vsts      (1001) docker     (121)    21386 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/old/x86/3/bli_gemmtrsm_l_opt_d4x2.c
--rw-r--r--   0 vsts      (1001) docker     (121)    21653 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/old/x86/3/bli_gemmtrsm_u_opt_d4x2.c
--rw-r--r--   0 vsts      (1001) docker     (121)     9615 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/old/x86/3/bli_trsm_l_opt_d4x2.c
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.752227 blis-0.9.1.dev0/blis/_src/kernels/penryn/
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.752227 blis-0.9.1.dev0/blis/_src/kernels/penryn/1/
--rw-r--r--   0 vsts      (1001) docker     (121)     4536 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/penryn/1/bli_axpyv_penryn_int.c
--rw-r--r--   0 vsts      (1001) docker     (121)     3996 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/penryn/1/bli_dotv_penryn_int.c
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.752227 blis-0.9.1.dev0/blis/_src/kernels/penryn/1f/
--rw-r--r--   0 vsts      (1001) docker     (121)     6872 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/penryn/1f/bli_axpy2v_penryn_int.c
--rw-r--r--   0 vsts      (1001) docker     (121)     6321 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/penryn/1f/bli_axpyf_penryn_int.c
--rw-r--r--   0 vsts      (1001) docker     (121)     5001 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/penryn/1f/bli_dotaxpyv_penryn_int.c
--rw-r--r--   0 vsts      (1001) docker     (121)     9544 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/penryn/1f/bli_dotxaxpyf_penryn_int.c
--rw-r--r--   0 vsts      (1001) docker     (121)     8405 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/penryn/1f/bli_dotxf_penryn_int.c
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.756227 blis-0.9.1.dev0/blis/_src/kernels/penryn/3/
--rw-r--r--   0 vsts      (1001) docker     (121)    25693 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/penryn/3/bli_gemm_penryn_asm_d4x4.c
--rw-r--r--   0 vsts      (1001) docker     (121)    16554 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/penryn/3/bli_gemmtrsm_l_penryn_asm_d4x4.c
--rw-r--r--   0 vsts      (1001) docker     (121)    15801 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/penryn/3/bli_gemmtrsm_u_penryn_asm_d4x4.c
--rw-r--r--   0 vsts      (1001) docker     (121)     7998 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/penryn/3/bli_trsm_l_penryn_asm_d4x4.c
--rw-r--r--   0 vsts      (1001) docker     (121)     8020 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/penryn/3/bli_trsm_u_penryn_asm_d4x4.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2000 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/penryn/bli_kernels_penryn.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.756227 blis-0.9.1.dev0/blis/_src/kernels/piledriver/
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.756227 blis-0.9.1.dev0/blis/_src/kernels/piledriver/3/
--rw-r--r--   0 vsts      (1001) docker     (121)    48133 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/piledriver/3/bli_gemm_piledriver_asm_d8x3.c
--rw-r--r--   0 vsts      (1001) docker     (121)     1910 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/piledriver/bli_kernels_piledriver.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.756227 blis-0.9.1.dev0/blis/_src/kernels/power10/
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.756227 blis-0.9.1.dev0/blis/_src/kernels/power10/3/
--rw-r--r--   0 vsts      (1001) docker     (121)     6779 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/power10/3/bli_dgemm_power10_mma.c
--rw-r--r--   0 vsts      (1001) docker     (121)     4759 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/power10/3/bli_i16gemm_power10_mma.c
--rw-r--r--   0 vsts      (1001) docker     (121)     4787 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/power10/3/bli_i16sgemm_power10_mma.c
--rw-r--r--   0 vsts      (1001) docker     (121)     4757 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/power10/3/bli_i4gemm_power10_mma.c
--rw-r--r--   0 vsts      (1001) docker     (121)     4753 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/power10/3/bli_i8gemm_power10_mma.c
--rw-r--r--   0 vsts      (1001) docker     (121)     4749 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/power10/3/bli_sbgemm_power10_mma.c
--rw-r--r--   0 vsts      (1001) docker     (121)     5194 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/power10/3/bli_sgemm_power10_mma.c
--rw-r--r--   0 vsts      (1001) docker     (121)     4726 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/power10/3/bli_shgemm_power10_mma.c
--rw-r--r--   0 vsts      (1001) docker     (121)     3155 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/power10/3/vector_int_macros.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1786 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/power10/bli_kernels_power10.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.760227 blis-0.9.1.dev0/blis/_src/kernels/power7/
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.760227 blis-0.9.1.dev0/blis/_src/kernels/power7/3/
--rw-r--r--   0 vsts      (1001) docker     (121)    21458 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/power7/3/bli_gemm_power7_int_8x4.c
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.760227 blis-0.9.1.dev0/blis/_src/kernels/power7/3/test/
--rw-r--r--   0 vsts      (1001) docker     (121)    21458 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/power7/3/test/bli_gemm_power7_int_8x4.c
--rw-r--r--   0 vsts      (1001) docker     (121)     3308 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/power7/3/test/bli_gemm_power7_int_8x4.h
--rw-r--r--   0 vsts      (1001) docker     (121)      573 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/power7/3/test/blis_utest.h
--rw-r--r--   0 vsts      (1001) docker     (121)     3687 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/power7/3/test/exp.c
--rw-r--r--   0 vsts      (1001) docker     (121)     1895 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/power7/bli_kernels_power7.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.760227 blis-0.9.1.dev0/blis/_src/kernels/power9/
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.760227 blis-0.9.1.dev0/blis/_src/kernels/power9/3/
--rw-r--r--   0 vsts      (1001) docker     (121)     8280 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/power9/3/bli_gemm_power9_asm_d12x6.c
--rw-r--r--   0 vsts      (1001) docker     (121)    87665 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/power9/3/bli_pwr9_asm_macros_12x6.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1761 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/power9/bli_kernels_power9.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.760227 blis-0.9.1.dev0/blis/_src/kernels/sandybridge/
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.760227 blis-0.9.1.dev0/blis/_src/kernels/sandybridge/3/
--rw-r--r--   0 vsts      (1001) docker     (121)    62718 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/sandybridge/3/bli_gemm_sandybridge_asm_d8x4.c
--rw-r--r--   0 vsts      (1001) docker     (121)    14538 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/sandybridge/3/bli_gemm_sandybridge_int_d8x4.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2155 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/sandybridge/bli_kernels_sandybridge.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.764227 blis-0.9.1.dev0/blis/_src/kernels/skx/
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.764227 blis-0.9.1.dev0/blis/_src/kernels/skx/3/
--rw-r--r--   0 vsts      (1001) docker     (121)    15652 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/skx/3/bli_dgemm_skx_asm_16x12_l2.c
--rw-r--r--   0 vsts      (1001) docker     (121)    11565 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/skx/3/bli_dgemm_skx_asm_16x14.c
--rw-r--r--   0 vsts      (1001) docker     (121)    16591 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/skx/3/bli_sgemm_skx_asm_32x12_l2.c
--rw-r--r--   0 vsts      (1001) docker     (121)     1881 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/skx/bli_kernels_skx.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.764227 blis-0.9.1.dev0/blis/_src/kernels/zen/
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.768227 blis-0.9.1.dev0/blis/_src/kernels/zen/1/
--rw-r--r--   0 vsts      (1001) docker     (121)    17207 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/zen/1/bli_amaxv_zen_int.c
--rw-r--r--   0 vsts      (1001) docker     (121)     8307 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/zen/1/bli_axpyv_zen_int.c
--rw-r--r--   0 vsts      (1001) docker     (121)    15587 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/zen/1/bli_axpyv_zen_int10.c
--rw-r--r--   0 vsts      (1001) docker     (121)    11667 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/zen/1/bli_copyv_zen_int.c
--rw-r--r--   0 vsts      (1001) docker     (121)     9123 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/zen/1/bli_dotv_zen_int.c
--rw-r--r--   0 vsts      (1001) docker     (121)    14192 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/zen/1/bli_dotv_zen_int10.c
--rw-r--r--   0 vsts      (1001) docker     (121)     9562 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/zen/1/bli_dotxv_zen_int.c
--rw-r--r--   0 vsts      (1001) docker     (121)     7363 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/zen/1/bli_scalv_zen_int.c
--rw-r--r--   0 vsts      (1001) docker     (121)    13541 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/zen/1/bli_scalv_zen_int10.c
--rw-r--r--   0 vsts      (1001) docker     (121)     7573 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/zen/1/bli_setv_zen_int.c
--rw-r--r--   0 vsts      (1001) docker     (121)    10830 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/zen/1/bli_swapv_zen_int8.c
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.768227 blis-0.9.1.dev0/blis/_src/kernels/zen/1f/
--rw-r--r--   0 vsts      (1001) docker     (121)     9138 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/zen/1f/bli_axpyf_zen_int_4.c
--rw-r--r--   0 vsts      (1001) docker     (121)    38725 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/zen/1f/bli_axpyf_zen_int_5.c
--rw-r--r--   0 vsts      (1001) docker     (121)    13138 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/zen/1f/bli_axpyf_zen_int_8.c
--rw-r--r--   0 vsts      (1001) docker     (121)    26897 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/zen/1f/bli_dotxf_zen_int_8.c
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.768227 blis-0.9.1.dev0/blis/_src/kernels/zen/3/
--rw-r--r--   0 vsts      (1001) docker     (121)   169097 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/zen/3/bli_gemm_small.c
--rw-r--r--   0 vsts      (1001) docker     (121)   170034 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/zen/3/bli_gemmt_small.c
--rw-r--r--   0 vsts      (1001) docker     (121)  1737390 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/zen/3/bli_trsm_small.c
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.504226 blis-0.9.1.dev0/blis/_src/kernels/zen/3/sup/
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.776227 blis-0.9.1.dev0/blis/_src/kernels/zen/3/sup/broken/
--rw-r--r--   0 vsts      (1001) docker     (121)    69777 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/zen/3/sup/broken/bli_gemmsup_rv_zen_asm_c3x8.c
--rw-r--r--   0 vsts      (1001) docker     (121)    51585 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/zen/3/sup/broken/bli_gemmsup_rv_zen_asm_c3x8m.c
--rw-r--r--   0 vsts      (1001) docker     (121)    53325 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/zen/3/sup/broken/bli_gemmsup_rv_zen_asm_c3x8n.c
--rw-r--r--   0 vsts      (1001) docker     (121)    49441 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/zen/3/sup/broken/bli_gemmsup_rv_zen_asm_z3x4.c
--rw-r--r--   0 vsts      (1001) docker     (121)    36551 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/zen/3/sup/broken/bli_gemmsup_rv_zen_asm_z3x4m.c
--rw-r--r--   0 vsts      (1001) docker     (121)    39419 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/zen/3/sup/broken/bli_gemmsup_rv_zen_asm_z3x4n.c
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.776227 blis-0.9.1.dev0/blis/_src/kernels/zen/3/sup/other/
--rw-r--r--   0 vsts      (1001) docker     (121)   106760 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/zen/3/sup/other/bli_gemmsup_rd_zen_asm_s6x16.c
--rw-r--r--   0 vsts      (1001) docker     (121)    66862 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/zen/3/sup/other/bli_gemmsup_rd_zen_asm_s6x16m.c
--rw-r--r--   0 vsts      (1001) docker     (121)    63138 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/zen/3/sup/other/bli_gemmsup_rd_zen_asm_s6x16n.c
--rw-r--r--   0 vsts      (1001) docker     (121)   307015 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/zen/3/sup/other/bli_gemmsup_rv_zen_asm_s6x16.c
--rw-r--r--   0 vsts      (1001) docker     (121)    78025 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/zen/3/sup/other/bli_gemmsup_rv_zen_asm_s6x16m.c
--rw-r--r--   0 vsts      (1001) docker     (121)   126101 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/zen/3/sup/other/bli_gemmsup_rv_zen_asm_s6x16n.c
--rw-r--r--   0 vsts      (1001) docker     (121)     8774 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/zen/bli_kernels_zen.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.776227 blis-0.9.1.dev0/blis/_src/kernels/zen2/
--rw-r--r--   0 vsts      (1001) docker     (121)     1839 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/kernels/zen2/bli_kernels_zen2.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.788227 blis-0.9.1.dev0/blis/_src/make/
--rw-r--r--   0 vsts      (1001) docker     (121)   136447 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/make/darwin-firestorm.jsonl
--rw-r--r--   0 vsts      (1001) docker     (121)   114321 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/make/darwin-generic.jsonl
--rw-r--r--   0 vsts      (1001) docker     (121)   419616 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/make/darwin-x86_64.jsonl
--rw-r--r--   0 vsts      (1001) docker     (121)   319287 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/make/darwin-x86_64_no_skx.jsonl
--rw-r--r--   0 vsts      (1001) docker     (121)   366357 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/make/darwin-x86_64_no_zen2.jsonl
--rw-r--r--   0 vsts      (1001) docker     (121)   410978 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/make/darwin-x86_64_no_zen3.jsonl
--rw-r--r--   0 vsts      (1001) docker     (121)   237677 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/make/linux-arm64.jsonl
--rw-r--r--   0 vsts      (1001) docker     (121)   197598 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/make/linux-arm64_no_sve.jsonl
--rw-r--r--   0 vsts      (1001) docker     (121)   115356 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/make/linux-generic.jsonl
--rw-r--r--   0 vsts      (1001) docker     (121)   114356 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/make/linux-power9.jsonl
--rw-r--r--   0 vsts      (1001) docker     (121)   414207 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/make/linux-x86_64.jsonl
--rw-r--r--   0 vsts      (1001) docker     (121)   312099 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/make/linux-x86_64_no_skx.jsonl
--rw-r--r--   0 vsts      (1001) docker     (121)   360983 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/make/linux-x86_64_no_zen2.jsonl
--rw-r--r--   0 vsts      (1001) docker     (121)   405530 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/make/linux-x86_64_no_zen3.jsonl
--rw-r--r--   0 vsts      (1001) docker     (121)   123566 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/make/windows-generic.jsonl
--rw-r--r--   0 vsts      (1001) docker     (121)   403925 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/make/windows-x86_64.jsonl
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.788227 blis-0.9.1.dev0/blis/_src/ref_kernels/
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.792227 blis-0.9.1.dev0/blis/_src/ref_kernels/1/
--rw-r--r--   0 vsts      (1001) docker     (121)     2855 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/ref_kernels/1/bli_addv_ref.c
--rw-r--r--   0 vsts      (1001) docker     (121)     5027 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/ref_kernels/1/bli_amaxv_ref.c
--rw-r--r--   0 vsts      (1001) docker     (121)     6312 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/ref_kernels/1/bli_axpbyv_ref.c
--rw-r--r--   0 vsts      (1001) docker     (121)     5265 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/ref_kernels/1/bli_axpyv_ref.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2764 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/ref_kernels/1/bli_copyv_ref.c
--rw-r--r--   0 vsts      (1001) docker     (121)     3317 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/ref_kernels/1/bli_dotv_ref.c
--rw-r--r--   0 vsts      (1001) docker     (121)     3644 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/ref_kernels/1/bli_dotxv_ref.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2281 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/ref_kernels/1/bli_invertv_ref.c
--rw-r--r--   0 vsts      (1001) docker     (121)     3694 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/ref_kernels/1/bli_scal2v_ref.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2972 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/ref_kernels/1/bli_scalv_ref.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2792 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/ref_kernels/1/bli_setv_ref.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2759 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/ref_kernels/1/bli_subv_ref.c
--rw-r--r--   0 vsts      (1001) docker     (121)     2355 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/ref_kernels/1/bli_swapv_ref.c
--rw-r--r--   0 vsts      (1001) docker     (121)     3618 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/ref_kernels/1/bli_xpbyv_ref.c
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.800227 blis-0.9.1.dev0/blis/_src/ref_kernels/1f/
--rw-r--r--   0 vsts      (1001) docker     (121)     3945 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/ref_kernels/1f/bli_axpy2v_ref.c
--rw-r--r--   0 vsts      (1001) docker     (121)     4088 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/ref_kernels/1f/bli_axpyf_ref.c
--rw-r--r--   0 vsts      (1001) docker     (121)     4438 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/ref_kernels/1f/bli_dotaxpyv_ref.c
--rw-r--r--   0 vsts      (1001) docker     (121)     6038 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/ref_kernels/1f/bli_dotxaxpyf_ref.c
--rw-r--r--   0 vsts      (1001) docker     (121)     4582 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/ref_kernels/1f/bli_dotxf_ref.c
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.800227 blis-0.9.1.dev0/blis/_src/ref_kernels/1f/other/
--rw-r--r--   0 vsts      (1001) docker     (121)     3519 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/ref_kernels/1f/other/bli_dotxaxpyf_ref_alt.c
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.800227 blis-0.9.1.dev0/blis/_src/ref_kernels/1m/
--rw-r--r--   0 vsts      (1001) docker     (121)    95930 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/ref_kernels/1m/bli_packm_cxk_1er_ref.c
--rw-r--r--   0 vsts      (1001) docker     (121)    23874 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/ref_kernels/1m/bli_packm_cxk_bb_ref.c
--rw-r--r--   0 vsts      (1001) docker     (121)    55513 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/ref_kernels/1m/bli_packm_cxk_ref.c
--rw-r--r--   0 vsts      (1001) docker     (121)    31541 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/ref_kernels/1m/bli_unpackm_cxk_ref.c
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.804227 blis-0.9.1.dev0/blis/_src/ref_kernels/3/
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.804227 blis-0.9.1.dev0/blis/_src/ref_kernels/3/bb/
--rw-r--r--   0 vsts      (1001) docker     (121)     4533 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/ref_kernels/3/bb/bli_gemmbb_ref.c
--rw-r--r--   0 vsts      (1001) docker     (121)     4733 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/ref_kernels/3/bb/bli_gemmtrsmbb_ref.c
--rw-r--r--   0 vsts      (1001) docker     (121)     7445 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/ref_kernels/3/bb/bli_trsmbb_ref.c
--rw-r--r--   0 vsts      (1001) docker     (121)     7493 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/ref_kernels/3/bli_gemm_ref.c
--rw-r--r--   0 vsts      (1001) docker     (121)    22803 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/ref_kernels/3/bli_gemmsup_ref.c
--rw-r--r--   0 vsts      (1001) docker     (121)     4590 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/ref_kernels/3/bli_gemmtrsm_ref.c
--rw-r--r--   0 vsts      (1001) docker     (121)     7457 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/ref_kernels/3/bli_trsm_ref.c
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.804227 blis-0.9.1.dev0/blis/_src/ref_kernels/3/old/
--rw-r--r--   0 vsts      (1001) docker     (121)     5194 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/ref_kernels/3/old/bli_gemm_simd_ref.c
--rw-r--r--   0 vsts      (1001) docker     (121)    12471 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/ref_kernels/3/old/bli_gemm_unrl_ref.c
--rw-r--r--   0 vsts      (1001) docker     (121)     5672 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/ref_kernels/3/old/bli_trsm_simd_ref.c
--rw-r--r--   0 vsts      (1001) docker     (121)    26841 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/ref_kernels/bli_cntx_ref.c
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.804227 blis-0.9.1.dev0/blis/_src/ref_kernels/ind/
--rw-r--r--   0 vsts      (1001) docker     (121)     8951 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/ref_kernels/ind/bli_gemm1m_ref.c
--rw-r--r--   0 vsts      (1001) docker     (121)     9018 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/ref_kernels/ind/bli_gemmtrsm1m_ref.c
--rw-r--r--   0 vsts      (1001) docker     (121)    17348 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/_src/ref_kernels/ind/bli_trsm1m_ref.c
--rw-r--r--   0 vsts      (1001) docker     (121)      542 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/about.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2669 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/benchmark.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3607 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/cy.pxd
--rw-r--r--   0 vsts      (1001) docker     (121)    16918 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/cy.pyx
--rw-r--r--   0 vsts      (1001) docker     (121)     7055 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/py.pyx
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.812227 blis-0.9.1.dev0/blis/tests/
--rw-r--r--   0 vsts      (1001) docker     (121)        0 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/tests/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2577 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/tests/common.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1134 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/tests/test_dotv.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2493 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/blis/tests/test_gemm.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-21 18:16:00.504226 blis-0.9.1.dev0/blis.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (121)     7728 2022-07-21 18:16:00.000000 blis-0.9.1.dev0/blis.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (121)    67517 2022-07-21 18:16:00.000000 blis-0.9.1.dev0/blis.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (121)        1 2022-07-21 18:16:00.000000 blis-0.9.1.dev0/blis.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (121)       14 2022-07-21 18:16:00.000000 blis-0.9.1.dev0/blis.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (121)        5 2022-07-21 18:16:00.000000 blis-0.9.1.dev0/blis.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (121)      129 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (121)       38 2022-07-21 18:16:00.816227 blis-0.9.1.dev0/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (121)    13630 2022-07-21 18:15:46.000000 blis-0.9.1.dev0/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.906470 blis-0.9.1.dev1/
+-rw-r--r--   0 vsts      (1001) docker     (121)     2033 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (121)      170 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (121)     7728 2022-08-01 16:04:04.906470 blis-0.9.1.dev1/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (121)     6696 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.710469 blis-0.9.1.dev1/blis/
+-rw-r--r--   0 vsts      (1001) docker     (121)        0 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/__init__.pxd
+-rw-r--r--   0 vsts      (1001) docker     (121)       79 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.710469 blis-0.9.1.dev1/blis/_src/
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.698469 blis-0.9.1.dev1/blis/_src/config/
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.714469 blis-0.9.1.dev1/blis/_src/config/a64fx/
+-rw-r--r--   0 vsts      (1001) docker     (121)     4399 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/config/a64fx/bli_a64fx_sector_cache.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     5804 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/config/a64fx/bli_cntx_init_a64fx.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2179 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/config/a64fx/bli_family_a64fx.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.714469 blis-0.9.1.dev1/blis/_src/config/amd64/
+-rw-r--r--   0 vsts      (1001) docker     (121)     1754 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/config/amd64/bli_family_amd64.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.714469 blis-0.9.1.dev1/blis/_src/config/amd64_legacy/
+-rw-r--r--   0 vsts      (1001) docker     (121)     1867 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/config/amd64_legacy/bli_family_amd64_legacy.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.714469 blis-0.9.1.dev1/blis/_src/config/arm32/
+-rw-r--r--   0 vsts      (1001) docker     (121)     1850 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/config/arm32/bli_family_arm32.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.714469 blis-0.9.1.dev1/blis/_src/config/arm64/
+-rw-r--r--   0 vsts      (1001) docker     (121)     2172 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/config/arm64/bli_family_arm64.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.714469 blis-0.9.1.dev1/blis/_src/config/armsve/
+-rw-r--r--   0 vsts      (1001) docker     (121)     6174 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/config/armsve/bli_cntx_init_armsve.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2179 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/config/armsve/bli_family_armsve.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.714469 blis-0.9.1.dev1/blis/_src/config/bgq/
+-rw-r--r--   0 vsts      (1001) docker     (121)     3097 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/config/bgq/bli_cntx_init_bgq.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     3211 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/config/bgq/bli_family_bgq.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.714469 blis-0.9.1.dev1/blis/_src/config/bulldozer/
+-rw-r--r--   0 vsts      (1001) docker     (121)     3279 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/config/bulldozer/bli_cntx_init_bulldozer.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2835 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/config/bulldozer/bli_family_bulldozer.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.714469 blis-0.9.1.dev1/blis/_src/config/cortexa15/
+-rw-r--r--   0 vsts      (1001) docker     (121)     3494 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/config/cortexa15/bli_cntx_init_cortexa15.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2938 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/config/cortexa15/bli_family_cortexa15.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.714469 blis-0.9.1.dev1/blis/_src/config/cortexa53/
+-rw-r--r--   0 vsts      (1001) docker     (121)     3117 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/config/cortexa53/bli_cntx_init_cortexa53.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     1800 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/config/cortexa53/bli_family_cortexa53.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.714469 blis-0.9.1.dev1/blis/_src/config/cortexa57/
+-rw-r--r--   0 vsts      (1001) docker     (121)     3117 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/config/cortexa57/bli_cntx_init_cortexa57.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     3092 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/config/cortexa57/bli_family_cortexa57.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.714469 blis-0.9.1.dev1/blis/_src/config/cortexa9/
+-rw-r--r--   0 vsts      (1001) docker     (121)     3113 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/config/cortexa9/bli_cntx_init_cortexa9.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2934 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/config/cortexa9/bli_family_cortexa9.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.714469 blis-0.9.1.dev1/blis/_src/config/excavator/
+-rw-r--r--   0 vsts      (1001) docker     (121)     3267 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/config/excavator/bli_cntx_init_excavator.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     3037 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/config/excavator/bli_family_excavator.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.714469 blis-0.9.1.dev1/blis/_src/config/firestorm/
+-rw-r--r--   0 vsts      (1001) docker     (121)     5618 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/config/firestorm/bli_cntx_init_firestorm.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     3092 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/config/firestorm/bli_family_firestorm.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.714469 blis-0.9.1.dev1/blis/_src/config/generic/
+-rw-r--r--   0 vsts      (1001) docker     (121)     1826 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/config/generic/bli_cntx_init_generic.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     1735 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/config/generic/bli_family_generic.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.714469 blis-0.9.1.dev1/blis/_src/config/haswell/
+-rw-r--r--   0 vsts      (1001) docker     (121)     9868 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/config/haswell/bli_cntx_init_haswell.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     4881 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/config/haswell/bli_family_haswell.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.714469 blis-0.9.1.dev1/blis/_src/config/intel64/
+-rw-r--r--   0 vsts      (1001) docker     (121)     1734 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/config/intel64/bli_family_intel64.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.714469 blis-0.9.1.dev1/blis/_src/config/intel64_no_skx/
+-rw-r--r--   0 vsts      (1001) docker     (121)     1734 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/config/intel64_no_skx/bli_family_intel64.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1734 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/config/intel64_no_skx/bli_family_intel64_no_skx.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.714469 blis-0.9.1.dev1/blis/_src/config/knc/
+-rw-r--r--   0 vsts      (1001) docker     (121)     3176 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/config/knc/bli_cntx_init_knc.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     3540 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/config/knc/bli_family_knc.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.714469 blis-0.9.1.dev1/blis/_src/config/knl/
+-rw-r--r--   0 vsts      (1001) docker     (121)     5048 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/config/knl/bli_cntx_init_knl.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     5007 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/config/knl/bli_family_knl.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.698469 blis-0.9.1.dev1/blis/_src/config/old/
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.714469 blis-0.9.1.dev1/blis/_src/config/old/armv7a/
+-rw-r--r--   0 vsts      (1001) docker     (121)     3235 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/config/old/armv7a/bli_cntx_init_armv7a.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     3064 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/config/old/armv7a/bli_family_armv7a.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.714469 blis-0.9.1.dev1/blis/_src/config/old/emscripten/
+-rw-r--r--   0 vsts      (1001) docker     (121)     6542 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/config/old/emscripten/bli_kernel.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.714469 blis-0.9.1.dev1/blis/_src/config/old/haswellbb/
+-rw-r--r--   0 vsts      (1001) docker     (121)    11201 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/config/old/haswellbb/bli_cntx_init_haswell.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     5296 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/config/old/haswellbb/bli_family_haswell.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.714469 blis-0.9.1.dev1/blis/_src/config/old/loongson3a/
+-rw-r--r--   0 vsts      (1001) docker     (121)     6547 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/config/old/loongson3a/bli_kernel.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.714469 blis-0.9.1.dev1/blis/_src/config/old/newarch/
+-rw-r--r--   0 vsts      (1001) docker     (121)     1728 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/config/old/newarch/bli_kernel.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.714469 blis-0.9.1.dev1/blis/_src/config/old/pnacl/
+-rw-r--r--   0 vsts      (1001) docker     (121)     7821 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/config/old/pnacl/bli_kernel.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.718469 blis-0.9.1.dev1/blis/_src/config/penryn/
+-rw-r--r--   0 vsts      (1001) docker     (121)     3401 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/config/penryn/bli_cntx_init_penryn.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     3162 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/config/penryn/bli_family_penryn.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.718469 blis-0.9.1.dev1/blis/_src/config/piledriver/
+-rw-r--r--   0 vsts      (1001) docker     (121)     3269 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/config/piledriver/bli_cntx_init_piledriver.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     3023 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/config/piledriver/bli_family_piledriver.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.718469 blis-0.9.1.dev1/blis/_src/config/power10/
+-rw-r--r--   0 vsts      (1001) docker     (121)     6104 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/config/power10/bli_cntx_init_power10.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     1838 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/config/power10/bli_family_power10.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.718469 blis-0.9.1.dev1/blis/_src/config/power7/
+-rw-r--r--   0 vsts      (1001) docker     (121)     3044 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/config/power7/bli_cntx_init_power7.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2098 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/config/power7/bli_family_power7.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.718469 blis-0.9.1.dev1/blis/_src/config/power9/
+-rw-r--r--   0 vsts      (1001) docker     (121)     6056 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/config/power9/bli_cntx_init_power9.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2089 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/config/power9/bli_family_power9.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.718469 blis-0.9.1.dev1/blis/_src/config/sandybridge/
+-rw-r--r--   0 vsts      (1001) docker     (121)     3271 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/config/sandybridge/bli_cntx_init_sandybridge.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2812 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/config/sandybridge/bli_family_sandybridge.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.718469 blis-0.9.1.dev1/blis/_src/config/skx/
+-rw-r--r--   0 vsts      (1001) docker     (121)     4776 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/config/skx/bli_cntx_init_skx.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     4815 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/config/skx/bli_family_skx.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.718469 blis-0.9.1.dev1/blis/_src/config/steamroller/
+-rw-r--r--   0 vsts      (1001) docker     (121)     3271 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/config/steamroller/bli_cntx_init_steamroller.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     1861 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/config/steamroller/bli_family_steamroller.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.718469 blis-0.9.1.dev1/blis/_src/config/template/
+-rw-r--r--   0 vsts      (1001) docker     (121)     4015 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/config/template/bli_cntx_init_template.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     1735 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/config/template/bli_family_template.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.698469 blis-0.9.1.dev1/blis/_src/config/template/kernels/
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.718469 blis-0.9.1.dev1/blis/_src/config/template/kernels/1/
+-rw-r--r--   0 vsts      (1001) docker     (121)     6920 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/config/template/kernels/1/bli_axpyv_template_noopt_var1.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     7848 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/config/template/kernels/1/bli_dotv_template_noopt_var1.c
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.718469 blis-0.9.1.dev1/blis/_src/config/template/kernels/1f/
+-rw-r--r--   0 vsts      (1001) docker     (121)    10294 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/config/template/kernels/1f/bli_axpy2v_template_noopt_var1.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     9443 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/config/template/kernels/1f/bli_axpyf_template_noopt_var1.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    11296 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/config/template/kernels/1f/bli_dotaxpyv_template_noopt_var1.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    14336 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/config/template/kernels/1f/bli_dotxaxpyf_template_noopt_var1.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    10133 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/config/template/kernels/1f/bli_dotxf_template_noopt_var1.c
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.718469 blis-0.9.1.dev1/blis/_src/config/template/kernels/3/
+-rw-r--r--   0 vsts      (1001) docker     (121)     4662 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/config/template/kernels/3/bli_gemm_template_noopt_mxn.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     3454 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/config/template/kernels/3/bli_gemmtrsm_l_template_noopt_mxn.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     3453 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/config/template/kernels/3/bli_gemmtrsm_u_template_noopt_mxn.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     4698 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/config/template/kernels/3/bli_trsm_l_template_noopt_mxn.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     4709 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/config/template/kernels/3/bli_trsm_u_template_noopt_mxn.c
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.718469 blis-0.9.1.dev1/blis/_src/config/thunderx2/
+-rw-r--r--   0 vsts      (1001) docker     (121)     3117 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/config/thunderx2/bli_cntx_init_thunderx2.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     1848 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/config/thunderx2/bli_family_thunderx2.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.718469 blis-0.9.1.dev1/blis/_src/config/x86_64/
+-rw-r--r--   0 vsts      (1001) docker     (121)     1734 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/config/x86_64/bli_family_x86_64.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.718469 blis-0.9.1.dev1/blis/_src/config/x86_64_no_skx/
+-rw-r--r--   0 vsts      (1001) docker     (121)     1734 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/config/x86_64_no_skx/bli_family_x86_64_no_skx.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.718469 blis-0.9.1.dev1/blis/_src/config/x86_64_no_zen2/
+-rw-r--r--   0 vsts      (1001) docker     (121)     1734 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/config/x86_64_no_zen2/bli_family_x86_64_no_zen2.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.718469 blis-0.9.1.dev1/blis/_src/config/x86_64_no_zen3/
+-rw-r--r--   0 vsts      (1001) docker     (121)     1734 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/config/x86_64_no_zen3/bli_family_x86_64_no_zen3.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.718469 blis-0.9.1.dev1/blis/_src/config/zen/
+-rw-r--r--   0 vsts      (1001) docker     (121)    12183 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/config/zen/bli_cntx_init_zen.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     3328 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/config/zen/bli_family_zen.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.718469 blis-0.9.1.dev1/blis/_src/config/zen/old/
+-rw-r--r--   0 vsts      (1001) docker     (121)     7542 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/config/zen/old/bli_kernel.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.718469 blis-0.9.1.dev1/blis/_src/config/zen2/
+-rw-r--r--   0 vsts      (1001) docker     (121)    10835 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/config/zen2/bli_cntx_init_zen2.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     3827 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/config/zen2/bli_family_zen2.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.718469 blis-0.9.1.dev1/blis/_src/config/zen3/
+-rw-r--r--   0 vsts      (1001) docker     (121)    11375 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/config/zen3/bli_cntx_init_zen3.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     3888 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/config/zen3/bli_family_zen3.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.706469 blis-0.9.1.dev1/blis/_src/frame/
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.722469 blis-0.9.1.dev1/blis/_src/frame/0/
+-rw-r--r--   0 vsts      (1001) docker     (121)     1889 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/0/bli_l0.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     8713 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/0/bli_l0_check.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     3458 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/0/bli_l0_check.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2374 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/0/bli_l0_fpa.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2047 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/0/bli_l0_fpa.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     4120 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/0/bli_l0_ft.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     8572 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/0/bli_l0_oapi.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     3086 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/0/bli_l0_oapi.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     5895 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/0/bli_l0_tapi.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     3977 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/0/bli_l0_tapi.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.722469 blis-0.9.1.dev1/blis/_src/frame/0/copysc/
+-rw-r--r--   0 vsts      (1001) docker     (121)     3760 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/0/copysc/bli_copysc.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2284 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/0/copysc/bli_copysc.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.722469 blis-0.9.1.dev1/blis/_src/frame/1/
+-rw-r--r--   0 vsts      (1001) docker     (121)     2604 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/1/bli_l1v.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    11714 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/1/bli_l1v_check.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     4215 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/1/bli_l1v_check.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2314 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/1/bli_l1v_fpa.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2107 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/1/bli_l1v_fpa.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     5044 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/1/bli_l1v_ft.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     5463 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/1/bli_l1v_ft_ker.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     3276 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/1/bli_l1v_ker.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     5755 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/1/bli_l1v_ker_prot.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    14345 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/1/bli_l1v_oapi.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     4010 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/1/bli_l1v_oapi.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1976 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/1/bli_l1v_oapi_ba.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     1974 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/1/bli_l1v_oapi_ex.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     9014 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/1/bli_l1v_tapi.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     5014 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/1/bli_l1v_tapi.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1974 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/1/bli_l1v_tapi_ba.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     1972 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/1/bli_l1v_tapi_ex.c
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.702469 blis-0.9.1.dev1/blis/_src/frame/1/other/
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.722469 blis-0.9.1.dev1/blis/_src/frame/1/other/packv/
+-rw-r--r--   0 vsts      (1001) docker     (121)     1692 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/1/other/packv/bli_packv.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     1819 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/1/other/packv/bli_packv.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2041 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/1/other/packv/bli_packv_check.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     1765 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/1/other/packv/bli_packv_check.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2606 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/1/other/packv/bli_packv_cntl.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2420 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/1/other/packv/bli_packv_cntl.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     6495 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/1/other/packv/bli_packv_init.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     1946 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/1/other/packv/bli_packv_init.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     4380 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/1/other/packv/bli_packv_int.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     1789 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/1/other/packv/bli_packv_int.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     3151 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/1/other/packv/bli_packv_unb_var1.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2084 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/1/other/packv/bli_packv_unb_var1.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.722469 blis-0.9.1.dev1/blis/_src/frame/1/other/scalv/
+-rw-r--r--   0 vsts      (1001) docker     (121)     2421 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/1/other/scalv/bli_scalv_cntl.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2187 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/1/other/scalv/bli_scalv_cntl.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2812 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/1/other/scalv/bli_scalv_int.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     1814 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/1/other/scalv/bli_scalv_int.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.726469 blis-0.9.1.dev1/blis/_src/frame/1/other/unpackv/
+-rw-r--r--   0 vsts      (1001) docker     (121)     1692 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/1/other/unpackv/bli_unpackv.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     1800 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/1/other/unpackv/bli_unpackv.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2199 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/1/other/unpackv/bli_unpackv_check.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     1767 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/1/other/unpackv/bli_unpackv_check.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2458 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/1/other/unpackv/bli_unpackv_cntl.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2463 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/1/other/unpackv/bli_unpackv_cntl.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     7960 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/1/other/unpackv/bli_unpackv_int.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     1951 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/1/other/unpackv/bli_unpackv_int.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     3173 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/1/other/unpackv/bli_unpackv_unb_var1.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2102 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/1/other/unpackv/bli_unpackv_unb_var1.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.726469 blis-0.9.1.dev1/blis/_src/frame/1d/
+-rw-r--r--   0 vsts      (1001) docker     (121)     2264 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/1d/bli_l1d.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     5909 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/1d/bli_l1d_check.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     3030 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/1d/bli_l1d_check.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2260 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/1d/bli_l1d_fpa.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2057 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/1d/bli_l1d_fpa.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     4485 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/1d/bli_l1d_ft.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    11491 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/1d/bli_l1d_oapi.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2882 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/1d/bli_l1d_oapi.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1976 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/1d/bli_l1d_oapi_ba.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     1974 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/1d/bli_l1d_oapi_ex.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    13381 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/1d/bli_l1d_tapi.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     4440 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/1d/bli_l1d_tapi.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1974 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/1d/bli_l1d_tapi_ba.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     1972 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/1d/bli_l1d_tapi_ex.c
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.726469 blis-0.9.1.dev1/blis/_src/frame/1f/
+-rw-r--r--   0 vsts      (1001) docker     (121)     2326 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/1f/bli_l1f.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    12540 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/1f/bli_l1f_check.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2907 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/1f/bli_l1f_check.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2159 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/1f/bli_l1f_fpa.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     1962 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/1f/bli_l1f_fpa.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     4031 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/1f/bli_l1f_ft.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     4464 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/1f/bli_l1f_ft_ker.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2455 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/1f/bli_l1f_ker.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     4065 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/1f/bli_l1f_ker_prot.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    12137 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/1f/bli_l1f_oapi.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     3142 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/1f/bli_l1f_oapi.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1976 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/1f/bli_l1f_oapi_ba.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     1974 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/1f/bli_l1f_oapi_ex.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     6386 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/1f/bli_l1f_tapi.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     3980 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/1f/bli_l1f_tapi.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1974 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/1f/bli_l1f_tapi_ba.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     1972 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/1f/bli_l1f_tapi_ex.c
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.730469 blis-0.9.1.dev1/blis/_src/frame/1m/
+-rw-r--r--   0 vsts      (1001) docker     (121)     2537 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/1m/bli_l1m.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     5411 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/1m/bli_l1m_check.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2784 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/1m/bli_l1m_check.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2645 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/1m/bli_l1m_fpa.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2178 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/1m/bli_l1m_fpa.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     4045 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/1m/bli_l1m_ft.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     4301 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/1m/bli_l1m_ft_ker.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     3443 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/1m/bli_l1m_ker.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2993 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/1m/bli_l1m_ker_prot.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    12092 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/1m/bli_l1m_oapi.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2659 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/1m/bli_l1m_oapi.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1976 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/1m/bli_l1m_oapi_ba.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     1974 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/1m/bli_l1m_oapi_ex.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2256 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/1m/bli_l1m_oft_var.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    11871 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/1m/bli_l1m_tapi.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     4092 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/1m/bli_l1m_tapi.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1974 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/1m/bli_l1m_tapi_ba.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     1972 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/1m/bli_l1m_tapi_ex.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    15140 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/1m/bli_l1m_unb_var1.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     4104 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/1m/bli_l1m_unb_var1.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.730469 blis-0.9.1.dev1/blis/_src/frame/1m/other/
+-rw-r--r--   0 vsts      (1001) docker     (121)     1702 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/1m/other/bli_scalm.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2181 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/1m/other/bli_scalm_cntl.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     1773 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/1m/other/bli_scalm_cntl.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     3356 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/1m/other/bli_scalm_int.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     1814 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/1m/other/bli_scalm_int.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.730469 blis-0.9.1.dev1/blis/_src/frame/1m/packm/
+-rw-r--r--   0 vsts      (1001) docker     (121)     2194 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/1m/packm/bli_packm.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     3556 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/1m/packm/bli_packm_alloc.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2027 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/1m/packm/bli_packm_alloc.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    11518 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/1m/packm/bli_packm_blk_var1.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2151 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/1m/packm/bli_packm_blk_var1.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2818 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/1m/packm/bli_packm_check.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     1868 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/1m/packm/bli_packm_check.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     3221 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/1m/packm/bli_packm_cntl.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     3608 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/1m/packm/bli_packm_cntl.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     7012 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/1m/packm/bli_packm_cxk.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2119 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/1m/packm/bli_packm_cxk.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     4308 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/1m/packm/bli_packm_cxk_1er.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2143 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/1m/packm/bli_packm_cxk_1er.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     7708 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/1m/packm/bli_packm_init.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     1850 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/1m/packm/bli_packm_init.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2312 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/1m/packm/bli_packm_int.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     1831 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/1m/packm/bli_packm_int.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     9249 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/1m/packm/bli_packm_part.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2606 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/1m/packm/bli_packm_part.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     3203 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/1m/packm/bli_packm_scalar.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     1741 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/1m/packm/bli_packm_scalar.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    14125 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/1m/packm/bli_packm_struc_cxk.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2536 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/1m/packm/bli_packm_struc_cxk.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    15130 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/1m/packm/bli_packm_struc_cxk_1er.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2604 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/1m/packm/bli_packm_struc_cxk_1er.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    13475 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/1m/packm/bli_packm_struc_cxk_md.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     3136 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/1m/packm/bli_packm_struc_cxk_md.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2278 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/1m/packm/bli_packm_thrinfo.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     3058 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/1m/packm/bli_packm_thrinfo.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.734469 blis-0.9.1.dev1/blis/_src/frame/1m/unpackm/
+-rw-r--r--   0 vsts      (1001) docker     (121)     1828 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/1m/unpackm/bli_unpackm.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     8579 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/1m/unpackm/bli_unpackm_blk_var1.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2341 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/1m/unpackm/bli_unpackm_blk_var1.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2458 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/1m/unpackm/bli_unpackm_check.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     1772 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/1m/unpackm/bli_unpackm_check.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2770 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/1m/unpackm/bli_unpackm_cntl.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2261 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/1m/unpackm/bli_unpackm_cntl.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     3079 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/1m/unpackm/bli_unpackm_cxk.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2032 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/1m/unpackm/bli_unpackm_cxk.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2559 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/1m/unpackm/bli_unpackm_int.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     1813 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/1m/unpackm/bli_unpackm_int.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.734469 blis-0.9.1.dev1/blis/_src/frame/2/
+-rw-r--r--   0 vsts      (1001) docker     (121)     2558 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/2/bli_l2.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    10509 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/2/bli_l2_check.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2909 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/2/bli_l2_check.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     3511 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/2/bli_l2_fpa.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     3161 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/2/bli_l2_fpa.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     4694 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/2/bli_l2_ft.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     4447 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/2/bli_l2_ft_unb.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    12392 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/2/bli_l2_oapi.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2770 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/2/bli_l2_oapi.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1975 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/2/bli_l2_oapi_ba.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     1973 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/2/bli_l2_oapi_ex.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    13995 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/2/bli_l2_tapi.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     4661 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/2/bli_l2_tapi.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1973 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/2/bli_l2_tapi_ba.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     1971 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/2/bli_l2_tapi_ex.c
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.734469 blis-0.9.1.dev1/blis/_src/frame/2/gemv/
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.734469 blis-0.9.1.dev1/blis/_src/frame/2/gemv/amd/
+-rw-r--r--   0 vsts      (1001) docker     (121)     5941 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/2/gemv/amd/bli_gemv_unf_var2_amd.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     1848 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/2/gemv/bli_gemv.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2996 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/2/gemv/bli_gemv_unb_var1.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     3571 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/2/gemv/bli_gemv_unb_var2.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     3173 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/2/gemv/bli_gemv_unf_var1.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     3641 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/2/gemv/bli_gemv_unf_var2.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2712 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/2/gemv/bli_gemv_var.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     3200 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/2/gemv/bli_gemv_var_oapi.c
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.734469 blis-0.9.1.dev1/blis/_src/frame/2/gemv/other/
+-rw-r--r--   0 vsts      (1001) docker     (121)     3846 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/2/gemv/other/bli_gemv_blk_var1.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     3841 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/2/gemv/other/bli_gemv_blk_var2.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     8532 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/2/gemv/other/bli_gemv_cntl.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     3514 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/2/gemv/other/bli_gemv_cntl.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     7610 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/2/gemv/other/bli_gemv_front.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2234 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/2/gemv/other/bli_gemv_front.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     3611 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/2/gemv/other/bli_gemv_int.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     1889 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/2/gemv/other/bli_gemv_int.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.734469 blis-0.9.1.dev1/blis/_src/frame/2/ger/
+-rw-r--r--   0 vsts      (1001) docker     (121)     1843 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/2/ger/bli_ger.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2769 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/2/ger/bli_ger_unb_var1.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2764 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/2/ger/bli_ger_unb_var2.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2527 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/2/ger/bli_ger_var.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     3026 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/2/ger/bli_ger_var_oapi.c
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.734469 blis-0.9.1.dev1/blis/_src/frame/2/ger/other/
+-rw-r--r--   0 vsts      (1001) docker     (121)     3813 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/2/ger/other/bli_ger_blk_var1.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     3812 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/2/ger/other/bli_ger_blk_var2.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     7748 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/2/ger/other/bli_ger_cntl.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     3093 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/2/ger/other/bli_ger_cntl.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     5782 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/2/ger/other/bli_ger_front.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2187 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/2/ger/other/bli_ger_front.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     4430 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/2/ger/other/bli_ger_int.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     1926 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/2/ger/other/bli_ger_int.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.738469 blis-0.9.1.dev1/blis/_src/frame/2/hemv/
+-rw-r--r--   0 vsts      (1001) docker     (121)     1848 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/2/hemv/bli_hemv.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     4873 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/2/hemv/bli_hemv_unb_var1.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     4923 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/2/hemv/bli_hemv_unb_var2.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     4869 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/2/hemv/bli_hemv_unb_var3.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     4802 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/2/hemv/bli_hemv_unb_var4.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     6147 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/2/hemv/bli_hemv_unf_var1.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     4727 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/2/hemv/bli_hemv_unf_var1a.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     6153 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/2/hemv/bli_hemv_unf_var3.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     4723 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/2/hemv/bli_hemv_unf_var3a.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     3076 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/2/hemv/bli_hemv_var.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     3362 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/2/hemv/bli_hemv_var_oapi.c
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.738469 blis-0.9.1.dev1/blis/_src/frame/2/hemv/other/
+-rw-r--r--   0 vsts      (1001) docker     (121)     5832 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/2/hemv/other/bli_hemv_blk_var1.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     5947 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/2/hemv/other/bli_hemv_blk_var2.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     5832 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/2/hemv/other/bli_hemv_blk_var3.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     5943 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/2/hemv/other/bli_hemv_blk_var4.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     7588 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/2/hemv/other/bli_hemv_cntl.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     3772 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/2/hemv/other/bli_hemv_cntl.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     7341 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/2/hemv/other/bli_hemv_front.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2312 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/2/hemv/other/bli_hemv_front.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     4260 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/2/hemv/other/bli_hemv_int.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     1932 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/2/hemv/other/bli_hemv_int.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.738469 blis-0.9.1.dev1/blis/_src/frame/2/her/
+-rw-r--r--   0 vsts      (1001) docker     (121)     1843 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/2/her/bli_her.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     4843 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/2/her/bli_her_unb_var1.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     4845 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/2/her/bli_her_unb_var2.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2581 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/2/her/bli_her_var.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2858 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/2/her/bli_her_var_oapi.c
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.738469 blis-0.9.1.dev1/blis/_src/frame/2/her/other/
+-rw-r--r--   0 vsts      (1001) docker     (121)     4773 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/2/her/other/bli_her_blk_var1.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     4773 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/2/her/other/bli_her_blk_var2.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     5599 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/2/her/other/bli_her_cntl.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2986 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/2/her/other/bli_her_cntl.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     5883 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/2/her/other/bli_her_front.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2141 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/2/her/other/bli_her_front.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     3696 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/2/her/other/bli_her_int.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     1864 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/2/her/other/bli_her_int.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.738469 blis-0.9.1.dev1/blis/_src/frame/2/her2/
+-rw-r--r--   0 vsts      (1001) docker     (121)     1847 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/2/her2/bli_her2.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     5417 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/2/her2/bli_her2_unb_var1.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     5655 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/2/her2/bli_her2_unb_var2.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     5653 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/2/her2/bli_her2_unb_var3.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     5623 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/2/her2/bli_her2_unb_var4.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     5352 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/2/her2/bli_her2_unf_var1.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     5560 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/2/her2/bli_her2_unf_var4.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2925 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/2/her2/bli_her2_var.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     3226 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/2/her2/bli_her2_var_oapi.c
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.742469 blis-0.9.1.dev1/blis/_src/frame/2/her2/other/
+-rw-r--r--   0 vsts      (1001) docker     (121)     5699 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/2/her2/other/bli_her2_blk_var1.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     5810 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/2/her2/other/bli_her2_blk_var2.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     5810 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/2/her2/other/bli_her2_blk_var3.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     5699 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/2/her2/other/bli_her2_blk_var4.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     6294 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/2/her2/other/bli_her2_cntl.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     3320 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/2/her2/other/bli_her2_cntl.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     6795 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/2/her2/other/bli_her2_front.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2202 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/2/her2/other/bli_her2_front.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     4572 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/2/her2/other/bli_her2_int.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     1939 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/2/her2/other/bli_her2_int.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.742469 blis-0.9.1.dev1/blis/_src/frame/2/symv/
+-rw-r--r--   0 vsts      (1001) docker     (121)     1764 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/2/symv/bli_symv.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.742469 blis-0.9.1.dev1/blis/_src/frame/2/symv/other/
+-rw-r--r--   0 vsts      (1001) docker     (121)     7348 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/2/symv/other/bli_symv_front.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2238 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/2/symv/other/bli_symv_front.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.742469 blis-0.9.1.dev1/blis/_src/frame/2/syr/
+-rw-r--r--   0 vsts      (1001) docker     (121)     1763 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/2/syr/bli_syr.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.742469 blis-0.9.1.dev1/blis/_src/frame/2/syr/other/
+-rw-r--r--   0 vsts      (1001) docker     (121)     6000 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/2/syr/other/bli_syr_front.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2124 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/2/syr/other/bli_syr_front.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.742469 blis-0.9.1.dev1/blis/_src/frame/2/syr2/
+-rw-r--r--   0 vsts      (1001) docker     (121)     1764 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/2/syr2/bli_syr2.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.742469 blis-0.9.1.dev1/blis/_src/frame/2/syr2/other/
+-rw-r--r--   0 vsts      (1001) docker     (121)     6514 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/2/syr2/other/bli_syr2_front.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2202 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/2/syr2/other/bli_syr2_front.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.742469 blis-0.9.1.dev1/blis/_src/frame/2/trmv/
+-rw-r--r--   0 vsts      (1001) docker     (121)     1848 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/2/trmv/bli_trmv.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     4522 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/2/trmv/bli_trmv_unb_var1.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     4492 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/2/trmv/bli_trmv_unb_var2.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     6383 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/2/trmv/bli_trmv_unf_var1.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     6286 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/2/trmv/bli_trmv_unf_var2.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2676 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/2/trmv/bli_trmv_var.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2954 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/2/trmv/bli_trmv_var_oapi.c
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.742469 blis-0.9.1.dev1/blis/_src/frame/2/trmv/other/
+-rw-r--r--   0 vsts      (1001) docker     (121)     6176 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/2/trmv/other/bli_trmv_cntl.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     3176 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/2/trmv/other/bli_trmv_cntl.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     5970 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/2/trmv/other/bli_trmv_front.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2152 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/2/trmv/other/bli_trmv_front.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     5135 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/2/trmv/other/bli_trmv_int.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     1836 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/2/trmv/other/bli_trmv_int.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     4157 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/2/trmv/other/bli_trmv_l_blk_var1.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     4157 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/2/trmv/other/bli_trmv_l_blk_var2.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     4157 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/2/trmv/other/bli_trmv_u_blk_var1.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     4157 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/2/trmv/other/bli_trmv_u_blk_var2.c
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.742469 blis-0.9.1.dev1/blis/_src/frame/2/trsv/
+-rw-r--r--   0 vsts      (1001) docker     (121)     1848 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/2/trsv/bli_trsv.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     4520 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/2/trsv/bli_trsv_unb_var1.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     4500 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/2/trsv/bli_trsv_unb_var2.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     6413 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/2/trsv/bli_trsv_unf_var1.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     6332 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/2/trsv/bli_trsv_unf_var2.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2676 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/2/trsv/bli_trsv_var.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2954 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/2/trsv/bli_trsv_var_oapi.c
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.746469 blis-0.9.1.dev1/blis/_src/frame/2/trsv/other/
+-rw-r--r--   0 vsts      (1001) docker     (121)     6639 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/2/trsv/other/bli_trsv_cntl.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     3314 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/2/trsv/other/bli_trsv_cntl.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     5694 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/2/trsv/other/bli_trsv_front.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2151 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/2/trsv/other/bli_trsv_front.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     5136 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/2/trsv/other/bli_trsv_int.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     1836 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/2/trsv/other/bli_trsv_int.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     4269 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/2/trsv/other/bli_trsv_l_blk_var1.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     4269 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/2/trsv/other/bli_trsv_l_blk_var2.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     4269 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/2/trsv/other/bli_trsv_u_blk_var1.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     4269 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/2/trsv/other/bli_trsv_u_blk_var2.c
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.750469 blis-0.9.1.dev1/blis/_src/frame/3/
+-rw-r--r--   0 vsts      (1001) docker     (121)     3216 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/3/bli_l3.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    10637 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/3/bli_l3_blocksize.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2752 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/3/bli_l3_blocksize.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    13347 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/3/bli_l3_check.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     3886 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/3/bli_l3_check.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     3673 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/3/bli_l3_cntl.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2163 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/3/bli_l3_cntl.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     3860 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/3/bli_l3_direct.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2117 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/3/bli_l3_direct.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     3271 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/3/bli_l3_ft_ukr.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     7843 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/3/bli_l3_ind.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2803 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/3/bli_l3_ind.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     3245 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/3/bli_l3_ind_ukr.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     4697 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/3/bli_l3_int.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     1890 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/3/bli_l3_int.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     3339 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/3/bli_l3_oapi.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2801 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/3/bli_l3_oapi.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    17009 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/3/bli_l3_oapi_ex.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     3050 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/3/bli_l3_oapi_ex.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2949 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/3/bli_l3_oft.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2059 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/3/bli_l3_oft_var.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     3329 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/3/bli_l3_packab.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2025 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/3/bli_l3_packab.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     6159 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/3/bli_l3_prune.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2398 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/3/bli_l3_prune.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     3207 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/3/bli_l3_schema.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     1786 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/3/bli_l3_schema.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     7134 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/3/bli_l3_sup.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2020 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/3/bli_l3_sup.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2470 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/3/bli_l3_sup_ft_ker.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    14424 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/3/bli_l3_sup_int.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2079 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/3/bli_l3_sup_int.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2371 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/3/bli_l3_sup_ker.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2325 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/3/bli_l3_sup_ker_prot.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2081 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/3/bli_l3_sup_oft.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    12622 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/3/bli_l3_sup_packm_a.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     4037 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/3/bli_l3_sup_packm_a.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    12643 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/3/bli_l3_sup_packm_b.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     4037 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/3/bli_l3_sup_packm_b.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    15254 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/3/bli_l3_sup_packm_var.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2866 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/3/bli_l3_sup_packm_var.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     5512 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/3/bli_l3_sup_ref.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2028 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/3/bli_l3_sup_ref.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    22400 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/3/bli_l3_sup_var12.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    46064 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/3/bli_l3_sup_var1n2m.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     6284 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/3/bli_l3_sup_vars.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     8312 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/3/bli_l3_tapi.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     5401 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/3/bli_l3_tapi.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    15114 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/3/bli_l3_tapi_ex.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     5918 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/3/bli_l3_tapi_ex.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    22929 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/3/bli_l3_thrinfo.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     4287 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/3/bli_l3_thrinfo.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2350 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/3/bli_l3_ukr.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2171 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/3/bli_l3_ukr_fpa.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2031 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/3/bli_l3_ukr_fpa.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     7006 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/3/bli_l3_ukr_oapi.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2488 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/3/bli_l3_ukr_oapi.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     3062 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/3/bli_l3_ukr_prot.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     4595 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/3/bli_l3_ukr_tapi.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2165 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/3/bli_l3_ukr_tapi.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.750469 blis-0.9.1.dev1/blis/_src/frame/3/gemm/
+-rw-r--r--   0 vsts      (1001) docker     (121)     1873 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/3/gemm/bli_gemm.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     3075 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/3/gemm/bli_gemm_blk_var1.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     3075 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/3/gemm/bli_gemm_blk_var2.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     4386 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/3/gemm/bli_gemm_blk_var3.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     7864 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/3/gemm/bli_gemm_cntl.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2656 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/3/gemm/bli_gemm_cntl.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     9834 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/3/gemm/bli_gemm_front.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2082 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/3/gemm/bli_gemm_front.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2226 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/3/gemm/bli_gemm_ker_var1.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    11371 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/3/gemm/bli_gemm_ker_var2.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    21475 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/3/gemm/bli_gemm_md.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     9304 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/3/gemm/bli_gemm_md.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     8532 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/3/gemm/bli_gemm_md_c2r_ref.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     1891 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/3/gemm/bli_gemm_md_c2r_ref.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2250 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/3/gemm/bli_gemm_var.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.750469 blis-0.9.1.dev1/blis/_src/frame/3/gemm/ind/
+-rw-r--r--   0 vsts      (1001) docker     (121)     2759 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/3/gemm/ind/bli_gemm_ind_opt.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.750469 blis-0.9.1.dev1/blis/_src/frame/3/gemm/other/
+-rw-r--r--   0 vsts      (1001) docker     (121)    10817 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/3/gemm/other/bli_gemm_ker_var2.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    11414 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/3/gemm/other/bli_gemm_ker_var2rr.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    11408 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/3/gemm/other/bli_gemm_ker_var2sl.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    10206 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/3/gemm/other/bli_gemm_ker_var5.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2619 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/3/gemm/other/bli_gemm_ker_var5.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.750469 blis-0.9.1.dev1/blis/_src/frame/3/gemmt/
+-rw-r--r--   0 vsts      (1001) docker     (121)     1726 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/3/gemmt/bli_gemmt.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     4173 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/3/gemmt/bli_gemmt_front.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     1920 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/3/gemmt/bli_gemmt_front.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    16264 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/3/gemmt/bli_gemmt_l_ker_var2.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    16500 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/3/gemmt/bli_gemmt_u_ker_var2.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2856 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/3/gemmt/bli_gemmt_var.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2386 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/3/gemmt/bli_gemmt_x_ker_var2.c
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.750469 blis-0.9.1.dev1/blis/_src/frame/3/gemmt/other/
+-rw-r--r--   0 vsts      (1001) docker     (121)    12337 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/3/gemmt/other/bli_gemmt_l_ker_var2.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    12339 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/3/gemmt/other/bli_gemmt_u_ker_var2.c
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.754469 blis-0.9.1.dev1/blis/_src/frame/3/hemm/
+-rw-r--r--   0 vsts      (1001) docker     (121)     1702 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/3/hemm/bli_hemm.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     6134 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/3/hemm/bli_hemm_front.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     1888 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/3/hemm/bli_hemm_front.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.754469 blis-0.9.1.dev1/blis/_src/frame/3/old/
+-rw-r--r--   0 vsts      (1001) docker     (121)     5944 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/3/old/bli_l3_ft_ex.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     4010 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/3/old/bli_l3_sup_edge.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    24752 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/3/old/bli_l3_sup_var1n2m.c
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.754469 blis-0.9.1.dev1/blis/_src/frame/3/symm/
+-rw-r--r--   0 vsts      (1001) docker     (121)     1702 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/3/symm/bli_symm.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     6098 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/3/symm/bli_symm_front.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     1888 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/3/symm/bli_symm_front.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.754469 blis-0.9.1.dev1/blis/_src/frame/3/trmm/
+-rw-r--r--   0 vsts      (1001) docker     (121)     1729 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/3/trmm/bli_trmm.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     7019 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/3/trmm/bli_trmm_front.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     1849 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/3/trmm/bli_trmm_front.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    13048 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/3/trmm/bli_trmm_ll_ker_var2.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    13206 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/3/trmm/bli_trmm_lu_ker_var2.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    15154 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/3/trmm/bli_trmm_rl_ker_var2.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    16080 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/3/trmm/bli_trmm_ru_ker_var2.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     3054 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/3/trmm/bli_trmm_var.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2835 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/3/trmm/bli_trmm_xx_ker_var2.c
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.754469 blis-0.9.1.dev1/blis/_src/frame/3/trmm/other/
+-rw-r--r--   0 vsts      (1001) docker     (121)    16003 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/3/trmm/other/bli_trmm_ll_ker_var2.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    16941 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/3/trmm/other/bli_trmm_ll_ker_var2rr.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    16933 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/3/trmm/other/bli_trmm_ll_ker_var2sl.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    16175 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/3/trmm/other/bli_trmm_lu_ker_var2.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    17053 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/3/trmm/other/bli_trmm_lu_ker_var2rr.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    17046 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/3/trmm/other/bli_trmm_lu_ker_var2sl.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    16489 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/3/trmm/other/bli_trmm_rl_ker_var2.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    18922 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/3/trmm/other/bli_trmm_rl_ker_var2rr.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    18915 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/3/trmm/other/bli_trmm_rl_ker_var2sl.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    16500 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/3/trmm/other/bli_trmm_ru_ker_var2.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    19844 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/3/trmm/other/bli_trmm_ru_ker_var2rr.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    19837 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/3/trmm/other/bli_trmm_ru_ker_var2sl.c
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.754469 blis-0.9.1.dev1/blis/_src/frame/3/trmm3/
+-rw-r--r--   0 vsts      (1001) docker     (121)     1703 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/3/trmm3/bli_trmm3.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     6378 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/3/trmm3/bli_trmm3_front.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     1889 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/3/trmm3/bli_trmm3_front.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.758469 blis-0.9.1.dev1/blis/_src/frame/3/trsm/
+-rw-r--r--   0 vsts      (1001) docker     (121)     1755 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/3/trsm/bli_trsm.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     6318 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/3/trsm/bli_trsm_blk_var1.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     3075 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/3/trsm/bli_trsm_blk_var2.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     3331 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/3/trsm/bli_trsm_blk_var3.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     8562 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/3/trsm/bli_trsm_cntl.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2522 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/3/trsm/bli_trsm_cntl.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     5204 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/3/trsm/bli_trsm_front.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2105 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/3/trsm/bli_trsm_front.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    15924 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/3/trsm/bli_trsm_ll_ker_var2.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    16411 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/3/trsm/bli_trsm_lu_ker_var2.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    16640 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/3/trsm/bli_trsm_rl_ker_var2.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    16270 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/3/trsm/bli_trsm_ru_ker_var2.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     3051 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/3/trsm/bli_trsm_var.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2835 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/3/trsm/bli_trsm_xx_ker_var2.c
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.758469 blis-0.9.1.dev1/blis/_src/frame/3/trsm/other/
+-rw-r--r--   0 vsts      (1001) docker     (121)    19746 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/3/trsm/other/bli_trsm_ll_ker_var2.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    20427 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/3/trsm/other/bli_trsm_ll_ker_var2rr.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    20420 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/3/trsm/other/bli_trsm_ll_ker_var2sl.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    18777 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/3/trsm/other/bli_trsm_lu_ker_var2.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    19458 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/3/trsm/other/bli_trsm_lu_ker_var2rr.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    19451 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/3/trsm/other/bli_trsm_lu_ker_var2sl.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    19921 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/3/trsm/other/bli_trsm_rl_ker_var2.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    19537 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/3/trsm/other/bli_trsm_ru_ker_var2.c
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.766469 blis-0.9.1.dev1/blis/_src/frame/base/
+-rw-r--r--   0 vsts      (1001) docker     (121)    18338 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/base/bli_apool.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     3579 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/base/bli_apool.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     9301 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/base/bli_arch.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2005 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/base/bli_arch.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     6732 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/base/bli_array.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     3086 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/base/bli_array.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     3623 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/base/bli_auxinfo.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    10571 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/base/bli_blksz.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     7214 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/base/bli_blksz.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    22154 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/base/bli_check.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     5144 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/base/bli_check.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     4618 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/base/bli_clock.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     1833 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/base/bli_clock.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    11136 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/base/bli_cntl.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     5458 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/base/bli_cntl.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    51655 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/base/bli_cntx.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    21693 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/base/bli_cntx.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     3336 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/base/bli_const.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     1736 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/base/bli_const.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    40207 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/base/bli_cpuid.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     6867 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/base/bli_cpuid.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     4491 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/base/bli_env.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     1955 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/base/bli_env.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     8639 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/base/bli_error.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2126 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/base/bli_error.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     3170 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/base/bli_func.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2914 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/base/bli_func.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     6220 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/base/bli_getopt.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     1954 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/base/bli_getopt.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    28407 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/base/bli_gks.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2689 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/base/bli_gks.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     6060 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/base/bli_ind.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2642 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/base/bli_ind.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     7720 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/base/bli_info.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     5455 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/base/bli_info.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     4444 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/base/bli_init.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     1941 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/base/bli_init.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     3549 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/base/bli_machval.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2123 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/base/bli_machval.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     7665 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/base/bli_malloc.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2804 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/base/bli_malloc.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2347 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/base/bli_mbool.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2354 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/base/bli_mbool.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     4266 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/base/bli_mem.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2637 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/base/bli_memsys.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     1998 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/base/bli_memsys.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    20018 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/base/bli_obj.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     3572 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/base/bli_obj.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     7575 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/base/bli_obj_scalar.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2599 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/base/bli_obj_scalar.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1798 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/base/bli_opid.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     5047 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/base/bli_pack.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2072 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/base/bli_pack.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     7681 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/base/bli_param_map.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     5701 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/base/bli_param_map.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    24778 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/base/bli_part.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     3447 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/base/bli_part.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    17574 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/base/bli_pba.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     4486 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/base/bli_pba.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    22049 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/base/bli_pool.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     6726 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/base/bli_pool.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     5700 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/base/bli_prune.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     1783 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/base/bli_prune.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     5928 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/base/bli_query.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     1856 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/base/bli_query.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    14720 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/base/bli_rntm.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    10592 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/base/bli_rntm.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     5914 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/base/bli_sba.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2382 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/base/bli_sba.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     4823 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/base/bli_setgetijm.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2668 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/base/bli_setgetijm.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     4380 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/base/bli_setgetijv.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2561 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/base/bli_setgetijv.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     4830 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/base/bli_setri.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2177 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/base/bli_setri.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1906 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/base/bli_string.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     1709 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/base/bli_string.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2377 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/base/bli_winsys.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     1801 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/base/bli_winsys.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.766469 blis-0.9.1.dev1/blis/_src/frame/base/cast/
+-rw-r--r--   0 vsts      (1001) docker     (121)     6855 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/base/cast/bli_castm.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2362 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/base/cast/bli_castm.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     6875 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/base/cast/bli_castnzm.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2370 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/base/cast/bli_castnzm.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     5161 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/base/cast/bli_castv.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2317 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/base/cast/bli_castv.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.766469 blis-0.9.1.dev1/blis/_src/frame/base/cast/old/
+-rw-r--r--   0 vsts      (1001) docker     (121)     3350 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/base/cast/old/bli_cast_check.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     1812 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/base/cast/old/bli_cast_check.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.766469 blis-0.9.1.dev1/blis/_src/frame/base/check/
+-rw-r--r--   0 vsts      (1001) docker     (121)     5732 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/base/check/bli_obj_check.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2965 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/base/check/bli_obj_check.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     3263 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/base/check/bli_part_check.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2476 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/base/check/bli_part_check.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.766469 blis-0.9.1.dev1/blis/_src/frame/base/noopt/
+-rw-r--r--   0 vsts      (1001) docker     (121)    29298 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/base/noopt/bli_dlamch.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     1738 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/base/noopt/bli_dlamch.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2797 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/base/noopt/bli_lsame.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     1766 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/base/noopt/bli_lsame.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    29227 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/base/noopt/bli_slamch.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     1736 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/base/noopt/bli_slamch.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.766469 blis-0.9.1.dev1/blis/_src/frame/base/proj/
+-rw-r--r--   0 vsts      (1001) docker     (121)     3662 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/base/proj/bli_projm.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     1824 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/base/proj/bli_projm.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     3668 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/base/proj/bli_projv.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     1824 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/base/proj/bli_projv.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.766469 blis-0.9.1.dev1/blis/_src/frame/base/proj/old/
+-rw-r--r--   0 vsts      (1001) docker     (121)     3286 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/base/proj/old/bli_proj_check.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     1812 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/base/proj/old/bli_proj_check.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.770469 blis-0.9.1.dev1/blis/_src/frame/compat/
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.770469 blis-0.9.1.dev1/blis/_src/frame/compat/amd/
+-rw-r--r--   0 vsts      (1001) docker     (121)     4686 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/amd/bla_copy_amd.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     5686 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/amd/bla_gemv_amd.c
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.774469 blis-0.9.1.dev1/blis/_src/frame/compat/attic/
+-rw-r--r--   0 vsts      (1001) docker     (121)     3273 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/attic/bla_gbmv.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2405 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/attic/bla_gbmv.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2971 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/attic/bla_hbmv.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2336 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/attic/bla_hbmv.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2914 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/attic/bla_hpmv.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2279 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/attic/bla_hpmv.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2722 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/attic/bla_hpr.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2174 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/attic/bla_hpr.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2868 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/attic/bla_hpr2.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2233 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/attic/bla_hpr2.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2725 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/attic/bla_rot.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2235 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/attic/bla_rot.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2215 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/attic/bla_rotg.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2133 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/attic/bla_rotg.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2602 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/attic/bla_rotm.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2126 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/attic/bla_rotm.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2219 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/attic/bla_rotmg.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2136 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/attic/bla_rotmg.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2957 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/attic/bla_sbmv.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2322 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/attic/bla_sbmv.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2900 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/attic/bla_spmv.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2265 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/attic/bla_spmv.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2708 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/attic/bla_spr.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2160 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/attic/bla_spr.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2854 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/attic/bla_spr2.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2219 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/attic/bla_spr2.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2981 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/attic/bla_tbmv.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2260 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/attic/bla_tbmv.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2981 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/attic/bla_tbsv.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2260 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/attic/bla_tbsv.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2924 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/attic/bla_tpmv.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2203 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/attic/bla_tpmv.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2924 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/attic/bla_tpsv.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2203 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/attic/bla_tpsv.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     3167 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/bla_amax.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     1989 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/bla_amax.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2638 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/bla_asum.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2011 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/bla_asum.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2780 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/bla_axpy.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2057 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/bla_axpy.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2729 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/bla_copy.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2026 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/bla_copy.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     5756 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/bla_dot.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     3010 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/bla_dot.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     7103 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/bla_gemm.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2261 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/bla_gemm.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     4788 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/bla_gemv.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2202 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/bla_gemv.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     3272 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/bla_ger.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2154 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/bla_ger.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     6206 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/bla_hemm.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2250 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/bla_hemm.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     3440 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/bla_hemv.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2193 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/bla_hemv.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     3196 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/bla_her.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2112 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/bla_her.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     3390 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/bla_her2.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2162 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/bla_her2.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     7171 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/bla_her2k.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2253 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/bla_her2k.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     6602 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/bla_herk.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2204 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/bla_herk.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2639 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/bla_nrm2.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2011 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/bla_nrm2.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     3012 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/bla_scal.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2039 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/bla_scal.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2693 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/bla_swap.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2014 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/bla_swap.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     6168 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/bla_symm.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2230 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/bla_symm.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     3426 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/bla_symv.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2179 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/bla_symv.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     3180 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/bla_syr.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2098 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/bla_syr.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     3378 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/bla_syr2.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2148 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/bla_syr2.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     6799 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/bla_syr2k.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2233 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/bla_syr2k.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     6224 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/bla_syrk.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2184 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/bla_syrk.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     5926 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/bla_trmm.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2216 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/bla_trmm.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     3523 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/bla_trmv.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2126 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/bla_trmv.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     5926 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/bla_trsm.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2216 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/bla_trsm.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     3523 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/bla_trsv.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2126 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/bla_trsv.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     5539 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/bli_blas.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.706469 blis-0.9.1.dev1/blis/_src/frame/compat/blis/
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.774469 blis-0.9.1.dev1/blis/_src/frame/compat/blis/thread/
+-rw-r--r--   0 vsts      (1001) docker     (121)     2754 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/blis/thread/b77_thread.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2029 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/blis/thread/b77_thread.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.774469 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/
+-rw-r--r--   0 vsts      (1001) docker     (121)     2157 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/bli_cblas.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.774469 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/f77_sub/
+-rw-r--r--   0 vsts      (1001) docker     (121)     2149 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/f77_sub/f77_amax_sub.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2032 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/f77_sub/f77_amax_sub.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2173 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/f77_sub/f77_asum_sub.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2054 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/f77_sub/f77_asum_sub.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     3760 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/f77_sub/f77_dot_sub.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2582 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/f77_sub/f77_dot_sub.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2173 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/f77_sub/f77_nrm2_sub.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2054 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/f77_sub/f77_nrm2_sub.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.786469 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/
+-rw-r--r--   0 vsts      (1001) docker     (121)    37101 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas.h
+-rw-r--r--   0 vsts      (1001) docker     (121)      576 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_caxpy.c
+-rw-r--r--   0 vsts      (1001) docker     (121)      537 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_ccopy.c
+-rw-r--r--   0 vsts      (1001) docker     (121)      635 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_cdotc_sub.c
+-rw-r--r--   0 vsts      (1001) docker     (121)      637 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_cdotu_sub.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     4350 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_cgbmv.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     3116 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_cgemm.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     4255 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_cgemv.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2037 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_cgerc.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     1251 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_cgeru.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     3659 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_chbmv.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2798 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_chemm.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     3617 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_chemv.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2635 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_cher.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     3506 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_cher2.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2981 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_cher2k.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2739 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_cherk.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     3543 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_chpmv.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2562 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_chpr.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     3375 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_chpr2.c
+-rw-r--r--   0 vsts      (1001) docker     (121)      484 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_cscal.c
+-rw-r--r--   0 vsts      (1001) docker     (121)      469 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_csscal.c
+-rw-r--r--   0 vsts      (1001) docker     (121)      532 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_cswap.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2793 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_csymm.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2919 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_csyr2k.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2790 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_csyrk.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     4032 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_ctbmv.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     4041 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_ctbsv.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     3848 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_ctpmv.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     3858 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_ctpsv.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     3986 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_ctrmm.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     3965 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_ctrmv.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     4044 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_ctrsm.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     3981 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_ctrsv.c
+-rw-r--r--   0 vsts      (1001) docker     (121)      518 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_dasum.c
+-rw-r--r--   0 vsts      (1001) docker     (121)      543 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_daxpy.c
+-rw-r--r--   0 vsts      (1001) docker     (121)      519 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_dcopy.c
+-rw-r--r--   0 vsts      (1001) docker     (121)      619 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_ddot.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2296 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_dgbmv.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2989 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_dgemm.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2145 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_dgemv.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     1179 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_dger.c
+-rw-r--r--   0 vsts      (1001) docker     (121)      517 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_dnrm2.c
+-rw-r--r--   0 vsts      (1001) docker     (121)      541 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_drot.c
+-rw-r--r--   0 vsts      (1001) docker     (121)      303 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_drotg.c
+-rw-r--r--   0 vsts      (1001) docker     (121)      420 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_drotm.c
+-rw-r--r--   0 vsts      (1001) docker     (121)      354 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_drotmg.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2028 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_dsbmv.c
+-rw-r--r--   0 vsts      (1001) docker     (121)      458 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_dscal.c
+-rw-r--r--   0 vsts      (1001) docker     (121)      624 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_dsdot.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     1909 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_dspmv.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     1688 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_dspr.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     1788 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_dspr2.c
+-rw-r--r--   0 vsts      (1001) docker     (121)      514 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_dswap.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2686 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_dsymm.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     1973 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_dsymv.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     1765 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_dsyr.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     1932 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_dsyr2.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2825 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_dsyr2k.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2700 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_dsyrk.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     3308 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_dtbmv.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     3318 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_dtbsv.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     3135 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_dtpmv.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     3136 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_dtpsv.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     3981 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_dtrmm.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     3277 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_dtrmv.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     4061 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_dtrsm.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     3263 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_dtrsv.c
+-rw-r--r--   0 vsts      (1001) docker     (121)      521 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_dzasum.c
+-rw-r--r--   0 vsts      (1001) docker     (121)      521 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_dznrm2.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     6368 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_f77.h
+-rw-r--r--   0 vsts      (1001) docker     (121)       93 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_globals.c
+-rw-r--r--   0 vsts      (1001) docker     (121)      550 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_icamax.c
+-rw-r--r--   0 vsts      (1001) docker     (121)      541 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_idamax.c
+-rw-r--r--   0 vsts      (1001) docker     (121)      540 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_isamax.c
+-rw-r--r--   0 vsts      (1001) docker     (121)      552 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_izamax.c
+-rw-r--r--   0 vsts      (1001) docker     (121)      515 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_sasum.c
+-rw-r--r--   0 vsts      (1001) docker     (121)      594 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_saxpy.c
+-rw-r--r--   0 vsts      (1001) docker     (121)      519 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_scasum.c
+-rw-r--r--   0 vsts      (1001) docker     (121)      519 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_scnrm2.c
+-rw-r--r--   0 vsts      (1001) docker     (121)      517 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_scopy.c
+-rw-r--r--   0 vsts      (1001) docker     (121)      615 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_sdot.c
+-rw-r--r--   0 vsts      (1001) docker     (121)      646 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_sdsdot.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2303 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_sgbmv.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     3129 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_sgemm.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2126 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_sgemv.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     1151 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_sger.c
+-rw-r--r--   0 vsts      (1001) docker     (121)      515 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_snrm2.c
+-rw-r--r--   0 vsts      (1001) docker     (121)      548 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_srot.c
+-rw-r--r--   0 vsts      (1001) docker     (121)      299 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_srotg.c
+-rw-r--r--   0 vsts      (1001) docker     (121)      534 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_srotm.c
+-rw-r--r--   0 vsts      (1001) docker     (121)      349 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_srotmg.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     1953 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_ssbmv.c
+-rw-r--r--   0 vsts      (1001) docker     (121)      456 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_sscal.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     1890 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_sspmv.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     1694 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_sspr.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     1789 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_sspr2.c
+-rw-r--r--   0 vsts      (1001) docker     (121)      512 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_sswap.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2760 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_ssymm.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     1968 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_ssymv.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     1761 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_ssyr.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     1928 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_ssyr2.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2900 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_ssyr2k.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2778 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_ssyrk.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     3333 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_stbmv.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     3317 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_stbsv.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     3148 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_stpmv.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     3134 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_stpsv.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     3953 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_strmm.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     3276 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_strmv.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     3975 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_strsm.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     3261 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_strsv.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     1982 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_xerbla.c
+-rw-r--r--   0 vsts      (1001) docker     (121)      576 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_zaxpy.c
+-rw-r--r--   0 vsts      (1001) docker     (121)      537 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_zcopy.c
+-rw-r--r--   0 vsts      (1001) docker     (121)      647 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_zdotc_sub.c
+-rw-r--r--   0 vsts      (1001) docker     (121)      649 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_zdotu_sub.c
+-rw-r--r--   0 vsts      (1001) docker     (121)      471 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_zdscal.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     4367 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_zgbmv.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     3112 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_zgemm.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     4219 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_zgemv.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2042 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_zgerc.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     1251 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_zgeru.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     3669 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_zhbmv.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2799 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_zhemm.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     3625 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_zhemv.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2560 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_zher.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     3522 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_zher2.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2981 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_zher2k.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2741 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_zherk.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     3553 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_zhpmv.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2568 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_zhpr.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     3399 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_zhpr2.c
+-rw-r--r--   0 vsts      (1001) docker     (121)      482 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_zscal.c
+-rw-r--r--   0 vsts      (1001) docker     (121)      534 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_zswap.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2794 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_zsymm.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2919 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_zsyr2k.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2790 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_zsyrk.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     4034 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_ztbmv.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     4043 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_ztbsv.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     3850 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_ztpmv.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     3860 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_ztpsv.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     4062 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_ztrmm.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     3981 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_ztrmv.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     4078 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_ztrsm.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     3983 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_ztrsv.c
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.790469 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/extra/
+-rw-r--r--   0 vsts      (1001) docker     (121)      646 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/extra/cblas_caxpby.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     3181 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/extra/cblas_cgemm3m.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     5593 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/extra/cblas_cgemm_batch.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     5349 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/extra/cblas_cgemmt.c
+-rw-r--r--   0 vsts      (1001) docker     (121)      594 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/extra/cblas_daxpby.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     5439 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/extra/cblas_dgemm_batch.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     5239 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/extra/cblas_dgemmt.c
+-rw-r--r--   0 vsts      (1001) docker     (121)      647 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/extra/cblas_saxpby.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     5435 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/extra/cblas_sgemm_batch.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     5234 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/extra/cblas_sgemmt.c
+-rw-r--r--   0 vsts      (1001) docker     (121)      648 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/extra/cblas_zaxpby.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     3179 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/extra/cblas_zgemm3m.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     5593 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/extra/cblas_zgemm_batch.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     5349 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/extra/cblas_zgemmt.c
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.790469 blis-0.9.1.dev1/blis/_src/frame/compat/check/
+-rw-r--r--   0 vsts      (1001) docker     (121)     3139 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/check/bla_gemm3m_check.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     3064 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/check/bla_gemm_check.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     3228 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/check/bla_gemmt_check.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2539 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/check/bla_gemv_check.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2370 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/check/bla_ger_check.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2782 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/check/bla_hemm_check.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2422 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/check/bla_hemv_check.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2421 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/check/bla_her2_check.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2783 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/check/bla_her2k_check.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2374 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/check/bla_her_check.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2726 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/check/bla_herk_check.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1744 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/check/bla_symm_check.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1744 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/check/bla_symv_check.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1744 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/check/bla_syr2_check.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2973 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/check/bla_syr2k_check.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1742 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/check/bla_syr_check.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2917 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/check/bla_syrk_check.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     3221 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/check/bla_trmm_check.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2873 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/check/bla_trmv_check.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1744 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/check/bla_trsm_check.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1744 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/check/bla_trsv_check.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.790469 blis-0.9.1.dev1/blis/_src/frame/compat/extra/
+-rw-r--r--   0 vsts      (1001) docker     (121)     2829 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/extra/bla_axpby.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2083 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/extra/bla_axpby.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     7544 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/extra/bla_gemm3m.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2299 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/extra/bla_gemm3m.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     7296 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/extra/bla_gemm_batch.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2415 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/extra/bla_gemm_batch.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     6351 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/extra/bla_gemmt.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2318 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/extra/bla_gemmt.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.794469 blis-0.9.1.dev1/blis/_src/frame/compat/f2c/
+-rw-r--r--   0 vsts      (1001) docker     (121)     2347 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/f2c/bla_cabs1.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     1834 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/f2c/bla_cabs1.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    51775 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/f2c/bla_gbmv.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     3066 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/f2c/bla_gbmv.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    36539 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/f2c/bla_hbmv.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2306 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/f2c/bla_hbmv.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    32318 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/f2c/bla_hpmv.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2216 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/f2c/bla_hpmv.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    22952 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/f2c/bla_hpr.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2060 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/f2c/bla_hpr.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    33391 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/f2c/bla_hpr2.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2164 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/f2c/bla_hpr2.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     4594 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/f2c/bla_lsame.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     1915 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/f2c/bla_lsame.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    10542 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/f2c/bla_rot.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2448 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/f2c/bla_rot.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     8027 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/f2c/bla_rotg.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2120 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/f2c/bla_rotg.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     9056 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/f2c/bla_rotm.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2038 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/f2c/bla_rotm.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    11542 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/f2c/bla_rotmg.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     1964 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/f2c/bla_rotmg.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    21669 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/f2c/bla_sbmv.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2276 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/f2c/bla_sbmv.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    17321 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/f2c/bla_spmv.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2186 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/f2c/bla_spmv.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    13888 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/f2c/bla_spr.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2048 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/f2c/bla_spr.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    16058 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/f2c/bla_spr2.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2140 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/f2c/bla_spr2.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    67667 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/f2c/bla_tbmv.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2710 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/f2c/bla_tbmv.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    64601 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/f2c/bla_tbsv.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2710 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/f2c/bla_tbsv.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    55833 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/f2c/bla_tpmv.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2530 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/f2c/bla_tpmv.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    52801 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/f2c/bla_tpsv.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2530 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/f2c/bla_tpsv.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     3215 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/f2c/bla_xerbla.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     1836 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/f2c/bla_xerbla.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2599 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/f2c/bla_xerbla_array.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     1836 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/f2c/bla_xerbla_array.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.798469 blis-0.9.1.dev1/blis/_src/frame/compat/f2c/util/
+-rw-r--r--   0 vsts      (1001) docker     (121)     1852 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/f2c/util/bla_c_abs.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     1748 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/f2c/util/bla_c_abs.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1864 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/f2c/util/bla_c_div.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     1789 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/f2c/util/bla_c_div.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1813 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/f2c/util/bla_d_abs.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     1746 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/f2c/util/bla_d_abs.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1820 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/f2c/util/bla_d_cnjg.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     1769 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/f2c/util/bla_d_cnjg.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1796 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/f2c/util/bla_d_imag.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     1749 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/f2c/util/bla_d_imag.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1857 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/f2c/util/bla_d_sign.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     1768 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/f2c/util/bla_d_sign.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2116 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/f2c/util/bla_f__cabs.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     1753 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/f2c/util/bla_f__cabs.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1811 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/f2c/util/bla_r_abs.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     1744 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/f2c/util/bla_r_abs.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1820 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/f2c/util/bla_r_cnjg.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     1769 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/f2c/util/bla_r_cnjg.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1798 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/f2c/util/bla_r_imag.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     1751 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/f2c/util/bla_r_imag.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1853 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/f2c/util/bla_r_sign.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     1764 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/f2c/util/bla_r_sign.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1852 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/f2c/util/bla_z_abs.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     1748 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/f2c/util/bla_z_abs.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1864 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/f2c/util/bla_z_div.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     1789 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/compat/f2c/util/bla_z_div.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.802469 blis-0.9.1.dev1/blis/_src/frame/include/
+-rw-r--r--   0 vsts      (1001) docker     (121)     7804 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/bli_arch_config.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2808 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/bli_arch_config_pre.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     3176 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/bli_blas_macro_defs.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2052 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/bli_builtin_macro_defs.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2337 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/bli_complex_macro_defs.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    10343 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/bli_config_macro_defs.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     7737 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/bli_edge_case_macro_defs.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1922 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/bli_error_macro_defs.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2225 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/bli_extern_defs.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2301 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/bli_f2c.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    10772 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/bli_genarray_macro_defs.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2871 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/bli_gentdef_macro_defs.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    54463 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/bli_gentfunc_macro_defs.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    27414 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/bli_gentprot_macro_defs.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     8415 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/bli_kernel_macro_defs.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     4043 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/bli_lang_defs.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     4527 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/bli_macro_defs.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     4435 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/bli_misc_macro_defs.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2547 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/bli_oapi_ba.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2469 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/bli_oapi_ex.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1808 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/bli_oapi_macro_defs.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    40527 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/bli_obj_macro_defs.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    33815 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/bli_param_macro_defs.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2687 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/bli_pragma_macro_defs.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2035 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/bli_sbox.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     5762 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/bli_scalar_macro_defs.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     4131 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/bli_system.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2546 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/bli_tapi_ba.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2468 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/bli_tapi_ex.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1807 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/bli_tapi_macro_defs.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    43725 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/bli_type_defs.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    46891 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/bli_x86_asm_macros.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2425 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/bli_xapi_undef.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     5488 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/blis.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.806469 blis-0.9.1.dev1/blis/_src/frame/include/level0/
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.806469 blis-0.9.1.dev1/blis/_src/frame/include/level0/1e/
+-rw-r--r--   0 vsts      (1001) docker     (121)     3282 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/level0/1e/bli_copy1es.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     3305 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/level0/1e/bli_copyj1es.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2108 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/level0/1e/bli_invert1es.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2166 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/level0/1e/bli_scal1es.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    10659 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/level0/1e/bli_scal21es.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    10730 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/level0/1e/bli_scal2j1es.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.806469 blis-0.9.1.dev1/blis/_src/frame/include/level0/1m/
+-rw-r--r--   0 vsts      (1001) docker     (121)     4503 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/level0/1m/bli_invert1ms_mxn_diag.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     3942 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/level0/1m/bli_scal1ms_mxn.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     5933 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/level0/1m/bli_scal21ms_mxn.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     4280 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/level0/1m/bli_scal21ms_mxn_diag.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     8706 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/level0/1m/bli_scal21ms_mxn_uplo.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     6489 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/level0/1m/bli_set1ms_mxn.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     4578 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/level0/1m/bli_set1ms_mxn_diag.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     6132 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/level0/1m/bli_set1ms_mxn_uplo.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     3702 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/level0/1m/bli_seti01ms_mxn_diag.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.806469 blis-0.9.1.dev1/blis/_src/frame/include/level0/1r/
+-rw-r--r--   0 vsts      (1001) docker     (121)     1936 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/level0/1r/bli_copy1rs.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1943 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/level0/1r/bli_copyj1rs.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1864 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/level0/1r/bli_invert1rs.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2136 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/level0/1r/bli_scal1rs.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2421 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/level0/1r/bli_scal21rs.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2432 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/level0/1r/bli_scal2j1rs.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.806469 blis-0.9.1.dev1/blis/_src/frame/include/level0/bb/
+-rw-r--r--   0 vsts      (1001) docker     (121)     2480 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/level0/bb/bli_bcastbbs_mxn.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     6341 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/level0/bb/bli_scal2bbs_mxn.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2468 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/level0/bb/bli_set0bbs_mxn.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     4986 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/level0/bli_absq2s.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     5104 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/level0/bli_abval2s.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    12899 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/level0/bli_add3s.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     4141 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/level0/bli_addjs.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     4050 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/level0/bli_adds.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    16133 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/level0/bli_adds_mxn.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     5651 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/level0/bli_adds_mxn_uplo.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    12947 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/level0/bli_axmys.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    55936 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/level0/bli_axpbyjs.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    54645 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/level0/bli_axpbys.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    13190 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/level0/bli_axpyjs.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    12947 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/level0/bli_axpys.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2208 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/level0/bli_conjs.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     3205 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/level0/bli_constants.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     4815 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/level0/bli_copycjs.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     4072 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/level0/bli_copyjnzs.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     4292 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/level0/bli_copyjs.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     3942 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/level0/bli_copynzs.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     3912 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/level0/bli_copys.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    16273 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/level0/bli_copys_mxn.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     5870 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/level0/bli_dotjs.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     5697 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/level0/bli_dots.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     4078 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/level0/bli_eq.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2327 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/level0/bli_fprints.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     4005 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/level0/bli_gets.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2292 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/level0/bli_inverts.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     4353 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/level0/bli_invscaljs.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     4262 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/level0/bli_invscals.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     4101 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/level0/bli_neg2s.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     5379 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/level0/bli_randnp2s.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2302 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/level0/bli_rands.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    13377 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/level0/bli_scal2js.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    13133 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/level0/bli_scal2s.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2891 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/level0/bli_scal2s_mxn.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     4699 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/level0/bli_scalcjs.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     4200 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/level0/bli_scaljs.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     4109 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/level0/bli_scals.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1941 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/level0/bli_set0s.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2883 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/level0/bli_set0s_mxn.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1941 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/level0/bli_set1s.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1927 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/level0/bli_seti0s.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2781 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/level0/bli_setis.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2821 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/level0/bli_setrs.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     4279 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/level0/bli_sets.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     5073 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/level0/bli_sqrt2s.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     4141 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/level0/bli_subjs.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     4050 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/level0/bli_subs.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     4194 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/level0/bli_swaps.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    13325 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/level0/bli_xpbyjs.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    13154 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/level0/bli_xpbys.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    21503 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/level0/bli_xpbys_mxn.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     8639 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/level0/bli_xpbys_mxn_uplo.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.806469 blis-0.9.1.dev1/blis/_src/frame/include/level0/old/
+-rw-r--r--   0 vsts      (1001) docker     (121)     4610 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/level0/old/bli_cast.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1672 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/level0/old/bli_castfrom.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1672 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/level0/old/bli_castto.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     3590 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/level0/old/bli_copynzjs.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     3518 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/level0/old/bli_copynzs.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     5273 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/level0/old/bli_invscalcjs.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     4707 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/level0/old/bli_scalcjs.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2692 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/level0/old/bli_set0ris_mxn.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.806469 blis-0.9.1.dev1/blis/_src/frame/include/level0/old/io/
+-rw-r--r--   0 vsts      (1001) docker     (121)     2133 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/level0/old/io/bli_scal2ios.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1973 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/level0/old/io/bli_scal2jios.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.810469 blis-0.9.1.dev1/blis/_src/frame/include/level0/old/ri3/
+-rw-r--r--   0 vsts      (1001) docker     (121)     2127 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/level0/old/ri3/bli_copyjri3s.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2107 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/level0/old/ri3/bli_copyri3s.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2521 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/level0/old/ri3/bli_scal2jri3s.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2508 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/level0/old/ri3/bli_scal2ri3s.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     5780 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/level0/old/ri3/bli_scal2ri3s_mxn.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.810469 blis-0.9.1.dev1/blis/_src/frame/include/level0/old/rih/
+-rw-r--r--   0 vsts      (1001) docker     (121)     6836 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/level0/old/rih/bli_scal2rihs_mxn.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     3540 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/level0/old/rih/bli_scal2rihs_mxn_diag.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     9612 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/level0/old/rih/bli_scal2rihs_mxn_uplo.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     3410 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/level0/old/rih/bli_setrihs_mxn_diag.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.810469 blis-0.9.1.dev1/blis/_src/frame/include/level0/old/ro/
+-rw-r--r--   0 vsts      (1001) docker     (121)     1972 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/level0/old/ro/bli_scal2jros.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2134 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/level0/old/ro/bli_scal2ros.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.810469 blis-0.9.1.dev1/blis/_src/frame/include/level0/old/rpi/
+-rw-r--r--   0 vsts      (1001) docker     (121)     2073 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/level0/old/rpi/bli_scal2jrpis.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2325 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/level0/old/rpi/bli_scal2rpis.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.814469 blis-0.9.1.dev1/blis/_src/frame/include/level0/ri/
+-rw-r--r--   0 vsts      (1001) docker     (121)     2090 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/level0/ri/bli_absq2ris.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2498 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/level0/ri/bli_abval2ris.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2102 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/level0/ri/bli_add3ris.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2057 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/level0/ri/bli_addjris.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2063 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/level0/ri/bli_addris.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2374 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/level0/ri/bli_axmyris.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     3396 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/level0/ri/bli_axpbyjris.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     3350 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/level0/ri/bli_axpbyris.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     5481 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/level0/ri/bli_axpyjris.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     5335 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/level0/ri/bli_axpyris.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1944 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/level0/ri/bli_conjris.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2402 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/level0/ri/bli_copycjris.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     3288 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/level0/ri/bli_copyjris.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     3215 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/level0/ri/bli_copyris.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     3132 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/level0/ri/bli_eqris.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2375 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/level0/ri/bli_invertris.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2280 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/level0/ri/bli_invscaljris.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2738 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/level0/ri/bli_invscalris.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2034 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/level0/ri/bli_neg2ris.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     9077 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/level0/ri/bli_scal2jris.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     5471 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/level0/ri/bli_scal2ris.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     5265 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/level0/ri/bli_scal2ris_mxn.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2656 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/level0/ri/bli_scalcjris.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2235 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/level0/ri/bli_scaljris.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2422 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/level0/ri/bli_scalris.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     3309 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/level0/ri/bli_scalris_mxn_uplo.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2005 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/level0/ri/bli_set0ris.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2811 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/level0/ri/bli_sqrt2ris.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2057 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/level0/ri/bli_subjris.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2063 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/level0/ri/bli_subris.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2531 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/level0/ri/bli_swapris.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     5459 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/level0/ri/bli_xpbyjris.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     5313 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/include/level0/ri/bli_xpbyris.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.818469 blis-0.9.1.dev1/blis/_src/frame/thread/
+-rw-r--r--   0 vsts      (1001) docker     (121)     2636 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/thread/bli_l3_decor.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     8790 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/thread/bli_l3_decor_openmp.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2065 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/thread/bli_l3_decor_openmp.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     8650 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/thread/bli_l3_decor_pthreads.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     1941 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/thread/bli_l3_decor_pthreads.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     5533 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/thread/bli_l3_decor_single.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     1859 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/thread/bli_l3_decor_single.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2646 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/thread/bli_l3_sup_decor.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     5123 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/thread/bli_l3_sup_decor_openmp.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     1864 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/thread/bli_l3_sup_decor_openmp.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     7091 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/thread/bli_l3_sup_decor_pthreads.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     1953 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/thread/bli_l3_sup_decor_pthreads.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     4905 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/thread/bli_l3_sup_decor_single.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     1867 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/thread/bli_l3_sup_decor_single.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    15102 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/thread/bli_pthread.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     7875 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/thread/bli_pthread.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     4729 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/thread/bli_thrcomm.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2627 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/thread/bli_thrcomm.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     5596 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/thread/bli_thrcomm_openmp.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     3203 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/thread/bli_thrcomm_openmp.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     3535 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/thread/bli_thrcomm_pthreads.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2629 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/thread/bli_thrcomm_pthreads.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2733 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/thread/bli_thrcomm_single.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2785 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/thread/bli_thrcomm_single.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    49078 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/thread/bli_thread.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     8482 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/thread/bli_thread.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    20289 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/thread/bli_thrinfo.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     6814 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/thread/bli_thrinfo.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    10397 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/thread/bli_thrinfo_sup.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2300 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/thread/bli_thrinfo_sup.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.818469 blis-0.9.1.dev1/blis/_src/frame/thread/old/
+-rw-r--r--   0 vsts      (1001) docker     (121)     2054 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/thread/old/bli_mutex.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2421 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/thread/old/bli_mutex_openmp.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2469 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/thread/old/bli_mutex_pthreads.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2256 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/thread/old/bli_mutex_single.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.818469 blis-0.9.1.dev1/blis/_src/frame/util/
+-rw-r--r--   0 vsts      (1001) docker     (121)     2343 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/util/bli_util.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     9068 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/util/bli_util_check.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     4264 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/util/bli_util_check.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2873 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/util/bli_util_fpa.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2447 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/util/bli_util_fpa.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     5973 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/util/bli_util_ft.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    16310 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/util/bli_util_oapi.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     4522 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/util/bli_util_oapi.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1977 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/util/bli_util_oapi_ba.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     1975 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/util/bli_util_oapi_ex.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    12097 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/util/bli_util_tapi.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     5854 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/util/bli_util_tapi.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1975 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/util/bli_util_tapi_ba.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     1973 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/util/bli_util_tapi_ex.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    33286 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/util/bli_util_unb_var1.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     5577 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/frame/util/bli_util_unb_var1.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.706469 blis-0.9.1.dev1/blis/_src/include/
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.818469 blis-0.9.1.dev1/blis/_src/include/darwin-firestorm/
+-rw-r--r--   0 vsts      (1001) docker     (121)  1241655 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/include/darwin-firestorm/blis.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.822469 blis-0.9.1.dev1/blis/_src/include/darwin-generic/
+-rw-r--r--   0 vsts      (1001) docker     (121)  1239020 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/include/darwin-generic/blis.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.822469 blis-0.9.1.dev1/blis/_src/include/darwin-x86_64/
+-rw-r--r--   0 vsts      (1001) docker     (121)  1282614 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/include/darwin-x86_64/blis.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.822469 blis-0.9.1.dev1/blis/_src/include/darwin-x86_64_no_skx/
+-rw-r--r--   0 vsts      (1001) docker     (121)  1269093 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/include/darwin-x86_64_no_skx/blis.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.826469 blis-0.9.1.dev1/blis/_src/include/darwin-x86_64_no_zen2/
+-rw-r--r--   0 vsts      (1001) docker     (121)  1274228 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/include/darwin-x86_64_no_zen2/blis.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.826469 blis-0.9.1.dev1/blis/_src/include/darwin-x86_64_no_zen3/
+-rw-r--r--   0 vsts      (1001) docker     (121)  1280323 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/include/darwin-x86_64_no_zen3/blis.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.826469 blis-0.9.1.dev1/blis/_src/include/linux-arm64/
+-rw-r--r--   0 vsts      (1001) docker     (121)  1246399 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/include/linux-arm64/blis.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.830469 blis-0.9.1.dev1/blis/_src/include/linux-arm64_no_sve/
+-rw-r--r--   0 vsts      (1001) docker     (121)  1243881 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/include/linux-arm64_no_sve/blis.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.830469 blis-0.9.1.dev1/blis/_src/include/linux-generic/
+-rw-r--r--   0 vsts      (1001) docker     (121)  1239020 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/include/linux-generic/blis.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.830469 blis-0.9.1.dev1/blis/_src/include/linux-power9/
+-rw-r--r--   0 vsts      (1001) docker     (121)  1239472 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/include/linux-power9/blis.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.834469 blis-0.9.1.dev1/blis/_src/include/linux-x86_64/
+-rw-r--r--   0 vsts      (1001) docker     (121)  1282614 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/include/linux-x86_64/blis.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.834469 blis-0.9.1.dev1/blis/_src/include/linux-x86_64_no_skx/
+-rw-r--r--   0 vsts      (1001) docker     (121)  1269093 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/include/linux-x86_64_no_skx/blis.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.834469 blis-0.9.1.dev1/blis/_src/include/linux-x86_64_no_zen2/
+-rw-r--r--   0 vsts      (1001) docker     (121)  1274228 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/include/linux-x86_64_no_zen2/blis.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.838469 blis-0.9.1.dev1/blis/_src/include/linux-x86_64_no_zen3/
+-rw-r--r--   0 vsts      (1001) docker     (121)  1280323 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/include/linux-x86_64_no_zen3/blis.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.838469 blis-0.9.1.dev1/blis/_src/include/windows-generic/
+-rw-r--r--   0 vsts      (1001) docker     (121)  1281621 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/include/windows-generic/blis.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.842470 blis-0.9.1.dev1/blis/_src/include/windows-x86_64/
+-rw-r--r--   0 vsts      (1001) docker     (121)  1326521 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/include/windows-x86_64/blis.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.710469 blis-0.9.1.dev1/blis/_src/kernels/
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.842470 blis-0.9.1.dev1/blis/_src/kernels/armsve/
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.842470 blis-0.9.1.dev1/blis/_src/kernels/armsve/1m/
+-rw-r--r--   0 vsts      (1001) docker     (121)     2260 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/armsve/1m/armsve512_asm_transpose_d8x2.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     4853 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/armsve/1m/armsve512_asm_transpose_d8x8.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     7979 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/armsve/1m/bli_dpackm_armsve256_int_8xk.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    13414 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/armsve/1m/bli_dpackm_armsve512_asm_10xk.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    13673 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/armsve/1m/bli_dpackm_armsve512_asm_16xk.c
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.842470 blis-0.9.1.dev1/blis/_src/kernels/armsve/1m/old/
+-rw-r--r--   0 vsts      (1001) docker     (121)    13739 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/armsve/1m/old/bli_dpackm_armsve512_int_12xk.c
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.846469 blis-0.9.1.dev1/blis/_src/kernels/armsve/3/
+-rw-r--r--   0 vsts      (1001) docker     (121)    13068 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/armsve/3/armsve_asm_2vx10.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     7360 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/armsve/3/armsve_asm_2vx10cmplx.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     6236 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/armsve/3/armsve_asm_macros.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     4155 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/armsve/3/armsve_asm_macros_cmplx.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1999 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/armsve/3/armsve_asm_macros_dcomplex.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1951 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/armsve/3/armsve_asm_macros_double.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2000 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/armsve/3/armsve_asm_macros_scomplex.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1952 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/armsve/3/armsve_asm_macros_single.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     3760 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/armsve/3/bli_armsve_utils.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2181 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/armsve/3/bli_armsve_utils.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    16175 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/armsve/3/bli_gemm_armsve_asm_c2vx10_unindexed.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    16261 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/armsve/3/bli_gemm_armsve_asm_d2vx10_unindexed.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    15390 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/armsve/3/bli_gemm_armsve_asm_s2vx10_unindexed.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    16121 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/armsve/3/bli_gemm_armsve_asm_z2vx10_unindexed.c
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.846469 blis-0.9.1.dev1/blis/_src/kernels/armsve/3/old/
+-rw-r--r--   0 vsts      (1001) docker     (121)     7945 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/armsve/3/old/armsve_asm_2vx7cmplx.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     6909 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/armsve/3/old/armsve_asm_2vx8cmplx.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1954 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/armsve/3/old/armsve_asm_macros_half.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    52816 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/armsve/3/old/bli_gemm_armsve256_asm_d8x8.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    18788 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/armsve/3/old/bli_gemm_armsve_asm_sh2vx10_unindexed.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    14679 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/armsve/3/old/bli_gemm_armsve_asm_z2vx7_unindexed.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    16041 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/armsve/3/old/bli_gemm_armsve_asm_z2vx8_unindexed.c
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.846469 blis-0.9.1.dev1/blis/_src/kernels/armsve/3/old/sup/
+-rw-r--r--   0 vsts      (1001) docker     (121)    12900 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/armsve/3/old/sup/bli_gemmsup_armsve_ref.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    25880 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/armsve/3/old/sup/bli_gemmsup_cv_armsve_asm_d2vx10_unindexed.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    20498 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/armsve/3/old/sup/bli_gemmsup_rv_armsve_asm_d2vx10_unindexed.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2656 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/armsve/bli_kernels_armsve.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.846469 blis-0.9.1.dev1/blis/_src/kernels/armv7a/
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.846469 blis-0.9.1.dev1/blis/_src/kernels/armv7a/3/
+-rw-r--r--   0 vsts      (1001) docker     (121)     5506 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/armv7a/3/bli_gemm_armv7a_asm_d4x4.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    12462 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/armv7a/3/bli_gemm_armv7a_int_d4x4.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     1974 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/armv7a/bli_kernels_armv7a.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.846469 blis-0.9.1.dev1/blis/_src/kernels/armv8a/
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.850469 blis-0.9.1.dev1/blis/_src/kernels/armv8a/1m/
+-rw-r--r--   0 vsts      (1001) docker     (121)    10641 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/armv8a/1m/bli_packm_armv8a_int_d6xk.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    12067 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/armv8a/1m/bli_packm_armv8a_int_d8xk.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    15957 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/armv8a/1m/bli_packm_armv8a_int_s12xk.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    12799 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/armv8a/1m/bli_packm_armv8a_int_s8xk.c
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.854469 blis-0.9.1.dev1/blis/_src/kernels/armv8a/3/
+-rw-r--r--   0 vsts      (1001) docker     (121)     2195 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/armv8a/3/armv8a_asm_d2x2.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     4187 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/armv8a/3/armv8a_asm_utils.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    85781 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/armv8a/3/bli_gemm_armv8a_asm_d6x8.c
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.854469 blis-0.9.1.dev1/blis/_src/kernels/armv8a/3/old/
+-rw-r--r--   0 vsts      (1001) docker     (121)    11291 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/armv8a/3/old/bli_gemm_armv8a_asm_d4x4.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    14722 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/armv8a/3/old/bli_gemm_armv8a_asm_d6x8r.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    12051 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/armv8a/3/old/bli_gemm_armv8a_asm_d8x4.c
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.854469 blis-0.9.1.dev1/blis/_src/kernels/armv8a/3/sup/
+-rw-r--r--   0 vsts      (1001) docker     (121)    12901 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/armv8a/3/sup/bli_gemmsup_armv8a_ref.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    20091 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/armv8a/3/sup/bli_gemmsup_rd_armv8a_asm_d6x8m.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    22063 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/armv8a/3/sup/bli_gemmsup_rd_armv8a_asm_d6x8n.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    18537 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/armv8a/3/sup/bli_gemmsup_rv_armv8a_asm_d4x8m.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    18689 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/armv8a/3/sup/bli_gemmsup_rv_armv8a_asm_d4x8n.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    21409 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/armv8a/3/sup/bli_gemmsup_rv_armv8a_asm_d6x8m.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    20655 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/armv8a/3/sup/bli_gemmsup_rv_armv8a_asm_d6x8n.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    17688 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/armv8a/3/sup/bli_gemmsup_rv_armv8a_asm_d8x4m.c
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.854469 blis-0.9.1.dev1/blis/_src/kernels/armv8a/3/sup/d3x4/
+-rw-r--r--   0 vsts      (1001) docker     (121)    13051 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/armv8a/3/sup/d3x4/bli_gemmsup_rd_armv8a_asm_d3x4.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    15813 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/armv8a/3/sup/d3x4/bli_gemmsup_rd_armv8a_asm_d6x3.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    14963 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/armv8a/3/sup/d3x4/bli_gemmsup_rd_armv8a_int_d2x8.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    12124 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/armv8a/3/sup/d3x4/bli_gemmsup_rd_armv8a_int_d3x4.c
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.858470 blis-0.9.1.dev1/blis/_src/kernels/armv8a/3/sup/d6x4/
+-rw-r--r--   0 vsts      (1001) docker     (121)    16425 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/armv8a/3/sup/d6x4/bli_gemmsup_rv_armv8a_int_d3x8mn.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    18893 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/armv8a/3/sup/d6x4/bli_gemmsup_rv_armv8a_int_d6x4mn.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2926 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/armv8a/bli_kernels_armv8a.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.858470 blis-0.9.1.dev1/blis/_src/kernels/bgq/
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.858470 blis-0.9.1.dev1/blis/_src/kernels/bgq/1/
+-rw-r--r--   0 vsts      (1001) docker     (121)     2960 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/bgq/1/bli_axpyv_bgq_int.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     3380 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/bgq/1/bli_dotv_bgq_int.c
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.858470 blis-0.9.1.dev1/blis/_src/kernels/bgq/1f/
+-rw-r--r--   0 vsts      (1001) docker     (121)     5553 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/bgq/1f/bli_axpyf_bgq_int.c
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.858470 blis-0.9.1.dev1/blis/_src/kernels/bgq/3/
+-rw-r--r--   0 vsts      (1001) docker     (121)    13754 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/bgq/3/bli_gemm_bgq_int_8x8.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     1902 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/bgq/bli_kernels_bgq.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.858470 blis-0.9.1.dev1/blis/_src/kernels/bulldozer/
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.858470 blis-0.9.1.dev1/blis/_src/kernels/bulldozer/3/
+-rw-r--r--   0 vsts      (1001) docker     (121)    51743 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/bulldozer/3/bli_gemm_bulldozer_asm_d4x6_fma4.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     1906 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/bulldozer/bli_kernels_bulldozer.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.858470 blis-0.9.1.dev1/blis/_src/kernels/haswell/
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.858470 blis-0.9.1.dev1/blis/_src/kernels/haswell/1m/
+-rw-r--r--   0 vsts      (1001) docker     (121)    12085 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/haswell/1m/bli_packm_haswell_asm_c3xk.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    12657 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/haswell/1m/bli_packm_haswell_asm_c8xk.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    11930 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/haswell/1m/bli_packm_haswell_asm_d6xk.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    12196 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/haswell/1m/bli_packm_haswell_asm_d8xk.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    17802 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/haswell/1m/bli_packm_haswell_asm_s16xk.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    13674 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/haswell/1m/bli_packm_haswell_asm_s6xk.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    12174 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/haswell/1m/bli_packm_haswell_asm_z3xk.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    12556 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/haswell/1m/bli_packm_haswell_asm_z4xk.c
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.858470 blis-0.9.1.dev1/blis/_src/kernels/haswell/3/
+-rw-r--r--   0 vsts      (1001) docker     (121)    56813 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/haswell/3/bli_gemm_haswell_asm_d6x8.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    40396 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/haswell/3/bli_gemm_haswell_asm_d8x6.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    41819 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/haswell/3/bli_gemmtrsm_l_haswell_asm_d6x8.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    42186 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/haswell/3/bli_gemmtrsm_u_haswell_asm_d6x8.c
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.862470 blis-0.9.1.dev1/blis/_src/kernels/haswell/3/old/
+-rw-r--r--   0 vsts      (1001) docker     (121)    68808 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/haswell/3/old/bli_gemm_haswell_asm_d12x4.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    64360 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/haswell/3/old/bli_gemm_haswell_asm_d4x12.c
+-rw-r--r--   0 vsts      (1001) docker     (121)   115770 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/haswell/3/old/bli_gemm_haswell_asm_d6x8.c
+-rw-r--r--   0 vsts      (1001) docker     (121)   116155 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/haswell/3/old/bli_gemm_haswell_asm_d8x6.c
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.862470 blis-0.9.1.dev1/blis/_src/kernels/haswell/3/sup/
+-rw-r--r--   0 vsts      (1001) docker     (121)    52381 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/haswell/3/sup/bli_gemmsup_rd_haswell_asm_d6x8m.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    63958 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/haswell/3/sup/bli_gemmsup_rd_haswell_asm_d6x8n.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    87529 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/haswell/3/sup/bli_gemmsup_rd_haswell_asm_s6x16m.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    64915 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/haswell/3/sup/bli_gemmsup_rd_haswell_asm_s6x16n.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    82422 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/haswell/3/sup/bli_gemmsup_rv_haswell_asm_d6x8m.c
+-rw-r--r--   0 vsts      (1001) docker     (121)   113882 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/haswell/3/sup/bli_gemmsup_rv_haswell_asm_d6x8n.c
+-rw-r--r--   0 vsts      (1001) docker     (121)   135283 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/haswell/3/sup/bli_gemmsup_rv_haswell_asm_s6x16m.c
+-rw-r--r--   0 vsts      (1001) docker     (121)   145184 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/haswell/3/sup/bli_gemmsup_rv_haswell_asm_s6x16n.c
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.866469 blis-0.9.1.dev1/blis/_src/kernels/haswell/3/sup/d6x8/
+-rw-r--r--   0 vsts      (1001) docker     (121)     5859 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/haswell/3/sup/d6x8/bli_gemmsup_r_haswell_ref_dMx1.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    45366 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/haswell/3/sup/d6x8/bli_gemmsup_rd_haswell_asm_dMx1.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    49003 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/haswell/3/sup/d6x8/bli_gemmsup_rd_haswell_asm_dMx2.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    38513 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/haswell/3/sup/d6x8/bli_gemmsup_rd_haswell_asm_dMx4.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    44125 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/haswell/3/sup/d6x8/bli_gemmsup_rd_haswell_asm_dMx8.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    66482 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/haswell/3/sup/d6x8/bli_gemmsup_rv_haswell_asm_dMx2.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    70571 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/haswell/3/sup/d6x8/bli_gemmsup_rv_haswell_asm_dMx4.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    84809 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/haswell/3/sup/d6x8/bli_gemmsup_rv_haswell_asm_dMx6.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    91255 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/haswell/3/sup/d6x8/bli_gemmsup_rv_haswell_asm_dMx8.c
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.866469 blis-0.9.1.dev1/blis/_src/kernels/haswell/3/sup/d6x8/old/
+-rw-r--r--   0 vsts      (1001) docker     (121)   123287 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/haswell/3/sup/d6x8/old/bli_gemmsup_rd_haswell_asm_d6x8.c
+-rw-r--r--   0 vsts      (1001) docker     (121)   304617 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/haswell/3/sup/d6x8/old/bli_gemmsup_rv_haswell_asm_d6x8.c
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.866469 blis-0.9.1.dev1/blis/_src/kernels/haswell/3/sup/old/
+-rw-r--r--   0 vsts      (1001) docker     (121)   141528 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/haswell/3/sup/old/bli_gemmsup_rd_haswell_asm_d6x8.c
+-rw-r--r--   0 vsts      (1001) docker     (121)   149744 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/haswell/3/sup/old/bli_gemmsup_rd_haswell_asm_d6x8m.c
+-rw-r--r--   0 vsts      (1001) docker     (121)   156805 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/haswell/3/sup/old/bli_gemmsup_rd_haswell_asm_d6x8n.c
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.870470 blis-0.9.1.dev1/blis/_src/kernels/haswell/3/sup/s6x16/
+-rw-r--r--   0 vsts      (1001) docker     (121)     7643 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/haswell/3/sup/s6x16/bli_gemmsup_r_haswell_ref_sMx1.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    46512 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/haswell/3/sup/s6x16/bli_gemmsup_rd_haswell_asm_sMx1.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    42106 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/haswell/3/sup/s6x16/bli_gemmsup_rd_haswell_asm_sMx12.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    45181 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/haswell/3/sup/s6x16/bli_gemmsup_rd_haswell_asm_sMx16.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    49994 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/haswell/3/sup/s6x16/bli_gemmsup_rd_haswell_asm_sMx2.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    39761 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/haswell/3/sup/s6x16/bli_gemmsup_rd_haswell_asm_sMx4.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    42097 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/haswell/3/sup/s6x16/bli_gemmsup_rd_haswell_asm_sMx8.c
+-rw-r--r--   0 vsts      (1001) docker     (121)   105003 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/haswell/3/sup/s6x16/bli_gemmsup_rv_haswell_asm_sMx12.c
+-rw-r--r--   0 vsts      (1001) docker     (121)   118893 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/haswell/3/sup/s6x16/bli_gemmsup_rv_haswell_asm_sMx16.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    68445 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/haswell/3/sup/s6x16/bli_gemmsup_rv_haswell_asm_sMx2.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    74065 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/haswell/3/sup/s6x16/bli_gemmsup_rv_haswell_asm_sMx4.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    96722 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/haswell/3/sup/s6x16/bli_gemmsup_rv_haswell_asm_sMx6.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    84611 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/haswell/3/sup/s6x16/bli_gemmsup_rv_haswell_asm_sMx8.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    12533 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/haswell/bli_kernels_haswell.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.870470 blis-0.9.1.dev1/blis/_src/kernels/knc/
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.870470 blis-0.9.1.dev1/blis/_src/kernels/knc/3/
+-rw-r--r--   0 vsts      (1001) docker     (121)    21055 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/knc/3/bli_dgemm_knc_asm_30x8.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    21252 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/knc/3/bli_sgemm_knc_asm_30x16.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     1771 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/knc/bli_kernels_knc.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.870470 blis-0.9.1.dev1/blis/_src/kernels/knl/
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.870470 blis-0.9.1.dev1/blis/_src/kernels/knl/1m/
+-rw-r--r--   0 vsts      (1001) docker     (121)    19685 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/knl/1m/bli_dpackm_knl_asm_24x8.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    20632 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/knl/1m/bli_spackm_knl_asm_24x16.c
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.870470 blis-0.9.1.dev1/blis/_src/kernels/knl/1m/old/
+-rw-r--r--   0 vsts      (1001) docker     (121)    15691 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/knl/1m/old/bli_packm_knl_asm_30x8.c
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.870470 blis-0.9.1.dev1/blis/_src/kernels/knl/3/
+-rw-r--r--   0 vsts      (1001) docker     (121)    19570 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/knl/3/bli_dgemm_knl_asm_24x8.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    19430 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/knl/3/bli_sgemm_knl_asm_24x16.c
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.870470 blis-0.9.1.dev1/blis/_src/kernels/knl/3/other/
+-rw-r--r--   0 vsts      (1001) docker     (121)    24893 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/knl/3/other/bli_dgemm_knl_asm_12x16.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    23763 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/knl/3/other/bli_dgemm_knl_asm_30x8.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    15936 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/knl/3/other/bli_dgemm_knl_asm_30x8_knc.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    22049 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/knl/3/other/bli_dgemm_knl_asm_8x24.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    16389 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/knl/3/other/bli_sgemm_knl_asm_30x16_knc.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2181 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/knl/bli_kernels_knl.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.710469 blis-0.9.1.dev1/blis/_src/kernels/old/
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.870470 blis-0.9.1.dev1/blis/_src/kernels/old/c99/
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.874470 blis-0.9.1.dev1/blis/_src/kernels/old/c99/3/
+-rw-r--r--   0 vsts      (1001) docker     (121)     6327 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/old/c99/3/bli_gemm_c99_4x4.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2808 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/old/c99/3/bli_gemmtrsm_l_c99_4x4.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2808 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/old/c99/3/bli_gemmtrsm_u_c99_4x4.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     5971 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/old/c99/3/bli_trsm_l_c99_4x4.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     6001 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/old/c99/3/bli_trsm_u_c99_4x4.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2374 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/old/c99/bli_kernels_c99.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.710469 blis-0.9.1.dev1/blis/_src/kernels/old/loongson3a/
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.874470 blis-0.9.1.dev1/blis/_src/kernels/old/loongson3a/3/
+-rw-r--r--   0 vsts      (1001) docker     (121)    23051 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/old/loongson3a/3/bli_gemm_loongson3a_opt_d4x4.c
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.710469 blis-0.9.1.dev1/blis/_src/kernels/old/nacl/
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.710469 blis-0.9.1.dev1/blis/_src/kernels/old/nacl/pnacl/
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.874470 blis-0.9.1.dev1/blis/_src/kernels/old/nacl/pnacl/1/
+-rw-r--r--   0 vsts      (1001) docker     (121)     4948 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/old/nacl/pnacl/1/bli_axpyv_opt.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    14220 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/old/nacl/pnacl/1/bli_dotv_opt.c
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.874470 blis-0.9.1.dev1/blis/_src/kernels/old/nacl/pnacl/3/
+-rw-r--r--   0 vsts      (1001) docker     (121)    14195 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/old/nacl/pnacl/3/bli_gemm_opt.c
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.710469 blis-0.9.1.dev1/blis/_src/kernels/old/x86/
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.874470 blis-0.9.1.dev1/blis/_src/kernels/old/x86/1m/
+-rw-r--r--   0 vsts      (1001) docker     (121)    10427 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/old/x86/1m/bli_packm_2xk.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2056 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/old/x86/1m/bli_packm_2xk.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    11378 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/old/x86/1m/bli_packm_4xk.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2056 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/old/x86/1m/bli_packm_4xk.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.874470 blis-0.9.1.dev1/blis/_src/kernels/old/x86/3/
+-rw-r--r--   0 vsts      (1001) docker     (121)    16862 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/old/x86/3/bli_gemm_opt_d2x4.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    15273 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/old/x86/3/bli_gemm_opt_d4x2.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    21386 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/old/x86/3/bli_gemmtrsm_l_opt_d4x2.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    21653 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/old/x86/3/bli_gemmtrsm_u_opt_d4x2.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     9615 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/old/x86/3/bli_trsm_l_opt_d4x2.c
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.874470 blis-0.9.1.dev1/blis/_src/kernels/penryn/
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.874470 blis-0.9.1.dev1/blis/_src/kernels/penryn/1/
+-rw-r--r--   0 vsts      (1001) docker     (121)     4536 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/penryn/1/bli_axpyv_penryn_int.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     3996 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/penryn/1/bli_dotv_penryn_int.c
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.874470 blis-0.9.1.dev1/blis/_src/kernels/penryn/1f/
+-rw-r--r--   0 vsts      (1001) docker     (121)     6872 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/penryn/1f/bli_axpy2v_penryn_int.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     6321 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/penryn/1f/bli_axpyf_penryn_int.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     5001 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/penryn/1f/bli_dotaxpyv_penryn_int.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     9544 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/penryn/1f/bli_dotxaxpyf_penryn_int.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     8405 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/penryn/1f/bli_dotxf_penryn_int.c
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.878470 blis-0.9.1.dev1/blis/_src/kernels/penryn/3/
+-rw-r--r--   0 vsts      (1001) docker     (121)    25693 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/penryn/3/bli_gemm_penryn_asm_d4x4.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    16554 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/penryn/3/bli_gemmtrsm_l_penryn_asm_d4x4.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    15801 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/penryn/3/bli_gemmtrsm_u_penryn_asm_d4x4.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     7998 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/penryn/3/bli_trsm_l_penryn_asm_d4x4.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     8020 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/penryn/3/bli_trsm_u_penryn_asm_d4x4.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2000 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/penryn/bli_kernels_penryn.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.878470 blis-0.9.1.dev1/blis/_src/kernels/piledriver/
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.878470 blis-0.9.1.dev1/blis/_src/kernels/piledriver/3/
+-rw-r--r--   0 vsts      (1001) docker     (121)    48133 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/piledriver/3/bli_gemm_piledriver_asm_d8x3.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     1910 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/piledriver/bli_kernels_piledriver.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.878470 blis-0.9.1.dev1/blis/_src/kernels/power10/
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.878470 blis-0.9.1.dev1/blis/_src/kernels/power10/3/
+-rw-r--r--   0 vsts      (1001) docker     (121)     6779 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/power10/3/bli_dgemm_power10_mma.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     4759 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/power10/3/bli_i16gemm_power10_mma.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     4787 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/power10/3/bli_i16sgemm_power10_mma.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     4757 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/power10/3/bli_i4gemm_power10_mma.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     4753 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/power10/3/bli_i8gemm_power10_mma.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     4749 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/power10/3/bli_sbgemm_power10_mma.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     5194 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/power10/3/bli_sgemm_power10_mma.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     4726 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/power10/3/bli_shgemm_power10_mma.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     3155 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/power10/3/vector_int_macros.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1786 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/power10/bli_kernels_power10.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.878470 blis-0.9.1.dev1/blis/_src/kernels/power7/
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.878470 blis-0.9.1.dev1/blis/_src/kernels/power7/3/
+-rw-r--r--   0 vsts      (1001) docker     (121)    21458 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/power7/3/bli_gemm_power7_int_8x4.c
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.878470 blis-0.9.1.dev1/blis/_src/kernels/power7/3/test/
+-rw-r--r--   0 vsts      (1001) docker     (121)    21458 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/power7/3/test/bli_gemm_power7_int_8x4.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     3308 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/power7/3/test/bli_gemm_power7_int_8x4.h
+-rw-r--r--   0 vsts      (1001) docker     (121)      573 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/power7/3/test/blis_utest.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     3687 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/power7/3/test/exp.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     1895 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/power7/bli_kernels_power7.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.878470 blis-0.9.1.dev1/blis/_src/kernels/power9/
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.878470 blis-0.9.1.dev1/blis/_src/kernels/power9/3/
+-rw-r--r--   0 vsts      (1001) docker     (121)     8280 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/power9/3/bli_gemm_power9_asm_d12x6.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    87665 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/power9/3/bli_pwr9_asm_macros_12x6.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1761 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/power9/bli_kernels_power9.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.878470 blis-0.9.1.dev1/blis/_src/kernels/sandybridge/
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.882470 blis-0.9.1.dev1/blis/_src/kernels/sandybridge/3/
+-rw-r--r--   0 vsts      (1001) docker     (121)    62718 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/sandybridge/3/bli_gemm_sandybridge_asm_d8x4.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    14538 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/sandybridge/3/bli_gemm_sandybridge_int_d8x4.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2155 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/sandybridge/bli_kernels_sandybridge.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.882470 blis-0.9.1.dev1/blis/_src/kernels/skx/
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.882470 blis-0.9.1.dev1/blis/_src/kernels/skx/3/
+-rw-r--r--   0 vsts      (1001) docker     (121)    15652 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/skx/3/bli_dgemm_skx_asm_16x12_l2.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    11565 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/skx/3/bli_dgemm_skx_asm_16x14.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    16591 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/skx/3/bli_sgemm_skx_asm_32x12_l2.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     1881 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/skx/bli_kernels_skx.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.882470 blis-0.9.1.dev1/blis/_src/kernels/zen/
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.882470 blis-0.9.1.dev1/blis/_src/kernels/zen/1/
+-rw-r--r--   0 vsts      (1001) docker     (121)    17207 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/zen/1/bli_amaxv_zen_int.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     8307 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/zen/1/bli_axpyv_zen_int.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    15587 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/zen/1/bli_axpyv_zen_int10.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    11667 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/zen/1/bli_copyv_zen_int.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     9123 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/zen/1/bli_dotv_zen_int.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    14192 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/zen/1/bli_dotv_zen_int10.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     9562 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/zen/1/bli_dotxv_zen_int.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     7363 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/zen/1/bli_scalv_zen_int.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    13541 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/zen/1/bli_scalv_zen_int10.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     7573 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/zen/1/bli_setv_zen_int.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    10830 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/zen/1/bli_swapv_zen_int8.c
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.882470 blis-0.9.1.dev1/blis/_src/kernels/zen/1f/
+-rw-r--r--   0 vsts      (1001) docker     (121)     9138 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/zen/1f/bli_axpyf_zen_int_4.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    38725 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/zen/1f/bli_axpyf_zen_int_5.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    13138 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/zen/1f/bli_axpyf_zen_int_8.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    26897 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/zen/1f/bli_dotxf_zen_int_8.c
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.886470 blis-0.9.1.dev1/blis/_src/kernels/zen/3/
+-rw-r--r--   0 vsts      (1001) docker     (121)   169097 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/zen/3/bli_gemm_small.c
+-rw-r--r--   0 vsts      (1001) docker     (121)   170034 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/zen/3/bli_gemmt_small.c
+-rw-r--r--   0 vsts      (1001) docker     (121)  1737390 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/zen/3/bli_trsm_small.c
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.710469 blis-0.9.1.dev1/blis/_src/kernels/zen/3/sup/
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.886470 blis-0.9.1.dev1/blis/_src/kernels/zen/3/sup/broken/
+-rw-r--r--   0 vsts      (1001) docker     (121)    69777 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/zen/3/sup/broken/bli_gemmsup_rv_zen_asm_c3x8.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    51585 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/zen/3/sup/broken/bli_gemmsup_rv_zen_asm_c3x8m.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    53325 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/zen/3/sup/broken/bli_gemmsup_rv_zen_asm_c3x8n.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    49441 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/zen/3/sup/broken/bli_gemmsup_rv_zen_asm_z3x4.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    36551 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/zen/3/sup/broken/bli_gemmsup_rv_zen_asm_z3x4m.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    39419 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/zen/3/sup/broken/bli_gemmsup_rv_zen_asm_z3x4n.c
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.890470 blis-0.9.1.dev1/blis/_src/kernels/zen/3/sup/other/
+-rw-r--r--   0 vsts      (1001) docker     (121)   106760 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/zen/3/sup/other/bli_gemmsup_rd_zen_asm_s6x16.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    66862 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/zen/3/sup/other/bli_gemmsup_rd_zen_asm_s6x16m.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    63138 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/zen/3/sup/other/bli_gemmsup_rd_zen_asm_s6x16n.c
+-rw-r--r--   0 vsts      (1001) docker     (121)   307015 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/zen/3/sup/other/bli_gemmsup_rv_zen_asm_s6x16.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    78025 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/zen/3/sup/other/bli_gemmsup_rv_zen_asm_s6x16m.c
+-rw-r--r--   0 vsts      (1001) docker     (121)   126101 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/zen/3/sup/other/bli_gemmsup_rv_zen_asm_s6x16n.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     8774 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/zen/bli_kernels_zen.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.890470 blis-0.9.1.dev1/blis/_src/kernels/zen2/
+-rw-r--r--   0 vsts      (1001) docker     (121)     1839 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/kernels/zen2/bli_kernels_zen2.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.898470 blis-0.9.1.dev1/blis/_src/make/
+-rw-r--r--   0 vsts      (1001) docker     (121)   136447 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/make/darwin-firestorm.jsonl
+-rw-r--r--   0 vsts      (1001) docker     (121)   114321 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/make/darwin-generic.jsonl
+-rw-r--r--   0 vsts      (1001) docker     (121)   419616 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/make/darwin-x86_64.jsonl
+-rw-r--r--   0 vsts      (1001) docker     (121)   319287 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/make/darwin-x86_64_no_skx.jsonl
+-rw-r--r--   0 vsts      (1001) docker     (121)   366357 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/make/darwin-x86_64_no_zen2.jsonl
+-rw-r--r--   0 vsts      (1001) docker     (121)   410978 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/make/darwin-x86_64_no_zen3.jsonl
+-rw-r--r--   0 vsts      (1001) docker     (121)   237677 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/make/linux-arm64.jsonl
+-rw-r--r--   0 vsts      (1001) docker     (121)   197598 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/make/linux-arm64_no_sve.jsonl
+-rw-r--r--   0 vsts      (1001) docker     (121)   115356 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/make/linux-generic.jsonl
+-rw-r--r--   0 vsts      (1001) docker     (121)   114356 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/make/linux-power9.jsonl
+-rw-r--r--   0 vsts      (1001) docker     (121)   414207 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/make/linux-x86_64.jsonl
+-rw-r--r--   0 vsts      (1001) docker     (121)   312099 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/make/linux-x86_64_no_skx.jsonl
+-rw-r--r--   0 vsts      (1001) docker     (121)   360983 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/make/linux-x86_64_no_zen2.jsonl
+-rw-r--r--   0 vsts      (1001) docker     (121)   405530 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/make/linux-x86_64_no_zen3.jsonl
+-rw-r--r--   0 vsts      (1001) docker     (121)   123566 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/make/windows-generic.jsonl
+-rw-r--r--   0 vsts      (1001) docker     (121)   403925 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/make/windows-x86_64.jsonl
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.898470 blis-0.9.1.dev1/blis/_src/ref_kernels/
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.898470 blis-0.9.1.dev1/blis/_src/ref_kernels/1/
+-rw-r--r--   0 vsts      (1001) docker     (121)     2855 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/ref_kernels/1/bli_addv_ref.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     5027 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/ref_kernels/1/bli_amaxv_ref.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     6312 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/ref_kernels/1/bli_axpbyv_ref.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     5265 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/ref_kernels/1/bli_axpyv_ref.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2764 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/ref_kernels/1/bli_copyv_ref.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     3317 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/ref_kernels/1/bli_dotv_ref.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     3644 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/ref_kernels/1/bli_dotxv_ref.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2281 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/ref_kernels/1/bli_invertv_ref.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     3694 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/ref_kernels/1/bli_scal2v_ref.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2972 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/ref_kernels/1/bli_scalv_ref.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2792 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/ref_kernels/1/bli_setv_ref.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2759 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/ref_kernels/1/bli_subv_ref.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     2355 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/ref_kernels/1/bli_swapv_ref.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     3618 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/ref_kernels/1/bli_xpbyv_ref.c
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.902470 blis-0.9.1.dev1/blis/_src/ref_kernels/1f/
+-rw-r--r--   0 vsts      (1001) docker     (121)     3945 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/ref_kernels/1f/bli_axpy2v_ref.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     4088 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/ref_kernels/1f/bli_axpyf_ref.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     4438 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/ref_kernels/1f/bli_dotaxpyv_ref.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     6038 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/ref_kernels/1f/bli_dotxaxpyf_ref.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     4582 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/ref_kernels/1f/bli_dotxf_ref.c
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.902470 blis-0.9.1.dev1/blis/_src/ref_kernels/1f/other/
+-rw-r--r--   0 vsts      (1001) docker     (121)     3519 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/ref_kernels/1f/other/bli_dotxaxpyf_ref_alt.c
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.902470 blis-0.9.1.dev1/blis/_src/ref_kernels/1m/
+-rw-r--r--   0 vsts      (1001) docker     (121)    95930 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/ref_kernels/1m/bli_packm_cxk_1er_ref.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    23874 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/ref_kernels/1m/bli_packm_cxk_bb_ref.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    55513 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/ref_kernels/1m/bli_packm_cxk_ref.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    31541 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/ref_kernels/1m/bli_unpackm_cxk_ref.c
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.902470 blis-0.9.1.dev1/blis/_src/ref_kernels/3/
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.902470 blis-0.9.1.dev1/blis/_src/ref_kernels/3/bb/
+-rw-r--r--   0 vsts      (1001) docker     (121)     4533 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/ref_kernels/3/bb/bli_gemmbb_ref.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     4733 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/ref_kernels/3/bb/bli_gemmtrsmbb_ref.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     7445 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/ref_kernels/3/bb/bli_trsmbb_ref.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     7493 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/ref_kernels/3/bli_gemm_ref.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    22803 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/ref_kernels/3/bli_gemmsup_ref.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     4590 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/ref_kernels/3/bli_gemmtrsm_ref.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     7457 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/ref_kernels/3/bli_trsm_ref.c
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.902470 blis-0.9.1.dev1/blis/_src/ref_kernels/3/old/
+-rw-r--r--   0 vsts      (1001) docker     (121)     5194 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/ref_kernels/3/old/bli_gemm_simd_ref.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    12471 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/ref_kernels/3/old/bli_gemm_unrl_ref.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     5672 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/ref_kernels/3/old/bli_trsm_simd_ref.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    26841 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/ref_kernels/bli_cntx_ref.c
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.902470 blis-0.9.1.dev1/blis/_src/ref_kernels/ind/
+-rw-r--r--   0 vsts      (1001) docker     (121)     8951 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/ref_kernels/ind/bli_gemm1m_ref.c
+-rw-r--r--   0 vsts      (1001) docker     (121)     9018 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/ref_kernels/ind/bli_gemmtrsm1m_ref.c
+-rw-r--r--   0 vsts      (1001) docker     (121)    17348 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/_src/ref_kernels/ind/bli_trsm1m_ref.c
+-rw-r--r--   0 vsts      (1001) docker     (121)      542 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/about.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2669 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/benchmark.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     3607 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/cy.pxd
+-rw-r--r--   0 vsts      (1001) docker     (121)    16918 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/cy.pyx
+-rw-r--r--   0 vsts      (1001) docker     (121)     7055 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/py.pyx
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.906470 blis-0.9.1.dev1/blis/tests/
+-rw-r--r--   0 vsts      (1001) docker     (121)        0 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/tests/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2577 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/tests/common.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1134 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/tests/test_dotv.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2493 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/blis/tests/test_gemm.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-08-01 16:04:04.714469 blis-0.9.1.dev1/blis.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (121)     7728 2022-08-01 16:04:04.000000 blis-0.9.1.dev1/blis.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (121)    67517 2022-08-01 16:04:04.000000 blis-0.9.1.dev1/blis.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)        1 2022-08-01 16:04:04.000000 blis-0.9.1.dev1/blis.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)       14 2022-08-01 16:04:04.000000 blis-0.9.1.dev1/blis.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)        5 2022-08-01 16:04:04.000000 blis-0.9.1.dev1/blis.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)      129 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (121)       38 2022-08-01 16:04:04.906470 blis-0.9.1.dev1/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (121)    13630 2022-08-01 16:03:51.000000 blis-0.9.1.dev1/setup.py
```

### Comparing `blis-0.9.1.dev0/LICENSE` & `blis-0.9.1.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/PKG-INFO` & `blis-0.9.1.dev1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blis
-Version: 0.9.1.dev0
+Version: 0.9.1.dev1
 Summary: The Blis BLAS-like linear algebra library, as a self-contained C-extension.
 Home-page: https://github.com/explosion/cython-blis
 Author: Explosion
 Author-email: contact@explosion.ai
 License: BSD
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: blis Version: 0.9.1.dev0 Summary: The Blis BLAS-
+Metadata-Version: 2.1 Name: blis Version: 0.9.1.dev1 Summary: The Blis BLAS-
 like linear algebra library, as a self-contained C-extension. Home-page: https:
 //github.com/explosion/cython-blis Author: Explosion Author-email:
 contact@explosion.ai License: BSD Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology Classifier: License ::
 OSI Approved :: BSD License Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X Classifier: Programming
```

### Comparing `blis-0.9.1.dev0/README.md` & `blis-0.9.1.dev1/README.md`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/config/a64fx/bli_a64fx_sector_cache.h` & `blis-0.9.1.dev1/blis/_src/config/a64fx/bli_a64fx_sector_cache.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/config/a64fx/bli_cntx_init_a64fx.c` & `blis-0.9.1.dev1/blis/_src/config/a64fx/bli_cntx_init_a64fx.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/config/a64fx/bli_family_a64fx.h` & `blis-0.9.1.dev1/blis/_src/config/a64fx/bli_family_a64fx.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/config/amd64/bli_family_amd64.h` & `blis-0.9.1.dev1/blis/_src/config/amd64/bli_family_amd64.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/config/amd64_legacy/bli_family_amd64_legacy.h` & `blis-0.9.1.dev1/blis/_src/config/amd64_legacy/bli_family_amd64_legacy.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/config/arm32/bli_family_arm32.h` & `blis-0.9.1.dev1/blis/_src/config/arm32/bli_family_arm32.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/config/arm64/bli_family_arm64.h` & `blis-0.9.1.dev1/blis/_src/config/arm64/bli_family_arm64.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/config/armsve/bli_cntx_init_armsve.c` & `blis-0.9.1.dev1/blis/_src/config/armsve/bli_cntx_init_armsve.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/config/armsve/bli_family_armsve.h` & `blis-0.9.1.dev1/blis/_src/config/armsve/bli_family_armsve.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/config/bgq/bli_cntx_init_bgq.c` & `blis-0.9.1.dev1/blis/_src/config/bgq/bli_cntx_init_bgq.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/config/bgq/bli_family_bgq.h` & `blis-0.9.1.dev1/blis/_src/config/bgq/bli_family_bgq.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/config/bulldozer/bli_cntx_init_bulldozer.c` & `blis-0.9.1.dev1/blis/_src/config/bulldozer/bli_cntx_init_bulldozer.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/config/bulldozer/bli_family_bulldozer.h` & `blis-0.9.1.dev1/blis/_src/config/bulldozer/bli_family_bulldozer.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/config/cortexa15/bli_cntx_init_cortexa15.c` & `blis-0.9.1.dev1/blis/_src/config/cortexa15/bli_cntx_init_cortexa15.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/config/cortexa15/bli_family_cortexa15.h` & `blis-0.9.1.dev1/blis/_src/config/cortexa15/bli_family_cortexa15.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/config/cortexa53/bli_cntx_init_cortexa53.c` & `blis-0.9.1.dev1/blis/_src/config/cortexa53/bli_cntx_init_cortexa53.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/config/cortexa53/bli_family_cortexa53.h` & `blis-0.9.1.dev1/blis/_src/config/cortexa53/bli_family_cortexa53.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/config/cortexa57/bli_cntx_init_cortexa57.c` & `blis-0.9.1.dev1/blis/_src/config/cortexa57/bli_cntx_init_cortexa57.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/config/cortexa57/bli_family_cortexa57.h` & `blis-0.9.1.dev1/blis/_src/config/cortexa57/bli_family_cortexa57.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/config/cortexa9/bli_cntx_init_cortexa9.c` & `blis-0.9.1.dev1/blis/_src/config/cortexa9/bli_cntx_init_cortexa9.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/config/cortexa9/bli_family_cortexa9.h` & `blis-0.9.1.dev1/blis/_src/config/cortexa9/bli_family_cortexa9.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/config/excavator/bli_cntx_init_excavator.c` & `blis-0.9.1.dev1/blis/_src/config/excavator/bli_cntx_init_excavator.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/config/excavator/bli_family_excavator.h` & `blis-0.9.1.dev1/blis/_src/config/excavator/bli_family_excavator.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/config/firestorm/bli_cntx_init_firestorm.c` & `blis-0.9.1.dev1/blis/_src/config/firestorm/bli_cntx_init_firestorm.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/config/firestorm/bli_family_firestorm.h` & `blis-0.9.1.dev1/blis/_src/config/firestorm/bli_family_firestorm.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/config/generic/bli_cntx_init_generic.c` & `blis-0.9.1.dev1/blis/_src/config/generic/bli_cntx_init_generic.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/config/generic/bli_family_generic.h` & `blis-0.9.1.dev1/blis/_src/config/generic/bli_family_generic.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/config/haswell/bli_cntx_init_haswell.c` & `blis-0.9.1.dev1/blis/_src/config/haswell/bli_cntx_init_haswell.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/config/haswell/bli_family_haswell.h` & `blis-0.9.1.dev1/blis/_src/config/haswell/bli_family_haswell.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/config/intel64/bli_family_intel64.h` & `blis-0.9.1.dev1/blis/_src/config/intel64/bli_family_intel64.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/config/intel64_no_skx/bli_family_intel64.h` & `blis-0.9.1.dev1/blis/_src/config/intel64_no_skx/bli_family_intel64.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/config/intel64_no_skx/bli_family_intel64_no_skx.h` & `blis-0.9.1.dev1/blis/_src/config/intel64_no_skx/bli_family_intel64_no_skx.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/config/knc/bli_cntx_init_knc.c` & `blis-0.9.1.dev1/blis/_src/config/knc/bli_cntx_init_knc.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/config/knc/bli_family_knc.h` & `blis-0.9.1.dev1/blis/_src/config/knc/bli_family_knc.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/config/knl/bli_cntx_init_knl.c` & `blis-0.9.1.dev1/blis/_src/config/knl/bli_cntx_init_knl.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/config/knl/bli_family_knl.h` & `blis-0.9.1.dev1/blis/_src/config/knl/bli_family_knl.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/config/old/armv7a/bli_cntx_init_armv7a.c` & `blis-0.9.1.dev1/blis/_src/config/old/armv7a/bli_cntx_init_armv7a.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/config/old/armv7a/bli_family_armv7a.h` & `blis-0.9.1.dev1/blis/_src/config/old/armv7a/bli_family_armv7a.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/config/old/emscripten/bli_kernel.h` & `blis-0.9.1.dev1/blis/_src/config/old/emscripten/bli_kernel.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/config/old/haswellbb/bli_cntx_init_haswell.c` & `blis-0.9.1.dev1/blis/_src/config/old/haswellbb/bli_cntx_init_haswell.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/config/old/haswellbb/bli_family_haswell.h` & `blis-0.9.1.dev1/blis/_src/config/old/haswellbb/bli_family_haswell.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/config/old/loongson3a/bli_kernel.h` & `blis-0.9.1.dev1/blis/_src/config/old/loongson3a/bli_kernel.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/config/old/newarch/bli_kernel.h` & `blis-0.9.1.dev1/blis/_src/config/old/newarch/bli_kernel.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/config/old/pnacl/bli_kernel.h` & `blis-0.9.1.dev1/blis/_src/config/old/pnacl/bli_kernel.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/config/penryn/bli_cntx_init_penryn.c` & `blis-0.9.1.dev1/blis/_src/config/penryn/bli_cntx_init_penryn.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/config/penryn/bli_family_penryn.h` & `blis-0.9.1.dev1/blis/_src/config/penryn/bli_family_penryn.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/config/piledriver/bli_cntx_init_piledriver.c` & `blis-0.9.1.dev1/blis/_src/config/piledriver/bli_cntx_init_piledriver.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/config/piledriver/bli_family_piledriver.h` & `blis-0.9.1.dev1/blis/_src/config/piledriver/bli_family_piledriver.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/config/power10/bli_cntx_init_power10.c` & `blis-0.9.1.dev1/blis/_src/config/power10/bli_cntx_init_power10.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/config/power10/bli_family_power10.h` & `blis-0.9.1.dev1/blis/_src/config/power10/bli_family_power10.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/config/power7/bli_cntx_init_power7.c` & `blis-0.9.1.dev1/blis/_src/config/power7/bli_cntx_init_power7.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/config/power7/bli_family_power7.h` & `blis-0.9.1.dev1/blis/_src/config/power7/bli_family_power7.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/config/power9/bli_cntx_init_power9.c` & `blis-0.9.1.dev1/blis/_src/config/power9/bli_cntx_init_power9.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/config/power9/bli_family_power9.h` & `blis-0.9.1.dev1/blis/_src/config/power9/bli_family_power9.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/config/sandybridge/bli_cntx_init_sandybridge.c` & `blis-0.9.1.dev1/blis/_src/config/sandybridge/bli_cntx_init_sandybridge.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/config/sandybridge/bli_family_sandybridge.h` & `blis-0.9.1.dev1/blis/_src/config/sandybridge/bli_family_sandybridge.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/config/skx/bli_cntx_init_skx.c` & `blis-0.9.1.dev1/blis/_src/config/skx/bli_cntx_init_skx.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/config/skx/bli_family_skx.h` & `blis-0.9.1.dev1/blis/_src/config/skx/bli_family_skx.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/config/steamroller/bli_cntx_init_steamroller.c` & `blis-0.9.1.dev1/blis/_src/config/steamroller/bli_cntx_init_steamroller.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/config/steamroller/bli_family_steamroller.h` & `blis-0.9.1.dev1/blis/_src/config/steamroller/bli_family_steamroller.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/config/template/bli_cntx_init_template.c` & `blis-0.9.1.dev1/blis/_src/config/template/bli_cntx_init_template.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/config/template/bli_family_template.h` & `blis-0.9.1.dev1/blis/_src/config/template/bli_family_template.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/config/template/kernels/1/bli_axpyv_template_noopt_var1.c` & `blis-0.9.1.dev1/blis/_src/config/template/kernels/1/bli_axpyv_template_noopt_var1.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/config/template/kernels/1/bli_dotv_template_noopt_var1.c` & `blis-0.9.1.dev1/blis/_src/config/template/kernels/1/bli_dotv_template_noopt_var1.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/config/template/kernels/1f/bli_axpy2v_template_noopt_var1.c` & `blis-0.9.1.dev1/blis/_src/config/template/kernels/1f/bli_axpy2v_template_noopt_var1.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/config/template/kernels/1f/bli_axpyf_template_noopt_var1.c` & `blis-0.9.1.dev1/blis/_src/config/template/kernels/1f/bli_axpyf_template_noopt_var1.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/config/template/kernels/1f/bli_dotaxpyv_template_noopt_var1.c` & `blis-0.9.1.dev1/blis/_src/config/template/kernels/1f/bli_dotaxpyv_template_noopt_var1.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/config/template/kernels/1f/bli_dotxaxpyf_template_noopt_var1.c` & `blis-0.9.1.dev1/blis/_src/config/template/kernels/1f/bli_dotxaxpyf_template_noopt_var1.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/config/template/kernels/1f/bli_dotxf_template_noopt_var1.c` & `blis-0.9.1.dev1/blis/_src/config/template/kernels/1f/bli_dotxf_template_noopt_var1.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/config/template/kernels/3/bli_gemm_template_noopt_mxn.c` & `blis-0.9.1.dev1/blis/_src/config/template/kernels/3/bli_gemm_template_noopt_mxn.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/config/template/kernels/3/bli_gemmtrsm_l_template_noopt_mxn.c` & `blis-0.9.1.dev1/blis/_src/config/template/kernels/3/bli_gemmtrsm_l_template_noopt_mxn.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/config/template/kernels/3/bli_gemmtrsm_u_template_noopt_mxn.c` & `blis-0.9.1.dev1/blis/_src/config/template/kernels/3/bli_gemmtrsm_u_template_noopt_mxn.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/config/template/kernels/3/bli_trsm_l_template_noopt_mxn.c` & `blis-0.9.1.dev1/blis/_src/config/template/kernels/3/bli_trsm_l_template_noopt_mxn.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/config/template/kernels/3/bli_trsm_u_template_noopt_mxn.c` & `blis-0.9.1.dev1/blis/_src/config/template/kernels/3/bli_trsm_u_template_noopt_mxn.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/config/thunderx2/bli_cntx_init_thunderx2.c` & `blis-0.9.1.dev1/blis/_src/config/thunderx2/bli_cntx_init_thunderx2.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/config/thunderx2/bli_family_thunderx2.h` & `blis-0.9.1.dev1/blis/_src/config/thunderx2/bli_family_thunderx2.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/config/x86_64/bli_family_x86_64.h` & `blis-0.9.1.dev1/blis/_src/config/x86_64/bli_family_x86_64.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/config/x86_64_no_skx/bli_family_x86_64_no_skx.h` & `blis-0.9.1.dev1/blis/_src/config/x86_64_no_skx/bli_family_x86_64_no_skx.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/config/x86_64_no_zen2/bli_family_x86_64_no_zen2.h` & `blis-0.9.1.dev1/blis/_src/config/x86_64_no_zen2/bli_family_x86_64_no_zen2.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/config/x86_64_no_zen3/bli_family_x86_64_no_zen3.h` & `blis-0.9.1.dev1/blis/_src/config/x86_64_no_zen3/bli_family_x86_64_no_zen3.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/config/zen/bli_cntx_init_zen.c` & `blis-0.9.1.dev1/blis/_src/config/zen/bli_cntx_init_zen.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/config/zen/bli_family_zen.h` & `blis-0.9.1.dev1/blis/_src/config/zen/bli_family_zen.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/config/zen/old/bli_kernel.h` & `blis-0.9.1.dev1/blis/_src/config/zen/old/bli_kernel.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/config/zen2/bli_cntx_init_zen2.c` & `blis-0.9.1.dev1/blis/_src/config/zen2/bli_cntx_init_zen2.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/config/zen2/bli_family_zen2.h` & `blis-0.9.1.dev1/blis/_src/config/zen2/bli_family_zen2.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/config/zen3/bli_cntx_init_zen3.c` & `blis-0.9.1.dev1/blis/_src/config/zen3/bli_cntx_init_zen3.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/config/zen3/bli_family_zen3.h` & `blis-0.9.1.dev1/blis/_src/config/zen3/bli_family_zen3.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/0/bli_l0.h` & `blis-0.9.1.dev1/blis/_src/frame/0/bli_l0.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/0/bli_l0_check.c` & `blis-0.9.1.dev1/blis/_src/frame/0/bli_l0_check.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/0/bli_l0_check.h` & `blis-0.9.1.dev1/blis/_src/frame/0/bli_l0_check.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/0/bli_l0_fpa.c` & `blis-0.9.1.dev1/blis/_src/frame/0/bli_l0_fpa.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/0/bli_l0_fpa.h` & `blis-0.9.1.dev1/blis/_src/frame/0/bli_l0_fpa.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/0/bli_l0_ft.h` & `blis-0.9.1.dev1/blis/_src/frame/0/bli_l0_ft.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/0/bli_l0_oapi.c` & `blis-0.9.1.dev1/blis/_src/frame/0/bli_l0_oapi.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/0/bli_l0_oapi.h` & `blis-0.9.1.dev1/blis/_src/frame/0/bli_l0_oapi.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/0/bli_l0_tapi.c` & `blis-0.9.1.dev1/blis/_src/frame/0/bli_l0_tapi.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/0/bli_l0_tapi.h` & `blis-0.9.1.dev1/blis/_src/frame/0/bli_l0_tapi.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/0/copysc/bli_copysc.c` & `blis-0.9.1.dev1/blis/_src/frame/0/copysc/bli_copysc.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/0/copysc/bli_copysc.h` & `blis-0.9.1.dev1/blis/_src/frame/0/copysc/bli_copysc.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/1/bli_l1v.h` & `blis-0.9.1.dev1/blis/_src/frame/1/bli_l1v.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/1/bli_l1v_check.c` & `blis-0.9.1.dev1/blis/_src/frame/1/bli_l1v_check.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/1/bli_l1v_check.h` & `blis-0.9.1.dev1/blis/_src/frame/1/bli_l1v_check.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/1/bli_l1v_fpa.c` & `blis-0.9.1.dev1/blis/_src/frame/1/bli_l1v_fpa.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/1/bli_l1v_fpa.h` & `blis-0.9.1.dev1/blis/_src/frame/1/bli_l1v_fpa.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/1/bli_l1v_ft.h` & `blis-0.9.1.dev1/blis/_src/frame/1/bli_l1v_ft.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/1/bli_l1v_ft_ker.h` & `blis-0.9.1.dev1/blis/_src/frame/1/bli_l1v_ft_ker.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/1/bli_l1v_ker.h` & `blis-0.9.1.dev1/blis/_src/frame/1/bli_l1v_ker.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/1/bli_l1v_ker_prot.h` & `blis-0.9.1.dev1/blis/_src/frame/1/bli_l1v_ker_prot.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/1/bli_l1v_oapi.c` & `blis-0.9.1.dev1/blis/_src/frame/1/bli_l1v_oapi.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/1/bli_l1v_oapi.h` & `blis-0.9.1.dev1/blis/_src/frame/1/bli_l1v_oapi.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/1/bli_l1v_oapi_ba.c` & `blis-0.9.1.dev1/blis/_src/frame/1/bli_l1v_oapi_ba.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/1/bli_l1v_oapi_ex.c` & `blis-0.9.1.dev1/blis/_src/frame/1/bli_l1v_oapi_ex.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/1/bli_l1v_tapi.c` & `blis-0.9.1.dev1/blis/_src/frame/1/bli_l1v_tapi.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/1/bli_l1v_tapi.h` & `blis-0.9.1.dev1/blis/_src/frame/1/bli_l1v_tapi.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/1/bli_l1v_tapi_ba.c` & `blis-0.9.1.dev1/blis/_src/frame/1/bli_l1v_tapi_ba.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/1/bli_l1v_tapi_ex.c` & `blis-0.9.1.dev1/blis/_src/frame/1/bli_l1v_tapi_ex.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/1/other/packv/bli_packv.c` & `blis-0.9.1.dev1/blis/_src/frame/1/other/packv/bli_packv.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/1/other/packv/bli_packv.h` & `blis-0.9.1.dev1/blis/_src/frame/1/other/packv/bli_packv.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/1/other/packv/bli_packv_check.c` & `blis-0.9.1.dev1/blis/_src/frame/1/other/packv/bli_packv_check.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/1/other/packv/bli_packv_check.h` & `blis-0.9.1.dev1/blis/_src/frame/1/other/packv/bli_packv_check.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/1/other/packv/bli_packv_cntl.c` & `blis-0.9.1.dev1/blis/_src/frame/1/other/packv/bli_packv_cntl.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/1/other/packv/bli_packv_cntl.h` & `blis-0.9.1.dev1/blis/_src/frame/1/other/packv/bli_packv_cntl.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/1/other/packv/bli_packv_init.c` & `blis-0.9.1.dev1/blis/_src/frame/1/other/packv/bli_packv_init.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/1/other/packv/bli_packv_init.h` & `blis-0.9.1.dev1/blis/_src/frame/1/other/packv/bli_packv_init.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/1/other/packv/bli_packv_int.c` & `blis-0.9.1.dev1/blis/_src/frame/1/other/packv/bli_packv_int.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/1/other/packv/bli_packv_int.h` & `blis-0.9.1.dev1/blis/_src/frame/1/other/packv/bli_packv_int.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/1/other/packv/bli_packv_unb_var1.c` & `blis-0.9.1.dev1/blis/_src/frame/1/other/packv/bli_packv_unb_var1.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/1/other/packv/bli_packv_unb_var1.h` & `blis-0.9.1.dev1/blis/_src/frame/1/other/packv/bli_packv_unb_var1.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/1/other/scalv/bli_scalv_cntl.c` & `blis-0.9.1.dev1/blis/_src/frame/1/other/scalv/bli_scalv_cntl.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/1/other/scalv/bli_scalv_cntl.h` & `blis-0.9.1.dev1/blis/_src/frame/1/other/scalv/bli_scalv_cntl.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/1/other/scalv/bli_scalv_int.c` & `blis-0.9.1.dev1/blis/_src/frame/1/other/scalv/bli_scalv_int.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/1/other/scalv/bli_scalv_int.h` & `blis-0.9.1.dev1/blis/_src/frame/1/other/scalv/bli_scalv_int.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/1/other/unpackv/bli_unpackv.c` & `blis-0.9.1.dev1/blis/_src/frame/1/other/unpackv/bli_unpackv.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/1/other/unpackv/bli_unpackv.h` & `blis-0.9.1.dev1/blis/_src/frame/1/other/unpackv/bli_unpackv.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/1/other/unpackv/bli_unpackv_check.c` & `blis-0.9.1.dev1/blis/_src/frame/1/other/unpackv/bli_unpackv_check.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/1/other/unpackv/bli_unpackv_check.h` & `blis-0.9.1.dev1/blis/_src/frame/1/other/unpackv/bli_unpackv_check.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/1/other/unpackv/bli_unpackv_cntl.c` & `blis-0.9.1.dev1/blis/_src/frame/1/other/unpackv/bli_unpackv_cntl.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/1/other/unpackv/bli_unpackv_cntl.h` & `blis-0.9.1.dev1/blis/_src/frame/1/other/unpackv/bli_unpackv_cntl.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/1/other/unpackv/bli_unpackv_int.c` & `blis-0.9.1.dev1/blis/_src/frame/1/other/unpackv/bli_unpackv_int.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/1/other/unpackv/bli_unpackv_int.h` & `blis-0.9.1.dev1/blis/_src/frame/1/other/unpackv/bli_unpackv_int.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/1/other/unpackv/bli_unpackv_unb_var1.c` & `blis-0.9.1.dev1/blis/_src/frame/1/other/unpackv/bli_unpackv_unb_var1.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/1/other/unpackv/bli_unpackv_unb_var1.h` & `blis-0.9.1.dev1/blis/_src/frame/1/other/unpackv/bli_unpackv_unb_var1.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/1d/bli_l1d.h` & `blis-0.9.1.dev1/blis/_src/frame/1d/bli_l1d.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/1d/bli_l1d_check.c` & `blis-0.9.1.dev1/blis/_src/frame/1d/bli_l1d_check.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/1d/bli_l1d_check.h` & `blis-0.9.1.dev1/blis/_src/frame/1d/bli_l1d_check.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/1d/bli_l1d_fpa.c` & `blis-0.9.1.dev1/blis/_src/frame/1d/bli_l1d_fpa.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/1d/bli_l1d_fpa.h` & `blis-0.9.1.dev1/blis/_src/frame/1d/bli_l1d_fpa.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/1d/bli_l1d_ft.h` & `blis-0.9.1.dev1/blis/_src/frame/1d/bli_l1d_ft.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/1d/bli_l1d_oapi.c` & `blis-0.9.1.dev1/blis/_src/frame/1d/bli_l1d_oapi.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/1d/bli_l1d_oapi.h` & `blis-0.9.1.dev1/blis/_src/frame/1d/bli_l1d_oapi.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/1d/bli_l1d_oapi_ba.c` & `blis-0.9.1.dev1/blis/_src/frame/1d/bli_l1d_oapi_ba.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/1d/bli_l1d_oapi_ex.c` & `blis-0.9.1.dev1/blis/_src/frame/1d/bli_l1d_oapi_ex.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/1d/bli_l1d_tapi.c` & `blis-0.9.1.dev1/blis/_src/frame/1d/bli_l1d_tapi.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/1d/bli_l1d_tapi.h` & `blis-0.9.1.dev1/blis/_src/frame/1d/bli_l1d_tapi.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/1d/bli_l1d_tapi_ba.c` & `blis-0.9.1.dev1/blis/_src/frame/1d/bli_l1d_tapi_ba.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/1d/bli_l1d_tapi_ex.c` & `blis-0.9.1.dev1/blis/_src/frame/1d/bli_l1d_tapi_ex.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/1f/bli_l1f.h` & `blis-0.9.1.dev1/blis/_src/frame/1f/bli_l1f.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/1f/bli_l1f_check.c` & `blis-0.9.1.dev1/blis/_src/frame/1f/bli_l1f_check.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/1f/bli_l1f_check.h` & `blis-0.9.1.dev1/blis/_src/frame/1f/bli_l1f_check.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/1f/bli_l1f_fpa.c` & `blis-0.9.1.dev1/blis/_src/frame/1f/bli_l1f_fpa.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/1f/bli_l1f_fpa.h` & `blis-0.9.1.dev1/blis/_src/frame/1f/bli_l1f_fpa.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/1f/bli_l1f_ft.h` & `blis-0.9.1.dev1/blis/_src/frame/1f/bli_l1f_ft.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/1f/bli_l1f_ft_ker.h` & `blis-0.9.1.dev1/blis/_src/frame/1f/bli_l1f_ft_ker.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/1f/bli_l1f_ker.h` & `blis-0.9.1.dev1/blis/_src/frame/1f/bli_l1f_ker.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/1f/bli_l1f_ker_prot.h` & `blis-0.9.1.dev1/blis/_src/frame/1f/bli_l1f_ker_prot.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/1f/bli_l1f_oapi.c` & `blis-0.9.1.dev1/blis/_src/frame/1f/bli_l1f_oapi.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/1f/bli_l1f_oapi.h` & `blis-0.9.1.dev1/blis/_src/frame/1f/bli_l1f_oapi.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/1f/bli_l1f_oapi_ba.c` & `blis-0.9.1.dev1/blis/_src/frame/1f/bli_l1f_oapi_ba.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/1f/bli_l1f_oapi_ex.c` & `blis-0.9.1.dev1/blis/_src/frame/1f/bli_l1f_oapi_ex.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/1f/bli_l1f_tapi.c` & `blis-0.9.1.dev1/blis/_src/frame/1f/bli_l1f_tapi.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/1f/bli_l1f_tapi.h` & `blis-0.9.1.dev1/blis/_src/frame/1f/bli_l1f_tapi.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/1f/bli_l1f_tapi_ba.c` & `blis-0.9.1.dev1/blis/_src/frame/1f/bli_l1f_tapi_ba.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/1f/bli_l1f_tapi_ex.c` & `blis-0.9.1.dev1/blis/_src/frame/1f/bli_l1f_tapi_ex.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/1m/bli_l1m.h` & `blis-0.9.1.dev1/blis/_src/frame/1m/bli_l1m.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/1m/bli_l1m_check.c` & `blis-0.9.1.dev1/blis/_src/frame/1m/bli_l1m_check.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/1m/bli_l1m_check.h` & `blis-0.9.1.dev1/blis/_src/frame/1m/bli_l1m_check.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/1m/bli_l1m_fpa.c` & `blis-0.9.1.dev1/blis/_src/frame/1m/bli_l1m_fpa.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/1m/bli_l1m_fpa.h` & `blis-0.9.1.dev1/blis/_src/frame/1m/bli_l1m_fpa.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/1m/bli_l1m_ft.h` & `blis-0.9.1.dev1/blis/_src/frame/1m/bli_l1m_ft.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/1m/bli_l1m_ft_ker.h` & `blis-0.9.1.dev1/blis/_src/frame/1m/bli_l1m_ft_ker.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/1m/bli_l1m_ker.h` & `blis-0.9.1.dev1/blis/_src/frame/1m/bli_l1m_ker.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/1m/bli_l1m_ker_prot.h` & `blis-0.9.1.dev1/blis/_src/frame/1m/bli_l1m_ker_prot.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/1m/bli_l1m_oapi.c` & `blis-0.9.1.dev1/blis/_src/frame/1m/bli_l1m_oapi.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/1m/bli_l1m_oapi.h` & `blis-0.9.1.dev1/blis/_src/frame/1m/bli_l1m_oapi.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/1m/bli_l1m_oapi_ba.c` & `blis-0.9.1.dev1/blis/_src/frame/1m/bli_l1m_oapi_ba.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/1m/bli_l1m_oapi_ex.c` & `blis-0.9.1.dev1/blis/_src/frame/1m/bli_l1m_oapi_ex.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/1m/bli_l1m_oft_var.h` & `blis-0.9.1.dev1/blis/_src/frame/1m/bli_l1m_oft_var.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/1m/bli_l1m_tapi.c` & `blis-0.9.1.dev1/blis/_src/frame/1m/bli_l1m_tapi.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/1m/bli_l1m_tapi.h` & `blis-0.9.1.dev1/blis/_src/frame/1m/bli_l1m_tapi.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/1m/bli_l1m_tapi_ba.c` & `blis-0.9.1.dev1/blis/_src/frame/1m/bli_l1m_tapi_ba.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/1m/bli_l1m_tapi_ex.c` & `blis-0.9.1.dev1/blis/_src/frame/1m/bli_l1m_tapi_ex.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/1m/bli_l1m_unb_var1.c` & `blis-0.9.1.dev1/blis/_src/frame/1m/bli_l1m_unb_var1.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/1m/bli_l1m_unb_var1.h` & `blis-0.9.1.dev1/blis/_src/frame/1m/bli_l1m_unb_var1.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/1m/other/bli_scalm.h` & `blis-0.9.1.dev1/blis/_src/frame/1m/other/bli_scalm.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/1m/other/bli_scalm_cntl.c` & `blis-0.9.1.dev1/blis/_src/frame/1m/other/bli_scalm_cntl.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/1m/other/bli_scalm_cntl.h` & `blis-0.9.1.dev1/blis/_src/frame/1m/other/bli_scalm_cntl.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/1m/other/bli_scalm_int.c` & `blis-0.9.1.dev1/blis/_src/frame/1m/other/bli_scalm_int.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/1m/other/bli_scalm_int.h` & `blis-0.9.1.dev1/blis/_src/frame/1m/other/bli_scalm_int.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/1m/packm/bli_packm.h` & `blis-0.9.1.dev1/blis/_src/frame/1m/packm/bli_packm.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/1m/packm/bli_packm_alloc.c` & `blis-0.9.1.dev1/blis/_src/frame/1m/packm/bli_packm_alloc.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/1m/packm/bli_packm_alloc.h` & `blis-0.9.1.dev1/blis/_src/frame/1m/packm/bli_packm_alloc.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/1m/packm/bli_packm_blk_var1.c` & `blis-0.9.1.dev1/blis/_src/frame/1m/packm/bli_packm_blk_var1.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/1m/packm/bli_packm_blk_var1.h` & `blis-0.9.1.dev1/blis/_src/frame/1m/packm/bli_packm_blk_var1.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/1m/packm/bli_packm_check.c` & `blis-0.9.1.dev1/blis/_src/frame/1m/packm/bli_packm_check.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/1m/packm/bli_packm_check.h` & `blis-0.9.1.dev1/blis/_src/frame/1m/packm/bli_packm_check.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/1m/packm/bli_packm_cntl.c` & `blis-0.9.1.dev1/blis/_src/frame/1m/packm/bli_packm_cntl.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/1m/packm/bli_packm_cntl.h` & `blis-0.9.1.dev1/blis/_src/frame/1m/packm/bli_packm_cntl.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/1m/packm/bli_packm_cxk.c` & `blis-0.9.1.dev1/blis/_src/frame/1m/packm/bli_packm_cxk.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/1m/packm/bli_packm_cxk.h` & `blis-0.9.1.dev1/blis/_src/frame/1m/packm/bli_packm_cxk.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/1m/packm/bli_packm_cxk_1er.c` & `blis-0.9.1.dev1/blis/_src/frame/1m/packm/bli_packm_cxk_1er.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/1m/packm/bli_packm_cxk_1er.h` & `blis-0.9.1.dev1/blis/_src/frame/1m/packm/bli_packm_cxk_1er.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/1m/packm/bli_packm_init.c` & `blis-0.9.1.dev1/blis/_src/frame/1m/packm/bli_packm_init.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/1m/packm/bli_packm_init.h` & `blis-0.9.1.dev1/blis/_src/frame/1m/packm/bli_packm_init.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/1m/packm/bli_packm_int.c` & `blis-0.9.1.dev1/blis/_src/frame/1m/packm/bli_packm_int.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/1m/packm/bli_packm_int.h` & `blis-0.9.1.dev1/blis/_src/frame/1m/packm/bli_packm_int.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/1m/packm/bli_packm_part.c` & `blis-0.9.1.dev1/blis/_src/frame/1m/packm/bli_packm_part.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/1m/packm/bli_packm_part.h` & `blis-0.9.1.dev1/blis/_src/frame/1m/packm/bli_packm_part.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/1m/packm/bli_packm_scalar.c` & `blis-0.9.1.dev1/blis/_src/frame/1m/packm/bli_packm_scalar.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/1m/packm/bli_packm_scalar.h` & `blis-0.9.1.dev1/blis/_src/frame/1m/packm/bli_packm_scalar.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/1m/packm/bli_packm_struc_cxk.c` & `blis-0.9.1.dev1/blis/_src/frame/1m/packm/bli_packm_struc_cxk.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/1m/packm/bli_packm_struc_cxk.h` & `blis-0.9.1.dev1/blis/_src/frame/1m/packm/bli_packm_struc_cxk.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/1m/packm/bli_packm_struc_cxk_1er.c` & `blis-0.9.1.dev1/blis/_src/frame/1m/packm/bli_packm_struc_cxk_1er.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/1m/packm/bli_packm_struc_cxk_1er.h` & `blis-0.9.1.dev1/blis/_src/frame/1m/packm/bli_packm_struc_cxk_1er.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/1m/packm/bli_packm_struc_cxk_md.c` & `blis-0.9.1.dev1/blis/_src/frame/1m/packm/bli_packm_struc_cxk_md.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/1m/packm/bli_packm_struc_cxk_md.h` & `blis-0.9.1.dev1/blis/_src/frame/1m/packm/bli_packm_struc_cxk_md.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/1m/packm/bli_packm_thrinfo.c` & `blis-0.9.1.dev1/blis/_src/frame/1m/packm/bli_packm_thrinfo.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/1m/packm/bli_packm_thrinfo.h` & `blis-0.9.1.dev1/blis/_src/frame/1m/packm/bli_packm_thrinfo.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/1m/unpackm/bli_unpackm.h` & `blis-0.9.1.dev1/blis/_src/frame/1m/unpackm/bli_unpackm.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/1m/unpackm/bli_unpackm_blk_var1.c` & `blis-0.9.1.dev1/blis/_src/frame/1m/unpackm/bli_unpackm_blk_var1.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/1m/unpackm/bli_unpackm_blk_var1.h` & `blis-0.9.1.dev1/blis/_src/frame/1m/unpackm/bli_unpackm_blk_var1.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/1m/unpackm/bli_unpackm_check.c` & `blis-0.9.1.dev1/blis/_src/frame/1m/unpackm/bli_unpackm_check.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/1m/unpackm/bli_unpackm_check.h` & `blis-0.9.1.dev1/blis/_src/frame/1m/unpackm/bli_unpackm_check.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/1m/unpackm/bli_unpackm_cntl.c` & `blis-0.9.1.dev1/blis/_src/frame/1m/unpackm/bli_unpackm_cntl.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/1m/unpackm/bli_unpackm_cntl.h` & `blis-0.9.1.dev1/blis/_src/frame/1m/unpackm/bli_unpackm_cntl.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/1m/unpackm/bli_unpackm_cxk.c` & `blis-0.9.1.dev1/blis/_src/frame/1m/unpackm/bli_unpackm_cxk.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/1m/unpackm/bli_unpackm_cxk.h` & `blis-0.9.1.dev1/blis/_src/frame/1m/unpackm/bli_unpackm_cxk.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/1m/unpackm/bli_unpackm_int.c` & `blis-0.9.1.dev1/blis/_src/frame/1m/unpackm/bli_unpackm_int.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/1m/unpackm/bli_unpackm_int.h` & `blis-0.9.1.dev1/blis/_src/frame/1m/unpackm/bli_unpackm_int.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/2/bli_l2.h` & `blis-0.9.1.dev1/blis/_src/frame/2/bli_l2.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/2/bli_l2_check.c` & `blis-0.9.1.dev1/blis/_src/frame/2/bli_l2_check.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/2/bli_l2_check.h` & `blis-0.9.1.dev1/blis/_src/frame/2/bli_l2_check.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/2/bli_l2_fpa.c` & `blis-0.9.1.dev1/blis/_src/frame/2/bli_l2_fpa.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/2/bli_l2_fpa.h` & `blis-0.9.1.dev1/blis/_src/frame/2/bli_l2_fpa.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/2/bli_l2_ft.h` & `blis-0.9.1.dev1/blis/_src/frame/2/bli_l2_ft.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/2/bli_l2_ft_unb.h` & `blis-0.9.1.dev1/blis/_src/frame/2/bli_l2_ft_unb.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/2/bli_l2_oapi.c` & `blis-0.9.1.dev1/blis/_src/frame/2/bli_l2_oapi.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/2/bli_l2_oapi.h` & `blis-0.9.1.dev1/blis/_src/frame/2/bli_l2_oapi.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/2/bli_l2_oapi_ba.c` & `blis-0.9.1.dev1/blis/_src/frame/2/bli_l2_oapi_ba.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/2/bli_l2_oapi_ex.c` & `blis-0.9.1.dev1/blis/_src/frame/2/bli_l2_oapi_ex.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/2/bli_l2_tapi.c` & `blis-0.9.1.dev1/blis/_src/frame/2/bli_l2_tapi.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/2/bli_l2_tapi.h` & `blis-0.9.1.dev1/blis/_src/frame/2/bli_l2_tapi.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/2/bli_l2_tapi_ba.c` & `blis-0.9.1.dev1/blis/_src/frame/2/bli_l2_tapi_ba.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/2/bli_l2_tapi_ex.c` & `blis-0.9.1.dev1/blis/_src/frame/2/bli_l2_tapi_ex.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/2/gemv/amd/bli_gemv_unf_var2_amd.c` & `blis-0.9.1.dev1/blis/_src/frame/2/gemv/amd/bli_gemv_unf_var2_amd.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/2/gemv/bli_gemv.h` & `blis-0.9.1.dev1/blis/_src/frame/2/gemv/bli_gemv.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/2/gemv/bli_gemv_unb_var1.c` & `blis-0.9.1.dev1/blis/_src/frame/2/gemv/bli_gemv_unb_var1.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/2/gemv/bli_gemv_unb_var2.c` & `blis-0.9.1.dev1/blis/_src/frame/2/gemv/bli_gemv_unb_var2.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/2/gemv/bli_gemv_unf_var1.c` & `blis-0.9.1.dev1/blis/_src/frame/2/gemv/bli_gemv_unf_var1.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/2/gemv/bli_gemv_unf_var2.c` & `blis-0.9.1.dev1/blis/_src/frame/2/gemv/bli_gemv_unf_var2.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/2/gemv/bli_gemv_var.h` & `blis-0.9.1.dev1/blis/_src/frame/2/gemv/bli_gemv_var.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/2/gemv/bli_gemv_var_oapi.c` & `blis-0.9.1.dev1/blis/_src/frame/2/gemv/bli_gemv_var_oapi.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/2/gemv/other/bli_gemv_blk_var1.c` & `blis-0.9.1.dev1/blis/_src/frame/2/gemv/other/bli_gemv_blk_var1.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/2/gemv/other/bli_gemv_blk_var2.c` & `blis-0.9.1.dev1/blis/_src/frame/2/gemv/other/bli_gemv_blk_var2.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/2/gemv/other/bli_gemv_cntl.c` & `blis-0.9.1.dev1/blis/_src/frame/2/gemv/other/bli_gemv_cntl.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/2/gemv/other/bli_gemv_cntl.h` & `blis-0.9.1.dev1/blis/_src/frame/2/gemv/other/bli_gemv_cntl.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/2/gemv/other/bli_gemv_front.c` & `blis-0.9.1.dev1/blis/_src/frame/2/gemv/other/bli_gemv_front.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/2/gemv/other/bli_gemv_front.h` & `blis-0.9.1.dev1/blis/_src/frame/2/gemv/other/bli_gemv_front.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/2/gemv/other/bli_gemv_int.c` & `blis-0.9.1.dev1/blis/_src/frame/2/gemv/other/bli_gemv_int.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/2/gemv/other/bli_gemv_int.h` & `blis-0.9.1.dev1/blis/_src/frame/2/gemv/other/bli_gemv_int.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/2/ger/bli_ger.h` & `blis-0.9.1.dev1/blis/_src/frame/2/ger/bli_ger.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/2/ger/bli_ger_unb_var1.c` & `blis-0.9.1.dev1/blis/_src/frame/2/ger/bli_ger_unb_var1.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/2/ger/bli_ger_unb_var2.c` & `blis-0.9.1.dev1/blis/_src/frame/2/ger/bli_ger_unb_var2.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/2/ger/bli_ger_var.h` & `blis-0.9.1.dev1/blis/_src/frame/2/ger/bli_ger_var.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/2/ger/bli_ger_var_oapi.c` & `blis-0.9.1.dev1/blis/_src/frame/2/ger/bli_ger_var_oapi.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/2/ger/other/bli_ger_blk_var1.c` & `blis-0.9.1.dev1/blis/_src/frame/2/ger/other/bli_ger_blk_var1.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/2/ger/other/bli_ger_blk_var2.c` & `blis-0.9.1.dev1/blis/_src/frame/2/ger/other/bli_ger_blk_var2.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/2/ger/other/bli_ger_cntl.c` & `blis-0.9.1.dev1/blis/_src/frame/2/ger/other/bli_ger_cntl.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/2/ger/other/bli_ger_cntl.h` & `blis-0.9.1.dev1/blis/_src/frame/2/ger/other/bli_ger_cntl.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/2/ger/other/bli_ger_front.c` & `blis-0.9.1.dev1/blis/_src/frame/2/ger/other/bli_ger_front.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/2/ger/other/bli_ger_front.h` & `blis-0.9.1.dev1/blis/_src/frame/2/ger/other/bli_ger_front.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/2/ger/other/bli_ger_int.c` & `blis-0.9.1.dev1/blis/_src/frame/2/ger/other/bli_ger_int.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/2/ger/other/bli_ger_int.h` & `blis-0.9.1.dev1/blis/_src/frame/2/ger/other/bli_ger_int.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/2/hemv/bli_hemv.h` & `blis-0.9.1.dev1/blis/_src/frame/2/hemv/bli_hemv.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/2/hemv/bli_hemv_unb_var1.c` & `blis-0.9.1.dev1/blis/_src/frame/2/hemv/bli_hemv_unb_var1.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/2/hemv/bli_hemv_unb_var2.c` & `blis-0.9.1.dev1/blis/_src/frame/2/hemv/bli_hemv_unb_var2.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/2/hemv/bli_hemv_unb_var3.c` & `blis-0.9.1.dev1/blis/_src/frame/2/hemv/bli_hemv_unb_var3.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/2/hemv/bli_hemv_unb_var4.c` & `blis-0.9.1.dev1/blis/_src/frame/2/hemv/bli_hemv_unb_var4.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/2/hemv/bli_hemv_unf_var1.c` & `blis-0.9.1.dev1/blis/_src/frame/2/hemv/bli_hemv_unf_var1.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/2/hemv/bli_hemv_unf_var1a.c` & `blis-0.9.1.dev1/blis/_src/frame/2/hemv/bli_hemv_unf_var1a.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/2/hemv/bli_hemv_unf_var3.c` & `blis-0.9.1.dev1/blis/_src/frame/2/hemv/bli_hemv_unf_var3.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/2/hemv/bli_hemv_unf_var3a.c` & `blis-0.9.1.dev1/blis/_src/frame/2/hemv/bli_hemv_unf_var3a.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/2/hemv/bli_hemv_var.h` & `blis-0.9.1.dev1/blis/_src/frame/2/hemv/bli_hemv_var.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/2/hemv/bli_hemv_var_oapi.c` & `blis-0.9.1.dev1/blis/_src/frame/2/hemv/bli_hemv_var_oapi.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/2/hemv/other/bli_hemv_blk_var1.c` & `blis-0.9.1.dev1/blis/_src/frame/2/hemv/other/bli_hemv_blk_var1.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/2/hemv/other/bli_hemv_blk_var2.c` & `blis-0.9.1.dev1/blis/_src/frame/2/hemv/other/bli_hemv_blk_var2.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/2/hemv/other/bli_hemv_blk_var3.c` & `blis-0.9.1.dev1/blis/_src/frame/2/hemv/other/bli_hemv_blk_var3.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/2/hemv/other/bli_hemv_blk_var4.c` & `blis-0.9.1.dev1/blis/_src/frame/2/hemv/other/bli_hemv_blk_var4.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/2/hemv/other/bli_hemv_cntl.c` & `blis-0.9.1.dev1/blis/_src/frame/2/hemv/other/bli_hemv_cntl.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/2/hemv/other/bli_hemv_cntl.h` & `blis-0.9.1.dev1/blis/_src/frame/2/hemv/other/bli_hemv_cntl.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/2/hemv/other/bli_hemv_front.c` & `blis-0.9.1.dev1/blis/_src/frame/2/hemv/other/bli_hemv_front.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/2/hemv/other/bli_hemv_front.h` & `blis-0.9.1.dev1/blis/_src/frame/2/hemv/other/bli_hemv_front.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/2/hemv/other/bli_hemv_int.c` & `blis-0.9.1.dev1/blis/_src/frame/2/hemv/other/bli_hemv_int.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/2/hemv/other/bli_hemv_int.h` & `blis-0.9.1.dev1/blis/_src/frame/2/hemv/other/bli_hemv_int.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/2/her/bli_her.h` & `blis-0.9.1.dev1/blis/_src/frame/2/her/bli_her.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/2/her/bli_her_unb_var1.c` & `blis-0.9.1.dev1/blis/_src/frame/2/her/bli_her_unb_var1.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/2/her/bli_her_unb_var2.c` & `blis-0.9.1.dev1/blis/_src/frame/2/her/bli_her_unb_var2.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/2/her/bli_her_var.h` & `blis-0.9.1.dev1/blis/_src/frame/2/her/bli_her_var.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/2/her/bli_her_var_oapi.c` & `blis-0.9.1.dev1/blis/_src/frame/2/her/bli_her_var_oapi.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/2/her/other/bli_her_blk_var1.c` & `blis-0.9.1.dev1/blis/_src/frame/2/her/other/bli_her_blk_var1.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/2/her/other/bli_her_blk_var2.c` & `blis-0.9.1.dev1/blis/_src/frame/2/her/other/bli_her_blk_var2.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/2/her/other/bli_her_cntl.c` & `blis-0.9.1.dev1/blis/_src/frame/2/her/other/bli_her_cntl.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/2/her/other/bli_her_cntl.h` & `blis-0.9.1.dev1/blis/_src/frame/2/her/other/bli_her_cntl.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/2/her/other/bli_her_front.c` & `blis-0.9.1.dev1/blis/_src/frame/2/her/other/bli_her_front.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/2/her/other/bli_her_front.h` & `blis-0.9.1.dev1/blis/_src/frame/2/her/other/bli_her_front.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/2/her/other/bli_her_int.c` & `blis-0.9.1.dev1/blis/_src/frame/2/her/other/bli_her_int.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/2/her/other/bli_her_int.h` & `blis-0.9.1.dev1/blis/_src/frame/2/her/other/bli_her_int.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/2/her2/bli_her2.h` & `blis-0.9.1.dev1/blis/_src/frame/2/her2/bli_her2.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/2/her2/bli_her2_unb_var1.c` & `blis-0.9.1.dev1/blis/_src/frame/2/her2/bli_her2_unb_var1.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/2/her2/bli_her2_unb_var2.c` & `blis-0.9.1.dev1/blis/_src/frame/2/her2/bli_her2_unb_var2.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/2/her2/bli_her2_unb_var3.c` & `blis-0.9.1.dev1/blis/_src/frame/2/her2/bli_her2_unb_var3.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/2/her2/bli_her2_unb_var4.c` & `blis-0.9.1.dev1/blis/_src/frame/2/her2/bli_her2_unb_var4.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/2/her2/bli_her2_unf_var1.c` & `blis-0.9.1.dev1/blis/_src/frame/2/her2/bli_her2_unf_var1.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/2/her2/bli_her2_unf_var4.c` & `blis-0.9.1.dev1/blis/_src/frame/2/her2/bli_her2_unf_var4.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/2/her2/bli_her2_var.h` & `blis-0.9.1.dev1/blis/_src/frame/2/her2/bli_her2_var.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/2/her2/bli_her2_var_oapi.c` & `blis-0.9.1.dev1/blis/_src/frame/2/her2/bli_her2_var_oapi.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/2/her2/other/bli_her2_blk_var1.c` & `blis-0.9.1.dev1/blis/_src/frame/2/her2/other/bli_her2_blk_var1.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/2/her2/other/bli_her2_blk_var2.c` & `blis-0.9.1.dev1/blis/_src/frame/2/her2/other/bli_her2_blk_var2.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/2/her2/other/bli_her2_blk_var3.c` & `blis-0.9.1.dev1/blis/_src/frame/2/her2/other/bli_her2_blk_var3.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/2/her2/other/bli_her2_blk_var4.c` & `blis-0.9.1.dev1/blis/_src/frame/2/her2/other/bli_her2_blk_var4.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/2/her2/other/bli_her2_cntl.c` & `blis-0.9.1.dev1/blis/_src/frame/2/her2/other/bli_her2_cntl.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/2/her2/other/bli_her2_cntl.h` & `blis-0.9.1.dev1/blis/_src/frame/2/her2/other/bli_her2_cntl.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/2/her2/other/bli_her2_front.c` & `blis-0.9.1.dev1/blis/_src/frame/2/her2/other/bli_her2_front.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/2/her2/other/bli_her2_front.h` & `blis-0.9.1.dev1/blis/_src/frame/2/her2/other/bli_her2_front.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/2/her2/other/bli_her2_int.c` & `blis-0.9.1.dev1/blis/_src/frame/2/her2/other/bli_her2_int.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/2/her2/other/bli_her2_int.h` & `blis-0.9.1.dev1/blis/_src/frame/2/her2/other/bli_her2_int.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/2/symv/bli_symv.h` & `blis-0.9.1.dev1/blis/_src/frame/2/symv/bli_symv.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/2/symv/other/bli_symv_front.c` & `blis-0.9.1.dev1/blis/_src/frame/2/symv/other/bli_symv_front.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/2/symv/other/bli_symv_front.h` & `blis-0.9.1.dev1/blis/_src/frame/2/symv/other/bli_symv_front.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/2/syr/bli_syr.h` & `blis-0.9.1.dev1/blis/_src/frame/2/syr/bli_syr.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/2/syr/other/bli_syr_front.c` & `blis-0.9.1.dev1/blis/_src/frame/2/syr/other/bli_syr_front.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/2/syr/other/bli_syr_front.h` & `blis-0.9.1.dev1/blis/_src/frame/2/syr/other/bli_syr_front.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/2/syr2/bli_syr2.h` & `blis-0.9.1.dev1/blis/_src/frame/2/syr2/bli_syr2.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/2/syr2/other/bli_syr2_front.c` & `blis-0.9.1.dev1/blis/_src/frame/2/syr2/other/bli_syr2_front.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/2/syr2/other/bli_syr2_front.h` & `blis-0.9.1.dev1/blis/_src/frame/2/syr2/other/bli_syr2_front.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/2/trmv/bli_trmv.h` & `blis-0.9.1.dev1/blis/_src/frame/2/trmv/bli_trmv.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/2/trmv/bli_trmv_unb_var1.c` & `blis-0.9.1.dev1/blis/_src/frame/2/trmv/bli_trmv_unb_var1.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/2/trmv/bli_trmv_unb_var2.c` & `blis-0.9.1.dev1/blis/_src/frame/2/trmv/bli_trmv_unb_var2.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/2/trmv/bli_trmv_unf_var1.c` & `blis-0.9.1.dev1/blis/_src/frame/2/trmv/bli_trmv_unf_var1.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/2/trmv/bli_trmv_unf_var2.c` & `blis-0.9.1.dev1/blis/_src/frame/2/trmv/bli_trmv_unf_var2.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/2/trmv/bli_trmv_var.h` & `blis-0.9.1.dev1/blis/_src/frame/2/trmv/bli_trmv_var.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/2/trmv/bli_trmv_var_oapi.c` & `blis-0.9.1.dev1/blis/_src/frame/2/trmv/bli_trmv_var_oapi.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/2/trmv/other/bli_trmv_cntl.c` & `blis-0.9.1.dev1/blis/_src/frame/2/trmv/other/bli_trmv_cntl.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/2/trmv/other/bli_trmv_cntl.h` & `blis-0.9.1.dev1/blis/_src/frame/2/trmv/other/bli_trmv_cntl.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/2/trmv/other/bli_trmv_front.c` & `blis-0.9.1.dev1/blis/_src/frame/2/trmv/other/bli_trmv_front.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/2/trmv/other/bli_trmv_front.h` & `blis-0.9.1.dev1/blis/_src/frame/2/trmv/other/bli_trmv_front.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/2/trmv/other/bli_trmv_int.c` & `blis-0.9.1.dev1/blis/_src/frame/2/trmv/other/bli_trmv_int.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/2/trmv/other/bli_trmv_int.h` & `blis-0.9.1.dev1/blis/_src/frame/2/trmv/other/bli_trmv_int.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/2/trmv/other/bli_trmv_l_blk_var1.c` & `blis-0.9.1.dev1/blis/_src/frame/2/trmv/other/bli_trmv_l_blk_var1.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/2/trmv/other/bli_trmv_l_blk_var2.c` & `blis-0.9.1.dev1/blis/_src/frame/2/trmv/other/bli_trmv_l_blk_var2.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/2/trmv/other/bli_trmv_u_blk_var1.c` & `blis-0.9.1.dev1/blis/_src/frame/2/trmv/other/bli_trmv_u_blk_var1.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/2/trmv/other/bli_trmv_u_blk_var2.c` & `blis-0.9.1.dev1/blis/_src/frame/2/trmv/other/bli_trmv_u_blk_var2.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/2/trsv/bli_trsv.h` & `blis-0.9.1.dev1/blis/_src/frame/2/trsv/bli_trsv.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/2/trsv/bli_trsv_unb_var1.c` & `blis-0.9.1.dev1/blis/_src/frame/2/trsv/bli_trsv_unb_var1.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/2/trsv/bli_trsv_unb_var2.c` & `blis-0.9.1.dev1/blis/_src/frame/2/trsv/bli_trsv_unb_var2.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/2/trsv/bli_trsv_unf_var1.c` & `blis-0.9.1.dev1/blis/_src/frame/2/trsv/bli_trsv_unf_var1.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/2/trsv/bli_trsv_unf_var2.c` & `blis-0.9.1.dev1/blis/_src/frame/2/trsv/bli_trsv_unf_var2.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/2/trsv/bli_trsv_var.h` & `blis-0.9.1.dev1/blis/_src/frame/2/trsv/bli_trsv_var.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/2/trsv/bli_trsv_var_oapi.c` & `blis-0.9.1.dev1/blis/_src/frame/2/trsv/bli_trsv_var_oapi.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/2/trsv/other/bli_trsv_cntl.c` & `blis-0.9.1.dev1/blis/_src/frame/2/trsv/other/bli_trsv_cntl.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/2/trsv/other/bli_trsv_cntl.h` & `blis-0.9.1.dev1/blis/_src/frame/2/trsv/other/bli_trsv_cntl.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/2/trsv/other/bli_trsv_front.c` & `blis-0.9.1.dev1/blis/_src/frame/2/trsv/other/bli_trsv_front.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/2/trsv/other/bli_trsv_front.h` & `blis-0.9.1.dev1/blis/_src/frame/2/trsv/other/bli_trsv_front.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/2/trsv/other/bli_trsv_int.c` & `blis-0.9.1.dev1/blis/_src/frame/2/trsv/other/bli_trsv_int.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/2/trsv/other/bli_trsv_int.h` & `blis-0.9.1.dev1/blis/_src/frame/2/trsv/other/bli_trsv_int.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/2/trsv/other/bli_trsv_l_blk_var1.c` & `blis-0.9.1.dev1/blis/_src/frame/2/trsv/other/bli_trsv_l_blk_var1.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/2/trsv/other/bli_trsv_l_blk_var2.c` & `blis-0.9.1.dev1/blis/_src/frame/2/trsv/other/bli_trsv_l_blk_var2.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/2/trsv/other/bli_trsv_u_blk_var1.c` & `blis-0.9.1.dev1/blis/_src/frame/2/trsv/other/bli_trsv_u_blk_var1.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/2/trsv/other/bli_trsv_u_blk_var2.c` & `blis-0.9.1.dev1/blis/_src/frame/2/trsv/other/bli_trsv_u_blk_var2.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/3/bli_l3.h` & `blis-0.9.1.dev1/blis/_src/frame/3/bli_l3.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/3/bli_l3_blocksize.c` & `blis-0.9.1.dev1/blis/_src/frame/3/bli_l3_blocksize.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/3/bli_l3_blocksize.h` & `blis-0.9.1.dev1/blis/_src/frame/3/bli_l3_blocksize.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/3/bli_l3_check.c` & `blis-0.9.1.dev1/blis/_src/frame/3/bli_l3_check.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/3/bli_l3_check.h` & `blis-0.9.1.dev1/blis/_src/frame/3/bli_l3_check.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/3/bli_l3_cntl.c` & `blis-0.9.1.dev1/blis/_src/frame/3/bli_l3_cntl.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/3/bli_l3_cntl.h` & `blis-0.9.1.dev1/blis/_src/frame/3/bli_l3_cntl.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/3/bli_l3_direct.c` & `blis-0.9.1.dev1/blis/_src/frame/3/bli_l3_direct.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/3/bli_l3_direct.h` & `blis-0.9.1.dev1/blis/_src/frame/3/bli_l3_direct.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/3/bli_l3_ft_ukr.h` & `blis-0.9.1.dev1/blis/_src/frame/3/bli_l3_ft_ukr.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/3/bli_l3_ind.c` & `blis-0.9.1.dev1/blis/_src/frame/3/bli_l3_ind.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/3/bli_l3_ind.h` & `blis-0.9.1.dev1/blis/_src/frame/3/bli_l3_ind.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/3/bli_l3_ind_ukr.h` & `blis-0.9.1.dev1/blis/_src/frame/3/bli_l3_ind_ukr.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/3/bli_l3_int.c` & `blis-0.9.1.dev1/blis/_src/frame/3/bli_l3_int.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/3/bli_l3_int.h` & `blis-0.9.1.dev1/blis/_src/frame/3/bli_l3_int.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/3/bli_l3_oapi.c` & `blis-0.9.1.dev1/blis/_src/frame/3/bli_l3_oapi.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/3/bli_l3_oapi.h` & `blis-0.9.1.dev1/blis/_src/frame/3/bli_l3_oapi.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/3/bli_l3_oapi_ex.c` & `blis-0.9.1.dev1/blis/_src/frame/3/bli_l3_oapi_ex.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/3/bli_l3_oapi_ex.h` & `blis-0.9.1.dev1/blis/_src/frame/3/bli_l3_oapi_ex.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/3/bli_l3_oft.h` & `blis-0.9.1.dev1/blis/_src/frame/3/bli_l3_oft.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/3/bli_l3_oft_var.h` & `blis-0.9.1.dev1/blis/_src/frame/3/bli_l3_oft_var.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/3/bli_l3_packab.c` & `blis-0.9.1.dev1/blis/_src/frame/3/bli_l3_packab.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/3/bli_l3_packab.h` & `blis-0.9.1.dev1/blis/_src/frame/3/bli_l3_packab.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/3/bli_l3_prune.c` & `blis-0.9.1.dev1/blis/_src/frame/3/bli_l3_prune.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/3/bli_l3_prune.h` & `blis-0.9.1.dev1/blis/_src/frame/3/bli_l3_prune.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/3/bli_l3_schema.c` & `blis-0.9.1.dev1/blis/_src/frame/3/bli_l3_schema.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/3/bli_l3_schema.h` & `blis-0.9.1.dev1/blis/_src/frame/3/bli_l3_schema.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/3/bli_l3_sup.c` & `blis-0.9.1.dev1/blis/_src/frame/3/bli_l3_sup.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/3/bli_l3_sup.h` & `blis-0.9.1.dev1/blis/_src/frame/3/bli_l3_sup.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/3/bli_l3_sup_ft_ker.h` & `blis-0.9.1.dev1/blis/_src/frame/3/bli_l3_sup_ft_ker.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/3/bli_l3_sup_int.c` & `blis-0.9.1.dev1/blis/_src/frame/3/bli_l3_sup_int.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/3/bli_l3_sup_int.h` & `blis-0.9.1.dev1/blis/_src/frame/3/bli_l3_sup_int.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/3/bli_l3_sup_ker.h` & `blis-0.9.1.dev1/blis/_src/frame/3/bli_l3_sup_ker.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/3/bli_l3_sup_ker_prot.h` & `blis-0.9.1.dev1/blis/_src/frame/3/bli_l3_sup_ker_prot.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/3/bli_l3_sup_oft.h` & `blis-0.9.1.dev1/blis/_src/frame/3/bli_l3_sup_oft.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/3/bli_l3_sup_packm_a.c` & `blis-0.9.1.dev1/blis/_src/frame/3/bli_l3_sup_packm_a.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/3/bli_l3_sup_packm_a.h` & `blis-0.9.1.dev1/blis/_src/frame/3/bli_l3_sup_packm_a.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/3/bli_l3_sup_packm_b.c` & `blis-0.9.1.dev1/blis/_src/frame/3/bli_l3_sup_packm_b.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/3/bli_l3_sup_packm_b.h` & `blis-0.9.1.dev1/blis/_src/frame/3/bli_l3_sup_packm_b.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/3/bli_l3_sup_packm_var.c` & `blis-0.9.1.dev1/blis/_src/frame/3/bli_l3_sup_packm_var.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/3/bli_l3_sup_packm_var.h` & `blis-0.9.1.dev1/blis/_src/frame/3/bli_l3_sup_packm_var.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/3/bli_l3_sup_ref.c` & `blis-0.9.1.dev1/blis/_src/frame/3/bli_l3_sup_ref.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/3/bli_l3_sup_ref.h` & `blis-0.9.1.dev1/blis/_src/frame/3/bli_l3_sup_ref.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/3/bli_l3_sup_var12.c` & `blis-0.9.1.dev1/blis/_src/frame/3/bli_l3_sup_var12.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/3/bli_l3_sup_var1n2m.c` & `blis-0.9.1.dev1/blis/_src/frame/3/bli_l3_sup_var1n2m.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/3/bli_l3_sup_vars.h` & `blis-0.9.1.dev1/blis/_src/frame/3/bli_l3_sup_vars.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/3/bli_l3_tapi.c` & `blis-0.9.1.dev1/blis/_src/frame/3/bli_l3_tapi.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/3/bli_l3_tapi.h` & `blis-0.9.1.dev1/blis/_src/frame/3/bli_l3_tapi.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/3/bli_l3_tapi_ex.c` & `blis-0.9.1.dev1/blis/_src/frame/3/bli_l3_tapi_ex.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/3/bli_l3_tapi_ex.h` & `blis-0.9.1.dev1/blis/_src/frame/3/bli_l3_tapi_ex.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/3/bli_l3_thrinfo.c` & `blis-0.9.1.dev1/blis/_src/frame/3/bli_l3_thrinfo.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/3/bli_l3_thrinfo.h` & `blis-0.9.1.dev1/blis/_src/frame/3/bli_l3_thrinfo.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/3/bli_l3_ukr.h` & `blis-0.9.1.dev1/blis/_src/frame/3/bli_l3_ukr.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/3/bli_l3_ukr_fpa.c` & `blis-0.9.1.dev1/blis/_src/frame/3/bli_l3_ukr_fpa.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/3/bli_l3_ukr_fpa.h` & `blis-0.9.1.dev1/blis/_src/frame/3/bli_l3_ukr_fpa.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/3/bli_l3_ukr_oapi.c` & `blis-0.9.1.dev1/blis/_src/frame/3/bli_l3_ukr_oapi.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/3/bli_l3_ukr_oapi.h` & `blis-0.9.1.dev1/blis/_src/frame/3/bli_l3_ukr_oapi.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/3/bli_l3_ukr_prot.h` & `blis-0.9.1.dev1/blis/_src/frame/3/bli_l3_ukr_prot.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/3/bli_l3_ukr_tapi.c` & `blis-0.9.1.dev1/blis/_src/frame/3/bli_l3_ukr_tapi.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/3/bli_l3_ukr_tapi.h` & `blis-0.9.1.dev1/blis/_src/frame/3/bli_l3_ukr_tapi.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/3/gemm/bli_gemm.h` & `blis-0.9.1.dev1/blis/_src/frame/3/gemm/bli_gemm.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/3/gemm/bli_gemm_blk_var1.c` & `blis-0.9.1.dev1/blis/_src/frame/3/gemm/bli_gemm_blk_var1.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/3/gemm/bli_gemm_blk_var2.c` & `blis-0.9.1.dev1/blis/_src/frame/3/gemm/bli_gemm_blk_var2.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/3/gemm/bli_gemm_blk_var3.c` & `blis-0.9.1.dev1/blis/_src/frame/3/gemm/bli_gemm_blk_var3.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/3/gemm/bli_gemm_cntl.c` & `blis-0.9.1.dev1/blis/_src/frame/3/gemm/bli_gemm_cntl.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/3/gemm/bli_gemm_cntl.h` & `blis-0.9.1.dev1/blis/_src/frame/3/gemm/bli_gemm_cntl.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/3/gemm/bli_gemm_front.c` & `blis-0.9.1.dev1/blis/_src/frame/3/gemm/bli_gemm_front.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/3/gemm/bli_gemm_front.h` & `blis-0.9.1.dev1/blis/_src/frame/3/gemm/bli_gemm_front.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/3/gemm/bli_gemm_ker_var1.c` & `blis-0.9.1.dev1/blis/_src/frame/3/gemm/bli_gemm_ker_var1.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/3/gemm/bli_gemm_ker_var2.c` & `blis-0.9.1.dev1/blis/_src/frame/3/gemm/bli_gemm_ker_var2.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/3/gemm/bli_gemm_md.c` & `blis-0.9.1.dev1/blis/_src/frame/3/gemm/bli_gemm_md.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/3/gemm/bli_gemm_md.h` & `blis-0.9.1.dev1/blis/_src/frame/3/gemm/bli_gemm_md.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/3/gemm/bli_gemm_md_c2r_ref.c` & `blis-0.9.1.dev1/blis/_src/frame/3/gemm/bli_gemm_md_c2r_ref.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/3/gemm/bli_gemm_md_c2r_ref.h` & `blis-0.9.1.dev1/blis/_src/frame/3/gemm/bli_gemm_md_c2r_ref.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/3/gemm/bli_gemm_var.h` & `blis-0.9.1.dev1/blis/_src/frame/3/gemm/bli_gemm_var.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/3/gemm/ind/bli_gemm_ind_opt.h` & `blis-0.9.1.dev1/blis/_src/frame/3/gemm/ind/bli_gemm_ind_opt.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/3/gemm/other/bli_gemm_ker_var2.c` & `blis-0.9.1.dev1/blis/_src/frame/3/gemm/other/bli_gemm_ker_var2.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/3/gemm/other/bli_gemm_ker_var2rr.c` & `blis-0.9.1.dev1/blis/_src/frame/3/gemm/other/bli_gemm_ker_var2rr.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/3/gemm/other/bli_gemm_ker_var2sl.c` & `blis-0.9.1.dev1/blis/_src/frame/3/gemm/other/bli_gemm_ker_var2sl.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/3/gemm/other/bli_gemm_ker_var5.c` & `blis-0.9.1.dev1/blis/_src/frame/3/gemm/other/bli_gemm_ker_var5.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/3/gemm/other/bli_gemm_ker_var5.h` & `blis-0.9.1.dev1/blis/_src/frame/3/gemm/other/bli_gemm_ker_var5.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/3/gemmt/bli_gemmt.h` & `blis-0.9.1.dev1/blis/_src/frame/3/gemmt/bli_gemmt.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/3/gemmt/bli_gemmt_front.c` & `blis-0.9.1.dev1/blis/_src/frame/3/gemmt/bli_gemmt_front.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/3/gemmt/bli_gemmt_front.h` & `blis-0.9.1.dev1/blis/_src/frame/3/gemmt/bli_gemmt_front.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/3/gemmt/bli_gemmt_l_ker_var2.c` & `blis-0.9.1.dev1/blis/_src/frame/3/gemmt/bli_gemmt_l_ker_var2.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/3/gemmt/bli_gemmt_u_ker_var2.c` & `blis-0.9.1.dev1/blis/_src/frame/3/gemmt/bli_gemmt_u_ker_var2.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/3/gemmt/bli_gemmt_var.h` & `blis-0.9.1.dev1/blis/_src/frame/3/gemmt/bli_gemmt_var.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/3/gemmt/bli_gemmt_x_ker_var2.c` & `blis-0.9.1.dev1/blis/_src/frame/3/gemmt/bli_gemmt_x_ker_var2.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/3/gemmt/other/bli_gemmt_l_ker_var2.c` & `blis-0.9.1.dev1/blis/_src/frame/3/gemmt/other/bli_gemmt_l_ker_var2.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/3/gemmt/other/bli_gemmt_u_ker_var2.c` & `blis-0.9.1.dev1/blis/_src/frame/3/gemmt/other/bli_gemmt_u_ker_var2.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/3/hemm/bli_hemm.h` & `blis-0.9.1.dev1/blis/_src/frame/3/hemm/bli_hemm.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/3/hemm/bli_hemm_front.c` & `blis-0.9.1.dev1/blis/_src/frame/3/hemm/bli_hemm_front.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/3/hemm/bli_hemm_front.h` & `blis-0.9.1.dev1/blis/_src/frame/3/hemm/bli_hemm_front.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/3/old/bli_l3_ft_ex.h` & `blis-0.9.1.dev1/blis/_src/frame/3/old/bli_l3_ft_ex.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/3/old/bli_l3_sup_edge.h` & `blis-0.9.1.dev1/blis/_src/frame/3/old/bli_l3_sup_edge.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/3/old/bli_l3_sup_var1n2m.c` & `blis-0.9.1.dev1/blis/_src/frame/3/old/bli_l3_sup_var1n2m.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/3/symm/bli_symm.h` & `blis-0.9.1.dev1/blis/_src/frame/3/symm/bli_symm.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/3/symm/bli_symm_front.c` & `blis-0.9.1.dev1/blis/_src/frame/3/symm/bli_symm_front.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/3/symm/bli_symm_front.h` & `blis-0.9.1.dev1/blis/_src/frame/3/symm/bli_symm_front.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/3/trmm/bli_trmm.h` & `blis-0.9.1.dev1/blis/_src/frame/3/trmm/bli_trmm.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/3/trmm/bli_trmm_front.c` & `blis-0.9.1.dev1/blis/_src/frame/3/trmm/bli_trmm_front.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/3/trmm/bli_trmm_front.h` & `blis-0.9.1.dev1/blis/_src/frame/3/trmm/bli_trmm_front.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/3/trmm/bli_trmm_ll_ker_var2.c` & `blis-0.9.1.dev1/blis/_src/frame/3/trmm/bli_trmm_ll_ker_var2.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/3/trmm/bli_trmm_lu_ker_var2.c` & `blis-0.9.1.dev1/blis/_src/frame/3/trmm/bli_trmm_lu_ker_var2.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/3/trmm/bli_trmm_rl_ker_var2.c` & `blis-0.9.1.dev1/blis/_src/frame/3/trmm/bli_trmm_rl_ker_var2.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/3/trmm/bli_trmm_ru_ker_var2.c` & `blis-0.9.1.dev1/blis/_src/frame/3/trmm/bli_trmm_ru_ker_var2.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/3/trmm/bli_trmm_var.h` & `blis-0.9.1.dev1/blis/_src/frame/3/trmm/bli_trmm_var.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/3/trmm/bli_trmm_xx_ker_var2.c` & `blis-0.9.1.dev1/blis/_src/frame/3/trmm/bli_trmm_xx_ker_var2.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/3/trmm/other/bli_trmm_ll_ker_var2.c` & `blis-0.9.1.dev1/blis/_src/frame/3/trmm/other/bli_trmm_ll_ker_var2.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/3/trmm/other/bli_trmm_ll_ker_var2rr.c` & `blis-0.9.1.dev1/blis/_src/frame/3/trmm/other/bli_trmm_ll_ker_var2rr.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/3/trmm/other/bli_trmm_ll_ker_var2sl.c` & `blis-0.9.1.dev1/blis/_src/frame/3/trmm/other/bli_trmm_ll_ker_var2sl.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/3/trmm/other/bli_trmm_lu_ker_var2.c` & `blis-0.9.1.dev1/blis/_src/frame/3/trmm/other/bli_trmm_lu_ker_var2.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/3/trmm/other/bli_trmm_lu_ker_var2rr.c` & `blis-0.9.1.dev1/blis/_src/frame/3/trmm/other/bli_trmm_lu_ker_var2rr.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/3/trmm/other/bli_trmm_lu_ker_var2sl.c` & `blis-0.9.1.dev1/blis/_src/frame/3/trmm/other/bli_trmm_lu_ker_var2sl.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/3/trmm/other/bli_trmm_rl_ker_var2.c` & `blis-0.9.1.dev1/blis/_src/frame/3/trmm/other/bli_trmm_rl_ker_var2.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/3/trmm/other/bli_trmm_rl_ker_var2rr.c` & `blis-0.9.1.dev1/blis/_src/frame/3/trmm/other/bli_trmm_rl_ker_var2rr.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/3/trmm/other/bli_trmm_rl_ker_var2sl.c` & `blis-0.9.1.dev1/blis/_src/frame/3/trmm/other/bli_trmm_rl_ker_var2sl.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/3/trmm/other/bli_trmm_ru_ker_var2.c` & `blis-0.9.1.dev1/blis/_src/frame/3/trmm/other/bli_trmm_ru_ker_var2.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/3/trmm/other/bli_trmm_ru_ker_var2rr.c` & `blis-0.9.1.dev1/blis/_src/frame/3/trmm/other/bli_trmm_ru_ker_var2rr.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/3/trmm/other/bli_trmm_ru_ker_var2sl.c` & `blis-0.9.1.dev1/blis/_src/frame/3/trmm/other/bli_trmm_ru_ker_var2sl.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/3/trmm3/bli_trmm3.h` & `blis-0.9.1.dev1/blis/_src/frame/3/trmm3/bli_trmm3.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/3/trmm3/bli_trmm3_front.c` & `blis-0.9.1.dev1/blis/_src/frame/3/trmm3/bli_trmm3_front.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/3/trmm3/bli_trmm3_front.h` & `blis-0.9.1.dev1/blis/_src/frame/3/trmm3/bli_trmm3_front.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/3/trsm/bli_trsm.h` & `blis-0.9.1.dev1/blis/_src/frame/3/trsm/bli_trsm.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/3/trsm/bli_trsm_blk_var1.c` & `blis-0.9.1.dev1/blis/_src/frame/3/trsm/bli_trsm_blk_var1.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/3/trsm/bli_trsm_blk_var2.c` & `blis-0.9.1.dev1/blis/_src/frame/3/trsm/bli_trsm_blk_var2.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/3/trsm/bli_trsm_blk_var3.c` & `blis-0.9.1.dev1/blis/_src/frame/3/trsm/bli_trsm_blk_var3.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/3/trsm/bli_trsm_cntl.c` & `blis-0.9.1.dev1/blis/_src/frame/3/trsm/bli_trsm_cntl.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/3/trsm/bli_trsm_cntl.h` & `blis-0.9.1.dev1/blis/_src/frame/3/trsm/bli_trsm_cntl.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/3/trsm/bli_trsm_front.c` & `blis-0.9.1.dev1/blis/_src/frame/3/trsm/bli_trsm_front.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/3/trsm/bli_trsm_front.h` & `blis-0.9.1.dev1/blis/_src/frame/3/trsm/bli_trsm_front.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/3/trsm/bli_trsm_ll_ker_var2.c` & `blis-0.9.1.dev1/blis/_src/frame/3/trsm/bli_trsm_ll_ker_var2.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/3/trsm/bli_trsm_lu_ker_var2.c` & `blis-0.9.1.dev1/blis/_src/frame/3/trsm/bli_trsm_lu_ker_var2.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/3/trsm/bli_trsm_rl_ker_var2.c` & `blis-0.9.1.dev1/blis/_src/frame/3/trsm/bli_trsm_rl_ker_var2.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/3/trsm/bli_trsm_ru_ker_var2.c` & `blis-0.9.1.dev1/blis/_src/frame/3/trsm/bli_trsm_ru_ker_var2.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/3/trsm/bli_trsm_var.h` & `blis-0.9.1.dev1/blis/_src/frame/3/trsm/bli_trsm_var.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/3/trsm/bli_trsm_xx_ker_var2.c` & `blis-0.9.1.dev1/blis/_src/frame/3/trsm/bli_trsm_xx_ker_var2.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/3/trsm/other/bli_trsm_ll_ker_var2.c` & `blis-0.9.1.dev1/blis/_src/frame/3/trsm/other/bli_trsm_ll_ker_var2.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/3/trsm/other/bli_trsm_ll_ker_var2rr.c` & `blis-0.9.1.dev1/blis/_src/frame/3/trsm/other/bli_trsm_ll_ker_var2rr.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/3/trsm/other/bli_trsm_ll_ker_var2sl.c` & `blis-0.9.1.dev1/blis/_src/frame/3/trsm/other/bli_trsm_ll_ker_var2sl.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/3/trsm/other/bli_trsm_lu_ker_var2.c` & `blis-0.9.1.dev1/blis/_src/frame/3/trsm/other/bli_trsm_lu_ker_var2.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/3/trsm/other/bli_trsm_lu_ker_var2rr.c` & `blis-0.9.1.dev1/blis/_src/frame/3/trsm/other/bli_trsm_lu_ker_var2rr.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/3/trsm/other/bli_trsm_lu_ker_var2sl.c` & `blis-0.9.1.dev1/blis/_src/frame/3/trsm/other/bli_trsm_lu_ker_var2sl.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/3/trsm/other/bli_trsm_rl_ker_var2.c` & `blis-0.9.1.dev1/blis/_src/frame/3/trsm/other/bli_trsm_rl_ker_var2.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/3/trsm/other/bli_trsm_ru_ker_var2.c` & `blis-0.9.1.dev1/blis/_src/frame/3/trsm/other/bli_trsm_ru_ker_var2.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/base/bli_apool.c` & `blis-0.9.1.dev1/blis/_src/frame/base/bli_apool.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/base/bli_apool.h` & `blis-0.9.1.dev1/blis/_src/frame/base/bli_apool.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/base/bli_arch.c` & `blis-0.9.1.dev1/blis/_src/frame/base/bli_arch.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/base/bli_arch.h` & `blis-0.9.1.dev1/blis/_src/frame/base/bli_arch.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/base/bli_array.c` & `blis-0.9.1.dev1/blis/_src/frame/base/bli_array.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/base/bli_array.h` & `blis-0.9.1.dev1/blis/_src/frame/base/bli_array.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/base/bli_auxinfo.h` & `blis-0.9.1.dev1/blis/_src/frame/base/bli_auxinfo.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/base/bli_blksz.c` & `blis-0.9.1.dev1/blis/_src/frame/base/bli_blksz.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/base/bli_blksz.h` & `blis-0.9.1.dev1/blis/_src/frame/base/bli_blksz.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/base/bli_check.c` & `blis-0.9.1.dev1/blis/_src/frame/base/bli_check.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/base/bli_check.h` & `blis-0.9.1.dev1/blis/_src/frame/base/bli_check.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/base/bli_clock.c` & `blis-0.9.1.dev1/blis/_src/frame/base/bli_clock.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/base/bli_clock.h` & `blis-0.9.1.dev1/blis/_src/frame/base/bli_clock.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/base/bli_cntl.c` & `blis-0.9.1.dev1/blis/_src/frame/base/bli_cntl.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/base/bli_cntl.h` & `blis-0.9.1.dev1/blis/_src/frame/base/bli_cntl.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/base/bli_cntx.c` & `blis-0.9.1.dev1/blis/_src/frame/base/bli_cntx.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/base/bli_cntx.h` & `blis-0.9.1.dev1/blis/_src/frame/base/bli_cntx.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/base/bli_const.c` & `blis-0.9.1.dev1/blis/_src/frame/base/bli_const.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/base/bli_const.h` & `blis-0.9.1.dev1/blis/_src/frame/base/bli_const.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/base/bli_cpuid.c` & `blis-0.9.1.dev1/blis/_src/frame/base/bli_cpuid.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/base/bli_cpuid.h` & `blis-0.9.1.dev1/blis/_src/frame/base/bli_cpuid.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/base/bli_env.c` & `blis-0.9.1.dev1/blis/_src/frame/base/bli_env.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/base/bli_env.h` & `blis-0.9.1.dev1/blis/_src/frame/base/bli_env.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/base/bli_error.c` & `blis-0.9.1.dev1/blis/_src/frame/base/bli_error.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/base/bli_error.h` & `blis-0.9.1.dev1/blis/_src/frame/base/bli_error.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/base/bli_func.c` & `blis-0.9.1.dev1/blis/_src/frame/base/bli_func.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/base/bli_func.h` & `blis-0.9.1.dev1/blis/_src/frame/base/bli_func.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/base/bli_getopt.c` & `blis-0.9.1.dev1/blis/_src/frame/base/bli_getopt.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/base/bli_getopt.h` & `blis-0.9.1.dev1/blis/_src/frame/base/bli_getopt.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/base/bli_gks.c` & `blis-0.9.1.dev1/blis/_src/frame/base/bli_gks.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/base/bli_gks.h` & `blis-0.9.1.dev1/blis/_src/frame/base/bli_gks.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/base/bli_ind.c` & `blis-0.9.1.dev1/blis/_src/frame/base/bli_ind.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/base/bli_ind.h` & `blis-0.9.1.dev1/blis/_src/frame/base/bli_ind.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/base/bli_info.c` & `blis-0.9.1.dev1/blis/_src/frame/base/bli_info.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/base/bli_info.h` & `blis-0.9.1.dev1/blis/_src/frame/base/bli_info.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/base/bli_init.c` & `blis-0.9.1.dev1/blis/_src/frame/base/bli_init.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/base/bli_init.h` & `blis-0.9.1.dev1/blis/_src/frame/base/bli_init.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/base/bli_machval.c` & `blis-0.9.1.dev1/blis/_src/frame/base/bli_machval.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/base/bli_machval.h` & `blis-0.9.1.dev1/blis/_src/frame/base/bli_machval.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/base/bli_malloc.c` & `blis-0.9.1.dev1/blis/_src/frame/base/bli_malloc.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/base/bli_malloc.h` & `blis-0.9.1.dev1/blis/_src/frame/base/bli_malloc.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/base/bli_mbool.c` & `blis-0.9.1.dev1/blis/_src/frame/base/bli_mbool.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/base/bli_mbool.h` & `blis-0.9.1.dev1/blis/_src/frame/base/bli_mbool.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/base/bli_mem.h` & `blis-0.9.1.dev1/blis/_src/frame/base/bli_mem.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/base/bli_memsys.c` & `blis-0.9.1.dev1/blis/_src/frame/base/bli_memsys.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/base/bli_memsys.h` & `blis-0.9.1.dev1/blis/_src/frame/base/bli_memsys.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/base/bli_obj.c` & `blis-0.9.1.dev1/blis/_src/frame/base/bli_obj.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/base/bli_obj.h` & `blis-0.9.1.dev1/blis/_src/frame/base/bli_obj.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/base/bli_obj_scalar.c` & `blis-0.9.1.dev1/blis/_src/frame/base/bli_obj_scalar.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/base/bli_obj_scalar.h` & `blis-0.9.1.dev1/blis/_src/frame/base/bli_obj_scalar.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/base/bli_opid.h` & `blis-0.9.1.dev1/blis/_src/frame/base/bli_opid.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/base/bli_pack.c` & `blis-0.9.1.dev1/blis/_src/frame/base/bli_pack.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/base/bli_pack.h` & `blis-0.9.1.dev1/blis/_src/frame/base/bli_pack.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/base/bli_param_map.c` & `blis-0.9.1.dev1/blis/_src/frame/base/bli_param_map.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/base/bli_param_map.h` & `blis-0.9.1.dev1/blis/_src/frame/base/bli_param_map.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/base/bli_part.c` & `blis-0.9.1.dev1/blis/_src/frame/base/bli_part.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/base/bli_part.h` & `blis-0.9.1.dev1/blis/_src/frame/base/bli_part.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/base/bli_pba.c` & `blis-0.9.1.dev1/blis/_src/frame/base/bli_pba.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/base/bli_pba.h` & `blis-0.9.1.dev1/blis/_src/frame/base/bli_pba.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/base/bli_pool.c` & `blis-0.9.1.dev1/blis/_src/frame/base/bli_pool.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/base/bli_pool.h` & `blis-0.9.1.dev1/blis/_src/frame/base/bli_pool.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/base/bli_prune.c` & `blis-0.9.1.dev1/blis/_src/frame/base/bli_prune.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/base/bli_prune.h` & `blis-0.9.1.dev1/blis/_src/frame/base/bli_prune.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/base/bli_query.c` & `blis-0.9.1.dev1/blis/_src/frame/base/bli_query.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/base/bli_query.h` & `blis-0.9.1.dev1/blis/_src/frame/base/bli_query.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/base/bli_rntm.c` & `blis-0.9.1.dev1/blis/_src/frame/base/bli_rntm.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/base/bli_rntm.h` & `blis-0.9.1.dev1/blis/_src/frame/base/bli_rntm.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/base/bli_sba.c` & `blis-0.9.1.dev1/blis/_src/frame/base/bli_sba.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/base/bli_sba.h` & `blis-0.9.1.dev1/blis/_src/frame/base/bli_sba.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/base/bli_setgetijm.c` & `blis-0.9.1.dev1/blis/_src/frame/base/bli_setgetijm.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/base/bli_setgetijm.h` & `blis-0.9.1.dev1/blis/_src/frame/base/bli_setgetijm.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/base/bli_setgetijv.c` & `blis-0.9.1.dev1/blis/_src/frame/base/bli_setgetijv.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/base/bli_setgetijv.h` & `blis-0.9.1.dev1/blis/_src/frame/base/bli_setgetijv.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/base/bli_setri.c` & `blis-0.9.1.dev1/blis/_src/frame/base/bli_setri.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/base/bli_setri.h` & `blis-0.9.1.dev1/blis/_src/frame/base/bli_setri.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/base/bli_string.c` & `blis-0.9.1.dev1/blis/_src/frame/base/bli_string.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/base/bli_string.h` & `blis-0.9.1.dev1/blis/_src/frame/base/bli_string.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/base/bli_winsys.c` & `blis-0.9.1.dev1/blis/_src/frame/base/bli_winsys.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/base/bli_winsys.h` & `blis-0.9.1.dev1/blis/_src/frame/base/bli_winsys.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/base/cast/bli_castm.c` & `blis-0.9.1.dev1/blis/_src/frame/base/cast/bli_castm.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/base/cast/bli_castm.h` & `blis-0.9.1.dev1/blis/_src/frame/base/cast/bli_castm.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/base/cast/bli_castnzm.c` & `blis-0.9.1.dev1/blis/_src/frame/base/cast/bli_castnzm.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/base/cast/bli_castnzm.h` & `blis-0.9.1.dev1/blis/_src/frame/base/cast/bli_castnzm.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/base/cast/bli_castv.c` & `blis-0.9.1.dev1/blis/_src/frame/base/cast/bli_castv.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/base/cast/bli_castv.h` & `blis-0.9.1.dev1/blis/_src/frame/base/cast/bli_castv.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/base/cast/old/bli_cast_check.c` & `blis-0.9.1.dev1/blis/_src/frame/base/cast/old/bli_cast_check.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/base/cast/old/bli_cast_check.h` & `blis-0.9.1.dev1/blis/_src/frame/base/cast/old/bli_cast_check.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/base/check/bli_obj_check.c` & `blis-0.9.1.dev1/blis/_src/frame/base/check/bli_obj_check.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/base/check/bli_obj_check.h` & `blis-0.9.1.dev1/blis/_src/frame/base/check/bli_obj_check.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/base/check/bli_part_check.c` & `blis-0.9.1.dev1/blis/_src/frame/base/check/bli_part_check.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/base/check/bli_part_check.h` & `blis-0.9.1.dev1/blis/_src/frame/base/check/bli_part_check.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/base/noopt/bli_dlamch.c` & `blis-0.9.1.dev1/blis/_src/frame/base/noopt/bli_dlamch.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/base/noopt/bli_dlamch.h` & `blis-0.9.1.dev1/blis/_src/frame/base/noopt/bli_dlamch.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/base/noopt/bli_lsame.c` & `blis-0.9.1.dev1/blis/_src/frame/base/noopt/bli_lsame.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/base/noopt/bli_lsame.h` & `blis-0.9.1.dev1/blis/_src/frame/base/noopt/bli_lsame.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/base/noopt/bli_slamch.c` & `blis-0.9.1.dev1/blis/_src/frame/base/noopt/bli_slamch.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/base/noopt/bli_slamch.h` & `blis-0.9.1.dev1/blis/_src/frame/base/noopt/bli_slamch.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/base/proj/bli_projm.c` & `blis-0.9.1.dev1/blis/_src/frame/base/proj/bli_projm.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/base/proj/bli_projm.h` & `blis-0.9.1.dev1/blis/_src/frame/base/proj/bli_projm.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/base/proj/bli_projv.c` & `blis-0.9.1.dev1/blis/_src/frame/base/proj/bli_projv.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/base/proj/bli_projv.h` & `blis-0.9.1.dev1/blis/_src/frame/base/proj/bli_projv.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/base/proj/old/bli_proj_check.c` & `blis-0.9.1.dev1/blis/_src/frame/base/proj/old/bli_proj_check.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/base/proj/old/bli_proj_check.h` & `blis-0.9.1.dev1/blis/_src/frame/base/proj/old/bli_proj_check.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/amd/bla_copy_amd.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/amd/bla_copy_amd.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/amd/bla_gemv_amd.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/amd/bla_gemv_amd.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/attic/bla_gbmv.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/attic/bla_gbmv.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/attic/bla_gbmv.h` & `blis-0.9.1.dev1/blis/_src/frame/compat/attic/bla_gbmv.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/attic/bla_hbmv.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/attic/bla_hbmv.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/attic/bla_hbmv.h` & `blis-0.9.1.dev1/blis/_src/frame/compat/attic/bla_hbmv.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/attic/bla_hpmv.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/attic/bla_hpmv.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/attic/bla_hpmv.h` & `blis-0.9.1.dev1/blis/_src/frame/compat/attic/bla_hpmv.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/attic/bla_hpr.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/attic/bla_hpr.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/attic/bla_hpr.h` & `blis-0.9.1.dev1/blis/_src/frame/compat/attic/bla_hpr.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/attic/bla_hpr2.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/attic/bla_hpr2.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/attic/bla_hpr2.h` & `blis-0.9.1.dev1/blis/_src/frame/compat/attic/bla_hpr2.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/attic/bla_rot.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/attic/bla_rot.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/attic/bla_rot.h` & `blis-0.9.1.dev1/blis/_src/frame/compat/attic/bla_rot.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/attic/bla_rotg.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/attic/bla_rotg.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/attic/bla_rotg.h` & `blis-0.9.1.dev1/blis/_src/frame/compat/attic/bla_rotg.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/attic/bla_rotm.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/attic/bla_rotm.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/attic/bla_rotm.h` & `blis-0.9.1.dev1/blis/_src/frame/compat/attic/bla_rotm.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/attic/bla_rotmg.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/attic/bla_rotmg.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/attic/bla_rotmg.h` & `blis-0.9.1.dev1/blis/_src/frame/compat/attic/bla_rotmg.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/attic/bla_sbmv.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/attic/bla_sbmv.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/attic/bla_sbmv.h` & `blis-0.9.1.dev1/blis/_src/frame/compat/attic/bla_sbmv.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/attic/bla_spmv.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/attic/bla_spmv.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/attic/bla_spmv.h` & `blis-0.9.1.dev1/blis/_src/frame/compat/attic/bla_spmv.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/attic/bla_spr.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/attic/bla_spr.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/attic/bla_spr.h` & `blis-0.9.1.dev1/blis/_src/frame/compat/attic/bla_spr.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/attic/bla_spr2.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/attic/bla_spr2.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/attic/bla_spr2.h` & `blis-0.9.1.dev1/blis/_src/frame/compat/attic/bla_spr2.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/attic/bla_tbmv.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/attic/bla_tbmv.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/attic/bla_tbmv.h` & `blis-0.9.1.dev1/blis/_src/frame/compat/attic/bla_tbmv.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/attic/bla_tbsv.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/attic/bla_tbsv.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/attic/bla_tbsv.h` & `blis-0.9.1.dev1/blis/_src/frame/compat/attic/bla_tbsv.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/attic/bla_tpmv.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/attic/bla_tpmv.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/attic/bla_tpmv.h` & `blis-0.9.1.dev1/blis/_src/frame/compat/attic/bla_tpmv.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/attic/bla_tpsv.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/attic/bla_tpsv.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/attic/bla_tpsv.h` & `blis-0.9.1.dev1/blis/_src/frame/compat/attic/bla_tpsv.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/bla_amax.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/bla_amax.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/bla_amax.h` & `blis-0.9.1.dev1/blis/_src/frame/compat/bla_amax.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/bla_asum.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/bla_asum.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/bla_asum.h` & `blis-0.9.1.dev1/blis/_src/frame/compat/bla_asum.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/bla_axpy.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/bla_axpy.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/bla_axpy.h` & `blis-0.9.1.dev1/blis/_src/frame/compat/bla_axpy.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/bla_copy.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/bla_copy.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/bla_copy.h` & `blis-0.9.1.dev1/blis/_src/frame/compat/bla_copy.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/bla_dot.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/bla_dot.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/bla_dot.h` & `blis-0.9.1.dev1/blis/_src/frame/compat/bla_dot.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/bla_gemm.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/bla_gemm.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/bla_gemm.h` & `blis-0.9.1.dev1/blis/_src/frame/compat/bla_gemm.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/bla_gemv.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/bla_gemv.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/bla_gemv.h` & `blis-0.9.1.dev1/blis/_src/frame/compat/bla_gemv.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/bla_ger.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/bla_ger.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/bla_ger.h` & `blis-0.9.1.dev1/blis/_src/frame/compat/bla_ger.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/bla_hemm.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/bla_hemm.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/bla_hemm.h` & `blis-0.9.1.dev1/blis/_src/frame/compat/bla_hemm.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/bla_hemv.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/bla_hemv.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/bla_hemv.h` & `blis-0.9.1.dev1/blis/_src/frame/compat/bla_hemv.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/bla_her.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/bla_her.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/bla_her.h` & `blis-0.9.1.dev1/blis/_src/frame/compat/bla_her.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/bla_her2.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/bla_her2.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/bla_her2.h` & `blis-0.9.1.dev1/blis/_src/frame/compat/bla_her2.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/bla_her2k.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/bla_her2k.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/bla_her2k.h` & `blis-0.9.1.dev1/blis/_src/frame/compat/bla_her2k.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/bla_herk.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/bla_herk.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/bla_herk.h` & `blis-0.9.1.dev1/blis/_src/frame/compat/bla_herk.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/bla_nrm2.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/bla_nrm2.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/bla_nrm2.h` & `blis-0.9.1.dev1/blis/_src/frame/compat/bla_nrm2.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/bla_scal.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/bla_scal.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/bla_scal.h` & `blis-0.9.1.dev1/blis/_src/frame/compat/bla_scal.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/bla_swap.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/bla_swap.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/bla_swap.h` & `blis-0.9.1.dev1/blis/_src/frame/compat/bla_swap.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/bla_symm.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/bla_symm.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/bla_symm.h` & `blis-0.9.1.dev1/blis/_src/frame/compat/bla_symm.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/bla_symv.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/bla_symv.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/bla_symv.h` & `blis-0.9.1.dev1/blis/_src/frame/compat/bla_symv.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/bla_syr.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/bla_syr.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/bla_syr.h` & `blis-0.9.1.dev1/blis/_src/frame/compat/bla_syr.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/bla_syr2.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/bla_syr2.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/bla_syr2.h` & `blis-0.9.1.dev1/blis/_src/frame/compat/bla_syr2.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/bla_syr2k.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/bla_syr2k.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/bla_syr2k.h` & `blis-0.9.1.dev1/blis/_src/frame/compat/bla_syr2k.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/bla_syrk.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/bla_syrk.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/bla_syrk.h` & `blis-0.9.1.dev1/blis/_src/frame/compat/bla_syrk.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/bla_trmm.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/bla_trmm.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/bla_trmm.h` & `blis-0.9.1.dev1/blis/_src/frame/compat/bla_trmm.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/bla_trmv.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/bla_trmv.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/bla_trmv.h` & `blis-0.9.1.dev1/blis/_src/frame/compat/bla_trmv.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/bla_trsm.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/bla_trsm.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/bla_trsm.h` & `blis-0.9.1.dev1/blis/_src/frame/compat/bla_trsm.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/bla_trsv.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/bla_trsv.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/bla_trsv.h` & `blis-0.9.1.dev1/blis/_src/frame/compat/bla_trsv.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/bli_blas.h` & `blis-0.9.1.dev1/blis/_src/frame/compat/bli_blas.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/blis/thread/b77_thread.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/blis/thread/b77_thread.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/blis/thread/b77_thread.h` & `blis-0.9.1.dev1/blis/_src/frame/compat/blis/thread/b77_thread.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/bli_cblas.h` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/bli_cblas.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/f77_sub/f77_amax_sub.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/f77_sub/f77_amax_sub.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/f77_sub/f77_amax_sub.h` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/f77_sub/f77_amax_sub.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/f77_sub/f77_asum_sub.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/f77_sub/f77_asum_sub.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/f77_sub/f77_asum_sub.h` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/f77_sub/f77_asum_sub.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/f77_sub/f77_dot_sub.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/f77_sub/f77_dot_sub.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/f77_sub/f77_dot_sub.h` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/f77_sub/f77_dot_sub.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/f77_sub/f77_nrm2_sub.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/f77_sub/f77_nrm2_sub.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/f77_sub/f77_nrm2_sub.h` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/f77_sub/f77_nrm2_sub.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas.h` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_caxpy.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_caxpy.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_ccopy.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_ccopy.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_cdotc_sub.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_cdotc_sub.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_cdotu_sub.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_cdotu_sub.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_cgbmv.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_cgbmv.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_cgemm.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_cgemm.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_cgemv.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_cgemv.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_cgerc.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_cgerc.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_cgeru.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_cgeru.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_chbmv.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_chbmv.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_chemm.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_chemm.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_chemv.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_chemv.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_cher.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_cher.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_cher2.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_cher2.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_cher2k.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_cher2k.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_cherk.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_cherk.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_chpmv.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_chpmv.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_chpr.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_chpr.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_chpr2.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_chpr2.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_cswap.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_cswap.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_csymm.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_csymm.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_csyr2k.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_csyr2k.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_csyrk.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_csyrk.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_ctbmv.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_ctbmv.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_ctbsv.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_ctbsv.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_ctpmv.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_ctpmv.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_ctpsv.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_ctpsv.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_ctrmm.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_ctrmm.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_ctrmv.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_ctrmv.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_ctrsm.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_ctrsm.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_ctrsv.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_ctrsv.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_dasum.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_dasum.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_daxpy.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_daxpy.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_dcopy.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_dcopy.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_ddot.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_ddot.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_dgbmv.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_dgbmv.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_dgemm.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_dgemm.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_dgemv.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_dgemv.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_dger.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_dger.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_dnrm2.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_dnrm2.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_drot.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_drot.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_dsbmv.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_dsbmv.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_dsdot.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_dsdot.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_dspmv.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_dspmv.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_dspr.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_dspr.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_dspr2.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_dspr2.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_dswap.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_dswap.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_dsymm.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_dsymm.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_dsymv.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_dsymv.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_dsyr.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_dsyr.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_dsyr2.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_dsyr2.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_dsyr2k.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_dsyr2k.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_dsyrk.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_dsyrk.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_dtbmv.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_dtbmv.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_dtbsv.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_dtbsv.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_dtpmv.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_dtpmv.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_dtpsv.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_dtpsv.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_dtrmm.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_dtrmm.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_dtrmv.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_dtrmv.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_dtrsm.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_dtrsm.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_dtrsv.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_dtrsv.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_dzasum.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_dzasum.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_dznrm2.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_dznrm2.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_f77.h` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_f77.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_icamax.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_icamax.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_idamax.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_idamax.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_isamax.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_isamax.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_izamax.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_izamax.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_sasum.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_sasum.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_saxpy.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_saxpy.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_scasum.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_scasum.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_scnrm2.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_scnrm2.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_scopy.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_scopy.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_sdot.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_sdot.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_sdsdot.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_sdsdot.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_sgbmv.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_sgbmv.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_sgemm.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_sgemm.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_sgemv.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_sgemv.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_sger.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_sger.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_snrm2.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_snrm2.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_srot.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_srot.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_srotm.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_srotm.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_ssbmv.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_ssbmv.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_sspmv.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_sspmv.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_sspr.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_sspr.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_sspr2.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_sspr2.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_sswap.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_sswap.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_ssymm.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_ssymm.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_ssymv.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_ssymv.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_ssyr.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_ssyr.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_ssyr2.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_ssyr2.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_ssyr2k.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_ssyr2k.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_ssyrk.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_ssyrk.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_stbmv.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_stbmv.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_stbsv.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_stbsv.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_stpmv.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_stpmv.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_stpsv.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_stpsv.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_strmm.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_strmm.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_strmv.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_strmv.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_strsm.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_strsm.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_strsv.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_strsv.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_xerbla.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_xerbla.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_zaxpy.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_zaxpy.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_zcopy.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_zcopy.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_zdotc_sub.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_zdotc_sub.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_zdotu_sub.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_zdotu_sub.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_zgbmv.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_zgbmv.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_zgemm.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_zgemm.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_zgemv.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_zgemv.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_zgerc.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_zgerc.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_zgeru.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_zgeru.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_zhbmv.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_zhbmv.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_zhemm.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_zhemm.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_zhemv.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_zhemv.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_zher.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_zher.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_zher2.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_zher2.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_zher2k.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_zher2k.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_zherk.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_zherk.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_zhpmv.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_zhpmv.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_zhpr.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_zhpr.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_zhpr2.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_zhpr2.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_zswap.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_zswap.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_zsymm.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_zsymm.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_zsyr2k.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_zsyr2k.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_zsyrk.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_zsyrk.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_ztbmv.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_ztbmv.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_ztbsv.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_ztbsv.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_ztpmv.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_ztpmv.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_ztpsv.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_ztpsv.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_ztrmm.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_ztrmm.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_ztrmv.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_ztrmv.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_ztrsm.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_ztrsm.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/cblas_ztrsv.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/cblas_ztrsv.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/extra/cblas_caxpby.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/extra/cblas_caxpby.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/extra/cblas_cgemm3m.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/extra/cblas_cgemm3m.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/extra/cblas_cgemm_batch.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/extra/cblas_cgemm_batch.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/extra/cblas_cgemmt.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/extra/cblas_cgemmt.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/extra/cblas_daxpby.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/extra/cblas_daxpby.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/extra/cblas_dgemm_batch.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/extra/cblas_dgemm_batch.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/extra/cblas_dgemmt.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/extra/cblas_dgemmt.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/extra/cblas_saxpby.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/extra/cblas_saxpby.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/extra/cblas_sgemm_batch.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/extra/cblas_sgemm_batch.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/extra/cblas_sgemmt.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/extra/cblas_sgemmt.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/extra/cblas_zaxpby.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/extra/cblas_zaxpby.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/extra/cblas_zgemm3m.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/extra/cblas_zgemm3m.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/extra/cblas_zgemm_batch.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/extra/cblas_zgemm_batch.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/cblas/src/extra/cblas_zgemmt.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/cblas/src/extra/cblas_zgemmt.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/check/bla_gemm3m_check.h` & `blis-0.9.1.dev1/blis/_src/frame/compat/check/bla_gemm3m_check.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/check/bla_gemm_check.h` & `blis-0.9.1.dev1/blis/_src/frame/compat/check/bla_gemm_check.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/check/bla_gemmt_check.h` & `blis-0.9.1.dev1/blis/_src/frame/compat/check/bla_gemmt_check.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/check/bla_gemv_check.h` & `blis-0.9.1.dev1/blis/_src/frame/compat/check/bla_gemv_check.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/check/bla_ger_check.h` & `blis-0.9.1.dev1/blis/_src/frame/compat/check/bla_ger_check.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/check/bla_hemm_check.h` & `blis-0.9.1.dev1/blis/_src/frame/compat/check/bla_hemm_check.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/check/bla_hemv_check.h` & `blis-0.9.1.dev1/blis/_src/frame/compat/check/bla_hemv_check.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/check/bla_her2_check.h` & `blis-0.9.1.dev1/blis/_src/frame/compat/check/bla_her2_check.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/check/bla_her2k_check.h` & `blis-0.9.1.dev1/blis/_src/frame/compat/check/bla_her2k_check.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/check/bla_her_check.h` & `blis-0.9.1.dev1/blis/_src/frame/compat/check/bla_her_check.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/check/bla_herk_check.h` & `blis-0.9.1.dev1/blis/_src/frame/compat/check/bla_herk_check.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/check/bla_symm_check.h` & `blis-0.9.1.dev1/blis/_src/frame/compat/check/bla_symm_check.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/check/bla_symv_check.h` & `blis-0.9.1.dev1/blis/_src/frame/compat/check/bla_symv_check.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/check/bla_syr2_check.h` & `blis-0.9.1.dev1/blis/_src/frame/compat/check/bla_syr2_check.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/check/bla_syr2k_check.h` & `blis-0.9.1.dev1/blis/_src/frame/compat/check/bla_syr2k_check.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/check/bla_syr_check.h` & `blis-0.9.1.dev1/blis/_src/frame/compat/check/bla_syr_check.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/check/bla_syrk_check.h` & `blis-0.9.1.dev1/blis/_src/frame/compat/check/bla_syrk_check.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/check/bla_trmm_check.h` & `blis-0.9.1.dev1/blis/_src/frame/compat/check/bla_trmm_check.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/check/bla_trmv_check.h` & `blis-0.9.1.dev1/blis/_src/frame/compat/check/bla_trmv_check.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/check/bla_trsm_check.h` & `blis-0.9.1.dev1/blis/_src/frame/compat/check/bla_trsm_check.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/check/bla_trsv_check.h` & `blis-0.9.1.dev1/blis/_src/frame/compat/check/bla_trsv_check.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/extra/bla_axpby.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/extra/bla_axpby.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/extra/bla_axpby.h` & `blis-0.9.1.dev1/blis/_src/frame/compat/extra/bla_axpby.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/extra/bla_gemm3m.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/extra/bla_gemm3m.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/extra/bla_gemm3m.h` & `blis-0.9.1.dev1/blis/_src/frame/compat/extra/bla_gemm3m.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/extra/bla_gemm_batch.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/extra/bla_gemm_batch.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/extra/bla_gemm_batch.h` & `blis-0.9.1.dev1/blis/_src/frame/compat/extra/bla_gemm_batch.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/extra/bla_gemmt.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/extra/bla_gemmt.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/extra/bla_gemmt.h` & `blis-0.9.1.dev1/blis/_src/frame/compat/extra/bla_gemmt.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/f2c/bla_cabs1.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/f2c/bla_cabs1.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/f2c/bla_cabs1.h` & `blis-0.9.1.dev1/blis/_src/frame/compat/f2c/bla_cabs1.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/f2c/bla_gbmv.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/f2c/bla_gbmv.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/f2c/bla_gbmv.h` & `blis-0.9.1.dev1/blis/_src/frame/compat/f2c/bla_gbmv.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/f2c/bla_hbmv.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/f2c/bla_hbmv.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/f2c/bla_hbmv.h` & `blis-0.9.1.dev1/blis/_src/frame/compat/f2c/bla_hbmv.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/f2c/bla_hpmv.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/f2c/bla_hpmv.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/f2c/bla_hpmv.h` & `blis-0.9.1.dev1/blis/_src/frame/compat/f2c/bla_hpmv.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/f2c/bla_hpr.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/f2c/bla_hpr.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/f2c/bla_hpr.h` & `blis-0.9.1.dev1/blis/_src/frame/compat/f2c/bla_hpr.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/f2c/bla_hpr2.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/f2c/bla_hpr2.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/f2c/bla_hpr2.h` & `blis-0.9.1.dev1/blis/_src/frame/compat/f2c/bla_hpr2.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/f2c/bla_lsame.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/f2c/bla_lsame.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/f2c/bla_lsame.h` & `blis-0.9.1.dev1/blis/_src/frame/compat/f2c/bla_lsame.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/f2c/bla_rot.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/f2c/bla_rot.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/f2c/bla_rot.h` & `blis-0.9.1.dev1/blis/_src/frame/compat/f2c/bla_rot.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/f2c/bla_rotg.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/f2c/bla_rotg.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/f2c/bla_rotg.h` & `blis-0.9.1.dev1/blis/_src/frame/compat/f2c/bla_rotg.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/f2c/bla_rotm.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/f2c/bla_rotm.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/f2c/bla_rotm.h` & `blis-0.9.1.dev1/blis/_src/frame/compat/f2c/bla_rotm.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/f2c/bla_rotmg.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/f2c/bla_rotmg.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/f2c/bla_rotmg.h` & `blis-0.9.1.dev1/blis/_src/frame/compat/f2c/bla_rotmg.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/f2c/bla_sbmv.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/f2c/bla_sbmv.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/f2c/bla_sbmv.h` & `blis-0.9.1.dev1/blis/_src/frame/compat/f2c/bla_sbmv.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/f2c/bla_spmv.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/f2c/bla_spmv.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/f2c/bla_spmv.h` & `blis-0.9.1.dev1/blis/_src/frame/compat/f2c/bla_spmv.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/f2c/bla_spr.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/f2c/bla_spr.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/f2c/bla_spr.h` & `blis-0.9.1.dev1/blis/_src/frame/compat/f2c/bla_spr.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/f2c/bla_spr2.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/f2c/bla_spr2.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/f2c/bla_spr2.h` & `blis-0.9.1.dev1/blis/_src/frame/compat/f2c/bla_spr2.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/f2c/bla_tbmv.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/f2c/bla_tbmv.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/f2c/bla_tbmv.h` & `blis-0.9.1.dev1/blis/_src/frame/compat/f2c/bla_tbmv.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/f2c/bla_tbsv.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/f2c/bla_tbsv.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/f2c/bla_tbsv.h` & `blis-0.9.1.dev1/blis/_src/frame/compat/f2c/bla_tbsv.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/f2c/bla_tpmv.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/f2c/bla_tpmv.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/f2c/bla_tpmv.h` & `blis-0.9.1.dev1/blis/_src/frame/compat/f2c/bla_tpmv.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/f2c/bla_tpsv.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/f2c/bla_tpsv.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/f2c/bla_tpsv.h` & `blis-0.9.1.dev1/blis/_src/frame/compat/f2c/bla_tpsv.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/f2c/bla_xerbla.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/f2c/bla_xerbla.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/f2c/bla_xerbla.h` & `blis-0.9.1.dev1/blis/_src/frame/compat/f2c/bla_xerbla.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/f2c/bla_xerbla_array.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/f2c/bla_xerbla_array.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/f2c/bla_xerbla_array.h` & `blis-0.9.1.dev1/blis/_src/frame/compat/f2c/bla_xerbla_array.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/f2c/util/bla_c_abs.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/f2c/util/bla_c_abs.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/f2c/util/bla_c_abs.h` & `blis-0.9.1.dev1/blis/_src/frame/compat/f2c/util/bla_c_abs.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/f2c/util/bla_c_div.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/f2c/util/bla_c_div.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/f2c/util/bla_c_div.h` & `blis-0.9.1.dev1/blis/_src/frame/compat/f2c/util/bla_c_div.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/f2c/util/bla_d_abs.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/f2c/util/bla_d_abs.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/f2c/util/bla_d_abs.h` & `blis-0.9.1.dev1/blis/_src/frame/compat/f2c/util/bla_d_abs.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/f2c/util/bla_d_cnjg.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/f2c/util/bla_d_cnjg.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/f2c/util/bla_d_cnjg.h` & `blis-0.9.1.dev1/blis/_src/frame/compat/f2c/util/bla_d_cnjg.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/f2c/util/bla_d_imag.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/f2c/util/bla_d_imag.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/f2c/util/bla_d_imag.h` & `blis-0.9.1.dev1/blis/_src/frame/compat/f2c/util/bla_d_imag.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/f2c/util/bla_d_sign.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/f2c/util/bla_d_sign.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/f2c/util/bla_d_sign.h` & `blis-0.9.1.dev1/blis/_src/frame/compat/f2c/util/bla_d_sign.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/f2c/util/bla_f__cabs.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/f2c/util/bla_f__cabs.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/f2c/util/bla_f__cabs.h` & `blis-0.9.1.dev1/blis/_src/frame/compat/f2c/util/bla_f__cabs.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/f2c/util/bla_r_abs.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/f2c/util/bla_r_abs.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/f2c/util/bla_r_abs.h` & `blis-0.9.1.dev1/blis/_src/frame/compat/f2c/util/bla_r_abs.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/f2c/util/bla_r_cnjg.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/f2c/util/bla_r_cnjg.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/f2c/util/bla_r_cnjg.h` & `blis-0.9.1.dev1/blis/_src/frame/compat/f2c/util/bla_r_cnjg.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/f2c/util/bla_r_imag.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/f2c/util/bla_r_imag.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/f2c/util/bla_r_imag.h` & `blis-0.9.1.dev1/blis/_src/frame/compat/f2c/util/bla_r_imag.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/f2c/util/bla_r_sign.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/f2c/util/bla_r_sign.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/f2c/util/bla_r_sign.h` & `blis-0.9.1.dev1/blis/_src/frame/compat/f2c/util/bla_r_sign.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/f2c/util/bla_z_abs.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/f2c/util/bla_z_abs.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/f2c/util/bla_z_abs.h` & `blis-0.9.1.dev1/blis/_src/frame/compat/f2c/util/bla_z_abs.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/f2c/util/bla_z_div.c` & `blis-0.9.1.dev1/blis/_src/frame/compat/f2c/util/bla_z_div.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/compat/f2c/util/bla_z_div.h` & `blis-0.9.1.dev1/blis/_src/frame/compat/f2c/util/bla_z_div.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/bli_arch_config.h` & `blis-0.9.1.dev1/blis/_src/frame/include/bli_arch_config.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/bli_arch_config_pre.h` & `blis-0.9.1.dev1/blis/_src/frame/include/bli_arch_config_pre.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/bli_blas_macro_defs.h` & `blis-0.9.1.dev1/blis/_src/frame/include/bli_blas_macro_defs.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/bli_builtin_macro_defs.h` & `blis-0.9.1.dev1/blis/_src/frame/include/bli_builtin_macro_defs.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/bli_complex_macro_defs.h` & `blis-0.9.1.dev1/blis/_src/frame/include/bli_complex_macro_defs.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/bli_config_macro_defs.h` & `blis-0.9.1.dev1/blis/_src/frame/include/bli_config_macro_defs.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/bli_edge_case_macro_defs.h` & `blis-0.9.1.dev1/blis/_src/frame/include/bli_edge_case_macro_defs.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/bli_error_macro_defs.h` & `blis-0.9.1.dev1/blis/_src/frame/include/bli_error_macro_defs.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/bli_extern_defs.h` & `blis-0.9.1.dev1/blis/_src/frame/include/bli_extern_defs.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/bli_f2c.h` & `blis-0.9.1.dev1/blis/_src/frame/include/bli_f2c.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/bli_genarray_macro_defs.h` & `blis-0.9.1.dev1/blis/_src/frame/include/bli_genarray_macro_defs.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/bli_gentdef_macro_defs.h` & `blis-0.9.1.dev1/blis/_src/frame/include/bli_gentdef_macro_defs.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/bli_gentfunc_macro_defs.h` & `blis-0.9.1.dev1/blis/_src/frame/include/bli_gentfunc_macro_defs.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/bli_gentprot_macro_defs.h` & `blis-0.9.1.dev1/blis/_src/frame/include/bli_gentprot_macro_defs.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/bli_kernel_macro_defs.h` & `blis-0.9.1.dev1/blis/_src/frame/include/bli_kernel_macro_defs.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/bli_lang_defs.h` & `blis-0.9.1.dev1/blis/_src/frame/include/bli_lang_defs.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/bli_macro_defs.h` & `blis-0.9.1.dev1/blis/_src/frame/include/bli_macro_defs.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/bli_misc_macro_defs.h` & `blis-0.9.1.dev1/blis/_src/frame/include/bli_misc_macro_defs.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/bli_oapi_ba.h` & `blis-0.9.1.dev1/blis/_src/frame/include/bli_oapi_ba.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/bli_oapi_ex.h` & `blis-0.9.1.dev1/blis/_src/frame/include/bli_oapi_ex.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/bli_oapi_macro_defs.h` & `blis-0.9.1.dev1/blis/_src/frame/include/bli_oapi_macro_defs.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/bli_obj_macro_defs.h` & `blis-0.9.1.dev1/blis/_src/frame/include/bli_obj_macro_defs.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/bli_param_macro_defs.h` & `blis-0.9.1.dev1/blis/_src/frame/include/bli_param_macro_defs.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/bli_pragma_macro_defs.h` & `blis-0.9.1.dev1/blis/_src/frame/include/bli_pragma_macro_defs.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/bli_sbox.h` & `blis-0.9.1.dev1/blis/_src/frame/include/bli_sbox.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/bli_scalar_macro_defs.h` & `blis-0.9.1.dev1/blis/_src/frame/include/bli_scalar_macro_defs.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/bli_system.h` & `blis-0.9.1.dev1/blis/_src/frame/include/bli_system.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/bli_tapi_ba.h` & `blis-0.9.1.dev1/blis/_src/frame/include/bli_tapi_ba.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/bli_tapi_ex.h` & `blis-0.9.1.dev1/blis/_src/frame/include/bli_tapi_ex.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/bli_tapi_macro_defs.h` & `blis-0.9.1.dev1/blis/_src/frame/include/bli_tapi_macro_defs.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/bli_type_defs.h` & `blis-0.9.1.dev1/blis/_src/frame/include/bli_type_defs.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/bli_x86_asm_macros.h` & `blis-0.9.1.dev1/blis/_src/frame/include/bli_x86_asm_macros.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/bli_xapi_undef.h` & `blis-0.9.1.dev1/blis/_src/frame/include/bli_xapi_undef.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/blis.h` & `blis-0.9.1.dev1/blis/_src/frame/include/blis.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/level0/1e/bli_copy1es.h` & `blis-0.9.1.dev1/blis/_src/frame/include/level0/1e/bli_copy1es.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/level0/1e/bli_copyj1es.h` & `blis-0.9.1.dev1/blis/_src/frame/include/level0/1e/bli_copyj1es.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/level0/1e/bli_invert1es.h` & `blis-0.9.1.dev1/blis/_src/frame/include/level0/1e/bli_invert1es.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/level0/1e/bli_scal1es.h` & `blis-0.9.1.dev1/blis/_src/frame/include/level0/1e/bli_scal1es.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/level0/1e/bli_scal21es.h` & `blis-0.9.1.dev1/blis/_src/frame/include/level0/1e/bli_scal21es.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/level0/1e/bli_scal2j1es.h` & `blis-0.9.1.dev1/blis/_src/frame/include/level0/1e/bli_scal2j1es.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/level0/1m/bli_invert1ms_mxn_diag.h` & `blis-0.9.1.dev1/blis/_src/frame/include/level0/1m/bli_invert1ms_mxn_diag.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/level0/1m/bli_scal1ms_mxn.h` & `blis-0.9.1.dev1/blis/_src/frame/include/level0/1m/bli_scal1ms_mxn.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/level0/1m/bli_scal21ms_mxn.h` & `blis-0.9.1.dev1/blis/_src/frame/include/level0/1m/bli_scal21ms_mxn.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/level0/1m/bli_scal21ms_mxn_diag.h` & `blis-0.9.1.dev1/blis/_src/frame/include/level0/1m/bli_scal21ms_mxn_diag.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/level0/1m/bli_scal21ms_mxn_uplo.h` & `blis-0.9.1.dev1/blis/_src/frame/include/level0/1m/bli_scal21ms_mxn_uplo.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/level0/1m/bli_set1ms_mxn.h` & `blis-0.9.1.dev1/blis/_src/frame/include/level0/1m/bli_set1ms_mxn.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/level0/1m/bli_set1ms_mxn_diag.h` & `blis-0.9.1.dev1/blis/_src/frame/include/level0/1m/bli_set1ms_mxn_diag.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/level0/1m/bli_set1ms_mxn_uplo.h` & `blis-0.9.1.dev1/blis/_src/frame/include/level0/1m/bli_set1ms_mxn_uplo.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/level0/1m/bli_seti01ms_mxn_diag.h` & `blis-0.9.1.dev1/blis/_src/frame/include/level0/1m/bli_seti01ms_mxn_diag.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/level0/1r/bli_copy1rs.h` & `blis-0.9.1.dev1/blis/_src/frame/include/level0/1r/bli_copy1rs.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/level0/1r/bli_copyj1rs.h` & `blis-0.9.1.dev1/blis/_src/frame/include/level0/1r/bli_copyj1rs.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/level0/1r/bli_invert1rs.h` & `blis-0.9.1.dev1/blis/_src/frame/include/level0/1r/bli_invert1rs.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/level0/1r/bli_scal1rs.h` & `blis-0.9.1.dev1/blis/_src/frame/include/level0/1r/bli_scal1rs.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/level0/1r/bli_scal21rs.h` & `blis-0.9.1.dev1/blis/_src/frame/include/level0/1r/bli_scal21rs.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/level0/1r/bli_scal2j1rs.h` & `blis-0.9.1.dev1/blis/_src/frame/include/level0/1r/bli_scal2j1rs.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/level0/bb/bli_bcastbbs_mxn.h` & `blis-0.9.1.dev1/blis/_src/frame/include/level0/bb/bli_bcastbbs_mxn.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/level0/bb/bli_scal2bbs_mxn.h` & `blis-0.9.1.dev1/blis/_src/frame/include/level0/bb/bli_scal2bbs_mxn.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/level0/bb/bli_set0bbs_mxn.h` & `blis-0.9.1.dev1/blis/_src/frame/include/level0/bb/bli_set0bbs_mxn.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/level0/bli_absq2s.h` & `blis-0.9.1.dev1/blis/_src/frame/include/level0/bli_absq2s.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/level0/bli_abval2s.h` & `blis-0.9.1.dev1/blis/_src/frame/include/level0/bli_abval2s.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/level0/bli_add3s.h` & `blis-0.9.1.dev1/blis/_src/frame/include/level0/bli_add3s.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/level0/bli_addjs.h` & `blis-0.9.1.dev1/blis/_src/frame/include/level0/bli_addjs.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/level0/bli_adds.h` & `blis-0.9.1.dev1/blis/_src/frame/include/level0/bli_adds.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/level0/bli_adds_mxn.h` & `blis-0.9.1.dev1/blis/_src/frame/include/level0/bli_adds_mxn.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/level0/bli_adds_mxn_uplo.h` & `blis-0.9.1.dev1/blis/_src/frame/include/level0/bli_adds_mxn_uplo.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/level0/bli_axmys.h` & `blis-0.9.1.dev1/blis/_src/frame/include/level0/bli_axmys.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/level0/bli_axpbyjs.h` & `blis-0.9.1.dev1/blis/_src/frame/include/level0/bli_axpbyjs.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/level0/bli_axpbys.h` & `blis-0.9.1.dev1/blis/_src/frame/include/level0/bli_axpbys.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/level0/bli_axpyjs.h` & `blis-0.9.1.dev1/blis/_src/frame/include/level0/bli_axpyjs.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/level0/bli_axpys.h` & `blis-0.9.1.dev1/blis/_src/frame/include/level0/bli_axpys.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/level0/bli_conjs.h` & `blis-0.9.1.dev1/blis/_src/frame/include/level0/bli_conjs.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/level0/bli_constants.h` & `blis-0.9.1.dev1/blis/_src/frame/include/level0/bli_constants.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/level0/bli_copycjs.h` & `blis-0.9.1.dev1/blis/_src/frame/include/level0/bli_copycjs.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/level0/bli_copyjnzs.h` & `blis-0.9.1.dev1/blis/_src/frame/include/level0/bli_copyjnzs.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/level0/bli_copyjs.h` & `blis-0.9.1.dev1/blis/_src/frame/include/level0/bli_copyjs.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/level0/bli_copynzs.h` & `blis-0.9.1.dev1/blis/_src/frame/include/level0/bli_copynzs.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/level0/bli_copys.h` & `blis-0.9.1.dev1/blis/_src/frame/include/level0/bli_copys.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/level0/bli_copys_mxn.h` & `blis-0.9.1.dev1/blis/_src/frame/include/level0/bli_copys_mxn.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/level0/bli_dotjs.h` & `blis-0.9.1.dev1/blis/_src/frame/include/level0/bli_dotjs.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/level0/bli_dots.h` & `blis-0.9.1.dev1/blis/_src/frame/include/level0/bli_dots.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/level0/bli_eq.h` & `blis-0.9.1.dev1/blis/_src/frame/include/level0/bli_eq.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/level0/bli_fprints.h` & `blis-0.9.1.dev1/blis/_src/frame/include/level0/bli_fprints.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/level0/bli_gets.h` & `blis-0.9.1.dev1/blis/_src/frame/include/level0/bli_gets.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/level0/bli_inverts.h` & `blis-0.9.1.dev1/blis/_src/frame/include/level0/bli_inverts.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/level0/bli_invscaljs.h` & `blis-0.9.1.dev1/blis/_src/frame/include/level0/bli_invscaljs.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/level0/bli_invscals.h` & `blis-0.9.1.dev1/blis/_src/frame/include/level0/bli_invscals.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/level0/bli_neg2s.h` & `blis-0.9.1.dev1/blis/_src/frame/include/level0/bli_neg2s.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/level0/bli_randnp2s.h` & `blis-0.9.1.dev1/blis/_src/frame/include/level0/bli_randnp2s.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/level0/bli_rands.h` & `blis-0.9.1.dev1/blis/_src/frame/include/level0/bli_rands.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/level0/bli_scal2js.h` & `blis-0.9.1.dev1/blis/_src/frame/include/level0/bli_scal2js.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/level0/bli_scal2s.h` & `blis-0.9.1.dev1/blis/_src/frame/include/level0/bli_scal2s.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/level0/bli_scal2s_mxn.h` & `blis-0.9.1.dev1/blis/_src/frame/include/level0/bli_scal2s_mxn.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/level0/bli_scalcjs.h` & `blis-0.9.1.dev1/blis/_src/frame/include/level0/bli_scalcjs.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/level0/bli_scaljs.h` & `blis-0.9.1.dev1/blis/_src/frame/include/level0/bli_scaljs.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/level0/bli_scals.h` & `blis-0.9.1.dev1/blis/_src/frame/include/level0/bli_scals.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/level0/bli_set0s.h` & `blis-0.9.1.dev1/blis/_src/frame/include/level0/bli_set0s.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/level0/bli_set0s_mxn.h` & `blis-0.9.1.dev1/blis/_src/frame/include/level0/bli_set0s_mxn.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/level0/bli_set1s.h` & `blis-0.9.1.dev1/blis/_src/frame/include/level0/bli_set1s.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/level0/bli_seti0s.h` & `blis-0.9.1.dev1/blis/_src/frame/include/level0/bli_seti0s.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/level0/bli_setis.h` & `blis-0.9.1.dev1/blis/_src/frame/include/level0/bli_setis.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/level0/bli_setrs.h` & `blis-0.9.1.dev1/blis/_src/frame/include/level0/bli_setrs.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/level0/bli_sets.h` & `blis-0.9.1.dev1/blis/_src/frame/include/level0/bli_sets.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/level0/bli_sqrt2s.h` & `blis-0.9.1.dev1/blis/_src/frame/include/level0/bli_sqrt2s.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/level0/bli_subjs.h` & `blis-0.9.1.dev1/blis/_src/frame/include/level0/bli_subjs.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/level0/bli_subs.h` & `blis-0.9.1.dev1/blis/_src/frame/include/level0/bli_subs.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/level0/bli_swaps.h` & `blis-0.9.1.dev1/blis/_src/frame/include/level0/bli_swaps.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/level0/bli_xpbyjs.h` & `blis-0.9.1.dev1/blis/_src/frame/include/level0/bli_xpbyjs.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/level0/bli_xpbys.h` & `blis-0.9.1.dev1/blis/_src/frame/include/level0/bli_xpbys.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/level0/bli_xpbys_mxn.h` & `blis-0.9.1.dev1/blis/_src/frame/include/level0/bli_xpbys_mxn.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/level0/bli_xpbys_mxn_uplo.h` & `blis-0.9.1.dev1/blis/_src/frame/include/level0/bli_xpbys_mxn_uplo.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/level0/old/bli_cast.h` & `blis-0.9.1.dev1/blis/_src/frame/include/level0/old/bli_cast.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/level0/old/bli_castfrom.h` & `blis-0.9.1.dev1/blis/_src/frame/include/level0/old/bli_castfrom.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/level0/old/bli_castto.h` & `blis-0.9.1.dev1/blis/_src/frame/include/level0/old/bli_castto.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/level0/old/bli_copynzjs.h` & `blis-0.9.1.dev1/blis/_src/frame/include/level0/old/bli_copynzjs.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/level0/old/bli_copynzs.h` & `blis-0.9.1.dev1/blis/_src/frame/include/level0/old/bli_copynzs.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/level0/old/bli_invscalcjs.h` & `blis-0.9.1.dev1/blis/_src/frame/include/level0/old/bli_invscalcjs.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/level0/old/bli_scalcjs.h` & `blis-0.9.1.dev1/blis/_src/frame/include/level0/old/bli_scalcjs.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/level0/old/bli_set0ris_mxn.h` & `blis-0.9.1.dev1/blis/_src/frame/include/level0/old/bli_set0ris_mxn.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/level0/old/io/bli_scal2ios.h` & `blis-0.9.1.dev1/blis/_src/frame/include/level0/old/io/bli_scal2ios.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/level0/old/io/bli_scal2jios.h` & `blis-0.9.1.dev1/blis/_src/frame/include/level0/old/io/bli_scal2jios.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/level0/old/ri3/bli_copyjri3s.h` & `blis-0.9.1.dev1/blis/_src/frame/include/level0/old/ri3/bli_copyjri3s.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/level0/old/ri3/bli_copyri3s.h` & `blis-0.9.1.dev1/blis/_src/frame/include/level0/old/ri3/bli_copyri3s.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/level0/old/ri3/bli_scal2jri3s.h` & `blis-0.9.1.dev1/blis/_src/frame/include/level0/old/ri3/bli_scal2jri3s.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/level0/old/ri3/bli_scal2ri3s.h` & `blis-0.9.1.dev1/blis/_src/frame/include/level0/old/ri3/bli_scal2ri3s.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/level0/old/ri3/bli_scal2ri3s_mxn.h` & `blis-0.9.1.dev1/blis/_src/frame/include/level0/old/ri3/bli_scal2ri3s_mxn.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/level0/old/rih/bli_scal2rihs_mxn.h` & `blis-0.9.1.dev1/blis/_src/frame/include/level0/old/rih/bli_scal2rihs_mxn.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/level0/old/rih/bli_scal2rihs_mxn_diag.h` & `blis-0.9.1.dev1/blis/_src/frame/include/level0/old/rih/bli_scal2rihs_mxn_diag.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/level0/old/rih/bli_scal2rihs_mxn_uplo.h` & `blis-0.9.1.dev1/blis/_src/frame/include/level0/old/rih/bli_scal2rihs_mxn_uplo.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/level0/old/rih/bli_setrihs_mxn_diag.h` & `blis-0.9.1.dev1/blis/_src/frame/include/level0/old/rih/bli_setrihs_mxn_diag.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/level0/old/ro/bli_scal2jros.h` & `blis-0.9.1.dev1/blis/_src/frame/include/level0/old/ro/bli_scal2jros.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/level0/old/ro/bli_scal2ros.h` & `blis-0.9.1.dev1/blis/_src/frame/include/level0/old/ro/bli_scal2ros.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/level0/old/rpi/bli_scal2jrpis.h` & `blis-0.9.1.dev1/blis/_src/frame/include/level0/old/rpi/bli_scal2jrpis.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/level0/old/rpi/bli_scal2rpis.h` & `blis-0.9.1.dev1/blis/_src/frame/include/level0/old/rpi/bli_scal2rpis.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/level0/ri/bli_absq2ris.h` & `blis-0.9.1.dev1/blis/_src/frame/include/level0/ri/bli_absq2ris.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/level0/ri/bli_abval2ris.h` & `blis-0.9.1.dev1/blis/_src/frame/include/level0/ri/bli_abval2ris.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/level0/ri/bli_add3ris.h` & `blis-0.9.1.dev1/blis/_src/frame/include/level0/ri/bli_add3ris.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/level0/ri/bli_addjris.h` & `blis-0.9.1.dev1/blis/_src/frame/include/level0/ri/bli_addjris.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/level0/ri/bli_addris.h` & `blis-0.9.1.dev1/blis/_src/frame/include/level0/ri/bli_addris.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/level0/ri/bli_axmyris.h` & `blis-0.9.1.dev1/blis/_src/frame/include/level0/ri/bli_axmyris.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/level0/ri/bli_axpbyjris.h` & `blis-0.9.1.dev1/blis/_src/frame/include/level0/ri/bli_axpbyjris.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/level0/ri/bli_axpbyris.h` & `blis-0.9.1.dev1/blis/_src/frame/include/level0/ri/bli_axpbyris.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/level0/ri/bli_axpyjris.h` & `blis-0.9.1.dev1/blis/_src/frame/include/level0/ri/bli_axpyjris.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/level0/ri/bli_axpyris.h` & `blis-0.9.1.dev1/blis/_src/frame/include/level0/ri/bli_axpyris.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/level0/ri/bli_conjris.h` & `blis-0.9.1.dev1/blis/_src/frame/include/level0/ri/bli_conjris.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/level0/ri/bli_copycjris.h` & `blis-0.9.1.dev1/blis/_src/frame/include/level0/ri/bli_copycjris.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/level0/ri/bli_copyjris.h` & `blis-0.9.1.dev1/blis/_src/frame/include/level0/ri/bli_copyjris.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/level0/ri/bli_copyris.h` & `blis-0.9.1.dev1/blis/_src/frame/include/level0/ri/bli_copyris.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/level0/ri/bli_eqris.h` & `blis-0.9.1.dev1/blis/_src/frame/include/level0/ri/bli_eqris.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/level0/ri/bli_invertris.h` & `blis-0.9.1.dev1/blis/_src/frame/include/level0/ri/bli_invertris.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/level0/ri/bli_invscaljris.h` & `blis-0.9.1.dev1/blis/_src/frame/include/level0/ri/bli_invscaljris.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/level0/ri/bli_invscalris.h` & `blis-0.9.1.dev1/blis/_src/frame/include/level0/ri/bli_invscalris.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/level0/ri/bli_neg2ris.h` & `blis-0.9.1.dev1/blis/_src/frame/include/level0/ri/bli_neg2ris.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/level0/ri/bli_scal2jris.h` & `blis-0.9.1.dev1/blis/_src/frame/include/level0/ri/bli_scal2jris.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/level0/ri/bli_scal2ris.h` & `blis-0.9.1.dev1/blis/_src/frame/include/level0/ri/bli_scal2ris.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/level0/ri/bli_scal2ris_mxn.h` & `blis-0.9.1.dev1/blis/_src/frame/include/level0/ri/bli_scal2ris_mxn.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/level0/ri/bli_scalcjris.h` & `blis-0.9.1.dev1/blis/_src/frame/include/level0/ri/bli_scalcjris.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/level0/ri/bli_scaljris.h` & `blis-0.9.1.dev1/blis/_src/frame/include/level0/ri/bli_scaljris.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/level0/ri/bli_scalris.h` & `blis-0.9.1.dev1/blis/_src/frame/include/level0/ri/bli_scalris.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/level0/ri/bli_scalris_mxn_uplo.h` & `blis-0.9.1.dev1/blis/_src/frame/include/level0/ri/bli_scalris_mxn_uplo.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/level0/ri/bli_set0ris.h` & `blis-0.9.1.dev1/blis/_src/frame/include/level0/ri/bli_set0ris.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/level0/ri/bli_sqrt2ris.h` & `blis-0.9.1.dev1/blis/_src/frame/include/level0/ri/bli_sqrt2ris.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/level0/ri/bli_subjris.h` & `blis-0.9.1.dev1/blis/_src/frame/include/level0/ri/bli_subjris.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/level0/ri/bli_subris.h` & `blis-0.9.1.dev1/blis/_src/frame/include/level0/ri/bli_subris.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/level0/ri/bli_swapris.h` & `blis-0.9.1.dev1/blis/_src/frame/include/level0/ri/bli_swapris.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/level0/ri/bli_xpbyjris.h` & `blis-0.9.1.dev1/blis/_src/frame/include/level0/ri/bli_xpbyjris.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/include/level0/ri/bli_xpbyris.h` & `blis-0.9.1.dev1/blis/_src/frame/include/level0/ri/bli_xpbyris.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/thread/bli_l3_decor.h` & `blis-0.9.1.dev1/blis/_src/frame/thread/bli_l3_decor.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/thread/bli_l3_decor_openmp.c` & `blis-0.9.1.dev1/blis/_src/frame/thread/bli_l3_decor_openmp.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/thread/bli_l3_decor_openmp.h` & `blis-0.9.1.dev1/blis/_src/frame/thread/bli_l3_decor_openmp.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/thread/bli_l3_decor_pthreads.c` & `blis-0.9.1.dev1/blis/_src/frame/thread/bli_l3_decor_pthreads.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/thread/bli_l3_decor_pthreads.h` & `blis-0.9.1.dev1/blis/_src/frame/thread/bli_l3_decor_pthreads.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/thread/bli_l3_decor_single.c` & `blis-0.9.1.dev1/blis/_src/frame/thread/bli_l3_decor_single.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/thread/bli_l3_decor_single.h` & `blis-0.9.1.dev1/blis/_src/frame/thread/bli_l3_decor_single.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/thread/bli_l3_sup_decor.h` & `blis-0.9.1.dev1/blis/_src/frame/thread/bli_l3_sup_decor.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/thread/bli_l3_sup_decor_openmp.c` & `blis-0.9.1.dev1/blis/_src/frame/thread/bli_l3_sup_decor_openmp.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/thread/bli_l3_sup_decor_openmp.h` & `blis-0.9.1.dev1/blis/_src/frame/thread/bli_l3_sup_decor_openmp.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/thread/bli_l3_sup_decor_pthreads.c` & `blis-0.9.1.dev1/blis/_src/frame/thread/bli_l3_sup_decor_pthreads.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/thread/bli_l3_sup_decor_pthreads.h` & `blis-0.9.1.dev1/blis/_src/frame/thread/bli_l3_sup_decor_pthreads.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/thread/bli_l3_sup_decor_single.c` & `blis-0.9.1.dev1/blis/_src/frame/thread/bli_l3_sup_decor_single.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/thread/bli_l3_sup_decor_single.h` & `blis-0.9.1.dev1/blis/_src/frame/thread/bli_l3_sup_decor_single.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/thread/bli_pthread.c` & `blis-0.9.1.dev1/blis/_src/frame/thread/bli_pthread.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/thread/bli_pthread.h` & `blis-0.9.1.dev1/blis/_src/frame/thread/bli_pthread.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/thread/bli_thrcomm.c` & `blis-0.9.1.dev1/blis/_src/frame/thread/bli_thrcomm.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/thread/bli_thrcomm.h` & `blis-0.9.1.dev1/blis/_src/frame/thread/bli_thrcomm.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/thread/bli_thrcomm_openmp.c` & `blis-0.9.1.dev1/blis/_src/frame/thread/bli_thrcomm_openmp.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/thread/bli_thrcomm_openmp.h` & `blis-0.9.1.dev1/blis/_src/frame/thread/bli_thrcomm_openmp.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/thread/bli_thrcomm_pthreads.c` & `blis-0.9.1.dev1/blis/_src/frame/thread/bli_thrcomm_pthreads.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/thread/bli_thrcomm_pthreads.h` & `blis-0.9.1.dev1/blis/_src/frame/thread/bli_thrcomm_pthreads.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/thread/bli_thrcomm_single.c` & `blis-0.9.1.dev1/blis/_src/frame/thread/bli_thrcomm_single.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/thread/bli_thrcomm_single.h` & `blis-0.9.1.dev1/blis/_src/frame/thread/bli_thrcomm_single.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/thread/bli_thread.c` & `blis-0.9.1.dev1/blis/_src/frame/thread/bli_thread.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/thread/bli_thread.h` & `blis-0.9.1.dev1/blis/_src/frame/thread/bli_thread.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/thread/bli_thrinfo.c` & `blis-0.9.1.dev1/blis/_src/frame/thread/bli_thrinfo.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/thread/bli_thrinfo.h` & `blis-0.9.1.dev1/blis/_src/frame/thread/bli_thrinfo.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/thread/bli_thrinfo_sup.c` & `blis-0.9.1.dev1/blis/_src/frame/thread/bli_thrinfo_sup.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/thread/bli_thrinfo_sup.h` & `blis-0.9.1.dev1/blis/_src/frame/thread/bli_thrinfo_sup.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/thread/old/bli_mutex.h` & `blis-0.9.1.dev1/blis/_src/frame/thread/old/bli_mutex.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/thread/old/bli_mutex_openmp.h` & `blis-0.9.1.dev1/blis/_src/frame/thread/old/bli_mutex_openmp.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/thread/old/bli_mutex_pthreads.h` & `blis-0.9.1.dev1/blis/_src/frame/thread/old/bli_mutex_pthreads.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/thread/old/bli_mutex_single.h` & `blis-0.9.1.dev1/blis/_src/frame/thread/old/bli_mutex_single.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/util/bli_util.h` & `blis-0.9.1.dev1/blis/_src/frame/util/bli_util.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/util/bli_util_check.c` & `blis-0.9.1.dev1/blis/_src/frame/util/bli_util_check.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/util/bli_util_check.h` & `blis-0.9.1.dev1/blis/_src/frame/util/bli_util_check.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/util/bli_util_fpa.c` & `blis-0.9.1.dev1/blis/_src/frame/util/bli_util_fpa.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/util/bli_util_fpa.h` & `blis-0.9.1.dev1/blis/_src/frame/util/bli_util_fpa.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/util/bli_util_ft.h` & `blis-0.9.1.dev1/blis/_src/frame/util/bli_util_ft.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/util/bli_util_oapi.c` & `blis-0.9.1.dev1/blis/_src/frame/util/bli_util_oapi.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/util/bli_util_oapi.h` & `blis-0.9.1.dev1/blis/_src/frame/util/bli_util_oapi.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/util/bli_util_oapi_ba.c` & `blis-0.9.1.dev1/blis/_src/frame/util/bli_util_oapi_ba.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/util/bli_util_oapi_ex.c` & `blis-0.9.1.dev1/blis/_src/frame/util/bli_util_oapi_ex.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/util/bli_util_tapi.c` & `blis-0.9.1.dev1/blis/_src/frame/util/bli_util_tapi.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/util/bli_util_tapi.h` & `blis-0.9.1.dev1/blis/_src/frame/util/bli_util_tapi.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/util/bli_util_tapi_ba.c` & `blis-0.9.1.dev1/blis/_src/frame/util/bli_util_tapi_ba.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/util/bli_util_tapi_ex.c` & `blis-0.9.1.dev1/blis/_src/frame/util/bli_util_tapi_ex.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/util/bli_util_unb_var1.c` & `blis-0.9.1.dev1/blis/_src/frame/util/bli_util_unb_var1.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/frame/util/bli_util_unb_var1.h` & `blis-0.9.1.dev1/blis/_src/frame/util/bli_util_unb_var1.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/include/darwin-firestorm/blis.h` & `blis-0.9.1.dev1/blis/_src/include/darwin-firestorm/blis.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/include/darwin-generic/blis.h` & `blis-0.9.1.dev1/blis/_src/include/darwin-generic/blis.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/include/darwin-x86_64/blis.h` & `blis-0.9.1.dev1/blis/_src/include/darwin-x86_64/blis.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/include/darwin-x86_64_no_skx/blis.h` & `blis-0.9.1.dev1/blis/_src/include/darwin-x86_64_no_skx/blis.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/include/darwin-x86_64_no_zen2/blis.h` & `blis-0.9.1.dev1/blis/_src/include/darwin-x86_64_no_zen2/blis.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/include/darwin-x86_64_no_zen3/blis.h` & `blis-0.9.1.dev1/blis/_src/include/darwin-x86_64_no_zen3/blis.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/include/linux-arm64/blis.h` & `blis-0.9.1.dev1/blis/_src/include/linux-arm64/blis.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/include/linux-arm64_no_sve/blis.h` & `blis-0.9.1.dev1/blis/_src/include/linux-arm64_no_sve/blis.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/include/linux-generic/blis.h` & `blis-0.9.1.dev1/blis/_src/include/linux-generic/blis.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/include/linux-power9/blis.h` & `blis-0.9.1.dev1/blis/_src/include/linux-power9/blis.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/include/linux-x86_64/blis.h` & `blis-0.9.1.dev1/blis/_src/include/linux-x86_64/blis.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/include/linux-x86_64_no_skx/blis.h` & `blis-0.9.1.dev1/blis/_src/include/linux-x86_64_no_skx/blis.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/include/linux-x86_64_no_zen2/blis.h` & `blis-0.9.1.dev1/blis/_src/include/linux-x86_64_no_zen2/blis.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/include/linux-x86_64_no_zen3/blis.h` & `blis-0.9.1.dev1/blis/_src/include/linux-x86_64_no_zen3/blis.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/include/windows-generic/blis.h` & `blis-0.9.1.dev1/blis/_src/include/windows-generic/blis.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/include/windows-x86_64/blis.h` & `blis-0.9.1.dev1/blis/_src/include/windows-x86_64/blis.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/armsve/1m/armsve512_asm_transpose_d8x2.h` & `blis-0.9.1.dev1/blis/_src/kernels/armsve/1m/armsve512_asm_transpose_d8x2.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/armsve/1m/armsve512_asm_transpose_d8x8.h` & `blis-0.9.1.dev1/blis/_src/kernels/armsve/1m/armsve512_asm_transpose_d8x8.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/armsve/1m/bli_dpackm_armsve256_int_8xk.c` & `blis-0.9.1.dev1/blis/_src/kernels/armsve/1m/bli_dpackm_armsve256_int_8xk.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/armsve/1m/bli_dpackm_armsve512_asm_10xk.c` & `blis-0.9.1.dev1/blis/_src/kernels/armsve/1m/bli_dpackm_armsve512_asm_10xk.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/armsve/1m/bli_dpackm_armsve512_asm_16xk.c` & `blis-0.9.1.dev1/blis/_src/kernels/armsve/1m/bli_dpackm_armsve512_asm_16xk.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/armsve/1m/old/bli_dpackm_armsve512_int_12xk.c` & `blis-0.9.1.dev1/blis/_src/kernels/armsve/1m/old/bli_dpackm_armsve512_int_12xk.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/armsve/3/armsve_asm_2vx10.h` & `blis-0.9.1.dev1/blis/_src/kernels/armsve/3/armsve_asm_2vx10.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/armsve/3/armsve_asm_2vx10cmplx.h` & `blis-0.9.1.dev1/blis/_src/kernels/armsve/3/armsve_asm_2vx10cmplx.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/armsve/3/armsve_asm_macros.h` & `blis-0.9.1.dev1/blis/_src/kernels/armsve/3/armsve_asm_macros.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/armsve/3/armsve_asm_macros_cmplx.h` & `blis-0.9.1.dev1/blis/_src/kernels/armsve/3/armsve_asm_macros_cmplx.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/armsve/3/armsve_asm_macros_dcomplex.h` & `blis-0.9.1.dev1/blis/_src/kernels/armsve/3/armsve_asm_macros_dcomplex.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/armsve/3/armsve_asm_macros_double.h` & `blis-0.9.1.dev1/blis/_src/kernels/armsve/3/armsve_asm_macros_double.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/armsve/3/armsve_asm_macros_scomplex.h` & `blis-0.9.1.dev1/blis/_src/kernels/armsve/3/armsve_asm_macros_scomplex.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/armsve/3/armsve_asm_macros_single.h` & `blis-0.9.1.dev1/blis/_src/kernels/armsve/3/armsve_asm_macros_single.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/armsve/3/bli_armsve_utils.c` & `blis-0.9.1.dev1/blis/_src/kernels/armsve/3/bli_armsve_utils.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/armsve/3/bli_armsve_utils.h` & `blis-0.9.1.dev1/blis/_src/kernels/armsve/3/bli_armsve_utils.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/armsve/3/bli_gemm_armsve_asm_c2vx10_unindexed.c` & `blis-0.9.1.dev1/blis/_src/kernels/armsve/3/bli_gemm_armsve_asm_c2vx10_unindexed.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/armsve/3/bli_gemm_armsve_asm_d2vx10_unindexed.c` & `blis-0.9.1.dev1/blis/_src/kernels/armsve/3/bli_gemm_armsve_asm_d2vx10_unindexed.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/armsve/3/bli_gemm_armsve_asm_s2vx10_unindexed.c` & `blis-0.9.1.dev1/blis/_src/kernels/armsve/3/bli_gemm_armsve_asm_s2vx10_unindexed.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/armsve/3/bli_gemm_armsve_asm_z2vx10_unindexed.c` & `blis-0.9.1.dev1/blis/_src/kernels/armsve/3/bli_gemm_armsve_asm_z2vx10_unindexed.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/armsve/3/old/armsve_asm_2vx7cmplx.h` & `blis-0.9.1.dev1/blis/_src/kernels/armsve/3/old/armsve_asm_2vx7cmplx.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/armsve/3/old/armsve_asm_2vx8cmplx.h` & `blis-0.9.1.dev1/blis/_src/kernels/armsve/3/old/armsve_asm_2vx8cmplx.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/armsve/3/old/armsve_asm_macros_half.h` & `blis-0.9.1.dev1/blis/_src/kernels/armsve/3/old/armsve_asm_macros_half.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/armsve/3/old/bli_gemm_armsve256_asm_d8x8.c` & `blis-0.9.1.dev1/blis/_src/kernels/armsve/3/old/bli_gemm_armsve256_asm_d8x8.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/armsve/3/old/bli_gemm_armsve_asm_sh2vx10_unindexed.c` & `blis-0.9.1.dev1/blis/_src/kernels/armsve/3/old/bli_gemm_armsve_asm_sh2vx10_unindexed.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/armsve/3/old/bli_gemm_armsve_asm_z2vx7_unindexed.c` & `blis-0.9.1.dev1/blis/_src/kernels/armsve/3/old/bli_gemm_armsve_asm_z2vx7_unindexed.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/armsve/3/old/bli_gemm_armsve_asm_z2vx8_unindexed.c` & `blis-0.9.1.dev1/blis/_src/kernels/armsve/3/old/bli_gemm_armsve_asm_z2vx8_unindexed.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/armsve/3/old/sup/bli_gemmsup_armsve_ref.c` & `blis-0.9.1.dev1/blis/_src/kernels/armsve/3/old/sup/bli_gemmsup_armsve_ref.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/armsve/3/old/sup/bli_gemmsup_cv_armsve_asm_d2vx10_unindexed.c` & `blis-0.9.1.dev1/blis/_src/kernels/armsve/3/old/sup/bli_gemmsup_cv_armsve_asm_d2vx10_unindexed.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/armsve/3/old/sup/bli_gemmsup_rv_armsve_asm_d2vx10_unindexed.c` & `blis-0.9.1.dev1/blis/_src/kernels/armsve/3/old/sup/bli_gemmsup_rv_armsve_asm_d2vx10_unindexed.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/armsve/bli_kernels_armsve.h` & `blis-0.9.1.dev1/blis/_src/kernels/armsve/bli_kernels_armsve.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/armv7a/3/bli_gemm_armv7a_asm_d4x4.c` & `blis-0.9.1.dev1/blis/_src/kernels/armv7a/3/bli_gemm_armv7a_asm_d4x4.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/armv7a/3/bli_gemm_armv7a_int_d4x4.c` & `blis-0.9.1.dev1/blis/_src/kernels/armv7a/3/bli_gemm_armv7a_int_d4x4.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/armv7a/bli_kernels_armv7a.h` & `blis-0.9.1.dev1/blis/_src/kernels/armv7a/bli_kernels_armv7a.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/armv8a/1m/bli_packm_armv8a_int_d6xk.c` & `blis-0.9.1.dev1/blis/_src/kernels/armv8a/1m/bli_packm_armv8a_int_d6xk.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/armv8a/1m/bli_packm_armv8a_int_d8xk.c` & `blis-0.9.1.dev1/blis/_src/kernels/armv8a/1m/bli_packm_armv8a_int_d8xk.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/armv8a/1m/bli_packm_armv8a_int_s12xk.c` & `blis-0.9.1.dev1/blis/_src/kernels/armv8a/1m/bli_packm_armv8a_int_s12xk.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/armv8a/1m/bli_packm_armv8a_int_s8xk.c` & `blis-0.9.1.dev1/blis/_src/kernels/armv8a/1m/bli_packm_armv8a_int_s8xk.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/armv8a/3/armv8a_asm_d2x2.h` & `blis-0.9.1.dev1/blis/_src/kernels/armv8a/3/armv8a_asm_d2x2.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/armv8a/3/armv8a_asm_utils.h` & `blis-0.9.1.dev1/blis/_src/kernels/armv8a/3/armv8a_asm_utils.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/armv8a/3/bli_gemm_armv8a_asm_d6x8.c` & `blis-0.9.1.dev1/blis/_src/kernels/armv8a/3/bli_gemm_armv8a_asm_d6x8.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/armv8a/3/old/bli_gemm_armv8a_asm_d4x4.c` & `blis-0.9.1.dev1/blis/_src/kernels/armv8a/3/old/bli_gemm_armv8a_asm_d4x4.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/armv8a/3/old/bli_gemm_armv8a_asm_d6x8r.c` & `blis-0.9.1.dev1/blis/_src/kernels/armv8a/3/old/bli_gemm_armv8a_asm_d6x8r.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/armv8a/3/old/bli_gemm_armv8a_asm_d8x4.c` & `blis-0.9.1.dev1/blis/_src/kernels/armv8a/3/old/bli_gemm_armv8a_asm_d8x4.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/armv8a/3/sup/bli_gemmsup_armv8a_ref.c` & `blis-0.9.1.dev1/blis/_src/kernels/armv8a/3/sup/bli_gemmsup_armv8a_ref.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/armv8a/3/sup/bli_gemmsup_rd_armv8a_asm_d6x8m.c` & `blis-0.9.1.dev1/blis/_src/kernels/armv8a/3/sup/bli_gemmsup_rd_armv8a_asm_d6x8m.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/armv8a/3/sup/bli_gemmsup_rd_armv8a_asm_d6x8n.c` & `blis-0.9.1.dev1/blis/_src/kernels/armv8a/3/sup/bli_gemmsup_rd_armv8a_asm_d6x8n.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/armv8a/3/sup/bli_gemmsup_rv_armv8a_asm_d4x8m.c` & `blis-0.9.1.dev1/blis/_src/kernels/armv8a/3/sup/bli_gemmsup_rv_armv8a_asm_d4x8m.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/armv8a/3/sup/bli_gemmsup_rv_armv8a_asm_d4x8n.c` & `blis-0.9.1.dev1/blis/_src/kernels/armv8a/3/sup/bli_gemmsup_rv_armv8a_asm_d4x8n.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/armv8a/3/sup/bli_gemmsup_rv_armv8a_asm_d6x8m.c` & `blis-0.9.1.dev1/blis/_src/kernels/armv8a/3/sup/bli_gemmsup_rv_armv8a_asm_d6x8m.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/armv8a/3/sup/bli_gemmsup_rv_armv8a_asm_d6x8n.c` & `blis-0.9.1.dev1/blis/_src/kernels/armv8a/3/sup/bli_gemmsup_rv_armv8a_asm_d6x8n.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/armv8a/3/sup/bli_gemmsup_rv_armv8a_asm_d8x4m.c` & `blis-0.9.1.dev1/blis/_src/kernels/armv8a/3/sup/bli_gemmsup_rv_armv8a_asm_d8x4m.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/armv8a/3/sup/d3x4/bli_gemmsup_rd_armv8a_asm_d3x4.c` & `blis-0.9.1.dev1/blis/_src/kernels/armv8a/3/sup/d3x4/bli_gemmsup_rd_armv8a_asm_d3x4.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/armv8a/3/sup/d3x4/bli_gemmsup_rd_armv8a_asm_d6x3.c` & `blis-0.9.1.dev1/blis/_src/kernels/armv8a/3/sup/d3x4/bli_gemmsup_rd_armv8a_asm_d6x3.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/armv8a/3/sup/d3x4/bli_gemmsup_rd_armv8a_int_d2x8.c` & `blis-0.9.1.dev1/blis/_src/kernels/armv8a/3/sup/d3x4/bli_gemmsup_rd_armv8a_int_d2x8.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/armv8a/3/sup/d3x4/bli_gemmsup_rd_armv8a_int_d3x4.c` & `blis-0.9.1.dev1/blis/_src/kernels/armv8a/3/sup/d3x4/bli_gemmsup_rd_armv8a_int_d3x4.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/armv8a/3/sup/d6x4/bli_gemmsup_rv_armv8a_int_d3x8mn.c` & `blis-0.9.1.dev1/blis/_src/kernels/armv8a/3/sup/d6x4/bli_gemmsup_rv_armv8a_int_d3x8mn.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/armv8a/3/sup/d6x4/bli_gemmsup_rv_armv8a_int_d6x4mn.c` & `blis-0.9.1.dev1/blis/_src/kernels/armv8a/3/sup/d6x4/bli_gemmsup_rv_armv8a_int_d6x4mn.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/armv8a/bli_kernels_armv8a.h` & `blis-0.9.1.dev1/blis/_src/kernels/armv8a/bli_kernels_armv8a.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/bgq/1/bli_axpyv_bgq_int.c` & `blis-0.9.1.dev1/blis/_src/kernels/bgq/1/bli_axpyv_bgq_int.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/bgq/1/bli_dotv_bgq_int.c` & `blis-0.9.1.dev1/blis/_src/kernels/bgq/1/bli_dotv_bgq_int.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/bgq/1f/bli_axpyf_bgq_int.c` & `blis-0.9.1.dev1/blis/_src/kernels/bgq/1f/bli_axpyf_bgq_int.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/bgq/3/bli_gemm_bgq_int_8x8.c` & `blis-0.9.1.dev1/blis/_src/kernels/bgq/3/bli_gemm_bgq_int_8x8.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/bgq/bli_kernels_bgq.h` & `blis-0.9.1.dev1/blis/_src/kernels/bgq/bli_kernels_bgq.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/bulldozer/3/bli_gemm_bulldozer_asm_d4x6_fma4.c` & `blis-0.9.1.dev1/blis/_src/kernels/bulldozer/3/bli_gemm_bulldozer_asm_d4x6_fma4.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/bulldozer/bli_kernels_bulldozer.h` & `blis-0.9.1.dev1/blis/_src/kernels/bulldozer/bli_kernels_bulldozer.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/haswell/1m/bli_packm_haswell_asm_c3xk.c` & `blis-0.9.1.dev1/blis/_src/kernels/haswell/1m/bli_packm_haswell_asm_c3xk.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/haswell/1m/bli_packm_haswell_asm_c8xk.c` & `blis-0.9.1.dev1/blis/_src/kernels/haswell/1m/bli_packm_haswell_asm_c8xk.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/haswell/1m/bli_packm_haswell_asm_d6xk.c` & `blis-0.9.1.dev1/blis/_src/kernels/haswell/1m/bli_packm_haswell_asm_d6xk.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/haswell/1m/bli_packm_haswell_asm_d8xk.c` & `blis-0.9.1.dev1/blis/_src/kernels/haswell/1m/bli_packm_haswell_asm_d8xk.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/haswell/1m/bli_packm_haswell_asm_s16xk.c` & `blis-0.9.1.dev1/blis/_src/kernels/haswell/1m/bli_packm_haswell_asm_s16xk.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/haswell/1m/bli_packm_haswell_asm_s6xk.c` & `blis-0.9.1.dev1/blis/_src/kernels/haswell/1m/bli_packm_haswell_asm_s6xk.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/haswell/1m/bli_packm_haswell_asm_z3xk.c` & `blis-0.9.1.dev1/blis/_src/kernels/haswell/1m/bli_packm_haswell_asm_z3xk.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/haswell/1m/bli_packm_haswell_asm_z4xk.c` & `blis-0.9.1.dev1/blis/_src/kernels/haswell/1m/bli_packm_haswell_asm_z4xk.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/haswell/3/bli_gemm_haswell_asm_d6x8.c` & `blis-0.9.1.dev1/blis/_src/kernels/haswell/3/bli_gemm_haswell_asm_d6x8.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/haswell/3/bli_gemm_haswell_asm_d8x6.c` & `blis-0.9.1.dev1/blis/_src/kernels/haswell/3/bli_gemm_haswell_asm_d8x6.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/haswell/3/bli_gemmtrsm_l_haswell_asm_d6x8.c` & `blis-0.9.1.dev1/blis/_src/kernels/haswell/3/bli_gemmtrsm_l_haswell_asm_d6x8.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/haswell/3/bli_gemmtrsm_u_haswell_asm_d6x8.c` & `blis-0.9.1.dev1/blis/_src/kernels/haswell/3/bli_gemmtrsm_u_haswell_asm_d6x8.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/haswell/3/old/bli_gemm_haswell_asm_d12x4.c` & `blis-0.9.1.dev1/blis/_src/kernels/haswell/3/old/bli_gemm_haswell_asm_d12x4.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/haswell/3/old/bli_gemm_haswell_asm_d4x12.c` & `blis-0.9.1.dev1/blis/_src/kernels/haswell/3/old/bli_gemm_haswell_asm_d4x12.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/haswell/3/old/bli_gemm_haswell_asm_d6x8.c` & `blis-0.9.1.dev1/blis/_src/kernels/haswell/3/old/bli_gemm_haswell_asm_d6x8.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/haswell/3/old/bli_gemm_haswell_asm_d8x6.c` & `blis-0.9.1.dev1/blis/_src/kernels/haswell/3/old/bli_gemm_haswell_asm_d8x6.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/haswell/3/sup/bli_gemmsup_rd_haswell_asm_d6x8m.c` & `blis-0.9.1.dev1/blis/_src/kernels/haswell/3/sup/bli_gemmsup_rd_haswell_asm_d6x8m.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/haswell/3/sup/bli_gemmsup_rd_haswell_asm_d6x8n.c` & `blis-0.9.1.dev1/blis/_src/kernels/haswell/3/sup/bli_gemmsup_rd_haswell_asm_d6x8n.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/haswell/3/sup/bli_gemmsup_rd_haswell_asm_s6x16m.c` & `blis-0.9.1.dev1/blis/_src/kernels/haswell/3/sup/bli_gemmsup_rd_haswell_asm_s6x16m.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/haswell/3/sup/bli_gemmsup_rd_haswell_asm_s6x16n.c` & `blis-0.9.1.dev1/blis/_src/kernels/haswell/3/sup/bli_gemmsup_rd_haswell_asm_s6x16n.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/haswell/3/sup/bli_gemmsup_rv_haswell_asm_d6x8m.c` & `blis-0.9.1.dev1/blis/_src/kernels/haswell/3/sup/bli_gemmsup_rv_haswell_asm_d6x8m.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/haswell/3/sup/bli_gemmsup_rv_haswell_asm_d6x8n.c` & `blis-0.9.1.dev1/blis/_src/kernels/haswell/3/sup/bli_gemmsup_rv_haswell_asm_d6x8n.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/haswell/3/sup/bli_gemmsup_rv_haswell_asm_s6x16m.c` & `blis-0.9.1.dev1/blis/_src/kernels/haswell/3/sup/bli_gemmsup_rv_haswell_asm_s6x16m.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/haswell/3/sup/bli_gemmsup_rv_haswell_asm_s6x16n.c` & `blis-0.9.1.dev1/blis/_src/kernels/haswell/3/sup/bli_gemmsup_rv_haswell_asm_s6x16n.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/haswell/3/sup/d6x8/bli_gemmsup_r_haswell_ref_dMx1.c` & `blis-0.9.1.dev1/blis/_src/kernels/haswell/3/sup/d6x8/bli_gemmsup_r_haswell_ref_dMx1.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/haswell/3/sup/d6x8/bli_gemmsup_rd_haswell_asm_dMx1.c` & `blis-0.9.1.dev1/blis/_src/kernels/haswell/3/sup/d6x8/bli_gemmsup_rd_haswell_asm_dMx1.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/haswell/3/sup/d6x8/bli_gemmsup_rd_haswell_asm_dMx2.c` & `blis-0.9.1.dev1/blis/_src/kernels/haswell/3/sup/d6x8/bli_gemmsup_rd_haswell_asm_dMx2.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/haswell/3/sup/d6x8/bli_gemmsup_rd_haswell_asm_dMx4.c` & `blis-0.9.1.dev1/blis/_src/kernels/haswell/3/sup/d6x8/bli_gemmsup_rd_haswell_asm_dMx4.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/haswell/3/sup/d6x8/bli_gemmsup_rd_haswell_asm_dMx8.c` & `blis-0.9.1.dev1/blis/_src/kernels/haswell/3/sup/d6x8/bli_gemmsup_rd_haswell_asm_dMx8.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/haswell/3/sup/d6x8/bli_gemmsup_rv_haswell_asm_dMx2.c` & `blis-0.9.1.dev1/blis/_src/kernels/haswell/3/sup/d6x8/bli_gemmsup_rv_haswell_asm_dMx2.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/haswell/3/sup/d6x8/bli_gemmsup_rv_haswell_asm_dMx4.c` & `blis-0.9.1.dev1/blis/_src/kernels/haswell/3/sup/d6x8/bli_gemmsup_rv_haswell_asm_dMx4.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/haswell/3/sup/d6x8/bli_gemmsup_rv_haswell_asm_dMx6.c` & `blis-0.9.1.dev1/blis/_src/kernels/haswell/3/sup/d6x8/bli_gemmsup_rv_haswell_asm_dMx6.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/haswell/3/sup/d6x8/bli_gemmsup_rv_haswell_asm_dMx8.c` & `blis-0.9.1.dev1/blis/_src/kernels/haswell/3/sup/d6x8/bli_gemmsup_rv_haswell_asm_dMx8.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/haswell/3/sup/d6x8/old/bli_gemmsup_rd_haswell_asm_d6x8.c` & `blis-0.9.1.dev1/blis/_src/kernels/haswell/3/sup/d6x8/old/bli_gemmsup_rd_haswell_asm_d6x8.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/haswell/3/sup/d6x8/old/bli_gemmsup_rv_haswell_asm_d6x8.c` & `blis-0.9.1.dev1/blis/_src/kernels/haswell/3/sup/d6x8/old/bli_gemmsup_rv_haswell_asm_d6x8.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/haswell/3/sup/old/bli_gemmsup_rd_haswell_asm_d6x8.c` & `blis-0.9.1.dev1/blis/_src/kernels/haswell/3/sup/old/bli_gemmsup_rd_haswell_asm_d6x8.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/haswell/3/sup/old/bli_gemmsup_rd_haswell_asm_d6x8m.c` & `blis-0.9.1.dev1/blis/_src/kernels/haswell/3/sup/old/bli_gemmsup_rd_haswell_asm_d6x8m.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/haswell/3/sup/old/bli_gemmsup_rd_haswell_asm_d6x8n.c` & `blis-0.9.1.dev1/blis/_src/kernels/haswell/3/sup/old/bli_gemmsup_rd_haswell_asm_d6x8n.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/haswell/3/sup/s6x16/bli_gemmsup_r_haswell_ref_sMx1.c` & `blis-0.9.1.dev1/blis/_src/kernels/haswell/3/sup/s6x16/bli_gemmsup_r_haswell_ref_sMx1.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/haswell/3/sup/s6x16/bli_gemmsup_rd_haswell_asm_sMx1.c` & `blis-0.9.1.dev1/blis/_src/kernels/haswell/3/sup/s6x16/bli_gemmsup_rd_haswell_asm_sMx1.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/haswell/3/sup/s6x16/bli_gemmsup_rd_haswell_asm_sMx12.c` & `blis-0.9.1.dev1/blis/_src/kernels/haswell/3/sup/s6x16/bli_gemmsup_rd_haswell_asm_sMx12.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/haswell/3/sup/s6x16/bli_gemmsup_rd_haswell_asm_sMx16.c` & `blis-0.9.1.dev1/blis/_src/kernels/haswell/3/sup/s6x16/bli_gemmsup_rd_haswell_asm_sMx16.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/haswell/3/sup/s6x16/bli_gemmsup_rd_haswell_asm_sMx2.c` & `blis-0.9.1.dev1/blis/_src/kernels/haswell/3/sup/s6x16/bli_gemmsup_rd_haswell_asm_sMx2.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/haswell/3/sup/s6x16/bli_gemmsup_rd_haswell_asm_sMx4.c` & `blis-0.9.1.dev1/blis/_src/kernels/haswell/3/sup/s6x16/bli_gemmsup_rd_haswell_asm_sMx4.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/haswell/3/sup/s6x16/bli_gemmsup_rd_haswell_asm_sMx8.c` & `blis-0.9.1.dev1/blis/_src/kernels/haswell/3/sup/s6x16/bli_gemmsup_rd_haswell_asm_sMx8.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/haswell/3/sup/s6x16/bli_gemmsup_rv_haswell_asm_sMx12.c` & `blis-0.9.1.dev1/blis/_src/kernels/haswell/3/sup/s6x16/bli_gemmsup_rv_haswell_asm_sMx12.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/haswell/3/sup/s6x16/bli_gemmsup_rv_haswell_asm_sMx16.c` & `blis-0.9.1.dev1/blis/_src/kernels/haswell/3/sup/s6x16/bli_gemmsup_rv_haswell_asm_sMx16.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/haswell/3/sup/s6x16/bli_gemmsup_rv_haswell_asm_sMx2.c` & `blis-0.9.1.dev1/blis/_src/kernels/haswell/3/sup/s6x16/bli_gemmsup_rv_haswell_asm_sMx2.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/haswell/3/sup/s6x16/bli_gemmsup_rv_haswell_asm_sMx4.c` & `blis-0.9.1.dev1/blis/_src/kernels/haswell/3/sup/s6x16/bli_gemmsup_rv_haswell_asm_sMx4.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/haswell/3/sup/s6x16/bli_gemmsup_rv_haswell_asm_sMx6.c` & `blis-0.9.1.dev1/blis/_src/kernels/haswell/3/sup/s6x16/bli_gemmsup_rv_haswell_asm_sMx6.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/haswell/3/sup/s6x16/bli_gemmsup_rv_haswell_asm_sMx8.c` & `blis-0.9.1.dev1/blis/_src/kernels/haswell/3/sup/s6x16/bli_gemmsup_rv_haswell_asm_sMx8.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/haswell/bli_kernels_haswell.h` & `blis-0.9.1.dev1/blis/_src/kernels/haswell/bli_kernels_haswell.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/knc/3/bli_dgemm_knc_asm_30x8.c` & `blis-0.9.1.dev1/blis/_src/kernels/knc/3/bli_dgemm_knc_asm_30x8.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/knc/3/bli_sgemm_knc_asm_30x16.c` & `blis-0.9.1.dev1/blis/_src/kernels/knc/3/bli_sgemm_knc_asm_30x16.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/knc/bli_kernels_knc.h` & `blis-0.9.1.dev1/blis/_src/kernels/knc/bli_kernels_knc.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/knl/1m/bli_dpackm_knl_asm_24x8.c` & `blis-0.9.1.dev1/blis/_src/kernels/knl/1m/bli_dpackm_knl_asm_24x8.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/knl/1m/bli_spackm_knl_asm_24x16.c` & `blis-0.9.1.dev1/blis/_src/kernels/knl/1m/bli_spackm_knl_asm_24x16.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/knl/1m/old/bli_packm_knl_asm_30x8.c` & `blis-0.9.1.dev1/blis/_src/kernels/knl/1m/old/bli_packm_knl_asm_30x8.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/knl/3/bli_dgemm_knl_asm_24x8.c` & `blis-0.9.1.dev1/blis/_src/kernels/knl/3/bli_dgemm_knl_asm_24x8.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/knl/3/bli_sgemm_knl_asm_24x16.c` & `blis-0.9.1.dev1/blis/_src/kernels/knl/3/bli_sgemm_knl_asm_24x16.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/knl/3/other/bli_dgemm_knl_asm_12x16.c` & `blis-0.9.1.dev1/blis/_src/kernels/knl/3/other/bli_dgemm_knl_asm_12x16.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/knl/3/other/bli_dgemm_knl_asm_30x8.c` & `blis-0.9.1.dev1/blis/_src/kernels/knl/3/other/bli_dgemm_knl_asm_30x8.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/knl/3/other/bli_dgemm_knl_asm_30x8_knc.c` & `blis-0.9.1.dev1/blis/_src/kernels/knl/3/other/bli_dgemm_knl_asm_30x8_knc.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/knl/3/other/bli_dgemm_knl_asm_8x24.c` & `blis-0.9.1.dev1/blis/_src/kernels/knl/3/other/bli_dgemm_knl_asm_8x24.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/knl/3/other/bli_sgemm_knl_asm_30x16_knc.c` & `blis-0.9.1.dev1/blis/_src/kernels/knl/3/other/bli_sgemm_knl_asm_30x16_knc.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/knl/bli_kernels_knl.h` & `blis-0.9.1.dev1/blis/_src/kernels/knl/bli_kernels_knl.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/old/c99/3/bli_gemm_c99_4x4.c` & `blis-0.9.1.dev1/blis/_src/kernels/old/c99/3/bli_gemm_c99_4x4.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/old/c99/3/bli_gemmtrsm_l_c99_4x4.c` & `blis-0.9.1.dev1/blis/_src/kernels/old/c99/3/bli_gemmtrsm_l_c99_4x4.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/old/c99/3/bli_gemmtrsm_u_c99_4x4.c` & `blis-0.9.1.dev1/blis/_src/kernels/old/c99/3/bli_gemmtrsm_u_c99_4x4.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/old/c99/3/bli_trsm_l_c99_4x4.c` & `blis-0.9.1.dev1/blis/_src/kernels/old/c99/3/bli_trsm_l_c99_4x4.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/old/c99/3/bli_trsm_u_c99_4x4.c` & `blis-0.9.1.dev1/blis/_src/kernels/old/c99/3/bli_trsm_u_c99_4x4.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/old/c99/bli_kernels_c99.h` & `blis-0.9.1.dev1/blis/_src/kernels/old/c99/bli_kernels_c99.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/old/loongson3a/3/bli_gemm_loongson3a_opt_d4x4.c` & `blis-0.9.1.dev1/blis/_src/kernels/old/loongson3a/3/bli_gemm_loongson3a_opt_d4x4.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/old/nacl/pnacl/1/bli_axpyv_opt.c` & `blis-0.9.1.dev1/blis/_src/kernels/old/nacl/pnacl/1/bli_axpyv_opt.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/old/nacl/pnacl/1/bli_dotv_opt.c` & `blis-0.9.1.dev1/blis/_src/kernels/old/nacl/pnacl/1/bli_dotv_opt.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/old/nacl/pnacl/3/bli_gemm_opt.c` & `blis-0.9.1.dev1/blis/_src/kernels/old/nacl/pnacl/3/bli_gemm_opt.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/old/x86/1m/bli_packm_2xk.c` & `blis-0.9.1.dev1/blis/_src/kernels/old/x86/1m/bli_packm_2xk.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/old/x86/1m/bli_packm_2xk.h` & `blis-0.9.1.dev1/blis/_src/kernels/old/x86/1m/bli_packm_2xk.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/old/x86/1m/bli_packm_4xk.c` & `blis-0.9.1.dev1/blis/_src/kernels/old/x86/1m/bli_packm_4xk.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/old/x86/1m/bli_packm_4xk.h` & `blis-0.9.1.dev1/blis/_src/kernels/old/x86/1m/bli_packm_4xk.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/old/x86/3/bli_gemm_opt_d2x4.c` & `blis-0.9.1.dev1/blis/_src/kernels/old/x86/3/bli_gemm_opt_d2x4.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/old/x86/3/bli_gemm_opt_d4x2.c` & `blis-0.9.1.dev1/blis/_src/kernels/old/x86/3/bli_gemm_opt_d4x2.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/old/x86/3/bli_gemmtrsm_l_opt_d4x2.c` & `blis-0.9.1.dev1/blis/_src/kernels/old/x86/3/bli_gemmtrsm_l_opt_d4x2.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/old/x86/3/bli_gemmtrsm_u_opt_d4x2.c` & `blis-0.9.1.dev1/blis/_src/kernels/old/x86/3/bli_gemmtrsm_u_opt_d4x2.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/old/x86/3/bli_trsm_l_opt_d4x2.c` & `blis-0.9.1.dev1/blis/_src/kernels/old/x86/3/bli_trsm_l_opt_d4x2.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/penryn/1/bli_axpyv_penryn_int.c` & `blis-0.9.1.dev1/blis/_src/kernels/penryn/1/bli_axpyv_penryn_int.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/penryn/1/bli_dotv_penryn_int.c` & `blis-0.9.1.dev1/blis/_src/kernels/penryn/1/bli_dotv_penryn_int.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/penryn/1f/bli_axpy2v_penryn_int.c` & `blis-0.9.1.dev1/blis/_src/kernels/penryn/1f/bli_axpy2v_penryn_int.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/penryn/1f/bli_axpyf_penryn_int.c` & `blis-0.9.1.dev1/blis/_src/kernels/penryn/1f/bli_axpyf_penryn_int.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/penryn/1f/bli_dotaxpyv_penryn_int.c` & `blis-0.9.1.dev1/blis/_src/kernels/penryn/1f/bli_dotaxpyv_penryn_int.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/penryn/1f/bli_dotxaxpyf_penryn_int.c` & `blis-0.9.1.dev1/blis/_src/kernels/penryn/1f/bli_dotxaxpyf_penryn_int.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/penryn/1f/bli_dotxf_penryn_int.c` & `blis-0.9.1.dev1/blis/_src/kernels/penryn/1f/bli_dotxf_penryn_int.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/penryn/3/bli_gemm_penryn_asm_d4x4.c` & `blis-0.9.1.dev1/blis/_src/kernels/penryn/3/bli_gemm_penryn_asm_d4x4.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/penryn/3/bli_gemmtrsm_l_penryn_asm_d4x4.c` & `blis-0.9.1.dev1/blis/_src/kernels/penryn/3/bli_gemmtrsm_l_penryn_asm_d4x4.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/penryn/3/bli_gemmtrsm_u_penryn_asm_d4x4.c` & `blis-0.9.1.dev1/blis/_src/kernels/penryn/3/bli_gemmtrsm_u_penryn_asm_d4x4.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/penryn/3/bli_trsm_l_penryn_asm_d4x4.c` & `blis-0.9.1.dev1/blis/_src/kernels/penryn/3/bli_trsm_l_penryn_asm_d4x4.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/penryn/3/bli_trsm_u_penryn_asm_d4x4.c` & `blis-0.9.1.dev1/blis/_src/kernels/penryn/3/bli_trsm_u_penryn_asm_d4x4.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/penryn/bli_kernels_penryn.h` & `blis-0.9.1.dev1/blis/_src/kernels/penryn/bli_kernels_penryn.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/piledriver/3/bli_gemm_piledriver_asm_d8x3.c` & `blis-0.9.1.dev1/blis/_src/kernels/piledriver/3/bli_gemm_piledriver_asm_d8x3.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/piledriver/bli_kernels_piledriver.h` & `blis-0.9.1.dev1/blis/_src/kernels/piledriver/bli_kernels_piledriver.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/power10/3/bli_dgemm_power10_mma.c` & `blis-0.9.1.dev1/blis/_src/kernels/power10/3/bli_dgemm_power10_mma.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/power10/3/bli_i16gemm_power10_mma.c` & `blis-0.9.1.dev1/blis/_src/kernels/power10/3/bli_i16gemm_power10_mma.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/power10/3/bli_i16sgemm_power10_mma.c` & `blis-0.9.1.dev1/blis/_src/kernels/power10/3/bli_i16sgemm_power10_mma.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/power10/3/bli_i4gemm_power10_mma.c` & `blis-0.9.1.dev1/blis/_src/kernels/power10/3/bli_i4gemm_power10_mma.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/power10/3/bli_i8gemm_power10_mma.c` & `blis-0.9.1.dev1/blis/_src/kernels/power10/3/bli_i8gemm_power10_mma.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/power10/3/bli_sbgemm_power10_mma.c` & `blis-0.9.1.dev1/blis/_src/kernels/power10/3/bli_sbgemm_power10_mma.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/power10/3/bli_sgemm_power10_mma.c` & `blis-0.9.1.dev1/blis/_src/kernels/power10/3/bli_sgemm_power10_mma.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/power10/3/bli_shgemm_power10_mma.c` & `blis-0.9.1.dev1/blis/_src/kernels/power10/3/bli_shgemm_power10_mma.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/power10/3/vector_int_macros.h` & `blis-0.9.1.dev1/blis/_src/kernels/power10/3/vector_int_macros.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/power10/bli_kernels_power10.h` & `blis-0.9.1.dev1/blis/_src/kernels/power10/bli_kernels_power10.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/power7/3/bli_gemm_power7_int_8x4.c` & `blis-0.9.1.dev1/blis/_src/kernels/power7/3/bli_gemm_power7_int_8x4.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/power7/3/test/bli_gemm_power7_int_8x4.c` & `blis-0.9.1.dev1/blis/_src/kernels/power7/3/test/bli_gemm_power7_int_8x4.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/power7/3/test/bli_gemm_power7_int_8x4.h` & `blis-0.9.1.dev1/blis/_src/kernels/power7/3/test/bli_gemm_power7_int_8x4.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/power7/3/test/blis_utest.h` & `blis-0.9.1.dev1/blis/_src/kernels/power7/3/test/blis_utest.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/power7/3/test/exp.c` & `blis-0.9.1.dev1/blis/_src/kernels/power7/3/test/exp.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/power7/bli_kernels_power7.h` & `blis-0.9.1.dev1/blis/_src/kernels/power7/bli_kernels_power7.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/power9/3/bli_gemm_power9_asm_d12x6.c` & `blis-0.9.1.dev1/blis/_src/kernels/power9/3/bli_gemm_power9_asm_d12x6.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/power9/3/bli_pwr9_asm_macros_12x6.h` & `blis-0.9.1.dev1/blis/_src/kernels/power9/3/bli_pwr9_asm_macros_12x6.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/power9/bli_kernels_power9.h` & `blis-0.9.1.dev1/blis/_src/kernels/power9/bli_kernels_power9.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/sandybridge/3/bli_gemm_sandybridge_asm_d8x4.c` & `blis-0.9.1.dev1/blis/_src/kernels/sandybridge/3/bli_gemm_sandybridge_asm_d8x4.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/sandybridge/3/bli_gemm_sandybridge_int_d8x4.c` & `blis-0.9.1.dev1/blis/_src/kernels/sandybridge/3/bli_gemm_sandybridge_int_d8x4.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/sandybridge/bli_kernels_sandybridge.h` & `blis-0.9.1.dev1/blis/_src/kernels/sandybridge/bli_kernels_sandybridge.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/skx/3/bli_dgemm_skx_asm_16x12_l2.c` & `blis-0.9.1.dev1/blis/_src/kernels/skx/3/bli_dgemm_skx_asm_16x12_l2.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/skx/3/bli_dgemm_skx_asm_16x14.c` & `blis-0.9.1.dev1/blis/_src/kernels/skx/3/bli_dgemm_skx_asm_16x14.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/skx/3/bli_sgemm_skx_asm_32x12_l2.c` & `blis-0.9.1.dev1/blis/_src/kernels/skx/3/bli_sgemm_skx_asm_32x12_l2.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/skx/bli_kernels_skx.h` & `blis-0.9.1.dev1/blis/_src/kernels/skx/bli_kernels_skx.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/zen/1/bli_amaxv_zen_int.c` & `blis-0.9.1.dev1/blis/_src/kernels/zen/1/bli_amaxv_zen_int.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/zen/1/bli_axpyv_zen_int.c` & `blis-0.9.1.dev1/blis/_src/kernels/zen/1/bli_axpyv_zen_int.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/zen/1/bli_axpyv_zen_int10.c` & `blis-0.9.1.dev1/blis/_src/kernels/zen/1/bli_axpyv_zen_int10.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/zen/1/bli_copyv_zen_int.c` & `blis-0.9.1.dev1/blis/_src/kernels/zen/1/bli_copyv_zen_int.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/zen/1/bli_dotv_zen_int.c` & `blis-0.9.1.dev1/blis/_src/kernels/zen/1/bli_dotv_zen_int.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/zen/1/bli_dotv_zen_int10.c` & `blis-0.9.1.dev1/blis/_src/kernels/zen/1/bli_dotv_zen_int10.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/zen/1/bli_dotxv_zen_int.c` & `blis-0.9.1.dev1/blis/_src/kernels/zen/1/bli_dotxv_zen_int.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/zen/1/bli_scalv_zen_int.c` & `blis-0.9.1.dev1/blis/_src/kernels/zen/1/bli_scalv_zen_int.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/zen/1/bli_scalv_zen_int10.c` & `blis-0.9.1.dev1/blis/_src/kernels/zen/1/bli_scalv_zen_int10.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/zen/1/bli_setv_zen_int.c` & `blis-0.9.1.dev1/blis/_src/kernels/zen/1/bli_setv_zen_int.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/zen/1/bli_swapv_zen_int8.c` & `blis-0.9.1.dev1/blis/_src/kernels/zen/1/bli_swapv_zen_int8.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/zen/1f/bli_axpyf_zen_int_4.c` & `blis-0.9.1.dev1/blis/_src/kernels/zen/1f/bli_axpyf_zen_int_4.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/zen/1f/bli_axpyf_zen_int_5.c` & `blis-0.9.1.dev1/blis/_src/kernels/zen/1f/bli_axpyf_zen_int_5.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/zen/1f/bli_axpyf_zen_int_8.c` & `blis-0.9.1.dev1/blis/_src/kernels/zen/1f/bli_axpyf_zen_int_8.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/zen/1f/bli_dotxf_zen_int_8.c` & `blis-0.9.1.dev1/blis/_src/kernels/zen/1f/bli_dotxf_zen_int_8.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/zen/3/bli_gemm_small.c` & `blis-0.9.1.dev1/blis/_src/kernels/zen/3/bli_gemm_small.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/zen/3/bli_gemmt_small.c` & `blis-0.9.1.dev1/blis/_src/kernels/zen/3/bli_gemmt_small.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/zen/3/bli_trsm_small.c` & `blis-0.9.1.dev1/blis/_src/kernels/zen/3/bli_trsm_small.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/zen/3/sup/broken/bli_gemmsup_rv_zen_asm_c3x8.c` & `blis-0.9.1.dev1/blis/_src/kernels/zen/3/sup/broken/bli_gemmsup_rv_zen_asm_c3x8.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/zen/3/sup/broken/bli_gemmsup_rv_zen_asm_c3x8m.c` & `blis-0.9.1.dev1/blis/_src/kernels/zen/3/sup/broken/bli_gemmsup_rv_zen_asm_c3x8m.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/zen/3/sup/broken/bli_gemmsup_rv_zen_asm_c3x8n.c` & `blis-0.9.1.dev1/blis/_src/kernels/zen/3/sup/broken/bli_gemmsup_rv_zen_asm_c3x8n.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/zen/3/sup/broken/bli_gemmsup_rv_zen_asm_z3x4.c` & `blis-0.9.1.dev1/blis/_src/kernels/zen/3/sup/broken/bli_gemmsup_rv_zen_asm_z3x4.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/zen/3/sup/broken/bli_gemmsup_rv_zen_asm_z3x4m.c` & `blis-0.9.1.dev1/blis/_src/kernels/zen/3/sup/broken/bli_gemmsup_rv_zen_asm_z3x4m.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/zen/3/sup/broken/bli_gemmsup_rv_zen_asm_z3x4n.c` & `blis-0.9.1.dev1/blis/_src/kernels/zen/3/sup/broken/bli_gemmsup_rv_zen_asm_z3x4n.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/zen/3/sup/other/bli_gemmsup_rd_zen_asm_s6x16.c` & `blis-0.9.1.dev1/blis/_src/kernels/zen/3/sup/other/bli_gemmsup_rd_zen_asm_s6x16.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/zen/3/sup/other/bli_gemmsup_rd_zen_asm_s6x16m.c` & `blis-0.9.1.dev1/blis/_src/kernels/zen/3/sup/other/bli_gemmsup_rd_zen_asm_s6x16m.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/zen/3/sup/other/bli_gemmsup_rd_zen_asm_s6x16n.c` & `blis-0.9.1.dev1/blis/_src/kernels/zen/3/sup/other/bli_gemmsup_rd_zen_asm_s6x16n.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/zen/3/sup/other/bli_gemmsup_rv_zen_asm_s6x16.c` & `blis-0.9.1.dev1/blis/_src/kernels/zen/3/sup/other/bli_gemmsup_rv_zen_asm_s6x16.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/zen/3/sup/other/bli_gemmsup_rv_zen_asm_s6x16m.c` & `blis-0.9.1.dev1/blis/_src/kernels/zen/3/sup/other/bli_gemmsup_rv_zen_asm_s6x16m.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/zen/3/sup/other/bli_gemmsup_rv_zen_asm_s6x16n.c` & `blis-0.9.1.dev1/blis/_src/kernels/zen/3/sup/other/bli_gemmsup_rv_zen_asm_s6x16n.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/zen/bli_kernels_zen.h` & `blis-0.9.1.dev1/blis/_src/kernels/zen/bli_kernels_zen.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/kernels/zen2/bli_kernels_zen2.h` & `blis-0.9.1.dev1/blis/_src/kernels/zen2/bli_kernels_zen2.h`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/make/darwin-firestorm.jsonl` & `blis-0.9.1.dev1/blis/_src/make/darwin-firestorm.jsonl`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/make/darwin-generic.jsonl` & `blis-0.9.1.dev1/blis/_src/make/darwin-generic.jsonl`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/make/darwin-x86_64.jsonl` & `blis-0.9.1.dev1/blis/_src/make/darwin-x86_64.jsonl`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/make/darwin-x86_64_no_skx.jsonl` & `blis-0.9.1.dev1/blis/_src/make/darwin-x86_64_no_skx.jsonl`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/make/darwin-x86_64_no_zen2.jsonl` & `blis-0.9.1.dev1/blis/_src/make/darwin-x86_64_no_zen2.jsonl`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/make/darwin-x86_64_no_zen3.jsonl` & `blis-0.9.1.dev1/blis/_src/make/darwin-x86_64_no_zen3.jsonl`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/make/linux-arm64.jsonl` & `blis-0.9.1.dev1/blis/_src/make/linux-arm64.jsonl`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/make/linux-arm64_no_sve.jsonl` & `blis-0.9.1.dev1/blis/_src/make/linux-arm64_no_sve.jsonl`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/make/linux-generic.jsonl` & `blis-0.9.1.dev1/blis/_src/make/linux-generic.jsonl`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/make/linux-power9.jsonl` & `blis-0.9.1.dev1/blis/_src/make/linux-power9.jsonl`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/make/linux-x86_64.jsonl` & `blis-0.9.1.dev1/blis/_src/make/linux-x86_64.jsonl`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/make/linux-x86_64_no_skx.jsonl` & `blis-0.9.1.dev1/blis/_src/make/linux-x86_64_no_skx.jsonl`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/make/linux-x86_64_no_zen2.jsonl` & `blis-0.9.1.dev1/blis/_src/make/linux-x86_64_no_zen2.jsonl`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/make/linux-x86_64_no_zen3.jsonl` & `blis-0.9.1.dev1/blis/_src/make/linux-x86_64_no_zen3.jsonl`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/make/windows-generic.jsonl` & `blis-0.9.1.dev1/blis/_src/make/windows-generic.jsonl`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/make/windows-x86_64.jsonl` & `blis-0.9.1.dev1/blis/_src/make/windows-x86_64.jsonl`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/ref_kernels/1/bli_addv_ref.c` & `blis-0.9.1.dev1/blis/_src/ref_kernels/1/bli_addv_ref.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/ref_kernels/1/bli_amaxv_ref.c` & `blis-0.9.1.dev1/blis/_src/ref_kernels/1/bli_amaxv_ref.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/ref_kernels/1/bli_axpbyv_ref.c` & `blis-0.9.1.dev1/blis/_src/ref_kernels/1/bli_axpbyv_ref.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/ref_kernels/1/bli_axpyv_ref.c` & `blis-0.9.1.dev1/blis/_src/ref_kernels/1/bli_axpyv_ref.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/ref_kernels/1/bli_copyv_ref.c` & `blis-0.9.1.dev1/blis/_src/ref_kernels/1/bli_copyv_ref.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/ref_kernels/1/bli_dotv_ref.c` & `blis-0.9.1.dev1/blis/_src/ref_kernels/1/bli_dotv_ref.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/ref_kernels/1/bli_dotxv_ref.c` & `blis-0.9.1.dev1/blis/_src/ref_kernels/1/bli_dotxv_ref.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/ref_kernels/1/bli_invertv_ref.c` & `blis-0.9.1.dev1/blis/_src/ref_kernels/1/bli_invertv_ref.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/ref_kernels/1/bli_scal2v_ref.c` & `blis-0.9.1.dev1/blis/_src/ref_kernels/1/bli_scal2v_ref.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/ref_kernels/1/bli_scalv_ref.c` & `blis-0.9.1.dev1/blis/_src/ref_kernels/1/bli_scalv_ref.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/ref_kernels/1/bli_setv_ref.c` & `blis-0.9.1.dev1/blis/_src/ref_kernels/1/bli_setv_ref.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/ref_kernels/1/bli_subv_ref.c` & `blis-0.9.1.dev1/blis/_src/ref_kernels/1/bli_subv_ref.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/ref_kernels/1/bli_swapv_ref.c` & `blis-0.9.1.dev1/blis/_src/ref_kernels/1/bli_swapv_ref.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/ref_kernels/1/bli_xpbyv_ref.c` & `blis-0.9.1.dev1/blis/_src/ref_kernels/1/bli_xpbyv_ref.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/ref_kernels/1f/bli_axpy2v_ref.c` & `blis-0.9.1.dev1/blis/_src/ref_kernels/1f/bli_axpy2v_ref.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/ref_kernels/1f/bli_axpyf_ref.c` & `blis-0.9.1.dev1/blis/_src/ref_kernels/1f/bli_axpyf_ref.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/ref_kernels/1f/bli_dotaxpyv_ref.c` & `blis-0.9.1.dev1/blis/_src/ref_kernels/1f/bli_dotaxpyv_ref.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/ref_kernels/1f/bli_dotxaxpyf_ref.c` & `blis-0.9.1.dev1/blis/_src/ref_kernels/1f/bli_dotxaxpyf_ref.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/ref_kernels/1f/bli_dotxf_ref.c` & `blis-0.9.1.dev1/blis/_src/ref_kernels/1f/bli_dotxf_ref.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/ref_kernels/1f/other/bli_dotxaxpyf_ref_alt.c` & `blis-0.9.1.dev1/blis/_src/ref_kernels/1f/other/bli_dotxaxpyf_ref_alt.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/ref_kernels/1m/bli_packm_cxk_1er_ref.c` & `blis-0.9.1.dev1/blis/_src/ref_kernels/1m/bli_packm_cxk_1er_ref.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/ref_kernels/1m/bli_packm_cxk_bb_ref.c` & `blis-0.9.1.dev1/blis/_src/ref_kernels/1m/bli_packm_cxk_bb_ref.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/ref_kernels/1m/bli_packm_cxk_ref.c` & `blis-0.9.1.dev1/blis/_src/ref_kernels/1m/bli_packm_cxk_ref.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/ref_kernels/1m/bli_unpackm_cxk_ref.c` & `blis-0.9.1.dev1/blis/_src/ref_kernels/1m/bli_unpackm_cxk_ref.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/ref_kernels/3/bb/bli_gemmbb_ref.c` & `blis-0.9.1.dev1/blis/_src/ref_kernels/3/bb/bli_gemmbb_ref.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/ref_kernels/3/bb/bli_gemmtrsmbb_ref.c` & `blis-0.9.1.dev1/blis/_src/ref_kernels/3/bb/bli_gemmtrsmbb_ref.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/ref_kernels/3/bb/bli_trsmbb_ref.c` & `blis-0.9.1.dev1/blis/_src/ref_kernels/3/bb/bli_trsmbb_ref.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/ref_kernels/3/bli_gemm_ref.c` & `blis-0.9.1.dev1/blis/_src/ref_kernels/3/bli_gemm_ref.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/ref_kernels/3/bli_gemmsup_ref.c` & `blis-0.9.1.dev1/blis/_src/ref_kernels/3/bli_gemmsup_ref.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/ref_kernels/3/bli_gemmtrsm_ref.c` & `blis-0.9.1.dev1/blis/_src/ref_kernels/3/bli_gemmtrsm_ref.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/ref_kernels/3/bli_trsm_ref.c` & `blis-0.9.1.dev1/blis/_src/ref_kernels/3/bli_trsm_ref.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/ref_kernels/3/old/bli_gemm_simd_ref.c` & `blis-0.9.1.dev1/blis/_src/ref_kernels/3/old/bli_gemm_simd_ref.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/ref_kernels/3/old/bli_gemm_unrl_ref.c` & `blis-0.9.1.dev1/blis/_src/ref_kernels/3/old/bli_gemm_unrl_ref.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/ref_kernels/3/old/bli_trsm_simd_ref.c` & `blis-0.9.1.dev1/blis/_src/ref_kernels/3/old/bli_trsm_simd_ref.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/ref_kernels/bli_cntx_ref.c` & `blis-0.9.1.dev1/blis/_src/ref_kernels/bli_cntx_ref.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/ref_kernels/ind/bli_gemm1m_ref.c` & `blis-0.9.1.dev1/blis/_src/ref_kernels/ind/bli_gemm1m_ref.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/ref_kernels/ind/bli_gemmtrsm1m_ref.c` & `blis-0.9.1.dev1/blis/_src/ref_kernels/ind/bli_gemmtrsm1m_ref.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/_src/ref_kernels/ind/bli_trsm1m_ref.c` & `blis-0.9.1.dev1/blis/_src/ref_kernels/ind/bli_trsm1m_ref.c`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/about.py` & `blis-0.9.1.dev1/blis/about.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright ExplosionAI GmbH, released under BSD
 # inspired from:
 
 # https://python-packaging-user-guide.readthedocs.org/en/latest/single_source_version/
 # https://github.com/pypa/warehouse/blob/master/warehouse/__about__.py
 
 __name__ = "blis"
-__version__ = "0.9.1.dev0"
+__version__ = "0.9.1.dev1"
 __summary__ = (
     "The Blis BLAS-like linear algebra library, as a self-contained C-extension."
 )
 __uri__ = "https://github.com/explosion/cython-blis"
 __author__ = "Explosion"
 __email__ = "contact@explosion.ai"
 __license__ = "BSD"
```

### Comparing `blis-0.9.1.dev0/blis/benchmark.py` & `blis-0.9.1.dev1/blis/benchmark.py`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/cy.pxd` & `blis-0.9.1.dev1/blis/cy.pxd`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/cy.pyx` & `blis-0.9.1.dev1/blis/cy.pyx`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/py.pyx` & `blis-0.9.1.dev1/blis/py.pyx`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/tests/common.py` & `blis-0.9.1.dev1/blis/tests/common.py`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/tests/test_dotv.py` & `blis-0.9.1.dev1/blis/tests/test_dotv.py`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis/tests/test_gemm.py` & `blis-0.9.1.dev1/blis/tests/test_gemm.py`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/blis.egg-info/PKG-INFO` & `blis-0.9.1.dev1/blis.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blis
-Version: 0.9.1.dev0
+Version: 0.9.1.dev1
 Summary: The Blis BLAS-like linear algebra library, as a self-contained C-extension.
 Home-page: https://github.com/explosion/cython-blis
 Author: Explosion
 Author-email: contact@explosion.ai
 License: BSD
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: blis Version: 0.9.1.dev0 Summary: The Blis BLAS-
+Metadata-Version: 2.1 Name: blis Version: 0.9.1.dev1 Summary: The Blis BLAS-
 like linear algebra library, as a self-contained C-extension. Home-page: https:
 //github.com/explosion/cython-blis Author: Explosion Author-email:
 contact@explosion.ai License: BSD Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology Classifier: License ::
 OSI Approved :: BSD License Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X Classifier: Programming
```

### Comparing `blis-0.9.1.dev0/blis.egg-info/SOURCES.txt` & `blis-0.9.1.dev1/blis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `blis-0.9.1.dev0/setup.py` & `blis-0.9.1.dev1/setup.py`

 * *Files identical despite different names*

