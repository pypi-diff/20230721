# Comparing `tmp/rapidfuzz-3.1.1.tar.gz` & `tmp/rapidfuzz-3.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rapidfuzz-3.1.1.tar", last modified: Tue Jun  6 12:33:19 2023, max compression
+gzip compressed data, was "rapidfuzz-3.1.2.tar", last modified: Thu Jul 20 21:25:12 2023, max compression
```

## Comparing `rapidfuzz-3.1.1.tar` & `rapidfuzz-3.1.2.tar`

### file list

```diff
@@ -1,283 +1,283 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:33:19.081034 rapidfuzz-3.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    27953 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11268 2023-06-06 12:33:19.081034 rapidfuzz-3.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10600 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:33:19.001035 rapidfuzz-3.1.1/_custom_build/
--rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/_custom_build/backend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:33:19.001035 rapidfuzz-3.1.1/cmake/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/cmake/CheckCPUArch.c.in
--rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/cmake/CheckCPUArch.cmake
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:33:19.001035 rapidfuzz-3.1.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:33:19.001035 rapidfuzz-3.1.1/docs/Contributing/
--rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/docs/Contributing/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/docs/Installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/docs/License.rst
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/docs/References.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:33:19.005035 rapidfuzz-3.1.1/docs/Usage/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:33:19.005035 rapidfuzz-3.1.1/docs/Usage/distance/
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/docs/Usage/distance/DamerauLevenshtein.rst
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/docs/Usage/distance/Hamming.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/docs/Usage/distance/Indel.rst
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/docs/Usage/distance/Jaro.rst
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/docs/Usage/distance/JaroWinkler.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/docs/Usage/distance/Levenshtein.rst
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/docs/Usage/distance/OSA.rst
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/docs/Usage/distance/Postfix.rst
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/docs/Usage/distance/Prefix.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:33:19.005035 rapidfuzz-3.1.1/docs/Usage/distance/img/
--rw-r--r--   0 runner    (1001) docker     (123)    37487 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/docs/Usage/distance/img/damerau_levenshtein.svg
--rw-r--r--   0 runner    (1001) docker     (123)    42028 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/docs/Usage/distance/img/indel_levenshtein.svg
--rw-r--r--   0 runner    (1001) docker     (123)    34090 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/docs/Usage/distance/img/jaro.svg
--rw-r--r--   0 runner    (1001) docker     (123)    34913 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/docs/Usage/distance/img/jaro_winkler.svg
--rw-r--r--   0 runner    (1001) docker     (123)    37821 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/docs/Usage/distance/img/osa.svg
--rw-r--r--   0 runner    (1001) docker     (123)    32664 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/docs/Usage/distance/img/uniform_levenshtein.svg
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/docs/Usage/distance/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/docs/Usage/fuzz.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:33:19.009034 rapidfuzz-3.1.1/docs/Usage/img/
--rw-r--r--   0 runner    (1001) docker     (123)    25251 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/docs/Usage/img/WRatio.svg
--rw-r--r--   0 runner    (1001) docker     (123)    42028 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/docs/Usage/img/indel_levenshtein.svg
--rw-r--r--   0 runner    (1001) docker     (123)    41626 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/docs/Usage/img/partial_ratio_long_needle.svg
--rw-r--r--   0 runner    (1001) docker     (123)    41360 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/docs/Usage/img/partial_ratio_short_needle.svg
--rw-r--r--   0 runner    (1001) docker     (123)    28491 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/docs/Usage/img/partial_token_ratio.svg
--rw-r--r--   0 runner    (1001) docker     (123)    24769 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/docs/Usage/img/partial_token_set_ratio.svg
--rw-r--r--   0 runner    (1001) docker     (123)    25404 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/docs/Usage/img/partial_token_sort_ratio.svg
--rw-r--r--   0 runner    (1001) docker     (123)    24367 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/docs/Usage/img/ratio.svg
--rw-r--r--   0 runner    (1001) docker     (123)    27273 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/docs/Usage/img/token_ratio.svg
--rw-r--r--   0 runner    (1001) docker     (123)    25693 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/docs/Usage/img/token_set_ratio.svg
--rw-r--r--   0 runner    (1001) docker     (123)    26611 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/docs/Usage/img/token_sort_ratio.svg
--rw-r--r--   0 runner    (1001) docker     (123)    32664 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/docs/Usage/img/uniform_levenshtein.svg
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/docs/Usage/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/docs/Usage/process.rst
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/docs/Usage/utils.rst
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/docs/changelog_link.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:33:19.013034 rapidfuzz-3.1.1/docs/img/
--rw-r--r--   0 runner    (1001) docker     (123)     5879 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/docs/img/RapidFuzz.svg
--rw-r--r--   0 runner    (1001) docker     (123)    56024 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/docs/img/cdist.svg
--rw-r--r--   0 runner    (1001) docker     (123)    54183 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/docs/img/scorer.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3160 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/docs/refs.bib
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:33:18.993034 rapidfuzz-3.1.1/extern/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:33:19.013034 rapidfuzz-3.1.1/extern/rapidfuzz-cpp/
--rw-r--r--   0 runner    (1001) docker     (123)     4397 2023-06-06 12:32:28.000000 rapidfuzz-3.1.1/extern/rapidfuzz-cpp/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-06 12:32:28.000000 rapidfuzz-3.1.1/extern/rapidfuzz-cpp/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:33:19.013034 rapidfuzz-3.1.1/extern/rapidfuzz-cpp/rapidfuzz/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:33:19.017034 rapidfuzz-3.1.1/extern/rapidfuzz-cpp/rapidfuzz/details/
--rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-06-06 12:32:28.000000 rapidfuzz-3.1.1/extern/rapidfuzz-cpp/rapidfuzz/details/CharSet.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4861 2023-06-06 12:32:28.000000 rapidfuzz-3.1.1/extern/rapidfuzz-cpp/rapidfuzz/details/GrowingHashmap.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4622 2023-06-06 12:32:28.000000 rapidfuzz-3.1.1/extern/rapidfuzz-cpp/rapidfuzz/details/Matrix.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5592 2023-06-06 12:32:28.000000 rapidfuzz-3.1.1/extern/rapidfuzz-cpp/rapidfuzz/details/PatternMatchVector.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-06-06 12:32:28.000000 rapidfuzz-3.1.1/extern/rapidfuzz-cpp/rapidfuzz/details/Range.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-06-06 12:32:28.000000 rapidfuzz-3.1.1/extern/rapidfuzz-cpp/rapidfuzz/details/SplittedSentenceView.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-06-06 12:32:28.000000 rapidfuzz-3.1.1/extern/rapidfuzz-cpp/rapidfuzz/details/common.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4345 2023-06-06 12:32:28.000000 rapidfuzz-3.1.1/extern/rapidfuzz-cpp/rapidfuzz/details/common_impl.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    23057 2023-06-06 12:32:28.000000 rapidfuzz-3.1.1/extern/rapidfuzz-cpp/rapidfuzz/details/distance.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4992 2023-06-06 12:32:28.000000 rapidfuzz-3.1.1/extern/rapidfuzz-cpp/rapidfuzz/details/intrinsics.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-06-06 12:32:28.000000 rapidfuzz-3.1.1/extern/rapidfuzz-cpp/rapidfuzz/details/simd.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    10815 2023-06-06 12:32:28.000000 rapidfuzz-3.1.1/extern/rapidfuzz-cpp/rapidfuzz/details/simd_avx2.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    11538 2023-06-06 12:32:28.000000 rapidfuzz-3.1.1/extern/rapidfuzz-cpp/rapidfuzz/details/simd_sse2.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-06-06 12:32:28.000000 rapidfuzz-3.1.1/extern/rapidfuzz-cpp/rapidfuzz/details/type_traits.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    17508 2023-06-06 12:32:28.000000 rapidfuzz-3.1.1/extern/rapidfuzz-cpp/rapidfuzz/details/types.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:33:19.021034 rapidfuzz-3.1.1/extern/rapidfuzz-cpp/rapidfuzz/distance/
--rw-r--r--   0 runner    (1001) docker     (123)     6231 2023-06-06 12:32:28.000000 rapidfuzz-3.1.1/extern/rapidfuzz-cpp/rapidfuzz/distance/DamerauLevenshtein.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-06-06 12:32:28.000000 rapidfuzz-3.1.1/extern/rapidfuzz-cpp/rapidfuzz/distance/DamerauLevenshtein_impl.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6734 2023-06-06 12:32:28.000000 rapidfuzz-3.1.1/extern/rapidfuzz-cpp/rapidfuzz/distance/Hamming.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-06-06 12:32:28.000000 rapidfuzz-3.1.1/extern/rapidfuzz-cpp/rapidfuzz/distance/Hamming_impl.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6493 2023-06-06 12:32:28.000000 rapidfuzz-3.1.1/extern/rapidfuzz-cpp/rapidfuzz/distance/Indel.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-06-06 12:32:28.000000 rapidfuzz-3.1.1/extern/rapidfuzz-cpp/rapidfuzz/distance/Indel_impl.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3603 2023-06-06 12:32:28.000000 rapidfuzz-3.1.1/extern/rapidfuzz-cpp/rapidfuzz/distance/Jaro.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5047 2023-06-06 12:32:28.000000 rapidfuzz-3.1.1/extern/rapidfuzz-cpp/rapidfuzz/distance/JaroWinkler.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-06-06 12:32:28.000000 rapidfuzz-3.1.1/extern/rapidfuzz-cpp/rapidfuzz/distance/JaroWinkler_impl.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    14569 2023-06-06 12:32:28.000000 rapidfuzz-3.1.1/extern/rapidfuzz-cpp/rapidfuzz/distance/Jaro_impl.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     8228 2023-06-06 12:32:28.000000 rapidfuzz-3.1.1/extern/rapidfuzz-cpp/rapidfuzz/distance/LCSseq.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    14461 2023-06-06 12:32:28.000000 rapidfuzz-3.1.1/extern/rapidfuzz-cpp/rapidfuzz/distance/LCSseq_impl.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    20759 2023-06-06 12:32:28.000000 rapidfuzz-3.1.1/extern/rapidfuzz-cpp/rapidfuzz/distance/Levenshtein.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    44317 2023-06-06 12:32:28.000000 rapidfuzz-3.1.1/extern/rapidfuzz-cpp/rapidfuzz/distance/Levenshtein_impl.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     9648 2023-06-06 12:32:28.000000 rapidfuzz-3.1.1/extern/rapidfuzz-cpp/rapidfuzz/distance/OSA.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     9729 2023-06-06 12:32:28.000000 rapidfuzz-3.1.1/extern/rapidfuzz-cpp/rapidfuzz/distance/OSA_impl.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-06-06 12:32:28.000000 rapidfuzz-3.1.1/extern/rapidfuzz-cpp/rapidfuzz/distance/Postfix.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-06-06 12:32:28.000000 rapidfuzz-3.1.1/extern/rapidfuzz-cpp/rapidfuzz/distance/Postfix_impl.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3931 2023-06-06 12:32:28.000000 rapidfuzz-3.1.1/extern/rapidfuzz-cpp/rapidfuzz/distance/Prefix.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-06-06 12:32:28.000000 rapidfuzz-3.1.1/extern/rapidfuzz-cpp/rapidfuzz/distance/Prefix_impl.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3833 2023-06-06 12:32:28.000000 rapidfuzz-3.1.1/extern/rapidfuzz-cpp/rapidfuzz/distance.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    27750 2023-06-06 12:32:28.000000 rapidfuzz-3.1.1/extern/rapidfuzz-cpp/rapidfuzz/fuzz.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    37923 2023-06-06 12:32:28.000000 rapidfuzz-3.1.1/extern/rapidfuzz-cpp/rapidfuzz/fuzz.impl
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-06 12:32:28.000000 rapidfuzz-3.1.1/extern/rapidfuzz-cpp/rapidfuzz/rapidfuzz_all.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:33:19.025034 rapidfuzz-3.1.1/extern/taskflow/
--rw-r--r--   0 runner    (1001) docker     (123)    14095 2023-06-06 12:32:30.000000 rapidfuzz-3.1.1/extern/taskflow/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-06 12:32:30.000000 rapidfuzz-3.1.1/extern/taskflow/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-06 12:32:30.000000 rapidfuzz-3.1.1/extern/taskflow/TaskflowConfig.cmake.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:33:19.025034 rapidfuzz-3.1.1/extern/taskflow/taskflow/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:33:19.025034 rapidfuzz-3.1.1/extern/taskflow/taskflow/algorithm/
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-06-06 12:32:31.000000 rapidfuzz-3.1.1/extern/taskflow/taskflow/algorithm/critical.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    16653 2023-06-06 12:32:31.000000 rapidfuzz-3.1.1/extern/taskflow/taskflow/algorithm/data_pipeline.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    14972 2023-06-06 12:32:31.000000 rapidfuzz-3.1.1/extern/taskflow/taskflow/algorithm/find.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4928 2023-06-06 12:32:31.000000 rapidfuzz-3.1.1/extern/taskflow/taskflow/algorithm/for_each.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-06-06 12:32:31.000000 rapidfuzz-3.1.1/extern/taskflow/taskflow/algorithm/launch.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    14524 2023-06-06 12:32:31.000000 rapidfuzz-3.1.1/extern/taskflow/taskflow/algorithm/partitioner.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    44892 2023-06-06 12:32:31.000000 rapidfuzz-3.1.1/extern/taskflow/taskflow/algorithm/pipeline.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     7902 2023-06-06 12:32:31.000000 rapidfuzz-3.1.1/extern/taskflow/taskflow/algorithm/reduce.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    17090 2023-06-06 12:32:31.000000 rapidfuzz-3.1.1/extern/taskflow/taskflow/algorithm/scan.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    20947 2023-06-06 12:32:31.000000 rapidfuzz-3.1.1/extern/taskflow/taskflow/algorithm/sort.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5870 2023-06-06 12:32:31.000000 rapidfuzz-3.1.1/extern/taskflow/taskflow/algorithm/transform.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:33:19.029034 rapidfuzz-3.1.1/extern/taskflow/taskflow/core/
--rw-r--r--   0 runner    (1001) docker     (123)    10955 2023-06-06 12:32:31.000000 rapidfuzz-3.1.1/extern/taskflow/taskflow/core/async.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-06-06 12:32:31.000000 rapidfuzz-3.1.1/extern/taskflow/taskflow/core/async_task.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-06-06 12:32:31.000000 rapidfuzz-3.1.1/extern/taskflow/taskflow/core/declarations.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-06 12:32:31.000000 rapidfuzz-3.1.1/extern/taskflow/taskflow/core/environment.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-06 12:32:31.000000 rapidfuzz-3.1.1/extern/taskflow/taskflow/core/error.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    54781 2023-06-06 12:32:31.000000 rapidfuzz-3.1.1/extern/taskflow/taskflow/core/executor-module-opt.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    66789 2023-06-06 12:32:31.000000 rapidfuzz-3.1.1/extern/taskflow/taskflow/core/executor.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    41751 2023-06-06 12:32:31.000000 rapidfuzz-3.1.1/extern/taskflow/taskflow/core/flow_builder.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    24153 2023-06-06 12:32:31.000000 rapidfuzz-3.1.1/extern/taskflow/taskflow/core/graph.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     9176 2023-06-06 12:32:31.000000 rapidfuzz-3.1.1/extern/taskflow/taskflow/core/notifier.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    26126 2023-06-06 12:32:31.000000 rapidfuzz-3.1.1/extern/taskflow/taskflow/core/observer.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-06-06 12:32:31.000000 rapidfuzz-3.1.1/extern/taskflow/taskflow/core/semaphore.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    18519 2023-06-06 12:32:31.000000 rapidfuzz-3.1.1/extern/taskflow/taskflow/core/task.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    15758 2023-06-06 12:32:31.000000 rapidfuzz-3.1.1/extern/taskflow/taskflow/core/taskflow.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-06 12:32:31.000000 rapidfuzz-3.1.1/extern/taskflow/taskflow/core/topology.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    12210 2023-06-06 12:32:31.000000 rapidfuzz-3.1.1/extern/taskflow/taskflow/core/tsq.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-06-06 12:32:31.000000 rapidfuzz-3.1.1/extern/taskflow/taskflow/core/worker.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-06-06 12:32:31.000000 rapidfuzz-3.1.1/extern/taskflow/taskflow/taskflow.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:33:19.033034 rapidfuzz-3.1.1/extern/taskflow/taskflow/utility/
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-06-06 12:32:31.000000 rapidfuzz-3.1.1/extern/taskflow/taskflow/utility/iterator.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-06 12:32:31.000000 rapidfuzz-3.1.1/extern/taskflow/taskflow/utility/macros.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-06-06 12:32:31.000000 rapidfuzz-3.1.1/extern/taskflow/taskflow/utility/math.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    19899 2023-06-06 12:32:31.000000 rapidfuzz-3.1.1/extern/taskflow/taskflow/utility/object_pool.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-06-06 12:32:31.000000 rapidfuzz-3.1.1/extern/taskflow/taskflow/utility/os.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    29321 2023-06-06 12:32:31.000000 rapidfuzz-3.1.1/extern/taskflow/taskflow/utility/serializer.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-06-06 12:32:31.000000 rapidfuzz-3.1.1/extern/taskflow/taskflow/utility/singleton.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    31329 2023-06-06 12:32:31.000000 rapidfuzz-3.1.1/extern/taskflow/taskflow/utility/small_vector.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-06-06 12:32:31.000000 rapidfuzz-3.1.1/extern/taskflow/taskflow/utility/stream.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     8631 2023-06-06 12:32:31.000000 rapidfuzz-3.1.1/extern/taskflow/taskflow/utility/traits.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5685 2023-06-06 12:32:31.000000 rapidfuzz-3.1.1/extern/taskflow/taskflow/utility/uuid.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-06-06 12:33:07.000000 rapidfuzz-3.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 12:33:19.081034 rapidfuzz-3.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:33:18.997034 rapidfuzz-3.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:33:19.053034 rapidfuzz-3.1.1/src/rapidfuzz/
--rw-r--r--   0 runner    (1001) docker     (123)     5251 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/src/rapidfuzz/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:33:19.053034 rapidfuzz-3.1.1/src/rapidfuzz/FeatureDetector/
--rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/src/rapidfuzz/FeatureDetector/CpuInfo.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/src/rapidfuzz/FeatureDetector/CpuInfo.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/src/rapidfuzz/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/src/rapidfuzz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/src/rapidfuzz/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:33:19.053034 rapidfuzz-3.1.1/src/rapidfuzz/__pyinstaller/
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/src/rapidfuzz/__pyinstaller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/src/rapidfuzz/__pyinstaller/hook-rapidfuzz.py
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/src/rapidfuzz/__pyinstaller/test_rapidfuzz_packaging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/src/rapidfuzz/_common_py.py
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/src/rapidfuzz/_feature_detector.py
--rw-r--r--   0 runner    (1001) docker     (123)   245534 2023-06-06 12:33:01.000000 rapidfuzz-3.1.1/src/rapidfuzz/_feature_detector_cpp.cxx
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/src/rapidfuzz/_feature_detector_cpp.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     3627 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/src/rapidfuzz/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    25512 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/src/rapidfuzz/cpp_common.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    15706 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/src/rapidfuzz/cpp_common.pxd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:33:19.073034 rapidfuzz-3.1.1/src/rapidfuzz/distance/
--rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/src/rapidfuzz/distance/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/src/rapidfuzz/distance/DamerauLevenshtein.py
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/src/rapidfuzz/distance/DamerauLevenshtein.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7090 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/src/rapidfuzz/distance/DamerauLevenshtein_py.py
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/src/rapidfuzz/distance/Hamming.py
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/src/rapidfuzz/distance/Hamming.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9757 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/src/rapidfuzz/distance/Hamming_py.py
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/src/rapidfuzz/distance/Indel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/src/rapidfuzz/distance/Indel.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10934 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/src/rapidfuzz/distance/Indel_py.py
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/src/rapidfuzz/distance/Jaro.py
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/src/rapidfuzz/distance/Jaro.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/src/rapidfuzz/distance/JaroWinkler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/src/rapidfuzz/distance/JaroWinkler.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6781 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/src/rapidfuzz/distance/JaroWinkler_py.py
--rw-r--r--   0 runner    (1001) docker     (123)     7960 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/src/rapidfuzz/distance/Jaro_py.py
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/src/rapidfuzz/distance/LCSseq.py
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/src/rapidfuzz/distance/LCSseq.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10290 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/src/rapidfuzz/distance/LCSseq_py.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/src/rapidfuzz/distance/Levenshtein.py
--rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/src/rapidfuzz/distance/Levenshtein.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    15750 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/src/rapidfuzz/distance/Levenshtein_py.py
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/src/rapidfuzz/distance/OSA.py
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/src/rapidfuzz/distance/OSA.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6748 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/src/rapidfuzz/distance/OSA_py.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/src/rapidfuzz/distance/Postfix.py
--rw-r--r--   0 runner    (1001) docker     (123)     5468 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/src/rapidfuzz/distance/Postfix_py.py
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/src/rapidfuzz/distance/Prefix.py
--rw-r--r--   0 runner    (1001) docker     (123)     5444 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/src/rapidfuzz/distance/Prefix_py.py
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/src/rapidfuzz/distance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/src/rapidfuzz/distance/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/src/rapidfuzz/distance/_initialize.py
--rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/src/rapidfuzz/distance/_initialize.pyi
--rw-r--r--   0 runner    (1001) docker     (123)  1620171 2023-06-06 12:33:03.000000 rapidfuzz-3.1.1/src/rapidfuzz/distance/_initialize_cpp.cxx
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/src/rapidfuzz/distance/_initialize_cpp.pxd
--rw-r--r--   0 runner    (1001) docker     (123)    29674 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/src/rapidfuzz/distance/_initialize_cpp.pyx
--rw-r--r--   0 runner    (1001) docker     (123)    28423 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/src/rapidfuzz/distance/_initialize_py.py
--rw-r--r--   0 runner    (1001) docker     (123)    29777 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/src/rapidfuzz/distance/metrics.hpp
--rw-r--r--   0 runner    (1001) docker     (123)  1391567 2023-06-06 12:33:05.000000 rapidfuzz-3.1.1/src/rapidfuzz/distance/metrics_cpp.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     7051 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/src/rapidfuzz/distance/metrics_cpp.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    57041 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/src/rapidfuzz/distance/metrics_cpp.pyx
--rw-r--r--   0 runner    (1001) docker     (123)  1399916 2023-06-06 12:33:06.000000 rapidfuzz-3.1.1/src/rapidfuzz/distance/metrics_cpp_avx2.cxx
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/src/rapidfuzz/distance/metrics_cpp_avx2.pyx
--rw-r--r--   0 runner    (1001) docker     (123)    10618 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/src/rapidfuzz/distance/metrics_py.py
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/src/rapidfuzz/fuzz.py
--rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/src/rapidfuzz/fuzz.pyi
--rw-r--r--   0 runner    (1001) docker     (123)   608429 2023-06-06 12:32:56.000000 rapidfuzz-3.1.1/src/rapidfuzz/fuzz_cpp.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     5876 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/src/rapidfuzz/fuzz_cpp.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    10319 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/src/rapidfuzz/fuzz_cpp.pyx
--rw-r--r--   0 runner    (1001) docker     (123)   610422 2023-06-06 12:32:57.000000 rapidfuzz-3.1.1/src/rapidfuzz/fuzz_cpp_avx2.cxx
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/src/rapidfuzz/fuzz_cpp_avx2.pyx
--rw-r--r--   0 runner    (1001) docker     (123)    25392 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/src/rapidfuzz/fuzz_py.py
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/src/rapidfuzz/process.py
--rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/src/rapidfuzz/process.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    19686 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/src/rapidfuzz/process_cpp.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/src/rapidfuzz/process_cpp.py
--rw-r--r--   0 runner    (1001) docker     (123)  1764130 2023-06-06 12:32:59.000000 rapidfuzz-3.1.1/src/rapidfuzz/process_cpp_impl.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/src/rapidfuzz/process_cpp_impl.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    56366 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/src/rapidfuzz/process_cpp_impl.pyx
--rw-r--r--   0 runner    (1001) docker     (123)    25632 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/src/rapidfuzz/process_py.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/src/rapidfuzz/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     6696 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/src/rapidfuzz/rapidfuzz.h
--rw-r--r--   0 runner    (1001) docker     (123)   293266 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/src/rapidfuzz/unicodetype_db.h
--rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/src/rapidfuzz/utils.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/src/rapidfuzz/utils.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/src/rapidfuzz/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/src/rapidfuzz/utils.pyi
--rw-r--r--   0 runner    (1001) docker     (123)   452279 2023-06-06 12:33:00.000000 rapidfuzz-3.1.1/src/rapidfuzz/utils_cpp.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/src/rapidfuzz/utils_cpp.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/src/rapidfuzz/utils_cpp.pyx
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/src/rapidfuzz/utils_py.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:33:19.053034 rapidfuzz-3.1.1/src/rapidfuzz.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11268 2023-06-06 12:33:18.000000 rapidfuzz-3.1.1/src/rapidfuzz.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9320 2023-06-06 12:33:18.000000 rapidfuzz-3.1.1/src/rapidfuzz.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 12:33:18.000000 rapidfuzz-3.1.1/src/rapidfuzz.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-06 12:33:18.000000 rapidfuzz-3.1.1/src/rapidfuzz.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-06 12:33:18.000000 rapidfuzz-3.1.1/src/rapidfuzz.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-06 12:33:18.000000 rapidfuzz-3.1.1/src/rapidfuzz.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:33:19.077034 rapidfuzz-3.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11904 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/tests/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:33:19.081034 rapidfuzz-3.1.1/tests/distance/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/tests/distance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4569 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/tests/distance/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/tests/distance/test_DamerauLevenshtein.py
--rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/tests/distance/test_Hamming.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/tests/distance/test_Indel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/tests/distance/test_Jaro.py
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/tests/distance/test_JaroWinkler.py
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/tests/distance/test_LCSseq.py
--rw-r--r--   0 runner    (1001) docker     (123)     4364 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/tests/distance/test_Levenshtein.py
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/tests/distance/test_OSA.py
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/tests/distance/test_Postfix.py
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/tests/distance/test_Prefix.py
--rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/tests/distance/test_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)    10165 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/tests/distance/test_init.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/tests/test_cpp_fallback.py
--rw-r--r--   0 runner    (1001) docker     (123)    12817 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/tests/test_fuzz.py
--rw-r--r--   0 runner    (1001) docker     (123)    14360 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/tests/test_hypothesis.py
--rw-r--r--   0 runner    (1001) docker     (123)    13749 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/tests/test_process.py
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/tests/test_pure_python_fallback.py
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-06-06 12:32:25.000000 rapidfuzz-3.1.1/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:25:12.591378 rapidfuzz-3.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    28449 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11468 2023-07-20 21:25:12.591378 rapidfuzz-3.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10800 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:25:12.511378 rapidfuzz-3.1.2/_custom_build/
+-rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/_custom_build/backend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:25:12.511378 rapidfuzz-3.1.2/cmake/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/cmake/CheckCPUArch.c.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/cmake/CheckCPUArch.cmake
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:25:12.511378 rapidfuzz-3.1.2/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:25:12.511378 rapidfuzz-3.1.2/docs/Contributing/
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/docs/Contributing/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/docs/Installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/docs/License.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/docs/References.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:25:12.511378 rapidfuzz-3.1.2/docs/Usage/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:25:12.515378 rapidfuzz-3.1.2/docs/Usage/distance/
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/docs/Usage/distance/DamerauLevenshtein.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/docs/Usage/distance/Hamming.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/docs/Usage/distance/Indel.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/docs/Usage/distance/Jaro.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/docs/Usage/distance/JaroWinkler.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/docs/Usage/distance/Levenshtein.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/docs/Usage/distance/OSA.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/docs/Usage/distance/Postfix.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/docs/Usage/distance/Prefix.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:25:12.515378 rapidfuzz-3.1.2/docs/Usage/distance/img/
+-rw-r--r--   0 runner    (1001) docker     (123)    37487 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/docs/Usage/distance/img/damerau_levenshtein.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    42028 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/docs/Usage/distance/img/indel_levenshtein.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    34090 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/docs/Usage/distance/img/jaro.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    34913 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/docs/Usage/distance/img/jaro_winkler.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    37821 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/docs/Usage/distance/img/osa.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    32664 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/docs/Usage/distance/img/uniform_levenshtein.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/docs/Usage/distance/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/docs/Usage/fuzz.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:25:12.519378 rapidfuzz-3.1.2/docs/Usage/img/
+-rw-r--r--   0 runner    (1001) docker     (123)    25251 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/docs/Usage/img/WRatio.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    42028 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/docs/Usage/img/indel_levenshtein.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    41626 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/docs/Usage/img/partial_ratio_long_needle.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    41360 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/docs/Usage/img/partial_ratio_short_needle.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    28491 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/docs/Usage/img/partial_token_ratio.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    24769 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/docs/Usage/img/partial_token_set_ratio.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    25404 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/docs/Usage/img/partial_token_sort_ratio.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    24367 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/docs/Usage/img/ratio.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    27273 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/docs/Usage/img/token_ratio.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    25693 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/docs/Usage/img/token_set_ratio.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    26611 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/docs/Usage/img/token_sort_ratio.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    32664 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/docs/Usage/img/uniform_levenshtein.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/docs/Usage/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/docs/Usage/process.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/docs/Usage/utils.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/docs/changelog_link.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:25:12.519378 rapidfuzz-3.1.2/docs/img/
+-rw-r--r--   0 runner    (1001) docker     (123)     5879 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/docs/img/RapidFuzz.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    56024 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/docs/img/cdist.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    54183 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/docs/img/scorer.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3160 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/docs/refs.bib
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:25:12.507378 rapidfuzz-3.1.2/extern/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:25:12.519378 rapidfuzz-3.1.2/extern/rapidfuzz-cpp/
+-rw-r--r--   0 runner    (1001) docker     (123)     4397 2023-07-20 21:24:26.000000 rapidfuzz-3.1.2/extern/rapidfuzz-cpp/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-20 21:24:26.000000 rapidfuzz-3.1.2/extern/rapidfuzz-cpp/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:25:12.519378 rapidfuzz-3.1.2/extern/rapidfuzz-cpp/rapidfuzz/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:25:12.523378 rapidfuzz-3.1.2/extern/rapidfuzz-cpp/rapidfuzz/details/
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-07-20 21:24:26.000000 rapidfuzz-3.1.2/extern/rapidfuzz-cpp/rapidfuzz/details/CharSet.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4861 2023-07-20 21:24:26.000000 rapidfuzz-3.1.2/extern/rapidfuzz-cpp/rapidfuzz/details/GrowingHashmap.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4622 2023-07-20 21:24:26.000000 rapidfuzz-3.1.2/extern/rapidfuzz-cpp/rapidfuzz/details/Matrix.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5592 2023-07-20 21:24:26.000000 rapidfuzz-3.1.2/extern/rapidfuzz-cpp/rapidfuzz/details/PatternMatchVector.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-07-20 21:24:26.000000 rapidfuzz-3.1.2/extern/rapidfuzz-cpp/rapidfuzz/details/Range.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-07-20 21:24:26.000000 rapidfuzz-3.1.2/extern/rapidfuzz-cpp/rapidfuzz/details/SplittedSentenceView.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-07-20 21:24:26.000000 rapidfuzz-3.1.2/extern/rapidfuzz-cpp/rapidfuzz/details/common.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4345 2023-07-20 21:24:26.000000 rapidfuzz-3.1.2/extern/rapidfuzz-cpp/rapidfuzz/details/common_impl.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    23057 2023-07-20 21:24:26.000000 rapidfuzz-3.1.2/extern/rapidfuzz-cpp/rapidfuzz/details/distance.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4992 2023-07-20 21:24:26.000000 rapidfuzz-3.1.2/extern/rapidfuzz-cpp/rapidfuzz/details/intrinsics.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-20 21:24:26.000000 rapidfuzz-3.1.2/extern/rapidfuzz-cpp/rapidfuzz/details/simd.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10815 2023-07-20 21:24:26.000000 rapidfuzz-3.1.2/extern/rapidfuzz-cpp/rapidfuzz/details/simd_avx2.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11538 2023-07-20 21:24:26.000000 rapidfuzz-3.1.2/extern/rapidfuzz-cpp/rapidfuzz/details/simd_sse2.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-07-20 21:24:26.000000 rapidfuzz-3.1.2/extern/rapidfuzz-cpp/rapidfuzz/details/type_traits.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    17508 2023-07-20 21:24:26.000000 rapidfuzz-3.1.2/extern/rapidfuzz-cpp/rapidfuzz/details/types.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:25:12.531378 rapidfuzz-3.1.2/extern/rapidfuzz-cpp/rapidfuzz/distance/
+-rw-r--r--   0 runner    (1001) docker     (123)     6231 2023-07-20 21:24:26.000000 rapidfuzz-3.1.2/extern/rapidfuzz-cpp/rapidfuzz/distance/DamerauLevenshtein.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-07-20 21:24:26.000000 rapidfuzz-3.1.2/extern/rapidfuzz-cpp/rapidfuzz/distance/DamerauLevenshtein_impl.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6734 2023-07-20 21:24:26.000000 rapidfuzz-3.1.2/extern/rapidfuzz-cpp/rapidfuzz/distance/Hamming.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-07-20 21:24:26.000000 rapidfuzz-3.1.2/extern/rapidfuzz-cpp/rapidfuzz/distance/Hamming_impl.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6493 2023-07-20 21:24:26.000000 rapidfuzz-3.1.2/extern/rapidfuzz-cpp/rapidfuzz/distance/Indel.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-07-20 21:24:26.000000 rapidfuzz-3.1.2/extern/rapidfuzz-cpp/rapidfuzz/distance/Indel_impl.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3603 2023-07-20 21:24:26.000000 rapidfuzz-3.1.2/extern/rapidfuzz-cpp/rapidfuzz/distance/Jaro.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5047 2023-07-20 21:24:26.000000 rapidfuzz-3.1.2/extern/rapidfuzz-cpp/rapidfuzz/distance/JaroWinkler.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-07-20 21:24:26.000000 rapidfuzz-3.1.2/extern/rapidfuzz-cpp/rapidfuzz/distance/JaroWinkler_impl.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    14569 2023-07-20 21:24:26.000000 rapidfuzz-3.1.2/extern/rapidfuzz-cpp/rapidfuzz/distance/Jaro_impl.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8228 2023-07-20 21:24:26.000000 rapidfuzz-3.1.2/extern/rapidfuzz-cpp/rapidfuzz/distance/LCSseq.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    14461 2023-07-20 21:24:26.000000 rapidfuzz-3.1.2/extern/rapidfuzz-cpp/rapidfuzz/distance/LCSseq_impl.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    20759 2023-07-20 21:24:26.000000 rapidfuzz-3.1.2/extern/rapidfuzz-cpp/rapidfuzz/distance/Levenshtein.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    44317 2023-07-20 21:24:26.000000 rapidfuzz-3.1.2/extern/rapidfuzz-cpp/rapidfuzz/distance/Levenshtein_impl.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9648 2023-07-20 21:24:26.000000 rapidfuzz-3.1.2/extern/rapidfuzz-cpp/rapidfuzz/distance/OSA.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9729 2023-07-20 21:24:26.000000 rapidfuzz-3.1.2/extern/rapidfuzz-cpp/rapidfuzz/distance/OSA_impl.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-07-20 21:24:26.000000 rapidfuzz-3.1.2/extern/rapidfuzz-cpp/rapidfuzz/distance/Postfix.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-07-20 21:24:26.000000 rapidfuzz-3.1.2/extern/rapidfuzz-cpp/rapidfuzz/distance/Postfix_impl.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3931 2023-07-20 21:24:26.000000 rapidfuzz-3.1.2/extern/rapidfuzz-cpp/rapidfuzz/distance/Prefix.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-07-20 21:24:26.000000 rapidfuzz-3.1.2/extern/rapidfuzz-cpp/rapidfuzz/distance/Prefix_impl.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3833 2023-07-20 21:24:26.000000 rapidfuzz-3.1.2/extern/rapidfuzz-cpp/rapidfuzz/distance.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    27750 2023-07-20 21:24:26.000000 rapidfuzz-3.1.2/extern/rapidfuzz-cpp/rapidfuzz/fuzz.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    37923 2023-07-20 21:24:26.000000 rapidfuzz-3.1.2/extern/rapidfuzz-cpp/rapidfuzz/fuzz.impl
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-20 21:24:26.000000 rapidfuzz-3.1.2/extern/rapidfuzz-cpp/rapidfuzz/rapidfuzz_all.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:25:12.531378 rapidfuzz-3.1.2/extern/taskflow/
+-rw-r--r--   0 runner    (1001) docker     (123)    14095 2023-07-20 21:24:28.000000 rapidfuzz-3.1.2/extern/taskflow/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-07-20 21:24:28.000000 rapidfuzz-3.1.2/extern/taskflow/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-20 21:24:28.000000 rapidfuzz-3.1.2/extern/taskflow/TaskflowConfig.cmake.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:25:12.531378 rapidfuzz-3.1.2/extern/taskflow/taskflow/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:25:12.535378 rapidfuzz-3.1.2/extern/taskflow/taskflow/algorithm/
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-07-20 21:24:29.000000 rapidfuzz-3.1.2/extern/taskflow/taskflow/algorithm/critical.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    16653 2023-07-20 21:24:29.000000 rapidfuzz-3.1.2/extern/taskflow/taskflow/algorithm/data_pipeline.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    14972 2023-07-20 21:24:29.000000 rapidfuzz-3.1.2/extern/taskflow/taskflow/algorithm/find.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4928 2023-07-20 21:24:29.000000 rapidfuzz-3.1.2/extern/taskflow/taskflow/algorithm/for_each.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-07-20 21:24:29.000000 rapidfuzz-3.1.2/extern/taskflow/taskflow/algorithm/launch.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    14524 2023-07-20 21:24:29.000000 rapidfuzz-3.1.2/extern/taskflow/taskflow/algorithm/partitioner.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    44892 2023-07-20 21:24:29.000000 rapidfuzz-3.1.2/extern/taskflow/taskflow/algorithm/pipeline.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7902 2023-07-20 21:24:29.000000 rapidfuzz-3.1.2/extern/taskflow/taskflow/algorithm/reduce.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    17090 2023-07-20 21:24:29.000000 rapidfuzz-3.1.2/extern/taskflow/taskflow/algorithm/scan.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    20947 2023-07-20 21:24:29.000000 rapidfuzz-3.1.2/extern/taskflow/taskflow/algorithm/sort.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5870 2023-07-20 21:24:29.000000 rapidfuzz-3.1.2/extern/taskflow/taskflow/algorithm/transform.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:25:12.539378 rapidfuzz-3.1.2/extern/taskflow/taskflow/core/
+-rw-r--r--   0 runner    (1001) docker     (123)    10955 2023-07-20 21:24:29.000000 rapidfuzz-3.1.2/extern/taskflow/taskflow/core/async.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-07-20 21:24:29.000000 rapidfuzz-3.1.2/extern/taskflow/taskflow/core/async_task.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-07-20 21:24:29.000000 rapidfuzz-3.1.2/extern/taskflow/taskflow/core/declarations.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-20 21:24:29.000000 rapidfuzz-3.1.2/extern/taskflow/taskflow/core/environment.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-07-20 21:24:29.000000 rapidfuzz-3.1.2/extern/taskflow/taskflow/core/error.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    54781 2023-07-20 21:24:29.000000 rapidfuzz-3.1.2/extern/taskflow/taskflow/core/executor-module-opt.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    66789 2023-07-20 21:24:29.000000 rapidfuzz-3.1.2/extern/taskflow/taskflow/core/executor.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    41751 2023-07-20 21:24:29.000000 rapidfuzz-3.1.2/extern/taskflow/taskflow/core/flow_builder.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    24153 2023-07-20 21:24:29.000000 rapidfuzz-3.1.2/extern/taskflow/taskflow/core/graph.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9176 2023-07-20 21:24:29.000000 rapidfuzz-3.1.2/extern/taskflow/taskflow/core/notifier.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    26126 2023-07-20 21:24:29.000000 rapidfuzz-3.1.2/extern/taskflow/taskflow/core/observer.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-07-20 21:24:29.000000 rapidfuzz-3.1.2/extern/taskflow/taskflow/core/semaphore.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    18519 2023-07-20 21:24:29.000000 rapidfuzz-3.1.2/extern/taskflow/taskflow/core/task.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    15758 2023-07-20 21:24:29.000000 rapidfuzz-3.1.2/extern/taskflow/taskflow/core/taskflow.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-20 21:24:29.000000 rapidfuzz-3.1.2/extern/taskflow/taskflow/core/topology.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    12210 2023-07-20 21:24:29.000000 rapidfuzz-3.1.2/extern/taskflow/taskflow/core/tsq.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-07-20 21:24:29.000000 rapidfuzz-3.1.2/extern/taskflow/taskflow/core/worker.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-07-20 21:24:29.000000 rapidfuzz-3.1.2/extern/taskflow/taskflow/taskflow.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:25:12.543378 rapidfuzz-3.1.2/extern/taskflow/taskflow/utility/
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-07-20 21:24:29.000000 rapidfuzz-3.1.2/extern/taskflow/taskflow/utility/iterator.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-07-20 21:24:29.000000 rapidfuzz-3.1.2/extern/taskflow/taskflow/utility/macros.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-07-20 21:24:29.000000 rapidfuzz-3.1.2/extern/taskflow/taskflow/utility/math.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    19899 2023-07-20 21:24:29.000000 rapidfuzz-3.1.2/extern/taskflow/taskflow/utility/object_pool.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-07-20 21:24:29.000000 rapidfuzz-3.1.2/extern/taskflow/taskflow/utility/os.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    29321 2023-07-20 21:24:29.000000 rapidfuzz-3.1.2/extern/taskflow/taskflow/utility/serializer.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-07-20 21:24:29.000000 rapidfuzz-3.1.2/extern/taskflow/taskflow/utility/singleton.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    31329 2023-07-20 21:24:29.000000 rapidfuzz-3.1.2/extern/taskflow/taskflow/utility/small_vector.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-20 21:24:29.000000 rapidfuzz-3.1.2/extern/taskflow/taskflow/utility/stream.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8631 2023-07-20 21:24:29.000000 rapidfuzz-3.1.2/extern/taskflow/taskflow/utility/traits.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5685 2023-07-20 21:24:29.000000 rapidfuzz-3.1.2/extern/taskflow/taskflow/utility/uuid.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-07-20 21:25:01.000000 rapidfuzz-3.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 21:25:12.591378 rapidfuzz-3.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:25:12.507378 rapidfuzz-3.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:25:12.559378 rapidfuzz-3.1.2/src/rapidfuzz/
+-rw-r--r--   0 runner    (1001) docker     (123)     5251 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/src/rapidfuzz/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:25:12.563378 rapidfuzz-3.1.2/src/rapidfuzz/FeatureDetector/
+-rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/src/rapidfuzz/FeatureDetector/CpuInfo.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/src/rapidfuzz/FeatureDetector/CpuInfo.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/src/rapidfuzz/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/src/rapidfuzz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/src/rapidfuzz/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:25:12.563378 rapidfuzz-3.1.2/src/rapidfuzz/__pyinstaller/
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/src/rapidfuzz/__pyinstaller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/src/rapidfuzz/__pyinstaller/hook-rapidfuzz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/src/rapidfuzz/__pyinstaller/test_rapidfuzz_packaging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/src/rapidfuzz/_common_py.py
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/src/rapidfuzz/_feature_detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)   246066 2023-07-20 21:24:57.000000 rapidfuzz-3.1.2/src/rapidfuzz/_feature_detector_cpp.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/src/rapidfuzz/_feature_detector_cpp.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     3627 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/src/rapidfuzz/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25512 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/src/rapidfuzz/cpp_common.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    15706 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/src/rapidfuzz/cpp_common.pxd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:25:12.583378 rapidfuzz-3.1.2/src/rapidfuzz/distance/
+-rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/src/rapidfuzz/distance/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/src/rapidfuzz/distance/DamerauLevenshtein.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/src/rapidfuzz/distance/DamerauLevenshtein.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7090 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/src/rapidfuzz/distance/DamerauLevenshtein_py.py
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/src/rapidfuzz/distance/Hamming.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/src/rapidfuzz/distance/Hamming.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9757 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/src/rapidfuzz/distance/Hamming_py.py
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/src/rapidfuzz/distance/Indel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/src/rapidfuzz/distance/Indel.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10934 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/src/rapidfuzz/distance/Indel_py.py
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/src/rapidfuzz/distance/Jaro.py
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/src/rapidfuzz/distance/Jaro.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/src/rapidfuzz/distance/JaroWinkler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/src/rapidfuzz/distance/JaroWinkler.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6781 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/src/rapidfuzz/distance/JaroWinkler_py.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7960 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/src/rapidfuzz/distance/Jaro_py.py
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/src/rapidfuzz/distance/LCSseq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/src/rapidfuzz/distance/LCSseq.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10290 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/src/rapidfuzz/distance/LCSseq_py.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/src/rapidfuzz/distance/Levenshtein.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/src/rapidfuzz/distance/Levenshtein.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15750 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/src/rapidfuzz/distance/Levenshtein_py.py
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/src/rapidfuzz/distance/OSA.py
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/src/rapidfuzz/distance/OSA.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6748 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/src/rapidfuzz/distance/OSA_py.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/src/rapidfuzz/distance/Postfix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5468 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/src/rapidfuzz/distance/Postfix_py.py
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/src/rapidfuzz/distance/Prefix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5444 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/src/rapidfuzz/distance/Prefix_py.py
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/src/rapidfuzz/distance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/src/rapidfuzz/distance/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/src/rapidfuzz/distance/_initialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/src/rapidfuzz/distance/_initialize.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)  1620875 2023-07-20 21:24:58.000000 rapidfuzz-3.1.2/src/rapidfuzz/distance/_initialize_cpp.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/src/rapidfuzz/distance/_initialize_cpp.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    29674 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/src/rapidfuzz/distance/_initialize_cpp.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)    28423 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/src/rapidfuzz/distance/_initialize_py.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29777 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/src/rapidfuzz/distance/metrics.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)  1392045 2023-07-20 21:25:00.000000 rapidfuzz-3.1.2/src/rapidfuzz/distance/metrics_cpp.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     7051 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/src/rapidfuzz/distance/metrics_cpp.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    57041 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/src/rapidfuzz/distance/metrics_cpp.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)  1400394 2023-07-20 21:25:01.000000 rapidfuzz-3.1.2/src/rapidfuzz/distance/metrics_cpp_avx2.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/src/rapidfuzz/distance/metrics_cpp_avx2.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)    10618 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/src/rapidfuzz/distance/metrics_py.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/src/rapidfuzz/fuzz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/src/rapidfuzz/fuzz.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)   608925 2023-07-20 21:24:52.000000 rapidfuzz-3.1.2/src/rapidfuzz/fuzz_cpp.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     5876 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/src/rapidfuzz/fuzz_cpp.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10319 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/src/rapidfuzz/fuzz_cpp.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)   610918 2023-07-20 21:24:53.000000 rapidfuzz-3.1.2/src/rapidfuzz/fuzz_cpp_avx2.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/src/rapidfuzz/fuzz_cpp_avx2.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)    25392 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/src/rapidfuzz/fuzz_py.py
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/src/rapidfuzz/process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/src/rapidfuzz/process.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    19686 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/src/rapidfuzz/process_cpp.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/src/rapidfuzz/process_cpp.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1764744 2023-07-20 21:24:55.000000 rapidfuzz-3.1.2/src/rapidfuzz/process_cpp_impl.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/src/rapidfuzz/process_cpp_impl.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    56366 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/src/rapidfuzz/process_cpp_impl.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)    25632 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/src/rapidfuzz/process_py.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/src/rapidfuzz/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     6696 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/src/rapidfuzz/rapidfuzz.h
+-rw-r--r--   0 runner    (1001) docker     (123)   293266 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/src/rapidfuzz/unicodetype_db.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/src/rapidfuzz/utils.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/src/rapidfuzz/utils.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/src/rapidfuzz/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/src/rapidfuzz/utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)   452778 2023-07-20 21:24:56.000000 rapidfuzz-3.1.2/src/rapidfuzz/utils_cpp.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/src/rapidfuzz/utils_cpp.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/src/rapidfuzz/utils_cpp.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/src/rapidfuzz/utils_py.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:25:12.559378 rapidfuzz-3.1.2/src/rapidfuzz.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11468 2023-07-20 21:25:12.000000 rapidfuzz-3.1.2/src/rapidfuzz.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9320 2023-07-20 21:25:12.000000 rapidfuzz-3.1.2/src/rapidfuzz.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 21:25:12.000000 rapidfuzz-3.1.2/src/rapidfuzz.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-20 21:25:12.000000 rapidfuzz-3.1.2/src/rapidfuzz.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-20 21:25:12.000000 rapidfuzz-3.1.2/src/rapidfuzz.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-20 21:25:12.000000 rapidfuzz-3.1.2/src/rapidfuzz.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:25:12.587378 rapidfuzz-3.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11904 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/tests/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:25:12.591378 rapidfuzz-3.1.2/tests/distance/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/tests/distance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4569 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/tests/distance/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/tests/distance/test_DamerauLevenshtein.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/tests/distance/test_Hamming.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/tests/distance/test_Indel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/tests/distance/test_Jaro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/tests/distance/test_JaroWinkler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/tests/distance/test_LCSseq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4364 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/tests/distance/test_Levenshtein.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/tests/distance/test_OSA.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/tests/distance/test_Postfix.py
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/tests/distance/test_Prefix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/tests/distance/test_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10165 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/tests/distance/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/tests/test_cpp_fallback.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12817 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/tests/test_fuzz.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14360 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/tests/test_hypothesis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13749 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/tests/test_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/tests/test_pure_python_fallback.py
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-07-20 21:24:22.000000 rapidfuzz-3.1.2/tests/test_utils.py
```

### Comparing `rapidfuzz-3.1.1/CHANGELOG.rst` & `rapidfuzz-3.1.2/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 Changelog
 ---------
 
