# Comparing `tmp/shtns-3.6.1.tar.gz` & `tmp/shtns-3.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shtns-3.6.1.tar", last modified: Thu Jul 13 12:18:14 2023, max compression
+gzip compressed data, was "shtns-3.6.2.tar", last modified: Fri Jul 21 11:48:35 2023, max compression
```

## Comparing `shtns-3.6.1.tar` & `shtns-3.6.2.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 nat       (1000)     1000        0 2023-07-13 12:18:14.130445 shtns-3.6.1/
--rw-r--r--   0 nat       (1000)     1000    13475 2023-07-13 12:18:11.000000 shtns-3.6.1/CHANGELOG.md
--rw-r--r--   0 nat       (1000)     1000    21782 2023-07-13 12:18:11.000000 shtns-3.6.1/LICENSE
--rw-r--r--   0 nat       (1000)     1000      126 2023-07-13 12:18:11.000000 shtns-3.6.1/MANIFEST.in
--rw-r--r--   0 nat       (1000)     1000     5236 2023-07-13 12:18:11.000000 shtns-3.6.1/Makefile.in
--rw-r--r--   0 nat       (1000)     1000     1647 2023-07-13 12:18:14.130445 shtns-3.6.1/PKG-INFO
--rw-r--r--   0 nat       (1000)     1000     4415 2023-07-13 12:18:11.000000 shtns-3.6.1/README.md
-drwxr-xr-x   0 nat       (1000)     1000        0 2023-07-13 12:18:14.130445 shtns-3.6.1/SHT/
--rw-r--r--   0 nat       (1000)     1000     2897 2023-07-13 12:18:11.000000 shtns-3.6.1/SHT/Makefile
--rw-r--r--   0 nat       (1000)     1000    18709 2023-07-13 12:18:11.000000 shtns-3.6.1/SHT/fly_SH_to_spat.gen.c
--rw-r--r--   0 nat       (1000)     1000    17015 2023-07-13 12:18:11.000000 shtns-3.6.1/SHT/fly_spat_to_SH.gen.c
--rw-r--r--   0 nat       (1000)     1000    17493 2023-07-13 12:18:11.000000 shtns-3.6.1/SHT/kernel_SH_to_spat.gen.c
--rw-r--r--   0 nat       (1000)     1000    23817 2023-07-13 12:18:11.000000 shtns-3.6.1/SHT/kernel_spat_to_SH.gen.c
--rw-r--r--   0 nat       (1000)     1000    10246 2023-07-13 12:18:11.000000 shtns-3.6.1/SHT/omp_SH_to_spat.gen.c
--rw-r--r--   0 nat       (1000)     1000     9549 2023-07-13 12:18:11.000000 shtns-3.6.1/SHT/omp_spat_to_SH.gen.c
--rwxr-xr-x   0 nat       (1000)     1000   199288 2023-07-13 12:18:11.000000 shtns-3.6.1/configure
-drwxr-xr-x   0 nat       (1000)     1000        0 2023-07-13 12:18:14.130445 shtns-3.6.1/fftw3/
--rw-r--r--   0 nat       (1000)     1000    16196 2023-07-13 12:18:11.000000 shtns-3.6.1/fftw3/cycle.h
--rw-r--r--   0 nat       (1000)     1000    16691 2023-07-13 12:18:11.000000 shtns-3.6.1/fftw3/fftw3.h
--rw-r--r--   0 nat       (1000)     1000      666 2023-07-13 12:18:11.000000 shtns-3.6.1/pyproject.toml
--rw-r--r--   0 nat       (1000)     1000       38 2023-07-13 12:18:14.130445 shtns-3.6.1/setup.cfg
--rw-r--r--   0 nat       (1000)     1000     4537 2023-07-13 12:18:11.000000 shtns-3.6.1/setup.py
--rw-r--r--   0 nat       (1000)     1000    11382 2023-07-13 12:18:11.000000 shtns-3.6.1/sht_com.c
--rw-r--r--   0 nat       (1000)     1000     4438 2023-07-13 12:18:11.000000 shtns-3.6.1/sht_config.h.in
--rw-r--r--   0 nat       (1000)     1000     9401 2023-07-13 12:18:11.000000 shtns-3.6.1/sht_fly.c
--rw-r--r--   0 nat       (1000)     1000    77670 2023-07-13 12:18:11.000000 shtns-3.6.1/sht_func.c
--rw-r--r--   0 nat       (1000)     1000    70368 2023-07-13 12:18:11.000000 shtns-3.6.1/sht_init.c
--rw-r--r--   0 nat       (1000)     1000    10553 2023-07-13 12:18:11.000000 shtns-3.6.1/sht_kernels_a.c
--rw-r--r--   0 nat       (1000)     1000     8448 2023-07-13 12:18:11.000000 shtns-3.6.1/sht_kernels_s.c
--rw-r--r--   0 nat       (1000)     1000    32326 2023-07-13 12:18:11.000000 shtns-3.6.1/sht_legendre.c
--rw-r--r--   0 nat       (1000)     1000     6411 2023-07-13 12:18:11.000000 shtns-3.6.1/sht_odd_nlat.c
--rw-r--r--   0 nat       (1000)     1000     6117 2023-07-13 12:18:11.000000 shtns-3.6.1/sht_omp.c
--rw-r--r--   0 nat       (1000)     1000    26415 2023-07-13 12:18:11.000000 shtns-3.6.1/sht_private.h
-drwxr-xr-x   0 nat       (1000)     1000        0 2023-07-13 12:18:14.130445 shtns-3.6.1/shtns.egg-info/
--rw-r--r--   0 nat       (1000)     1000     1647 2023-07-13 12:18:13.000000 shtns-3.6.1/shtns.egg-info/PKG-INFO
--rw-r--r--   0 nat       (1000)     1000      633 2023-07-13 12:18:14.000000 shtns-3.6.1/shtns.egg-info/SOURCES.txt
--rw-r--r--   0 nat       (1000)     1000        1 2023-07-13 12:18:13.000000 shtns-3.6.1/shtns.egg-info/dependency_links.txt
--rw-r--r--   0 nat       (1000)     1000        6 2023-07-13 12:18:13.000000 shtns-3.6.1/shtns.egg-info/requires.txt
--rw-r--r--   0 nat       (1000)     1000       13 2023-07-13 12:18:13.000000 shtns-3.6.1/shtns.egg-info/top_level.txt
--rw-r--r--   0 nat       (1000)     1000    22950 2023-07-13 12:18:11.000000 shtns-3.6.1/shtns.h
--rw-r--r--   0 nat       (1000)     1000    26180 2023-07-13 12:18:11.000000 shtns-3.6.1/shtns.py
--rw-r--r--   0 nat       (1000)     1000   235692 2023-07-13 12:18:11.000000 shtns-3.6.1/shtns_numpy_wrap.c
--rw-r--r--   0 nat       (1000)     1000    26877 2023-07-13 12:18:11.000000 shtns-3.6.1/shtns_simd.h
--rw-r--r--   0 nat       (1000)     1000    35288 2023-07-13 12:18:11.000000 shtns-3.6.1/time_SHT.c
+drwxr-xr-x   0 nat       (1000)     1000        0 2023-07-21 11:48:35.319600 shtns-3.6.2/
+-rw-r--r--   0 nat       (1000)     1000    13810 2023-07-21 11:48:31.000000 shtns-3.6.2/CHANGELOG.md
+-rw-r--r--   0 nat       (1000)     1000    21782 2023-07-21 11:48:31.000000 shtns-3.6.2/LICENSE
+-rw-r--r--   0 nat       (1000)     1000      126 2023-07-21 11:48:31.000000 shtns-3.6.2/MANIFEST.in
+-rw-r--r--   0 nat       (1000)     1000     4624 2023-07-21 11:48:31.000000 shtns-3.6.2/Makefile.in
+-rw-r--r--   0 nat       (1000)     1000     2182 2023-07-21 11:48:35.319600 shtns-3.6.2/PKG-INFO
+-rw-r--r--   0 nat       (1000)     1000     4415 2023-07-21 11:48:31.000000 shtns-3.6.2/README.md
+drwxr-xr-x   0 nat       (1000)     1000        0 2023-07-21 11:48:35.316266 shtns-3.6.2/SHT/
+-rw-r--r--   0 nat       (1000)     1000     2897 2023-07-21 11:48:31.000000 shtns-3.6.2/SHT/Makefile
+-rw-r--r--   0 nat       (1000)     1000    18709 2023-07-21 11:48:31.000000 shtns-3.6.2/SHT/fly_SH_to_spat.gen.c
+-rw-r--r--   0 nat       (1000)     1000    17015 2023-07-21 11:48:31.000000 shtns-3.6.2/SHT/fly_spat_to_SH.gen.c
+-rw-r--r--   0 nat       (1000)     1000    17493 2023-07-21 11:48:31.000000 shtns-3.6.2/SHT/kernel_SH_to_spat.gen.c
+-rw-r--r--   0 nat       (1000)     1000    23817 2023-07-21 11:48:31.000000 shtns-3.6.2/SHT/kernel_spat_to_SH.gen.c
+-rw-r--r--   0 nat       (1000)     1000    10246 2023-07-21 11:48:31.000000 shtns-3.6.2/SHT/omp_SH_to_spat.gen.c
+-rw-r--r--   0 nat       (1000)     1000     9549 2023-07-21 11:48:31.000000 shtns-3.6.2/SHT/omp_spat_to_SH.gen.c
+-rwxr-xr-x   0 nat       (1000)     1000   198199 2023-07-21 11:48:31.000000 shtns-3.6.2/configure
+drwxr-xr-x   0 nat       (1000)     1000        0 2023-07-21 11:48:35.316266 shtns-3.6.2/fftw3/
+-rw-r--r--   0 nat       (1000)     1000    16196 2023-07-21 11:48:31.000000 shtns-3.6.2/fftw3/cycle.h
+-rw-r--r--   0 nat       (1000)     1000    16691 2023-07-21 11:48:31.000000 shtns-3.6.2/fftw3/fftw3.h
+-rw-r--r--   0 nat       (1000)     1000     2198 2023-07-21 11:48:31.000000 shtns-3.6.2/pyproject.toml
+-rw-r--r--   0 nat       (1000)     1000       38 2023-07-21 11:48:35.319600 shtns-3.6.2/setup.cfg
+-rw-r--r--   0 nat       (1000)     1000     3727 2023-07-21 11:48:31.000000 shtns-3.6.2/setup.py
+-rw-r--r--   0 nat       (1000)     1000    11382 2023-07-21 11:48:31.000000 shtns-3.6.2/sht_com.c
+-rw-r--r--   0 nat       (1000)     1000     4438 2023-07-21 11:48:31.000000 shtns-3.6.2/sht_config.h.in
+-rw-r--r--   0 nat       (1000)     1000     9401 2023-07-21 11:48:31.000000 shtns-3.6.2/sht_fly.c
+-rw-r--r--   0 nat       (1000)     1000    77670 2023-07-21 11:48:31.000000 shtns-3.6.2/sht_func.c
+-rw-r--r--   0 nat       (1000)     1000    70368 2023-07-21 11:48:31.000000 shtns-3.6.2/sht_init.c
+-rw-r--r--   0 nat       (1000)     1000    10553 2023-07-21 11:48:31.000000 shtns-3.6.2/sht_kernels_a.c
+-rw-r--r--   0 nat       (1000)     1000     8448 2023-07-21 11:48:31.000000 shtns-3.6.2/sht_kernels_s.c
+-rw-r--r--   0 nat       (1000)     1000    32326 2023-07-21 11:48:31.000000 shtns-3.6.2/sht_legendre.c
+-rw-r--r--   0 nat       (1000)     1000     6411 2023-07-21 11:48:31.000000 shtns-3.6.2/sht_odd_nlat.c
+-rw-r--r--   0 nat       (1000)     1000     6117 2023-07-21 11:48:31.000000 shtns-3.6.2/sht_omp.c
+-rw-r--r--   0 nat       (1000)     1000    26415 2023-07-21 11:48:31.000000 shtns-3.6.2/sht_private.h
+drwxr-xr-x   0 nat       (1000)     1000        0 2023-07-21 11:48:35.316266 shtns-3.6.2/shtns.egg-info/
+-rw-r--r--   0 nat       (1000)     1000     2182 2023-07-21 11:48:35.000000 shtns-3.6.2/shtns.egg-info/PKG-INFO
+-rw-r--r--   0 nat       (1000)     1000      633 2023-07-21 11:48:35.000000 shtns-3.6.2/shtns.egg-info/SOURCES.txt
+-rw-r--r--   0 nat       (1000)     1000        1 2023-07-21 11:48:35.000000 shtns-3.6.2/shtns.egg-info/dependency_links.txt
+-rw-r--r--   0 nat       (1000)     1000        6 2023-07-21 11:48:35.000000 shtns-3.6.2/shtns.egg-info/requires.txt
+-rw-r--r--   0 nat       (1000)     1000       13 2023-07-21 11:48:35.000000 shtns-3.6.2/shtns.egg-info/top_level.txt
+-rw-r--r--   0 nat       (1000)     1000    22950 2023-07-21 11:48:31.000000 shtns-3.6.2/shtns.h
+-rw-r--r--   0 nat       (1000)     1000    26180 2023-07-21 11:48:31.000000 shtns-3.6.2/shtns.py
+-rw-r--r--   0 nat       (1000)     1000   235692 2023-07-21 11:48:31.000000 shtns-3.6.2/shtns_numpy_wrap.c
+-rw-r--r--   0 nat       (1000)     1000    26877 2023-07-21 11:48:31.000000 shtns-3.6.2/shtns_simd.h
+-rw-r--r--   0 nat       (1000)     1000    35288 2023-07-21 11:48:31.000000 shtns-3.6.2/time_SHT.c
```

### Comparing `shtns-3.6.1/CHANGELOG.md` & `shtns-3.6.2/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 SHTNS CHANGE LOG:
 -----------------
 
