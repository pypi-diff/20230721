# Comparing `tmp/dwave-preprocessing-0.6.2.tar.gz` & `tmp/dwave-preprocessing-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dwave-preprocessing-0.6.2.tar", last modified: Thu Jul  6 22:21:43 2023, max compression
+gzip compressed data, was "dwave-preprocessing-0.6.3.tar", last modified: Fri Jul 21 20:09:26 2023, max compression
```

## Comparing `dwave-preprocessing-0.6.2.tar` & `dwave-preprocessing-0.6.3.tar`

### file list

```diff
@@ -1,165 +1,165 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-06 22:21:43.667941 dwave-preprocessing-0.6.2/
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11359 2023-07-06 22:21:21.000000 dwave-preprocessing-0.6.2/LICENSE
--rw-r--r--   0 circleci  (3434) circleci  (3434)      254 2023-07-06 22:21:21.000000 dwave-preprocessing-0.6.2/MANIFEST.in
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3242 2023-07-06 22:21:43.671941 dwave-preprocessing-0.6.2/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2449 2023-07-06 22:21:21.000000 dwave-preprocessing-0.6.2/README.rst
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-06 22:21:43.651941 dwave-preprocessing-0.6.2/dwave/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      648 2023-07-06 22:21:21.000000 dwave-preprocessing-0.6.2/dwave/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-06 22:21:43.651941 dwave-preprocessing-0.6.2/dwave/preprocessing/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1034 2023-07-06 22:21:21.000000 dwave-preprocessing-0.6.2/dwave/preprocessing/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-06 22:21:43.651941 dwave-preprocessing-0.6.2/dwave/preprocessing/composites/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      877 2023-07-06 22:21:21.000000 dwave-preprocessing-0.6.2/dwave/preprocessing/composites/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3753 2023-07-06 22:21:21.000000 dwave-preprocessing-0.6.2/dwave/preprocessing/composites/clip.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4234 2023-07-06 22:21:21.000000 dwave-preprocessing-0.6.2/dwave/preprocessing/composites/connected_components.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5941 2023-07-06 22:21:21.000000 dwave-preprocessing-0.6.2/dwave/preprocessing/composites/fix_variables.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5295 2023-07-06 22:21:21.000000 dwave-preprocessing-0.6.2/dwave/preprocessing/composites/scale.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6919 2023-07-06 22:21:21.000000 dwave-preprocessing-0.6.2/dwave/preprocessing/composites/spin_reversal_transform.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)   937814 2023-07-06 22:21:41.000000 dwave-preprocessing-0.6.2/dwave/preprocessing/cyfix_variables.cpp
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2283 2023-07-06 22:21:21.000000 dwave-preprocessing-0.6.2/dwave/preprocessing/cyfix_variables.pyx
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-06 22:21:43.647941 dwave-preprocessing-0.6.2/dwave/preprocessing/include/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-06 22:21:43.651941 dwave-preprocessing-0.6.2/dwave/preprocessing/include/dwave/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      973 2023-07-06 22:21:21.000000 dwave-preprocessing-0.6.2/dwave/preprocessing/include/dwave/exceptions.hpp
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2319 2023-07-06 22:21:21.000000 dwave-preprocessing-0.6.2/dwave/preprocessing/include/dwave/flags.hpp
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2752 2023-07-06 22:21:21.000000 dwave-preprocessing-0.6.2/dwave/preprocessing/include/dwave/presolve.hpp
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-06 22:21:43.655941 dwave-preprocessing-0.6.2/dwave/preprocessing/include/dwave-preprocessing/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5386 2023-07-06 22:21:21.000000 dwave-preprocessing-0.6.2/dwave/preprocessing/include/dwave-preprocessing/fix_variables.hpp
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3900 2023-07-06 22:21:21.000000 dwave-preprocessing-0.6.2/dwave/preprocessing/include/dwave-preprocessing/helper_data_structures.hpp
--rw-r--r--   0 circleci  (3434) circleci  (3434)    19997 2023-07-06 22:21:21.000000 dwave-preprocessing-0.6.2/dwave/preprocessing/include/dwave-preprocessing/helper_graph_algorithms.hpp
--rw-r--r--   0 circleci  (3434) circleci  (3434)    29940 2023-07-06 22:21:21.000000 dwave-preprocessing-0.6.2/dwave/preprocessing/include/dwave-preprocessing/implication_network.hpp
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4617 2023-07-06 22:21:21.000000 dwave-preprocessing-0.6.2/dwave/preprocessing/include/dwave-preprocessing/mapping_policy.hpp
--rw-r--r--   0 circleci  (3434) circleci  (3434)    15765 2023-07-06 22:21:21.000000 dwave-preprocessing-0.6.2/dwave/preprocessing/include/dwave-preprocessing/posiform_info.hpp
--rw-r--r--   0 circleci  (3434) circleci  (3434)    33374 2023-07-06 22:21:21.000000 dwave-preprocessing-0.6.2/dwave/preprocessing/include/dwave-preprocessing/push_relabel.hpp
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2031 2023-07-06 22:21:21.000000 dwave-preprocessing-0.6.2/dwave/preprocessing/libcpp.pxd
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3585 2023-07-06 22:21:21.000000 dwave-preprocessing-0.6.2/dwave/preprocessing/lower_bounds.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-06 22:21:43.655941 dwave-preprocessing-0.6.2/dwave/preprocessing/presolve/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      610 2023-07-06 22:21:21.000000 dwave-preprocessing-0.6.2/dwave/preprocessing/presolve/__init__.pxd
--rw-r--r--   0 circleci  (3434) circleci  (3434)      719 2023-07-06 22:21:21.000000 dwave-preprocessing-0.6.2/dwave/preprocessing/presolve/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)  1227101 2023-07-06 22:21:43.000000 dwave-preprocessing-0.6.2/dwave/preprocessing/presolve/cypresolve.cpp
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1353 2023-07-06 22:21:21.000000 dwave-preprocessing-0.6.2/dwave/preprocessing/presolve/cypresolve.pxd
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11614 2023-07-06 22:21:21.000000 dwave-preprocessing-0.6.2/dwave/preprocessing/presolve/cypresolve.pyx
--rw-r--r--   0 circleci  (3434) circleci  (3434)      782 2023-07-06 22:21:21.000000 dwave-preprocessing-0.6.2/dwave/preprocessing/presolve/exceptions.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6036 2023-07-06 22:21:21.000000 dwave-preprocessing-0.6.2/dwave/preprocessing/presolve/pypresolve.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-06 22:21:43.655941 dwave-preprocessing-0.6.2/dwave/preprocessing/src/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      809 2023-07-06 22:21:21.000000 dwave-preprocessing-0.6.2/dwave/preprocessing/src/exceptions.cpp
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3907 2023-07-06 22:21:21.000000 dwave-preprocessing-0.6.2/dwave/preprocessing/src/presolve.cpp
--rw-r--r--   0 circleci  (3434) circleci  (3434)    41637 2023-07-06 22:21:21.000000 dwave-preprocessing-0.6.2/dwave/preprocessing/src/presolveimpl.hpp
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-06 22:21:43.655941 dwave-preprocessing-0.6.2/dwave_preprocessing.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3242 2023-07-06 22:21:43.000000 dwave-preprocessing-0.6.2/dwave_preprocessing.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6756 2023-07-06 22:21:43.000000 dwave-preprocessing-0.6.2/dwave_preprocessing.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-07-06 22:21:43.000000 dwave-preprocessing-0.6.2/dwave_preprocessing.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-07-06 22:21:43.000000 dwave-preprocessing-0.6.2/dwave_preprocessing.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (3434) circleci  (3434)       43 2023-07-06 22:21:43.000000 dwave-preprocessing-0.6.2/dwave_preprocessing.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        6 2023-07-06 22:21:43.000000 dwave-preprocessing-0.6.2/dwave_preprocessing.egg-info/top_level.txt
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-06 22:21:43.651941 dwave-preprocessing-0.6.2/extern/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-06 22:21:43.655941 dwave-preprocessing-0.6.2/extern/spdlog/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1348 2023-07-06 22:21:26.000000 dwave-preprocessing-0.6.2/extern/spdlog/LICENSE
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-06 22:21:43.651941 dwave-preprocessing-0.6.2/extern/spdlog/include/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-06 22:21:43.659941 dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3587 2023-07-06 22:21:26.000000 dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/async.h
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2494 2023-07-06 22:21:26.000000 dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/async_logger-inl.h
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2276 2023-07-06 22:21:26.000000 dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/async_logger.h
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-06 22:21:43.659941 dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/cfg/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1229 2023-07-06 22:21:26.000000 dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/cfg/argv.h
--rw-r--r--   0 circleci  (3434) circleci  (3434)      988 2023-07-06 22:21:26.000000 dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/cfg/env.h
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3174 2023-07-06 22:21:26.000000 dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/cfg/helpers-inl.h
--rw-r--r--   0 circleci  (3434) circleci  (3434)      714 2023-07-06 22:21:26.000000 dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/cfg/helpers.h
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2064 2023-07-06 22:21:26.000000 dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/common-inl.h
--rw-r--r--   0 circleci  (3434) circleci  (3434)    12011 2023-07-06 22:21:26.000000 dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/common.h
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-06 22:21:43.663941 dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/details/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1884 2023-07-06 22:21:26.000000 dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/details/backtracer-inl.h
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1139 2023-07-06 22:21:26.000000 dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/details/backtracer.h
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3512 2023-07-06 22:21:26.000000 dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/details/circular_q.h
--rw-r--r--   0 circleci  (3434) circleci  (3434)      609 2023-07-06 22:21:26.000000 dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/details/console_globals.h
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4582 2023-07-06 22:21:26.000000 dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/details/file_helper-inl.h
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1739 2023-07-06 22:21:26.000000 dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/details/file_helper.h
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4586 2023-07-06 22:21:26.000000 dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/details/fmt_helper.h
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1104 2023-07-06 22:21:26.000000 dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/details/log_msg-inl.h
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1154 2023-07-06 22:21:26.000000 dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/details/log_msg.h
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1656 2023-07-06 22:21:26.000000 dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/details/log_msg_buffer-inl.h
--rw-r--r--   0 circleci  (3434) circleci  (3434)      933 2023-07-06 22:21:26.000000 dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/details/log_msg_buffer.h
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3784 2023-07-06 22:21:26.000000 dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/details/mpmc_blocking_q.h
--rw-r--r--   0 circleci  (3434) circleci  (3434)      967 2023-07-06 22:21:26.000000 dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/details/null_mutex.h
--rw-r--r--   0 circleci  (3434) circleci  (3434)    16664 2023-07-06 22:21:26.000000 dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/details/os-inl.h
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3818 2023-07-06 22:21:26.000000 dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/details/os.h
--rw-r--r--   0 circleci  (3434) circleci  (3434)      622 2023-07-06 22:21:26.000000 dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/details/periodic_worker-inl.h
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1766 2023-07-06 22:21:26.000000 dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/details/periodic_worker.h
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8411 2023-07-06 22:21:26.000000 dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/details/registry-inl.h
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3936 2023-07-06 22:21:26.000000 dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/details/registry.h
--rw-r--r--   0 circleci  (3434) circleci  (3434)      754 2023-07-06 22:21:26.000000 dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/details/synchronous_factory.h
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4329 2023-07-06 22:21:26.000000 dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/details/tcp_client-windows.h
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3911 2023-07-06 22:21:26.000000 dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/details/tcp_client.h
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3628 2023-07-06 22:21:26.000000 dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/details/thread_pool-inl.h
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3394 2023-07-06 22:21:26.000000 dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/details/thread_pool.h
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3108 2023-07-06 22:21:26.000000 dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/details/udp_client-windows.h
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2264 2023-07-06 22:21:26.000000 dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/details/udp_client.h
--rw-r--r--   0 circleci  (3434) circleci  (3434)      187 2023-07-06 22:21:26.000000 dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/details/windows_include.h
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-06 22:21:43.663941 dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/fmt/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7284 2023-07-06 22:21:26.000000 dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/fmt/bin_to_hex.h
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-06 22:21:43.663941 dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/fmt/bundled/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7420 2023-07-06 22:21:26.000000 dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/fmt/bundled/args.h
--rw-r--r--   0 circleci  (3434) circleci  (3434)    68076 2023-07-06 22:21:26.000000 dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/fmt/bundled/chrono.h
--rw-r--r--   0 circleci  (3434) circleci  (3434)    24896 2023-07-06 22:21:26.000000 dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/fmt/bundled/color.h
--rw-r--r--   0 circleci  (3434) circleci  (3434)    21245 2023-07-06 22:21:26.000000 dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/fmt/bundled/compile.h
--rw-r--r--   0 circleci  (3434) circleci  (3434)   111215 2023-07-06 22:21:26.000000 dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/fmt/bundled/core.h
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1408 2023-07-06 22:21:26.000000 dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/fmt/bundled/fmt.license.rst
--rw-r--r--   0 circleci  (3434) circleci  (3434)    74272 2023-07-06 22:21:26.000000 dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/fmt/bundled/format-inl.h
--rw-r--r--   0 circleci  (3434) circleci  (3434)   154181 2023-07-06 22:21:26.000000 dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/fmt/bundled/format.h
--rw-r--r--   0 circleci  (3434) circleci  (3434)      100 2023-07-06 22:21:26.000000 dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/fmt/bundled/locale.h
--rw-r--r--   0 circleci  (3434) circleci  (3434)    14123 2023-07-06 22:21:26.000000 dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/fmt/bundled/os.h
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7586 2023-07-06 22:21:26.000000 dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/fmt/bundled/ostream.h
--rw-r--r--   0 circleci  (3434) circleci  (3434)    20023 2023-07-06 22:21:26.000000 dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/fmt/bundled/printf.h
--rw-r--r--   0 circleci  (3434) circleci  (3434)    23218 2023-07-06 22:21:26.000000 dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/fmt/bundled/ranges.h
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9001 2023-07-06 22:21:26.000000 dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/fmt/bundled/xchar.h
--rw-r--r--   0 circleci  (3434) circleci  (3434)      523 2023-07-06 22:21:26.000000 dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/fmt/chrono.h
--rw-r--r--   0 circleci  (3434) circleci  (3434)      531 2023-07-06 22:21:26.000000 dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/fmt/compile.h
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1004 2023-07-06 22:21:26.000000 dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/fmt/fmt.h
--rw-r--r--   0 circleci  (3434) circleci  (3434)      526 2023-07-06 22:21:26.000000 dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/fmt/ostr.h
--rw-r--r--   0 circleci  (3434) circleci  (3434)      523 2023-07-06 22:21:26.000000 dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/fmt/ranges.h
--rw-r--r--   0 circleci  (3434) circleci  (3434)      520 2023-07-06 22:21:26.000000 dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/fmt/xchar.h
--rw-r--r--   0 circleci  (3434) circleci  (3434)      462 2023-07-06 22:21:26.000000 dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/formatter.h
--rw-r--r--   0 circleci  (3434) circleci  (3434)      304 2023-07-06 22:21:26.000000 dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/fwd.h
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7036 2023-07-06 22:21:26.000000 dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/logger-inl.h
--rw-r--r--   0 circleci  (3434) circleci  (3434)    15636 2023-07-06 22:21:26.000000 dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/logger.h
--rw-r--r--   0 circleci  (3434) circleci  (3434)    43590 2023-07-06 22:21:26.000000 dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/pattern_formatter-inl.h
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3603 2023-07-06 22:21:26.000000 dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/pattern_formatter.h
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-06 22:21:43.667941 dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/sinks/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4562 2023-07-06 22:21:26.000000 dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/sinks/android_sink.h
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4594 2023-07-06 22:21:26.000000 dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/sinks/ansicolor_sink-inl.h
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3954 2023-07-06 22:21:26.000000 dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/sinks/ansicolor_sink.h
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1778 2023-07-06 22:21:26.000000 dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/sinks/base_sink-inl.h
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1565 2023-07-06 22:21:26.000000 dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/sinks/base_sink.h
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1102 2023-07-06 22:21:26.000000 dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/sinks/basic_file_sink-inl.h
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1834 2023-07-06 22:21:26.000000 dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/sinks/basic_file_sink.h
--rw-r--r--   0 circleci  (3434) circleci  (3434)    10310 2023-07-06 22:21:26.000000 dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/sinks/daily_file_sink.h
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2438 2023-07-06 22:21:26.000000 dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/sinks/dist_sink.h
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3014 2023-07-06 22:21:26.000000 dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/sinks/dup_filter_sink.h
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6623 2023-07-06 22:21:26.000000 dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/sinks/hourly_file_sink.h
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3744 2023-07-06 22:21:26.000000 dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/sinks/mongo_sink.h
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1545 2023-07-06 22:21:26.000000 dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/sinks/msvc_sink.h
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1229 2023-07-06 22:21:26.000000 dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/sinks/null_sink.h
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1250 2023-07-06 22:21:26.000000 dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/sinks/ostream_sink.h
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3382 2023-07-06 22:21:26.000000 dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/sinks/qt_sinks.h
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2121 2023-07-06 22:21:26.000000 dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/sinks/ringbuffer_sink.h
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4733 2023-07-06 22:21:26.000000 dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/sinks/rotating_file_sink-inl.h
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2648 2023-07-06 22:21:26.000000 dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/sinks/rotating_file_sink.h
--rw-r--r--   0 circleci  (3434) circleci  (3434)      725 2023-07-06 22:21:26.000000 dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/sinks/sink-inl.h
--rw-r--r--   0 circleci  (3434) circleci  (3434)      891 2023-07-06 22:21:26.000000 dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/sinks/sink.h
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1214 2023-07-06 22:21:26.000000 dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/sinks/stdout_color_sinks-inl.h
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1626 2023-07-06 22:21:26.000000 dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/sinks/stdout_color_sinks.h
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4364 2023-07-06 22:21:26.000000 dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/sinks/stdout_sinks-inl.h
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2419 2023-07-06 22:21:26.000000 dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/sinks/stdout_sinks.h
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3727 2023-07-06 22:21:26.000000 dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/sinks/syslog_sink.h
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4146 2023-07-06 22:21:26.000000 dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/sinks/systemd_sink.h
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2147 2023-07-06 22:21:26.000000 dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/sinks/tcp_sink.h
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1820 2023-07-06 22:21:26.000000 dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/sinks/udp_sink.h
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8870 2023-07-06 22:21:26.000000 dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/sinks/win_eventlog_sink.h
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6357 2023-07-06 22:21:26.000000 dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/sinks/wincolor_sink-inl.h
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2711 2023-07-06 22:21:26.000000 dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/sinks/wincolor_sink.h
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2974 2023-07-06 22:21:26.000000 dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/spdlog-inl.h
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11279 2023-07-06 22:21:26.000000 dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/spdlog.h
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1726 2023-07-06 22:21:26.000000 dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/stopwatch.h
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6453 2023-07-06 22:21:26.000000 dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/tweakme.h
--rw-r--r--   0 circleci  (3434) circleci  (3434)      331 2023-07-06 22:21:26.000000 dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/version.h
--rw-r--r--   0 circleci  (3434) circleci  (3434)      824 2023-07-06 22:21:21.000000 dwave-preprocessing-0.6.2/pyproject.toml
--rw-r--r--   0 circleci  (3434) circleci  (3434)      965 2023-07-06 22:21:43.671941 dwave-preprocessing-0.6.2/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1961 2023-07-06 22:21:21.000000 dwave-preprocessing-0.6.2/setup.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-21 20:09:26.372667 dwave-preprocessing-0.6.3/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11359 2023-07-21 20:09:06.000000 dwave-preprocessing-0.6.3/LICENSE
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      254 2023-07-21 20:09:06.000000 dwave-preprocessing-0.6.3/MANIFEST.in
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3242 2023-07-21 20:09:26.372667 dwave-preprocessing-0.6.3/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2449 2023-07-21 20:09:06.000000 dwave-preprocessing-0.6.3/README.rst
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-21 20:09:26.356667 dwave-preprocessing-0.6.3/dwave/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      648 2023-07-21 20:09:06.000000 dwave-preprocessing-0.6.3/dwave/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-21 20:09:26.356667 dwave-preprocessing-0.6.3/dwave/preprocessing/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1034 2023-07-21 20:09:06.000000 dwave-preprocessing-0.6.3/dwave/preprocessing/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-21 20:09:26.356667 dwave-preprocessing-0.6.3/dwave/preprocessing/composites/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      877 2023-07-21 20:09:06.000000 dwave-preprocessing-0.6.3/dwave/preprocessing/composites/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3753 2023-07-21 20:09:06.000000 dwave-preprocessing-0.6.3/dwave/preprocessing/composites/clip.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4234 2023-07-21 20:09:06.000000 dwave-preprocessing-0.6.3/dwave/preprocessing/composites/connected_components.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5941 2023-07-21 20:09:06.000000 dwave-preprocessing-0.6.3/dwave/preprocessing/composites/fix_variables.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5295 2023-07-21 20:09:06.000000 dwave-preprocessing-0.6.3/dwave/preprocessing/composites/scale.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6919 2023-07-21 20:09:06.000000 dwave-preprocessing-0.6.3/dwave/preprocessing/composites/spin_reversal_transform.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)   937814 2023-07-21 20:09:24.000000 dwave-preprocessing-0.6.3/dwave/preprocessing/cyfix_variables.cpp
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2283 2023-07-21 20:09:06.000000 dwave-preprocessing-0.6.3/dwave/preprocessing/cyfix_variables.pyx
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-21 20:09:26.352667 dwave-preprocessing-0.6.3/dwave/preprocessing/include/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-21 20:09:26.356667 dwave-preprocessing-0.6.3/dwave/preprocessing/include/dwave/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      973 2023-07-21 20:09:06.000000 dwave-preprocessing-0.6.3/dwave/preprocessing/include/dwave/exceptions.hpp
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2319 2023-07-21 20:09:06.000000 dwave-preprocessing-0.6.3/dwave/preprocessing/include/dwave/flags.hpp
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2752 2023-07-21 20:09:06.000000 dwave-preprocessing-0.6.3/dwave/preprocessing/include/dwave/presolve.hpp
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-21 20:09:26.356667 dwave-preprocessing-0.6.3/dwave/preprocessing/include/dwave-preprocessing/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5386 2023-07-21 20:09:06.000000 dwave-preprocessing-0.6.3/dwave/preprocessing/include/dwave-preprocessing/fix_variables.hpp
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3900 2023-07-21 20:09:06.000000 dwave-preprocessing-0.6.3/dwave/preprocessing/include/dwave-preprocessing/helper_data_structures.hpp
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    19997 2023-07-21 20:09:06.000000 dwave-preprocessing-0.6.3/dwave/preprocessing/include/dwave-preprocessing/helper_graph_algorithms.hpp
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    29940 2023-07-21 20:09:06.000000 dwave-preprocessing-0.6.3/dwave/preprocessing/include/dwave-preprocessing/implication_network.hpp
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4617 2023-07-21 20:09:06.000000 dwave-preprocessing-0.6.3/dwave/preprocessing/include/dwave-preprocessing/mapping_policy.hpp
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    15765 2023-07-21 20:09:06.000000 dwave-preprocessing-0.6.3/dwave/preprocessing/include/dwave-preprocessing/posiform_info.hpp
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    33374 2023-07-21 20:09:06.000000 dwave-preprocessing-0.6.3/dwave/preprocessing/include/dwave-preprocessing/push_relabel.hpp
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2031 2023-07-21 20:09:06.000000 dwave-preprocessing-0.6.3/dwave/preprocessing/libcpp.pxd
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3585 2023-07-21 20:09:06.000000 dwave-preprocessing-0.6.3/dwave/preprocessing/lower_bounds.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-21 20:09:26.360667 dwave-preprocessing-0.6.3/dwave/preprocessing/presolve/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      610 2023-07-21 20:09:06.000000 dwave-preprocessing-0.6.3/dwave/preprocessing/presolve/__init__.pxd
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      719 2023-07-21 20:09:06.000000 dwave-preprocessing-0.6.3/dwave/preprocessing/presolve/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)  1227101 2023-07-21 20:09:26.000000 dwave-preprocessing-0.6.3/dwave/preprocessing/presolve/cypresolve.cpp
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1353 2023-07-21 20:09:06.000000 dwave-preprocessing-0.6.3/dwave/preprocessing/presolve/cypresolve.pxd
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11614 2023-07-21 20:09:06.000000 dwave-preprocessing-0.6.3/dwave/preprocessing/presolve/cypresolve.pyx
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      782 2023-07-21 20:09:06.000000 dwave-preprocessing-0.6.3/dwave/preprocessing/presolve/exceptions.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6036 2023-07-21 20:09:06.000000 dwave-preprocessing-0.6.3/dwave/preprocessing/presolve/pypresolve.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-21 20:09:26.360667 dwave-preprocessing-0.6.3/dwave/preprocessing/src/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      809 2023-07-21 20:09:06.000000 dwave-preprocessing-0.6.3/dwave/preprocessing/src/exceptions.cpp
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3907 2023-07-21 20:09:06.000000 dwave-preprocessing-0.6.3/dwave/preprocessing/src/presolve.cpp
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    41637 2023-07-21 20:09:06.000000 dwave-preprocessing-0.6.3/dwave/preprocessing/src/presolveimpl.hpp
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-21 20:09:26.360667 dwave-preprocessing-0.6.3/dwave_preprocessing.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3242 2023-07-21 20:09:26.000000 dwave-preprocessing-0.6.3/dwave_preprocessing.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6756 2023-07-21 20:09:26.000000 dwave-preprocessing-0.6.3/dwave_preprocessing.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-07-21 20:09:26.000000 dwave-preprocessing-0.6.3/dwave_preprocessing.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-07-21 20:09:26.000000 dwave-preprocessing-0.6.3/dwave_preprocessing.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       43 2023-07-21 20:09:26.000000 dwave-preprocessing-0.6.3/dwave_preprocessing.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        6 2023-07-21 20:09:26.000000 dwave-preprocessing-0.6.3/dwave_preprocessing.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-21 20:09:26.352667 dwave-preprocessing-0.6.3/extern/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-21 20:09:26.360667 dwave-preprocessing-0.6.3/extern/spdlog/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1348 2023-07-21 20:09:11.000000 dwave-preprocessing-0.6.3/extern/spdlog/LICENSE
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-21 20:09:26.352667 dwave-preprocessing-0.6.3/extern/spdlog/include/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-21 20:09:26.364667 dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3587 2023-07-21 20:09:11.000000 dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/async.h
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2494 2023-07-21 20:09:11.000000 dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/async_logger-inl.h
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2276 2023-07-21 20:09:11.000000 dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/async_logger.h
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-21 20:09:26.364667 dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/cfg/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1229 2023-07-21 20:09:11.000000 dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/cfg/argv.h
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      988 2023-07-21 20:09:11.000000 dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/cfg/env.h
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3174 2023-07-21 20:09:11.000000 dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/cfg/helpers-inl.h
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      714 2023-07-21 20:09:11.000000 dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/cfg/helpers.h
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2064 2023-07-21 20:09:11.000000 dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/common-inl.h
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    12011 2023-07-21 20:09:11.000000 dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/common.h
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-21 20:09:26.368667 dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/details/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1884 2023-07-21 20:09:11.000000 dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/details/backtracer-inl.h
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1139 2023-07-21 20:09:11.000000 dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/details/backtracer.h
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3512 2023-07-21 20:09:11.000000 dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/details/circular_q.h
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      609 2023-07-21 20:09:11.000000 dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/details/console_globals.h
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4582 2023-07-21 20:09:11.000000 dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/details/file_helper-inl.h
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1739 2023-07-21 20:09:11.000000 dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/details/file_helper.h
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4586 2023-07-21 20:09:11.000000 dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/details/fmt_helper.h
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1104 2023-07-21 20:09:11.000000 dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/details/log_msg-inl.h
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1154 2023-07-21 20:09:11.000000 dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/details/log_msg.h
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1656 2023-07-21 20:09:11.000000 dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/details/log_msg_buffer-inl.h
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      933 2023-07-21 20:09:11.000000 dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/details/log_msg_buffer.h
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3784 2023-07-21 20:09:11.000000 dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/details/mpmc_blocking_q.h
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      967 2023-07-21 20:09:11.000000 dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/details/null_mutex.h
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    16664 2023-07-21 20:09:11.000000 dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/details/os-inl.h
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3818 2023-07-21 20:09:11.000000 dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/details/os.h
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      622 2023-07-21 20:09:11.000000 dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/details/periodic_worker-inl.h
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1766 2023-07-21 20:09:11.000000 dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/details/periodic_worker.h
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8411 2023-07-21 20:09:11.000000 dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/details/registry-inl.h
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3936 2023-07-21 20:09:11.000000 dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/details/registry.h
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      754 2023-07-21 20:09:11.000000 dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/details/synchronous_factory.h
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4329 2023-07-21 20:09:11.000000 dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/details/tcp_client-windows.h
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3911 2023-07-21 20:09:11.000000 dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/details/tcp_client.h
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3628 2023-07-21 20:09:11.000000 dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/details/thread_pool-inl.h
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3394 2023-07-21 20:09:11.000000 dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/details/thread_pool.h
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3108 2023-07-21 20:09:11.000000 dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/details/udp_client-windows.h
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2264 2023-07-21 20:09:11.000000 dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/details/udp_client.h
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      187 2023-07-21 20:09:11.000000 dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/details/windows_include.h
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-21 20:09:26.368667 dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/fmt/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7284 2023-07-21 20:09:11.000000 dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/fmt/bin_to_hex.h
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-21 20:09:26.368667 dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/fmt/bundled/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7420 2023-07-21 20:09:11.000000 dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/fmt/bundled/args.h
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    68076 2023-07-21 20:09:11.000000 dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/fmt/bundled/chrono.h
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    24896 2023-07-21 20:09:11.000000 dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/fmt/bundled/color.h
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    21245 2023-07-21 20:09:11.000000 dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/fmt/bundled/compile.h
+-rw-r--r--   0 circleci  (3434) circleci  (3434)   111215 2023-07-21 20:09:11.000000 dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/fmt/bundled/core.h
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1408 2023-07-21 20:09:11.000000 dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/fmt/bundled/fmt.license.rst
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    74272 2023-07-21 20:09:11.000000 dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/fmt/bundled/format-inl.h
+-rw-r--r--   0 circleci  (3434) circleci  (3434)   154181 2023-07-21 20:09:11.000000 dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/fmt/bundled/format.h
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      100 2023-07-21 20:09:11.000000 dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/fmt/bundled/locale.h
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    14123 2023-07-21 20:09:11.000000 dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/fmt/bundled/os.h
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7586 2023-07-21 20:09:11.000000 dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/fmt/bundled/ostream.h
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    20023 2023-07-21 20:09:11.000000 dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/fmt/bundled/printf.h
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    23218 2023-07-21 20:09:11.000000 dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/fmt/bundled/ranges.h
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     9001 2023-07-21 20:09:11.000000 dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/fmt/bundled/xchar.h
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      523 2023-07-21 20:09:11.000000 dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/fmt/chrono.h
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      531 2023-07-21 20:09:11.000000 dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/fmt/compile.h
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1004 2023-07-21 20:09:11.000000 dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/fmt/fmt.h
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      526 2023-07-21 20:09:11.000000 dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/fmt/ostr.h
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      523 2023-07-21 20:09:11.000000 dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/fmt/ranges.h
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      520 2023-07-21 20:09:11.000000 dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/fmt/xchar.h
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      462 2023-07-21 20:09:11.000000 dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/formatter.h
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      304 2023-07-21 20:09:11.000000 dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/fwd.h
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7036 2023-07-21 20:09:11.000000 dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/logger-inl.h
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    15636 2023-07-21 20:09:11.000000 dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/logger.h
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    43590 2023-07-21 20:09:11.000000 dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/pattern_formatter-inl.h
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3603 2023-07-21 20:09:11.000000 dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/pattern_formatter.h
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-21 20:09:26.372667 dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/sinks/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4562 2023-07-21 20:09:11.000000 dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/sinks/android_sink.h
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4594 2023-07-21 20:09:11.000000 dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/sinks/ansicolor_sink-inl.h
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3954 2023-07-21 20:09:11.000000 dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/sinks/ansicolor_sink.h
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1778 2023-07-21 20:09:11.000000 dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/sinks/base_sink-inl.h
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1565 2023-07-21 20:09:11.000000 dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/sinks/base_sink.h
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1102 2023-07-21 20:09:11.000000 dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/sinks/basic_file_sink-inl.h
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1834 2023-07-21 20:09:11.000000 dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/sinks/basic_file_sink.h
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    10310 2023-07-21 20:09:11.000000 dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/sinks/daily_file_sink.h
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2438 2023-07-21 20:09:11.000000 dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/sinks/dist_sink.h
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3014 2023-07-21 20:09:11.000000 dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/sinks/dup_filter_sink.h
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6623 2023-07-21 20:09:11.000000 dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/sinks/hourly_file_sink.h
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3744 2023-07-21 20:09:11.000000 dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/sinks/mongo_sink.h
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1545 2023-07-21 20:09:11.000000 dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/sinks/msvc_sink.h
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1229 2023-07-21 20:09:11.000000 dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/sinks/null_sink.h
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1250 2023-07-21 20:09:11.000000 dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/sinks/ostream_sink.h
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3382 2023-07-21 20:09:11.000000 dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/sinks/qt_sinks.h
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2121 2023-07-21 20:09:11.000000 dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/sinks/ringbuffer_sink.h
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4733 2023-07-21 20:09:11.000000 dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/sinks/rotating_file_sink-inl.h
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2648 2023-07-21 20:09:11.000000 dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/sinks/rotating_file_sink.h
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      725 2023-07-21 20:09:11.000000 dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/sinks/sink-inl.h
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      891 2023-07-21 20:09:11.000000 dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/sinks/sink.h
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1214 2023-07-21 20:09:11.000000 dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/sinks/stdout_color_sinks-inl.h
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1626 2023-07-21 20:09:11.000000 dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/sinks/stdout_color_sinks.h
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4364 2023-07-21 20:09:11.000000 dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/sinks/stdout_sinks-inl.h
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2419 2023-07-21 20:09:11.000000 dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/sinks/stdout_sinks.h
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3727 2023-07-21 20:09:11.000000 dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/sinks/syslog_sink.h
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4146 2023-07-21 20:09:11.000000 dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/sinks/systemd_sink.h
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2147 2023-07-21 20:09:11.000000 dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/sinks/tcp_sink.h
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1820 2023-07-21 20:09:11.000000 dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/sinks/udp_sink.h
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8870 2023-07-21 20:09:11.000000 dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/sinks/win_eventlog_sink.h
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6357 2023-07-21 20:09:11.000000 dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/sinks/wincolor_sink-inl.h
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2711 2023-07-21 20:09:11.000000 dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/sinks/wincolor_sink.h
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2974 2023-07-21 20:09:11.000000 dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/spdlog-inl.h
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11279 2023-07-21 20:09:11.000000 dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/spdlog.h
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1726 2023-07-21 20:09:11.000000 dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/stopwatch.h
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6453 2023-07-21 20:09:11.000000 dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/tweakme.h
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      331 2023-07-21 20:09:11.000000 dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/version.h
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      853 2023-07-21 20:09:06.000000 dwave-preprocessing-0.6.3/pyproject.toml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      965 2023-07-21 20:09:26.372667 dwave-preprocessing-0.6.3/setup.cfg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1961 2023-07-21 20:09:06.000000 dwave-preprocessing-0.6.3/setup.py
```

### Comparing `dwave-preprocessing-0.6.2/LICENSE` & `dwave-preprocessing-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dwave-preprocessing-0.6.2/PKG-INFO` & `dwave-preprocessing-0.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dwave-preprocessing
-Version: 0.6.2
+Version: 0.6.3
 Summary: An API for preprocessing tools
 Home-page: https://github.com/dwavesystems/dwave-preprocessing
 Author: D-Wave Systems Inc.
 Author-email: tools@dwavesys.com
 License: Apache 2.0
 Download-URL: https://github.com/dwavesystems/dwave-preprocessing/releases
 Platform: UNKNOWN
