# Comparing `tmp/cppbktree-0.0.1.tar.gz` & `tmp/cppbktree-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cppbktree-0.0.1.tar", last modified: Sun Jul  5 18:12:20 2020, max compression
+gzip compressed data, was "cppbktree-0.1.0.tar", last modified: Fri Jul 21 15:15:07 2023, max compression
```

## Comparing `cppbktree-0.0.1.tar` & `cppbktree-0.1.0.tar`

### file list

```diff
@@ -1,16 +1,20 @@
-drwxrwxr-x   0 hypatia   (1000) hypatia   (1000)        0 2020-07-05 18:12:20.836029 cppbktree-0.0.1/
--rwxrwxr-x   0 hypatia   (1000) hypatia   (1000)     1070 2020-07-05 17:40:27.000000 cppbktree-0.0.1/LICENSE
--rwxrwxr-x   0 hypatia   (1000) hypatia   (1000)      233 2020-07-05 17:40:27.000000 cppbktree-0.0.1/MANIFEST.in
--rw-rw-r--   0 hypatia   (1000) hypatia   (1000)     5831 2020-07-05 18:12:20.836029 cppbktree-0.0.1/PKG-INFO
--rwxrwxr-x   0 hypatia   (1000) hypatia   (1000)     4584 2020-07-05 17:40:27.000000 cppbktree-0.0.1/README.md
-drwxrwxr-x   0 hypatia   (1000) hypatia   (1000)        0 2020-07-05 18:12:20.836029 cppbktree-0.0.1/cppbktree/
--rw-rw-r--   0 hypatia   (1000) hypatia   (1000)   265374 2020-07-05 17:40:27.000000 cppbktree-0.0.1/cppbktree/cppbktree.cpp
--rwxrwxr-x   0 hypatia   (1000) hypatia   (1000)    12670 2020-07-05 17:40:27.000000 cppbktree-0.0.1/cppbktree/cppbktree.hpp
--rwxrwxr-x   0 hypatia   (1000) hypatia   (1000)     3170 2020-07-05 17:40:27.000000 cppbktree-0.0.1/cppbktree/cppbktree.pyx
-drwxrwxr-x   0 hypatia   (1000) hypatia   (1000)        0 2020-07-05 18:12:20.836029 cppbktree-0.0.1/cppbktree.egg-info/
--rw-rw-r--   0 hypatia   (1000) hypatia   (1000)     5831 2020-07-05 18:12:20.000000 cppbktree-0.0.1/cppbktree.egg-info/PKG-INFO
--rw-rw-r--   0 hypatia   (1000) hypatia   (1000)      242 2020-07-05 18:12:20.000000 cppbktree-0.0.1/cppbktree.egg-info/SOURCES.txt
--rw-rw-r--   0 hypatia   (1000) hypatia   (1000)        1 2020-07-05 18:12:20.000000 cppbktree-0.0.1/cppbktree.egg-info/dependency_links.txt
--rw-rw-r--   0 hypatia   (1000) hypatia   (1000)       10 2020-07-05 18:12:20.000000 cppbktree-0.0.1/cppbktree.egg-info/top_level.txt
--rw-rw-r--   0 hypatia   (1000) hypatia   (1000)       38 2020-07-05 18:12:20.836029 cppbktree-0.0.1/setup.cfg
--rwxrwxr-x   0 hypatia   (1000) hypatia   (1000)     1718 2020-07-05 17:40:27.000000 cppbktree-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:15:07.854271 cppbktree-0.1.0/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1070 2023-07-21 15:14:48.000000 cppbktree-0.1.0/LICENSE
+-rwxr-xr-x   0 runner    (1001) docker     (123)      233 2023-07-21 15:14:48.000000 cppbktree-0.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7955 2023-07-21 15:15:07.854271 cppbktree-0.1.0/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6813 2023-07-21 15:14:48.000000 cppbktree-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:15:07.854271 cppbktree-0.1.0/cppbktree/
+-rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-07-21 15:14:48.000000 cppbktree-0.1.0/cppbktree/AlignedAllocator.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-07-21 15:14:48.000000 cppbktree-0.1.0/cppbktree/LinearLookup.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-07-21 15:14:48.000000 cppbktree-0.1.0/cppbktree/TestHelpers.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)   625270 2023-07-21 15:15:07.000000 cppbktree-0.1.0/cppbktree/cppbktree.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17619 2023-07-21 15:14:48.000000 cppbktree-0.1.0/cppbktree/cppbktree.hpp
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6901 2023-07-21 15:14:48.000000 cppbktree-0.1.0/cppbktree/cppbktree.pyx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:15:07.854271 cppbktree-0.1.0/cppbktree.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7955 2023-07-21 15:15:07.000000 cppbktree-0.1.0/cppbktree.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-07-21 15:15:07.000000 cppbktree-0.1.0/cppbktree.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 15:15:07.000000 cppbktree-0.1.0/cppbktree.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-21 15:15:07.000000 cppbktree-0.1.0/cppbktree.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-07-21 15:14:48.000000 cppbktree-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-07-21 15:15:07.854271 cppbktree-0.1.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4346 2023-07-21 15:14:48.000000 cppbktree-0.1.0/setup.py
```

### Comparing `cppbktree-0.0.1/LICENSE` & `cppbktree-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cppbktree-0.0.1/PKG-INFO` & `cppbktree-0.1.0/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,106 +1,135 @@
-Metadata-Version: 2.1
-Name: cppbktree
-Version: 0.0.1
-Summary: C++ Implementation of a Burkhard-Keller Tree (BK-Tree)
-Home-page: https://github.com/mxmlnkn/cppbktree
-Author: Maximilian Knespel
-Author-email: mxmlnkn@github.de
-License: MIT
-Description: # C++ BK-Tree
-        
-        [![PyPI version](https://badge.fury.io/py/cppbktree.svg)](https://badge.fury.io/py/cppbktree)
-        [![Downloads](https://pepy.tech/badge/cppbktree/month)](https://pepy.tech/project/cppbktree/month)
-        [![License](https://img.shields.io/badge/license-MIT-blue.svg)](http://opensource.org/licenses/MIT)
-        [![Build Status](https://travis-ci.org/mxmlnkn/cppbktree.svg?branch=master)](https://travis-ci.com/mxmlnkn/cppbktree)
-        
-        This module provides a BK-Tree class written in C++ to hopefully better speed than pure-python solutions.
-        
-        
-        # Installation
-        
-        You can simply install it from PyPI:
-        ```
-        pip install cppbktree
-        ```
-        
-        # Usage
-        
-        ```python3
-        from cppbktree import BKTree
-        
-        tree = BKTree( [ bytes( [ x ] ) for x in [0, 4, 5, 14] ] )
-        tree.add( bytes( [ 15 ] ) )
-        print( tree.find( 13, 1 ) )
-        ```
-        
-        Because of the Python/C++ interface, currently this BK-Tree is limited to only hamming distances of bytearrays.
-        Pull requests are welcome.
-        
-        # Benchmarks
-        
-        The benchmark consists of inserting a varying amount of random 64-bit elements into the tree and then querying a value at varying distances.
-        This is done five times to get a hint for the standard deviation as is plotted with error bars.
-        
-        ## Comparison pybktree vs. cppbktree
-        
-        ![Comparison pybktree cppbktree](results/compare-scalings-pybktree-cppbktree.png)
-        
-        In this log-log plot, it can be seen that the lookups and creations follow various sublinear power laws.
-        Inserting one element in a tree of depth $d$ should roughly take `O(log(d))` hamming distance evaluations.
-        Assuming an evenly distributed tree, the number of elements is given as `N=d^n` where `n` is the maximum distance the metric returns.
-        For the hamming distance, n is the number of bits of the hash.
-        Solving this for the depth, gives `d=log N / log n`.
-        If you are only interested in the dependence to `N`, then `log n` can be seen as a small constant factor.
-        Henceforth, the tree creation should follow `O(\sum_i^N \log i) = O( log( \product_i^N i )  ) = O(log(N!))`.
-        Using the Stirling's approximation for the faculty, we get `O(log(sqrt(N) N^N)) = O(log(N^(N+1/2))) = O(N log(N))`.
-        However, `log(N)` is a very slow growing function, so the tree creation looks almost a linear function.
-        
-        Both, pybktree and cppbktree, have some jumps at roughly 1e4 elements but only cppbktree as a second jump at ~2e6 elements but only when looking up elements with distance <= 16.
-        I can't explain these jumps.
-        They almost look like memory caching effects.
-        Because of these jumps, the effective speedups for 10M elements varies quite a lot depending on the lookup distance.
-        Only the tree creation scaling is a very smooth curve except for some outliers for smaller runtimes.
-        
-        Here are the fitted power laws to the curves from the plot:
-        
-        | operation             | pybktree        | cppbktree
-        |-----------------------|:---------------:|:---------------:|
-        | Tree creation         | 1.12e-06 N^1.12 | 4.92e-07 N^1.05 |
-        | Distance threshold 0  | 2.04e-06 N^0.27 | 4.19e-07 N^0.27 |
-        | Distance threshold 1  | 2.06e-06 N^0.37 | 2.77e-07 N^0.38 |
-        | Distance threshold 2  | 1.68e-06 N^0.51 | 1.76e-07 N^0.54 |
-        | Distance threshold 4  | 1.36e-06 N^0.73 | 1.11e-07 N^0.74 |
-        | Distance threshold 8  | 1.10e-06 N^0.92 | 7.47e-08 N^0.94 |
-        | Distance threshold 16 | 1.05e-06 N^0.99 | 4.93e-08 N^1.05 |
-        
-        And here are the timings and speedups for operations on a tree with 10 million 64-bit elements:
-        
-        | Operation | pybktree / s | cppbktree / s | Speedup |
-        |-----------------------|:--------:|:--------:|:----:|
-        | Tree creation time    | 88.53    | 19.35    | 4.6  |
-        | Distance threshold 0  | 2.42e-04 | 2.38e-05 | 10.2 |
-        | Distance threshold 1  | 7.49e-04 | 1.55e-04 | 4.8  |
-        | Distance threshold 2  | 8.55e-03 | 1.61e-03 | 5.3  |
-        | Distance threshold 4  | 2.21e-01 | 3.73e-02 | 5.9  |
-        | Distance threshold 8  | 4.22     | 0.60     | 7.1  |
-        | Distance threshold 16 | 11.5     | 6.93     | 1.7  |
-        
-        The speedups of cppbktree over pybktree vary between ~2 and 10.
-        For smaller trees, the speedups would be even better.
-        Only the tree creation time speedup is quite independent of the tree size at roughly 5.
-        
-        
-        ## Comparison pybktree vs. vptree
-        
-        At least in this benchmark with only 64-bit hashes and a hamming distance as metric and at least with this pure python implementation of a VP-Tree, the results are quite disappointing.
-        The vptree module is almost always slower.
-        The lookups are actually quite similar to pybktree (meaning still slower than lookups with cppbktree) but the tree creation is a full magnitude slower.
-        For the 100k elements, this results in pybktree being 7.7 times faster than vptree.
-        
-Platform: UNKNOWN
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Development Status :: 3 - Alpha
-Classifier: Operating System :: POSIX
-Classifier: Operating System :: Unix
-Classifier: Programming Language :: Python :: 3
-Description-Content-Type: text/markdown
+# C++ BK-Tree
+
+[![PyPI version](https://badge.fury.io/py/cppbktree.svg)](https://badge.fury.io/py/cppbktree)
+[![Downloads](https://pepy.tech/badge/cppbktree/month)](https://pepy.tech/project/cppbktree/month)
+[![License](https://img.shields.io/badge/license-MIT-blue.svg)](http://opensource.org/licenses/MIT)
+[![Build Status](https://travis-ci.org/mxmlnkn/cppbktree.svg?branch=master)](https://travis-ci.com/mxmlnkn/cppbktree)
+
+This module provides a BK-Tree class written in C++ to hopefully better speed than pure-python solutions.
+
+
+# Installation
+
+You can simply install it from PyPI:
+```
+pip install cppbktree
+```
+
+## From Source
+
+```python3
+python3 -m build . &&
+python3 -m pip install dist/cppbktree-*.whl
+```
+
+
+# Usage
+
+```python3
+from cppbktree import BKTree
+
+tree = BKTree( [ bytes( [ x ] ) for x in [0, 4, 5, 14] ] )
+tree.add( bytes( [ 15 ] ) )
+print( tree.find( 13, 1 ) )
+```
+
+Because of the Python/C++ interface, currently this BK-Tree is limited to only hamming distances of bytearrays.
+Pull requests are welcome.
+
+# Benchmarks
+
+The benchmark consists of inserting a varying amount of random 64-bit elements into the tree and then querying a value at varying distances.
+This is done five times to get a hint for the standard deviation as is plotted with error bars.
+
+## Comparison pybktree vs. cppbktree 0.1.0 with 32 K element chunking for 64-bit elements
+
+![Comparison pybktree cppbktree chunked](benchmark/results/compare-scalings-pybktree-cppbktree-chunked-8K.png) 
+
+This is a benchmark for the specialized `BKTree64`, which operates on 64-bit values.
+Doing the same with `BKTree` and byte vectors of size 8 to represent 64-bit values is roughly 4x slower
+because of additional allocations and because of pointer-chasing slowing down the linear lookup.
+A more intricate version could simply concatenate the element vectors into one consecutive memory chunk to avoid these performance issues.
+
+| Operation | pybktree / s | cppbktree (8K chunks) / s | Speedup |
+|-----------------------|:--------:|:--------:|:----:|
+| Tree creation time    | 88.53    | 1.57     | 56
+| Distance threshold 0  | 2.42e-04 | 1.81e-05 | 13
+| Distance threshold 1  | 7.49e-04 | 1.11e-04 | 6.7
+| Distance threshold 2  | 8.55e-03 | 4.46e-04 | 19
+| Distance threshold 4  | 2.21e-01 | 3.35e-03 | 66
+| Distance threshold 8  | 4.22e+00 | 1.55e-02 | 272
+| Distance threshold 16 | 1.15e+01 | 3.00e-02 | 383
+
+
+## Scaling Analysis
+
+![Comparison pybktree cppbktree](benchmark/results/compare-scalings-pybktree-cppbktree.png)
+
+In this log-log plot, it can be seen that the lookups and creations follow various sublinear power laws.
+Inserting one element in a tree of depth $d$ should roughly take `O(log(d))` hamming distance evaluations.
+Assuming an evenly distributed tree, the number of elements is given as `N=d^n` where `n` is the maximum distance the metric returns.
+For the hamming distance, n is the number of bits of the hash.
+Solving this for the depth, gives `d=log N / log n`.
+If you are only interested in the dependence to `N`, then `log n` can be seen as a small constant factor.
+Henceforth, the tree creation should follow `O(\sum_i^N \log i) = O( log( \product_i^N i )  ) = O(log(N!))`.
+Using the Stirling's approximation for the faculty, we get `O(log(sqrt(N) N^N)) = O(log(N^(N+1/2))) = O(N log(N))`.
+However, `log(N)` is a very slow growing function, so the tree creation looks almost a linear function.
+
+Both, pybktree and cppbktree, have some jumps at roughly 1e4 elements but only cppbktree as a second jump at ~2e6 elements but only when looking up elements with distance <= 16.
+I can't explain these jumps.
+They almost look like memory caching effects.
+Because of these jumps, the effective speedups for 10M elements varies quite a lot depending on the lookup distance.
+Only the tree creation scaling is a very smooth curve except for some outliers for smaller runtimes.
+
+Here are the fitted power laws to the curves from the plot:
+
+| operation             | pybktree        | cppbktree
+|-----------------------|:---------------:|:---------------:|
+| Tree creation         | 1.12e-06 N^1.12 | 4.92e-07 N^1.05 |
+| Distance threshold 0  | 2.04e-06 N^0.27 | 4.19e-07 N^0.27 |
+| Distance threshold 1  | 2.06e-06 N^0.37 | 2.77e-07 N^0.38 |
+| Distance threshold 2  | 1.68e-06 N^0.51 | 1.76e-07 N^0.54 |
+| Distance threshold 4  | 1.36e-06 N^0.73 | 1.11e-07 N^0.74 |
+| Distance threshold 8  | 1.10e-06 N^0.92 | 7.47e-08 N^0.94 |
+| Distance threshold 16 | 1.05e-06 N^0.99 | 4.93e-08 N^1.05 |
+
+And here are the timings and speedups for operations on a tree with 10 million 64-bit elements:
+
+| Operation | pybktree / s | cppbktree / s | Speedup |
+|-----------------------|:--------:|:--------:|:----:|
+| Tree creation time    | 88.53    | 19.35    | 4.6  |
+| Distance threshold 0  | 2.42e-04 | 2.38e-05 | 10.2 |
+| Distance threshold 1  | 7.49e-04 | 1.55e-04 | 4.8  |
+| Distance threshold 2  | 8.55e-03 | 1.61e-03 | 5.3  |
+| Distance threshold 4  | 2.21e-01 | 3.73e-02 | 5.9  |
+| Distance threshold 8  | 4.22     | 0.60     | 7.1  |
+| Distance threshold 16 | 11.5     | 6.93     | 1.7  |
+
+The speedups of cppbktree over pybktree vary between ~2 and 10.
+For smaller trees, the speedups would be even better.
+Only the tree creation time speedup is quite independent of the tree size at roughly 5.
+
+
+## Comparison pybktree vs. vptree
+
+
+![Comparison pybktree cppbktree](benchmark/results/compare-scalings-pybktree-vptree.png)
+
+At least in this benchmark with only 64-bit hashes and a hamming distance as metric and at least with this pure python implementation of a VP-Tree, the results are quite disappointing.
+The vptree module is almost always slower.
+The lookups are actually quite similar to pybktree (meaning still slower than lookups with cppbktree) but the tree creation is a full magnitude slower.
+For the 100k elements, this results in pybktree being 7.7 times faster than vptree.
+
+
+## Comparison linear lookup vs. cppbktree
+
+![Comparison pybktree cppbktree](benchmark/results/compare-scalings-cppbktree-linear-lookup.png)
+
+This log-log comparison plot shows that a simple linear lookup can compete with a BK tree.
+For exact and almost exact lookups, the BK tree can become faster but even for a distance of 2,
+it requires more than 1 M elements of size 8 B to amortize.
+For lookups with even larger distance, the simple linear lookup dominates for the whole tested range up to 80 MB of data!
+
+The advantage of the linear lookup is better streaming behavior and less branching making it run faster on modern CPUs.
+For batched lookup, the advantage might be even larger because whole batches can be looked up while the chunks of the haystack is still in CPU caches.
+A mixture a BK tree and linear lookup, e.g., a BK tree with nodes with 1-10k elements, might be better over the whole range of test configurations.
```

### Comparing `cppbktree-0.0.1/cppbktree/cppbktree.hpp` & `cppbktree-0.1.0/cppbktree/cppbktree.hpp`

 * *Files 26% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 #pragma once
 
 #include <algorithm>
 #include <bitset>
 #include <cassert>
 #include <cstdint>
+#include <fstream>
 #include <functional>
 #include <iomanip>
 #include <iostream>
 #include <iterator>
 #include <limits>
 #include <map>
 #include <memory>
+#include <numeric>
 #include <stack>
 #include <stdexcept>
+#include <tuple>
 #include <type_traits>
 #include <utility>
 #include <vector>
 
 
-namespace
-{
 template<typename T,
          typename std::enable_if<std::is_integral<T>::value, int>::type = 0>
 size_t
 countBits( T x )
 {
     static_assert( std::numeric_limits<T>::radix == 2, "non-binary type" );
 
@@ -31,15 +32,15 @@
     static_assert( bitWidth <= std::numeric_limits<unsigned long long>::digits,
                    "arg too wide for std::bitset() constructor");
 
     return std::bitset<bitWidth>( static_cast<typename std::make_unsigned<T>::type>( x ) ).count();
 }
 
 
-size_t
+inline size_t
 hammingDistance( const std::vector<uint8_t>& a,
                  const std::vector<uint8_t>& b )
 {
     if ( a.size() != b.size() ) {
         throw std::invalid_argument( "Hashes to compare must be of equal length!" );
     }
     size_t nDifferingBits = 0;
@@ -57,60 +58,214 @@
         }
     }
 
     return nDifferingBits;
 }
 
 
-template<typename T>
-std::ostream&
-operator<<( std::ostream&         out,
-            const std::vector<T>& values )
+inline size_t
+hammingDistance64( const uint64_t a,
+                   const uint64_t b )
 {
-    std::ios ioState( nullptr );
-    ioState.copyfmt( out );
-
-    out << "{";
-    for ( const auto& x : values ) {
-        out << " ";
-
-        //out << std::showbase << std::internal << std::setfill( '0' ) << std::hex << std::setw( 2 );
-        out << static_cast<unsigned int>( x );
-        out.copyfmt( ioState );
-    }
-
-    out << " }";
-    return out;
-}
+    return countBits( a ^ b );
 }
 
 
 template<typename T_ValueType,
          typename T_DistanceType>
 class CppBKTree
 {
 public:
     using ValueType      = T_ValueType;
     using DistanceType   = T_DistanceType;
     using MetricFunction = std::function<DistanceType( const ValueType&, const ValueType& )>;
 
+    /* Benchmarks show that linear lookup of 1 to ~1000 all take roughly the same time.
+     * Only after that, the cost begins to scale linearly up. */
+    static constexpr size_t CHUNK_SIZE = 1024;
+
     struct Node
     {
         /**
-         * Even if there are other values with a hamming distance of zero for this node,
-         * it must suffice to only store one value because of the identity of indiscernibles axiom of metrics.
+         * This is the bisection value for this node. For leaf nodes, it is only tentative and is effectively unused.
          */
-        ValueType value;
+        ValueType referenceValue;
+
+        /**
+         * Even if the CHUNK_SIZE is 1, there might be other values with a hamming distance of zero for this node.
+         */
+        std::vector<ValueType> values;
         /**
          * for now only an ordinal number signifying when it was inserted.
          * 0 for the first inserted, 1 for the second inserted item, and so on.
          * If there are multiple values identical under the metric, then there might be more than one payload.
          */
         std::vector<size_t> payloads;
-        std::map<DistanceType, std::unique_ptr<Node>> children;
+        std::map<DistanceType, std::unique_ptr<Node> > children;
+
+    public:
+        void
+        addToChild( ValueType             value,
+                    size_t                payload,
+                    const MetricFunction& metricFunction )
+        {
+            const auto distance = metricFunction( referenceValue, value );
+            const auto child = children.find( distance );
+            if ( child == children.end() ) {
+                auto node = std::unique_ptr<Node>( new Node{ value, { value }, { payload }, {} } );
+                children.emplace( distance, std::move( node ) );
+            } else {
+                child->second->add( std::move( value ), payload, metricFunction );
+            }
+        }
+
+        void
+        add( ValueType             value,
+             size_t                payload,
+             const MetricFunction& metricFunction )
+        {
+            /** Simply append to leaf nodes. They are split inside @ref rebalance. */
+            if ( children.empty() && ( values.size() == payloads.size() ) ) {
+                values.emplace_back( std::move( value ) );
+                payloads.emplace_back( payload );
+            } else {
+                addToChild( std::move( value ), payload, metricFunction );
+            }
+        }
+
+        void
+        rebalance( const size_t          maxElementCount,
+                   const MetricFunction& metricFunction )
+        {
+            /* Would be good to have a maximum possible hamming distance safely derived
+             * from ValueType and MetricFunction. But even if we had that, the ideal chunk size also depends
+             * on the benchmarks, which are dependant on both. Not possibly to do it generically autlomatically.
+             * Simply assume std::vecto<uint8_t> with 8 values (effectively uint64_t) for now.
+             * One problem here is that a single node split on average would lead to maximum distance more nodes.
+             * For uint64_t, this means almost two magnitudes more nodes for a single split.
+             * This makes the tradeoff consideration for splitting vs not splitting difficult.
+             * For large distance lookups (distance > maximum distance / 4), splitting is not necessary at all.
+             * This means, we are doing this to optimize small distances such as distance = 0.
+             * For distance = 0, we need to find splitting makes almost always sense, except if a linear lookup
+             * is not reduced any further, which is the case for element counts < 1k.
+             * However, splitting for more than 1k would result in sub nodes with each only ~16 elements!
+             * This would impede lookup for large distances!
+             * Therefore, do a compromise and split at 10k. Note that 100k is the point at which linear lookup
+             * becomes slower than BK tree lookup for distance == 0. So any split point < 100k would be fine
+             * even if not ideal. */
+            if ( payloads.size() > maxElementCount ) {
+                referenceValue = values.back();
+                std::vector<size_t> zeroDistancePayloads;
+                for ( size_t i = 0; i < std::min( values.size(), payloads.size() ); ++i ) {
+                    const auto distance = metricFunction( referenceValue, values[i] );
+                    if ( distance == 0 ) {
+                        zeroDistancePayloads.emplace_back( payloads[i] );
+                    } else {
+                        addToChild( std::move( values[i] ), payloads[i], metricFunction );
+                    }
+                }
+                values.clear();
+                payloads = std::move( zeroDistancePayloads );
+            }
+
+            for ( const auto& [_, child] : children ) {
+                child->rebalance( maxElementCount, metricFunction );
+            }
+        }
+
+        [[nodiscard]] std::vector<size_t>
+        find( const ValueType&      value,
+              DistanceType          distance,
+              const MetricFunction& metricFunction ) const
+        {
+            std::vector<size_t> result;
+
+            if ( children.empty() && ( values.size() == payloads.size() ) ) {
+                for ( size_t i = 0; i < values.size(); ++i ) {
+                    if ( metricFunction( value, values[i] ) <= distance ) {
+                        result.emplace_back( payloads[i] );
+                    }
+                }
+                return result;
+            }
+
+            /* If there are children or more payloads than values, then @ref referenceValue should be valid! */
+            const auto distanceToThisNode = metricFunction( value, referenceValue );
+            if ( distanceToThisNode <= distance ) {
+                std::copy( payloads.begin(), payloads.end(), std::back_inserter( result ) );
+            }
+
+            /* The map of children is inherently sorted by distance, so it suffices
+             * to search for a lower bound and then iterate to the upper bound.
+             * Be pedantic for overflow checks! */
+            const auto lowerBound = distanceToThisNode >= distance ? distanceToThisNode - distance : 0;
+            const auto upperBound = std::numeric_limits<DistanceType>::max() - distanceToThisNode >= distance
+                                    ? distanceToThisNode + distance
+                                    : std::numeric_limits<DistanceType>::max();
+            for ( auto candidate = children.lower_bound( lowerBound );
+                  ( candidate->first <= upperBound ) && ( candidate != children.end() );
+                  ++candidate )
+            {
+                const auto recursiveResult = candidate->second->find( value, distance, metricFunction );
+                result.insert( result.end(), recursiveResult.begin(), recursiveResult.end() );
+            }
+
+            return result;
+        }
+
+        bool
+        operator==( const Node& other ) const
+        {
+            if ( ( referenceValue  != other.referenceValue  ) ||
+                 ( values          != other.values          ) ||
+                 ( payloads        != other.payloads        ) ||
+                 ( children.size() != other.children.size() ) )
+            {
+                return false;
+            }
+
+            using ChildKeyValue = decltype( *children.begin() );
+
+            const auto childrenAreEqual =
+                [] ( const ChildKeyValue& child1, const ChildKeyValue& child2 )
+                {
+                    if ( ( child1.first != child2.first ) ||
+                         ( static_cast<bool>( child1.second ) != static_cast<bool>( child2.second ) ) )
+                    {
+                        return false;
+                    }
+
+                    if ( child1.second && child2.second ) {
+                        return *child1.second == *child2.second;
+                    }
+
+                    return true;
+                };
+
+            return std::equal( children.begin(), children.end(), other.children.begin(), childrenAreEqual );
+        }
+
+
+        void
+        print( std::ostream&    out,
+               uint32_t         depth = 0 ) const
+        {
+            std::ios ioState( nullptr );
+            ioState.copyfmt( out );
+
+            out << "Value: " << referenceValue << ", Values: " << values << ", Payloads: " << payloads << std::endl;
+
+            for ( const auto& child : children ) {
+                out << std::setw( ( depth + 1 ) * 2 ) << std::setfill( ' ' ) << ""
+                    << std::setw( 8 ) << child.first;
+                out.copyfmt( ioState );
+                out << " : ";
+                child.second->print( out, depth + 1 );
+            }
+        }
     };
 
     struct TreeStatistics
     {
         size_t nodeCount = 0;
         size_t leafCount = 0;
         /** Might generally be larger than nodeCount as one node might have multiple identical values attached */
@@ -128,146 +283,77 @@
         /** Can be derived as valueCount - nodeCount. */
         size_t duplicateCount = 0;
         /**
          * Basically the hash length and therefore gives the hamming distance range of [0,valueBitCount].
          * All values have the same bit count or else hammingDistance will throw.
          */
         size_t valueBitCount = 0;
+
+        size_t minPayloadsPerNode{ 0 };
+        size_t maxPayloadsPerNode{ 0 };
     };
 
 public:
     /**
      * Takes a vector of byte arrays to construct the tree from.
      */
     explicit
     CppBKTree( MetricFunction metricFunction,
-               const std::vector<ValueType>& values = {} ) :
+               std::vector<ValueType> values = {} ) :
+        m_itemCount( values.size() ),
         m_metricFunction( metricFunction )
     {
-        for ( const auto& value : values ) {
-            add( value );
+        if ( !values.empty() ) {
+            std::vector<size_t> payloads( m_itemCount );
+            std::iota( payloads.begin(), payloads.end(), 0 );
+            m_root = std::unique_ptr<Node>( new Node{ {}, std::move( values ), std::move( payloads ), {} } );
+        }
+
+        if ( !m_metricFunction ) {
+            if constexpr ( std::is_same_v<ValueType, uint64_t> ) {
+                m_metricFunction = MetricFunction( &hammingDistance64 );
+            } else if constexpr ( std::is_same_v<ValueType, std::vector<uint8_t> > ) {
+                m_metricFunction = MetricFunction( &hammingDistance );
+            } else {
+                throw std::invalid_argument( "Could not find a suitable default metric function. Please specify one!" );
+            }
         }
     }
 
     explicit
-    CppBKTree( const std::vector<ValueType>& values = {} ) :
-        m_metricFunction( &hammingDistance )
+    CppBKTree( std::vector<ValueType> values = {} ) :
+        CppBKTree( MetricFunction{}, std::move( values ) )
+    {}
+
+    void
+    add( ValueType value )
     {
-        for ( const auto& value : values ) {
-            add( value );
+        if ( m_root ) {
+            m_root->add( std::move( value ), m_itemCount++, m_metricFunction );
+        } else {
+            m_root = std::unique_ptr<Node>( new Node{ {}, { value }, { m_itemCount++ }, /* children */ {} } );
         }
     }
 
     void
-    add( const ValueType& value )
+    rebalance( const size_t maxElementCount )
     {
-        if ( !m_root ) {
-            m_root = std::unique_ptr<Node>( new Node{ value, { m_itemCount++ }, {} } );
-            return;
-        }
-
-        /* Descend into the tree along edges with equal distance to the node's item until there is no such edge. */
-        auto* ppnode = &m_root;
-        while ( true ) {
-            const auto distance = m_metricFunction( (*ppnode)->value, value );
-
-            /* Append identical value to this node */
-            if ( distance == 0 ) {
-                (*ppnode)->payloads.push_back( m_itemCount++ );
-                break;
-            }
-
-            /* Insert a new child */
-            auto& children = (*ppnode)->children;
-            const auto child = children.find( distance );
-            if ( child == children.end() ) {
-                children.emplace( distance, std::unique_ptr<Node>( new Node{ value, { m_itemCount++ }, {} } ) );
-                break;
-            }
-
-            /* Descend along the found edge */
-            ppnode = &child->second;
+        if ( m_root ) {
+            m_root->rebalance( maxElementCount, m_metricFunction );
         }
     }
 
-    std::vector<size_t>
-    find( const ValueType&             value,
-          DistanceType                 distance,
-          const std::unique_ptr<Node>* root = nullptr ) const
+    [[nodiscard]] std::vector<size_t>
+    find( const ValueType& value,
+          DistanceType     distance ) const
     {
-        if ( root == nullptr ) {
-            if ( !m_root ) {
-                return {};
-            }
-            return find( value, distance, &m_root );
-        }
-
-        std::vector<size_t> result;
-
-        std::stack<const std::unique_ptr<Node>*> candidates;
-        candidates.push( root );
-        while ( !candidates.empty() ) {
-            const auto ppnode = candidates.top();
-            candidates.pop();
-            const auto distanceToThisNode = m_metricFunction( (*ppnode)->value, value );
-
-            if ( distanceToThisNode <= distance ) {
-                const auto& payloads = (*ppnode)->payloads;
-                std::copy( payloads.begin(), payloads.end(), std::back_inserter( result ) );
-            }
-
-            /* The map of children is inherently sorted by distance, so it suffices
-             * to search for a lower bound and then iterate to the upper bound.
-             * Be pedantic for overflow checks! */
-            const auto lowerBound = distanceToThisNode >= distance ? distanceToThisNode - distance : 0;
-            const auto upperBound = std::numeric_limits<DistanceType>::max() - distanceToThisNode >= distance
-                                    ? distanceToThisNode + distance
-                                    : std::numeric_limits<DistanceType>::max();
-            for ( auto candidate = (*ppnode)->children.lower_bound( lowerBound );
-                  ( candidate->first <= upperBound ) && ( candidate != (*ppnode)->children.end() );
-                  ++candidate )
-            {
-                /**
-                 * Consider a hash with n bits. The distance will range in [0,n]. The hash will have at most 2^n
-                 * distinct values and therefore tree nodes. Assuming a balanced tree, a depth d will be able to
-                 * encode n^d values. As there are only 2^n values possible, the max depth D is given as 2^n = n^D.
-                 * This is equivalent to n log(2) = D log(n) giving D = n log(2) / log(n).
-                 * For most hashes, recursion shouldn't be a problem but I don't know. I arbitrarily decided
-                 * to avoid recursion using a stack. This might also help avoiding multiple copies.
-                 * In the worst case, the stack will have to store d * n pointers because the push pop mechanism
-                 * basically boils down to a depth-first search.
-                 * Note that the maxium depth for a very uneven tree would be D = n if we inserted successively
-                 * elements with distance one from each other. This would only require n elements so deep trees
-                 * can do happen for few elements.
-                 * I compared three versions:
-                 *  1. A recursive version, which is still in the code with FIND_RECURSIVE = true
-                 *  2. A depth-first search using a stack, which is still in the code with FIND_RECURSIVE = false
-                 *  3. A temporary version using a vector with a capacity of maxDistance * log(2) / log( maxDistance ).
-                 *     It might have been better to simply use .reserve( maxDistance ) but I checked with debug output
-                 *     and the vector size never seemed to exceed the capacity, so there should be no reallocations.
-                 * The benchmark also always compares the results to the pybktree implementation, so the results should
-                 * be correct.
-                 * Conclusion: All versions suffer a performance degradation after 2e4 (1), 2e4 (2), 3e3 (3) elements.
-                 *             The recursive version is pretty much identical to the version using the stack.
-                 *             The vector version has better performance than the other versions for 3e3 elements,
-                 *             but then the runtime suddenly spikes to 1e-4 seconds and the scalings for all different
-                 *             distance threshold begin to overlap, probably because some huge offset make them
-                 *             pretty much indiscernible.
-                 *             For distances <= 8 (n=64), this version is actually slower than pybktree!
-                 */
-                if ( FIND_RECURSIVE ) {
-                    const auto recursiveResult = find( value, distance, &candidate->second );
-                    result.insert( result.end(), recursiveResult.begin(), recursiveResult.end() );
-                } else {
-                    candidates.push( &candidate->second );
-                }
-            }
+        if ( m_root ) {
+            return m_root->find( value, distance, m_metricFunction );
         }
-
-        return result;
+        return {};
     }
 
     size_t
     size() const
     {
         return m_itemCount;
     }
@@ -279,16 +365,29 @@
     statistics() const
     {
         if ( !m_root ) {
             return TreeStatistics();
         }
 
         TreeStatistics result;
-        result.valueBitCount = m_root->value.size() * std::numeric_limits<uint8_t>::digits;
+
+        if constexpr ( std::is_integral_v<ValueType> ) {
+            result.valueBitCount = std::numeric_limits<ValueType>::digits;
+        } else {
+            const auto elementCount = m_root->values.empty()
+                                      ? m_root->referenceValue.size()
+                                      : m_root->values.front().size();
+            result.valueBitCount = elementCount * std::numeric_limits<uint8_t>::digits;
+        }
+
         result.minChildrenPerNode = std::numeric_limits<decltype( result.minChildrenPerNode )>::max();
+        result.maxChildrenPerNode = std::numeric_limits<decltype( result.minChildrenPerNode )>::min();
+
+        result.minPayloadsPerNode = std::numeric_limits<decltype( result.minPayloadsPerNode )>::max();
+        result.maxPayloadsPerNode = std::numeric_limits<decltype( result.minPayloadsPerNode )>::min();
 
         std::stack<std::pair<const std::unique_ptr<Node>*, /* depth */ size_t> > nodesToProcess;
         nodesToProcess.push( std::make_pair( &m_root, 1 ) );
         while ( !nodesToProcess.empty() ) {
             const auto nodeToProcess = nodesToProcess.top();
             const auto ppnode = nodeToProcess.first;
             const auto nodeDepth = nodeToProcess.second;
@@ -302,25 +401,64 @@
             if ( children.empty() ) {
                 result.leafCount += 1;
             } else {
                 result.minChildrenPerNode = std::min( result.minChildrenPerNode, children.size() );
                 result.maxChildrenPerNode = std::max( result.maxChildrenPerNode, children.size() );
             }
 
+            const auto& payloads = (*ppnode)->payloads;
+            result.minPayloadsPerNode = std::min( result.minPayloadsPerNode, payloads.size() );
+            result.maxPayloadsPerNode = std::max( result.maxPayloadsPerNode, payloads.size() );
+
             for ( auto child = children.begin(); child != children.end(); ++child ) {
                 nodesToProcess.push( std::make_pair( &child->second, nodeDepth + 1 ) );
             }
         }
 
+        if ( result.minChildrenPerNode > result.maxChildrenPerNode ) {
+            result.minChildrenPerNode = 0;
+            result.maxChildrenPerNode = 0;
+        }
+
         result.duplicateCount = result.valueCount - result.nodeCount;
         result.averageChildCountPerNode = static_cast<double>( result.nodeCount - 1 )
                                           / ( result.nodeCount - result.leafCount );
 
         return result;
     }
 
+    bool
+    operator==( const CppBKTree& other ) const
+    {
+        if ( ( static_cast<bool>( m_root ) != static_cast<bool>( other.m_root ) ) ||
+             ( m_itemCount != other.m_itemCount ) )
+        {
+             return false;
+        }
+
+        if ( m_root && other.m_root ) {
+            return *m_root == *other.m_root;
+        }
+
+        return true;
+
+    }
+
+    friend std::ostream&
+    operator<<( std::ostream&    out,
+                const CppBKTree& tree )
+    {
+        out << "Tree with " << tree.m_itemCount << " items:\n";
+        if ( tree.m_root ) {
+            tree.m_root->print( out, 1 );
+        } else {
+            out << "<empty tree>";
+        }
+        out << std::endl;
+        return out;
+    }
+
 private:
     std::unique_ptr<Node> m_root;
     size_t m_itemCount = 0;
-    const MetricFunction m_metricFunction;
-    static constexpr bool FIND_RECURSIVE = false;
+    MetricFunction m_metricFunction;
 };
```