+* v3.6.1  (13 Jul 2023)
+	- better python module installation, using `pip install shtns` (thanks to all testers!)
+	- float (single precision) vector transforms supported on GPU.
+	- fix `shallow_water.py` example to work with recent numpy (thanks to P. Personnettaz)
+	- better nested openmp parallelism support (thanks to M. Schreiber)
+
 * v3.6  (30 May 2023)
 	- Rewrite of GPU transforms, with important performance improvements.
 	- New support for AMD GPU MI100 and MI200 series.
 	- Switch to VkFFT for the FFTs on GPU by default.
 	- New batch transforms: especially useful on GPU for smaller transforms (lmax<1000).
 	- Remove useless `shtns_use_gpu()` function.
```

### Comparing `shtns-3.6.1/LICENSE` & `shtns-3.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `shtns-3.6.1/Makefile.in` & `shtns-3.6.2/Makefile.in`

 * *Files 16% similar despite different names*

```diff
@@ -109,29 +109,20 @@
 	$(MAKE) clean -C SHT
 	rm -f $(objs) $(libname)
 	rm -rf doc/html
 	rm -rf doc/latex
 	rm -rf build
 
 
-# build a python interface using SWIG.
-# use it with "from shtns import *" in a python program/shell
-_shtns.so : shtns_numpy_wrap.c Makefile $(hfiles) $(objs)
-	CC="$(CC)" $(PYTHON) setup.py build
-	@echo "*****************************************************************************************"
-	@echo "*** Now, for system wide install, run 'make install' as root.                           *"
-	@echo "*** Otherwise run '$(PYTHON) setup.py install --user' to install for current user only. *"
-	@echo "*****************************************************************************************"
-
 # generate python and c glue code with SWIG.
 shtns_numpy_wrap.c : shtns_numpy.i sht_private.h shtns.h
 	-swig -python shtns_numpy.i
 
-install-py : _shtns.so
-	$(PYTHON) setup.py install
+install-py :
+	pip install shtns
 
 .PHONY : install install-py install-lib clean docs
 
 
 #fftw compiling options :
 #-O3 -fomit-frame-pointer -fstrict-aliasing -ffast-math -fno-schedule-insns -fno-web -fno-loop-optimize --param inline-unit-growth=1000 --param large-function-growth=1000
```