+[3.1.2] - 2023-07-19
+^^^^^^^^^^^^^^^^^^^^
+Changed
+~~~~~~~
+- upgrade to ``Cython==3.0.0``
+
 [3.1.1] - 2023-06-06
 ^^^^^^^^^^^^^^^^^^^^
 Changed
 ~~~~~~~
 - upgrade to ``taskflow==3.6``
 
 Fixed
@@ -30,18 +36,22 @@
 ^^^^^^^^^^^^^^^^^^^^
 Changed
 ~~~~~~~
 - allow the usage of ``Hamming`` for different string lengths. Length differences are handled as
   insertions / deletions
 - remove support for boolean preprocessor functions in ``rapidfuzz.fuzz`` and ``rapidfuzz.process``.
   The processor argument is now always a callable or None.
-- update defaults of the processor argument to be ``None`` everywhere. This changes the defaults of some of
-  the functions in ``rapidfuzz.fuzz`` and ``rapidfuzz.process``.
-- ``rapidfuzz.process`` no longer calls scorers with ``processor=None``. For this reason scorer functions
-  do not need to provide this argument anymore.
+- update defaults of the processor argument to be ``None`` everywhere. For affected functions this can change results, since strings are no longer preprocessed.
+  To get back the old behaviour pass ``processor=utils.default_process`` to these functions.
+  The following functions are affected by this:
+
+  - ``process.extract``, ``process.extract_iter``, ``process.extractOne``
+  - ``fuzz.token_sort_ratio``, ``fuzz.token_set_ratio``, ``fuzz.token_ratio``, ``fuzz.partial_token_sort_ratio``, ``fuzz.partial_token_set_ratio``, ``fuzz.partial_token_ratio``, ``fuzz.WRatio``, ``fuzz.QRatio``
+
+- ``rapidfuzz.process`` no longer calls scorers with ``processor=None``. For this reason user provided scorers no longer require this argument.
 - remove option to pass keyword arguments to scorer via ``**kwargs`` in ``rapidfuzz.process``. They can be passed
   via a ``scorer_kwargs`` argument now. This ensures this does not break when extending function parameters and
   prevents naming clashes.
 - remove ``rapidfuzz.string_metric`` module. Replacements for all functions are available in ``rapidfuzz.distance``
 
 Added
 ~~~~~
```

### Comparing `rapidfuzz-3.1.1/CMakeLists.txt` & `rapidfuzz-3.1.2/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/LICENSE` & `rapidfuzz-3.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/MANIFEST.in` & `rapidfuzz-3.1.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/PKG-INFO` & `rapidfuzz-3.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rapidfuzz
-Version: 3.1.1
+Version: 3.1.2
 Summary: rapid fuzzy string matching
 Home-page: https://github.com/maxbachmann/RapidFuzz
 Author: Max Bachmann
 Author-email: pypi@maxbachmann.de
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
@@ -61,14 +61,15 @@
 
 ## Description
 RapidFuzz is a fast string matching library for Python and C++, which is using the string similarity calculations from [FuzzyWuzzy](https://github.com/seatgeek/fuzzywuzzy). However there are a couple of aspects that set RapidFuzz apart from FuzzyWuzzy:
 1) It is MIT licensed so it can be used whichever License you might want to choose for your project, while you're forced to adopt the GPL license when using FuzzyWuzzy
 2) It provides many string_metrics like hamming or jaro_winkler, which are not included in FuzzyWuzzy
 3) It is mostly written in C++ and on top of this comes with a lot of Algorithmic improvements to make string matching even faster, while still providing the same results. For detailed benchmarks check the [documentation](https://maxbachmann.github.io/RapidFuzz)
 4) Fixes multiple bugs in the `partial_ratio` implementation