```

### Comparing `dwave-preprocessing-0.6.2/README.rst` & `dwave-preprocessing-0.6.3/README.rst`

 * *Files identical despite different names*

### Comparing `dwave-preprocessing-0.6.2/dwave/__init__.py` & `dwave-preprocessing-0.6.3/dwave/__init__.py`

 * *Files identical despite different names*

### Comparing `dwave-preprocessing-0.6.2/dwave/preprocessing/__init__.py` & `dwave-preprocessing-0.6.3/dwave/preprocessing/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = '0.6.2'
+__version__ = '0.6.3'
 
 from dwave.preprocessing import *
 import dwave.preprocessing.composites
 from dwave.preprocessing.composites import *
 import dwave.preprocessing.lower_bounds
 from dwave.preprocessing.lower_bounds import *
```

### Comparing `dwave-preprocessing-0.6.2/dwave/preprocessing/composites/__init__.py` & `dwave-preprocessing-0.6.3/dwave/preprocessing/composites/__init__.py`

 * *Files identical despite different names*

### Comparing `dwave-preprocessing-0.6.2/dwave/preprocessing/composites/clip.py` & `dwave-preprocessing-0.6.3/dwave/preprocessing/composites/clip.py`

 * *Files identical despite different names*

### Comparing `dwave-preprocessing-0.6.2/dwave/preprocessing/composites/connected_components.py` & `dwave-preprocessing-0.6.3/dwave/preprocessing/composites/connected_components.py`

 * *Files identical despite different names*

### Comparing `dwave-preprocessing-0.6.2/dwave/preprocessing/composites/fix_variables.py` & `dwave-preprocessing-0.6.3/dwave/preprocessing/composites/fix_variables.py`

 * *Files identical despite different names*

### Comparing `dwave-preprocessing-0.6.2/dwave/preprocessing/composites/scale.py` & `dwave-preprocessing-0.6.3/dwave/preprocessing/composites/scale.py`

 * *Files identical despite different names*

### Comparing `dwave-preprocessing-0.6.2/dwave/preprocessing/composites/spin_reversal_transform.py` & `dwave-preprocessing-0.6.3/dwave/preprocessing/composites/spin_reversal_transform.py`

 * *Files identical despite different names*

### Comparing `dwave-preprocessing-0.6.2/dwave/preprocessing/cyfix_variables.cpp` & `dwave-preprocessing-0.6.3/dwave/preprocessing/cyfix_variables.cpp`

 * *Files identical despite different names*

### Comparing `dwave-preprocessing-0.6.2/dwave/preprocessing/cyfix_variables.pyx` & `dwave-preprocessing-0.6.3/dwave/preprocessing/cyfix_variables.pyx`

 * *Files identical despite different names*

### Comparing `dwave-preprocessing-0.6.2/dwave/preprocessing/include/dwave/exceptions.hpp` & `dwave-preprocessing-0.6.3/dwave/preprocessing/include/dwave/exceptions.hpp`

 * *Files identical despite different names*

### Comparing `dwave-preprocessing-0.6.2/dwave/preprocessing/include/dwave/flags.hpp` & `dwave-preprocessing-0.6.3/dwave/preprocessing/include/dwave/flags.hpp`

 * *Files identical despite different names*

### Comparing `dwave-preprocessing-0.6.2/dwave/preprocessing/include/dwave/presolve.hpp` & `dwave-preprocessing-0.6.3/dwave/preprocessing/include/dwave/presolve.hpp`

 * *Files identical despite different names*

### Comparing `dwave-preprocessing-0.6.2/dwave/preprocessing/include/dwave-preprocessing/fix_variables.hpp` & `dwave-preprocessing-0.6.3/dwave/preprocessing/include/dwave-preprocessing/fix_variables.hpp`

 * *Files identical despite different names*

### Comparing `dwave-preprocessing-0.6.2/dwave/preprocessing/include/dwave-preprocessing/helper_data_structures.hpp` & `dwave-preprocessing-0.6.3/dwave/preprocessing/include/dwave-preprocessing/helper_data_structures.hpp`

 * *Files identical despite different names*

### Comparing `dwave-preprocessing-0.6.2/dwave/preprocessing/include/dwave-preprocessing/helper_graph_algorithms.hpp` & `dwave-preprocessing-0.6.3/dwave/preprocessing/include/dwave-preprocessing/helper_graph_algorithms.hpp`

 * *Files identical despite different names*

### Comparing `dwave-preprocessing-0.6.2/dwave/preprocessing/include/dwave-preprocessing/implication_network.hpp` & `dwave-preprocessing-0.6.3/dwave/preprocessing/include/dwave-preprocessing/implication_network.hpp`

 * *Files identical despite different names*

### Comparing `dwave-preprocessing-0.6.2/dwave/preprocessing/include/dwave-preprocessing/mapping_policy.hpp` & `dwave-preprocessing-0.6.3/dwave/preprocessing/include/dwave-preprocessing/mapping_policy.hpp`

 * *Files identical despite different names*

### Comparing `dwave-preprocessing-0.6.2/dwave/preprocessing/include/dwave-preprocessing/posiform_info.hpp` & `dwave-preprocessing-0.6.3/dwave/preprocessing/include/dwave-preprocessing/posiform_info.hpp`

 * *Files identical despite different names*

### Comparing `dwave-preprocessing-0.6.2/dwave/preprocessing/include/dwave-preprocessing/push_relabel.hpp` & `dwave-preprocessing-0.6.3/dwave/preprocessing/include/dwave-preprocessing/push_relabel.hpp`

 * *Files identical despite different names*

### Comparing `dwave-preprocessing-0.6.2/dwave/preprocessing/libcpp.pxd` & `dwave-preprocessing-0.6.3/dwave/preprocessing/libcpp.pxd`

 * *Files identical despite different names*

### Comparing `dwave-preprocessing-0.6.2/dwave/preprocessing/lower_bounds.py` & `dwave-preprocessing-0.6.3/dwave/preprocessing/lower_bounds.py`

 * *Files identical despite different names*

### Comparing `dwave-preprocessing-0.6.2/dwave/preprocessing/presolve/__init__.pxd` & `dwave-preprocessing-0.6.3/dwave/preprocessing/presolve/__init__.pxd`

 * *Files identical despite different names*

### Comparing `dwave-preprocessing-0.6.2/dwave/preprocessing/presolve/__init__.py` & `dwave-preprocessing-0.6.3/dwave/preprocessing/presolve/__init__.py`

 * *Files identical despite different names*

### Comparing `dwave-preprocessing-0.6.2/dwave/preprocessing/presolve/cypresolve.cpp` & `dwave-preprocessing-0.6.3/dwave/preprocessing/presolve/cypresolve.cpp`

 * *Files identical despite different names*

### Comparing `dwave-preprocessing-0.6.2/dwave/preprocessing/presolve/cypresolve.pxd` & `dwave-preprocessing-0.6.3/dwave/preprocessing/presolve/cypresolve.pxd`

 * *Files identical despite different names*

### Comparing `dwave-preprocessing-0.6.2/dwave/preprocessing/presolve/cypresolve.pyx` & `dwave-preprocessing-0.6.3/dwave/preprocessing/presolve/cypresolve.pyx`

 * *Files identical despite different names*

### Comparing `dwave-preprocessing-0.6.2/dwave/preprocessing/presolve/exceptions.py` & `dwave-preprocessing-0.6.3/dwave/preprocessing/presolve/exceptions.py`

 * *Files identical despite different names*

### Comparing `dwave-preprocessing-0.6.2/dwave/preprocessing/presolve/pypresolve.py` & `dwave-preprocessing-0.6.3/dwave/preprocessing/presolve/pypresolve.py`

 * *Files identical despite different names*

### Comparing `dwave-preprocessing-0.6.2/dwave/preprocessing/src/exceptions.cpp` & `dwave-preprocessing-0.6.3/dwave/preprocessing/src/exceptions.cpp`

 * *Files identical despite different names*

### Comparing `dwave-preprocessing-0.6.2/dwave/preprocessing/src/presolve.cpp` & `dwave-preprocessing-0.6.3/dwave/preprocessing/src/presolve.cpp`

 * *Files identical despite different names*

### Comparing `dwave-preprocessing-0.6.2/dwave/preprocessing/src/presolveimpl.hpp` & `dwave-preprocessing-0.6.3/dwave/preprocessing/src/presolveimpl.hpp`

 * *Files identical despite different names*

### Comparing `dwave-preprocessing-0.6.2/dwave_preprocessing.egg-info/PKG-INFO` & `dwave-preprocessing-0.6.3/dwave_preprocessing.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dwave-preprocessing
-Version: 0.6.2
+Version: 0.6.3
 Summary: An API for preprocessing tools
 Home-page: https://github.com/dwavesystems/dwave-preprocessing
 Author: D-Wave Systems Inc.
 Author-email: tools@dwavesys.com
 License: Apache 2.0
 Download-URL: https://github.com/dwavesystems/dwave-preprocessing/releases
 Platform: UNKNOWN