### Comparing `shtns-3.6.1/PKG-INFO` & `shtns-3.6.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: shtns
-Version: 3.6.1
+Version: 3.6.2
 Summary: High performance Spherical Harmonic Transform
 Home-page: https://bitbucket.org/nschaeff/shtns
 Author: Nathanael Schaeffer
 Author-email: Nathanael Schaeffer <nathanael.schaeffer@gmail.com>
+Project-URL: Homepage, https://bitbucket.org/nschaeff/shtns/
 Project-URL: Documentation, https://nschaeff.bitbucket.io/shtns/
-Project-URL: Source, https://bitbucket.org/nschaeff/shtns/
+Project-URL: Repository, https://bitbucket.org/nschaeff/shtns/
 Project-URL: Changelog, https://bitbucket.org/nschaeff/shtns/src/master/CHANGELOG.md
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: CEA CNRS Inria Logiciel Libre License, version 2.1 (CeCILL-2.1)
 Classifier: Intended Audience :: Science/Research
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Scientific/Engineering
 Requires: numpy
 Requires-Python: >=3.2
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-
 This is the python module to use **SHTns, a high performance spherical harmonic transform and rotation** library.
 It requires FFTW installed in your system.
 
 ## GETTING STARTED
 
 ### Basic Installation:
 - make sure FFTW is installed in your system; if not, install it using your system package manager.