+5) It can be largely used as a drop in replacement for `fuzzywuzzy`. However there are a couple API differences described [here](https://github.com/maxbachmann/RapidFuzz/blob/main/api_differences.md)
 
 ## Requirements
 
 - Python 3.7 or later
 - On Windows the [Visual C++ 2019 redistributable](https://support.microsoft.com/en-us/help/2977003/the-latest-supported-visual-c-downloads) is required
 
 ## Installation
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: rapidfuzz Version: 3.1.1 Summary: rapid fuzzy
+Metadata-Version: 2.1 Name: rapidfuzz Version: 3.1.2 Summary: rapid fuzzy
 string matching Home-page: https://github.com/maxbachmann/RapidFuzz Author: Max
 Bachmann Author-email: pypi@maxbachmann.de License: MIT Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: License :: OSI
 Approved :: MIT License Requires-Python: >=3.7 Description-Content-Type: text/
@@ -21,27 +21,30 @@
 whichever License you might want to choose for your project, while you're
 forced to adopt the GPL license when using FuzzyWuzzy 2) It provides many
 string_metrics like hamming or jaro_winkler, which are not included in
 FuzzyWuzzy 3) It is mostly written in C++ and on top of this comes with a lot
 of Algorithmic improvements to make string matching even faster, while still
 providing the same results. For detailed benchmarks check the [documentation]
 (https://maxbachmann.github.io/RapidFuzz) 4) Fixes multiple bugs in the
-`partial_ratio` implementation ## Requirements - Python 3.7 or later - On
-Windows the [Visual C++ 2019 redistributable](https://support.microsoft.com/en-
-us/help/2977003/the-latest-supported-visual-c-downloads) is required ##
-Installation There are several ways to install RapidFuzz, the recommended
-methods are to either use `pip`(the Python package manager) or `conda` (an
-open-source, cross-platform, package manager) ### with pip RapidFuzz can be
-installed with `pip` the following way: ```bash pip install rapidfuzz ``` There
-are pre-built binaries (wheels) of RapidFuzz for MacOS (10.9 and later), Linux
-x86_64 and Windows. Wheels for armv6l (Raspberry Pi Zero) and armv7l (Raspberry
-Pi) are available on [piwheels](https://www.piwheels.org/project/rapidfuzz/). >
-:heavy_multiplication_x:   **failure "ImportError: DLL load failed"** > > If
-you run into this error on Windows the reason is most likely, that the [Visual
-C++ 2019 redistributable](https://support.microsoft.com/en-us/help/2977003/the-
+`partial_ratio` implementation 5) It can be largely used as a drop in
+replacement for `fuzzywuzzy`. However there are a couple API differences
+described [here](https://github.com/maxbachmann/RapidFuzz/blob/main/
+api_differences.md) ## Requirements - Python 3.7 or later - On Windows the
+[Visual C++ 2019 redistributable](https://support.microsoft.com/en-us/help/
+2977003/the-latest-supported-visual-c-downloads) is required ## Installation
+There are several ways to install RapidFuzz, the recommended methods are to
+either use `pip`(the Python package manager) or `conda` (an open-source, cross-
+platform, package manager) ### with pip RapidFuzz can be installed with `pip`
+the following way: ```bash pip install rapidfuzz ``` There are pre-built
+binaries (wheels) of RapidFuzz for MacOS (10.9 and later), Linux x86_64 and
+Windows. Wheels for armv6l (Raspberry Pi Zero) and armv7l (Raspberry Pi) are
+available on [piwheels](https://www.piwheels.org/project/rapidfuzz/). > :
+heavy_multiplication_x:   **failure "ImportError: DLL load failed"** > > If you
+run into this error on Windows the reason is most likely, that the [Visual C++
+2019 redistributable](https://support.microsoft.com/en-us/help/2977003/the-
 latest-supported-visual-c-downloads) is not installed, which is required to
 find C++ Libraries (The C++ 2019 version includes the 2015, 2017 and 2019
 version). ### with conda RapidFuzz can be installed with `conda`: ```bash conda
 install -c conda-forge rapidfuzz ``` ### from git RapidFuzz can be installed
 directly from the source distribution by cloning the repository. This requires
 a C++17 capable compiler. ```bash git clone --recursive https://github.com/
 maxbachmann/rapidfuzz.git cd rapidfuzz pip install . ``` ## Usage Some simple
```

### Comparing `rapidfuzz-3.1.1/README.md` & `rapidfuzz-3.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -41,14 +41,15 @@
 
 ## Description
 RapidFuzz is a fast string matching library for Python and C++, which is using the string similarity calculations from [FuzzyWuzzy](https://github.com/seatgeek/fuzzywuzzy). However there are a couple of aspects that set RapidFuzz apart from FuzzyWuzzy:
 1) It is MIT licensed so it can be used whichever License you might want to choose for your project, while you're forced to adopt the GPL license when using FuzzyWuzzy
 2) It provides many string_metrics like hamming or jaro_winkler, which are not included in FuzzyWuzzy
 3) It is mostly written in C++ and on top of this comes with a lot of Algorithmic improvements to make string matching even faster, while still providing the same results. For detailed benchmarks check the [documentation](https://maxbachmann.github.io/RapidFuzz)
 4) Fixes multiple bugs in the `partial_ratio` implementation
+5) It can be largely used as a drop in replacement for `fuzzywuzzy`. However there are a couple API differences described [here](https://github.com/maxbachmann/RapidFuzz/blob/main/api_differences.md)
 
 ## Requirements
 
 - Python 3.7 or later
 - On Windows the [Visual C++ 2019 redistributable](https://support.microsoft.com/en-us/help/2977003/the-latest-supported-visual-c-downloads) is required
 
 ## Installation
```

#### html2text {}

```diff
@@ -12,27 +12,30 @@
 whichever License you might want to choose for your project, while you're
 forced to adopt the GPL license when using FuzzyWuzzy 2) It provides many
 string_metrics like hamming or jaro_winkler, which are not included in
 FuzzyWuzzy 3) It is mostly written in C++ and on top of this comes with a lot
 of Algorithmic improvements to make string matching even faster, while still
 providing the same results. For detailed benchmarks check the [documentation]
 (https://maxbachmann.github.io/RapidFuzz) 4) Fixes multiple bugs in the
-`partial_ratio` implementation ## Requirements - Python 3.7 or later - On
-Windows the [Visual C++ 2019 redistributable](https://support.microsoft.com/en-
-us/help/2977003/the-latest-supported-visual-c-downloads) is required ##
-Installation There are several ways to install RapidFuzz, the recommended
-methods are to either use `pip`(the Python package manager) or `conda` (an
-open-source, cross-platform, package manager) ### with pip RapidFuzz can be
-installed with `pip` the following way: ```bash pip install rapidfuzz ``` There
-are pre-built binaries (wheels) of RapidFuzz for MacOS (10.9 and later), Linux
-x86_64 and Windows. Wheels for armv6l (Raspberry Pi Zero) and armv7l (Raspberry
-Pi) are available on [piwheels](https://www.piwheels.org/project/rapidfuzz/). >
-:heavy_multiplication_x:   **failure "ImportError: DLL load failed"** > > If
-you run into this error on Windows the reason is most likely, that the [Visual
-C++ 2019 redistributable](https://support.microsoft.com/en-us/help/2977003/the-
+`partial_ratio` implementation 5) It can be largely used as a drop in
+replacement for `fuzzywuzzy`. However there are a couple API differences
+described [here](https://github.com/maxbachmann/RapidFuzz/blob/main/
+api_differences.md) ## Requirements - Python 3.7 or later - On Windows the
+[Visual C++ 2019 redistributable](https://support.microsoft.com/en-us/help/
+2977003/the-latest-supported-visual-c-downloads) is required ## Installation
+There are several ways to install RapidFuzz, the recommended methods are to
+either use `pip`(the Python package manager) or `conda` (an open-source, cross-
+platform, package manager) ### with pip RapidFuzz can be installed with `pip`
+the following way: ```bash pip install rapidfuzz ``` There are pre-built
+binaries (wheels) of RapidFuzz for MacOS (10.9 and later), Linux x86_64 and
+Windows. Wheels for armv6l (Raspberry Pi Zero) and armv7l (Raspberry Pi) are
+available on [piwheels](https://www.piwheels.org/project/rapidfuzz/). > :
+heavy_multiplication_x:   **failure "ImportError: DLL load failed"** > > If you
+run into this error on Windows the reason is most likely, that the [Visual C++
+2019 redistributable](https://support.microsoft.com/en-us/help/2977003/the-
 latest-supported-visual-c-downloads) is not installed, which is required to
 find C++ Libraries (The C++ 2019 version includes the 2015, 2017 and 2019
 version). ### with conda RapidFuzz can be installed with `conda`: ```bash conda
 install -c conda-forge rapidfuzz ``` ### from git RapidFuzz can be installed
 directly from the source distribution by cloning the repository. This requires
 a C++17 capable compiler. ```bash git clone --recursive https://github.com/
 maxbachmann/rapidfuzz.git cd rapidfuzz pip install . ``` ## Usage Some simple
```

### Comparing `rapidfuzz-3.1.1/_custom_build/backend.py` & `rapidfuzz-3.1.2/_custom_build/backend.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/cmake/CheckCPUArch.cmake` & `rapidfuzz-3.1.2/cmake/CheckCPUArch.cmake`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/docs/Contributing/index.rst` & `rapidfuzz-3.1.2/docs/Contributing/index.rst`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/docs/Installation.rst` & `rapidfuzz-3.1.2/docs/Installation.rst`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/docs/Usage/distance/DamerauLevenshtein.rst` & `rapidfuzz-3.1.2/docs/Usage/distance/DamerauLevenshtein.rst`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/docs/Usage/distance/Indel.rst` & `rapidfuzz-3.1.2/docs/Usage/distance/Indel.rst`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/docs/Usage/distance/Jaro.rst` & `rapidfuzz-3.1.2/docs/Usage/distance/Jaro.rst`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/docs/Usage/distance/JaroWinkler.rst` & `rapidfuzz-3.1.2/docs/Usage/distance/JaroWinkler.rst`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/docs/Usage/distance/Levenshtein.rst` & `rapidfuzz-3.1.2/docs/Usage/distance/Levenshtein.rst`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/docs/Usage/distance/OSA.rst` & `rapidfuzz-3.1.2/docs/Usage/distance/OSA.rst`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/docs/Usage/distance/img/damerau_levenshtein.svg` & `rapidfuzz-3.1.2/docs/Usage/distance/img/damerau_levenshtein.svg`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/docs/Usage/distance/img/indel_levenshtein.svg` & `rapidfuzz-3.1.2/docs/Usage/distance/img/indel_levenshtein.svg`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/docs/Usage/distance/img/jaro.svg` & `rapidfuzz-3.1.2/docs/Usage/distance/img/jaro.svg`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/docs/Usage/distance/img/jaro_winkler.svg` & `rapidfuzz-3.1.2/docs/Usage/distance/img/jaro_winkler.svg`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/docs/Usage/distance/img/osa.svg` & `rapidfuzz-3.1.2/docs/Usage/distance/img/osa.svg`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/docs/Usage/distance/img/uniform_levenshtein.svg` & `rapidfuzz-3.1.2/docs/Usage/distance/img/uniform_levenshtein.svg`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/docs/Usage/fuzz.rst` & `rapidfuzz-3.1.2/docs/Usage/fuzz.rst`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/docs/Usage/img/WRatio.svg` & `rapidfuzz-3.1.2/docs/Usage/img/WRatio.svg`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/docs/Usage/img/indel_levenshtein.svg` & `rapidfuzz-3.1.2/docs/Usage/img/indel_levenshtein.svg`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/docs/Usage/img/partial_ratio_long_needle.svg` & `rapidfuzz-3.1.2/docs/Usage/img/partial_ratio_long_needle.svg`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/docs/Usage/img/partial_ratio_short_needle.svg` & `rapidfuzz-3.1.2/docs/Usage/img/partial_ratio_short_needle.svg`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/docs/Usage/img/partial_token_ratio.svg` & `rapidfuzz-3.1.2/docs/Usage/img/partial_token_ratio.svg`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/docs/Usage/img/partial_token_set_ratio.svg` & `rapidfuzz-3.1.2/docs/Usage/img/partial_token_set_ratio.svg`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/docs/Usage/img/partial_token_sort_ratio.svg` & `rapidfuzz-3.1.2/docs/Usage/img/partial_token_sort_ratio.svg`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/docs/Usage/img/ratio.svg` & `rapidfuzz-3.1.2/docs/Usage/img/ratio.svg`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/docs/Usage/img/token_ratio.svg` & `rapidfuzz-3.1.2/docs/Usage/img/token_ratio.svg`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/docs/Usage/img/token_set_ratio.svg` & `rapidfuzz-3.1.2/docs/Usage/img/token_set_ratio.svg`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/docs/Usage/img/token_sort_ratio.svg` & `rapidfuzz-3.1.2/docs/Usage/img/token_sort_ratio.svg`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/docs/Usage/img/uniform_levenshtein.svg` & `rapidfuzz-3.1.2/docs/Usage/img/uniform_levenshtein.svg`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/docs/conf.py` & `rapidfuzz-3.1.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/docs/img/RapidFuzz.svg` & `rapidfuzz-3.1.2/docs/img/RapidFuzz.svg`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/docs/img/cdist.svg` & `rapidfuzz-3.1.2/docs/img/cdist.svg`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/docs/img/scorer.svg` & `rapidfuzz-3.1.2/docs/img/scorer.svg`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/docs/index.rst` & `rapidfuzz-3.1.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/docs/refs.bib` & `rapidfuzz-3.1.2/docs/refs.bib`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/extern/rapidfuzz-cpp/CMakeLists.txt` & `rapidfuzz-3.1.2/extern/rapidfuzz-cpp/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/extern/rapidfuzz-cpp/LICENSE` & `rapidfuzz-3.1.2/extern/rapidfuzz-cpp/LICENSE`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/extern/rapidfuzz-cpp/rapidfuzz/details/CharSet.hpp` & `rapidfuzz-3.1.2/extern/rapidfuzz-cpp/rapidfuzz/details/CharSet.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/extern/rapidfuzz-cpp/rapidfuzz/details/GrowingHashmap.hpp` & `rapidfuzz-3.1.2/extern/rapidfuzz-cpp/rapidfuzz/details/GrowingHashmap.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/extern/rapidfuzz-cpp/rapidfuzz/details/Matrix.hpp` & `rapidfuzz-3.1.2/extern/rapidfuzz-cpp/rapidfuzz/details/Matrix.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/extern/rapidfuzz-cpp/rapidfuzz/details/PatternMatchVector.hpp` & `rapidfuzz-3.1.2/extern/rapidfuzz-cpp/rapidfuzz/details/PatternMatchVector.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/extern/rapidfuzz-cpp/rapidfuzz/details/Range.hpp` & `rapidfuzz-3.1.2/extern/rapidfuzz-cpp/rapidfuzz/details/Range.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/extern/rapidfuzz-cpp/rapidfuzz/details/SplittedSentenceView.hpp` & `rapidfuzz-3.1.2/extern/rapidfuzz-cpp/rapidfuzz/details/SplittedSentenceView.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/extern/rapidfuzz-cpp/rapidfuzz/details/common.hpp` & `rapidfuzz-3.1.2/extern/rapidfuzz-cpp/rapidfuzz/details/common.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/extern/rapidfuzz-cpp/rapidfuzz/details/common_impl.hpp` & `rapidfuzz-3.1.2/extern/rapidfuzz-cpp/rapidfuzz/details/common_impl.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/extern/rapidfuzz-cpp/rapidfuzz/details/distance.hpp` & `rapidfuzz-3.1.2/extern/rapidfuzz-cpp/rapidfuzz/details/distance.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/extern/rapidfuzz-cpp/rapidfuzz/details/intrinsics.hpp` & `rapidfuzz-3.1.2/extern/rapidfuzz-cpp/rapidfuzz/details/intrinsics.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/extern/rapidfuzz-cpp/rapidfuzz/details/simd.hpp` & `rapidfuzz-3.1.2/extern/rapidfuzz-cpp/rapidfuzz/details/simd.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/extern/rapidfuzz-cpp/rapidfuzz/details/simd_avx2.hpp` & `rapidfuzz-3.1.2/extern/rapidfuzz-cpp/rapidfuzz/details/simd_avx2.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/extern/rapidfuzz-cpp/rapidfuzz/details/simd_sse2.hpp` & `rapidfuzz-3.1.2/extern/rapidfuzz-cpp/rapidfuzz/details/simd_sse2.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/extern/rapidfuzz-cpp/rapidfuzz/details/type_traits.hpp` & `rapidfuzz-3.1.2/extern/rapidfuzz-cpp/rapidfuzz/details/type_traits.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/extern/rapidfuzz-cpp/rapidfuzz/details/types.hpp` & `rapidfuzz-3.1.2/extern/rapidfuzz-cpp/rapidfuzz/details/types.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/extern/rapidfuzz-cpp/rapidfuzz/distance/DamerauLevenshtein.hpp` & `rapidfuzz-3.1.2/extern/rapidfuzz-cpp/rapidfuzz/distance/DamerauLevenshtein.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/extern/rapidfuzz-cpp/rapidfuzz/distance/DamerauLevenshtein_impl.hpp` & `rapidfuzz-3.1.2/extern/rapidfuzz-cpp/rapidfuzz/distance/DamerauLevenshtein_impl.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/extern/rapidfuzz-cpp/rapidfuzz/distance/Hamming.hpp` & `rapidfuzz-3.1.2/extern/rapidfuzz-cpp/rapidfuzz/distance/Hamming.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/extern/rapidfuzz-cpp/rapidfuzz/distance/Hamming_impl.hpp` & `rapidfuzz-3.1.2/extern/rapidfuzz-cpp/rapidfuzz/distance/Hamming_impl.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/extern/rapidfuzz-cpp/rapidfuzz/distance/Indel.hpp` & `rapidfuzz-3.1.2/extern/rapidfuzz-cpp/rapidfuzz/distance/Indel.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/extern/rapidfuzz-cpp/rapidfuzz/distance/Indel_impl.hpp` & `rapidfuzz-3.1.2/extern/rapidfuzz-cpp/rapidfuzz/distance/Indel_impl.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/extern/rapidfuzz-cpp/rapidfuzz/distance/Jaro.hpp` & `rapidfuzz-3.1.2/extern/rapidfuzz-cpp/rapidfuzz/distance/Jaro.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/extern/rapidfuzz-cpp/rapidfuzz/distance/JaroWinkler.hpp` & `rapidfuzz-3.1.2/extern/rapidfuzz-cpp/rapidfuzz/distance/JaroWinkler.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/extern/rapidfuzz-cpp/rapidfuzz/distance/JaroWinkler_impl.hpp` & `rapidfuzz-3.1.2/extern/rapidfuzz-cpp/rapidfuzz/distance/JaroWinkler_impl.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/extern/rapidfuzz-cpp/rapidfuzz/distance/Jaro_impl.hpp` & `rapidfuzz-3.1.2/extern/rapidfuzz-cpp/rapidfuzz/distance/Jaro_impl.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/extern/rapidfuzz-cpp/rapidfuzz/distance/LCSseq.hpp` & `rapidfuzz-3.1.2/extern/rapidfuzz-cpp/rapidfuzz/distance/LCSseq.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/extern/rapidfuzz-cpp/rapidfuzz/distance/LCSseq_impl.hpp` & `rapidfuzz-3.1.2/extern/rapidfuzz-cpp/rapidfuzz/distance/LCSseq_impl.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/extern/rapidfuzz-cpp/rapidfuzz/distance/Levenshtein.hpp` & `rapidfuzz-3.1.2/extern/rapidfuzz-cpp/rapidfuzz/distance/Levenshtein.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/extern/rapidfuzz-cpp/rapidfuzz/distance/Levenshtein_impl.hpp` & `rapidfuzz-3.1.2/extern/rapidfuzz-cpp/rapidfuzz/distance/Levenshtein_impl.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/extern/rapidfuzz-cpp/rapidfuzz/distance/OSA.hpp` & `rapidfuzz-3.1.2/extern/rapidfuzz-cpp/rapidfuzz/distance/OSA.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/extern/rapidfuzz-cpp/rapidfuzz/distance/OSA_impl.hpp` & `rapidfuzz-3.1.2/extern/rapidfuzz-cpp/rapidfuzz/distance/OSA_impl.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/extern/rapidfuzz-cpp/rapidfuzz/distance/Postfix.hpp` & `rapidfuzz-3.1.2/extern/rapidfuzz-cpp/rapidfuzz/distance/Postfix.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/extern/rapidfuzz-cpp/rapidfuzz/distance/Postfix_impl.hpp` & `rapidfuzz-3.1.2/extern/rapidfuzz-cpp/rapidfuzz/distance/Postfix_impl.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/extern/rapidfuzz-cpp/rapidfuzz/distance/Prefix.hpp` & `rapidfuzz-3.1.2/extern/rapidfuzz-cpp/rapidfuzz/distance/Prefix.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/extern/rapidfuzz-cpp/rapidfuzz/distance/Prefix_impl.hpp` & `rapidfuzz-3.1.2/extern/rapidfuzz-cpp/rapidfuzz/distance/Prefix_impl.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/extern/rapidfuzz-cpp/rapidfuzz/distance.hpp` & `rapidfuzz-3.1.2/extern/rapidfuzz-cpp/rapidfuzz/distance.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/extern/rapidfuzz-cpp/rapidfuzz/fuzz.hpp` & `rapidfuzz-3.1.2/extern/rapidfuzz-cpp/rapidfuzz/fuzz.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/extern/rapidfuzz-cpp/rapidfuzz/fuzz.impl` & `rapidfuzz-3.1.2/extern/rapidfuzz-cpp/rapidfuzz/fuzz.impl`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/extern/taskflow/CMakeLists.txt` & `rapidfuzz-3.1.2/extern/taskflow/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/extern/taskflow/LICENSE` & `rapidfuzz-3.1.2/extern/taskflow/LICENSE`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/extern/taskflow/taskflow/algorithm/critical.hpp` & `rapidfuzz-3.1.2/extern/taskflow/taskflow/algorithm/critical.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/extern/taskflow/taskflow/algorithm/data_pipeline.hpp` & `rapidfuzz-3.1.2/extern/taskflow/taskflow/algorithm/data_pipeline.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/extern/taskflow/taskflow/algorithm/find.hpp` & `rapidfuzz-3.1.2/extern/taskflow/taskflow/algorithm/find.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/extern/taskflow/taskflow/algorithm/for_each.hpp` & `rapidfuzz-3.1.2/extern/taskflow/taskflow/algorithm/for_each.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/extern/taskflow/taskflow/algorithm/launch.hpp` & `rapidfuzz-3.1.2/extern/taskflow/taskflow/algorithm/launch.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/extern/taskflow/taskflow/algorithm/partitioner.hpp` & `rapidfuzz-3.1.2/extern/taskflow/taskflow/algorithm/partitioner.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/extern/taskflow/taskflow/algorithm/pipeline.hpp` & `rapidfuzz-3.1.2/extern/taskflow/taskflow/algorithm/pipeline.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/extern/taskflow/taskflow/algorithm/reduce.hpp` & `rapidfuzz-3.1.2/extern/taskflow/taskflow/algorithm/reduce.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/extern/taskflow/taskflow/algorithm/scan.hpp` & `rapidfuzz-3.1.2/extern/taskflow/taskflow/algorithm/scan.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/extern/taskflow/taskflow/algorithm/sort.hpp` & `rapidfuzz-3.1.2/extern/taskflow/taskflow/algorithm/sort.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/extern/taskflow/taskflow/algorithm/transform.hpp` & `rapidfuzz-3.1.2/extern/taskflow/taskflow/algorithm/transform.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/extern/taskflow/taskflow/core/async.hpp` & `rapidfuzz-3.1.2/extern/taskflow/taskflow/core/async.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/extern/taskflow/taskflow/core/async_task.hpp` & `rapidfuzz-3.1.2/extern/taskflow/taskflow/core/async_task.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/extern/taskflow/taskflow/core/declarations.hpp` & `rapidfuzz-3.1.2/extern/taskflow/taskflow/core/declarations.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/extern/taskflow/taskflow/core/error.hpp` & `rapidfuzz-3.1.2/extern/taskflow/taskflow/core/error.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/extern/taskflow/taskflow/core/executor-module-opt.hpp` & `rapidfuzz-3.1.2/extern/taskflow/taskflow/core/executor-module-opt.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/extern/taskflow/taskflow/core/executor.hpp` & `rapidfuzz-3.1.2/extern/taskflow/taskflow/core/executor.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/extern/taskflow/taskflow/core/flow_builder.hpp` & `rapidfuzz-3.1.2/extern/taskflow/taskflow/core/flow_builder.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/extern/taskflow/taskflow/core/graph.hpp` & `rapidfuzz-3.1.2/extern/taskflow/taskflow/core/graph.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/extern/taskflow/taskflow/core/notifier.hpp` & `rapidfuzz-3.1.2/extern/taskflow/taskflow/core/notifier.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/extern/taskflow/taskflow/core/observer.hpp` & `rapidfuzz-3.1.2/extern/taskflow/taskflow/core/observer.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/extern/taskflow/taskflow/core/semaphore.hpp` & `rapidfuzz-3.1.2/extern/taskflow/taskflow/core/semaphore.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/extern/taskflow/taskflow/core/task.hpp` & `rapidfuzz-3.1.2/extern/taskflow/taskflow/core/task.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/extern/taskflow/taskflow/core/taskflow.hpp` & `rapidfuzz-3.1.2/extern/taskflow/taskflow/core/taskflow.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/extern/taskflow/taskflow/core/topology.hpp` & `rapidfuzz-3.1.2/extern/taskflow/taskflow/core/topology.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/extern/taskflow/taskflow/core/tsq.hpp` & `rapidfuzz-3.1.2/extern/taskflow/taskflow/core/tsq.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/extern/taskflow/taskflow/core/worker.hpp` & `rapidfuzz-3.1.2/extern/taskflow/taskflow/core/worker.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/extern/taskflow/taskflow/taskflow.hpp` & `rapidfuzz-3.1.2/extern/taskflow/taskflow/taskflow.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/extern/taskflow/taskflow/utility/iterator.hpp` & `rapidfuzz-3.1.2/extern/taskflow/taskflow/utility/iterator.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/extern/taskflow/taskflow/utility/math.hpp` & `rapidfuzz-3.1.2/extern/taskflow/taskflow/utility/math.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/extern/taskflow/taskflow/utility/object_pool.hpp` & `rapidfuzz-3.1.2/extern/taskflow/taskflow/utility/object_pool.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/extern/taskflow/taskflow/utility/os.hpp` & `rapidfuzz-3.1.2/extern/taskflow/taskflow/utility/os.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/extern/taskflow/taskflow/utility/serializer.hpp` & `rapidfuzz-3.1.2/extern/taskflow/taskflow/utility/serializer.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/extern/taskflow/taskflow/utility/singleton.hpp` & `rapidfuzz-3.1.2/extern/taskflow/taskflow/utility/singleton.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/extern/taskflow/taskflow/utility/small_vector.hpp` & `rapidfuzz-3.1.2/extern/taskflow/taskflow/utility/small_vector.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/extern/taskflow/taskflow/utility/stream.hpp` & `rapidfuzz-3.1.2/extern/taskflow/taskflow/utility/stream.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/extern/taskflow/taskflow/utility/traits.hpp` & `rapidfuzz-3.1.2/extern/taskflow/taskflow/utility/traits.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/extern/taskflow/taskflow/utility/uuid.hpp` & `rapidfuzz-3.1.2/extern/taskflow/taskflow/utility/uuid.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/pyproject.toml` & `rapidfuzz-3.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/setup.py` & `rapidfuzz-3.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 
 with open("README.md", encoding="utf8") as f:
     readme = f.read()
 
 setup_args = {
     "name": "rapidfuzz",
-    "version": "3.1.1",
+    "version": "3.1.2",
     "extras_require": {"full": ["numpy"]},
     "url": "https://github.com/maxbachmann/RapidFuzz",
     "author": "Max Bachmann",
     "author_email": "pypi@maxbachmann.de",
     "description": "rapid fuzzy string matching",
     "long_description": readme,
     "long_description_content_type": "text/markdown",
```

### Comparing `rapidfuzz-3.1.1/src/rapidfuzz/CMakeLists.txt` & `rapidfuzz-3.1.2/src/rapidfuzz/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/src/rapidfuzz/FeatureDetector/CpuInfo.cpp` & `rapidfuzz-3.1.2/src/rapidfuzz/FeatureDetector/CpuInfo.cpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/src/rapidfuzz/FeatureDetector/CpuInfo.hpp` & `rapidfuzz-3.1.2/src/rapidfuzz/FeatureDetector/CpuInfo.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/src/rapidfuzz/__init__.pxd` & `rapidfuzz-3.1.2/src/rapidfuzz/__init__.pxd`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/src/rapidfuzz/__init__.py` & `rapidfuzz-3.1.2/src/rapidfuzz/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 rapid string matching library
 """
 from __future__ import annotations
 
 __author__: str = "Max Bachmann"
 __license__: str = "MIT"
-__version__: str = "3.1.1"
+__version__: str = "3.1.2"
 
 from rapidfuzz import distance, fuzz, process, utils
 
 __all__ = ["distance", "fuzz", "process", "utils", "get_include"]
 
 
 def get_include():
```

### Comparing `rapidfuzz-3.1.1/src/rapidfuzz/__pyinstaller/test_rapidfuzz_packaging.py` & `rapidfuzz-3.1.2/src/rapidfuzz/__pyinstaller/test_rapidfuzz_packaging.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/src/rapidfuzz/_common_py.py` & `rapidfuzz-3.1.2/src/rapidfuzz/_common_py.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/src/rapidfuzz/_feature_detector_cpp.cxx` & `rapidfuzz-3.1.2/src/rapidfuzz/_feature_detector_cpp.cxx`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 3.0.0b3 */
+/* Generated by Cython 3.0.0 */
 
 #ifndef PY_SSIZE_T_CLEAN
 #define PY_SSIZE_T_CLEAN
 #endif /* PY_SSIZE_T_CLEAN */
 #if defined(CYTHON_LIMITED_API) && 0
   #ifndef Py_LIMITED_API
     #if CYTHON_LIMITED_API+0 > 0x03030000
@@ -15,18 +15,18 @@
 
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02070000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.7+ or Python 3.3+.
 #else
-#define CYTHON_ABI "3_0_0b3"
+#define CYTHON_ABI "3_0_0"
 #define __PYX_ABI_MODULE_NAME "_cython_" CYTHON_ABI
 #define __PYX_TYPE_MODULE_PREFIX __PYX_ABI_MODULE_NAME "."
-#define CYTHON_HEX_VERSION 0x030000B3
+#define CYTHON_HEX_VERSION 0x030000F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(_WIN32) && !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -641,14 +641,19 @@
 #endif
 #if PY_VERSION_HEX >= 0x030A00B1 || defined(Py_IsFalse)
   #define __Pyx_Py_IsFalse(ob) Py_IsFalse(ob)
 #else
   #define __Pyx_Py_IsFalse(ob) __Pyx_Py_Is((ob), Py_False)
 #endif
 #define __Pyx_NoneAsNull(obj)  (__Pyx_Py_IsNone(obj) ? NULL : (obj))
+#if PY_VERSION_HEX >= 0x030900F0 && !CYTHON_COMPILING_IN_PYPY
+  #define __Pyx_PyObject_GC_IsFinalized(o) PyObject_GC_IsFinalized(o)
+#else
+  #define __Pyx_PyObject_GC_IsFinalized(o) _PyGC_FINALIZED(o)
+#endif
 #ifndef CO_COROUTINE
   #define CO_COROUTINE 0x80
 #endif
 #ifndef CO_ASYNC_GENERATOR
   #define CO_ASYNC_GENERATOR 0x200
 #endif
 #ifndef Py_TPFLAGS_CHECKTYPES
@@ -885,15 +890,15 @@
   #endif
   #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GET_LENGTH(u)
   #define __Pyx_PyUnicode_READ_CHAR(u, i) PyUnicode_READ_CHAR(u, i)
   #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   PyUnicode_MAX_CHAR_VALUE(u)
   #define __Pyx_PyUnicode_KIND(u)         ((int)PyUnicode_KIND(u))
   #define __Pyx_PyUnicode_DATA(u)         PyUnicode_DATA(u)
   #define __Pyx_PyUnicode_READ(k, d, i)   PyUnicode_READ(k, d, i)
-  #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  PyUnicode_WRITE(k, d, i, ch)
+  #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  PyUnicode_WRITE(k, d, i, (Py_UCS4) ch)
   #if PY_VERSION_HEX >= 0x030C0000
     #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
   #else
     #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
     #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
     #else
     #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
@@ -907,15 +912,15 @@
   #define __Pyx_PyUnicode_READY(op)       (0)
   #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GET_SIZE(u)
   #define __Pyx_PyUnicode_READ_CHAR(u, i) ((Py_UCS4)(PyUnicode_AS_UNICODE(u)[i]))
   #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   ((sizeof(Py_UNICODE) == 2) ? 65535U : 1114111U)
   #define __Pyx_PyUnicode_KIND(u)         ((int)sizeof(Py_UNICODE))
   #define __Pyx_PyUnicode_DATA(u)         ((void*)PyUnicode_AS_UNICODE(u))
   #define __Pyx_PyUnicode_READ(k, d, i)   ((void)(k), (Py_UCS4)(((Py_UNICODE*)d)[i]))
-  #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  (((void)(k)), ((Py_UNICODE*)d)[i] = ch)
+  #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  (((void)(k)), ((Py_UNICODE*)d)[i] = (Py_UNICODE) ch)
   #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_SIZE(u))
 #endif
 #if CYTHON_COMPILING_IN_PYPY
   #define __Pyx_PyUnicode_Concat(a, b)      PyNumber_Add(a, b)
   #define __Pyx_PyUnicode_ConcatSafe(a, b)  PyNumber_Add(a, b)
 #else
   #define __Pyx_PyUnicode_Concat(a, b)      PyUnicode_Concat(a, b)
@@ -1214,20 +1219,20 @@
   #endif
   #define __Pyx_PyLong_Sign(x)  (((PyLongObject*)x)->long_value.lv_tag & _PyLong_SIGN_MASK)
   #define __Pyx_PyLong_IsNeg(x)  ((__Pyx_PyLong_Sign(x) & 2) != 0)
   #define __Pyx_PyLong_IsNonNeg(x)  (!__Pyx_PyLong_IsNeg(x))
   #define __Pyx_PyLong_IsZero(x)  (__Pyx_PyLong_Sign(x) & 1)
   #define __Pyx_PyLong_IsPos(x)  (__Pyx_PyLong_Sign(x) == 0)
   #define __Pyx_PyLong_CompactValueUnsigned(x)  (__Pyx_PyLong_Digits(x)[0])
-  #define __Pyx_PyLong_DigitCount(x)  (((PyLongObject*)x)->long_value.lv_tag >> _PyLong_NON_SIZE_BITS)
+  #define __Pyx_PyLong_DigitCount(x)  ((Py_ssize_t) (((PyLongObject*)x)->long_value.lv_tag >> _PyLong_NON_SIZE_BITS))
   #define __Pyx_PyLong_SignedDigitCount(x)\
-        ((1 - (Py_ssize_t) __Pyx_PyLong_Sign(x)) * (Py_ssize_t) __Pyx_PyLong_DigitCount(x))
+        ((1 - (Py_ssize_t) __Pyx_PyLong_Sign(x)) * __Pyx_PyLong_DigitCount(x))
   #if defined(PyUnstable_Long_IsCompact) && defined(PyUnstable_Long_CompactValue)
-    #define __Pyx_PyLong_IsCompact(x)     PyUnstable_Long_IsCompact(x)
-    #define __Pyx_PyLong_CompactValue(x)  PyUnstable_Long_CompactValue(x)
+    #define __Pyx_PyLong_IsCompact(x)     PyUnstable_Long_IsCompact((PyLongObject*) x)
+    #define __Pyx_PyLong_CompactValue(x)  PyUnstable_Long_CompactValue((PyLongObject*) x)
   #else
     #define __Pyx_PyLong_IsCompact(x)     (((PyLongObject*)x)->long_value.lv_tag < (2 << _PyLong_NON_SIZE_BITS))
     #define __Pyx_PyLong_CompactValue(x)  ((1 - (Py_ssize_t) __Pyx_PyLong_Sign(x)) * (Py_ssize_t) __Pyx_PyLong_Digits(x)[0])
   #endif
   typedef Py_ssize_t  __Pyx_compact_pylong;
   typedef size_t  __Pyx_compact_upylong;
   #else  // Py < 3.12
@@ -1267,15 +1272,15 @@
     if (!default_encoding_c) goto bad;
     if (strcmp(default_encoding_c, "ascii") == 0) {
         __Pyx_sys_getdefaultencoding_not_ascii = 0;
     } else {
         char ascii_chars[128];
         int c;
         for (c = 0; c < 128; c++) {
-            ascii_chars[c] = c;
+            ascii_chars[c] = (char) c;
         }
         __Pyx_sys_getdefaultencoding_not_ascii = 1;
         ascii_chars_u = PyUnicode_DecodeASCII(ascii_chars, 128, NULL);
         if (!ascii_chars_u) goto bad;
         ascii_chars_b = PyUnicode_AsEncodedString(ascii_chars_u, default_encoding_c, NULL);
         if (!ascii_chars_b || !PyBytes_Check(ascii_chars_b) || memcmp(ascii_chars, PyBytes_AS_STRING(ascii_chars_b), 128) != 0) {
             PyErr_Format(
@@ -1586,20 +1591,26 @@
   #define __Pyx_TraceDeclarations\
       static PyCodeObject *__pyx_frame_code = NULL;\
       CYTHON_FRAME_MODIFIER PyFrameObject *__pyx_frame = NULL;\
       int __Pyx_use_tracing = 0;
   #define __Pyx_TraceFrameInit(codeobj)\
       if (codeobj) __pyx_frame_code = (PyCodeObject*) codeobj;
 #if PY_VERSION_HEX >= 0x030b00a2
+  #if PY_VERSION_HEX >= 0x030C00b1
+  #define __Pyx_IsTracing(tstate, check_tracing, check_funcs)\
+     ((!(check_tracing) || !(tstate)->tracing) &&\
+         (!(check_funcs) || (tstate)->c_profilefunc || (CYTHON_TRACE && (tstate)->c_tracefunc)))
+  #else
   #define __Pyx_IsTracing(tstate, check_tracing, check_funcs)\
      (unlikely((tstate)->cframe->use_tracing) &&\
          (!(check_tracing) || !(tstate)->tracing) &&\
          (!(check_funcs) || (tstate)->c_profilefunc || (CYTHON_TRACE && (tstate)->c_tracefunc)))
-  #define __Pyx_EnterTracing(tstate) PyThreadState_EnterTracing(tstate)
-  #define __Pyx_LeaveTracing(tstate) PyThreadState_LeaveTracing(tstate)
+  #endif
+  #define __Pyx_EnterTracing(tstate)  PyThreadState_EnterTracing(tstate)
+  #define __Pyx_LeaveTracing(tstate)  PyThreadState_LeaveTracing(tstate)
 #elif PY_VERSION_HEX >= 0x030a00b1
   #define __Pyx_IsTracing(tstate, check_tracing, check_funcs)\
      (unlikely((tstate)->cframe->use_tracing) &&\
          (!(check_tracing) || !(tstate)->tracing) &&\
          (!(check_funcs) || (tstate)->c_profilefunc || (CYTHON_TRACE && (tstate)->c_tracefunc)))
   #define __Pyx_EnterTracing(tstate)\
       do { tstate->tracing++; tstate->cframe->use_tracing = 0; } while (0)
```

### Comparing `rapidfuzz-3.1.1/src/rapidfuzz/_utils.py` & `rapidfuzz-3.1.2/src/rapidfuzz/_utils.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/src/rapidfuzz/cpp_common.hpp` & `rapidfuzz-3.1.2/src/rapidfuzz/cpp_common.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/src/rapidfuzz/cpp_common.pxd` & `rapidfuzz-3.1.2/src/rapidfuzz/cpp_common.pxd`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/src/rapidfuzz/distance/CMakeLists.txt` & `rapidfuzz-3.1.2/src/rapidfuzz/distance/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/src/rapidfuzz/distance/DamerauLevenshtein.py` & `rapidfuzz-3.1.2/src/rapidfuzz/distance/DamerauLevenshtein.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/src/rapidfuzz/distance/DamerauLevenshtein.pyi` & `rapidfuzz-3.1.2/src/rapidfuzz/distance/DamerauLevenshtein.pyi`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/src/rapidfuzz/distance/DamerauLevenshtein_py.py` & `rapidfuzz-3.1.2/src/rapidfuzz/distance/DamerauLevenshtein_py.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/src/rapidfuzz/distance/Hamming.py` & `rapidfuzz-3.1.2/src/rapidfuzz/distance/Hamming.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/src/rapidfuzz/distance/Hamming.pyi` & `rapidfuzz-3.1.2/src/rapidfuzz/distance/Hamming.pyi`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/src/rapidfuzz/distance/Hamming_py.py` & `rapidfuzz-3.1.2/src/rapidfuzz/distance/Hamming_py.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/src/rapidfuzz/distance/Indel.py` & `rapidfuzz-3.1.2/src/rapidfuzz/distance/Indel.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/src/rapidfuzz/distance/Indel.pyi` & `rapidfuzz-3.1.2/src/rapidfuzz/distance/Indel.pyi`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/src/rapidfuzz/distance/Indel_py.py` & `rapidfuzz-3.1.2/src/rapidfuzz/distance/Indel_py.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/src/rapidfuzz/distance/Jaro.pyi` & `rapidfuzz-3.1.2/src/rapidfuzz/distance/Jaro.pyi`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/src/rapidfuzz/distance/JaroWinkler.pyi` & `rapidfuzz-3.1.2/src/rapidfuzz/distance/JaroWinkler.pyi`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/src/rapidfuzz/distance/JaroWinkler_py.py` & `rapidfuzz-3.1.2/src/rapidfuzz/distance/JaroWinkler_py.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/src/rapidfuzz/distance/Jaro_py.py` & `rapidfuzz-3.1.2/src/rapidfuzz/distance/Jaro_py.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/src/rapidfuzz/distance/LCSseq.py` & `rapidfuzz-3.1.2/src/rapidfuzz/distance/LCSseq.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/src/rapidfuzz/distance/LCSseq.pyi` & `rapidfuzz-3.1.2/src/rapidfuzz/distance/LCSseq.pyi`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/src/rapidfuzz/distance/LCSseq_py.py` & `rapidfuzz-3.1.2/src/rapidfuzz/distance/LCSseq_py.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/src/rapidfuzz/distance/Levenshtein.py` & `rapidfuzz-3.1.2/src/rapidfuzz/distance/Levenshtein.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/src/rapidfuzz/distance/Levenshtein.pyi` & `rapidfuzz-3.1.2/src/rapidfuzz/distance/Levenshtein.pyi`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/src/rapidfuzz/distance/Levenshtein_py.py` & `rapidfuzz-3.1.2/src/rapidfuzz/distance/Levenshtein_py.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/src/rapidfuzz/distance/OSA.pyi` & `rapidfuzz-3.1.2/src/rapidfuzz/distance/OSA.pyi`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/src/rapidfuzz/distance/OSA_py.py` & `rapidfuzz-3.1.2/src/rapidfuzz/distance/OSA_py.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/src/rapidfuzz/distance/Postfix_py.py` & `rapidfuzz-3.1.2/src/rapidfuzz/distance/Postfix_py.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/src/rapidfuzz/distance/Prefix_py.py` & `rapidfuzz-3.1.2/src/rapidfuzz/distance/Prefix_py.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/src/rapidfuzz/distance/__init__.py` & `rapidfuzz-3.1.2/src/rapidfuzz/distance/__init__.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/src/rapidfuzz/distance/__init__.pyi` & `rapidfuzz-3.1.2/src/rapidfuzz/distance/__init__.pyi`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/src/rapidfuzz/distance/_initialize.py` & `rapidfuzz-3.1.2/src/rapidfuzz/distance/_initialize.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/src/rapidfuzz/distance/_initialize.pyi` & `rapidfuzz-3.1.2/src/rapidfuzz/distance/_initialize.pyi`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/src/rapidfuzz/distance/_initialize_cpp.cxx` & `rapidfuzz-3.1.2/src/rapidfuzz/distance/_initialize_cpp.cxx`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 3.0.0b3 */
+/* Generated by Cython 3.0.0 */
 
 #ifndef PY_SSIZE_T_CLEAN
 #define PY_SSIZE_T_CLEAN
 #endif /* PY_SSIZE_T_CLEAN */
 #if defined(CYTHON_LIMITED_API) && 0
   #ifndef Py_LIMITED_API
     #if CYTHON_LIMITED_API+0 > 0x03030000
@@ -15,18 +15,18 @@
 
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02070000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.7+ or Python 3.3+.
 #else
-#define CYTHON_ABI "3_0_0b3"
+#define CYTHON_ABI "3_0_0"
 #define __PYX_ABI_MODULE_NAME "_cython_" CYTHON_ABI
 #define __PYX_TYPE_MODULE_PREFIX __PYX_ABI_MODULE_NAME "."
-#define CYTHON_HEX_VERSION 0x030000B3
+#define CYTHON_HEX_VERSION 0x030000F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(_WIN32) && !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -641,14 +641,19 @@
 #endif
 #if PY_VERSION_HEX >= 0x030A00B1 || defined(Py_IsFalse)
   #define __Pyx_Py_IsFalse(ob) Py_IsFalse(ob)
 #else
   #define __Pyx_Py_IsFalse(ob) __Pyx_Py_Is((ob), Py_False)
 #endif
 #define __Pyx_NoneAsNull(obj)  (__Pyx_Py_IsNone(obj) ? NULL : (obj))
+#if PY_VERSION_HEX >= 0x030900F0 && !CYTHON_COMPILING_IN_PYPY
+  #define __Pyx_PyObject_GC_IsFinalized(o) PyObject_GC_IsFinalized(o)
+#else
+  #define __Pyx_PyObject_GC_IsFinalized(o) _PyGC_FINALIZED(o)
+#endif
 #ifndef CO_COROUTINE
   #define CO_COROUTINE 0x80
 #endif
 #ifndef CO_ASYNC_GENERATOR
   #define CO_ASYNC_GENERATOR 0x200
 #endif
 #ifndef Py_TPFLAGS_CHECKTYPES
@@ -885,15 +890,15 @@
   #endif
   #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GET_LENGTH(u)
   #define __Pyx_PyUnicode_READ_CHAR(u, i) PyUnicode_READ_CHAR(u, i)
   #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   PyUnicode_MAX_CHAR_VALUE(u)
   #define __Pyx_PyUnicode_KIND(u)         ((int)PyUnicode_KIND(u))
   #define __Pyx_PyUnicode_DATA(u)         PyUnicode_DATA(u)
   #define __Pyx_PyUnicode_READ(k, d, i)   PyUnicode_READ(k, d, i)
-  #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  PyUnicode_WRITE(k, d, i, ch)
+  #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  PyUnicode_WRITE(k, d, i, (Py_UCS4) ch)
   #if PY_VERSION_HEX >= 0x030C0000
     #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
   #else
     #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
     #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
     #else
     #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
@@ -907,15 +912,15 @@
   #define __Pyx_PyUnicode_READY(op)       (0)
   #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GET_SIZE(u)
   #define __Pyx_PyUnicode_READ_CHAR(u, i) ((Py_UCS4)(PyUnicode_AS_UNICODE(u)[i]))
   #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   ((sizeof(Py_UNICODE) == 2) ? 65535U : 1114111U)
   #define __Pyx_PyUnicode_KIND(u)         ((int)sizeof(Py_UNICODE))
   #define __Pyx_PyUnicode_DATA(u)         ((void*)PyUnicode_AS_UNICODE(u))
   #define __Pyx_PyUnicode_READ(k, d, i)   ((void)(k), (Py_UCS4)(((Py_UNICODE*)d)[i]))
-  #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  (((void)(k)), ((Py_UNICODE*)d)[i] = ch)
+  #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  (((void)(k)), ((Py_UNICODE*)d)[i] = (Py_UNICODE) ch)
   #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_SIZE(u))
 #endif
 #if CYTHON_COMPILING_IN_PYPY
   #define __Pyx_PyUnicode_Concat(a, b)      PyNumber_Add(a, b)
   #define __Pyx_PyUnicode_ConcatSafe(a, b)  PyNumber_Add(a, b)
 #else
   #define __Pyx_PyUnicode_Concat(a, b)      PyUnicode_Concat(a, b)
@@ -1238,20 +1243,20 @@
   #endif
   #define __Pyx_PyLong_Sign(x)  (((PyLongObject*)x)->long_value.lv_tag & _PyLong_SIGN_MASK)
   #define __Pyx_PyLong_IsNeg(x)  ((__Pyx_PyLong_Sign(x) & 2) != 0)
   #define __Pyx_PyLong_IsNonNeg(x)  (!__Pyx_PyLong_IsNeg(x))
   #define __Pyx_PyLong_IsZero(x)  (__Pyx_PyLong_Sign(x) & 1)
   #define __Pyx_PyLong_IsPos(x)  (__Pyx_PyLong_Sign(x) == 0)
   #define __Pyx_PyLong_CompactValueUnsigned(x)  (__Pyx_PyLong_Digits(x)[0])
-  #define __Pyx_PyLong_DigitCount(x)  (((PyLongObject*)x)->long_value.lv_tag >> _PyLong_NON_SIZE_BITS)
+  #define __Pyx_PyLong_DigitCount(x)  ((Py_ssize_t) (((PyLongObject*)x)->long_value.lv_tag >> _PyLong_NON_SIZE_BITS))
   #define __Pyx_PyLong_SignedDigitCount(x)\
-        ((1 - (Py_ssize_t) __Pyx_PyLong_Sign(x)) * (Py_ssize_t) __Pyx_PyLong_DigitCount(x))
+        ((1 - (Py_ssize_t) __Pyx_PyLong_Sign(x)) * __Pyx_PyLong_DigitCount(x))
   #if defined(PyUnstable_Long_IsCompact) && defined(PyUnstable_Long_CompactValue)
-    #define __Pyx_PyLong_IsCompact(x)     PyUnstable_Long_IsCompact(x)
-    #define __Pyx_PyLong_CompactValue(x)  PyUnstable_Long_CompactValue(x)
+    #define __Pyx_PyLong_IsCompact(x)     PyUnstable_Long_IsCompact((PyLongObject*) x)
+    #define __Pyx_PyLong_CompactValue(x)  PyUnstable_Long_CompactValue((PyLongObject*) x)
   #else
     #define __Pyx_PyLong_IsCompact(x)     (((PyLongObject*)x)->long_value.lv_tag < (2 << _PyLong_NON_SIZE_BITS))
     #define __Pyx_PyLong_CompactValue(x)  ((1 - (Py_ssize_t) __Pyx_PyLong_Sign(x)) * (Py_ssize_t) __Pyx_PyLong_Digits(x)[0])
   #endif
   typedef Py_ssize_t  __Pyx_compact_pylong;
   typedef size_t  __Pyx_compact_upylong;
   #else  // Py < 3.12
@@ -1291,15 +1296,15 @@
     if (!default_encoding_c) goto bad;
     if (strcmp(default_encoding_c, "ascii") == 0) {
         __Pyx_sys_getdefaultencoding_not_ascii = 0;
     } else {
         char ascii_chars[128];
         int c;
         for (c = 0; c < 128; c++) {
-            ascii_chars[c] = c;
+            ascii_chars[c] = (char) c;
         }
         __Pyx_sys_getdefaultencoding_not_ascii = 1;
         ascii_chars_u = PyUnicode_DecodeASCII(ascii_chars, 128, NULL);
         if (!ascii_chars_u) goto bad;
         ascii_chars_b = PyUnicode_AsEncodedString(ascii_chars_u, default_encoding_c, NULL);
         if (!ascii_chars_b || !PyBytes_Check(ascii_chars_b) || memcmp(ascii_chars, PyBytes_AS_STRING(ascii_chars_b), 128) != 0) {
             PyErr_Format(
@@ -1798,20 +1803,26 @@
   #define __Pyx_TraceDeclarations\
       static PyCodeObject *__pyx_frame_code = NULL;\
       CYTHON_FRAME_MODIFIER PyFrameObject *__pyx_frame = NULL;\
       int __Pyx_use_tracing = 0;
   #define __Pyx_TraceFrameInit(codeobj)\
       if (codeobj) __pyx_frame_code = (PyCodeObject*) codeobj;
 #if PY_VERSION_HEX >= 0x030b00a2
+  #if PY_VERSION_HEX >= 0x030C00b1
+  #define __Pyx_IsTracing(tstate, check_tracing, check_funcs)\
+     ((!(check_tracing) || !(tstate)->tracing) &&\
+         (!(check_funcs) || (tstate)->c_profilefunc || (CYTHON_TRACE && (tstate)->c_tracefunc)))
+  #else
   #define __Pyx_IsTracing(tstate, check_tracing, check_funcs)\
      (unlikely((tstate)->cframe->use_tracing) &&\
          (!(check_tracing) || !(tstate)->tracing) &&\
          (!(check_funcs) || (tstate)->c_profilefunc || (CYTHON_TRACE && (tstate)->c_tracefunc)))
-  #define __Pyx_EnterTracing(tstate) PyThreadState_EnterTracing(tstate)
-  #define __Pyx_LeaveTracing(tstate) PyThreadState_LeaveTracing(tstate)
+  #endif
+  #define __Pyx_EnterTracing(tstate)  PyThreadState_EnterTracing(tstate)
+  #define __Pyx_LeaveTracing(tstate)  PyThreadState_LeaveTracing(tstate)
 #elif PY_VERSION_HEX >= 0x030a00b1
   #define __Pyx_IsTracing(tstate, check_tracing, check_funcs)\
      (unlikely((tstate)->cframe->use_tracing) &&\
          (!(check_tracing) || !(tstate)->tracing) &&\
          (!(check_funcs) || (tstate)->c_profilefunc || (CYTHON_TRACE && (tstate)->c_tracefunc)))
   #define __Pyx_EnterTracing(tstate)\
       do { tstate->tracing++; tstate->cframe->use_tracing = 0; } while (0)
@@ -2435,30 +2446,30 @@
 
 /* SetupReduce.proto */
 #if !CYTHON_COMPILING_IN_LIMITED_API
 static int __Pyx_setup_reduce(PyObject* type_obj);
 #endif
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto_3_0_0b3
-#define __PYX_HAVE_RT_ImportType_proto_3_0_0b3
+#ifndef __PYX_HAVE_RT_ImportType_proto_3_0_0
+#define __PYX_HAVE_RT_ImportType_proto_3_0_0
 #if defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L
 #include <stdalign.h>
 #endif
 #if (defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L) || __cplusplus >= 201103L
-#define __PYX_GET_STRUCT_ALIGNMENT_3_0_0b3(s) alignof(s)
+#define __PYX_GET_STRUCT_ALIGNMENT_3_0_0(s) alignof(s)
 #else
-#define __PYX_GET_STRUCT_ALIGNMENT_3_0_0b3(s) sizeof(void*)
+#define __PYX_GET_STRUCT_ALIGNMENT_3_0_0(s) sizeof(void*)
 #endif
-enum __Pyx_ImportType_CheckSize_3_0_0b3 {
-   __Pyx_ImportType_CheckSize_Error_3_0_0b3 = 0,
-   __Pyx_ImportType_CheckSize_Warn_3_0_0b3 = 1,
-   __Pyx_ImportType_CheckSize_Ignore_3_0_0b3 = 2
+enum __Pyx_ImportType_CheckSize_3_0_0 {
+   __Pyx_ImportType_CheckSize_Error_3_0_0 = 0,
+   __Pyx_ImportType_CheckSize_Warn_3_0_0 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_3_0_0 = 2
 };
-static PyTypeObject *__Pyx_ImportType_3_0_0b3(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_0b3 check_size);
+static PyTypeObject *__Pyx_ImportType_3_0_0(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_0 check_size);
 #endif
 
 /* FetchSharedCythonModule.proto */
 static PyObject *__Pyx_FetchSharedCythonABIModule(void);
 
 /* FetchCommonType.proto */
 #if !CYTHON_USE_TYPE_SPECS
@@ -5062,17 +5073,17 @@
  *         s_proc.data = NULL
  */
     __Pyx_TraceLine(291,0,__PYX_ERR(1, 291, __pyx_L6_except_error))
     __pyx_t_13 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_13) {
       __Pyx_AddTraceback("cpp_common.hash_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_1, &__pyx_t_14, &__pyx_t_15) < 0) __PYX_ERR(1, 291, __pyx_L6_except_error)
-      __Pyx_GOTREF(__pyx_t_1);
-      __Pyx_GOTREF(__pyx_t_14);
-      __Pyx_GOTREF(__pyx_t_15);
+      __Pyx_XGOTREF(__pyx_t_1);
+      __Pyx_XGOTREF(__pyx_t_14);
+      __Pyx_XGOTREF(__pyx_t_15);
       __Pyx_INCREF(__pyx_t_14);
       __pyx_v_e = __pyx_t_14;
       /*try:*/ {
 
         /* "cpp_common.pxd":292
  *                 (<uint64_t*>s_proc.data)[i] = <uint64_t>hash(arr[i])
  *     except Exception as e:
@@ -5479,17 +5490,17 @@
  *         s_proc.data = NULL
  */
     __Pyx_TraceLine(320,0,__PYX_ERR(1, 320, __pyx_L6_except_error))
     __pyx_t_13 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_13) {
       __Pyx_AddTraceback("cpp_common.hash_sequence", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_9, &__pyx_t_14, &__pyx_t_15) < 0) __PYX_ERR(1, 320, __pyx_L6_except_error)
-      __Pyx_GOTREF(__pyx_t_9);
-      __Pyx_GOTREF(__pyx_t_14);
-      __Pyx_GOTREF(__pyx_t_15);
+      __Pyx_XGOTREF(__pyx_t_9);
+      __Pyx_XGOTREF(__pyx_t_14);
+      __Pyx_XGOTREF(__pyx_t_15);
       __Pyx_INCREF(__pyx_t_14);
       __pyx_v_e = __pyx_t_14;
       /*try:*/ {
 
         /* "cpp_common.pxd":321
  *                 (<uint64_t*>s_proc.data)[i] = <uint64_t>hash(elem)
  *     except Exception as e:
@@ -9925,17 +9936,17 @@
  *             return False
  * 
  */
     __Pyx_TraceLine(205,0,__PYX_ERR(0, 205, __pyx_L5_except_error))
     /*except:*/ {
       __Pyx_AddTraceback("rapidfuzz.distance._initialize_cpp.MatchingBlock.__eq__", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_6, &__pyx_t_9, &__pyx_t_8) < 0) __PYX_ERR(0, 205, __pyx_L5_except_error)
-      __Pyx_GOTREF(__pyx_t_6);
-      __Pyx_GOTREF(__pyx_t_9);
-      __Pyx_GOTREF(__pyx_t_8);
+      __Pyx_XGOTREF(__pyx_t_6);
+      __Pyx_XGOTREF(__pyx_t_9);
+      __Pyx_XGOTREF(__pyx_t_8);
 
       /* "rapidfuzz/distance/_initialize_cpp.pyx":206
  *                 and other[2] == self.size)
  *         except:
  *             return False             # <<<<<<<<<<<<<<
  * 
  *     def __getitem__(self, Py_ssize_t i):
@@ -12738,17 +12749,17 @@
  *             return False
  * 
  */
     __Pyx_TraceLine(346,0,__PYX_ERR(0, 346, __pyx_L5_except_error))
     /*except:*/ {
       __Pyx_AddTraceback("rapidfuzz.distance._initialize_cpp.Editop.__eq__", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_6, &__pyx_t_8, &__pyx_t_7) < 0) __PYX_ERR(0, 346, __pyx_L5_except_error)
-      __Pyx_GOTREF(__pyx_t_6);
-      __Pyx_GOTREF(__pyx_t_8);
-      __Pyx_GOTREF(__pyx_t_7);
+      __Pyx_XGOTREF(__pyx_t_6);
+      __Pyx_XGOTREF(__pyx_t_8);
+      __Pyx_XGOTREF(__pyx_t_7);
 
       /* "rapidfuzz/distance/_initialize_cpp.pyx":347
  *                 and other[2] == self.dest_pos)
  *         except:
  *             return False             # <<<<<<<<<<<<<<
  * 
  *     def __getitem__(self, Py_ssize_t i):
@@ -17659,17 +17670,17 @@
  *             return False
  * 
  */
     __Pyx_TraceLine(639,0,__PYX_ERR(0, 639, __pyx_L5_except_error))
     /*except:*/ {
       __Pyx_AddTraceback("rapidfuzz.distance._initialize_cpp.Opcode.__eq__", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_6, &__pyx_t_8, &__pyx_t_7) < 0) __PYX_ERR(0, 639, __pyx_L5_except_error)
-      __Pyx_GOTREF(__pyx_t_6);
-      __Pyx_GOTREF(__pyx_t_8);
-      __Pyx_GOTREF(__pyx_t_7);
+      __Pyx_XGOTREF(__pyx_t_6);
+      __Pyx_XGOTREF(__pyx_t_8);
+      __Pyx_XGOTREF(__pyx_t_7);
 
       /* "rapidfuzz/distance/_initialize_cpp.pyx":640
  *                 and other[4] == self.dest_end)
  *         except:
  *             return False             # <<<<<<<<<<<<<<
  * 
  *     def __getitem__(self, Py_ssize_t i):
@@ -22231,17 +22242,17 @@
  *             return False
  * 
  */
     __Pyx_TraceLine(873,0,__PYX_ERR(0, 873, __pyx_L5_except_error))
     /*except:*/ {
       __Pyx_AddTraceback("rapidfuzz.distance._initialize_cpp.ScoreAlignment.__eq__", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_6, &__pyx_t_8, &__pyx_t_7) < 0) __PYX_ERR(0, 873, __pyx_L5_except_error)
-      __Pyx_GOTREF(__pyx_t_6);
-      __Pyx_GOTREF(__pyx_t_8);
-      __Pyx_GOTREF(__pyx_t_7);
+      __Pyx_XGOTREF(__pyx_t_6);
+      __Pyx_XGOTREF(__pyx_t_8);
+      __Pyx_XGOTREF(__pyx_t_7);
 
       /* "rapidfuzz/distance/_initialize_cpp.pyx":874
  *                 and other[4] == self.dest_end)
  *         except:
  *             return False             # <<<<<<<<<<<<<<
  * 
  *     def __getitem__(self, Py_ssize_t i):
@@ -25125,15 +25136,15 @@
   new((void*)&(p->editops)) rapidfuzz::Editops();
   return o;
 }
 
 static void __pyx_tp_dealloc_9rapidfuzz_8distance_15_initialize_cpp_Editops(PyObject *o) {
   struct __pyx_obj_9rapidfuzz_8distance_15_initialize_cpp_Editops *p = (struct __pyx_obj_9rapidfuzz_8distance_15_initialize_cpp_Editops *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely((PY_VERSION_HEX >= 0x03080000 || __Pyx_PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE)) && __Pyx_PyObject_GetSlot(o, tp_finalize, destructor)) && (!PyType_IS_GC(Py_TYPE(o)) || !_PyGC_FINALIZED(o))) {
+  if (unlikely((PY_VERSION_HEX >= 0x03080000 || __Pyx_PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE)) && __Pyx_PyObject_GetSlot(o, tp_finalize, destructor)) && (!PyType_IS_GC(Py_TYPE(o)) || !__Pyx_PyObject_GC_IsFinalized(o))) {
     if (__Pyx_PyObject_GetSlot(o, tp_dealloc, destructor) == __pyx_tp_dealloc_9rapidfuzz_8distance_15_initialize_cpp_Editops) {
       if (PyObject_CallFinalizerFromDealloc(o)) return;
     }
   }
   #endif
   __Pyx_call_destructor(p->editops);
   (*Py_TYPE(o)->tp_free)(o);
@@ -25381,15 +25392,15 @@
   new((void*)&(p->opcodes)) rapidfuzz::Opcodes();
   return o;
 }
 
 static void __pyx_tp_dealloc_9rapidfuzz_8distance_15_initialize_cpp_Opcodes(PyObject *o) {
   struct __pyx_obj_9rapidfuzz_8distance_15_initialize_cpp_Opcodes *p = (struct __pyx_obj_9rapidfuzz_8distance_15_initialize_cpp_Opcodes *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely((PY_VERSION_HEX >= 0x03080000 || __Pyx_PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE)) && __Pyx_PyObject_GetSlot(o, tp_finalize, destructor)) && (!PyType_IS_GC(Py_TYPE(o)) || !_PyGC_FINALIZED(o))) {
+  if (unlikely((PY_VERSION_HEX >= 0x03080000 || __Pyx_PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE)) && __Pyx_PyObject_GetSlot(o, tp_finalize, destructor)) && (!PyType_IS_GC(Py_TYPE(o)) || !__Pyx_PyObject_GC_IsFinalized(o))) {
     if (__Pyx_PyObject_GetSlot(o, tp_dealloc, destructor) == __pyx_tp_dealloc_9rapidfuzz_8distance_15_initialize_cpp_Opcodes) {
       if (PyObject_CallFinalizerFromDealloc(o)) return;
     }
   }
   #endif
   __Pyx_call_destructor(p->opcodes);
   (*Py_TYPE(o)->tp_free)(o);
@@ -25621,15 +25632,15 @@
   p->score = Py_None; Py_INCREF(Py_None);
   return o;
 }
 
 static void __pyx_tp_dealloc_9rapidfuzz_8distance_15_initialize_cpp_ScoreAlignment(PyObject *o) {
   struct __pyx_obj_9rapidfuzz_8distance_15_initialize_cpp_ScoreAlignment *p = (struct __pyx_obj_9rapidfuzz_8distance_15_initialize_cpp_ScoreAlignment *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely((PY_VERSION_HEX >= 0x03080000 || __Pyx_PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE)) && __Pyx_PyObject_GetSlot(o, tp_finalize, destructor)) && !_PyGC_FINALIZED(o)) {
+  if (unlikely((PY_VERSION_HEX >= 0x03080000 || __Pyx_PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE)) && __Pyx_PyObject_GetSlot(o, tp_finalize, destructor)) && !__Pyx_PyObject_GC_IsFinalized(o)) {
     if (__Pyx_PyObject_GetSlot(o, tp_dealloc, destructor) == __pyx_tp_dealloc_9rapidfuzz_8distance_15_initialize_cpp_ScoreAlignment) {
       if (PyObject_CallFinalizerFromDealloc(o)) return;
     }
   }
   #endif
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->score);
@@ -25919,15 +25930,15 @@
   bad:
   Py_DECREF(o); o = 0;
   return NULL;
 }
 
 static void __pyx_tp_dealloc_9rapidfuzz_8distance_15_initialize_cpp_MatchingBlock(PyObject *o) {
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely((PY_VERSION_HEX >= 0x03080000 || __Pyx_PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE)) && __Pyx_PyObject_GetSlot(o, tp_finalize, destructor)) && (!PyType_IS_GC(Py_TYPE(o)) || !_PyGC_FINALIZED(o))) {
+  if (unlikely((PY_VERSION_HEX >= 0x03080000 || __Pyx_PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE)) && __Pyx_PyObject_GetSlot(o, tp_finalize, destructor)) && (!PyType_IS_GC(Py_TYPE(o)) || !__Pyx_PyObject_GC_IsFinalized(o))) {
     if (__Pyx_PyObject_GetSlot(o, tp_dealloc, destructor) == __pyx_tp_dealloc_9rapidfuzz_8distance_15_initialize_cpp_MatchingBlock) {
       if (PyObject_CallFinalizerFromDealloc(o)) return;
     }
   }
   #endif
   (*Py_TYPE(o)->tp_free)(o);
 }
@@ -26165,15 +26176,15 @@
   p->tag = ((PyObject*)Py_None); Py_INCREF(Py_None);
   return o;
 }
 
 static void __pyx_tp_dealloc_9rapidfuzz_8distance_15_initialize_cpp_Editop(PyObject *o) {
   struct __pyx_obj_9rapidfuzz_8distance_15_initialize_cpp_Editop *p = (struct __pyx_obj_9rapidfuzz_8distance_15_initialize_cpp_Editop *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely((PY_VERSION_HEX >= 0x03080000 || __Pyx_PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE)) && __Pyx_PyObject_GetSlot(o, tp_finalize, destructor)) && (!PyType_IS_GC(Py_TYPE(o)) || !_PyGC_FINALIZED(o))) {
+  if (unlikely((PY_VERSION_HEX >= 0x03080000 || __Pyx_PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE)) && __Pyx_PyObject_GetSlot(o, tp_finalize, destructor)) && (!PyType_IS_GC(Py_TYPE(o)) || !__Pyx_PyObject_GC_IsFinalized(o))) {
     if (__Pyx_PyObject_GetSlot(o, tp_dealloc, destructor) == __pyx_tp_dealloc_9rapidfuzz_8distance_15_initialize_cpp_Editop) {
       if (PyObject_CallFinalizerFromDealloc(o)) return;
     }
   }
   #endif
   Py_CLEAR(p->tag);
   (*Py_TYPE(o)->tp_free)(o);
@@ -26412,15 +26423,15 @@
   p->tag = ((PyObject*)Py_None); Py_INCREF(Py_None);
   return o;
 }
 
 static void __pyx_tp_dealloc_9rapidfuzz_8distance_15_initialize_cpp_Opcode(PyObject *o) {
   struct __pyx_obj_9rapidfuzz_8distance_15_initialize_cpp_Opcode *p = (struct __pyx_obj_9rapidfuzz_8distance_15_initialize_cpp_Opcode *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely((PY_VERSION_HEX >= 0x03080000 || __Pyx_PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE)) && __Pyx_PyObject_GetSlot(o, tp_finalize, destructor)) && (!PyType_IS_GC(Py_TYPE(o)) || !_PyGC_FINALIZED(o))) {
+  if (unlikely((PY_VERSION_HEX >= 0x03080000 || __Pyx_PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE)) && __Pyx_PyObject_GetSlot(o, tp_finalize, destructor)) && (!PyType_IS_GC(Py_TYPE(o)) || !__Pyx_PyObject_GC_IsFinalized(o))) {
     if (__Pyx_PyObject_GetSlot(o, tp_dealloc, destructor) == __pyx_tp_dealloc_9rapidfuzz_8distance_15_initialize_cpp_Opcode) {
       if (PyObject_CallFinalizerFromDealloc(o)) return;
     }
   }
   #endif
   Py_CLEAR(p->tag);
   (*Py_TYPE(o)->tp_free)(o);
@@ -26692,15 +26703,15 @@
   #endif
   return o;
 }
 
 static void __pyx_tp_dealloc_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct____iter__(PyObject *o) {
   struct __pyx_obj_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct____iter__ *p = (struct __pyx_obj_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct____iter__ *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely((PY_VERSION_HEX >= 0x03080000 || __Pyx_PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE)) && __Pyx_PyObject_GetSlot(o, tp_finalize, destructor)) && !_PyGC_FINALIZED(o)) {
+  if (unlikely((PY_VERSION_HEX >= 0x03080000 || __Pyx_PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE)) && __Pyx_PyObject_GetSlot(o, tp_finalize, destructor)) && !__Pyx_PyObject_GC_IsFinalized(o)) {
     if (__Pyx_PyObject_GetSlot(o, tp_dealloc, destructor) == __pyx_tp_dealloc_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct____iter__) {
       if (PyObject_CallFinalizerFromDealloc(o)) return;
     }
   }
   #endif
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->__pyx_v_self);
@@ -26838,15 +26849,15 @@
   #endif
   return o;
 }
 
 static void __pyx_tp_dealloc_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct_1___iter__(PyObject *o) {
   struct __pyx_obj_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct_1___iter__ *p = (struct __pyx_obj_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct_1___iter__ *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely((PY_VERSION_HEX >= 0x03080000 || __Pyx_PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE)) && __Pyx_PyObject_GetSlot(o, tp_finalize, destructor)) && !_PyGC_FINALIZED(o)) {
+  if (unlikely((PY_VERSION_HEX >= 0x03080000 || __Pyx_PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE)) && __Pyx_PyObject_GetSlot(o, tp_finalize, destructor)) && !__Pyx_PyObject_GC_IsFinalized(o)) {
     if (__Pyx_PyObject_GetSlot(o, tp_dealloc, destructor) == __pyx_tp_dealloc_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct_1___iter__) {
       if (PyObject_CallFinalizerFromDealloc(o)) return;
     }
   }
   #endif
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->__pyx_v_self);
@@ -26984,15 +26995,15 @@
   #endif
   return o;
 }
 
 static void __pyx_tp_dealloc_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct_2___iter__(PyObject *o) {
   struct __pyx_obj_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct_2___iter__ *p = (struct __pyx_obj_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct_2___iter__ *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely((PY_VERSION_HEX >= 0x03080000 || __Pyx_PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE)) && __Pyx_PyObject_GetSlot(o, tp_finalize, destructor)) && !_PyGC_FINALIZED(o)) {
+  if (unlikely((PY_VERSION_HEX >= 0x03080000 || __Pyx_PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE)) && __Pyx_PyObject_GetSlot(o, tp_finalize, destructor)) && !__Pyx_PyObject_GC_IsFinalized(o)) {
     if (__Pyx_PyObject_GetSlot(o, tp_dealloc, destructor) == __pyx_tp_dealloc_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct_2___iter__) {
       if (PyObject_CallFinalizerFromDealloc(o)) return;
     }
   }
   #endif
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->__pyx_v_self);
@@ -27130,15 +27141,15 @@
   #endif
   return o;
 }
 
 static void __pyx_tp_dealloc_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct_3_genexpr(PyObject *o) {
   struct __pyx_obj_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct_3_genexpr *p = (struct __pyx_obj_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct_3_genexpr *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely((PY_VERSION_HEX >= 0x03080000 || __Pyx_PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE)) && __Pyx_PyObject_GetSlot(o, tp_finalize, destructor)) && !_PyGC_FINALIZED(o)) {
+  if (unlikely((PY_VERSION_HEX >= 0x03080000 || __Pyx_PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE)) && __Pyx_PyObject_GetSlot(o, tp_finalize, destructor)) && !__Pyx_PyObject_GC_IsFinalized(o)) {
     if (__Pyx_PyObject_GetSlot(o, tp_dealloc, destructor) == __pyx_tp_dealloc_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct_3_genexpr) {
       if (PyObject_CallFinalizerFromDealloc(o)) return;
     }
   }
   #endif
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->__pyx_genexpr_arg_0);
@@ -27280,15 +27291,15 @@
   #endif
   return o;
 }
 
 static void __pyx_tp_dealloc_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct_4___iter__(PyObject *o) {
   struct __pyx_obj_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct_4___iter__ *p = (struct __pyx_obj_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct_4___iter__ *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely((PY_VERSION_HEX >= 0x03080000 || __Pyx_PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE)) && __Pyx_PyObject_GetSlot(o, tp_finalize, destructor)) && !_PyGC_FINALIZED(o)) {
+  if (unlikely((PY_VERSION_HEX >= 0x03080000 || __Pyx_PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE)) && __Pyx_PyObject_GetSlot(o, tp_finalize, destructor)) && !__Pyx_PyObject_GC_IsFinalized(o)) {
     if (__Pyx_PyObject_GetSlot(o, tp_dealloc, destructor) == __pyx_tp_dealloc_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct_4___iter__) {
       if (PyObject_CallFinalizerFromDealloc(o)) return;
     }
   }
   #endif
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->__pyx_v_self);
@@ -27426,15 +27437,15 @@
   #endif
   return o;
 }
 
 static void __pyx_tp_dealloc_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct_5___iter__(PyObject *o) {
   struct __pyx_obj_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct_5___iter__ *p = (struct __pyx_obj_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct_5___iter__ *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely((PY_VERSION_HEX >= 0x03080000 || __Pyx_PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE)) && __Pyx_PyObject_GetSlot(o, tp_finalize, destructor)) && !_PyGC_FINALIZED(o)) {
+  if (unlikely((PY_VERSION_HEX >= 0x03080000 || __Pyx_PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE)) && __Pyx_PyObject_GetSlot(o, tp_finalize, destructor)) && !__Pyx_PyObject_GC_IsFinalized(o)) {
     if (__Pyx_PyObject_GetSlot(o, tp_dealloc, destructor) == __pyx_tp_dealloc_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct_5___iter__) {
       if (PyObject_CallFinalizerFromDealloc(o)) return;
     }
   }
   #endif
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->__pyx_v_self);
@@ -27572,15 +27583,15 @@
   #endif
   return o;
 }
 
 static void __pyx_tp_dealloc_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct_6_genexpr(PyObject *o) {
   struct __pyx_obj_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct_6_genexpr *p = (struct __pyx_obj_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct_6_genexpr *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely((PY_VERSION_HEX >= 0x03080000 || __Pyx_PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE)) && __Pyx_PyObject_GetSlot(o, tp_finalize, destructor)) && !_PyGC_FINALIZED(o)) {
+  if (unlikely((PY_VERSION_HEX >= 0x03080000 || __Pyx_PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE)) && __Pyx_PyObject_GetSlot(o, tp_finalize, destructor)) && !__Pyx_PyObject_GC_IsFinalized(o)) {
     if (__Pyx_PyObject_GetSlot(o, tp_dealloc, destructor) == __pyx_tp_dealloc_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct_6_genexpr) {
       if (PyObject_CallFinalizerFromDealloc(o)) return;
     }
   }
   #endif
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->__pyx_genexpr_arg_0);
@@ -27722,15 +27733,15 @@
   #endif
   return o;
 }
 
 static void __pyx_tp_dealloc_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct_7___iter__(PyObject *o) {
   struct __pyx_obj_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct_7___iter__ *p = (struct __pyx_obj_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct_7___iter__ *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely((PY_VERSION_HEX >= 0x03080000 || __Pyx_PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE)) && __Pyx_PyObject_GetSlot(o, tp_finalize, destructor)) && !_PyGC_FINALIZED(o)) {
+  if (unlikely((PY_VERSION_HEX >= 0x03080000 || __Pyx_PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE)) && __Pyx_PyObject_GetSlot(o, tp_finalize, destructor)) && !__Pyx_PyObject_GC_IsFinalized(o)) {
     if (__Pyx_PyObject_GetSlot(o, tp_dealloc, destructor) == __pyx_tp_dealloc_9rapidfuzz_8distance_15_initialize_cpp___pyx_scope_struct_7___iter__) {
       if (PyObject_CallFinalizerFromDealloc(o)) return;
     }
   }
   #endif
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->__pyx_v_self);
@@ -28915,23 +28926,23 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(4, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_3_0_0b3(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
+  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_3_0_0(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0b3(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(PyTypeObject),
   #elif CYTHON_COMPILING_IN_LIMITED_API
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0b3(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0b3(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(PyHeapTypeObject),
   #endif
-  __Pyx_ImportType_CheckSize_Warn_3_0_0b3); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(4, 9, __pyx_L1_error)
+  __Pyx_ImportType_CheckSize_Warn_3_0_0); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(4, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -32760,18 +32771,18 @@
     Py_XDECREF(setstate);
     Py_XDECREF(setstate_cython);
     return ret;
 }
 #endif
 
 /* TypeImport */
-#ifndef __PYX_HAVE_RT_ImportType_3_0_0b3
-#define __PYX_HAVE_RT_ImportType_3_0_0b3
-static PyTypeObject *__Pyx_ImportType_3_0_0b3(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_0b3 check_size)
+#ifndef __PYX_HAVE_RT_ImportType_3_0_0
+#define __PYX_HAVE_RT_ImportType_3_0_0
+static PyTypeObject *__Pyx_ImportType_3_0_0(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_0 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
     Py_ssize_t itemsize;
 #if CYTHON_COMPILING_IN_LIMITED_API
     PyObject *py_basicsize;
@@ -32817,23 +32828,23 @@
     if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize+itemsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error_3_0_0b3 &&
+    if (check_size == __Pyx_ImportType_CheckSize_Error_3_0_0 &&
             ((size_t)basicsize > size || (size_t)(basicsize + itemsize) < size)) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd-%zd from PyObject",
             module_name, class_name, size, basicsize, basicsize+itemsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn_3_0_0b3 && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_3_0_0 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
```

### Comparing `rapidfuzz-3.1.1/src/rapidfuzz/distance/_initialize_cpp.pyx` & `rapidfuzz-3.1.2/src/rapidfuzz/distance/_initialize_cpp.pyx`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/src/rapidfuzz/distance/_initialize_py.py` & `rapidfuzz-3.1.2/src/rapidfuzz/distance/_initialize_py.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/src/rapidfuzz/distance/metrics.hpp` & `rapidfuzz-3.1.2/src/rapidfuzz/distance/metrics.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/src/rapidfuzz/distance/metrics_cpp.cxx` & `rapidfuzz-3.1.2/src/rapidfuzz/distance/metrics_cpp.cxx`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 3.0.0b3 */
+/* Generated by Cython 3.0.0 */
 
 #ifndef PY_SSIZE_T_CLEAN
 #define PY_SSIZE_T_CLEAN
 #endif /* PY_SSIZE_T_CLEAN */
 #if defined(CYTHON_LIMITED_API) && 0
   #ifndef Py_LIMITED_API
     #if CYTHON_LIMITED_API+0 > 0x03030000
@@ -15,18 +15,18 @@
 
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02070000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.7+ or Python 3.3+.
 #else
-#define CYTHON_ABI "3_0_0b3"
+#define CYTHON_ABI "3_0_0"
 #define __PYX_ABI_MODULE_NAME "_cython_" CYTHON_ABI
 #define __PYX_TYPE_MODULE_PREFIX __PYX_ABI_MODULE_NAME "."
-#define CYTHON_HEX_VERSION 0x030000B3
+#define CYTHON_HEX_VERSION 0x030000F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(_WIN32) && !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -641,14 +641,19 @@
 #endif
 #if PY_VERSION_HEX >= 0x030A00B1 || defined(Py_IsFalse)
   #define __Pyx_Py_IsFalse(ob) Py_IsFalse(ob)
 #else
   #define __Pyx_Py_IsFalse(ob) __Pyx_Py_Is((ob), Py_False)
 #endif
 #define __Pyx_NoneAsNull(obj)  (__Pyx_Py_IsNone(obj) ? NULL : (obj))
+#if PY_VERSION_HEX >= 0x030900F0 && !CYTHON_COMPILING_IN_PYPY
+  #define __Pyx_PyObject_GC_IsFinalized(o) PyObject_GC_IsFinalized(o)
+#else
+  #define __Pyx_PyObject_GC_IsFinalized(o) _PyGC_FINALIZED(o)
+#endif
 #ifndef CO_COROUTINE
   #define CO_COROUTINE 0x80
 #endif
 #ifndef CO_ASYNC_GENERATOR
   #define CO_ASYNC_GENERATOR 0x200
 #endif
 #ifndef Py_TPFLAGS_CHECKTYPES
@@ -885,15 +890,15 @@
   #endif
   #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GET_LENGTH(u)
   #define __Pyx_PyUnicode_READ_CHAR(u, i) PyUnicode_READ_CHAR(u, i)
   #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   PyUnicode_MAX_CHAR_VALUE(u)
   #define __Pyx_PyUnicode_KIND(u)         ((int)PyUnicode_KIND(u))
   #define __Pyx_PyUnicode_DATA(u)         PyUnicode_DATA(u)
   #define __Pyx_PyUnicode_READ(k, d, i)   PyUnicode_READ(k, d, i)
-  #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  PyUnicode_WRITE(k, d, i, ch)
+  #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  PyUnicode_WRITE(k, d, i, (Py_UCS4) ch)
   #if PY_VERSION_HEX >= 0x030C0000
     #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
   #else
     #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
     #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
     #else
     #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
@@ -907,15 +912,15 @@
   #define __Pyx_PyUnicode_READY(op)       (0)
   #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GET_SIZE(u)
   #define __Pyx_PyUnicode_READ_CHAR(u, i) ((Py_UCS4)(PyUnicode_AS_UNICODE(u)[i]))
   #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   ((sizeof(Py_UNICODE) == 2) ? 65535U : 1114111U)
   #define __Pyx_PyUnicode_KIND(u)         ((int)sizeof(Py_UNICODE))
   #define __Pyx_PyUnicode_DATA(u)         ((void*)PyUnicode_AS_UNICODE(u))
   #define __Pyx_PyUnicode_READ(k, d, i)   ((void)(k), (Py_UCS4)(((Py_UNICODE*)d)[i]))
-  #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  (((void)(k)), ((Py_UNICODE*)d)[i] = ch)
+  #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  (((void)(k)), ((Py_UNICODE*)d)[i] = (Py_UNICODE) ch)
   #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_SIZE(u))
 #endif
 #if CYTHON_COMPILING_IN_PYPY
   #define __Pyx_PyUnicode_Concat(a, b)      PyNumber_Add(a, b)
   #define __Pyx_PyUnicode_ConcatSafe(a, b)  PyNumber_Add(a, b)
 #else
   #define __Pyx_PyUnicode_Concat(a, b)      PyUnicode_Concat(a, b)
@@ -1240,20 +1245,20 @@
   #endif
   #define __Pyx_PyLong_Sign(x)  (((PyLongObject*)x)->long_value.lv_tag & _PyLong_SIGN_MASK)
   #define __Pyx_PyLong_IsNeg(x)  ((__Pyx_PyLong_Sign(x) & 2) != 0)
   #define __Pyx_PyLong_IsNonNeg(x)  (!__Pyx_PyLong_IsNeg(x))
   #define __Pyx_PyLong_IsZero(x)  (__Pyx_PyLong_Sign(x) & 1)
   #define __Pyx_PyLong_IsPos(x)  (__Pyx_PyLong_Sign(x) == 0)
   #define __Pyx_PyLong_CompactValueUnsigned(x)  (__Pyx_PyLong_Digits(x)[0])
-  #define __Pyx_PyLong_DigitCount(x)  (((PyLongObject*)x)->long_value.lv_tag >> _PyLong_NON_SIZE_BITS)
+  #define __Pyx_PyLong_DigitCount(x)  ((Py_ssize_t) (((PyLongObject*)x)->long_value.lv_tag >> _PyLong_NON_SIZE_BITS))
   #define __Pyx_PyLong_SignedDigitCount(x)\
-        ((1 - (Py_ssize_t) __Pyx_PyLong_Sign(x)) * (Py_ssize_t) __Pyx_PyLong_DigitCount(x))
+        ((1 - (Py_ssize_t) __Pyx_PyLong_Sign(x)) * __Pyx_PyLong_DigitCount(x))
   #if defined(PyUnstable_Long_IsCompact) && defined(PyUnstable_Long_CompactValue)
-    #define __Pyx_PyLong_IsCompact(x)     PyUnstable_Long_IsCompact(x)
-    #define __Pyx_PyLong_CompactValue(x)  PyUnstable_Long_CompactValue(x)
+    #define __Pyx_PyLong_IsCompact(x)     PyUnstable_Long_IsCompact((PyLongObject*) x)
+    #define __Pyx_PyLong_CompactValue(x)  PyUnstable_Long_CompactValue((PyLongObject*) x)
   #else
     #define __Pyx_PyLong_IsCompact(x)     (((PyLongObject*)x)->long_value.lv_tag < (2 << _PyLong_NON_SIZE_BITS))
     #define __Pyx_PyLong_CompactValue(x)  ((1 - (Py_ssize_t) __Pyx_PyLong_Sign(x)) * (Py_ssize_t) __Pyx_PyLong_Digits(x)[0])
   #endif
   typedef Py_ssize_t  __Pyx_compact_pylong;
   typedef size_t  __Pyx_compact_upylong;
   #else  // Py < 3.12
@@ -1293,15 +1298,15 @@
     if (!default_encoding_c) goto bad;
     if (strcmp(default_encoding_c, "ascii") == 0) {
         __Pyx_sys_getdefaultencoding_not_ascii = 0;
     } else {
         char ascii_chars[128];
         int c;
         for (c = 0; c < 128; c++) {
-            ascii_chars[c] = c;
+            ascii_chars[c] = (char) c;
         }
         __Pyx_sys_getdefaultencoding_not_ascii = 1;
         ascii_chars_u = PyUnicode_DecodeASCII(ascii_chars, 128, NULL);
         if (!ascii_chars_u) goto bad;
         ascii_chars_b = PyUnicode_AsEncodedString(ascii_chars_u, default_encoding_c, NULL);
         if (!ascii_chars_b || !PyBytes_Check(ascii_chars_b) || memcmp(ascii_chars, PyBytes_AS_STRING(ascii_chars_b), 128) != 0) {
             PyErr_Format(
@@ -1632,20 +1637,26 @@
   #define __Pyx_TraceDeclarations\
       static PyCodeObject *__pyx_frame_code = NULL;\
       CYTHON_FRAME_MODIFIER PyFrameObject *__pyx_frame = NULL;\
       int __Pyx_use_tracing = 0;
   #define __Pyx_TraceFrameInit(codeobj)\
       if (codeobj) __pyx_frame_code = (PyCodeObject*) codeobj;
 #if PY_VERSION_HEX >= 0x030b00a2
+  #if PY_VERSION_HEX >= 0x030C00b1
+  #define __Pyx_IsTracing(tstate, check_tracing, check_funcs)\
+     ((!(check_tracing) || !(tstate)->tracing) &&\
+         (!(check_funcs) || (tstate)->c_profilefunc || (CYTHON_TRACE && (tstate)->c_tracefunc)))
+  #else
   #define __Pyx_IsTracing(tstate, check_tracing, check_funcs)\
      (unlikely((tstate)->cframe->use_tracing) &&\
          (!(check_tracing) || !(tstate)->tracing) &&\
          (!(check_funcs) || (tstate)->c_profilefunc || (CYTHON_TRACE && (tstate)->c_tracefunc)))
-  #define __Pyx_EnterTracing(tstate) PyThreadState_EnterTracing(tstate)
-  #define __Pyx_LeaveTracing(tstate) PyThreadState_LeaveTracing(tstate)
+  #endif
+  #define __Pyx_EnterTracing(tstate)  PyThreadState_EnterTracing(tstate)
+  #define __Pyx_LeaveTracing(tstate)  PyThreadState_LeaveTracing(tstate)
 #elif PY_VERSION_HEX >= 0x030a00b1
   #define __Pyx_IsTracing(tstate, check_tracing, check_funcs)\
      (unlikely((tstate)->cframe->use_tracing) &&\
          (!(check_tracing) || !(tstate)->tracing) &&\
          (!(check_funcs) || (tstate)->c_profilefunc || (CYTHON_TRACE && (tstate)->c_tracefunc)))
   #define __Pyx_EnterTracing(tstate)\
       do { tstate->tracing++; tstate->cframe->use_tracing = 0; } while (0)
@@ -2160,30 +2171,30 @@
 #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030600B1
 static CYTHON_INLINE PyObject *__Pyx_CallUnboundCMethod2(__Pyx_CachedCFunction *cfunc, PyObject *self, PyObject *arg1, PyObject *arg2);
 #else
 #define __Pyx_CallUnboundCMethod2(cfunc, self, arg1, arg2)  __Pyx__CallUnboundCMethod2(cfunc, self, arg1, arg2)
 #endif
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto_3_0_0b3
-#define __PYX_HAVE_RT_ImportType_proto_3_0_0b3
+#ifndef __PYX_HAVE_RT_ImportType_proto_3_0_0
+#define __PYX_HAVE_RT_ImportType_proto_3_0_0
 #if defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L
 #include <stdalign.h>
 #endif
 #if (defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L) || __cplusplus >= 201103L
-#define __PYX_GET_STRUCT_ALIGNMENT_3_0_0b3(s) alignof(s)
+#define __PYX_GET_STRUCT_ALIGNMENT_3_0_0(s) alignof(s)
 #else
-#define __PYX_GET_STRUCT_ALIGNMENT_3_0_0b3(s) sizeof(void*)
+#define __PYX_GET_STRUCT_ALIGNMENT_3_0_0(s) sizeof(void*)
 #endif
-enum __Pyx_ImportType_CheckSize_3_0_0b3 {
-   __Pyx_ImportType_CheckSize_Error_3_0_0b3 = 0,
-   __Pyx_ImportType_CheckSize_Warn_3_0_0b3 = 1,
-   __Pyx_ImportType_CheckSize_Ignore_3_0_0b3 = 2
+enum __Pyx_ImportType_CheckSize_3_0_0 {
+   __Pyx_ImportType_CheckSize_Error_3_0_0 = 0,
+   __Pyx_ImportType_CheckSize_Warn_3_0_0 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_3_0_0 = 2
 };
-static PyTypeObject *__Pyx_ImportType_3_0_0b3(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_0b3 check_size);
+static PyTypeObject *__Pyx_ImportType_3_0_0(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_0 check_size);
 #endif
 
 /* Import.proto */
 static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level);
 
 /* ImportFrom.proto */
 static PyObject* __Pyx_ImportFrom(PyObject* module, PyObject* name);
@@ -4172,17 +4183,17 @@
  *         s_proc.data = NULL
  */
     __Pyx_TraceLine(291,0,__PYX_ERR(1, 291, __pyx_L6_except_error))
     __pyx_t_13 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_13) {
       __Pyx_AddTraceback("cpp_common.hash_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_1, &__pyx_t_14, &__pyx_t_15) < 0) __PYX_ERR(1, 291, __pyx_L6_except_error)
-      __Pyx_GOTREF(__pyx_t_1);
-      __Pyx_GOTREF(__pyx_t_14);
-      __Pyx_GOTREF(__pyx_t_15);
+      __Pyx_XGOTREF(__pyx_t_1);
+      __Pyx_XGOTREF(__pyx_t_14);
+      __Pyx_XGOTREF(__pyx_t_15);
       __Pyx_INCREF(__pyx_t_14);
       __pyx_v_e = __pyx_t_14;
       /*try:*/ {
 
         /* "cpp_common.pxd":292
  *                 (<uint64_t*>s_proc.data)[i] = <uint64_t>hash(arr[i])
  *     except Exception as e:
@@ -4589,17 +4600,17 @@
  *         s_proc.data = NULL
  */
     __Pyx_TraceLine(320,0,__PYX_ERR(1, 320, __pyx_L6_except_error))
     __pyx_t_13 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_13) {
       __Pyx_AddTraceback("cpp_common.hash_sequence", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_9, &__pyx_t_14, &__pyx_t_15) < 0) __PYX_ERR(1, 320, __pyx_L6_except_error)
-      __Pyx_GOTREF(__pyx_t_9);
-      __Pyx_GOTREF(__pyx_t_14);
-      __Pyx_GOTREF(__pyx_t_15);
+      __Pyx_XGOTREF(__pyx_t_9);
+      __Pyx_XGOTREF(__pyx_t_14);
+      __Pyx_XGOTREF(__pyx_t_15);
       __Pyx_INCREF(__pyx_t_14);
       __pyx_v_e = __pyx_t_14;
       /*try:*/ {
 
         /* "cpp_common.pxd":321
  *                 (<uint64_t*>s_proc.data)[i] = <uint64_t>hash(elem)
  *     except Exception as e:
@@ -22363,29 +22374,29 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_3_0_0b3(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
+  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_3_0_0(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0b3(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(PyTypeObject),
   #elif CYTHON_COMPILING_IN_LIMITED_API
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0b3(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0b3(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(PyHeapTypeObject),
   #endif
-  __Pyx_ImportType_CheckSize_Warn_3_0_0b3); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(2, 9, __pyx_L1_error)
+  __Pyx_ImportType_CheckSize_Warn_3_0_0); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(2, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("rapidfuzz.distance._initialize_cpp"); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_9rapidfuzz_8distance_15_initialize_cpp_Editops = __Pyx_ImportType_3_0_0b3(__pyx_t_1, "rapidfuzz.distance._initialize_cpp", "Editops", sizeof(struct __pyx_obj_9rapidfuzz_8distance_15_initialize_cpp_Editops), __PYX_GET_STRUCT_ALIGNMENT_3_0_0b3(struct __pyx_obj_9rapidfuzz_8distance_15_initialize_cpp_Editops),__Pyx_ImportType_CheckSize_Warn_3_0_0b3); if (!__pyx_ptype_9rapidfuzz_8distance_15_initialize_cpp_Editops) __PYX_ERR(3, 9, __pyx_L1_error)
-  __pyx_ptype_9rapidfuzz_8distance_15_initialize_cpp_Opcodes = __Pyx_ImportType_3_0_0b3(__pyx_t_1, "rapidfuzz.distance._initialize_cpp", "Opcodes", sizeof(struct __pyx_obj_9rapidfuzz_8distance_15_initialize_cpp_Opcodes), __PYX_GET_STRUCT_ALIGNMENT_3_0_0b3(struct __pyx_obj_9rapidfuzz_8distance_15_initialize_cpp_Opcodes),__Pyx_ImportType_CheckSize_Warn_3_0_0b3); if (!__pyx_ptype_9rapidfuzz_8distance_15_initialize_cpp_Opcodes) __PYX_ERR(3, 12, __pyx_L1_error)
-  __pyx_ptype_9rapidfuzz_8distance_15_initialize_cpp_ScoreAlignment = __Pyx_ImportType_3_0_0b3(__pyx_t_1, "rapidfuzz.distance._initialize_cpp", "ScoreAlignment", sizeof(struct __pyx_obj_9rapidfuzz_8distance_15_initialize_cpp_ScoreAlignment), __PYX_GET_STRUCT_ALIGNMENT_3_0_0b3(struct __pyx_obj_9rapidfuzz_8distance_15_initialize_cpp_ScoreAlignment),__Pyx_ImportType_CheckSize_Warn_3_0_0b3); if (!__pyx_ptype_9rapidfuzz_8distance_15_initialize_cpp_ScoreAlignment) __PYX_ERR(3, 15, __pyx_L1_error)
+  __pyx_ptype_9rapidfuzz_8distance_15_initialize_cpp_Editops = __Pyx_ImportType_3_0_0(__pyx_t_1, "rapidfuzz.distance._initialize_cpp", "Editops", sizeof(struct __pyx_obj_9rapidfuzz_8distance_15_initialize_cpp_Editops), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(struct __pyx_obj_9rapidfuzz_8distance_15_initialize_cpp_Editops),__Pyx_ImportType_CheckSize_Warn_3_0_0); if (!__pyx_ptype_9rapidfuzz_8distance_15_initialize_cpp_Editops) __PYX_ERR(3, 9, __pyx_L1_error)
+  __pyx_ptype_9rapidfuzz_8distance_15_initialize_cpp_Opcodes = __Pyx_ImportType_3_0_0(__pyx_t_1, "rapidfuzz.distance._initialize_cpp", "Opcodes", sizeof(struct __pyx_obj_9rapidfuzz_8distance_15_initialize_cpp_Opcodes), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(struct __pyx_obj_9rapidfuzz_8distance_15_initialize_cpp_Opcodes),__Pyx_ImportType_CheckSize_Warn_3_0_0); if (!__pyx_ptype_9rapidfuzz_8distance_15_initialize_cpp_Opcodes) __PYX_ERR(3, 12, __pyx_L1_error)
+  __pyx_ptype_9rapidfuzz_8distance_15_initialize_cpp_ScoreAlignment = __Pyx_ImportType_3_0_0(__pyx_t_1, "rapidfuzz.distance._initialize_cpp", "ScoreAlignment", sizeof(struct __pyx_obj_9rapidfuzz_8distance_15_initialize_cpp_ScoreAlignment), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(struct __pyx_obj_9rapidfuzz_8distance_15_initialize_cpp_ScoreAlignment),__Pyx_ImportType_CheckSize_Warn_3_0_0); if (!__pyx_ptype_9rapidfuzz_8distance_15_initialize_cpp_ScoreAlignment) __PYX_ERR(3, 15, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -27559,18 +27570,18 @@
         else
             value = __Pyx_CallUnboundCMethod2(&__pyx_umethod_PyDict_Type_get, d, key, default_value);
     }
     return value;
 }
 
 /* TypeImport */
-#ifndef __PYX_HAVE_RT_ImportType_3_0_0b3
-#define __PYX_HAVE_RT_ImportType_3_0_0b3
-static PyTypeObject *__Pyx_ImportType_3_0_0b3(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_0b3 check_size)
+#ifndef __PYX_HAVE_RT_ImportType_3_0_0
+#define __PYX_HAVE_RT_ImportType_3_0_0
+static PyTypeObject *__Pyx_ImportType_3_0_0(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_0 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
     Py_ssize_t itemsize;
 #if CYTHON_COMPILING_IN_LIMITED_API
     PyObject *py_basicsize;
@@ -27616,23 +27627,23 @@
     if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize+itemsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error_3_0_0b3 &&
+    if (check_size == __Pyx_ImportType_CheckSize_Error_3_0_0 &&
             ((size_t)basicsize > size || (size_t)(basicsize + itemsize) < size)) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd-%zd from PyObject",
             module_name, class_name, size, basicsize, basicsize+itemsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn_3_0_0b3 && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_3_0_0 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
```

### Comparing `rapidfuzz-3.1.1/src/rapidfuzz/distance/metrics_cpp.pyi` & `rapidfuzz-3.1.2/src/rapidfuzz/distance/metrics_cpp.pyi`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/src/rapidfuzz/distance/metrics_cpp.pyx` & `rapidfuzz-3.1.2/src/rapidfuzz/distance/metrics_cpp.pyx`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/src/rapidfuzz/distance/metrics_cpp_avx2.cxx` & `rapidfuzz-3.1.2/src/rapidfuzz/distance/metrics_cpp_avx2.cxx`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 3.0.0b3 */
+/* Generated by Cython 3.0.0 */
 
 #ifndef PY_SSIZE_T_CLEAN
 #define PY_SSIZE_T_CLEAN
 #endif /* PY_SSIZE_T_CLEAN */
 #if defined(CYTHON_LIMITED_API) && 0
   #ifndef Py_LIMITED_API
     #if CYTHON_LIMITED_API+0 > 0x03030000
@@ -15,18 +15,18 @@
 
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02070000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.7+ or Python 3.3+.
 #else
-#define CYTHON_ABI "3_0_0b3"
+#define CYTHON_ABI "3_0_0"
 #define __PYX_ABI_MODULE_NAME "_cython_" CYTHON_ABI
 #define __PYX_TYPE_MODULE_PREFIX __PYX_ABI_MODULE_NAME "."
-#define CYTHON_HEX_VERSION 0x030000B3
+#define CYTHON_HEX_VERSION 0x030000F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(_WIN32) && !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -641,14 +641,19 @@
 #endif
 #if PY_VERSION_HEX >= 0x030A00B1 || defined(Py_IsFalse)
   #define __Pyx_Py_IsFalse(ob) Py_IsFalse(ob)
 #else
   #define __Pyx_Py_IsFalse(ob) __Pyx_Py_Is((ob), Py_False)
 #endif
 #define __Pyx_NoneAsNull(obj)  (__Pyx_Py_IsNone(obj) ? NULL : (obj))
+#if PY_VERSION_HEX >= 0x030900F0 && !CYTHON_COMPILING_IN_PYPY
+  #define __Pyx_PyObject_GC_IsFinalized(o) PyObject_GC_IsFinalized(o)
+#else
+  #define __Pyx_PyObject_GC_IsFinalized(o) _PyGC_FINALIZED(o)
+#endif
 #ifndef CO_COROUTINE
   #define CO_COROUTINE 0x80
 #endif
 #ifndef CO_ASYNC_GENERATOR
   #define CO_ASYNC_GENERATOR 0x200
 #endif
 #ifndef Py_TPFLAGS_CHECKTYPES
@@ -885,15 +890,15 @@
   #endif
   #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GET_LENGTH(u)
   #define __Pyx_PyUnicode_READ_CHAR(u, i) PyUnicode_READ_CHAR(u, i)
   #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   PyUnicode_MAX_CHAR_VALUE(u)
   #define __Pyx_PyUnicode_KIND(u)         ((int)PyUnicode_KIND(u))
   #define __Pyx_PyUnicode_DATA(u)         PyUnicode_DATA(u)
   #define __Pyx_PyUnicode_READ(k, d, i)   PyUnicode_READ(k, d, i)
-  #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  PyUnicode_WRITE(k, d, i, ch)
+  #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  PyUnicode_WRITE(k, d, i, (Py_UCS4) ch)
   #if PY_VERSION_HEX >= 0x030C0000
     #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
   #else
     #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
     #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
     #else
     #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
@@ -907,15 +912,15 @@
   #define __Pyx_PyUnicode_READY(op)       (0)
   #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GET_SIZE(u)
   #define __Pyx_PyUnicode_READ_CHAR(u, i) ((Py_UCS4)(PyUnicode_AS_UNICODE(u)[i]))
   #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   ((sizeof(Py_UNICODE) == 2) ? 65535U : 1114111U)
   #define __Pyx_PyUnicode_KIND(u)         ((int)sizeof(Py_UNICODE))
   #define __Pyx_PyUnicode_DATA(u)         ((void*)PyUnicode_AS_UNICODE(u))
   #define __Pyx_PyUnicode_READ(k, d, i)   ((void)(k), (Py_UCS4)(((Py_UNICODE*)d)[i]))
-  #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  (((void)(k)), ((Py_UNICODE*)d)[i] = ch)
+  #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  (((void)(k)), ((Py_UNICODE*)d)[i] = (Py_UNICODE) ch)
   #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_SIZE(u))
 #endif
 #if CYTHON_COMPILING_IN_PYPY
   #define __Pyx_PyUnicode_Concat(a, b)      PyNumber_Add(a, b)
   #define __Pyx_PyUnicode_ConcatSafe(a, b)  PyNumber_Add(a, b)
 #else
   #define __Pyx_PyUnicode_Concat(a, b)      PyUnicode_Concat(a, b)
@@ -1240,20 +1245,20 @@
   #endif
   #define __Pyx_PyLong_Sign(x)  (((PyLongObject*)x)->long_value.lv_tag & _PyLong_SIGN_MASK)
   #define __Pyx_PyLong_IsNeg(x)  ((__Pyx_PyLong_Sign(x) & 2) != 0)
   #define __Pyx_PyLong_IsNonNeg(x)  (!__Pyx_PyLong_IsNeg(x))
   #define __Pyx_PyLong_IsZero(x)  (__Pyx_PyLong_Sign(x) & 1)
   #define __Pyx_PyLong_IsPos(x)  (__Pyx_PyLong_Sign(x) == 0)
   #define __Pyx_PyLong_CompactValueUnsigned(x)  (__Pyx_PyLong_Digits(x)[0])
-  #define __Pyx_PyLong_DigitCount(x)  (((PyLongObject*)x)->long_value.lv_tag >> _PyLong_NON_SIZE_BITS)
+  #define __Pyx_PyLong_DigitCount(x)  ((Py_ssize_t) (((PyLongObject*)x)->long_value.lv_tag >> _PyLong_NON_SIZE_BITS))
   #define __Pyx_PyLong_SignedDigitCount(x)\
-        ((1 - (Py_ssize_t) __Pyx_PyLong_Sign(x)) * (Py_ssize_t) __Pyx_PyLong_DigitCount(x))
+        ((1 - (Py_ssize_t) __Pyx_PyLong_Sign(x)) * __Pyx_PyLong_DigitCount(x))
   #if defined(PyUnstable_Long_IsCompact) && defined(PyUnstable_Long_CompactValue)
-    #define __Pyx_PyLong_IsCompact(x)     PyUnstable_Long_IsCompact(x)
-    #define __Pyx_PyLong_CompactValue(x)  PyUnstable_Long_CompactValue(x)
+    #define __Pyx_PyLong_IsCompact(x)     PyUnstable_Long_IsCompact((PyLongObject*) x)
+    #define __Pyx_PyLong_CompactValue(x)  PyUnstable_Long_CompactValue((PyLongObject*) x)
   #else
     #define __Pyx_PyLong_IsCompact(x)     (((PyLongObject*)x)->long_value.lv_tag < (2 << _PyLong_NON_SIZE_BITS))
     #define __Pyx_PyLong_CompactValue(x)  ((1 - (Py_ssize_t) __Pyx_PyLong_Sign(x)) * (Py_ssize_t) __Pyx_PyLong_Digits(x)[0])
   #endif
   typedef Py_ssize_t  __Pyx_compact_pylong;
   typedef size_t  __Pyx_compact_upylong;
   #else  // Py < 3.12
@@ -1293,15 +1298,15 @@
     if (!default_encoding_c) goto bad;
     if (strcmp(default_encoding_c, "ascii") == 0) {
         __Pyx_sys_getdefaultencoding_not_ascii = 0;
     } else {
         char ascii_chars[128];
         int c;
         for (c = 0; c < 128; c++) {
-            ascii_chars[c] = c;
+            ascii_chars[c] = (char) c;
         }
         __Pyx_sys_getdefaultencoding_not_ascii = 1;
         ascii_chars_u = PyUnicode_DecodeASCII(ascii_chars, 128, NULL);
         if (!ascii_chars_u) goto bad;
         ascii_chars_b = PyUnicode_AsEncodedString(ascii_chars_u, default_encoding_c, NULL);
         if (!ascii_chars_b || !PyBytes_Check(ascii_chars_b) || memcmp(ascii_chars, PyBytes_AS_STRING(ascii_chars_b), 128) != 0) {
             PyErr_Format(
@@ -1633,20 +1638,26 @@
   #define __Pyx_TraceDeclarations\
       static PyCodeObject *__pyx_frame_code = NULL;\
       CYTHON_FRAME_MODIFIER PyFrameObject *__pyx_frame = NULL;\
       int __Pyx_use_tracing = 0;
   #define __Pyx_TraceFrameInit(codeobj)\
       if (codeobj) __pyx_frame_code = (PyCodeObject*) codeobj;
 #if PY_VERSION_HEX >= 0x030b00a2
+  #if PY_VERSION_HEX >= 0x030C00b1
+  #define __Pyx_IsTracing(tstate, check_tracing, check_funcs)\
+     ((!(check_tracing) || !(tstate)->tracing) &&\
+         (!(check_funcs) || (tstate)->c_profilefunc || (CYTHON_TRACE && (tstate)->c_tracefunc)))
+  #else
   #define __Pyx_IsTracing(tstate, check_tracing, check_funcs)\
      (unlikely((tstate)->cframe->use_tracing) &&\
          (!(check_tracing) || !(tstate)->tracing) &&\
          (!(check_funcs) || (tstate)->c_profilefunc || (CYTHON_TRACE && (tstate)->c_tracefunc)))
-  #define __Pyx_EnterTracing(tstate) PyThreadState_EnterTracing(tstate)
-  #define __Pyx_LeaveTracing(tstate) PyThreadState_LeaveTracing(tstate)
+  #endif
+  #define __Pyx_EnterTracing(tstate)  PyThreadState_EnterTracing(tstate)
+  #define __Pyx_LeaveTracing(tstate)  PyThreadState_LeaveTracing(tstate)
 #elif PY_VERSION_HEX >= 0x030a00b1
   #define __Pyx_IsTracing(tstate, check_tracing, check_funcs)\
      (unlikely((tstate)->cframe->use_tracing) &&\
          (!(check_tracing) || !(tstate)->tracing) &&\
          (!(check_funcs) || (tstate)->c_profilefunc || (CYTHON_TRACE && (tstate)->c_tracefunc)))
   #define __Pyx_EnterTracing(tstate)\
       do { tstate->tracing++; tstate->cframe->use_tracing = 0; } while (0)
@@ -2161,30 +2172,30 @@
 #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030600B1
 static CYTHON_INLINE PyObject *__Pyx_CallUnboundCMethod2(__Pyx_CachedCFunction *cfunc, PyObject *self, PyObject *arg1, PyObject *arg2);
 #else
 #define __Pyx_CallUnboundCMethod2(cfunc, self, arg1, arg2)  __Pyx__CallUnboundCMethod2(cfunc, self, arg1, arg2)
 #endif
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto_3_0_0b3
-#define __PYX_HAVE_RT_ImportType_proto_3_0_0b3
+#ifndef __PYX_HAVE_RT_ImportType_proto_3_0_0
+#define __PYX_HAVE_RT_ImportType_proto_3_0_0
 #if defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L
 #include <stdalign.h>
 #endif
 #if (defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L) || __cplusplus >= 201103L
-#define __PYX_GET_STRUCT_ALIGNMENT_3_0_0b3(s) alignof(s)
+#define __PYX_GET_STRUCT_ALIGNMENT_3_0_0(s) alignof(s)
 #else
-#define __PYX_GET_STRUCT_ALIGNMENT_3_0_0b3(s) sizeof(void*)
+#define __PYX_GET_STRUCT_ALIGNMENT_3_0_0(s) sizeof(void*)
 #endif
-enum __Pyx_ImportType_CheckSize_3_0_0b3 {
-   __Pyx_ImportType_CheckSize_Error_3_0_0b3 = 0,
-   __Pyx_ImportType_CheckSize_Warn_3_0_0b3 = 1,
-   __Pyx_ImportType_CheckSize_Ignore_3_0_0b3 = 2
+enum __Pyx_ImportType_CheckSize_3_0_0 {
+   __Pyx_ImportType_CheckSize_Error_3_0_0 = 0,
+   __Pyx_ImportType_CheckSize_Warn_3_0_0 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_3_0_0 = 2
 };
-static PyTypeObject *__Pyx_ImportType_3_0_0b3(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_0b3 check_size);
+static PyTypeObject *__Pyx_ImportType_3_0_0(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_0 check_size);
 #endif
 
 /* Import.proto */
 static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level);
 
 /* ImportFrom.proto */
 static PyObject* __Pyx_ImportFrom(PyObject* module, PyObject* name);
@@ -4173,17 +4184,17 @@
  *         s_proc.data = NULL
  */
     __Pyx_TraceLine(291,0,__PYX_ERR(1, 291, __pyx_L6_except_error))
     __pyx_t_13 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_13) {
       __Pyx_AddTraceback("cpp_common.hash_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_1, &__pyx_t_14, &__pyx_t_15) < 0) __PYX_ERR(1, 291, __pyx_L6_except_error)
-      __Pyx_GOTREF(__pyx_t_1);
-      __Pyx_GOTREF(__pyx_t_14);
-      __Pyx_GOTREF(__pyx_t_15);
+      __Pyx_XGOTREF(__pyx_t_1);
+      __Pyx_XGOTREF(__pyx_t_14);
+      __Pyx_XGOTREF(__pyx_t_15);
       __Pyx_INCREF(__pyx_t_14);
       __pyx_v_e = __pyx_t_14;
       /*try:*/ {
 
         /* "cpp_common.pxd":292
  *                 (<uint64_t*>s_proc.data)[i] = <uint64_t>hash(arr[i])
  *     except Exception as e:
@@ -4590,17 +4601,17 @@
  *         s_proc.data = NULL
  */
     __Pyx_TraceLine(320,0,__PYX_ERR(1, 320, __pyx_L6_except_error))
     __pyx_t_13 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_13) {
       __Pyx_AddTraceback("cpp_common.hash_sequence", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_9, &__pyx_t_14, &__pyx_t_15) < 0) __PYX_ERR(1, 320, __pyx_L6_except_error)
-      __Pyx_GOTREF(__pyx_t_9);
-      __Pyx_GOTREF(__pyx_t_14);
-      __Pyx_GOTREF(__pyx_t_15);
+      __Pyx_XGOTREF(__pyx_t_9);
+      __Pyx_XGOTREF(__pyx_t_14);
+      __Pyx_XGOTREF(__pyx_t_15);
       __Pyx_INCREF(__pyx_t_14);
       __pyx_v_e = __pyx_t_14;
       /*try:*/ {
 
         /* "cpp_common.pxd":321
  *                 (<uint64_t*>s_proc.data)[i] = <uint64_t>hash(elem)
  *     except Exception as e:
@@ -22364,29 +22375,29 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_3_0_0b3(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
+  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_3_0_0(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0b3(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(PyTypeObject),
   #elif CYTHON_COMPILING_IN_LIMITED_API
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0b3(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0b3(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(PyHeapTypeObject),
   #endif
-  __Pyx_ImportType_CheckSize_Warn_3_0_0b3); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
+  __Pyx_ImportType_CheckSize_Warn_3_0_0); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("rapidfuzz.distance._initialize_cpp"); if (unlikely(!__pyx_t_1)) __PYX_ERR(4, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_9rapidfuzz_8distance_15_initialize_cpp_Editops = __Pyx_ImportType_3_0_0b3(__pyx_t_1, "rapidfuzz.distance._initialize_cpp", "Editops", sizeof(struct __pyx_obj_9rapidfuzz_8distance_15_initialize_cpp_Editops), __PYX_GET_STRUCT_ALIGNMENT_3_0_0b3(struct __pyx_obj_9rapidfuzz_8distance_15_initialize_cpp_Editops),__Pyx_ImportType_CheckSize_Warn_3_0_0b3); if (!__pyx_ptype_9rapidfuzz_8distance_15_initialize_cpp_Editops) __PYX_ERR(4, 9, __pyx_L1_error)
-  __pyx_ptype_9rapidfuzz_8distance_15_initialize_cpp_Opcodes = __Pyx_ImportType_3_0_0b3(__pyx_t_1, "rapidfuzz.distance._initialize_cpp", "Opcodes", sizeof(struct __pyx_obj_9rapidfuzz_8distance_15_initialize_cpp_Opcodes), __PYX_GET_STRUCT_ALIGNMENT_3_0_0b3(struct __pyx_obj_9rapidfuzz_8distance_15_initialize_cpp_Opcodes),__Pyx_ImportType_CheckSize_Warn_3_0_0b3); if (!__pyx_ptype_9rapidfuzz_8distance_15_initialize_cpp_Opcodes) __PYX_ERR(4, 12, __pyx_L1_error)
-  __pyx_ptype_9rapidfuzz_8distance_15_initialize_cpp_ScoreAlignment = __Pyx_ImportType_3_0_0b3(__pyx_t_1, "rapidfuzz.distance._initialize_cpp", "ScoreAlignment", sizeof(struct __pyx_obj_9rapidfuzz_8distance_15_initialize_cpp_ScoreAlignment), __PYX_GET_STRUCT_ALIGNMENT_3_0_0b3(struct __pyx_obj_9rapidfuzz_8distance_15_initialize_cpp_ScoreAlignment),__Pyx_ImportType_CheckSize_Warn_3_0_0b3); if (!__pyx_ptype_9rapidfuzz_8distance_15_initialize_cpp_ScoreAlignment) __PYX_ERR(4, 15, __pyx_L1_error)
+  __pyx_ptype_9rapidfuzz_8distance_15_initialize_cpp_Editops = __Pyx_ImportType_3_0_0(__pyx_t_1, "rapidfuzz.distance._initialize_cpp", "Editops", sizeof(struct __pyx_obj_9rapidfuzz_8distance_15_initialize_cpp_Editops), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(struct __pyx_obj_9rapidfuzz_8distance_15_initialize_cpp_Editops),__Pyx_ImportType_CheckSize_Warn_3_0_0); if (!__pyx_ptype_9rapidfuzz_8distance_15_initialize_cpp_Editops) __PYX_ERR(4, 9, __pyx_L1_error)
+  __pyx_ptype_9rapidfuzz_8distance_15_initialize_cpp_Opcodes = __Pyx_ImportType_3_0_0(__pyx_t_1, "rapidfuzz.distance._initialize_cpp", "Opcodes", sizeof(struct __pyx_obj_9rapidfuzz_8distance_15_initialize_cpp_Opcodes), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(struct __pyx_obj_9rapidfuzz_8distance_15_initialize_cpp_Opcodes),__Pyx_ImportType_CheckSize_Warn_3_0_0); if (!__pyx_ptype_9rapidfuzz_8distance_15_initialize_cpp_Opcodes) __PYX_ERR(4, 12, __pyx_L1_error)
+  __pyx_ptype_9rapidfuzz_8distance_15_initialize_cpp_ScoreAlignment = __Pyx_ImportType_3_0_0(__pyx_t_1, "rapidfuzz.distance._initialize_cpp", "ScoreAlignment", sizeof(struct __pyx_obj_9rapidfuzz_8distance_15_initialize_cpp_ScoreAlignment), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(struct __pyx_obj_9rapidfuzz_8distance_15_initialize_cpp_ScoreAlignment),__Pyx_ImportType_CheckSize_Warn_3_0_0); if (!__pyx_ptype_9rapidfuzz_8distance_15_initialize_cpp_ScoreAlignment) __PYX_ERR(4, 15, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -27560,18 +27571,18 @@
         else
             value = __Pyx_CallUnboundCMethod2(&__pyx_umethod_PyDict_Type_get, d, key, default_value);
     }
     return value;
 }
 
 /* TypeImport */
-#ifndef __PYX_HAVE_RT_ImportType_3_0_0b3
-#define __PYX_HAVE_RT_ImportType_3_0_0b3
-static PyTypeObject *__Pyx_ImportType_3_0_0b3(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_0b3 check_size)
+#ifndef __PYX_HAVE_RT_ImportType_3_0_0
+#define __PYX_HAVE_RT_ImportType_3_0_0
+static PyTypeObject *__Pyx_ImportType_3_0_0(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_0 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
     Py_ssize_t itemsize;
 #if CYTHON_COMPILING_IN_LIMITED_API
     PyObject *py_basicsize;
@@ -27617,23 +27628,23 @@
     if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize+itemsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error_3_0_0b3 &&
+    if (check_size == __Pyx_ImportType_CheckSize_Error_3_0_0 &&
             ((size_t)basicsize > size || (size_t)(basicsize + itemsize) < size)) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd-%zd from PyObject",
             module_name, class_name, size, basicsize, basicsize+itemsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn_3_0_0b3 && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_3_0_0 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
```

### Comparing `rapidfuzz-3.1.1/src/rapidfuzz/distance/metrics_py.py` & `rapidfuzz-3.1.2/src/rapidfuzz/distance/metrics_py.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/src/rapidfuzz/fuzz.py` & `rapidfuzz-3.1.2/src/rapidfuzz/fuzz.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/src/rapidfuzz/fuzz.pyi` & `rapidfuzz-3.1.2/src/rapidfuzz/fuzz.pyi`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/src/rapidfuzz/fuzz_cpp.cxx` & `rapidfuzz-3.1.2/src/rapidfuzz/fuzz_cpp.cxx`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 3.0.0b3 */
+/* Generated by Cython 3.0.0 */
 
 #ifndef PY_SSIZE_T_CLEAN
 #define PY_SSIZE_T_CLEAN
 #endif /* PY_SSIZE_T_CLEAN */
 #if defined(CYTHON_LIMITED_API) && 0
   #ifndef Py_LIMITED_API
     #if CYTHON_LIMITED_API+0 > 0x03030000
@@ -15,18 +15,18 @@
 
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02070000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.7+ or Python 3.3+.
 #else
-#define CYTHON_ABI "3_0_0b3"
+#define CYTHON_ABI "3_0_0"
 #define __PYX_ABI_MODULE_NAME "_cython_" CYTHON_ABI
 #define __PYX_TYPE_MODULE_PREFIX __PYX_ABI_MODULE_NAME "."
-#define CYTHON_HEX_VERSION 0x030000B3
+#define CYTHON_HEX_VERSION 0x030000F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(_WIN32) && !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -641,14 +641,19 @@
 #endif
 #if PY_VERSION_HEX >= 0x030A00B1 || defined(Py_IsFalse)
   #define __Pyx_Py_IsFalse(ob) Py_IsFalse(ob)
 #else
   #define __Pyx_Py_IsFalse(ob) __Pyx_Py_Is((ob), Py_False)
 #endif
 #define __Pyx_NoneAsNull(obj)  (__Pyx_Py_IsNone(obj) ? NULL : (obj))
+#if PY_VERSION_HEX >= 0x030900F0 && !CYTHON_COMPILING_IN_PYPY
+  #define __Pyx_PyObject_GC_IsFinalized(o) PyObject_GC_IsFinalized(o)
+#else
+  #define __Pyx_PyObject_GC_IsFinalized(o) _PyGC_FINALIZED(o)
+#endif
 #ifndef CO_COROUTINE
   #define CO_COROUTINE 0x80
 #endif
 #ifndef CO_ASYNC_GENERATOR
   #define CO_ASYNC_GENERATOR 0x200
 #endif
 #ifndef Py_TPFLAGS_CHECKTYPES
@@ -885,15 +890,15 @@
   #endif
   #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GET_LENGTH(u)
   #define __Pyx_PyUnicode_READ_CHAR(u, i) PyUnicode_READ_CHAR(u, i)
   #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   PyUnicode_MAX_CHAR_VALUE(u)
   #define __Pyx_PyUnicode_KIND(u)         ((int)PyUnicode_KIND(u))
   #define __Pyx_PyUnicode_DATA(u)         PyUnicode_DATA(u)
   #define __Pyx_PyUnicode_READ(k, d, i)   PyUnicode_READ(k, d, i)
-  #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  PyUnicode_WRITE(k, d, i, ch)
+  #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  PyUnicode_WRITE(k, d, i, (Py_UCS4) ch)
   #if PY_VERSION_HEX >= 0x030C0000
     #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
   #else
     #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
     #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
     #else
     #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
@@ -907,15 +912,15 @@
   #define __Pyx_PyUnicode_READY(op)       (0)
   #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GET_SIZE(u)
   #define __Pyx_PyUnicode_READ_CHAR(u, i) ((Py_UCS4)(PyUnicode_AS_UNICODE(u)[i]))
   #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   ((sizeof(Py_UNICODE) == 2) ? 65535U : 1114111U)
   #define __Pyx_PyUnicode_KIND(u)         ((int)sizeof(Py_UNICODE))
   #define __Pyx_PyUnicode_DATA(u)         ((void*)PyUnicode_AS_UNICODE(u))
   #define __Pyx_PyUnicode_READ(k, d, i)   ((void)(k), (Py_UCS4)(((Py_UNICODE*)d)[i]))
-  #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  (((void)(k)), ((Py_UNICODE*)d)[i] = ch)
+  #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  (((void)(k)), ((Py_UNICODE*)d)[i] = (Py_UNICODE) ch)
   #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_SIZE(u))
 #endif
 #if CYTHON_COMPILING_IN_PYPY
   #define __Pyx_PyUnicode_Concat(a, b)      PyNumber_Add(a, b)
   #define __Pyx_PyUnicode_ConcatSafe(a, b)  PyNumber_Add(a, b)
 #else
   #define __Pyx_PyUnicode_Concat(a, b)      PyUnicode_Concat(a, b)
@@ -1240,20 +1245,20 @@
   #endif
   #define __Pyx_PyLong_Sign(x)  (((PyLongObject*)x)->long_value.lv_tag & _PyLong_SIGN_MASK)
   #define __Pyx_PyLong_IsNeg(x)  ((__Pyx_PyLong_Sign(x) & 2) != 0)
   #define __Pyx_PyLong_IsNonNeg(x)  (!__Pyx_PyLong_IsNeg(x))
   #define __Pyx_PyLong_IsZero(x)  (__Pyx_PyLong_Sign(x) & 1)
   #define __Pyx_PyLong_IsPos(x)  (__Pyx_PyLong_Sign(x) == 0)
   #define __Pyx_PyLong_CompactValueUnsigned(x)  (__Pyx_PyLong_Digits(x)[0])
-  #define __Pyx_PyLong_DigitCount(x)  (((PyLongObject*)x)->long_value.lv_tag >> _PyLong_NON_SIZE_BITS)
+  #define __Pyx_PyLong_DigitCount(x)  ((Py_ssize_t) (((PyLongObject*)x)->long_value.lv_tag >> _PyLong_NON_SIZE_BITS))
   #define __Pyx_PyLong_SignedDigitCount(x)\
-        ((1 - (Py_ssize_t) __Pyx_PyLong_Sign(x)) * (Py_ssize_t) __Pyx_PyLong_DigitCount(x))
+        ((1 - (Py_ssize_t) __Pyx_PyLong_Sign(x)) * __Pyx_PyLong_DigitCount(x))
   #if defined(PyUnstable_Long_IsCompact) && defined(PyUnstable_Long_CompactValue)
-    #define __Pyx_PyLong_IsCompact(x)     PyUnstable_Long_IsCompact(x)
-    #define __Pyx_PyLong_CompactValue(x)  PyUnstable_Long_CompactValue(x)
+    #define __Pyx_PyLong_IsCompact(x)     PyUnstable_Long_IsCompact((PyLongObject*) x)
+    #define __Pyx_PyLong_CompactValue(x)  PyUnstable_Long_CompactValue((PyLongObject*) x)
   #else
     #define __Pyx_PyLong_IsCompact(x)     (((PyLongObject*)x)->long_value.lv_tag < (2 << _PyLong_NON_SIZE_BITS))
     #define __Pyx_PyLong_CompactValue(x)  ((1 - (Py_ssize_t) __Pyx_PyLong_Sign(x)) * (Py_ssize_t) __Pyx_PyLong_Digits(x)[0])
   #endif
   typedef Py_ssize_t  __Pyx_compact_pylong;
   typedef size_t  __Pyx_compact_upylong;
   #else  // Py < 3.12
@@ -1293,15 +1298,15 @@
     if (!default_encoding_c) goto bad;
     if (strcmp(default_encoding_c, "ascii") == 0) {
         __Pyx_sys_getdefaultencoding_not_ascii = 0;
     } else {
         char ascii_chars[128];
         int c;
         for (c = 0; c < 128; c++) {
-            ascii_chars[c] = c;
+            ascii_chars[c] = (char) c;
         }
         __Pyx_sys_getdefaultencoding_not_ascii = 1;
         ascii_chars_u = PyUnicode_DecodeASCII(ascii_chars, 128, NULL);
         if (!ascii_chars_u) goto bad;
         ascii_chars_b = PyUnicode_AsEncodedString(ascii_chars_u, default_encoding_c, NULL);
         if (!ascii_chars_b || !PyBytes_Check(ascii_chars_b) || memcmp(ascii_chars, PyBytes_AS_STRING(ascii_chars_b), 128) != 0) {
             PyErr_Format(
@@ -1564,20 +1569,26 @@
   #define __Pyx_TraceDeclarations\
       static PyCodeObject *__pyx_frame_code = NULL;\
       CYTHON_FRAME_MODIFIER PyFrameObject *__pyx_frame = NULL;\
       int __Pyx_use_tracing = 0;
   #define __Pyx_TraceFrameInit(codeobj)\
       if (codeobj) __pyx_frame_code = (PyCodeObject*) codeobj;
 #if PY_VERSION_HEX >= 0x030b00a2
+  #if PY_VERSION_HEX >= 0x030C00b1
+  #define __Pyx_IsTracing(tstate, check_tracing, check_funcs)\
+     ((!(check_tracing) || !(tstate)->tracing) &&\
+         (!(check_funcs) || (tstate)->c_profilefunc || (CYTHON_TRACE && (tstate)->c_tracefunc)))
+  #else
   #define __Pyx_IsTracing(tstate, check_tracing, check_funcs)\
      (unlikely((tstate)->cframe->use_tracing) &&\
          (!(check_tracing) || !(tstate)->tracing) &&\
          (!(check_funcs) || (tstate)->c_profilefunc || (CYTHON_TRACE && (tstate)->c_tracefunc)))
-  #define __Pyx_EnterTracing(tstate) PyThreadState_EnterTracing(tstate)
-  #define __Pyx_LeaveTracing(tstate) PyThreadState_LeaveTracing(tstate)
+  #endif
+  #define __Pyx_EnterTracing(tstate)  PyThreadState_EnterTracing(tstate)
+  #define __Pyx_LeaveTracing(tstate)  PyThreadState_LeaveTracing(tstate)
 #elif PY_VERSION_HEX >= 0x030a00b1
   #define __Pyx_IsTracing(tstate, check_tracing, check_funcs)\
      (unlikely((tstate)->cframe->use_tracing) &&\
          (!(check_tracing) || !(tstate)->tracing) &&\
          (!(check_funcs) || (tstate)->c_profilefunc || (CYTHON_TRACE && (tstate)->c_tracefunc)))
   #define __Pyx_EnterTracing(tstate)\
       do { tstate->tracing++; tstate->cframe->use_tracing = 0; } while (0)
@@ -2068,30 +2079,30 @@
   #include <utility>
   #define __PYX_STD_MOVE_IF_SUPPORTED(x) std::move(x)
 #else
   #define __PYX_STD_MOVE_IF_SUPPORTED(x) x
 #endif
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto_3_0_0b3
-#define __PYX_HAVE_RT_ImportType_proto_3_0_0b3
+#ifndef __PYX_HAVE_RT_ImportType_proto_3_0_0
+#define __PYX_HAVE_RT_ImportType_proto_3_0_0
 #if defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L
 #include <stdalign.h>
 #endif
 #if (defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L) || __cplusplus >= 201103L
-#define __PYX_GET_STRUCT_ALIGNMENT_3_0_0b3(s) alignof(s)
+#define __PYX_GET_STRUCT_ALIGNMENT_3_0_0(s) alignof(s)
 #else
-#define __PYX_GET_STRUCT_ALIGNMENT_3_0_0b3(s) sizeof(void*)
+#define __PYX_GET_STRUCT_ALIGNMENT_3_0_0(s) sizeof(void*)
 #endif
-enum __Pyx_ImportType_CheckSize_3_0_0b3 {
-   __Pyx_ImportType_CheckSize_Error_3_0_0b3 = 0,
-   __Pyx_ImportType_CheckSize_Warn_3_0_0b3 = 1,
-   __Pyx_ImportType_CheckSize_Ignore_3_0_0b3 = 2
+enum __Pyx_ImportType_CheckSize_3_0_0 {
+   __Pyx_ImportType_CheckSize_Error_3_0_0 = 0,
+   __Pyx_ImportType_CheckSize_Warn_3_0_0 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_3_0_0 = 2
 };
-static PyTypeObject *__Pyx_ImportType_3_0_0b3(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_0b3 check_size);
+static PyTypeObject *__Pyx_ImportType_3_0_0(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_0 check_size);
 #endif
 
 /* Import.proto */
 static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level);
 
 /* ImportFrom.proto */
 static PyObject* __Pyx_ImportFrom(PyObject* module, PyObject* name);
@@ -3491,17 +3502,17 @@
  *         s_proc.data = NULL
  */
     __Pyx_TraceLine(291,0,__PYX_ERR(0, 291, __pyx_L6_except_error))
     __pyx_t_13 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_13) {
       __Pyx_AddTraceback("cpp_common.hash_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_1, &__pyx_t_14, &__pyx_t_15) < 0) __PYX_ERR(0, 291, __pyx_L6_except_error)
-      __Pyx_GOTREF(__pyx_t_1);
-      __Pyx_GOTREF(__pyx_t_14);
-      __Pyx_GOTREF(__pyx_t_15);
+      __Pyx_XGOTREF(__pyx_t_1);
+      __Pyx_XGOTREF(__pyx_t_14);
+      __Pyx_XGOTREF(__pyx_t_15);
       __Pyx_INCREF(__pyx_t_14);
       __pyx_v_e = __pyx_t_14;
       /*try:*/ {
 
         /* "cpp_common.pxd":292
  *                 (<uint64_t*>s_proc.data)[i] = <uint64_t>hash(arr[i])
  *     except Exception as e:
@@ -3908,17 +3919,17 @@
  *         s_proc.data = NULL
  */
     __Pyx_TraceLine(320,0,__PYX_ERR(0, 320, __pyx_L6_except_error))
     __pyx_t_13 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_13) {
       __Pyx_AddTraceback("cpp_common.hash_sequence", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_9, &__pyx_t_14, &__pyx_t_15) < 0) __PYX_ERR(0, 320, __pyx_L6_except_error)
-      __Pyx_GOTREF(__pyx_t_9);
-      __Pyx_GOTREF(__pyx_t_14);
-      __Pyx_GOTREF(__pyx_t_15);
+      __Pyx_XGOTREF(__pyx_t_9);
+      __Pyx_XGOTREF(__pyx_t_14);
+      __Pyx_XGOTREF(__pyx_t_15);
       __Pyx_INCREF(__pyx_t_14);
       __pyx_v_e = __pyx_t_14;
       /*try:*/ {
 
         /* "cpp_common.pxd":321
  *                 (<uint64_t*>s_proc.data)[i] = <uint64_t>hash(elem)
  *     except Exception as e:
@@ -8861,23 +8872,23 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_3_0_0b3(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
+  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_3_0_0(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0b3(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(PyTypeObject),
   #elif CYTHON_COMPILING_IN_LIMITED_API
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0b3(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0b3(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(PyHeapTypeObject),
   #endif
-  __Pyx_ImportType_CheckSize_Warn_3_0_0b3); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(2, 9, __pyx_L1_error)
+  __Pyx_ImportType_CheckSize_Warn_3_0_0); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(2, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -11693,18 +11704,18 @@
         function_name, key);
     #endif
 bad:
     return -1;
 }
 
 /* TypeImport */
-#ifndef __PYX_HAVE_RT_ImportType_3_0_0b3
-#define __PYX_HAVE_RT_ImportType_3_0_0b3
-static PyTypeObject *__Pyx_ImportType_3_0_0b3(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_0b3 check_size)
+#ifndef __PYX_HAVE_RT_ImportType_3_0_0
+#define __PYX_HAVE_RT_ImportType_3_0_0
+static PyTypeObject *__Pyx_ImportType_3_0_0(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_0 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
     Py_ssize_t itemsize;
 #if CYTHON_COMPILING_IN_LIMITED_API
     PyObject *py_basicsize;
@@ -11750,23 +11761,23 @@
     if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize+itemsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error_3_0_0b3 &&
+    if (check_size == __Pyx_ImportType_CheckSize_Error_3_0_0 &&
             ((size_t)basicsize > size || (size_t)(basicsize + itemsize) < size)) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd-%zd from PyObject",
             module_name, class_name, size, basicsize, basicsize+itemsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn_3_0_0b3 && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_3_0_0 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
```

### Comparing `rapidfuzz-3.1.1/src/rapidfuzz/fuzz_cpp.hpp` & `rapidfuzz-3.1.2/src/rapidfuzz/fuzz_cpp.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/src/rapidfuzz/fuzz_cpp.pyx` & `rapidfuzz-3.1.2/src/rapidfuzz/fuzz_cpp.pyx`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/src/rapidfuzz/fuzz_cpp_avx2.cxx` & `rapidfuzz-3.1.2/src/rapidfuzz/fuzz_cpp_avx2.cxx`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 3.0.0b3 */
+/* Generated by Cython 3.0.0 */
 
 #ifndef PY_SSIZE_T_CLEAN
 #define PY_SSIZE_T_CLEAN
 #endif /* PY_SSIZE_T_CLEAN */
 #if defined(CYTHON_LIMITED_API) && 0
   #ifndef Py_LIMITED_API
     #if CYTHON_LIMITED_API+0 > 0x03030000
@@ -15,18 +15,18 @@
 
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02070000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.7+ or Python 3.3+.
 #else
-#define CYTHON_ABI "3_0_0b3"
+#define CYTHON_ABI "3_0_0"
 #define __PYX_ABI_MODULE_NAME "_cython_" CYTHON_ABI
 #define __PYX_TYPE_MODULE_PREFIX __PYX_ABI_MODULE_NAME "."
-#define CYTHON_HEX_VERSION 0x030000B3
+#define CYTHON_HEX_VERSION 0x030000F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(_WIN32) && !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -641,14 +641,19 @@
 #endif
 #if PY_VERSION_HEX >= 0x030A00B1 || defined(Py_IsFalse)
   #define __Pyx_Py_IsFalse(ob) Py_IsFalse(ob)
 #else
   #define __Pyx_Py_IsFalse(ob) __Pyx_Py_Is((ob), Py_False)
 #endif
 #define __Pyx_NoneAsNull(obj)  (__Pyx_Py_IsNone(obj) ? NULL : (obj))
+#if PY_VERSION_HEX >= 0x030900F0 && !CYTHON_COMPILING_IN_PYPY
+  #define __Pyx_PyObject_GC_IsFinalized(o) PyObject_GC_IsFinalized(o)
+#else
+  #define __Pyx_PyObject_GC_IsFinalized(o) _PyGC_FINALIZED(o)
+#endif
 #ifndef CO_COROUTINE
   #define CO_COROUTINE 0x80
 #endif
 #ifndef CO_ASYNC_GENERATOR
   #define CO_ASYNC_GENERATOR 0x200
 #endif
 #ifndef Py_TPFLAGS_CHECKTYPES
@@ -885,15 +890,15 @@
   #endif
   #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GET_LENGTH(u)
   #define __Pyx_PyUnicode_READ_CHAR(u, i) PyUnicode_READ_CHAR(u, i)
   #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   PyUnicode_MAX_CHAR_VALUE(u)
   #define __Pyx_PyUnicode_KIND(u)         ((int)PyUnicode_KIND(u))
   #define __Pyx_PyUnicode_DATA(u)         PyUnicode_DATA(u)
   #define __Pyx_PyUnicode_READ(k, d, i)   PyUnicode_READ(k, d, i)
-  #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  PyUnicode_WRITE(k, d, i, ch)
+  #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  PyUnicode_WRITE(k, d, i, (Py_UCS4) ch)
   #if PY_VERSION_HEX >= 0x030C0000
     #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
   #else
     #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
     #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
     #else
     #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
@@ -907,15 +912,15 @@
   #define __Pyx_PyUnicode_READY(op)       (0)
   #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GET_SIZE(u)
   #define __Pyx_PyUnicode_READ_CHAR(u, i) ((Py_UCS4)(PyUnicode_AS_UNICODE(u)[i]))
   #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   ((sizeof(Py_UNICODE) == 2) ? 65535U : 1114111U)
   #define __Pyx_PyUnicode_KIND(u)         ((int)sizeof(Py_UNICODE))
   #define __Pyx_PyUnicode_DATA(u)         ((void*)PyUnicode_AS_UNICODE(u))
   #define __Pyx_PyUnicode_READ(k, d, i)   ((void)(k), (Py_UCS4)(((Py_UNICODE*)d)[i]))
-  #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  (((void)(k)), ((Py_UNICODE*)d)[i] = ch)
+  #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  (((void)(k)), ((Py_UNICODE*)d)[i] = (Py_UNICODE) ch)
   #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_SIZE(u))
 #endif
 #if CYTHON_COMPILING_IN_PYPY
   #define __Pyx_PyUnicode_Concat(a, b)      PyNumber_Add(a, b)
   #define __Pyx_PyUnicode_ConcatSafe(a, b)  PyNumber_Add(a, b)
 #else
   #define __Pyx_PyUnicode_Concat(a, b)      PyUnicode_Concat(a, b)
@@ -1240,20 +1245,20 @@
   #endif
   #define __Pyx_PyLong_Sign(x)  (((PyLongObject*)x)->long_value.lv_tag & _PyLong_SIGN_MASK)
   #define __Pyx_PyLong_IsNeg(x)  ((__Pyx_PyLong_Sign(x) & 2) != 0)
   #define __Pyx_PyLong_IsNonNeg(x)  (!__Pyx_PyLong_IsNeg(x))
   #define __Pyx_PyLong_IsZero(x)  (__Pyx_PyLong_Sign(x) & 1)
   #define __Pyx_PyLong_IsPos(x)  (__Pyx_PyLong_Sign(x) == 0)
   #define __Pyx_PyLong_CompactValueUnsigned(x)  (__Pyx_PyLong_Digits(x)[0])
-  #define __Pyx_PyLong_DigitCount(x)  (((PyLongObject*)x)->long_value.lv_tag >> _PyLong_NON_SIZE_BITS)
+  #define __Pyx_PyLong_DigitCount(x)  ((Py_ssize_t) (((PyLongObject*)x)->long_value.lv_tag >> _PyLong_NON_SIZE_BITS))
   #define __Pyx_PyLong_SignedDigitCount(x)\
-        ((1 - (Py_ssize_t) __Pyx_PyLong_Sign(x)) * (Py_ssize_t) __Pyx_PyLong_DigitCount(x))
+        ((1 - (Py_ssize_t) __Pyx_PyLong_Sign(x)) * __Pyx_PyLong_DigitCount(x))
   #if defined(PyUnstable_Long_IsCompact) && defined(PyUnstable_Long_CompactValue)
-    #define __Pyx_PyLong_IsCompact(x)     PyUnstable_Long_IsCompact(x)
-    #define __Pyx_PyLong_CompactValue(x)  PyUnstable_Long_CompactValue(x)
+    #define __Pyx_PyLong_IsCompact(x)     PyUnstable_Long_IsCompact((PyLongObject*) x)
+    #define __Pyx_PyLong_CompactValue(x)  PyUnstable_Long_CompactValue((PyLongObject*) x)
   #else
     #define __Pyx_PyLong_IsCompact(x)     (((PyLongObject*)x)->long_value.lv_tag < (2 << _PyLong_NON_SIZE_BITS))
     #define __Pyx_PyLong_CompactValue(x)  ((1 - (Py_ssize_t) __Pyx_PyLong_Sign(x)) * (Py_ssize_t) __Pyx_PyLong_Digits(x)[0])
   #endif
   typedef Py_ssize_t  __Pyx_compact_pylong;
   typedef size_t  __Pyx_compact_upylong;
   #else  // Py < 3.12
@@ -1293,15 +1298,15 @@
     if (!default_encoding_c) goto bad;
     if (strcmp(default_encoding_c, "ascii") == 0) {
         __Pyx_sys_getdefaultencoding_not_ascii = 0;
     } else {
         char ascii_chars[128];
         int c;
         for (c = 0; c < 128; c++) {
-            ascii_chars[c] = c;
+            ascii_chars[c] = (char) c;
         }
         __Pyx_sys_getdefaultencoding_not_ascii = 1;
         ascii_chars_u = PyUnicode_DecodeASCII(ascii_chars, 128, NULL);
         if (!ascii_chars_u) goto bad;
         ascii_chars_b = PyUnicode_AsEncodedString(ascii_chars_u, default_encoding_c, NULL);
         if (!ascii_chars_b || !PyBytes_Check(ascii_chars_b) || memcmp(ascii_chars, PyBytes_AS_STRING(ascii_chars_b), 128) != 0) {
             PyErr_Format(
@@ -1565,20 +1570,26 @@
   #define __Pyx_TraceDeclarations\
       static PyCodeObject *__pyx_frame_code = NULL;\
       CYTHON_FRAME_MODIFIER PyFrameObject *__pyx_frame = NULL;\
       int __Pyx_use_tracing = 0;
   #define __Pyx_TraceFrameInit(codeobj)\
       if (codeobj) __pyx_frame_code = (PyCodeObject*) codeobj;
 #if PY_VERSION_HEX >= 0x030b00a2
+  #if PY_VERSION_HEX >= 0x030C00b1
+  #define __Pyx_IsTracing(tstate, check_tracing, check_funcs)\
+     ((!(check_tracing) || !(tstate)->tracing) &&\
+         (!(check_funcs) || (tstate)->c_profilefunc || (CYTHON_TRACE && (tstate)->c_tracefunc)))
+  #else
   #define __Pyx_IsTracing(tstate, check_tracing, check_funcs)\
      (unlikely((tstate)->cframe->use_tracing) &&\
          (!(check_tracing) || !(tstate)->tracing) &&\
          (!(check_funcs) || (tstate)->c_profilefunc || (CYTHON_TRACE && (tstate)->c_tracefunc)))
-  #define __Pyx_EnterTracing(tstate) PyThreadState_EnterTracing(tstate)
-  #define __Pyx_LeaveTracing(tstate) PyThreadState_LeaveTracing(tstate)
+  #endif
+  #define __Pyx_EnterTracing(tstate)  PyThreadState_EnterTracing(tstate)
+  #define __Pyx_LeaveTracing(tstate)  PyThreadState_LeaveTracing(tstate)
 #elif PY_VERSION_HEX >= 0x030a00b1
   #define __Pyx_IsTracing(tstate, check_tracing, check_funcs)\
      (unlikely((tstate)->cframe->use_tracing) &&\
          (!(check_tracing) || !(tstate)->tracing) &&\
          (!(check_funcs) || (tstate)->c_profilefunc || (CYTHON_TRACE && (tstate)->c_tracefunc)))
   #define __Pyx_EnterTracing(tstate)\
       do { tstate->tracing++; tstate->cframe->use_tracing = 0; } while (0)
@@ -2069,30 +2080,30 @@
   #include <utility>
   #define __PYX_STD_MOVE_IF_SUPPORTED(x) std::move(x)
 #else
   #define __PYX_STD_MOVE_IF_SUPPORTED(x) x
 #endif
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto_3_0_0b3
-#define __PYX_HAVE_RT_ImportType_proto_3_0_0b3
+#ifndef __PYX_HAVE_RT_ImportType_proto_3_0_0
+#define __PYX_HAVE_RT_ImportType_proto_3_0_0
 #if defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L
 #include <stdalign.h>
 #endif
 #if (defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L) || __cplusplus >= 201103L
-#define __PYX_GET_STRUCT_ALIGNMENT_3_0_0b3(s) alignof(s)
+#define __PYX_GET_STRUCT_ALIGNMENT_3_0_0(s) alignof(s)
 #else
-#define __PYX_GET_STRUCT_ALIGNMENT_3_0_0b3(s) sizeof(void*)
+#define __PYX_GET_STRUCT_ALIGNMENT_3_0_0(s) sizeof(void*)
 #endif
-enum __Pyx_ImportType_CheckSize_3_0_0b3 {
-   __Pyx_ImportType_CheckSize_Error_3_0_0b3 = 0,
-   __Pyx_ImportType_CheckSize_Warn_3_0_0b3 = 1,
-   __Pyx_ImportType_CheckSize_Ignore_3_0_0b3 = 2
+enum __Pyx_ImportType_CheckSize_3_0_0 {
+   __Pyx_ImportType_CheckSize_Error_3_0_0 = 0,
+   __Pyx_ImportType_CheckSize_Warn_3_0_0 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_3_0_0 = 2
 };
-static PyTypeObject *__Pyx_ImportType_3_0_0b3(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_0b3 check_size);
+static PyTypeObject *__Pyx_ImportType_3_0_0(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_0 check_size);
 #endif
 
 /* Import.proto */
 static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level);
 
 /* ImportFrom.proto */
 static PyObject* __Pyx_ImportFrom(PyObject* module, PyObject* name);
@@ -3492,17 +3503,17 @@
  *         s_proc.data = NULL
  */
     __Pyx_TraceLine(291,0,__PYX_ERR(0, 291, __pyx_L6_except_error))
     __pyx_t_13 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_13) {
       __Pyx_AddTraceback("cpp_common.hash_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_1, &__pyx_t_14, &__pyx_t_15) < 0) __PYX_ERR(0, 291, __pyx_L6_except_error)
-      __Pyx_GOTREF(__pyx_t_1);
-      __Pyx_GOTREF(__pyx_t_14);
-      __Pyx_GOTREF(__pyx_t_15);
+      __Pyx_XGOTREF(__pyx_t_1);
+      __Pyx_XGOTREF(__pyx_t_14);
+      __Pyx_XGOTREF(__pyx_t_15);
       __Pyx_INCREF(__pyx_t_14);
       __pyx_v_e = __pyx_t_14;
       /*try:*/ {
 
         /* "cpp_common.pxd":292
  *                 (<uint64_t*>s_proc.data)[i] = <uint64_t>hash(arr[i])
  *     except Exception as e:
@@ -3909,17 +3920,17 @@
  *         s_proc.data = NULL
  */
     __Pyx_TraceLine(320,0,__PYX_ERR(0, 320, __pyx_L6_except_error))
     __pyx_t_13 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_13) {
       __Pyx_AddTraceback("cpp_common.hash_sequence", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_9, &__pyx_t_14, &__pyx_t_15) < 0) __PYX_ERR(0, 320, __pyx_L6_except_error)
-      __Pyx_GOTREF(__pyx_t_9);
-      __Pyx_GOTREF(__pyx_t_14);
-      __Pyx_GOTREF(__pyx_t_15);
+      __Pyx_XGOTREF(__pyx_t_9);
+      __Pyx_XGOTREF(__pyx_t_14);
+      __Pyx_XGOTREF(__pyx_t_15);
       __Pyx_INCREF(__pyx_t_14);
       __pyx_v_e = __pyx_t_14;
       /*try:*/ {
 
         /* "cpp_common.pxd":321
  *                 (<uint64_t*>s_proc.data)[i] = <uint64_t>hash(elem)
  *     except Exception as e:
@@ -8862,23 +8873,23 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_3_0_0b3(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
+  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_3_0_0(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0b3(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(PyTypeObject),
   #elif CYTHON_COMPILING_IN_LIMITED_API
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0b3(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0b3(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(PyHeapTypeObject),
   #endif
-  __Pyx_ImportType_CheckSize_Warn_3_0_0b3); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
+  __Pyx_ImportType_CheckSize_Warn_3_0_0); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -11694,18 +11705,18 @@
         function_name, key);
     #endif
 bad:
     return -1;
 }
 
 /* TypeImport */
-#ifndef __PYX_HAVE_RT_ImportType_3_0_0b3
-#define __PYX_HAVE_RT_ImportType_3_0_0b3
-static PyTypeObject *__Pyx_ImportType_3_0_0b3(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_0b3 check_size)
+#ifndef __PYX_HAVE_RT_ImportType_3_0_0
+#define __PYX_HAVE_RT_ImportType_3_0_0
+static PyTypeObject *__Pyx_ImportType_3_0_0(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_0 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
     Py_ssize_t itemsize;
 #if CYTHON_COMPILING_IN_LIMITED_API
     PyObject *py_basicsize;
@@ -11751,23 +11762,23 @@
     if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize+itemsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error_3_0_0b3 &&
+    if (check_size == __Pyx_ImportType_CheckSize_Error_3_0_0 &&
             ((size_t)basicsize > size || (size_t)(basicsize + itemsize) < size)) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd-%zd from PyObject",
             module_name, class_name, size, basicsize, basicsize+itemsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn_3_0_0b3 && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_3_0_0 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
```

### Comparing `rapidfuzz-3.1.1/src/rapidfuzz/fuzz_py.py` & `rapidfuzz-3.1.2/src/rapidfuzz/fuzz_py.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/src/rapidfuzz/process.pyi` & `rapidfuzz-3.1.2/src/rapidfuzz/process.pyi`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/src/rapidfuzz/process_cpp.hpp` & `rapidfuzz-3.1.2/src/rapidfuzz/process_cpp.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/src/rapidfuzz/process_cpp.py` & `rapidfuzz-3.1.2/src/rapidfuzz/process_cpp.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/src/rapidfuzz/process_cpp_impl.cxx` & `rapidfuzz-3.1.2/src/rapidfuzz/process_cpp_impl.cxx`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 3.0.0b3 */
+/* Generated by Cython 3.0.0 */
 
 #ifndef PY_SSIZE_T_CLEAN
 #define PY_SSIZE_T_CLEAN
 #endif /* PY_SSIZE_T_CLEAN */
 #if defined(CYTHON_LIMITED_API) && 0
   #ifndef Py_LIMITED_API
     #if CYTHON_LIMITED_API+0 > 0x03030000
@@ -32,18 +32,18 @@
     #endif
     
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02070000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.7+ or Python 3.3+.
 #else
-#define CYTHON_ABI "3_0_0b3"
+#define CYTHON_ABI "3_0_0"
 #define __PYX_ABI_MODULE_NAME "_cython_" CYTHON_ABI
 #define __PYX_TYPE_MODULE_PREFIX __PYX_ABI_MODULE_NAME "."
-#define CYTHON_HEX_VERSION 0x030000B3
+#define CYTHON_HEX_VERSION 0x030000F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(_WIN32) && !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -658,14 +658,19 @@
 #endif
 #if PY_VERSION_HEX >= 0x030A00B1 || defined(Py_IsFalse)
   #define __Pyx_Py_IsFalse(ob) Py_IsFalse(ob)
 #else
   #define __Pyx_Py_IsFalse(ob) __Pyx_Py_Is((ob), Py_False)
 #endif
 #define __Pyx_NoneAsNull(obj)  (__Pyx_Py_IsNone(obj) ? NULL : (obj))
+#if PY_VERSION_HEX >= 0x030900F0 && !CYTHON_COMPILING_IN_PYPY
+  #define __Pyx_PyObject_GC_IsFinalized(o) PyObject_GC_IsFinalized(o)
+#else
+  #define __Pyx_PyObject_GC_IsFinalized(o) _PyGC_FINALIZED(o)
+#endif
 #ifndef CO_COROUTINE
   #define CO_COROUTINE 0x80
 #endif
 #ifndef CO_ASYNC_GENERATOR
   #define CO_ASYNC_GENERATOR 0x200
 #endif
 #ifndef Py_TPFLAGS_CHECKTYPES
@@ -902,15 +907,15 @@
   #endif
   #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GET_LENGTH(u)
   #define __Pyx_PyUnicode_READ_CHAR(u, i) PyUnicode_READ_CHAR(u, i)
   #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   PyUnicode_MAX_CHAR_VALUE(u)
   #define __Pyx_PyUnicode_KIND(u)         ((int)PyUnicode_KIND(u))
   #define __Pyx_PyUnicode_DATA(u)         PyUnicode_DATA(u)
   #define __Pyx_PyUnicode_READ(k, d, i)   PyUnicode_READ(k, d, i)
-  #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  PyUnicode_WRITE(k, d, i, ch)
+  #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  PyUnicode_WRITE(k, d, i, (Py_UCS4) ch)
   #if PY_VERSION_HEX >= 0x030C0000
     #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
   #else
     #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
     #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
     #else
     #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
@@ -924,15 +929,15 @@
   #define __Pyx_PyUnicode_READY(op)       (0)
   #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GET_SIZE(u)
   #define __Pyx_PyUnicode_READ_CHAR(u, i) ((Py_UCS4)(PyUnicode_AS_UNICODE(u)[i]))
   #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   ((sizeof(Py_UNICODE) == 2) ? 65535U : 1114111U)
   #define __Pyx_PyUnicode_KIND(u)         ((int)sizeof(Py_UNICODE))
   #define __Pyx_PyUnicode_DATA(u)         ((void*)PyUnicode_AS_UNICODE(u))
   #define __Pyx_PyUnicode_READ(k, d, i)   ((void)(k), (Py_UCS4)(((Py_UNICODE*)d)[i]))
-  #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  (((void)(k)), ((Py_UNICODE*)d)[i] = ch)
+  #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  (((void)(k)), ((Py_UNICODE*)d)[i] = (Py_UNICODE) ch)
   #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_SIZE(u))
 #endif
 #if CYTHON_COMPILING_IN_PYPY
   #define __Pyx_PyUnicode_Concat(a, b)      PyNumber_Add(a, b)
   #define __Pyx_PyUnicode_ConcatSafe(a, b)  PyNumber_Add(a, b)
 #else
   #define __Pyx_PyUnicode_Concat(a, b)      PyUnicode_Concat(a, b)
@@ -1259,20 +1264,20 @@
   #endif
   #define __Pyx_PyLong_Sign(x)  (((PyLongObject*)x)->long_value.lv_tag & _PyLong_SIGN_MASK)
   #define __Pyx_PyLong_IsNeg(x)  ((__Pyx_PyLong_Sign(x) & 2) != 0)
   #define __Pyx_PyLong_IsNonNeg(x)  (!__Pyx_PyLong_IsNeg(x))
   #define __Pyx_PyLong_IsZero(x)  (__Pyx_PyLong_Sign(x) & 1)
   #define __Pyx_PyLong_IsPos(x)  (__Pyx_PyLong_Sign(x) == 0)
   #define __Pyx_PyLong_CompactValueUnsigned(x)  (__Pyx_PyLong_Digits(x)[0])
-  #define __Pyx_PyLong_DigitCount(x)  (((PyLongObject*)x)->long_value.lv_tag >> _PyLong_NON_SIZE_BITS)
+  #define __Pyx_PyLong_DigitCount(x)  ((Py_ssize_t) (((PyLongObject*)x)->long_value.lv_tag >> _PyLong_NON_SIZE_BITS))
   #define __Pyx_PyLong_SignedDigitCount(x)\
-        ((1 - (Py_ssize_t) __Pyx_PyLong_Sign(x)) * (Py_ssize_t) __Pyx_PyLong_DigitCount(x))
+        ((1 - (Py_ssize_t) __Pyx_PyLong_Sign(x)) * __Pyx_PyLong_DigitCount(x))
   #if defined(PyUnstable_Long_IsCompact) && defined(PyUnstable_Long_CompactValue)
-    #define __Pyx_PyLong_IsCompact(x)     PyUnstable_Long_IsCompact(x)
-    #define __Pyx_PyLong_CompactValue(x)  PyUnstable_Long_CompactValue(x)
+    #define __Pyx_PyLong_IsCompact(x)     PyUnstable_Long_IsCompact((PyLongObject*) x)
+    #define __Pyx_PyLong_CompactValue(x)  PyUnstable_Long_CompactValue((PyLongObject*) x)
   #else
     #define __Pyx_PyLong_IsCompact(x)     (((PyLongObject*)x)->long_value.lv_tag < (2 << _PyLong_NON_SIZE_BITS))
     #define __Pyx_PyLong_CompactValue(x)  ((1 - (Py_ssize_t) __Pyx_PyLong_Sign(x)) * (Py_ssize_t) __Pyx_PyLong_Digits(x)[0])
   #endif
   typedef Py_ssize_t  __Pyx_compact_pylong;
   typedef size_t  __Pyx_compact_upylong;
   #else  // Py < 3.12
@@ -1312,15 +1317,15 @@
     if (!default_encoding_c) goto bad;
     if (strcmp(default_encoding_c, "ascii") == 0) {
         __Pyx_sys_getdefaultencoding_not_ascii = 0;
     } else {
         char ascii_chars[128];
         int c;
         for (c = 0; c < 128; c++) {
-            ascii_chars[c] = c;
+            ascii_chars[c] = (char) c;
         }
         __Pyx_sys_getdefaultencoding_not_ascii = 1;
         ascii_chars_u = PyUnicode_DecodeASCII(ascii_chars, 128, NULL);
         if (!ascii_chars_u) goto bad;
         ascii_chars_b = PyUnicode_AsEncodedString(ascii_chars_u, default_encoding_c, NULL);
         if (!ascii_chars_b || !PyBytes_Check(ascii_chars_b) || memcmp(ascii_chars, PyBytes_AS_STRING(ascii_chars_b), 128) != 0) {
             PyErr_Format(
@@ -2134,20 +2139,26 @@
   #define __Pyx_TraceDeclarations\
       static PyCodeObject *__pyx_frame_code = NULL;\
       CYTHON_FRAME_MODIFIER PyFrameObject *__pyx_frame = NULL;\
       int __Pyx_use_tracing = 0;
   #define __Pyx_TraceFrameInit(codeobj)\
       if (codeobj) __pyx_frame_code = (PyCodeObject*) codeobj;
 #if PY_VERSION_HEX >= 0x030b00a2
+  #if PY_VERSION_HEX >= 0x030C00b1
+  #define __Pyx_IsTracing(tstate, check_tracing, check_funcs)\
+     ((!(check_tracing) || !(tstate)->tracing) &&\
+         (!(check_funcs) || (tstate)->c_profilefunc || (CYTHON_TRACE && (tstate)->c_tracefunc)))
+  #else
   #define __Pyx_IsTracing(tstate, check_tracing, check_funcs)\
      (unlikely((tstate)->cframe->use_tracing) &&\
          (!(check_tracing) || !(tstate)->tracing) &&\
          (!(check_funcs) || (tstate)->c_profilefunc || (CYTHON_TRACE && (tstate)->c_tracefunc)))
-  #define __Pyx_EnterTracing(tstate) PyThreadState_EnterTracing(tstate)
-  #define __Pyx_LeaveTracing(tstate) PyThreadState_LeaveTracing(tstate)
+  #endif
+  #define __Pyx_EnterTracing(tstate)  PyThreadState_EnterTracing(tstate)
+  #define __Pyx_LeaveTracing(tstate)  PyThreadState_LeaveTracing(tstate)
 #elif PY_VERSION_HEX >= 0x030a00b1
   #define __Pyx_IsTracing(tstate, check_tracing, check_funcs)\
      (unlikely((tstate)->cframe->use_tracing) &&\
          (!(check_tracing) || !(tstate)->tracing) &&\
          (!(check_funcs) || (tstate)->c_profilefunc || (CYTHON_TRACE && (tstate)->c_tracefunc)))
   #define __Pyx_EnterTracing(tstate)\
       do { tstate->tracing++; tstate->cframe->use_tracing = 0; } while (0)
@@ -2770,30 +2781,30 @@
 
 /* SetupReduce.proto */
 #if !CYTHON_COMPILING_IN_LIMITED_API
 static int __Pyx_setup_reduce(PyObject* type_obj);
 #endif
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto_3_0_0b3
-#define __PYX_HAVE_RT_ImportType_proto_3_0_0b3
+#ifndef __PYX_HAVE_RT_ImportType_proto_3_0_0
+#define __PYX_HAVE_RT_ImportType_proto_3_0_0
 #if defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L
 #include <stdalign.h>
 #endif
 #if (defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L) || __cplusplus >= 201103L
-#define __PYX_GET_STRUCT_ALIGNMENT_3_0_0b3(s) alignof(s)
+#define __PYX_GET_STRUCT_ALIGNMENT_3_0_0(s) alignof(s)
 #else
-#define __PYX_GET_STRUCT_ALIGNMENT_3_0_0b3(s) sizeof(void*)
+#define __PYX_GET_STRUCT_ALIGNMENT_3_0_0(s) sizeof(void*)
 #endif
-enum __Pyx_ImportType_CheckSize_3_0_0b3 {
-   __Pyx_ImportType_CheckSize_Error_3_0_0b3 = 0,
-   __Pyx_ImportType_CheckSize_Warn_3_0_0b3 = 1,
-   __Pyx_ImportType_CheckSize_Ignore_3_0_0b3 = 2
+enum __Pyx_ImportType_CheckSize_3_0_0 {
+   __Pyx_ImportType_CheckSize_Error_3_0_0 = 0,
+   __Pyx_ImportType_CheckSize_Warn_3_0_0 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_3_0_0 = 2
 };
-static PyTypeObject *__Pyx_ImportType_3_0_0b3(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_0b3 check_size);
+static PyTypeObject *__Pyx_ImportType_3_0_0(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_0 check_size);
 #endif
 
 /* Py3UpdateBases.proto */
 static PyObject* __Pyx_PEP560_update_bases(PyObject *bases);
 
 /* SetNameInClass.proto */
 #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030500A1
@@ -8136,17 +8147,17 @@
  *         s_proc.data = NULL
  */
     __Pyx_TraceLine(291,0,__PYX_ERR(2, 291, __pyx_L6_except_error))
     __pyx_t_13 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_13) {
       __Pyx_AddTraceback("cpp_common.hash_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_1, &__pyx_t_14, &__pyx_t_15) < 0) __PYX_ERR(2, 291, __pyx_L6_except_error)
-      __Pyx_GOTREF(__pyx_t_1);
-      __Pyx_GOTREF(__pyx_t_14);
-      __Pyx_GOTREF(__pyx_t_15);
+      __Pyx_XGOTREF(__pyx_t_1);
+      __Pyx_XGOTREF(__pyx_t_14);
+      __Pyx_XGOTREF(__pyx_t_15);
       __Pyx_INCREF(__pyx_t_14);
       __pyx_v_e = __pyx_t_14;
       /*try:*/ {
 
         /* "cpp_common.pxd":292
  *                 (<uint64_t*>s_proc.data)[i] = <uint64_t>hash(arr[i])
  *     except Exception as e:
@@ -8553,17 +8564,17 @@
  *         s_proc.data = NULL
  */
     __Pyx_TraceLine(320,0,__PYX_ERR(2, 320, __pyx_L6_except_error))
     __pyx_t_13 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_13) {
       __Pyx_AddTraceback("cpp_common.hash_sequence", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_9, &__pyx_t_14, &__pyx_t_15) < 0) __PYX_ERR(2, 320, __pyx_L6_except_error)
-      __Pyx_GOTREF(__pyx_t_9);
-      __Pyx_GOTREF(__pyx_t_14);
-      __Pyx_GOTREF(__pyx_t_15);
+      __Pyx_XGOTREF(__pyx_t_9);
+      __Pyx_XGOTREF(__pyx_t_14);
+      __Pyx_XGOTREF(__pyx_t_15);
       __Pyx_INCREF(__pyx_t_14);
       __pyx_v_e = __pyx_t_14;
       /*try:*/ {
 
         /* "cpp_common.pxd":321
  *                 (<uint64_t*>s_proc.data)[i] = <uint64_t>hash(elem)
  *     except Exception as e:
@@ -20580,17 +20591,17 @@
  *         # preprocessing the choices, but this is good enough for now
  */
     __Pyx_TraceLine(964,0,__PYX_ERR(0, 964, __pyx_L6_except_error))
     __pyx_t_6 = __Pyx_PyErr_ExceptionMatches(__pyx_builtin_TypeError);
     if (__pyx_t_6) {
       __Pyx_AddTraceback("rapidfuzz.process_cpp_impl.extract", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_3, &__pyx_t_1, &__pyx_t_4) < 0) __PYX_ERR(0, 964, __pyx_L6_except_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __Pyx_GOTREF(__pyx_t_1);
-      __Pyx_GOTREF(__pyx_t_4);
+      __Pyx_XGOTREF(__pyx_t_3);
+      __Pyx_XGOTREF(__pyx_t_1);
+      __Pyx_XGOTREF(__pyx_t_4);
 
       /* "rapidfuzz/process_cpp_impl.pyx":967
  *         # handle generators. In Theory we could retrieve the length later on while
  *         # preprocessing the choices, but this is good enough for now
  *         choices = list(choices)             # <<<<<<<<<<<<<<
  *         if limit is None or limit > len(choices):
  *             limit = len(choices)
@@ -29040,15 +29051,15 @@
   new((void*)&(p->matrix)) Matrix();
   return o;
 }
 
 static void __pyx_tp_dealloc_9rapidfuzz_16process_cpp_impl_Matrix(PyObject *o) {
   struct __pyx_obj_9rapidfuzz_16process_cpp_impl_Matrix *p = (struct __pyx_obj_9rapidfuzz_16process_cpp_impl_Matrix *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely((PY_VERSION_HEX >= 0x03080000 || __Pyx_PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE)) && __Pyx_PyObject_GetSlot(o, tp_finalize, destructor)) && (!PyType_IS_GC(Py_TYPE(o)) || !_PyGC_FINALIZED(o))) {
+  if (unlikely((PY_VERSION_HEX >= 0x03080000 || __Pyx_PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE)) && __Pyx_PyObject_GetSlot(o, tp_finalize, destructor)) && (!PyType_IS_GC(Py_TYPE(o)) || !__Pyx_PyObject_GC_IsFinalized(o))) {
     if (__Pyx_PyObject_GetSlot(o, tp_dealloc, destructor) == __pyx_tp_dealloc_9rapidfuzz_16process_cpp_impl_Matrix) {
       if (PyObject_CallFinalizerFromDealloc(o)) return;
     }
   }
   #endif
   __Pyx_call_destructor(p->matrix);
   (*Py_TYPE(o)->tp_free)(o);
@@ -29224,15 +29235,15 @@
   new((void*)&(p->__pyx_v_scorer_flags)) RF_ScorerFlags();
   return o;
 }
 
 static void __pyx_tp_dealloc_9rapidfuzz_16process_cpp_impl___pyx_scope_struct__extract_iter(PyObject *o) {
   struct __pyx_obj_9rapidfuzz_16process_cpp_impl___pyx_scope_struct__extract_iter *p = (struct __pyx_obj_9rapidfuzz_16process_cpp_impl___pyx_scope_struct__extract_iter *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely((PY_VERSION_HEX >= 0x03080000 || __Pyx_PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE)) && __Pyx_PyObject_GetSlot(o, tp_finalize, destructor)) && !_PyGC_FINALIZED(o)) {
+  if (unlikely((PY_VERSION_HEX >= 0x03080000 || __Pyx_PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE)) && __Pyx_PyObject_GetSlot(o, tp_finalize, destructor)) && !__Pyx_PyObject_GC_IsFinalized(o)) {
     if (__Pyx_PyObject_GetSlot(o, tp_dealloc, destructor) == __pyx_tp_dealloc_9rapidfuzz_16process_cpp_impl___pyx_scope_struct__extract_iter) {
       if (PyObject_CallFinalizerFromDealloc(o)) return;
     }
   }
   #endif
   PyObject_GC_UnTrack(o);
   __Pyx_call_destructor(p->__pyx_v_kwargs_context);
@@ -29443,15 +29454,15 @@
   new((void*)&(p->__pyx_v_scorer_func)) RF_ScorerFunc();
   return o;
 }
 
 static void __pyx_tp_dealloc_9rapidfuzz_16process_cpp_impl___pyx_scope_struct_1_extract_iter_dict_f64(PyObject *o) {
   struct __pyx_obj_9rapidfuzz_16process_cpp_impl___pyx_scope_struct_1_extract_iter_dict_f64 *p = (struct __pyx_obj_9rapidfuzz_16process_cpp_impl___pyx_scope_struct_1_extract_iter_dict_f64 *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely((PY_VERSION_HEX >= 0x03080000 || __Pyx_PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE)) && __Pyx_PyObject_GetSlot(o, tp_finalize, destructor)) && !_PyGC_FINALIZED(o)) {
+  if (unlikely((PY_VERSION_HEX >= 0x03080000 || __Pyx_PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE)) && __Pyx_PyObject_GetSlot(o, tp_finalize, destructor)) && !__Pyx_PyObject_GC_IsFinalized(o)) {
     if (__Pyx_PyObject_GetSlot(o, tp_dealloc, destructor) == __pyx_tp_dealloc_9rapidfuzz_16process_cpp_impl___pyx_scope_struct_1_extract_iter_dict_f64) {
       if (PyObject_CallFinalizerFromDealloc(o)) return;
     }
   }
   #endif
   PyObject_GC_UnTrack(o);
   __Pyx_call_destructor(p->__pyx_v_ScorerFunc);
@@ -29617,15 +29628,15 @@
   new((void*)&(p->__pyx_v_scorer_func)) RF_ScorerFunc();
   return o;
 }
 
 static void __pyx_tp_dealloc_9rapidfuzz_16process_cpp_impl___pyx_scope_struct_2_extract_iter_dict_i64(PyObject *o) {
   struct __pyx_obj_9rapidfuzz_16process_cpp_impl___pyx_scope_struct_2_extract_iter_dict_i64 *p = (struct __pyx_obj_9rapidfuzz_16process_cpp_impl___pyx_scope_struct_2_extract_iter_dict_i64 *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely((PY_VERSION_HEX >= 0x03080000 || __Pyx_PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE)) && __Pyx_PyObject_GetSlot(o, tp_finalize, destructor)) && !_PyGC_FINALIZED(o)) {
+  if (unlikely((PY_VERSION_HEX >= 0x03080000 || __Pyx_PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE)) && __Pyx_PyObject_GetSlot(o, tp_finalize, destructor)) && !__Pyx_PyObject_GC_IsFinalized(o)) {
     if (__Pyx_PyObject_GetSlot(o, tp_dealloc, destructor) == __pyx_tp_dealloc_9rapidfuzz_16process_cpp_impl___pyx_scope_struct_2_extract_iter_dict_i64) {
       if (PyObject_CallFinalizerFromDealloc(o)) return;
     }
   }
   #endif
   PyObject_GC_UnTrack(o);
   __Pyx_call_destructor(p->__pyx_v_ScorerFunc);
@@ -29791,15 +29802,15 @@
   new((void*)&(p->__pyx_v_scorer_func)) RF_ScorerFunc();
   return o;
 }
 
 static void __pyx_tp_dealloc_9rapidfuzz_16process_cpp_impl___pyx_scope_struct_3_extract_iter_list_f64(PyObject *o) {
   struct __pyx_obj_9rapidfuzz_16process_cpp_impl___pyx_scope_struct_3_extract_iter_list_f64 *p = (struct __pyx_obj_9rapidfuzz_16process_cpp_impl___pyx_scope_struct_3_extract_iter_list_f64 *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely((PY_VERSION_HEX >= 0x03080000 || __Pyx_PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE)) && __Pyx_PyObject_GetSlot(o, tp_finalize, destructor)) && !_PyGC_FINALIZED(o)) {
+  if (unlikely((PY_VERSION_HEX >= 0x03080000 || __Pyx_PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE)) && __Pyx_PyObject_GetSlot(o, tp_finalize, destructor)) && !__Pyx_PyObject_GC_IsFinalized(o)) {
     if (__Pyx_PyObject_GetSlot(o, tp_dealloc, destructor) == __pyx_tp_dealloc_9rapidfuzz_16process_cpp_impl___pyx_scope_struct_3_extract_iter_list_f64) {
       if (PyObject_CallFinalizerFromDealloc(o)) return;
     }
   }
   #endif
   PyObject_GC_UnTrack(o);
   __Pyx_call_destructor(p->__pyx_v_ScorerFunc);
@@ -29969,15 +29980,15 @@
   new((void*)&(p->__pyx_v_scorer_func)) RF_ScorerFunc();
   return o;
 }
 
 static void __pyx_tp_dealloc_9rapidfuzz_16process_cpp_impl___pyx_scope_struct_4_extract_iter_list_i64(PyObject *o) {
   struct __pyx_obj_9rapidfuzz_16process_cpp_impl___pyx_scope_struct_4_extract_iter_list_i64 *p = (struct __pyx_obj_9rapidfuzz_16process_cpp_impl___pyx_scope_struct_4_extract_iter_list_i64 *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely((PY_VERSION_HEX >= 0x03080000 || __Pyx_PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE)) && __Pyx_PyObject_GetSlot(o, tp_finalize, destructor)) && !_PyGC_FINALIZED(o)) {
+  if (unlikely((PY_VERSION_HEX >= 0x03080000 || __Pyx_PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE)) && __Pyx_PyObject_GetSlot(o, tp_finalize, destructor)) && !__Pyx_PyObject_GC_IsFinalized(o)) {
     if (__Pyx_PyObject_GetSlot(o, tp_dealloc, destructor) == __pyx_tp_dealloc_9rapidfuzz_16process_cpp_impl___pyx_scope_struct_4_extract_iter_list_i64) {
       if (PyObject_CallFinalizerFromDealloc(o)) return;
     }
   }
   #endif
   PyObject_GC_UnTrack(o);
   __Pyx_call_destructor(p->__pyx_v_ScorerFunc);
@@ -30140,15 +30151,15 @@
   #endif
   return o;
 }
 
 static void __pyx_tp_dealloc_9rapidfuzz_16process_cpp_impl___pyx_scope_struct_5_py_extract_iter_dict(PyObject *o) {
   struct __pyx_obj_9rapidfuzz_16process_cpp_impl___pyx_scope_struct_5_py_extract_iter_dict *p = (struct __pyx_obj_9rapidfuzz_16process_cpp_impl___pyx_scope_struct_5_py_extract_iter_dict *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely((PY_VERSION_HEX >= 0x03080000 || __Pyx_PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE)) && __Pyx_PyObject_GetSlot(o, tp_finalize, destructor)) && !_PyGC_FINALIZED(o)) {
+  if (unlikely((PY_VERSION_HEX >= 0x03080000 || __Pyx_PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE)) && __Pyx_PyObject_GetSlot(o, tp_finalize, destructor)) && !__Pyx_PyObject_GC_IsFinalized(o)) {
     if (__Pyx_PyObject_GetSlot(o, tp_dealloc, destructor) == __pyx_tp_dealloc_9rapidfuzz_16process_cpp_impl___pyx_scope_struct_5_py_extract_iter_dict) {
       if (PyObject_CallFinalizerFromDealloc(o)) return;
     }
   }
   #endif
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->__pyx_outer_scope);
@@ -30310,15 +30321,15 @@
   #endif
   return o;
 }
 
 static void __pyx_tp_dealloc_9rapidfuzz_16process_cpp_impl___pyx_scope_struct_6_py_extract_iter_list(PyObject *o) {
   struct __pyx_obj_9rapidfuzz_16process_cpp_impl___pyx_scope_struct_6_py_extract_iter_list *p = (struct __pyx_obj_9rapidfuzz_16process_cpp_impl___pyx_scope_struct_6_py_extract_iter_list *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely((PY_VERSION_HEX >= 0x03080000 || __Pyx_PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE)) && __Pyx_PyObject_GetSlot(o, tp_finalize, destructor)) && !_PyGC_FINALIZED(o)) {
+  if (unlikely((PY_VERSION_HEX >= 0x03080000 || __Pyx_PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE)) && __Pyx_PyObject_GetSlot(o, tp_finalize, destructor)) && !__Pyx_PyObject_GC_IsFinalized(o)) {
     if (__Pyx_PyObject_GetSlot(o, tp_dealloc, destructor) == __pyx_tp_dealloc_9rapidfuzz_16process_cpp_impl___pyx_scope_struct_6_py_extract_iter_list) {
       if (PyObject_CallFinalizerFromDealloc(o)) return;
     }
   }
   #endif
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->__pyx_outer_scope);
@@ -31374,31 +31385,31 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(4, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_3_0_0b3(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
+  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_3_0_0(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0b3(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(PyTypeObject),
   #elif CYTHON_COMPILING_IN_LIMITED_API
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0b3(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0b3(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(PyHeapTypeObject),
   #endif
-  __Pyx_ImportType_CheckSize_Warn_3_0_0b3); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(4, 9, __pyx_L1_error)
+  __Pyx_ImportType_CheckSize_Warn_3_0_0); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(4, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(5, 8, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4bool_bool = __Pyx_ImportType_3_0_0b3(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "bool", sizeof(PyBoolObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0b3(PyBoolObject),__Pyx_ImportType_CheckSize_Warn_3_0_0b3); if (!__pyx_ptype_7cpython_4bool_bool) __PYX_ERR(5, 8, __pyx_L1_error)
+  __pyx_ptype_7cpython_4bool_bool = __Pyx_ImportType_3_0_0(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "bool", sizeof(PyBoolObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(PyBoolObject),__Pyx_ImportType_CheckSize_Warn_3_0_0); if (!__pyx_ptype_7cpython_4bool_bool) __PYX_ERR(5, 8, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(6, 15, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_7complex_complex = __Pyx_ImportType_3_0_0b3(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "complex", sizeof(PyComplexObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0b3(PyComplexObject),__Pyx_ImportType_CheckSize_Warn_3_0_0b3); if (!__pyx_ptype_7cpython_7complex_complex) __PYX_ERR(6, 15, __pyx_L1_error)
+  __pyx_ptype_7cpython_7complex_complex = __Pyx_ImportType_3_0_0(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "complex", sizeof(PyComplexObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(PyComplexObject),__Pyx_ImportType_CheckSize_Warn_3_0_0); if (!__pyx_ptype_7cpython_7complex_complex) __PYX_ERR(6, 15, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -37223,15 +37234,15 @@
     CYTHON_UNUSED_VAR(zerodivision_check);
     #if PY_MAJOR_VERSION < 3
     if (likely(PyInt_CheckExact(op1))) {
         const long b = intval;
         long x;
         long a = PyInt_AS_LONG(op1);
         
-            x = (long)((unsigned long)a + b);
+            x = (long)((unsigned long)a + (unsigned long)b);
             if (likely((x^a) >= 0 || (x^b) >= 0))
                 return PyInt_FromLong(x);
             return PyLong_Type.tp_as_number->nb_add(op1, op2);
     }
     #endif
     #if CYTHON_USE_PYLONG_INTERNALS
     if (likely(PyLong_CheckExact(op1))) {
@@ -38941,18 +38952,18 @@
     Py_XDECREF(setstate);
     Py_XDECREF(setstate_cython);
     return ret;
 }
 #endif
 
 /* TypeImport */
-#ifndef __PYX_HAVE_RT_ImportType_3_0_0b3
-#define __PYX_HAVE_RT_ImportType_3_0_0b3
-static PyTypeObject *__Pyx_ImportType_3_0_0b3(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_0b3 check_size)
+#ifndef __PYX_HAVE_RT_ImportType_3_0_0
+#define __PYX_HAVE_RT_ImportType_3_0_0
+static PyTypeObject *__Pyx_ImportType_3_0_0(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_0 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
     Py_ssize_t itemsize;
 #if CYTHON_COMPILING_IN_LIMITED_API
     PyObject *py_basicsize;
@@ -38998,23 +39009,23 @@
     if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize+itemsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error_3_0_0b3 &&
+    if (check_size == __Pyx_ImportType_CheckSize_Error_3_0_0 &&
             ((size_t)basicsize > size || (size_t)(basicsize + itemsize) < size)) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd-%zd from PyObject",
             module_name, class_name, size, basicsize, basicsize+itemsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn_3_0_0b3 && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_3_0_0 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
```

### Comparing `rapidfuzz-3.1.1/src/rapidfuzz/process_cpp_impl.pyi` & `rapidfuzz-3.1.2/src/rapidfuzz/process_cpp_impl.pyi`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/src/rapidfuzz/process_cpp_impl.pyx` & `rapidfuzz-3.1.2/src/rapidfuzz/process_cpp_impl.pyx`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/src/rapidfuzz/process_py.py` & `rapidfuzz-3.1.2/src/rapidfuzz/process_py.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/src/rapidfuzz/rapidfuzz.h` & `rapidfuzz-3.1.2/src/rapidfuzz/rapidfuzz.h`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/src/rapidfuzz/unicodetype_db.h` & `rapidfuzz-3.1.2/src/rapidfuzz/unicodetype_db.h`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/src/rapidfuzz/utils.cpp` & `rapidfuzz-3.1.2/src/rapidfuzz/utils.cpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/src/rapidfuzz/utils.hpp` & `rapidfuzz-3.1.2/src/rapidfuzz/utils.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/src/rapidfuzz/utils_cpp.cxx` & `rapidfuzz-3.1.2/src/rapidfuzz/utils_cpp.cxx`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 3.0.0b3 */
+/* Generated by Cython 3.0.0 */
 
 #ifndef PY_SSIZE_T_CLEAN
 #define PY_SSIZE_T_CLEAN
 #endif /* PY_SSIZE_T_CLEAN */
 #if defined(CYTHON_LIMITED_API) && 0
   #ifndef Py_LIMITED_API
     #if CYTHON_LIMITED_API+0 > 0x03030000
@@ -15,18 +15,18 @@
 
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02070000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.7+ or Python 3.3+.
 #else
-#define CYTHON_ABI "3_0_0b3"
+#define CYTHON_ABI "3_0_0"
 #define __PYX_ABI_MODULE_NAME "_cython_" CYTHON_ABI
 #define __PYX_TYPE_MODULE_PREFIX __PYX_ABI_MODULE_NAME "."
-#define CYTHON_HEX_VERSION 0x030000B3
+#define CYTHON_HEX_VERSION 0x030000F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(_WIN32) && !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -641,14 +641,19 @@
 #endif
 #if PY_VERSION_HEX >= 0x030A00B1 || defined(Py_IsFalse)
   #define __Pyx_Py_IsFalse(ob) Py_IsFalse(ob)
 #else
   #define __Pyx_Py_IsFalse(ob) __Pyx_Py_Is((ob), Py_False)
 #endif
 #define __Pyx_NoneAsNull(obj)  (__Pyx_Py_IsNone(obj) ? NULL : (obj))
+#if PY_VERSION_HEX >= 0x030900F0 && !CYTHON_COMPILING_IN_PYPY
+  #define __Pyx_PyObject_GC_IsFinalized(o) PyObject_GC_IsFinalized(o)
+#else
+  #define __Pyx_PyObject_GC_IsFinalized(o) _PyGC_FINALIZED(o)
+#endif
 #ifndef CO_COROUTINE
   #define CO_COROUTINE 0x80
 #endif
 #ifndef CO_ASYNC_GENERATOR
   #define CO_ASYNC_GENERATOR 0x200
 #endif
 #ifndef Py_TPFLAGS_CHECKTYPES
@@ -885,15 +890,15 @@
   #endif
   #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GET_LENGTH(u)
   #define __Pyx_PyUnicode_READ_CHAR(u, i) PyUnicode_READ_CHAR(u, i)
   #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   PyUnicode_MAX_CHAR_VALUE(u)
   #define __Pyx_PyUnicode_KIND(u)         ((int)PyUnicode_KIND(u))
   #define __Pyx_PyUnicode_DATA(u)         PyUnicode_DATA(u)
   #define __Pyx_PyUnicode_READ(k, d, i)   PyUnicode_READ(k, d, i)
-  #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  PyUnicode_WRITE(k, d, i, ch)
+  #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  PyUnicode_WRITE(k, d, i, (Py_UCS4) ch)
   #if PY_VERSION_HEX >= 0x030C0000
     #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
   #else
     #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
     #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
     #else
     #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
@@ -907,15 +912,15 @@
   #define __Pyx_PyUnicode_READY(op)       (0)
   #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GET_SIZE(u)
   #define __Pyx_PyUnicode_READ_CHAR(u, i) ((Py_UCS4)(PyUnicode_AS_UNICODE(u)[i]))
   #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   ((sizeof(Py_UNICODE) == 2) ? 65535U : 1114111U)
   #define __Pyx_PyUnicode_KIND(u)         ((int)sizeof(Py_UNICODE))
   #define __Pyx_PyUnicode_DATA(u)         ((void*)PyUnicode_AS_UNICODE(u))
   #define __Pyx_PyUnicode_READ(k, d, i)   ((void)(k), (Py_UCS4)(((Py_UNICODE*)d)[i]))
-  #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  (((void)(k)), ((Py_UNICODE*)d)[i] = ch)
+  #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  (((void)(k)), ((Py_UNICODE*)d)[i] = (Py_UNICODE) ch)
   #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_SIZE(u))
 #endif
 #if CYTHON_COMPILING_IN_PYPY
   #define __Pyx_PyUnicode_Concat(a, b)      PyNumber_Add(a, b)
   #define __Pyx_PyUnicode_ConcatSafe(a, b)  PyNumber_Add(a, b)
 #else
   #define __Pyx_PyUnicode_Concat(a, b)      PyUnicode_Concat(a, b)
@@ -1239,20 +1244,20 @@
   #endif
   #define __Pyx_PyLong_Sign(x)  (((PyLongObject*)x)->long_value.lv_tag & _PyLong_SIGN_MASK)
   #define __Pyx_PyLong_IsNeg(x)  ((__Pyx_PyLong_Sign(x) & 2) != 0)
   #define __Pyx_PyLong_IsNonNeg(x)  (!__Pyx_PyLong_IsNeg(x))
   #define __Pyx_PyLong_IsZero(x)  (__Pyx_PyLong_Sign(x) & 1)
   #define __Pyx_PyLong_IsPos(x)  (__Pyx_PyLong_Sign(x) == 0)
   #define __Pyx_PyLong_CompactValueUnsigned(x)  (__Pyx_PyLong_Digits(x)[0])
-  #define __Pyx_PyLong_DigitCount(x)  (((PyLongObject*)x)->long_value.lv_tag >> _PyLong_NON_SIZE_BITS)
+  #define __Pyx_PyLong_DigitCount(x)  ((Py_ssize_t) (((PyLongObject*)x)->long_value.lv_tag >> _PyLong_NON_SIZE_BITS))
   #define __Pyx_PyLong_SignedDigitCount(x)\
-        ((1 - (Py_ssize_t) __Pyx_PyLong_Sign(x)) * (Py_ssize_t) __Pyx_PyLong_DigitCount(x))
+        ((1 - (Py_ssize_t) __Pyx_PyLong_Sign(x)) * __Pyx_PyLong_DigitCount(x))
   #if defined(PyUnstable_Long_IsCompact) && defined(PyUnstable_Long_CompactValue)
-    #define __Pyx_PyLong_IsCompact(x)     PyUnstable_Long_IsCompact(x)
-    #define __Pyx_PyLong_CompactValue(x)  PyUnstable_Long_CompactValue(x)
+    #define __Pyx_PyLong_IsCompact(x)     PyUnstable_Long_IsCompact((PyLongObject*) x)
+    #define __Pyx_PyLong_CompactValue(x)  PyUnstable_Long_CompactValue((PyLongObject*) x)
   #else
     #define __Pyx_PyLong_IsCompact(x)     (((PyLongObject*)x)->long_value.lv_tag < (2 << _PyLong_NON_SIZE_BITS))
     #define __Pyx_PyLong_CompactValue(x)  ((1 - (Py_ssize_t) __Pyx_PyLong_Sign(x)) * (Py_ssize_t) __Pyx_PyLong_Digits(x)[0])
   #endif
   typedef Py_ssize_t  __Pyx_compact_pylong;
   typedef size_t  __Pyx_compact_upylong;
   #else  // Py < 3.12
@@ -1292,15 +1297,15 @@
     if (!default_encoding_c) goto bad;
     if (strcmp(default_encoding_c, "ascii") == 0) {
         __Pyx_sys_getdefaultencoding_not_ascii = 0;
     } else {
         char ascii_chars[128];
         int c;
         for (c = 0; c < 128; c++) {
-            ascii_chars[c] = c;
+            ascii_chars[c] = (char) c;
         }
         __Pyx_sys_getdefaultencoding_not_ascii = 1;
         ascii_chars_u = PyUnicode_DecodeASCII(ascii_chars, 128, NULL);
         if (!ascii_chars_u) goto bad;
         ascii_chars_b = PyUnicode_AsEncodedString(ascii_chars_u, default_encoding_c, NULL);
         if (!ascii_chars_b || !PyBytes_Check(ascii_chars_b) || memcmp(ascii_chars, PyBytes_AS_STRING(ascii_chars_b), 128) != 0) {
             PyErr_Format(
@@ -1558,20 +1563,26 @@
   #define __Pyx_TraceDeclarations\
       static PyCodeObject *__pyx_frame_code = NULL;\
       CYTHON_FRAME_MODIFIER PyFrameObject *__pyx_frame = NULL;\
       int __Pyx_use_tracing = 0;
   #define __Pyx_TraceFrameInit(codeobj)\
       if (codeobj) __pyx_frame_code = (PyCodeObject*) codeobj;
 #if PY_VERSION_HEX >= 0x030b00a2
+  #if PY_VERSION_HEX >= 0x030C00b1
+  #define __Pyx_IsTracing(tstate, check_tracing, check_funcs)\
+     ((!(check_tracing) || !(tstate)->tracing) &&\
+         (!(check_funcs) || (tstate)->c_profilefunc || (CYTHON_TRACE && (tstate)->c_tracefunc)))
+  #else
   #define __Pyx_IsTracing(tstate, check_tracing, check_funcs)\
      (unlikely((tstate)->cframe->use_tracing) &&\
          (!(check_tracing) || !(tstate)->tracing) &&\
          (!(check_funcs) || (tstate)->c_profilefunc || (CYTHON_TRACE && (tstate)->c_tracefunc)))
-  #define __Pyx_EnterTracing(tstate) PyThreadState_EnterTracing(tstate)
-  #define __Pyx_LeaveTracing(tstate) PyThreadState_LeaveTracing(tstate)
+  #endif
+  #define __Pyx_EnterTracing(tstate)  PyThreadState_EnterTracing(tstate)
+  #define __Pyx_LeaveTracing(tstate)  PyThreadState_LeaveTracing(tstate)
 #elif PY_VERSION_HEX >= 0x030a00b1
   #define __Pyx_IsTracing(tstate, check_tracing, check_funcs)\
      (unlikely((tstate)->cframe->use_tracing) &&\
          (!(check_tracing) || !(tstate)->tracing) &&\
          (!(check_funcs) || (tstate)->c_profilefunc || (CYTHON_TRACE && (tstate)->c_tracefunc)))
   #define __Pyx_EnterTracing(tstate)\
       do { tstate->tracing++; tstate->cframe->use_tracing = 0; } while (0)
@@ -2054,30 +2065,30 @@
     const char* function_name);
 
 /* RaiseArgTupleInvalid.proto */
 static void __Pyx_RaiseArgtupleInvalid(const char* func_name, int exact,
     Py_ssize_t num_min, Py_ssize_t num_max, Py_ssize_t num_found);
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto_3_0_0b3
-#define __PYX_HAVE_RT_ImportType_proto_3_0_0b3
+#ifndef __PYX_HAVE_RT_ImportType_proto_3_0_0
+#define __PYX_HAVE_RT_ImportType_proto_3_0_0
 #if defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L
 #include <stdalign.h>
 #endif
 #if (defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L) || __cplusplus >= 201103L
-#define __PYX_GET_STRUCT_ALIGNMENT_3_0_0b3(s) alignof(s)
+#define __PYX_GET_STRUCT_ALIGNMENT_3_0_0(s) alignof(s)
 #else
-#define __PYX_GET_STRUCT_ALIGNMENT_3_0_0b3(s) sizeof(void*)
+#define __PYX_GET_STRUCT_ALIGNMENT_3_0_0(s) sizeof(void*)
 #endif
-enum __Pyx_ImportType_CheckSize_3_0_0b3 {
-   __Pyx_ImportType_CheckSize_Error_3_0_0b3 = 0,
-   __Pyx_ImportType_CheckSize_Warn_3_0_0b3 = 1,
-   __Pyx_ImportType_CheckSize_Ignore_3_0_0b3 = 2
+enum __Pyx_ImportType_CheckSize_3_0_0 {
+   __Pyx_ImportType_CheckSize_Error_3_0_0 = 0,
+   __Pyx_ImportType_CheckSize_Warn_3_0_0 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_3_0_0 = 2
 };
-static PyTypeObject *__Pyx_ImportType_3_0_0b3(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_0b3 check_size);
+static PyTypeObject *__Pyx_ImportType_3_0_0(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_0 check_size);
 #endif
 
 /* Import.proto */
 static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level);
 
 /* ImportFrom.proto */
 static PyObject* __Pyx_ImportFrom(PyObject* module, PyObject* name);
@@ -3305,17 +3316,17 @@
  *         s_proc.data = NULL
  */
     __Pyx_TraceLine(291,0,__PYX_ERR(0, 291, __pyx_L6_except_error))
     __pyx_t_13 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_13) {
       __Pyx_AddTraceback("cpp_common.hash_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_1, &__pyx_t_14, &__pyx_t_15) < 0) __PYX_ERR(0, 291, __pyx_L6_except_error)
-      __Pyx_GOTREF(__pyx_t_1);
-      __Pyx_GOTREF(__pyx_t_14);
-      __Pyx_GOTREF(__pyx_t_15);
+      __Pyx_XGOTREF(__pyx_t_1);
+      __Pyx_XGOTREF(__pyx_t_14);
+      __Pyx_XGOTREF(__pyx_t_15);
       __Pyx_INCREF(__pyx_t_14);
       __pyx_v_e = __pyx_t_14;
       /*try:*/ {
 
         /* "cpp_common.pxd":292
  *                 (<uint64_t*>s_proc.data)[i] = <uint64_t>hash(arr[i])
  *     except Exception as e:
@@ -3722,17 +3733,17 @@
  *         s_proc.data = NULL
  */
     __Pyx_TraceLine(320,0,__PYX_ERR(0, 320, __pyx_L6_except_error))
     __pyx_t_13 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_13) {
       __Pyx_AddTraceback("cpp_common.hash_sequence", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_9, &__pyx_t_14, &__pyx_t_15) < 0) __PYX_ERR(0, 320, __pyx_L6_except_error)
-      __Pyx_GOTREF(__pyx_t_9);
-      __Pyx_GOTREF(__pyx_t_14);
-      __Pyx_GOTREF(__pyx_t_15);
+      __Pyx_XGOTREF(__pyx_t_9);
+      __Pyx_XGOTREF(__pyx_t_14);
+      __Pyx_XGOTREF(__pyx_t_15);
       __Pyx_INCREF(__pyx_t_14);
       __pyx_v_e = __pyx_t_14;
       /*try:*/ {
 
         /* "cpp_common.pxd":321
  *                 (<uint64_t*>s_proc.data)[i] = <uint64_t>hash(elem)
  *     except Exception as e:
@@ -5654,17 +5665,17 @@
  *         if proc_str.dtor:
  *             proc_str.dtor(&proc_str)
  */
     __Pyx_TraceLine(37,0,__PYX_ERR(1, 37, __pyx_L5_except_error))
     /*except:*/ {
       __Pyx_AddTraceback("rapidfuzz.utils_cpp.default_process_capi", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 37, __pyx_L5_except_error)
-      __Pyx_GOTREF(__pyx_t_5);
-      __Pyx_GOTREF(__pyx_t_6);
-      __Pyx_GOTREF(__pyx_t_7);
+      __Pyx_XGOTREF(__pyx_t_5);
+      __Pyx_XGOTREF(__pyx_t_6);
+      __Pyx_XGOTREF(__pyx_t_7);
 
       /* "rapidfuzz/utils_cpp.pyx":38
  *         proc_str = default_process_func(proc_str)
  *     except:
  *         if proc_str.dtor:             # <<<<<<<<<<<<<<
  *             proc_str.dtor(&proc_str)
  *         raise
@@ -5914,23 +5925,23 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_3_0_0b3(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
+  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_3_0_0(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0b3(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(PyTypeObject),
   #elif CYTHON_COMPILING_IN_LIMITED_API
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0b3(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0b3(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(PyHeapTypeObject),
   #endif
-  __Pyx_ImportType_CheckSize_Warn_3_0_0b3); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(2, 9, __pyx_L1_error)
+  __Pyx_ImportType_CheckSize_Warn_3_0_0); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(2, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -8216,18 +8227,18 @@
     PyErr_Format(PyExc_TypeError,
                  "%.200s() takes %.8s %" CYTHON_FORMAT_SSIZE_T "d positional argument%.1s (%" CYTHON_FORMAT_SSIZE_T "d given)",
                  func_name, more_or_less, num_expected,
                  (num_expected == 1) ? "" : "s", num_found);
 }
 
 /* TypeImport */
-#ifndef __PYX_HAVE_RT_ImportType_3_0_0b3
-#define __PYX_HAVE_RT_ImportType_3_0_0b3
-static PyTypeObject *__Pyx_ImportType_3_0_0b3(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_0b3 check_size)
+#ifndef __PYX_HAVE_RT_ImportType_3_0_0
+#define __PYX_HAVE_RT_ImportType_3_0_0
+static PyTypeObject *__Pyx_ImportType_3_0_0(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_0 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
     Py_ssize_t itemsize;
 #if CYTHON_COMPILING_IN_LIMITED_API
     PyObject *py_basicsize;
@@ -8273,23 +8284,23 @@
     if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize+itemsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error_3_0_0b3 &&
+    if (check_size == __Pyx_ImportType_CheckSize_Error_3_0_0 &&
             ((size_t)basicsize > size || (size_t)(basicsize + itemsize) < size)) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd-%zd from PyObject",
             module_name, class_name, size, basicsize, basicsize+itemsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn_3_0_0b3 && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_3_0_0 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
```

### Comparing `rapidfuzz-3.1.1/src/rapidfuzz/utils_cpp.hpp` & `rapidfuzz-3.1.2/src/rapidfuzz/utils_cpp.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/src/rapidfuzz/utils_cpp.pyx` & `rapidfuzz-3.1.2/src/rapidfuzz/utils_cpp.pyx`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/src/rapidfuzz/utils_py.py` & `rapidfuzz-3.1.2/src/rapidfuzz/utils_py.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/src/rapidfuzz.egg-info/PKG-INFO` & `rapidfuzz-3.1.2/src/rapidfuzz.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rapidfuzz
-Version: 3.1.1
+Version: 3.1.2
 Summary: rapid fuzzy string matching
 Home-page: https://github.com/maxbachmann/RapidFuzz
 Author: Max Bachmann
 Author-email: pypi@maxbachmann.de
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
@@ -61,14 +61,15 @@
 
 ## Description
 RapidFuzz is a fast string matching library for Python and C++, which is using the string similarity calculations from [FuzzyWuzzy](https://github.com/seatgeek/fuzzywuzzy). However there are a couple of aspects that set RapidFuzz apart from FuzzyWuzzy:
 1) It is MIT licensed so it can be used whichever License you might want to choose for your project, while you're forced to adopt the GPL license when using FuzzyWuzzy
 2) It provides many string_metrics like hamming or jaro_winkler, which are not included in FuzzyWuzzy
 3) It is mostly written in C++ and on top of this comes with a lot of Algorithmic improvements to make string matching even faster, while still providing the same results. For detailed benchmarks check the [documentation](https://maxbachmann.github.io/RapidFuzz)
 4) Fixes multiple bugs in the `partial_ratio` implementation
+5) It can be largely used as a drop in replacement for `fuzzywuzzy`. However there are a couple API differences described [here](https://github.com/maxbachmann/RapidFuzz/blob/main/api_differences.md)
 
 ## Requirements
 
 - Python 3.7 or later
 - On Windows the [Visual C++ 2019 redistributable](https://support.microsoft.com/en-us/help/2977003/the-latest-supported-visual-c-downloads) is required
 
 ## Installation
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: rapidfuzz Version: 3.1.1 Summary: rapid fuzzy
+Metadata-Version: 2.1 Name: rapidfuzz Version: 3.1.2 Summary: rapid fuzzy
 string matching Home-page: https://github.com/maxbachmann/RapidFuzz Author: Max
 Bachmann Author-email: pypi@maxbachmann.de License: MIT Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: License :: OSI
 Approved :: MIT License Requires-Python: >=3.7 Description-Content-Type: text/
@@ -21,27 +21,30 @@
 whichever License you might want to choose for your project, while you're
 forced to adopt the GPL license when using FuzzyWuzzy 2) It provides many
 string_metrics like hamming or jaro_winkler, which are not included in
 FuzzyWuzzy 3) It is mostly written in C++ and on top of this comes with a lot
 of Algorithmic improvements to make string matching even faster, while still
 providing the same results. For detailed benchmarks check the [documentation]
 (https://maxbachmann.github.io/RapidFuzz) 4) Fixes multiple bugs in the
-`partial_ratio` implementation ## Requirements - Python 3.7 or later - On
-Windows the [Visual C++ 2019 redistributable](https://support.microsoft.com/en-
-us/help/2977003/the-latest-supported-visual-c-downloads) is required ##
-Installation There are several ways to install RapidFuzz, the recommended
-methods are to either use `pip`(the Python package manager) or `conda` (an
-open-source, cross-platform, package manager) ### with pip RapidFuzz can be
-installed with `pip` the following way: ```bash pip install rapidfuzz ``` There
-are pre-built binaries (wheels) of RapidFuzz for MacOS (10.9 and later), Linux
-x86_64 and Windows. Wheels for armv6l (Raspberry Pi Zero) and armv7l (Raspberry
-Pi) are available on [piwheels](https://www.piwheels.org/project/rapidfuzz/). >
-:heavy_multiplication_x:   **failure "ImportError: DLL load failed"** > > If
-you run into this error on Windows the reason is most likely, that the [Visual
-C++ 2019 redistributable](https://support.microsoft.com/en-us/help/2977003/the-
+`partial_ratio` implementation 5) It can be largely used as a drop in
+replacement for `fuzzywuzzy`. However there are a couple API differences
+described [here](https://github.com/maxbachmann/RapidFuzz/blob/main/
+api_differences.md) ## Requirements - Python 3.7 or later - On Windows the
+[Visual C++ 2019 redistributable](https://support.microsoft.com/en-us/help/
+2977003/the-latest-supported-visual-c-downloads) is required ## Installation
+There are several ways to install RapidFuzz, the recommended methods are to
+either use `pip`(the Python package manager) or `conda` (an open-source, cross-
+platform, package manager) ### with pip RapidFuzz can be installed with `pip`
+the following way: ```bash pip install rapidfuzz ``` There are pre-built
+binaries (wheels) of RapidFuzz for MacOS (10.9 and later), Linux x86_64 and
+Windows. Wheels for armv6l (Raspberry Pi Zero) and armv7l (Raspberry Pi) are
+available on [piwheels](https://www.piwheels.org/project/rapidfuzz/). > :
+heavy_multiplication_x:   **failure "ImportError: DLL load failed"** > > If you
+run into this error on Windows the reason is most likely, that the [Visual C++
+2019 redistributable](https://support.microsoft.com/en-us/help/2977003/the-
 latest-supported-visual-c-downloads) is not installed, which is required to
 find C++ Libraries (The C++ 2019 version includes the 2015, 2017 and 2019
 version). ### with conda RapidFuzz can be installed with `conda`: ```bash conda
 install -c conda-forge rapidfuzz ``` ### from git RapidFuzz can be installed
 directly from the source distribution by cloning the repository. This requires
 a C++17 capable compiler. ```bash git clone --recursive https://github.com/
 maxbachmann/rapidfuzz.git cd rapidfuzz pip install . ``` ## Usage Some simple
```

### Comparing `rapidfuzz-3.1.1/src/rapidfuzz.egg-info/SOURCES.txt` & `rapidfuzz-3.1.2/src/rapidfuzz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/tests/common.py` & `rapidfuzz-3.1.2/tests/common.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/tests/distance/common.py` & `rapidfuzz-3.1.2/tests/distance/common.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/tests/distance/test_DamerauLevenshtein.py` & `rapidfuzz-3.1.2/tests/distance/test_DamerauLevenshtein.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/tests/distance/test_Hamming.py` & `rapidfuzz-3.1.2/tests/distance/test_Hamming.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/tests/distance/test_Indel.py` & `rapidfuzz-3.1.2/tests/distance/test_Indel.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/tests/distance/test_Jaro.py` & `rapidfuzz-3.1.2/tests/distance/test_Jaro.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/tests/distance/test_JaroWinkler.py` & `rapidfuzz-3.1.2/tests/distance/test_JaroWinkler.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/tests/distance/test_Levenshtein.py` & `rapidfuzz-3.1.2/tests/distance/test_Levenshtein.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/tests/distance/test_OSA.py` & `rapidfuzz-3.1.2/tests/distance/test_OSA.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/tests/distance/test_Postfix.py` & `rapidfuzz-3.1.2/tests/distance/test_Postfix.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/tests/distance/test_Prefix.py` & `rapidfuzz-3.1.2/tests/distance/test_Prefix.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/tests/distance/test_distance.py` & `rapidfuzz-3.1.2/tests/distance/test_distance.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/tests/distance/test_init.py` & `rapidfuzz-3.1.2/tests/distance/test_init.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/tests/test_fuzz.py` & `rapidfuzz-3.1.2/tests/test_fuzz.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/tests/test_hypothesis.py` & `rapidfuzz-3.1.2/tests/test_hypothesis.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/tests/test_process.py` & `rapidfuzz-3.1.2/tests/test_process.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.1.1/tests/test_utils.py` & `rapidfuzz-3.1.2/tests/test_utils.py`

 * *Files identical despite different names*