```

### Comparing `dwave-preprocessing-0.6.2/dwave_preprocessing.egg-info/SOURCES.txt` & `dwave-preprocessing-0.6.3/dwave_preprocessing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dwave-preprocessing-0.6.2/extern/spdlog/LICENSE` & `dwave-preprocessing-0.6.3/extern/spdlog/LICENSE`

 * *Files identical despite different names*

### Comparing `dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/async.h` & `dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/async.h`

 * *Files identical despite different names*

### Comparing `dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/async_logger-inl.h` & `dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/async_logger-inl.h`

 * *Files identical despite different names*

### Comparing `dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/async_logger.h` & `dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/async_logger.h`

 * *Files identical despite different names*

### Comparing `dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/cfg/argv.h` & `dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/cfg/argv.h`

 * *Files identical despite different names*

### Comparing `dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/cfg/env.h` & `dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/cfg/env.h`

 * *Files identical despite different names*

### Comparing `dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/cfg/helpers-inl.h` & `dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/cfg/helpers-inl.h`

 * *Files identical despite different names*

### Comparing `dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/cfg/helpers.h` & `dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/cfg/helpers.h`

 * *Files identical despite different names*

### Comparing `dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/common-inl.h` & `dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/common-inl.h`

 * *Files identical despite different names*

### Comparing `dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/common.h` & `dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/common.h`

 * *Files identical despite different names*

### Comparing `dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/details/backtracer-inl.h` & `dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/details/backtracer-inl.h`

 * *Files identical despite different names*

### Comparing `dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/details/backtracer.h` & `dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/details/backtracer.h`

 * *Files identical despite different names*

### Comparing `dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/details/circular_q.h` & `dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/details/circular_q.h`

 * *Files identical despite different names*

### Comparing `dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/details/console_globals.h` & `dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/details/console_globals.h`

 * *Files identical despite different names*

### Comparing `dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/details/file_helper-inl.h` & `dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/details/file_helper-inl.h`

 * *Files identical despite different names*

### Comparing `dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/details/file_helper.h` & `dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/details/file_helper.h`

 * *Files identical despite different names*

### Comparing `dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/details/fmt_helper.h` & `dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/details/fmt_helper.h`

 * *Files identical despite different names*

### Comparing `dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/details/log_msg-inl.h` & `dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/details/log_msg-inl.h`

 * *Files identical despite different names*

### Comparing `dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/details/log_msg.h` & `dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/details/log_msg.h`

 * *Files identical despite different names*

### Comparing `dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/details/log_msg_buffer-inl.h` & `dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/details/log_msg_buffer-inl.h`

 * *Files identical despite different names*

### Comparing `dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/details/log_msg_buffer.h` & `dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/details/log_msg_buffer.h`

 * *Files identical despite different names*

### Comparing `dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/details/mpmc_blocking_q.h` & `dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/details/mpmc_blocking_q.h`

 * *Files identical despite different names*

### Comparing `dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/details/null_mutex.h` & `dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/details/null_mutex.h`

 * *Files identical despite different names*

### Comparing `dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/details/os-inl.h` & `dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/details/os-inl.h`

 * *Files identical despite different names*

### Comparing `dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/details/os.h` & `dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/details/os.h`

 * *Files identical despite different names*

### Comparing `dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/details/periodic_worker-inl.h` & `dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/details/periodic_worker-inl.h`

 * *Files identical despite different names*

### Comparing `dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/details/periodic_worker.h` & `dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/details/periodic_worker.h`

 * *Files identical despite different names*

### Comparing `dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/details/registry-inl.h` & `dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/details/registry-inl.h`

 * *Files identical despite different names*

### Comparing `dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/details/registry.h` & `dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/details/registry.h`

 * *Files identical despite different names*

### Comparing `dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/details/synchronous_factory.h` & `dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/details/synchronous_factory.h`

 * *Files identical despite different names*

### Comparing `dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/details/tcp_client-windows.h` & `dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/details/tcp_client-windows.h`

 * *Files identical despite different names*

### Comparing `dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/details/tcp_client.h` & `dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/details/tcp_client.h`

 * *Files identical despite different names*

### Comparing `dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/details/thread_pool-inl.h` & `dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/details/thread_pool-inl.h`

 * *Files identical despite different names*

### Comparing `dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/details/thread_pool.h` & `dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/details/thread_pool.h`

 * *Files identical despite different names*

### Comparing `dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/details/udp_client-windows.h` & `dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/details/udp_client-windows.h`

 * *Files identical despite different names*

### Comparing `dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/details/udp_client.h` & `dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/details/udp_client.h`

 * *Files identical despite different names*

### Comparing `dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/fmt/bin_to_hex.h` & `dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/fmt/bin_to_hex.h`

 * *Files identical despite different names*

### Comparing `dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/fmt/bundled/args.h` & `dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/fmt/bundled/args.h`

 * *Files identical despite different names*

### Comparing `dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/fmt/bundled/chrono.h` & `dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/fmt/bundled/chrono.h`

 * *Files identical despite different names*

### Comparing `dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/fmt/bundled/color.h` & `dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/fmt/bundled/color.h`

 * *Files identical despite different names*

### Comparing `dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/fmt/bundled/compile.h` & `dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/fmt/bundled/compile.h`

 * *Files identical despite different names*

### Comparing `dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/fmt/bundled/core.h` & `dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/fmt/bundled/core.h`

 * *Files identical despite different names*

### Comparing `dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/fmt/bundled/fmt.license.rst` & `dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/fmt/bundled/fmt.license.rst`

 * *Files identical despite different names*

### Comparing `dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/fmt/bundled/format-inl.h` & `dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/fmt/bundled/format-inl.h`

 * *Files identical despite different names*

### Comparing `dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/fmt/bundled/format.h` & `dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/fmt/bundled/format.h`

 * *Files identical despite different names*

### Comparing `dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/fmt/bundled/os.h` & `dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/fmt/bundled/os.h`

 * *Files identical despite different names*

### Comparing `dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/fmt/bundled/ostream.h` & `dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/fmt/bundled/ostream.h`

 * *Files identical despite different names*

### Comparing `dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/fmt/bundled/printf.h` & `dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/fmt/bundled/printf.h`

 * *Files identical despite different names*

### Comparing `dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/fmt/bundled/ranges.h` & `dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/fmt/bundled/ranges.h`

 * *Files identical despite different names*

### Comparing `dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/fmt/bundled/xchar.h` & `dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/fmt/bundled/xchar.h`

 * *Files identical despite different names*

### Comparing `dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/fmt/chrono.h` & `dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/fmt/chrono.h`

 * *Files identical despite different names*

### Comparing `dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/fmt/compile.h` & `dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/fmt/compile.h`

 * *Files identical despite different names*

### Comparing `dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/fmt/fmt.h` & `dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/fmt/fmt.h`

 * *Files identical despite different names*

### Comparing `dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/fmt/ostr.h` & `dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/fmt/ostr.h`

 * *Files identical despite different names*

### Comparing `dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/fmt/ranges.h` & `dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/fmt/ranges.h`

 * *Files identical despite different names*

### Comparing `dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/fmt/xchar.h` & `dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/fmt/xchar.h`

 * *Files identical despite different names*

### Comparing `dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/logger-inl.h` & `dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/logger-inl.h`

 * *Files identical despite different names*

### Comparing `dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/logger.h` & `dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/logger.h`

 * *Files identical despite different names*

### Comparing `dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/pattern_formatter-inl.h` & `dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/pattern_formatter-inl.h`

 * *Files identical despite different names*

### Comparing `dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/pattern_formatter.h` & `dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/pattern_formatter.h`

 * *Files identical despite different names*

### Comparing `dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/sinks/android_sink.h` & `dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/sinks/android_sink.h`

 * *Files identical despite different names*

### Comparing `dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/sinks/ansicolor_sink-inl.h` & `dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/sinks/ansicolor_sink-inl.h`

 * *Files identical despite different names*

### Comparing `dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/sinks/ansicolor_sink.h` & `dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/sinks/ansicolor_sink.h`

 * *Files identical despite different names*

### Comparing `dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/sinks/base_sink-inl.h` & `dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/sinks/base_sink-inl.h`

 * *Files identical despite different names*

### Comparing `dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/sinks/base_sink.h` & `dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/sinks/base_sink.h`

 * *Files identical despite different names*

### Comparing `dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/sinks/basic_file_sink-inl.h` & `dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/sinks/basic_file_sink-inl.h`

 * *Files identical despite different names*

### Comparing `dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/sinks/basic_file_sink.h` & `dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/sinks/basic_file_sink.h`

 * *Files identical despite different names*

### Comparing `dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/sinks/daily_file_sink.h` & `dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/sinks/daily_file_sink.h`

 * *Files identical despite different names*

### Comparing `dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/sinks/dist_sink.h` & `dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/sinks/dist_sink.h`

 * *Files identical despite different names*

### Comparing `dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/sinks/dup_filter_sink.h` & `dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/sinks/dup_filter_sink.h`

 * *Files identical despite different names*

### Comparing `dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/sinks/hourly_file_sink.h` & `dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/sinks/hourly_file_sink.h`

 * *Files identical despite different names*

### Comparing `dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/sinks/mongo_sink.h` & `dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/sinks/mongo_sink.h`

 * *Files identical despite different names*

### Comparing `dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/sinks/msvc_sink.h` & `dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/sinks/msvc_sink.h`

 * *Files identical despite different names*

### Comparing `dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/sinks/null_sink.h` & `dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/sinks/null_sink.h`

 * *Files identical despite different names*

### Comparing `dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/sinks/ostream_sink.h` & `dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/sinks/ostream_sink.h`

 * *Files identical despite different names*

### Comparing `dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/sinks/qt_sinks.h` & `dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/sinks/qt_sinks.h`

 * *Files identical despite different names*

### Comparing `dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/sinks/ringbuffer_sink.h` & `dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/sinks/ringbuffer_sink.h`

 * *Files identical despite different names*

### Comparing `dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/sinks/rotating_file_sink-inl.h` & `dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/sinks/rotating_file_sink-inl.h`

 * *Files identical despite different names*

### Comparing `dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/sinks/rotating_file_sink.h` & `dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/sinks/rotating_file_sink.h`

 * *Files identical despite different names*

### Comparing `dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/sinks/sink-inl.h` & `dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/sinks/sink-inl.h`

 * *Files identical despite different names*

### Comparing `dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/sinks/sink.h` & `dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/sinks/sink.h`

 * *Files identical despite different names*

### Comparing `dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/sinks/stdout_color_sinks-inl.h` & `dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/sinks/stdout_color_sinks-inl.h`

 * *Files identical despite different names*

### Comparing `dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/sinks/stdout_color_sinks.h` & `dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/sinks/stdout_color_sinks.h`

 * *Files identical despite different names*

### Comparing `dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/sinks/stdout_sinks-inl.h` & `dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/sinks/stdout_sinks-inl.h`

 * *Files identical despite different names*

### Comparing `dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/sinks/stdout_sinks.h` & `dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/sinks/stdout_sinks.h`

 * *Files identical despite different names*

### Comparing `dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/sinks/syslog_sink.h` & `dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/sinks/syslog_sink.h`

 * *Files identical despite different names*

### Comparing `dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/sinks/systemd_sink.h` & `dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/sinks/systemd_sink.h`

 * *Files identical despite different names*

### Comparing `dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/sinks/tcp_sink.h` & `dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/sinks/tcp_sink.h`

 * *Files identical despite different names*

### Comparing `dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/sinks/udp_sink.h` & `dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/sinks/udp_sink.h`

 * *Files identical despite different names*

### Comparing `dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/sinks/win_eventlog_sink.h` & `dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/sinks/win_eventlog_sink.h`

 * *Files identical despite different names*

### Comparing `dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/sinks/wincolor_sink-inl.h` & `dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/sinks/wincolor_sink-inl.h`

 * *Files identical despite different names*

### Comparing `dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/sinks/wincolor_sink.h` & `dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/sinks/wincolor_sink.h`

 * *Files identical despite different names*

### Comparing `dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/spdlog-inl.h` & `dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/spdlog-inl.h`

 * *Files identical despite different names*

### Comparing `dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/spdlog.h` & `dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/spdlog.h`

 * *Files identical despite different names*

### Comparing `dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/stopwatch.h` & `dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/stopwatch.h`

 * *Files identical despite different names*

### Comparing `dwave-preprocessing-0.6.2/extern/spdlog/include/spdlog/tweakme.h` & `dwave-preprocessing-0.6.3/extern/spdlog/include/spdlog/tweakme.h`

 * *Files identical despite different names*

### Comparing `dwave-preprocessing-0.6.2/setup.cfg` & `dwave-preprocessing-0.6.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `dwave-preprocessing-0.6.2/setup.py` & `dwave-preprocessing-0.6.3/setup.py`

 * *Files identical despite different names*