@@ -31,12 +31,19 @@
 
     `pip install shtns`
 
 This simple installation should work and be enough for most use cases.
 However, **in order to have the highest possible performance, FFTW should be compiled and tuned for your machine**,
 which is not the case with pre-compiled system packages.
 
+### Cuda GPU support:
+Make sure the environment variable `CUDA_PATH` points to the installed cuda toolkit before running `pip install shtns`.
+This will automatically add transparent support for nvidia gpus, in "offload" mode (that means data transfers are
+performed by shtns).
+
 ### Example code:
-See <https://bitbucket.org/nschaeff/shtns/src/master/example/shallow_water.py>
+See <https://bitbucket.org/nschaeff/shtns/src/master/examples/SHT_example.py>
+and <https://bitbucket.org/nschaeff/shtns/src/master/examples/shallow_water.py>.
+For using the GPU from python, see <https://bitbucket.org/nschaeff/shtns/src/master/examples/SHT_gpu_example.py>
 
 ## MORE INFO
 See <https://bitbucket.org/nschaeff/shtns/src/master/README.md>
```

### Comparing `shtns-3.6.1/README.md` & `shtns-3.6.2/README.md`

 * *Files identical despite different names*

### Comparing `shtns-3.6.1/SHT/Makefile` & `shtns-3.6.2/SHT/Makefile`

 * *Files identical despite different names*

### Comparing `shtns-3.6.1/SHT/fly_SH_to_spat.gen.c` & `shtns-3.6.2/SHT/fly_SH_to_spat.gen.c`

 * *Files identical despite different names*

### Comparing `shtns-3.6.1/SHT/fly_spat_to_SH.gen.c` & `shtns-3.6.2/SHT/fly_spat_to_SH.gen.c`

 * *Files identical despite different names*

### Comparing `shtns-3.6.1/SHT/kernel_SH_to_spat.gen.c` & `shtns-3.6.2/SHT/kernel_SH_to_spat.gen.c`

 * *Files identical despite different names*

### Comparing `shtns-3.6.1/SHT/kernel_spat_to_SH.gen.c` & `shtns-3.6.2/SHT/kernel_spat_to_SH.gen.c`

 * *Files identical despite different names*

### Comparing `shtns-3.6.1/SHT/omp_SH_to_spat.gen.c` & `shtns-3.6.2/SHT/omp_SH_to_spat.gen.c`

 * *Files identical despite different names*

### Comparing `shtns-3.6.1/SHT/omp_spat_to_SH.gen.c` & `shtns-3.6.2/SHT/omp_spat_to_SH.gen.c`

 * *Files identical despite different names*

### Comparing `shtns-3.6.1/configure` & `shtns-3.6.2/configure`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #! /bin/sh
 # Guess values for system-dependent variables and create Makefiles.
-# Generated by GNU Autoconf 2.71 for SHTns 3.6.
+# Generated by GNU Autoconf 2.71 for SHTns 3.6.1.
 #
 #
 # Copyright (C) 1992-1996, 1998-2017, 2020-2021 Free Software Foundation,
 # Inc.
 #
 #
 # This configure script is free software; the Free Software Foundation
@@ -604,16 +604,16 @@
 subdirs=
 MFLAGS=
 MAKEFLAGS=
 
 # Identity of this package.
 PACKAGE_NAME='SHTns'
 PACKAGE_TARNAME='shtns'
-PACKAGE_VERSION='3.6'
-PACKAGE_STRING='SHTns 3.6'
+PACKAGE_VERSION='3.6.1'
+PACKAGE_STRING='SHTns 3.6.1'
 PACKAGE_BUGREPORT=''
 PACKAGE_URL='https://bitbucket.org/nschaeff/shtns'
 
 ac_unique_file="sht_init.c"
 # Factoring default headers for most tests.
 ac_includes_default="\
 #include <stddef.h>
@@ -664,15 +664,14 @@
 OBJEXT
 EXEEXT
 ac_ct_CC
 CPPFLAGS
 LDFLAGS
 CFLAGS
 CC
-PYTHON
 target_alias
 host_alias
 build_alias
 LIBS
 ECHO_T
 ECHO_N
 ECHO_C
@@ -725,15 +724,14 @@
 enable_ishioka
 enable_kernel_compiler
 enable_march
 '
       ac_precious_vars='build_alias
 host_alias
 target_alias
-PYTHON
 CC
 CFLAGS
 LDFLAGS
 LIBS
 CPPFLAGS
 FC
 FCFLAGS'
@@ -1281,15 +1279,15 @@
 #
 # Report the --help message.
 #
 if test "$ac_init_help" = "long"; then
   # Omit some internal or obsolete options to make the list less imposing.
   # This message is too long to be a string in the A/UX 3.1 sh.
   cat <<_ACEOF
-\`configure' configures SHTns 3.6 to adapt to many kinds of systems.
+\`configure' configures SHTns 3.6.1 to adapt to many kinds of systems.
 
 Usage: $0 [OPTION]... [VAR=VALUE]...
 
 To assign environment variables (e.g., CC, CFLAGS...), specify them as
 VAR=VALUE.  See below for descriptions of some of the useful variables.
 
 Defaults for the options are specified in brackets.
@@ -1343,15 +1341,15 @@
 
   cat <<\_ACEOF
 _ACEOF
 fi
 
 if test -n "$ac_init_help"; then
   case $ac_init_help in
-     short | recursive ) echo "Configuration of SHTns 3.6:";;
+     short | recursive ) echo "Configuration of SHTns 3.6.1:";;
    esac
   cat <<\_ACEOF
 
 Optional Features:
   --disable-option-checking  ignore unrecognized --enable/--with options
   --disable-FEATURE       do not include FEATURE (same as --enable-FEATURE=no)
   --enable-FEATURE[=ARG]  include FEATURE [ARG=yes]
@@ -1381,15 +1379,14 @@
                           (default=gcc)
   --enable-march=native   select target cpu architecture with a -march=XXX
                           compiler option (for gcc, icc and clang) (default:
                           XXX=native for best performance)
   --disable-openmp        do not use OpenMP
 
 Some influential environment variables:
-  PYTHON      the python interpreter (defaults to 'python')
   CC          C compiler command
   CFLAGS      C compiler flags
   LDFLAGS     linker flags, e.g. -L<lib dir> if you have libraries in a
               nonstandard directory <lib dir>
   LIBS        libraries to pass to the linker, e.g. -l<library>
   CPPFLAGS    (Objective) C/C++ preprocessor flags, e.g. -I<include dir> if
               you have headers in a nonstandard directory <include dir>
@@ -1460,15 +1457,15 @@
     cd "$ac_pwd" || { ac_status=$?; break; }
   done
 fi
 
 test -n "$ac_init_help" && exit $ac_status
 if $ac_init_version; then
   cat <<\_ACEOF
-SHTns configure 3.6
+SHTns configure 3.6.1
 generated by GNU Autoconf 2.71
 
 Copyright (C) 2021 Free Software Foundation, Inc.
 This configure script is free software; the Free Software Foundation
 gives unlimited permission to copy, distribute and modify it.
 _ACEOF
   exit
@@ -1774,15 +1771,15 @@
     ac_configure_args_raw=`      printf "%s\n" "$ac_configure_args_raw" | sed "$ac_safe_unquote"`;;
 esac
 
 cat >config.log <<_ACEOF
 This file contains any messages produced by compilers while
 running configure, to aid debugging if configure makes a mistake.
 
-It was created by SHTns $as_me 3.6, which was
+It was created by SHTns $as_me 3.6.1, which was
 generated by GNU Autoconf 2.71.  Invocation command line was
 
   $ $0$ac_configure_args_raw
 
 _ACEOF
 exec 5>>config.log
 {
@@ -2444,16 +2441,14 @@
 
 ac_config_headers="$ac_config_headers sht_config.h"
 
 target="libshtns.a"		# by default, build the library.
 objs="sht_fly.o"
 install="install-lib"	# by default, install the library.
 
-# optional variables :
-
 # optional features with --enable-XXX
 # Check whether --enable-verbose was given.
 if test ${enable_verbose+y}
 then :
   enableval=$enable_verbose;
 else $as_nop
   enable_verbose=1
@@ -4496,22 +4491,25 @@
   LIBS="-lm $LIBS"
 
 else $as_nop
   as_fn_error $? "math library not found." "$LINENO" 5
 fi
 
 
-# With Python, enable openmp by default.
+# Checks related to Python:
 if test "x$enable_python" != "xno"
 then :
 
 	if test "x$enable_openmp" = "xdefault"
 then :
   enable_openmp=yes
-fi
+fi   # enable openmp by default
+	CFLAGS="$CFLAGS -fpic"	# required compile flag for python extensions.
+	CFLAGS2="$CFLAGS2 -fpic"	# required compile flag for python extensions.
+	install="install-py"	# install python extension instead of C library.
 
 fi
 
 # for MagIC code, also disable matrix transforms.
 if test "x$enable_magic_layout" != "xno"
 then :
 
@@ -5000,14 +4998,20 @@
 	if test "x$enable_openmp" = "xyes"
 then :
 
 	    gpu_compile="$gpu_compile -Xcompiler -fopenmp"
 	    target="libshtns_cuda_omp.a"
 
 fi
+	if test "x$enable_python" != "xno"
+then :
+
+	    gpu_compile="$gpu_compile -Xcompiler -fpic"
+
+fi
 	LIBS="$LIBS -lstdc++"	# cuda uses the c++ standard library. This is needed to link with gcc
 	{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for vkfft/vkFFT.h" >&5
 printf %s "checking for vkfft/vkFFT.h... " >&6; }
 if test ${ac_cv_file_vkfft_vkFFT_h+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
@@ -5026,15 +5030,15 @@
 
 printf "%s\n" "#define VKFFT_BACKEND 1" >>confdefs.h
 
 fi
 
 
 fi
-libname=$target		# set the libname befor checking for python.
+libname=$target
 
 # Check for FFTW (MKL preferred, FFTW optional)
 if test "x$enable_mkl" == "xyes"
 then :
 
   mkl_found=no
 
@@ -5275,62 +5279,14 @@
 fi
 
 
 fi
 
 fi
 
-
-# Checks related to Python and NumPy paths:
-if test "x$enable_python" != "xno"
-then :
-
-	if test "x$PYTHON" = "x"
-then :
-
-		{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for python with numpy package" >&5
-printf %s "checking for python with numpy package... " >&6; }
-		py_test="python python2 python3"
-
-else $as_nop
-
-		{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking if $PYTHON has numpy package" >&5
-printf %s "checking if $PYTHON has numpy package... " >&6; }
-		py_test="$PYTHON"
-
-fi
-	for py in $py_test
-	do :
-		numpy_inc=`$py -c "from numpy import get_include; print(get_include())" 2>/dev/null`
-		if test "x$numpy_inc" != "x"
-then :
-  break
-fi
-	done
-	if test "x$numpy_inc" = "x"
-then :
-
-		{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: no" >&5
-printf "%s\n" "no" >&6; }
-		as_fn_error $? "NumPy package is required for the python interface." "$LINENO" 5
-
-else $as_nop
-
-		{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $py" >&5
-printf "%s\n" "$py" >&6; }
-		PYTHON=$py
-
-fi
-	CFLAGS="$CFLAGS -fpic"	# required compile flag for python extensions.
-	CFLAGS2="$CFLAGS2 -fpic"	# required compile flag for python extensions.
-	target="_shtns.so"	# build python extension instead of C library.
-	install="install-py"	# install python extension instead of C library.
-
-fi
-
 # Checks related to long double
 if test "x$enable_long_double" == "xyes"
 then :
 
 
   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for long double with more range or precision than double" >&5
 printf %s "checking for long double with more range or precision than double... " >&6; }
@@ -6334,15 +6290,15 @@
 test $as_write_fail = 0 && chmod +x $CONFIG_STATUS || ac_write_fail=1
 
 cat >>$CONFIG_STATUS <<\_ACEOF || ac_write_fail=1
 # Save the log message, to keep $0 and so on meaningful, and to
 # report actual input values of CONFIG_FILES etc. instead of their
 # values after options handling.
 ac_log="
-This file was extended by SHTns $as_me 3.6, which was
+This file was extended by SHTns $as_me 3.6.1, which was
 generated by GNU Autoconf 2.71.  Invocation command line was
 
   CONFIG_FILES    = $CONFIG_FILES
   CONFIG_HEADERS  = $CONFIG_HEADERS
   CONFIG_LINKS    = $CONFIG_LINKS
   CONFIG_COMMANDS = $CONFIG_COMMANDS
   $ $0 $@
@@ -6399,15 +6355,15 @@
 
 _ACEOF
 ac_cs_config=`printf "%s\n" "$ac_configure_args" | sed "$ac_safe_unquote"`
 ac_cs_config_escaped=`printf "%s\n" "$ac_cs_config" | sed "s/^ //; s/'/'\\\\\\\\''/g"`
 cat >>$CONFIG_STATUS <<_ACEOF || ac_write_fail=1
 ac_cs_config='$ac_cs_config_escaped'
 ac_cs_version="\\
-SHTns config.status 3.6
+SHTns config.status 3.6.1
 configured by $0, generated by GNU Autoconf 2.71,
   with options \\"\$ac_cs_config\\"
 
 Copyright (C) 2021 Free Software Foundation, Inc.
 This config.status script is free software; the Free Software Foundation
 gives unlimited permission to copy, distribute and modify it."
```

