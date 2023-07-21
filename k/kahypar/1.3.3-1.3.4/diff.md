# Comparing `tmp/kahypar-1.3.3-pp39-pypy39_pp73-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip` & `tmp/kahypar-1.3.4-cp39-cp39-macosx_11_0_arm64.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,10 @@
-Zip file size: 1124870 bytes, number of entries: 11
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-23 00:31 kahypar.libs/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-23 00:31 kahypar-1.3.3.dist-info/
--rwxr-xr-x  2.0 unx  3052193 b- defN 23-May-23 00:31 kahypar.pypy39-pp73-x86_64-linux-gnu.so
--rwxr-xr-x  2.0 unx   868985 b- defN 23-May-23 00:31 kahypar.libs/libboost_program_options-3ad63c06.so.1.69.0
--rw-r--r--  2.0 unx    35148 b- defN 23-May-23 00:31 kahypar-1.3.3.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      162 b- defN 23-May-23 00:31 kahypar-1.3.3.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 23-May-23 00:31 kahypar-1.3.3.dist-info/top_level.txt
--rw-r--r--  2.0 unx    35146 b- defN 23-May-23 00:31 kahypar-1.3.3.dist-info/COPYING
--rw-rw-r--  2.0 unx      791 b- defN 23-May-23 00:31 kahypar-1.3.3.dist-info/RECORD
--rw-r--r--  2.0 unx      339 b- defN 23-May-23 00:31 kahypar-1.3.3.dist-info/AUTHORS
--rw-r--r--  2.0 unx    34652 b- defN 23-May-23 00:31 kahypar-1.3.3.dist-info/METADATA
-11 files, 4027424 bytes uncompressed, 1123298 bytes compressed:  72.1%
+Zip file size: 771274 bytes, number of entries: 8
+-rwxr-xr-x  2.0 unx  2859952 b- defN 23-Jul-21 03:02 kahypar.cpython-39-darwin.so
+-rw-rw-r--  2.0 unx      656 b- defN 23-Jul-21 03:40 kahypar-1.3.4.dist-info/RECORD
+-rw-r--r--  2.0 unx      339 b- defN 23-Jul-21 03:40 kahypar-1.3.4.dist-info/AUTHORS
+-rw-r--r--  2.0 unx      108 b- defN 23-Jul-21 03:40 kahypar-1.3.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx    35146 b- defN 23-Jul-21 03:40 kahypar-1.3.4.dist-info/COPYING
+-rw-r--r--  2.0 unx        8 b- defN 23-Jul-21 03:40 kahypar-1.3.4.dist-info/top_level.txt
+-rw-r--r--  2.0 unx    35148 b- defN 23-Jul-21 03:40 kahypar-1.3.4.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx    35380 b- defN 23-Jul-21 03:40 kahypar-1.3.4.dist-info/METADATA
+8 files, 2966737 bytes uncompressed, 770138 bytes compressed:  74.1%
```

## zipnote {}

```diff
@@ -1,34 +1,25 @@
-Filename: kahypar.libs/
+Filename: kahypar.cpython-39-darwin.so
 Comment: 
 
-Filename: kahypar-1.3.3.dist-info/
+Filename: kahypar-1.3.4.dist-info/RECORD
 Comment: 
 
-Filename: kahypar.pypy39-pp73-x86_64-linux-gnu.so
+Filename: kahypar-1.3.4.dist-info/AUTHORS
 Comment: 
 
-Filename: kahypar.libs/libboost_program_options-3ad63c06.so.1.69.0
+Filename: kahypar-1.3.4.dist-info/WHEEL
 Comment: 
 
-Filename: kahypar-1.3.3.dist-info/LICENSE.txt
+Filename: kahypar-1.3.4.dist-info/COPYING
 Comment: 
 
-Filename: kahypar-1.3.3.dist-info/WHEEL
+Filename: kahypar-1.3.4.dist-info/top_level.txt
 Comment: 
 
-Filename: kahypar-1.3.3.dist-info/top_level.txt
+Filename: kahypar-1.3.4.dist-info/LICENSE.txt
 Comment: 
 
-Filename: kahypar-1.3.3.dist-info/COPYING
-Comment: 
-
-Filename: kahypar-1.3.3.dist-info/RECORD
-Comment: 
-
-Filename: kahypar-1.3.3.dist-info/AUTHORS
-Comment: 
-
-Filename: kahypar-1.3.3.dist-info/METADATA
+Filename: kahypar-1.3.4.dist-info/METADATA
 Comment: 
 
 Zip file comment:
```

## filetype from file(1)

```diff
@@ -1 +1 @@
-Zip archive data, at least v2.0 to extract, compression method=store
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## Comparing `kahypar-1.3.3.dist-info/LICENSE.txt` & `kahypar-1.3.4.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `kahypar-1.3.3.dist-info/COPYING` & `kahypar-1.3.4.dist-info/COPYING`

 * *Files identical despite different names*

## Comparing `kahypar-1.3.3.dist-info/METADATA` & `kahypar-1.3.4.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kahypar
-Version: 1.3.3
+Version: 1.3.4
 Summary: Python Inferface for the Karlsruhe Hypergraph Partitioning Framework (KaHyPar)
 Home-page: https://www.kahypar.org
 Author: Sebastian Schlag
 Author-email: kahypar@sebastianschlag.de
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -264,14 +264,23 @@
 
 To start KaHyPar in recursive bisection mode (KaHyPar-R) optimizing the cut-net objective run:
 
     ./KaHyPar -h <path-to-hgr> -k <# blocks> -e <imbalance (e.g. 0.03)> -o cut -m recursive -p ../../../config/old_reference_configs/cut_rb_alenex16.ini
 
 All preset parameters can be overwritten by using the corresponding command line options.
 
+#### Input Validation
+
+When creating a hypergraph KaHyPar validates that the input is actually a correct hypergraph, otherwise printing an error and aborting.
+This applies to hgr input files, the C interface and the Python interface. The runtime cost of the validation should be negligible in almost all cases.
+However, the input validation can also be disabled using the cmake flag `-DKAHYPAR_INPUT_VALIDATION=OFF`.
+
+Additionally, warnings are printed for non-fatal issues (e.g. hyperedges with duplicate pins).
+To treat non-fatal issues as hard errors instead, use the cmake flag `-DKAHYPAR_INPUT_VALIDATION_PROMOTE_WARNINGS_TO_ERRORS=ON`.
+
 Using the Library Interfaces
 -----------
 
 #### The C-Style Interface
 We provide a simple C-style interface to use KaHyPar as a library. Note that this interface is not thread-safe yet. However there are some existing [workarounds](https://github.com/kahypar/kahypar/issues/142#issuecomment-1410015774). The library can be built and installed via
 
 ```sh
@@ -338,17 +347,19 @@
 
   kahypar_context_free(context);
 }
 ```
 To compile the program using `g++` run:
 
 ```sh
-g++ -std=c++14 -DNDEBUG -O3 -I/usr/local/include -L/usr/local/lib -lkahypar -L/path/to/boost/lib -I/path/to/boost/include -lboost_program_options program.cc -o program
+g++ -std=c++14 -DNDEBUG -O3 -I/usr/local/include -L/usr/local/lib program.cc -o program -lkahypar
 ```
 
+Note: If boost is not found during linking, you might need to add `-L/path/to/boost/lib -I/path/to/boost/include -lboost_program_options` to the command.
+
 To remove the library from your system use the provided uninstall target:
 
 ```sh
 make uninstall-kahypar
 ```
 #### The Python Interface
 To compile the Python interface, do the following:
```