### Comparing `shtns-3.6.1/fftw3/cycle.h` & `shtns-3.6.2/fftw3/cycle.h`

 * *Files identical despite different names*

### Comparing `shtns-3.6.1/fftw3/fftw3.h` & `shtns-3.6.2/fftw3/fftw3.h`

 * *Files identical despite different names*

### Comparing `shtns-3.6.1/setup.py` & `shtns-3.6.2/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,37 +3,14 @@
 # and https://stackoverflow.com/questions/42585210/extending-setuptools-extension-to-use-cmake-in-setup-py
 
 from setuptools import setup, Extension
 from setuptools.command.build_ext import build_ext, new_compiler, customize_compiler
 from numpy import get_include
 import os,sys
 
-long_description = """
-This is the python module to use **SHTns, a high performance spherical harmonic transform and rotation** library.
-It requires FFTW installed in your system.
-
-## GETTING STARTED
-
-### Basic Installation:
-- make sure FFTW is installed in your system; if not, install it using your system package manager.
-- run:
-
-    `pip install shtns`
-
-This simple installation should work and be enough for most use cases.
-However, **in order to have the highest possible performance, FFTW should be compiled and tuned for your machine**,
-which is not the case with pre-compiled system packages.
-
-### Example code:
-See <https://bitbucket.org/nschaeff/shtns/src/master/example/shallow_water.py>
-
-## MORE INFO
-See <https://bitbucket.org/nschaeff/shtns/src/master/README.md>
-"""
-
 def getver():
     with open('CHANGELOG.md') as f:
         for l in f:
             s=l.find('* v')
             if s>=0:
                 return l[s+3:].split()[0]
     return 'unknown'
@@ -53,19 +30,19 @@
     ccompiler = new_compiler()
     customize_compiler(ccompiler)
     openmp_ok = True
     with tempfile.TemporaryDirectory() as tmp_dir:
         start_dir = os.path.abspath('.')
         try:
             os.chdir(tmp_dir)
-            # Use sht_init.c as test program (will also test fftw openmp support!)
+            # Write source of test program (will also test fftw openmp support!)
             with open('test_openmp.c', 'w') as f:
                 f.write(OPENMP_TEST_C)
             os.mkdir('objects')
-            # Compile, test program
+            # Compile test program
             ccompiler.compile(['test_openmp.c'], output_dir='objects', extra_postargs=[omp_flags, "-I"+start_dir])
             # Link test program with fftw3_omp library
             objects = glob.glob(os.path.join('objects', '*' + ccompiler.obj_extension))
             ccompiler.link_executable(objects, 'test_openmp', extra_postargs=[omp_flags, "-lfftw3_omp"])
         except Exception:
             openmp_ok = False
         finally:
@@ -75,14 +52,23 @@
 numpy_inc = get_include()               #  NumPy include path.
 shtns_o = "sht_init.o sht_kernels_a.o sht_kernels_s.o sht_odd_nlat.o sht_fly.o sht_omp.o".split()
 libdir = []
 cargs = ['-std=c99', '-DSHTNS_VER="' + getver() +'"']
 libs = ['fftw3', 'm']
 config_cmd = ['./configure','--enable-python','--prefix='+sys.prefix]
 
+## for cuda support:
+cuda_path = os.environ.get('CUDA_PATH')
+if cuda_path is not None:
+    config_cmd.append('--enable-cuda')
+    cargs.append('-I' + cuda_path + '/include')
+    libdir.extend([cuda_path + '/lib64', cuda_path + '/lib64/stubs'])
+    libs.extend(['cudart','nvrtc','cuda','stdc++'])
+    shtns_o.append('sht_gpu.o')
+
 use_openmp = os.environ.get('SHTNS_OPENMP', '1') != '0'   # allows to disable openmp with environment variable SHTNS_OPENMP=0
 if use_openmp:
     use_openmp = check_openmp_support()
 if use_openmp:
     cargs.append('-fopenmp')
     libs.insert(0,'fftw3_omp')
 else:
@@ -104,18 +90,11 @@
 setup(name='shtns',
     cmdclass={'build_ext': make },
         version=getver(),
         description='High performance Spherical Harmonic Transform',
         author='Nathanael Schaeffer',
         author_email='nathanael.schaeffer@univ-grenoble-alpes.fr',
         url='https://bitbucket.org/nschaeff/shtns',
-        project_urls={
-            "Documentation": "https://nschaeff.bitbucket.io/shtns/",
-            "Source": "https://bitbucket.org/nschaeff/shtns/",
-            "Changelog": "https://bitbucket.org/nschaeff/shtns/src/master/CHANGELOG.md",
-        },
-        long_description=long_description,
-        long_description_content_type='text/markdown',
         ext_modules=[shtns_module],
         py_modules=["shtns"],
         requires=["numpy"],
         )
```

### Comparing `shtns-3.6.1/sht_com.c` & `shtns-3.6.2/sht_com.c`

 * *Files identical despite different names*

### Comparing `shtns-3.6.1/sht_config.h.in` & `shtns-3.6.2/sht_config.h.in`

 * *Files identical despite different names*

### Comparing `shtns-3.6.1/sht_fly.c` & `shtns-3.6.2/sht_fly.c`

 * *Files identical despite different names*

### Comparing `shtns-3.6.1/sht_func.c` & `shtns-3.6.2/sht_func.c`

 * *Files identical despite different names*

### Comparing `shtns-3.6.1/sht_init.c` & `shtns-3.6.2/sht_init.c`

 * *Files identical despite different names*

### Comparing `shtns-3.6.1/sht_kernels_a.c` & `shtns-3.6.2/sht_kernels_a.c`

 * *Files identical despite different names*

### Comparing `shtns-3.6.1/sht_kernels_s.c` & `shtns-3.6.2/sht_kernels_s.c`

 * *Files identical despite different names*

### Comparing `shtns-3.6.1/sht_legendre.c` & `shtns-3.6.2/sht_legendre.c`

 * *Files identical despite different names*

### Comparing `shtns-3.6.1/sht_odd_nlat.c` & `shtns-3.6.2/sht_odd_nlat.c`

 * *Files identical despite different names*

### Comparing `shtns-3.6.1/sht_omp.c` & `shtns-3.6.2/sht_omp.c`

 * *Files identical despite different names*

### Comparing `shtns-3.6.1/sht_private.h` & `shtns-3.6.2/sht_private.h`

 * *Files identical despite different names*

### Comparing `shtns-3.6.1/shtns.egg-info/PKG-INFO` & `shtns-3.6.2/shtns.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: shtns
-Version: 3.6.1
+Version: 3.6.2
 Summary: High performance Spherical Harmonic Transform
 Home-page: https://bitbucket.org/nschaeff/shtns
 Author: Nathanael Schaeffer
 Author-email: Nathanael Schaeffer <nathanael.schaeffer@gmail.com>
+Project-URL: Homepage, https://bitbucket.org/nschaeff/shtns/
 Project-URL: Documentation, https://nschaeff.bitbucket.io/shtns/
-Project-URL: Source, https://bitbucket.org/nschaeff/shtns/
+Project-URL: Repository, https://bitbucket.org/nschaeff/shtns/
 Project-URL: Changelog, https://bitbucket.org/nschaeff/shtns/src/master/CHANGELOG.md
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: CEA CNRS Inria Logiciel Libre License, version 2.1 (CeCILL-2.1)
 Classifier: Intended Audience :: Science/Research
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Scientific/Engineering
 Requires: numpy
 Requires-Python: >=3.2
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-
 This is the python module to use **SHTns, a high performance spherical harmonic transform and rotation** library.
 It requires FFTW installed in your system.
 
 ## GETTING STARTED
 
 ### Basic Installation:
 - make sure FFTW is installed in your system; if not, install it using your system package manager.
@@ -31,12 +31,19 @@
 
     `pip install shtns`
 
 This simple installation should work and be enough for most use cases.
 However, **in order to have the highest possible performance, FFTW should be compiled and tuned for your machine**,
 which is not the case with pre-compiled system packages.
 
+### Cuda GPU support:
+Make sure the environment variable `CUDA_PATH` points to the installed cuda toolkit before running `pip install shtns`.
+This will automatically add transparent support for nvidia gpus, in "offload" mode (that means data transfers are
+performed by shtns).
+
 ### Example code:
-See <https://bitbucket.org/nschaeff/shtns/src/master/example/shallow_water.py>
+See <https://bitbucket.org/nschaeff/shtns/src/master/examples/SHT_example.py>
+and <https://bitbucket.org/nschaeff/shtns/src/master/examples/shallow_water.py>.
+For using the GPU from python, see <https://bitbucket.org/nschaeff/shtns/src/master/examples/SHT_gpu_example.py>
 
 ## MORE INFO
 See <https://bitbucket.org/nschaeff/shtns/src/master/README.md>
```

### Comparing `shtns-3.6.1/shtns.egg-info/SOURCES.txt` & `shtns-3.6.2/shtns.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `shtns-3.6.1/shtns.h` & `shtns-3.6.2/shtns.h`

 * *Files identical despite different names*

### Comparing `shtns-3.6.1/shtns.py` & `shtns-3.6.2/shtns.py`

 * *Files identical despite different names*

### Comparing `shtns-3.6.1/shtns_numpy_wrap.c` & `shtns-3.6.2/shtns_numpy_wrap.c`

 * *Files identical despite different names*

### Comparing `shtns-3.6.1/shtns_simd.h` & `shtns-3.6.2/shtns_simd.h`

 * *Files identical despite different names*

### Comparing `shtns-3.6.1/time_SHT.c` & `shtns-3.6.2/time_SHT.c`

 * *Files identical despite different names*

