# Comparing `tmp/rapidfuzz-3.9.0.tar.gz` & `tmp/rapidfuzz-3.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rapidfuzz-3.9.0.tar", last modified: Thu May  2 21:44:17 2024, max compression
+gzip compressed data, was "rapidfuzz-3.9.1.tar", last modified: Sun May 19 20:11:26 2024, max compression
```

## Comparing `rapidfuzz-3.9.0.tar` & `rapidfuzz-3.9.1.tar`

### file list

```diff
@@ -1,288 +1,288 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:44:17.796198 rapidfuzz-3.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)    31507 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3041 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      939 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    11677 2024-05-02 21:44:17.796198 rapidfuzz-3.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10972 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:44:17.740198 rapidfuzz-3.9.0/_custom_build/
--rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/_custom_build/backend.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:44:17.740198 rapidfuzz-3.9.0/cmake/
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/cmake/CheckCPUArch.c.in
--rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/cmake/CheckCPUArch.cmake
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:44:17.744198 rapidfuzz-3.9.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:44:17.744198 rapidfuzz-3.9.0/docs/Contributing/
--rw-r--r--   0 runner    (1001) docker     (127)     1844 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/docs/Contributing/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/docs/Installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/docs/License.rst
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/docs/References.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:44:17.744198 rapidfuzz-3.9.0/docs/Usage/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:44:17.744198 rapidfuzz-3.9.0/docs/Usage/distance/
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/docs/Usage/distance/DamerauLevenshtein.rst
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/docs/Usage/distance/Hamming.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/docs/Usage/distance/Indel.rst
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/docs/Usage/distance/Jaro.rst
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/docs/Usage/distance/JaroWinkler.rst
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/docs/Usage/distance/LCSseq.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3914 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/docs/Usage/distance/Levenshtein.rst
--rw-r--r--   0 runner    (1001) docker     (127)      807 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/docs/Usage/distance/OSA.rst
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/docs/Usage/distance/Postfix.rst
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/docs/Usage/distance/Prefix.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:44:17.744198 rapidfuzz-3.9.0/docs/Usage/distance/img/
--rw-r--r--   0 runner    (1001) docker     (127)    37487 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/docs/Usage/distance/img/damerau_levenshtein.svg
--rw-r--r--   0 runner    (1001) docker     (127)    42028 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/docs/Usage/distance/img/indel_levenshtein.svg
--rw-r--r--   0 runner    (1001) docker     (127)    34090 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/docs/Usage/distance/img/jaro.svg
--rw-r--r--   0 runner    (1001) docker     (127)    34913 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/docs/Usage/distance/img/jaro_winkler.svg
--rw-r--r--   0 runner    (1001) docker     (127)    37821 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/docs/Usage/distance/img/osa.svg
--rw-r--r--   0 runner    (1001) docker     (127)    32664 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/docs/Usage/distance/img/uniform_levenshtein.svg
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/docs/Usage/distance/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      920 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/docs/Usage/fuzz.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:44:17.748198 rapidfuzz-3.9.0/docs/Usage/img/
--rw-r--r--   0 runner    (1001) docker     (127)    25251 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/docs/Usage/img/WRatio.svg
--rw-r--r--   0 runner    (1001) docker     (127)    42028 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/docs/Usage/img/indel_levenshtein.svg
--rw-r--r--   0 runner    (1001) docker     (127)    41626 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/docs/Usage/img/partial_ratio_long_needle.svg
--rw-r--r--   0 runner    (1001) docker     (127)    41360 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/docs/Usage/img/partial_ratio_short_needle.svg
--rw-r--r--   0 runner    (1001) docker     (127)    28491 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/docs/Usage/img/partial_token_ratio.svg
--rw-r--r--   0 runner    (1001) docker     (127)    24769 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/docs/Usage/img/partial_token_set_ratio.svg
--rw-r--r--   0 runner    (1001) docker     (127)    25404 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/docs/Usage/img/partial_token_sort_ratio.svg
--rw-r--r--   0 runner    (1001) docker     (127)    24367 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/docs/Usage/img/ratio.svg
--rw-r--r--   0 runner    (1001) docker     (127)    27273 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/docs/Usage/img/token_ratio.svg
--rw-r--r--   0 runner    (1001) docker     (127)    25693 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/docs/Usage/img/token_set_ratio.svg
--rw-r--r--   0 runner    (1001) docker     (127)    26611 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/docs/Usage/img/token_sort_ratio.svg
--rw-r--r--   0 runner    (1001) docker     (127)    32664 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/docs/Usage/img/uniform_levenshtein.svg
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/docs/Usage/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/docs/Usage/process.rst
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/docs/Usage/utils.rst
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/docs/changelog_link.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:44:17.748198 rapidfuzz-3.9.0/docs/img/
--rw-r--r--   0 runner    (1001) docker     (127)     5879 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/docs/img/RapidFuzz.svg
--rw-r--r--   0 runner    (1001) docker     (127)    56024 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/docs/img/cdist.svg
--rw-r--r--   0 runner    (1001) docker     (127)    54183 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/docs/img/scorer.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3160 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/docs/refs.bib
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:44:17.740198 rapidfuzz-3.9.0/extern/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:44:17.748198 rapidfuzz-3.9.0/extern/rapidfuzz-cpp/
--rw-r--r--   0 runner    (1001) docker     (127)     4395 2024-05-02 21:43:48.000000 rapidfuzz-3.9.0/extern/rapidfuzz-cpp/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-02 21:43:48.000000 rapidfuzz-3.9.0/extern/rapidfuzz-cpp/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:44:17.748198 rapidfuzz-3.9.0/extern/rapidfuzz-cpp/rapidfuzz/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:44:17.752198 rapidfuzz-3.9.0/extern/rapidfuzz-cpp/rapidfuzz/details/
--rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-05-02 21:43:48.000000 rapidfuzz-3.9.0/extern/rapidfuzz-cpp/rapidfuzz/details/CharSet.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     4855 2024-05-02 21:43:48.000000 rapidfuzz-3.9.0/extern/rapidfuzz-cpp/rapidfuzz/details/GrowingHashmap.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     4540 2024-05-02 21:43:48.000000 rapidfuzz-3.9.0/extern/rapidfuzz-cpp/rapidfuzz/details/Matrix.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     5510 2024-05-02 21:43:48.000000 rapidfuzz-3.9.0/extern/rapidfuzz-cpp/rapidfuzz/details/PatternMatchVector.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     5515 2024-05-02 21:43:48.000000 rapidfuzz-3.9.0/extern/rapidfuzz-cpp/rapidfuzz/details/Range.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-05-02 21:43:48.000000 rapidfuzz-3.9.0/extern/rapidfuzz-cpp/rapidfuzz/details/SplittedSentenceView.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2817 2024-05-02 21:43:48.000000 rapidfuzz-3.9.0/extern/rapidfuzz-cpp/rapidfuzz/details/common.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     4314 2024-05-02 21:43:48.000000 rapidfuzz-3.9.0/extern/rapidfuzz-cpp/rapidfuzz/details/common_impl.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    23194 2024-05-02 21:43:48.000000 rapidfuzz-3.9.0/extern/rapidfuzz-cpp/rapidfuzz/details/distance.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     5265 2024-05-02 21:43:48.000000 rapidfuzz-3.9.0/extern/rapidfuzz-cpp/rapidfuzz/details/intrinsics.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-05-02 21:43:48.000000 rapidfuzz-3.9.0/extern/rapidfuzz-cpp/rapidfuzz/details/simd.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    17962 2024-05-02 21:43:48.000000 rapidfuzz-3.9.0/extern/rapidfuzz-cpp/rapidfuzz/details/simd_avx2.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    16290 2024-05-02 21:43:48.000000 rapidfuzz-3.9.0/extern/rapidfuzz-cpp/rapidfuzz/details/simd_sse2.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-05-02 21:43:48.000000 rapidfuzz-3.9.0/extern/rapidfuzz-cpp/rapidfuzz/details/type_traits.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    17443 2024-05-02 21:43:48.000000 rapidfuzz-3.9.0/extern/rapidfuzz-cpp/rapidfuzz/details/types.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:44:17.756198 rapidfuzz-3.9.0/extern/rapidfuzz-cpp/rapidfuzz/distance/
--rw-r--r--   0 runner    (1001) docker     (127)     6203 2024-05-02 21:43:48.000000 rapidfuzz-3.9.0/extern/rapidfuzz-cpp/rapidfuzz/distance/DamerauLevenshtein.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     4749 2024-05-02 21:43:48.000000 rapidfuzz-3.9.0/extern/rapidfuzz-cpp/rapidfuzz/distance/DamerauLevenshtein_impl.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     6649 2024-05-02 21:43:48.000000 rapidfuzz-3.9.0/extern/rapidfuzz-cpp/rapidfuzz/distance/Hamming.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-05-02 21:43:48.000000 rapidfuzz-3.9.0/extern/rapidfuzz-cpp/rapidfuzz/distance/Hamming_impl.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     6480 2024-05-02 21:43:48.000000 rapidfuzz-3.9.0/extern/rapidfuzz-cpp/rapidfuzz/distance/Indel.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3017 2024-05-02 21:43:48.000000 rapidfuzz-3.9.0/extern/rapidfuzz-cpp/rapidfuzz/distance/Indel_impl.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     7537 2024-05-02 21:43:48.000000 rapidfuzz-3.9.0/extern/rapidfuzz-cpp/rapidfuzz/distance/Jaro.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     8008 2024-05-02 21:43:48.000000 rapidfuzz-3.9.0/extern/rapidfuzz-cpp/rapidfuzz/distance/JaroWinkler.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3054 2024-05-02 21:43:48.000000 rapidfuzz-3.9.0/extern/rapidfuzz-cpp/rapidfuzz/distance/JaroWinkler_impl.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    30315 2024-05-02 21:43:48.000000 rapidfuzz-3.9.0/extern/rapidfuzz-cpp/rapidfuzz/distance/Jaro_impl.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     8100 2024-05-02 21:43:48.000000 rapidfuzz-3.9.0/extern/rapidfuzz-cpp/rapidfuzz/distance/LCSseq.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    18309 2024-05-02 21:43:48.000000 rapidfuzz-3.9.0/extern/rapidfuzz-cpp/rapidfuzz/distance/LCSseq_impl.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    20702 2024-05-02 21:43:48.000000 rapidfuzz-3.9.0/extern/rapidfuzz-cpp/rapidfuzz/distance/Levenshtein.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    45010 2024-05-02 21:43:48.000000 rapidfuzz-3.9.0/extern/rapidfuzz-cpp/rapidfuzz/distance/Levenshtein_impl.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     9556 2024-05-02 21:43:48.000000 rapidfuzz-3.9.0/extern/rapidfuzz-cpp/rapidfuzz/distance/OSA.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     9776 2024-05-02 21:43:48.000000 rapidfuzz-3.9.0/extern/rapidfuzz-cpp/rapidfuzz/distance/OSA_impl.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3904 2024-05-02 21:43:48.000000 rapidfuzz-3.9.0/extern/rapidfuzz-cpp/rapidfuzz/distance/Postfix.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-05-02 21:43:48.000000 rapidfuzz-3.9.0/extern/rapidfuzz-cpp/rapidfuzz/distance/Postfix_impl.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3831 2024-05-02 21:43:48.000000 rapidfuzz-3.9.0/extern/rapidfuzz-cpp/rapidfuzz/distance/Prefix.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-05-02 21:43:48.000000 rapidfuzz-3.9.0/extern/rapidfuzz-cpp/rapidfuzz/distance/Prefix_impl.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3833 2024-05-02 21:43:48.000000 rapidfuzz-3.9.0/extern/rapidfuzz-cpp/rapidfuzz/distance.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    27628 2024-05-02 21:43:48.000000 rapidfuzz-3.9.0/extern/rapidfuzz-cpp/rapidfuzz/fuzz.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    37942 2024-05-02 21:43:48.000000 rapidfuzz-3.9.0/extern/rapidfuzz-cpp/rapidfuzz/fuzz_impl.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-02 21:43:48.000000 rapidfuzz-3.9.0/extern/rapidfuzz-cpp/rapidfuzz/rapidfuzz_all.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:44:17.756198 rapidfuzz-3.9.0/extern/taskflow/
--rw-r--r--   0 runner    (1001) docker     (127)    14095 2024-05-02 21:43:49.000000 rapidfuzz-3.9.0/extern/taskflow/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-05-02 21:43:49.000000 rapidfuzz-3.9.0/extern/taskflow/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-05-02 21:43:49.000000 rapidfuzz-3.9.0/extern/taskflow/TaskflowConfig.cmake.in
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:44:17.756198 rapidfuzz-3.9.0/extern/taskflow/taskflow/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:44:17.756198 rapidfuzz-3.9.0/extern/taskflow/taskflow/algorithm/
--rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-05-02 21:43:49.000000 rapidfuzz-3.9.0/extern/taskflow/taskflow/algorithm/critical.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    16653 2024-05-02 21:43:49.000000 rapidfuzz-3.9.0/extern/taskflow/taskflow/algorithm/data_pipeline.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    14972 2024-05-02 21:43:49.000000 rapidfuzz-3.9.0/extern/taskflow/taskflow/algorithm/find.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     4928 2024-05-02 21:43:49.000000 rapidfuzz-3.9.0/extern/taskflow/taskflow/algorithm/for_each.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-02 21:43:49.000000 rapidfuzz-3.9.0/extern/taskflow/taskflow/algorithm/launch.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    14524 2024-05-02 21:43:49.000000 rapidfuzz-3.9.0/extern/taskflow/taskflow/algorithm/partitioner.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    44892 2024-05-02 21:43:49.000000 rapidfuzz-3.9.0/extern/taskflow/taskflow/algorithm/pipeline.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     7902 2024-05-02 21:43:49.000000 rapidfuzz-3.9.0/extern/taskflow/taskflow/algorithm/reduce.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    17090 2024-05-02 21:43:49.000000 rapidfuzz-3.9.0/extern/taskflow/taskflow/algorithm/scan.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    20947 2024-05-02 21:43:49.000000 rapidfuzz-3.9.0/extern/taskflow/taskflow/algorithm/sort.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     5870 2024-05-02 21:43:49.000000 rapidfuzz-3.9.0/extern/taskflow/taskflow/algorithm/transform.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:44:17.760198 rapidfuzz-3.9.0/extern/taskflow/taskflow/core/
--rw-r--r--   0 runner    (1001) docker     (127)    10955 2024-05-02 21:43:49.000000 rapidfuzz-3.9.0/extern/taskflow/taskflow/core/async.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3082 2024-05-02 21:43:49.000000 rapidfuzz-3.9.0/extern/taskflow/taskflow/core/async_task.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-02 21:43:49.000000 rapidfuzz-3.9.0/extern/taskflow/taskflow/core/declarations.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-02 21:43:49.000000 rapidfuzz-3.9.0/extern/taskflow/taskflow/core/environment.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-05-02 21:43:49.000000 rapidfuzz-3.9.0/extern/taskflow/taskflow/core/error.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    54781 2024-05-02 21:43:49.000000 rapidfuzz-3.9.0/extern/taskflow/taskflow/core/executor-module-opt.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    66789 2024-05-02 21:43:49.000000 rapidfuzz-3.9.0/extern/taskflow/taskflow/core/executor.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    41751 2024-05-02 21:43:49.000000 rapidfuzz-3.9.0/extern/taskflow/taskflow/core/flow_builder.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    24153 2024-05-02 21:43:49.000000 rapidfuzz-3.9.0/extern/taskflow/taskflow/core/graph.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     9176 2024-05-02 21:43:49.000000 rapidfuzz-3.9.0/extern/taskflow/taskflow/core/notifier.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    26126 2024-05-02 21:43:49.000000 rapidfuzz-3.9.0/extern/taskflow/taskflow/core/observer.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3441 2024-05-02 21:43:49.000000 rapidfuzz-3.9.0/extern/taskflow/taskflow/core/semaphore.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    18519 2024-05-02 21:43:49.000000 rapidfuzz-3.9.0/extern/taskflow/taskflow/core/task.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    15758 2024-05-02 21:43:49.000000 rapidfuzz-3.9.0/extern/taskflow/taskflow/core/taskflow.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-02 21:43:49.000000 rapidfuzz-3.9.0/extern/taskflow/taskflow/core/topology.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    12210 2024-05-02 21:43:49.000000 rapidfuzz-3.9.0/extern/taskflow/taskflow/core/tsq.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     6624 2024-05-02 21:43:49.000000 rapidfuzz-3.9.0/extern/taskflow/taskflow/core/worker.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-05-02 21:43:49.000000 rapidfuzz-3.9.0/extern/taskflow/taskflow/taskflow.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:44:17.764198 rapidfuzz-3.9.0/extern/taskflow/taskflow/utility/
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-02 21:43:49.000000 rapidfuzz-3.9.0/extern/taskflow/taskflow/utility/iterator.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-02 21:43:49.000000 rapidfuzz-3.9.0/extern/taskflow/taskflow/utility/macros.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3815 2024-05-02 21:43:49.000000 rapidfuzz-3.9.0/extern/taskflow/taskflow/utility/math.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    19899 2024-05-02 21:43:49.000000 rapidfuzz-3.9.0/extern/taskflow/taskflow/utility/object_pool.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     4239 2024-05-02 21:43:49.000000 rapidfuzz-3.9.0/extern/taskflow/taskflow/utility/os.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    29321 2024-05-02 21:43:49.000000 rapidfuzz-3.9.0/extern/taskflow/taskflow/utility/serializer.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-02 21:43:49.000000 rapidfuzz-3.9.0/extern/taskflow/taskflow/utility/singleton.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    31329 2024-05-02 21:43:49.000000 rapidfuzz-3.9.0/extern/taskflow/taskflow/utility/small_vector.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-05-02 21:43:49.000000 rapidfuzz-3.9.0/extern/taskflow/taskflow/utility/stream.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     8631 2024-05-02 21:43:49.000000 rapidfuzz-3.9.0/extern/taskflow/taskflow/utility/traits.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     5685 2024-05-02 21:43:49.000000 rapidfuzz-3.9.0/extern/taskflow/taskflow/utility/uuid.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-05-02 21:44:14.000000 rapidfuzz-3.9.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 21:44:17.796198 rapidfuzz-3.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:44:17.740198 rapidfuzz-3.9.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:44:17.776198 rapidfuzz-3.9.0/src/rapidfuzz/
--rw-r--r--   0 runner    (1001) docker     (127)     7447 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/src/rapidfuzz/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:44:17.776198 rapidfuzz-3.9.0/src/rapidfuzz/FeatureDetector/
--rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/src/rapidfuzz/FeatureDetector/CpuInfo.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/src/rapidfuzz/FeatureDetector/CpuInfo.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2991 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/src/rapidfuzz/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/src/rapidfuzz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/src/rapidfuzz/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:44:17.776198 rapidfuzz-3.9.0/src/rapidfuzz/__pyinstaller/
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/src/rapidfuzz/__pyinstaller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/src/rapidfuzz/__pyinstaller/hook-rapidfuzz.py
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/src/rapidfuzz/__pyinstaller/test_rapidfuzz_packaging.py
--rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/src/rapidfuzz/_common_py.py
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/src/rapidfuzz/_feature_detector.py
--rw-r--r--   0 runner    (1001) docker     (127)   266395 2024-05-02 21:44:10.000000 rapidfuzz-3.9.0/src/rapidfuzz/_feature_detector_cpp.cxx
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/src/rapidfuzz/_feature_detector_cpp.pyx
--rw-r--r--   0 runner    (1001) docker     (127)     4027 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/src/rapidfuzz/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    25736 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/src/rapidfuzz/cpp_common.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    17473 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/src/rapidfuzz/cpp_common.pxd
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:44:17.792198 rapidfuzz-3.9.0/src/rapidfuzz/distance/
--rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/src/rapidfuzz/distance/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/src/rapidfuzz/distance/DamerauLevenshtein.py
--rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/src/rapidfuzz/distance/DamerauLevenshtein.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6591 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/src/rapidfuzz/distance/DamerauLevenshtein_py.py
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/src/rapidfuzz/distance/Hamming.py
--rw-r--r--   0 runner    (1001) docker     (127)     2742 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/src/rapidfuzz/distance/Hamming.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9081 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/src/rapidfuzz/distance/Hamming_py.py
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/src/rapidfuzz/distance/Indel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2566 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/src/rapidfuzz/distance/Indel.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10034 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/src/rapidfuzz/distance/Indel_py.py
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/src/rapidfuzz/distance/Jaro.py
--rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/src/rapidfuzz/distance/Jaro.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/src/rapidfuzz/distance/JaroWinkler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/src/rapidfuzz/distance/JaroWinkler.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6481 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/src/rapidfuzz/distance/JaroWinkler_py.py
--rw-r--r--   0 runner    (1001) docker     (127)     7345 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/src/rapidfuzz/distance/Jaro_py.py
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/src/rapidfuzz/distance/LCSseq.py
--rw-r--r--   0 runner    (1001) docker     (127)     2566 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/src/rapidfuzz/distance/LCSseq.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    11504 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/src/rapidfuzz/distance/LCSseq_py.py
--rw-r--r--   0 runner    (1001) docker     (127)      836 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/src/rapidfuzz/distance/Levenshtein.py
--rw-r--r--   0 runner    (1001) docker     (127)     3651 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/src/rapidfuzz/distance/Levenshtein.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    17103 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/src/rapidfuzz/distance/Levenshtein_py.py
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/src/rapidfuzz/distance/OSA.py
--rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/src/rapidfuzz/distance/OSA.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6251 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/src/rapidfuzz/distance/OSA_py.py
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/src/rapidfuzz/distance/Postfix.py
--rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/src/rapidfuzz/distance/Postfix.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5039 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/src/rapidfuzz/distance/Postfix_py.py
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/src/rapidfuzz/distance/Prefix.py
--rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/src/rapidfuzz/distance/Prefix.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5015 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/src/rapidfuzz/distance/Prefix_py.py
--rw-r--r--   0 runner    (1001) docker     (127)      621 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/src/rapidfuzz/distance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/src/rapidfuzz/distance/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/src/rapidfuzz/distance/_initialize.py
--rw-r--r--   0 runner    (1001) docker     (127)     3989 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/src/rapidfuzz/distance/_initialize.pyi
--rw-r--r--   0 runner    (1001) docker     (127)  1693935 2024-05-02 21:44:11.000000 rapidfuzz-3.9.0/src/rapidfuzz/distance/_initialize_cpp.cxx
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/src/rapidfuzz/distance/_initialize_cpp.pxd
--rw-r--r--   0 runner    (1001) docker     (127)    29674 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/src/rapidfuzz/distance/_initialize_cpp.pyx
--rw-r--r--   0 runner    (1001) docker     (127)    26320 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/src/rapidfuzz/distance/_initialize_py.py
--rw-r--r--   0 runner    (1001) docker     (127)    49089 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/src/rapidfuzz/distance/metrics.hpp
--rw-r--r--   0 runner    (1001) docker     (127)  1506049 2024-05-02 21:44:12.000000 rapidfuzz-3.9.0/src/rapidfuzz/distance/metrics_cpp.cxx
--rw-r--r--   0 runner    (1001) docker     (127)    62949 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/src/rapidfuzz/distance/metrics_cpp.pyx
--rw-r--r--   0 runner    (1001) docker     (127)  1514092 2024-05-02 21:44:13.000000 rapidfuzz-3.9.0/src/rapidfuzz/distance/metrics_cpp_avx2.cxx
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/src/rapidfuzz/distance/metrics_cpp_avx2.pyx
--rw-r--r--   0 runner    (1001) docker     (127)  1514092 2024-05-02 21:44:14.000000 rapidfuzz-3.9.0/src/rapidfuzz/distance/metrics_cpp_sse2.cxx
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/src/rapidfuzz/distance/metrics_cpp_sse2.pyx
--rw-r--r--   0 runner    (1001) docker     (127)    10624 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/src/rapidfuzz/distance/metrics_py.py
--rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/src/rapidfuzz/fuzz.py
--rw-r--r--   0 runner    (1001) docker     (127)     4784 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/src/rapidfuzz/fuzz.pyi
--rw-r--r--   0 runner    (1001) docker     (127)   678100 2024-05-02 21:44:06.000000 rapidfuzz-3.9.0/src/rapidfuzz/fuzz_cpp.cxx
--rw-r--r--   0 runner    (1001) docker     (127)     9678 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/src/rapidfuzz/fuzz_cpp.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    11635 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/src/rapidfuzz/fuzz_cpp.pyx
--rw-r--r--   0 runner    (1001) docker     (127)   680081 2024-05-02 21:44:07.000000 rapidfuzz-3.9.0/src/rapidfuzz/fuzz_cpp_avx2.cxx
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/src/rapidfuzz/fuzz_cpp_avx2.pyx
--rw-r--r--   0 runner    (1001) docker     (127)   680081 2024-05-02 21:44:07.000000 rapidfuzz-3.9.0/src/rapidfuzz/fuzz_cpp_sse2.cxx
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/src/rapidfuzz/fuzz_cpp_sse2.pyx
--rw-r--r--   0 runner    (1001) docker     (127)    25530 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/src/rapidfuzz/fuzz_py.py
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/src/rapidfuzz/process.py
--rw-r--r--   0 runner    (1001) docker     (127)    16771 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/src/rapidfuzz/process.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    23286 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/src/rapidfuzz/process_cpp.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/src/rapidfuzz/process_cpp.py
--rw-r--r--   0 runner    (1001) docker     (127)  2151605 2024-05-02 21:44:09.000000 rapidfuzz-3.9.0/src/rapidfuzz/process_cpp_impl.cxx
--rw-r--r--   0 runner    (1001) docker     (127)    79018 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/src/rapidfuzz/process_cpp_impl.pyx
--rw-r--r--   0 runner    (1001) docker     (127)    26688 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/src/rapidfuzz/process_py.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/src/rapidfuzz/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     7782 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/src/rapidfuzz/rapidfuzz.h
--rw-r--r--   0 runner    (1001) docker     (127)   293266 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/src/rapidfuzz/unicodetype_db.h
--rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/src/rapidfuzz/utils.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/src/rapidfuzz/utils.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/src/rapidfuzz/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/src/rapidfuzz/utils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)   502929 2024-05-02 21:44:09.000000 rapidfuzz-3.9.0/src/rapidfuzz/utils_cpp.cxx
--rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/src/rapidfuzz/utils_cpp.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/src/rapidfuzz/utils_cpp.pyx
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/src/rapidfuzz/utils_py.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:44:17.796198 rapidfuzz-3.9.0/src/rapidfuzz.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11677 2024-05-02 21:44:17.000000 rapidfuzz-3.9.0/src/rapidfuzz.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9502 2024-05-02 21:44:17.000000 rapidfuzz-3.9.0/src/rapidfuzz.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 21:44:17.000000 rapidfuzz-3.9.0/src/rapidfuzz.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-02 21:44:17.000000 rapidfuzz-3.9.0/src/rapidfuzz.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-02 21:44:17.000000 rapidfuzz-3.9.0/src/rapidfuzz.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-02 21:44:17.000000 rapidfuzz-3.9.0/src/rapidfuzz.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:44:17.792198 rapidfuzz-3.9.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15407 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/tests/common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:44:17.796198 rapidfuzz-3.9.0/tests/distance/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/tests/distance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4855 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/tests/distance/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/tests/distance/test_DamerauLevenshtein.py
--rw-r--r--   0 runner    (1001) docker     (127)     3185 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/tests/distance/test_Hamming.py
--rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/tests/distance/test_Indel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/tests/distance/test_Jaro.py
--rw-r--r--   0 runner    (1001) docker     (127)     2717 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/tests/distance/test_JaroWinkler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/tests/distance/test_LCSseq.py
--rw-r--r--   0 runner    (1001) docker     (127)     4665 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/tests/distance/test_Levenshtein.py
--rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/tests/distance/test_OSA.py
--rw-r--r--   0 runner    (1001) docker     (127)      984 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/tests/distance/test_Postfix.py
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/tests/distance/test_Prefix.py
--rw-r--r--   0 runner    (1001) docker     (127)     3988 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/tests/distance/test_distance.py
--rw-r--r--   0 runner    (1001) docker     (127)    10165 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/tests/distance/test_init.py
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/tests/test_cpp_fallback.py
--rw-r--r--   0 runner    (1001) docker     (127)    12939 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/tests/test_fuzz.py
--rw-r--r--   0 runner    (1001) docker     (127)    14447 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/tests/test_hypothesis.py
--rw-r--r--   0 runner    (1001) docker     (127)    26380 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/tests/test_process.py
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/tests/test_pure_python_fallback.py
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-02 21:43:45.000000 rapidfuzz-3.9.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:11:26.954500 rapidfuzz-3.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    31645 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3041 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    11677 2024-05-19 20:11:26.954500 rapidfuzz-3.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10972 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:11:26.894500 rapidfuzz-3.9.1/_custom_build/
+-rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/_custom_build/backend.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:11:26.894500 rapidfuzz-3.9.1/cmake/
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/cmake/CheckCPUArch.c.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/cmake/CheckCPUArch.cmake
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:11:26.894500 rapidfuzz-3.9.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:11:26.894500 rapidfuzz-3.9.1/docs/Contributing/
+-rw-r--r--   0 runner    (1001) docker     (127)     1844 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/docs/Contributing/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/docs/Installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/docs/License.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/docs/References.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:11:26.894500 rapidfuzz-3.9.1/docs/Usage/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:11:26.898500 rapidfuzz-3.9.1/docs/Usage/distance/
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/docs/Usage/distance/DamerauLevenshtein.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/docs/Usage/distance/Hamming.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/docs/Usage/distance/Indel.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/docs/Usage/distance/Jaro.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/docs/Usage/distance/JaroWinkler.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/docs/Usage/distance/LCSseq.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3914 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/docs/Usage/distance/Levenshtein.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/docs/Usage/distance/OSA.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/docs/Usage/distance/Postfix.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/docs/Usage/distance/Prefix.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:11:26.898500 rapidfuzz-3.9.1/docs/Usage/distance/img/
+-rw-r--r--   0 runner    (1001) docker     (127)    37487 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/docs/Usage/distance/img/damerau_levenshtein.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    42028 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/docs/Usage/distance/img/indel_levenshtein.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    34090 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/docs/Usage/distance/img/jaro.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    34913 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/docs/Usage/distance/img/jaro_winkler.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    37821 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/docs/Usage/distance/img/osa.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    32664 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/docs/Usage/distance/img/uniform_levenshtein.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/docs/Usage/distance/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/docs/Usage/fuzz.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:11:26.902500 rapidfuzz-3.9.1/docs/Usage/img/
+-rw-r--r--   0 runner    (1001) docker     (127)    25251 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/docs/Usage/img/WRatio.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    42028 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/docs/Usage/img/indel_levenshtein.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    41626 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/docs/Usage/img/partial_ratio_long_needle.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    41360 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/docs/Usage/img/partial_ratio_short_needle.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    28491 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/docs/Usage/img/partial_token_ratio.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    24769 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/docs/Usage/img/partial_token_set_ratio.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    25404 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/docs/Usage/img/partial_token_sort_ratio.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    24367 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/docs/Usage/img/ratio.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    27273 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/docs/Usage/img/token_ratio.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    25693 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/docs/Usage/img/token_set_ratio.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    26611 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/docs/Usage/img/token_sort_ratio.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    32664 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/docs/Usage/img/uniform_levenshtein.svg
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/docs/Usage/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/docs/Usage/process.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/docs/Usage/utils.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/docs/changelog_link.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:11:26.902500 rapidfuzz-3.9.1/docs/img/
+-rw-r--r--   0 runner    (1001) docker     (127)     5879 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/docs/img/RapidFuzz.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    56024 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/docs/img/cdist.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    54183 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/docs/img/scorer.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3160 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/docs/refs.bib
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:11:26.890500 rapidfuzz-3.9.1/extern/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:11:26.902500 rapidfuzz-3.9.1/extern/rapidfuzz-cpp/
+-rw-r--r--   0 runner    (1001) docker     (127)     4395 2024-05-19 20:10:59.000000 rapidfuzz-3.9.1/extern/rapidfuzz-cpp/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-19 20:10:59.000000 rapidfuzz-3.9.1/extern/rapidfuzz-cpp/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:11:26.902500 rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:11:26.906500 rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/details/
+-rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-05-19 20:10:59.000000 rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/details/CharSet.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4855 2024-05-19 20:10:59.000000 rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/details/GrowingHashmap.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4540 2024-05-19 20:10:59.000000 rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/details/Matrix.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5510 2024-05-19 20:10:59.000000 rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/details/PatternMatchVector.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5515 2024-05-19 20:10:59.000000 rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/details/Range.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-05-19 20:10:59.000000 rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/details/SplittedSentenceView.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2817 2024-05-19 20:10:59.000000 rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/details/common.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4314 2024-05-19 20:10:59.000000 rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/details/common_impl.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    23194 2024-05-19 20:10:59.000000 rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/details/distance.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5265 2024-05-19 20:10:59.000000 rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/details/intrinsics.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-05-19 20:10:59.000000 rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/details/simd.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    17962 2024-05-19 20:10:59.000000 rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/details/simd_avx2.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    16290 2024-05-19 20:10:59.000000 rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/details/simd_sse2.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-05-19 20:10:59.000000 rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/details/type_traits.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    17443 2024-05-19 20:10:59.000000 rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/details/types.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:11:26.906500 rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/distance/
+-rw-r--r--   0 runner    (1001) docker     (127)     6203 2024-05-19 20:10:59.000000 rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/distance/DamerauLevenshtein.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4749 2024-05-19 20:10:59.000000 rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/distance/DamerauLevenshtein_impl.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6649 2024-05-19 20:10:59.000000 rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/distance/Hamming.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-05-19 20:10:59.000000 rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/distance/Hamming_impl.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6480 2024-05-19 20:10:59.000000 rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/distance/Indel.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3017 2024-05-19 20:10:59.000000 rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/distance/Indel_impl.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7537 2024-05-19 20:10:59.000000 rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/distance/Jaro.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8008 2024-05-19 20:10:59.000000 rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/distance/JaroWinkler.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3054 2024-05-19 20:10:59.000000 rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/distance/JaroWinkler_impl.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    30315 2024-05-19 20:10:59.000000 rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/distance/Jaro_impl.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8100 2024-05-19 20:10:59.000000 rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/distance/LCSseq.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    18309 2024-05-19 20:10:59.000000 rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/distance/LCSseq_impl.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    20702 2024-05-19 20:10:59.000000 rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/distance/Levenshtein.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    45010 2024-05-19 20:10:59.000000 rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/distance/Levenshtein_impl.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     9556 2024-05-19 20:10:59.000000 rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/distance/OSA.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     9776 2024-05-19 20:10:59.000000 rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/distance/OSA_impl.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3904 2024-05-19 20:10:59.000000 rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/distance/Postfix.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-05-19 20:10:59.000000 rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/distance/Postfix_impl.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3831 2024-05-19 20:10:59.000000 rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/distance/Prefix.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-05-19 20:10:59.000000 rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/distance/Prefix_impl.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3833 2024-05-19 20:10:59.000000 rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/distance.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    27628 2024-05-19 20:10:59.000000 rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/fuzz.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    37942 2024-05-19 20:10:59.000000 rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/fuzz_impl.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-19 20:10:59.000000 rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/rapidfuzz_all.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:11:26.910500 rapidfuzz-3.9.1/extern/taskflow/
+-rw-r--r--   0 runner    (1001) docker     (127)    14371 2024-05-19 20:11:00.000000 rapidfuzz-3.9.1/extern/taskflow/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-05-19 20:11:00.000000 rapidfuzz-3.9.1/extern/taskflow/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-05-19 20:11:00.000000 rapidfuzz-3.9.1/extern/taskflow/TaskflowConfig.cmake.in
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:11:26.910500 rapidfuzz-3.9.1/extern/taskflow/taskflow/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:11:26.910500 rapidfuzz-3.9.1/extern/taskflow/taskflow/algorithm/
+-rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-05-19 20:11:01.000000 rapidfuzz-3.9.1/extern/taskflow/taskflow/algorithm/critical.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    16653 2024-05-19 20:11:01.000000 rapidfuzz-3.9.1/extern/taskflow/taskflow/algorithm/data_pipeline.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    14616 2024-05-19 20:11:01.000000 rapidfuzz-3.9.1/extern/taskflow/taskflow/algorithm/find.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4804 2024-05-19 20:11:01.000000 rapidfuzz-3.9.1/extern/taskflow/taskflow/algorithm/for_each.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-05-19 20:11:01.000000 rapidfuzz-3.9.1/extern/taskflow/taskflow/algorithm/launch.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    21985 2024-05-19 20:11:01.000000 rapidfuzz-3.9.1/extern/taskflow/taskflow/algorithm/partitioner.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    47366 2024-05-19 20:11:01.000000 rapidfuzz-3.9.1/extern/taskflow/taskflow/algorithm/pipeline.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    12080 2024-05-19 20:11:01.000000 rapidfuzz-3.9.1/extern/taskflow/taskflow/algorithm/reduce.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    18008 2024-05-19 20:11:01.000000 rapidfuzz-3.9.1/extern/taskflow/taskflow/algorithm/scan.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    21365 2024-05-19 20:11:01.000000 rapidfuzz-3.9.1/extern/taskflow/taskflow/algorithm/sort.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5733 2024-05-19 20:11:01.000000 rapidfuzz-3.9.1/extern/taskflow/taskflow/algorithm/transform.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:11:26.914500 rapidfuzz-3.9.1/extern/taskflow/taskflow/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     9658 2024-05-19 20:11:01.000000 rapidfuzz-3.9.1/extern/taskflow/taskflow/core/async.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5007 2024-05-19 20:11:01.000000 rapidfuzz-3.9.1/extern/taskflow/taskflow/core/async_task.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-05-19 20:11:01.000000 rapidfuzz-3.9.1/extern/taskflow/taskflow/core/declarations.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-19 20:11:01.000000 rapidfuzz-3.9.1/extern/taskflow/taskflow/core/environment.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-05-19 20:11:01.000000 rapidfuzz-3.9.1/extern/taskflow/taskflow/core/error.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    54781 2024-05-19 20:11:01.000000 rapidfuzz-3.9.1/extern/taskflow/taskflow/core/executor-module-opt.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    69853 2024-05-19 20:11:01.000000 rapidfuzz-3.9.1/extern/taskflow/taskflow/core/executor.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    45123 2024-05-19 20:11:01.000000 rapidfuzz-3.9.1/extern/taskflow/taskflow/core/flow_builder.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    28114 2024-05-19 20:11:01.000000 rapidfuzz-3.9.1/extern/taskflow/taskflow/core/graph.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    10209 2024-05-19 20:11:01.000000 rapidfuzz-3.9.1/extern/taskflow/taskflow/core/notifier.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    26126 2024-05-19 20:11:01.000000 rapidfuzz-3.9.1/extern/taskflow/taskflow/core/observer.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3441 2024-05-19 20:11:01.000000 rapidfuzz-3.9.1/extern/taskflow/taskflow/core/semaphore.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    18518 2024-05-19 20:11:01.000000 rapidfuzz-3.9.1/extern/taskflow/taskflow/core/task.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    16679 2024-05-19 20:11:01.000000 rapidfuzz-3.9.1/extern/taskflow/taskflow/core/taskflow.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-05-19 20:11:01.000000 rapidfuzz-3.9.1/extern/taskflow/taskflow/core/topology.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    12210 2024-05-19 20:11:01.000000 rapidfuzz-3.9.1/extern/taskflow/taskflow/core/tsq.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4163 2024-05-19 20:11:01.000000 rapidfuzz-3.9.1/extern/taskflow/taskflow/core/worker.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-05-19 20:11:01.000000 rapidfuzz-3.9.1/extern/taskflow/taskflow/taskflow.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:11:26.918500 rapidfuzz-3.9.1/extern/taskflow/taskflow/utility/
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-05-19 20:11:01.000000 rapidfuzz-3.9.1/extern/taskflow/taskflow/utility/iterator.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-05-19 20:11:01.000000 rapidfuzz-3.9.1/extern/taskflow/taskflow/utility/macros.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3815 2024-05-19 20:11:01.000000 rapidfuzz-3.9.1/extern/taskflow/taskflow/utility/math.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    19899 2024-05-19 20:11:01.000000 rapidfuzz-3.9.1/extern/taskflow/taskflow/utility/object_pool.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4239 2024-05-19 20:11:01.000000 rapidfuzz-3.9.1/extern/taskflow/taskflow/utility/os.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    29321 2024-05-19 20:11:01.000000 rapidfuzz-3.9.1/extern/taskflow/taskflow/utility/serializer.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-19 20:11:01.000000 rapidfuzz-3.9.1/extern/taskflow/taskflow/utility/singleton.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    31329 2024-05-19 20:11:01.000000 rapidfuzz-3.9.1/extern/taskflow/taskflow/utility/small_vector.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-19 20:11:01.000000 rapidfuzz-3.9.1/extern/taskflow/taskflow/utility/stream.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8689 2024-05-19 20:11:01.000000 rapidfuzz-3.9.1/extern/taskflow/taskflow/utility/traits.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5685 2024-05-19 20:11:01.000000 rapidfuzz-3.9.1/extern/taskflow/taskflow/utility/uuid.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-05-19 20:11:23.000000 rapidfuzz-3.9.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 20:11:26.954500 rapidfuzz-3.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:11:26.890500 rapidfuzz-3.9.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:11:26.930500 rapidfuzz-3.9.1/src/rapidfuzz/
+-rw-r--r--   0 runner    (1001) docker     (127)     7594 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:11:26.934500 rapidfuzz-3.9.1/src/rapidfuzz/FeatureDetector/
+-rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/FeatureDetector/CpuInfo.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/FeatureDetector/CpuInfo.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2991 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:11:26.934500 rapidfuzz-3.9.1/src/rapidfuzz/__pyinstaller/
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/__pyinstaller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/__pyinstaller/hook-rapidfuzz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/__pyinstaller/test_rapidfuzz_packaging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/_common_py.py
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/_feature_detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)   266395 2024-05-19 20:11:19.000000 rapidfuzz-3.9.1/src/rapidfuzz/_feature_detector_cpp.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/_feature_detector_cpp.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)     4027 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25736 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/cpp_common.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    17473 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/cpp_common.pxd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:11:26.950500 rapidfuzz-3.9.1/src/rapidfuzz/distance/
+-rw-r--r--   0 runner    (1001) docker     (127)     3481 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/distance/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/distance/DamerauLevenshtein.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/distance/DamerauLevenshtein.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6591 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/distance/DamerauLevenshtein_py.py
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/distance/Hamming.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2742 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/distance/Hamming.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9081 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/distance/Hamming_py.py
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/distance/Indel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2566 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/distance/Indel.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10034 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/distance/Indel_py.py
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/distance/Jaro.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/distance/Jaro.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/distance/JaroWinkler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/distance/JaroWinkler.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6481 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/distance/JaroWinkler_py.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7345 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/distance/Jaro_py.py
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/distance/LCSseq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2566 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/distance/LCSseq.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    11504 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/distance/LCSseq_py.py
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/distance/Levenshtein.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3651 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/distance/Levenshtein.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    17103 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/distance/Levenshtein_py.py
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/distance/OSA.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/distance/OSA.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6251 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/distance/OSA_py.py
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/distance/Postfix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/distance/Postfix.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5039 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/distance/Postfix_py.py
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/distance/Prefix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/distance/Prefix.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5015 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/distance/Prefix_py.py
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/distance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/distance/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/distance/_initialize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3989 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/distance/_initialize.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)  1693935 2024-05-19 20:11:20.000000 rapidfuzz-3.9.1/src/rapidfuzz/distance/_initialize_cpp.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/distance/_initialize_cpp.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)    29674 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/distance/_initialize_cpp.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)    26320 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/distance/_initialize_py.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49089 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/distance/metrics.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)  1506049 2024-05-19 20:11:21.000000 rapidfuzz-3.9.1/src/rapidfuzz/distance/metrics_cpp.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)    62949 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/distance/metrics_cpp.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)  1514092 2024-05-19 20:11:22.000000 rapidfuzz-3.9.1/src/rapidfuzz/distance/metrics_cpp_avx2.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/distance/metrics_cpp_avx2.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)  1514092 2024-05-19 20:11:23.000000 rapidfuzz-3.9.1/src/rapidfuzz/distance/metrics_cpp_sse2.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/distance/metrics_cpp_sse2.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)    10624 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/distance/metrics_py.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/fuzz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4784 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/fuzz.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)   678100 2024-05-19 20:11:15.000000 rapidfuzz-3.9.1/src/rapidfuzz/fuzz_cpp.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)     9678 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/fuzz_cpp.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    11635 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/fuzz_cpp.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)   680081 2024-05-19 20:11:16.000000 rapidfuzz-3.9.1/src/rapidfuzz/fuzz_cpp_avx2.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/fuzz_cpp_avx2.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)   680081 2024-05-19 20:11:16.000000 rapidfuzz-3.9.1/src/rapidfuzz/fuzz_cpp_sse2.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/fuzz_cpp_sse2.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)    25530 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/fuzz_py.py
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/process.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16771 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/process.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    23286 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/process_cpp.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/process_cpp.py
+-rw-r--r--   0 runner    (1001) docker     (127)  2151605 2024-05-19 20:11:18.000000 rapidfuzz-3.9.1/src/rapidfuzz/process_cpp_impl.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)    79018 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/process_cpp_impl.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)    26688 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/process_py.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     7782 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/rapidfuzz.h
+-rw-r--r--   0 runner    (1001) docker     (127)   293266 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/unicodetype_db.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/utils.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/utils.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)   502929 2024-05-19 20:11:19.000000 rapidfuzz-3.9.1/src/rapidfuzz/utils_cpp.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/utils_cpp.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/utils_cpp.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/utils_py.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:11:26.954500 rapidfuzz-3.9.1/src/rapidfuzz.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11677 2024-05-19 20:11:26.000000 rapidfuzz-3.9.1/src/rapidfuzz.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9502 2024-05-19 20:11:26.000000 rapidfuzz-3.9.1/src/rapidfuzz.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 20:11:26.000000 rapidfuzz-3.9.1/src/rapidfuzz.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-19 20:11:26.000000 rapidfuzz-3.9.1/src/rapidfuzz.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-19 20:11:26.000000 rapidfuzz-3.9.1/src/rapidfuzz.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-19 20:11:26.000000 rapidfuzz-3.9.1/src/rapidfuzz.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:11:26.950500 rapidfuzz-3.9.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15407 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/tests/common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:11:26.954500 rapidfuzz-3.9.1/tests/distance/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/tests/distance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4855 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/tests/distance/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/tests/distance/test_DamerauLevenshtein.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3185 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/tests/distance/test_Hamming.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/tests/distance/test_Indel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/tests/distance/test_Jaro.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2717 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/tests/distance/test_JaroWinkler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/tests/distance/test_LCSseq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4665 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/tests/distance/test_Levenshtein.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/tests/distance/test_OSA.py
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/tests/distance/test_Postfix.py
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/tests/distance/test_Prefix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3988 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/tests/distance/test_distance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10165 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/tests/distance/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/tests/test_cpp_fallback.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12939 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/tests/test_fuzz.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14447 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/tests/test_hypothesis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26380 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/tests/test_process.py
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/tests/test_pure_python_fallback.py
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/tests/test_utils.py
```

### Comparing `rapidfuzz-3.9.0/CHANGELOG.rst` & `rapidfuzz-3.9.1/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 Changelog
 ---------
 
+[3.9.1] - 2024-05-19
+^^^^^^^^^^^^^^^^^^^^
+Fixed
+~~~~~
+* disable AVX2 on MacOS since it did lead to illegal instructions being generated
+
+
 [3.9.0] - 2024-05-02
 ^^^^^^^^^^^^^^^^^^^^
 Changed
 ~~~~~~~
 * significantly improve type hints for the library
 
 Fixed
```

### Comparing `rapidfuzz-3.9.0/CMakeLists.txt` & `rapidfuzz-3.9.1/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/LICENSE` & `rapidfuzz-3.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/MANIFEST.in` & `rapidfuzz-3.9.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/PKG-INFO` & `rapidfuzz-3.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rapidfuzz
-Version: 3.9.0
+Version: 3.9.1
 Summary: rapid fuzzy string matching
 Home-page: https://github.com/rapidfuzz/RapidFuzz
 Author: Max Bachmann
 Author-email: pypi@maxbachmann.de
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: rapidfuzz Version: 3.9.0 Summary: rapid fuzzy
+Metadata-Version: 2.1 Name: rapidfuzz Version: 3.9.1 Summary: rapid fuzzy
 string matching Home-page: https://github.com/rapidfuzz/RapidFuzz Author: Max
 Bachmann Author-email: pypi@maxbachmann.de License: MIT Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12 Classifier: License :: OSI
 Approved :: MIT License Requires-Python: >=3.8 Description-Content-Type: text/
```

### Comparing `rapidfuzz-3.9.0/README.md` & `rapidfuzz-3.9.1/README.md`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/_custom_build/backend.py` & `rapidfuzz-3.9.1/_custom_build/backend.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/cmake/CheckCPUArch.cmake` & `rapidfuzz-3.9.1/cmake/CheckCPUArch.cmake`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/docs/Contributing/index.rst` & `rapidfuzz-3.9.1/docs/Contributing/index.rst`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/docs/Installation.rst` & `rapidfuzz-3.9.1/docs/Installation.rst`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/docs/Usage/distance/DamerauLevenshtein.rst` & `rapidfuzz-3.9.1/docs/Usage/distance/DamerauLevenshtein.rst`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/docs/Usage/distance/Indel.rst` & `rapidfuzz-3.9.1/docs/Usage/distance/Indel.rst`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/docs/Usage/distance/Jaro.rst` & `rapidfuzz-3.9.1/docs/Usage/distance/Jaro.rst`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/docs/Usage/distance/JaroWinkler.rst` & `rapidfuzz-3.9.1/docs/Usage/distance/JaroWinkler.rst`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/docs/Usage/distance/LCSseq.rst` & `rapidfuzz-3.9.1/docs/Usage/distance/LCSseq.rst`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/docs/Usage/distance/Levenshtein.rst` & `rapidfuzz-3.9.1/docs/Usage/distance/Levenshtein.rst`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/docs/Usage/distance/OSA.rst` & `rapidfuzz-3.9.1/docs/Usage/distance/OSA.rst`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/docs/Usage/distance/img/damerau_levenshtein.svg` & `rapidfuzz-3.9.1/docs/Usage/distance/img/damerau_levenshtein.svg`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/docs/Usage/distance/img/indel_levenshtein.svg` & `rapidfuzz-3.9.1/docs/Usage/distance/img/indel_levenshtein.svg`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/docs/Usage/distance/img/jaro.svg` & `rapidfuzz-3.9.1/docs/Usage/distance/img/jaro.svg`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/docs/Usage/distance/img/jaro_winkler.svg` & `rapidfuzz-3.9.1/docs/Usage/distance/img/jaro_winkler.svg`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/docs/Usage/distance/img/osa.svg` & `rapidfuzz-3.9.1/docs/Usage/distance/img/osa.svg`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/docs/Usage/distance/img/uniform_levenshtein.svg` & `rapidfuzz-3.9.1/docs/Usage/distance/img/uniform_levenshtein.svg`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/docs/Usage/fuzz.rst` & `rapidfuzz-3.9.1/docs/Usage/fuzz.rst`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/docs/Usage/img/WRatio.svg` & `rapidfuzz-3.9.1/docs/Usage/img/WRatio.svg`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/docs/Usage/img/indel_levenshtein.svg` & `rapidfuzz-3.9.1/docs/Usage/img/indel_levenshtein.svg`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/docs/Usage/img/partial_ratio_long_needle.svg` & `rapidfuzz-3.9.1/docs/Usage/img/partial_ratio_long_needle.svg`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/docs/Usage/img/partial_ratio_short_needle.svg` & `rapidfuzz-3.9.1/docs/Usage/img/partial_ratio_short_needle.svg`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/docs/Usage/img/partial_token_ratio.svg` & `rapidfuzz-3.9.1/docs/Usage/img/partial_token_ratio.svg`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/docs/Usage/img/partial_token_set_ratio.svg` & `rapidfuzz-3.9.1/docs/Usage/img/partial_token_set_ratio.svg`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/docs/Usage/img/partial_token_sort_ratio.svg` & `rapidfuzz-3.9.1/docs/Usage/img/partial_token_sort_ratio.svg`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/docs/Usage/img/ratio.svg` & `rapidfuzz-3.9.1/docs/Usage/img/ratio.svg`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/docs/Usage/img/token_ratio.svg` & `rapidfuzz-3.9.1/docs/Usage/img/token_ratio.svg`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/docs/Usage/img/token_set_ratio.svg` & `rapidfuzz-3.9.1/docs/Usage/img/token_set_ratio.svg`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/docs/Usage/img/token_sort_ratio.svg` & `rapidfuzz-3.9.1/docs/Usage/img/token_sort_ratio.svg`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/docs/Usage/img/uniform_levenshtein.svg` & `rapidfuzz-3.9.1/docs/Usage/img/uniform_levenshtein.svg`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/docs/conf.py` & `rapidfuzz-3.9.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/docs/img/RapidFuzz.svg` & `rapidfuzz-3.9.1/docs/img/RapidFuzz.svg`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/docs/img/cdist.svg` & `rapidfuzz-3.9.1/docs/img/cdist.svg`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/docs/img/scorer.svg` & `rapidfuzz-3.9.1/docs/img/scorer.svg`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/docs/index.rst` & `rapidfuzz-3.9.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/docs/refs.bib` & `rapidfuzz-3.9.1/docs/refs.bib`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/extern/rapidfuzz-cpp/CMakeLists.txt` & `rapidfuzz-3.9.1/extern/rapidfuzz-cpp/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/extern/rapidfuzz-cpp/LICENSE` & `rapidfuzz-3.9.1/extern/rapidfuzz-cpp/LICENSE`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/extern/rapidfuzz-cpp/rapidfuzz/details/CharSet.hpp` & `rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/details/CharSet.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/extern/rapidfuzz-cpp/rapidfuzz/details/GrowingHashmap.hpp` & `rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/details/GrowingHashmap.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/extern/rapidfuzz-cpp/rapidfuzz/details/Matrix.hpp` & `rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/details/Matrix.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/extern/rapidfuzz-cpp/rapidfuzz/details/PatternMatchVector.hpp` & `rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/details/PatternMatchVector.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/extern/rapidfuzz-cpp/rapidfuzz/details/Range.hpp` & `rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/details/Range.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/extern/rapidfuzz-cpp/rapidfuzz/details/SplittedSentenceView.hpp` & `rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/details/SplittedSentenceView.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/extern/rapidfuzz-cpp/rapidfuzz/details/common.hpp` & `rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/details/common.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/extern/rapidfuzz-cpp/rapidfuzz/details/common_impl.hpp` & `rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/details/common_impl.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/extern/rapidfuzz-cpp/rapidfuzz/details/distance.hpp` & `rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/details/distance.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/extern/rapidfuzz-cpp/rapidfuzz/details/intrinsics.hpp` & `rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/details/intrinsics.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/extern/rapidfuzz-cpp/rapidfuzz/details/simd.hpp` & `rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/details/simd.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/extern/rapidfuzz-cpp/rapidfuzz/details/simd_avx2.hpp` & `rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/details/simd_avx2.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/extern/rapidfuzz-cpp/rapidfuzz/details/simd_sse2.hpp` & `rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/details/simd_sse2.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/extern/rapidfuzz-cpp/rapidfuzz/details/type_traits.hpp` & `rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/details/type_traits.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/extern/rapidfuzz-cpp/rapidfuzz/details/types.hpp` & `rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/details/types.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/extern/rapidfuzz-cpp/rapidfuzz/distance/DamerauLevenshtein.hpp` & `rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/distance/DamerauLevenshtein.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/extern/rapidfuzz-cpp/rapidfuzz/distance/DamerauLevenshtein_impl.hpp` & `rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/distance/DamerauLevenshtein_impl.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/extern/rapidfuzz-cpp/rapidfuzz/distance/Hamming.hpp` & `rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/distance/Hamming.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/extern/rapidfuzz-cpp/rapidfuzz/distance/Hamming_impl.hpp` & `rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/distance/Hamming_impl.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/extern/rapidfuzz-cpp/rapidfuzz/distance/Indel.hpp` & `rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/distance/Indel.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/extern/rapidfuzz-cpp/rapidfuzz/distance/Indel_impl.hpp` & `rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/distance/Indel_impl.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/extern/rapidfuzz-cpp/rapidfuzz/distance/Jaro.hpp` & `rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/distance/Jaro.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/extern/rapidfuzz-cpp/rapidfuzz/distance/JaroWinkler.hpp` & `rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/distance/JaroWinkler.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/extern/rapidfuzz-cpp/rapidfuzz/distance/JaroWinkler_impl.hpp` & `rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/distance/JaroWinkler_impl.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/extern/rapidfuzz-cpp/rapidfuzz/distance/Jaro_impl.hpp` & `rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/distance/Jaro_impl.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/extern/rapidfuzz-cpp/rapidfuzz/distance/LCSseq.hpp` & `rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/distance/LCSseq.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/extern/rapidfuzz-cpp/rapidfuzz/distance/LCSseq_impl.hpp` & `rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/distance/LCSseq_impl.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/extern/rapidfuzz-cpp/rapidfuzz/distance/Levenshtein.hpp` & `rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/distance/Levenshtein.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/extern/rapidfuzz-cpp/rapidfuzz/distance/Levenshtein_impl.hpp` & `rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/distance/Levenshtein_impl.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/extern/rapidfuzz-cpp/rapidfuzz/distance/OSA.hpp` & `rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/distance/OSA.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/extern/rapidfuzz-cpp/rapidfuzz/distance/OSA_impl.hpp` & `rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/distance/OSA_impl.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/extern/rapidfuzz-cpp/rapidfuzz/distance/Postfix.hpp` & `rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/distance/Postfix.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/extern/rapidfuzz-cpp/rapidfuzz/distance/Postfix_impl.hpp` & `rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/distance/Postfix_impl.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/extern/rapidfuzz-cpp/rapidfuzz/distance/Prefix.hpp` & `rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/distance/Prefix.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/extern/rapidfuzz-cpp/rapidfuzz/distance/Prefix_impl.hpp` & `rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/distance/Prefix_impl.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/extern/rapidfuzz-cpp/rapidfuzz/distance.hpp` & `rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/distance.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/extern/rapidfuzz-cpp/rapidfuzz/fuzz.hpp` & `rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/fuzz.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/extern/rapidfuzz-cpp/rapidfuzz/fuzz_impl.hpp` & `rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/fuzz_impl.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/extern/taskflow/CMakeLists.txt` & `rapidfuzz-3.9.1/extern/taskflow/CMakeLists.txt`

 * *Files 2% similar despite different names*

```diff
@@ -2,23 +2,30 @@
 # Taskflow CMake 
 #
 # To enable thread sanitizer: 
 # -DCMAKE_CXX_FLAGS="-fsanitize=thread -g"
 #
 # To enable address and leak sanitizers
 # -DCMAKE_CXX_FLAGS="-fsanitize=address  -fsanitize=leak -g"
+#
+# To enable different c++ standards
+# -DCMAKE_CXX_STANDARD=17
+# -DCMAKE_CXX_STANDARD=20
+# -DCMAKE_CXX_STANDARD=23
 # -------------------------------------------------------------------
 
 
 # CMake version
 cmake_minimum_required (VERSION 3.18)
 MESSAGE(STATUS "CMAKE_ROOT: " ${CMAKE_ROOT})
 
 # Project name
-project(Taskflow VERSION 3.6.0 LANGUAGES CXX)
+project(Taskflow VERSION 3.7.0 LANGUAGES CXX)
+
+set(CMAKE_CXX_STANDARD 17)
 
 # build options
 option(TF_BUILD_BENCHMARKS "Enables builds of benchmarks" OFF)
 option(TF_BUILD_CUDA "Enables builds of cuda code" OFF)
 option(TF_BUILD_SYCL "Enables builds of sycl code" OFF)
 option(TF_BUILD_TESTS "Enables builds of tests" ON)
 option(TF_BUILD_EXAMPLES "Enables builds of examples" ON)
@@ -39,28 +46,28 @@
 
 # Adhere to GNU conventions
 include(GNUInstallDirs)
 
 # Compiler vendors
 ## g++
 if (CMAKE_CXX_COMPILER_ID STREQUAL "GNU")
-  if(CMAKE_CXX_COMPILER_VERSION VERSION_LESS "7.0")
+  if(CMAKE_CXX_COMPILER_VERSION VERSION_LESS "8.4")
     message(STATUS "CMAKE_CXX_COMPILER_VERSION: ${CMAKE_CXX_COMPILER_VERSION}")
-    message(FATAL_ERROR "\nTaskflow requires g++ at least v7.0")
+    message(FATAL_ERROR "\nTaskflow requires g++ at least v8.4")
   endif()
 ## clang++
 elseif (CMAKE_CXX_COMPILER_ID STREQUAL "Clang")
   if(CMAKE_CXX_COMPILER_VERSION VERSION_LESS "6.0")
     message(STATUS "CMAKE_CXX_COMPILER_VERSION: ${CMAKE_CXX_COMPILER_VERSION}")
     message(FATAL_ERROR "\nTaskflow requires clang++ at least v6.0")
   endif() 
 ## AppleClang
 elseif (CMAKE_CXX_COMPILER_ID STREQUAL "AppleClang")
-  if(CMAKE_CXX_COMPILER_VERSION VERSION_LESS "8.0")
-    message(FATAL_ERROR "\nTaskflow requires AppleClang at least v8.0")
+  if(CMAKE_CXX_COMPILER_VERSION VERSION_LESS "12.0")
+    message(FATAL_ERROR "\nTaskflow requires AppleClang at least v12.0")
   endif()
 ## microsoft visual c++
 elseif (CMAKE_CXX_COMPILER_ID STREQUAL "MSVC")
   add_definitions(/bigobj)
   if(NOT MSVC_VERSION GREATER_EQUAL 1914)
     message(STATUS "CMAKE_CXX_COMPILER_VERSION: ${CMAKE_CXX_COMPILER_VERSION}")
     message(FATAL_ERROR "\nTaskflow requires MSVC++ at least v14.14") 
@@ -128,15 +135,15 @@
 #  find_package(ComputeCpp REQUIRED)
 #  message(STATUS "ComputeCpp_DIR: " ${ComputeCpp_DIR})
 #  message(STATUS "ComputeCpp_INCLUDE_DIRS: " ${ComputeCpp_INCLUDE_DIRS})
 #  include_directories(${ComputeCpp_INCLUDE_DIRS})
 #endif()
 
 # -----------------------------------------------------------------------------
-# defult release build
+# default to release build, unless explicitly specified
 # -----------------------------------------------------------------------------
 if(NOT CMAKE_BUILD_TYPE AND NOT CMAKE_CONFIGURATION_TYPES)
   message(STATUS "Setting build type to '${TF_DEFAULT_BUILD_TYPE}'")
   set(
     CMAKE_BUILD_TYPE "${TF_DEFAULT_BUILD_TYPE}" 
     CACHE
     STRING "Choose the type of build." 
@@ -159,28 +166,28 @@
 # error setting
 add_library(error_settings INTERFACE)
 add_library(tf::error_settings ALIAS error_settings)
 
 target_compile_options(
   error_settings
   INTERFACE
-  $<$<CXX_COMPILER_ID:AppleClang>:-Wall -Wextra -Wfatal-errors>
-  $<$<AND:$<COMPILE_LANGUAGE:CXX>,$<CXX_COMPILER_ID:Clang>>:-Wall -Wextra -Wfatal-errors>
-  $<$<AND:$<COMPILE_LANGUAGE:CXX>,$<CXX_COMPILER_ID:GNU>>:-Wall -Wextra -Wfatal-errors>
+  $<$<CXX_COMPILER_ID:AppleClang>:-Wall -Wextra -Wfatal-errors -Wshadow>
+  $<$<AND:$<COMPILE_LANGUAGE:CXX>,$<CXX_COMPILER_ID:Clang>>:-Wall -Wextra -Wfatal-errors -Wshadow>
+  $<$<AND:$<COMPILE_LANGUAGE:CXX>,$<CXX_COMPILER_ID:GNU>>:-Wall -Wextra -Wfatal-errors -Wshadow>
   $<$<AND:$<COMPILE_LANGUAGE:CXX>,$<CXX_COMPILER_ID:MSVC>>:/W3 /permissive->
 )
 
 # cuda compiler options
 if(TF_BUILD_CUDA)
   message(STATUS "Configuring CUDA compiler options ...")
   target_compile_options(
     error_settings
     BEFORE
     INTERFACE
-    $<$<COMPILE_LANGUAGE:CUDA>:--extended-lambda -Xcompiler=-Wall,-Wextra,-Wfatal-errors>
+    $<$<COMPILE_LANGUAGE:CUDA>:--extended-lambda -Xcompiler=-Wall,-Wextra,-Wfatal-errors,-Wshadow>
   )
 endif(TF_BUILD_CUDA)
 
 # sycl compiler options (currently support only DPC++)
 if(TF_BUILD_SYCL)
   message(STATUS "Configuring SYCL compiler options ...")
   message(STATUS "You may specify -DTF_BUILD_SYCL_BITCODE=ptx64 for CUDA devices")
@@ -243,14 +250,15 @@
 message(STATUS "PROJECT_NAME: " ${PROJECT_NAME})
 message(STATUS "CMAKE_HOST_SYSTEM: ${CMAKE_HOST_SYSTEM}")
 message(STATUS "CMAKE_BUILD_TYPE: " ${CMAKE_BUILD_TYPE})
 message(STATUS "CMAKE_CXX_COMPILER: " ${CMAKE_CXX_COMPILER})
 message(STATUS "CMAKE_CXX_COMPILER_ID: " ${CMAKE_CXX_COMPILER_ID})
 message(STATUS "CMAKE_CXX_COMPILER_VERSION: " ${CMAKE_CXX_COMPILER_VERSION})
 message(STATUS "CMAKE_CXX_FLAGS: " ${CMAKE_CXX_FLAGS})
+message(STATUS "CMAKE_CXX_STANDARD: " ${CMAKE_CXX_STANDARD})
 message(STATUS "CMAKE_CUDA_COMPILER: " ${CMAKE_CUDA_COMPILER})
 message(STATUS "CMAKE_CUDA_COMPILER_ID: " ${CMAKE_CUDA_COMPILER_ID})
 message(STATUS "CMAKE_CUDA_COMPILER_VERSION: " ${CMAKE_CUDA_COMPILER_VERSION})
 message(STATUS "CMAKE_CUDA_FLAGS: " ${CMAKE_CUDA_FLAGS})
 message(STATUS "CMAKE_MODULE_PATH: " ${CMAKE_MODULE_PATH})
 message(STATUS "CMAKE_CURRENT_SOURCE_DIR: " ${CMAKE_CURRENT_SOURCE_DIR})
 message(STATUS "CMAKE_CURRENT_BINARY_DIR: " ${CMAKE_CURRENT_BINARY_DIR})
@@ -360,15 +368,15 @@
   ${CMAKE_CURRENT_BINARY_DIR}/${PROJECT_NAME}Config.cmake
   INSTALL_DESTINATION ${CMAKE_INSTALL_LIBDIR}/cmake/${PROJECT_NAME}
   PATH_VARS CMAKE_INSTALL_FULL_INCLUDEDIR
 )
 
 write_basic_package_version_file(
   ${PROJECT_NAME}ConfigVersion.cmake 
-  COMPATIBILITY SameMajorVersion
+  COMPATIBILITY SameMinorVersion
 )
 
 install(
   FILES ${CMAKE_CURRENT_BINARY_DIR}/${PROJECT_NAME}Config.cmake
         ${CMAKE_CURRENT_BINARY_DIR}/${PROJECT_NAME}ConfigVersion.cmake
   DESTINATION ${CMAKE_INSTALL_LIBDIR}/cmake/${PROJECT_NAME}
 )
```

### Comparing `rapidfuzz-3.9.0/extern/taskflow/LICENSE` & `rapidfuzz-3.9.1/extern/taskflow/LICENSE`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 TASKFLOW MIT LICENSE 
 
-Copyright (c) 2018-2022 Dr. Tsung-Wei Huang
+Copyright (c) 2018-2024 Dr. Tsung-Wei Huang
+
+The University of Wisconsin at Madison
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `rapidfuzz-3.9.0/extern/taskflow/taskflow/algorithm/critical.hpp` & `rapidfuzz-3.9.1/extern/taskflow/taskflow/algorithm/critical.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 // ----------------------------------------------------------------------------
 
 /**
 @class CriticalSection
 
 @brief class to create a critical region of limited workers to run tasks
 
-tf::CriticalSection is a warpper over tf::Semaphore and is specialized for
+tf::CriticalSection is a wrapper over tf::Semaphore and is specialized for
 limiting the maximum concurrency over a set of tasks.
 A critical section starts with an initial count representing that limit.
 When a task is added to the critical section,
 the task acquires and releases the semaphore internal to the critical section.
 This design avoids explicit call of tf::Task::acquire and tf::Task::release.
 The following example creates a critical section of one worker and adds
 the five tasks to the critical section.
```

### Comparing `rapidfuzz-3.9.0/extern/taskflow/taskflow/algorithm/data_pipeline.hpp` & `rapidfuzz-3.9.1/extern/taskflow/taskflow/algorithm/data_pipeline.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/extern/taskflow/taskflow/algorithm/find.hpp` & `rapidfuzz-3.9.1/extern/taskflow/taskflow/algorithm/find.hpp`

 * *Files 7% similar despite different names*

```diff
@@ -4,21 +4,21 @@
 
 namespace tf {
 
 namespace detail {
 
 // Function: find_if_loop
 template <typename Iterator, typename Predicate>
-TF_FORCE_INLINE bool find_if_loop(
+bool find_if_loop(
   std::atomic<size_t>& offset, 
   Iterator& beg,
   size_t& prev_e,
   size_t  curr_b, 
   size_t  curr_e,
-  Predicate&& predicate
+  Predicate predicate
 ) {
   // early prune
   if(offset.load(std::memory_order_relaxed) < curr_b) {
     return true;
   }
   std::advance(beg, curr_b - prev_e);
   for(size_t x = curr_b; x<curr_e; x++) {
@@ -29,21 +29,21 @@
   }
   prev_e = curr_e;
   return false;
 }
 
 // Function: find_if_not_loop
 template <typename Iterator, typename Predicate>
-TF_FORCE_INLINE bool find_if_not_loop(
+bool find_if_not_loop(
   std::atomic<size_t>& offset, 
   Iterator& beg,
   size_t& prev_e,
   size_t  curr_b, 
   size_t  curr_e,
-  Predicate&& predicate
+  Predicate predicate
 ) {
 
   // early prune
   if(offset.load(std::memory_order_relaxed) < curr_b) {
     return true;
   }
   std::advance(beg, curr_b - prev_e);
@@ -53,222 +53,213 @@
       return true;
     }
   }
   prev_e = curr_e;
   return false;
 }
 
+}  // namespace detail --------------------------------------------------------
+
 // Function: make_find_if_task
-template <typename B, typename E, typename T, typename UOP, typename P>
-TF_FORCE_INLINE auto make_find_if_task(
-  B first, E last, T& result, UOP predicate, P&& part
-) {
+template <typename B, typename E, typename T, typename UOP, typename P = DefaultPartitioner>
+auto make_find_if_task(B first, E last, T& result, UOP predicate, P part = P()) {
   
   using B_t = std::decay_t<unwrap_ref_decay_t<B>>;
   using E_t = std::decay_t<unwrap_ref_decay_t<E>>;
-  using namespace std::string_literals;
 
-  return 
-  [b=first, e=last, predicate, &result, part=std::forward<P>(part)] 
-  (Runtime& rt) mutable {
+  return [=, &result] (Runtime& rt) mutable {
 
     // fetch the stateful values
-    B_t beg = b;
-    E_t end = e;
+    B_t beg = first;
+    E_t end = last;
 
     size_t W = rt.executor().num_workers();
     size_t N = std::distance(beg, end);
 
     // only myself - no need to spawn another graph
     if(W <= 1 || N <= part.chunk_size()) {
-      result = std::find_if(beg, end, predicate);
+      launch_loop(part, [&](){
+        result = std::find_if(beg, end, predicate);
+      });
       return;
     }
 
     if(N < W) {
       W = N;
     }
     
     std::atomic<size_t> offset(N);
     
     // static partitioner
-    if constexpr(std::is_same_v<std::decay_t<P>, StaticPartitioner>) {
+    if constexpr(part.type() == PartitionerType::STATIC) {
 
       size_t chunk_size;
 
       for(size_t w=0, curr_b=0; w<W && curr_b < N; ++w, curr_b += chunk_size) {
       
         chunk_size = part.adjusted_chunk_size(N, W, w);
 
-        launch_loop(W, w, rt,
-          [N, W, curr_b, chunk_size, beg, &predicate, &offset, &part] 
-          () mutable {
+        launch_loop(W, w, rt, part,
+          [N, W, curr_b, chunk_size, beg, &predicate, &offset, &part] () mutable {
             part.loop_until(N, W, curr_b, chunk_size,
-              [&, prev_e=size_t{0}](size_t curr_b, size_t curr_e) mutable {
+              [&, prev_e=size_t{0}](size_t part_b, size_t part_e) mutable {
                 return detail::find_if_loop(
-                  offset, beg, prev_e, curr_b, curr_e, predicate
+                  offset, beg, prev_e, part_b, part_e, predicate
                 );
               }
-            ); 
+            );
           }
         );
       }
 
-      rt.join();
+      rt.corun_all();
     }
     // dynamic partitioner
     else {
       std::atomic<size_t> next(0);
       launch_loop(N, W, rt, next, part, 
         [N, W, beg, &predicate, &offset, &next, &part] () mutable {
           part.loop_until(N, W, next, 
             [&, prev_e=size_t{0}](size_t curr_b, size_t curr_e) mutable {
               return detail::find_if_loop(
                 offset, beg, prev_e, curr_b, curr_e, predicate
               );
             }
-          ); 
+          );
         }
       );
     }
 
     // update the result iterator by the offset
     result = std::next(beg, offset.load(std::memory_order_relaxed));
   };
 }
 
 // Function: make_find_if_not_task
-template <typename B, typename E, typename T, typename UOP, typename P>
-TF_FORCE_INLINE auto make_find_if_not_task(
-  B first, E last, T& result, UOP predicate, P&& part
-) {
+template <typename B, typename E, typename T, typename UOP, typename P = DefaultPartitioner>
+auto make_find_if_not_task(B first, E last, T& result, UOP predicate, P part = P()) {
   
   using B_t = std::decay_t<unwrap_ref_decay_t<B>>;
   using E_t = std::decay_t<unwrap_ref_decay_t<E>>;
-  using namespace std::string_literals;
 
-  return
-  [b=first, e=last, predicate, &result, part=std::forward<P>(part)] 
-  (Runtime& rt) mutable {
+  return [=, &result] (Runtime& rt) mutable {
 
     // fetch the stateful values
-    B_t beg = b;
-    E_t end = e;
+    B_t beg = first;
+    E_t end = last;
 
     size_t W = rt.executor().num_workers();
     size_t N = std::distance(beg, end);
 
     // only myself - no need to spawn another graph
     if(W <= 1 || N <= part.chunk_size()) {
-      result = std::find_if_not(beg, end, predicate);
+      launch_loop(part, [&](){
+        result = std::find_if_not(beg, end, predicate);
+      });
       return;
     }
 
     if(N < W) {
       W = N;
     }
     
     std::atomic<size_t> offset(N);
     
     // static partitioner
-    if constexpr(std::is_same_v<std::decay_t<P>, StaticPartitioner>) {
+    if constexpr(part.type() == PartitionerType::STATIC) {
 
       size_t chunk_size;
 
       for(size_t w=0, curr_b=0; w<W && curr_b < N; ++w, curr_b += chunk_size) {
       
         chunk_size = part.adjusted_chunk_size(N, W, w);
 
-        launch_loop(W, w, rt,
+        launch_loop(W, w, rt, part,
           [N, W, curr_b, chunk_size, beg, &predicate, &offset, &part] () mutable {
             part.loop_until(N, W, curr_b, chunk_size,
-              [&, prev_e=size_t{0}](size_t curr_b, size_t curr_e) mutable {
+              [&, prev_e=size_t{0}](size_t part_b, size_t part_e) mutable {
                 return detail::find_if_not_loop(
-                  offset, beg, prev_e, curr_b, curr_e, predicate
+                  offset, beg, prev_e, part_b, part_e, predicate
                 );
               }
-            ); 
+            );
           }
         );
       }
 
-      rt.join();
+      rt.corun_all();
     }
     // dynamic partitioner
     else {
       std::atomic<size_t> next(0);
       launch_loop(N, W, rt, next, part,
         [N, W, beg, &predicate, &offset, &next, &part] () mutable {
           part.loop_until(N, W, next, 
             [&, prev_e=size_t{0}](size_t curr_b, size_t curr_e) mutable {
               return detail::find_if_not_loop(
                 offset, beg, prev_e, curr_b, curr_e, predicate
               );
             }
-          ); 
+          );
         }
       );
     }
 
     // update the result iterator by the offset
     result = std::next(beg, offset.load(std::memory_order_relaxed));
   };
 }
 
 // Function: make_min_element_task
-template <typename B, typename E, typename T, typename C, typename P>
-TF_FORCE_INLINE auto make_min_element_task(
-  B first, E last, T& result, C comp, P&& part
-) {
+template <typename B, typename E, typename T, typename C, typename P = DefaultPartitioner>
+auto make_min_element_task(B first, E last, T& result, C comp, P part = P()) {
 
   using B_t = std::decay_t<unwrap_ref_decay_t<B>>;
   using E_t = std::decay_t<unwrap_ref_decay_t<E>>;
-  using namespace std::string_literals;
 
-  return 
-  [b=first, e=last, &result, comp, part=std::forward<P>(part)] 
-  (Runtime& rt) mutable {
+  return [=, &result] (Runtime& rt) mutable {
 
     // fetch the iterator values
-    B_t beg = b;
-    E_t end = e;
+    B_t beg = first;
+    E_t end = last;
 
     size_t W = rt.executor().num_workers();
     size_t N = std::distance(beg, end);
 
     // only myself - no need to spawn another graph
     if(W <= 1 || N <= part.chunk_size()) {
-      result = std::min_element(beg, end, comp);
+      launch_loop(part, [&](){
+        result = std::min_element(beg, end, comp);
+      });
       return;
     }
 
     if(N < W) {
       W = N;
     }
 
     std::mutex mutex;
     
     // initialize the result to the first element
     result = beg++;
     N--;
 
     // static partitioner
-    if constexpr(std::is_same_v<std::decay_t<P>, StaticPartitioner>) {
+    if constexpr(part.type() == PartitionerType::STATIC) {
       
       size_t chunk_size;
 
       for(size_t w=0, curr_b=0; w<W && curr_b < N; ++w, curr_b += chunk_size) {
         
         // we force chunk size to be at least two because the temporary
         // variable sum needs to avoid copy at the first step
         chunk_size = std::max(size_t{2}, part.adjusted_chunk_size(N, W, w));
         
-        launch_loop(W, w, rt,
+        launch_loop(W, w, rt, part,
         [beg, curr_b, N, W, chunk_size, &comp, &mutex, &result, &part] () mutable {
-
           std::advance(beg, curr_b);
 
           if(N - curr_b == 1) {
             std::lock_guard<std::mutex> lock(mutex);
             if(comp(*beg, *result)) {
               result = beg;
             }
@@ -277,40 +268,40 @@
 
           auto beg1 = beg++;
           auto beg2 = beg++;
           T smallest = comp(*beg1, *beg2) ? beg1 : beg2;
         
           // loop reduce
           part.loop(N, W, curr_b, chunk_size,
-            [&, prev_e=curr_b+2](size_t curr_b, size_t curr_e) mutable {
+            [&, prev_e=curr_b+2](size_t part_b, size_t part_e) mutable {
 
-              if(curr_b > prev_e) {
-                std::advance(beg, curr_b - prev_e);
+              if(part_b > prev_e) {
+                std::advance(beg, part_b - prev_e);
               }
               else {
-                curr_b = prev_e;
+                part_b = prev_e;
               }
 
-              for(size_t x=curr_b; x<curr_e; x++, beg++) {
+              for(size_t x=part_b; x<part_e; x++, beg++) {
                 if(comp(*beg, *smallest)) {
                   smallest = beg;
                 }
               }
-              prev_e = curr_e;
+              prev_e = part_e;
             }
           ); 
           
           // final reduce
           std::lock_guard<std::mutex> lock(mutex);
           if(comp(*smallest, *result)) {
             result = smallest;
           }
         });
       }
-      rt.join();
+      rt.corun_all();
     }
     // dynamic partitioner
     else {
       std::atomic<size_t> next(0);
       launch_loop(N, W, rt, next, part, 
         [beg, N, W, &next, &comp, &mutex, &result, &part] () mutable {
           // pre-reduce
@@ -333,22 +324,22 @@
           auto beg1 = beg++;
           auto beg2 = beg++;
 
           T smallest = comp(*beg1, *beg2) ? beg1 : beg2;
           
           // loop reduce
           part.loop(N, W, next, 
-            [&, prev_e=s0+2](size_t curr_b, size_t curr_e) mutable {
-              std::advance(beg, curr_b - prev_e);
-              for(size_t x=curr_b; x<curr_e; x++, beg++) {
+            [&, prev_e=s0+2](size_t part_b, size_t part_e) mutable {
+              std::advance(beg, part_b - prev_e);
+              for(size_t x=part_b; x<part_e; x++, beg++) {
                 if(comp(*beg, *smallest)) {
                   smallest = beg;
                 }
               }
-              prev_e = curr_e;
+              prev_e = part_e;
             }
           ); 
           
           // final reduce
           std::lock_guard<std::mutex> lock(mutex);
           if(comp(*smallest, *result)) {
             result = smallest;
@@ -356,62 +347,60 @@
         }
       );
     }
   };
 }
 
 // Function: make_max_element_task
-template <typename B, typename E, typename T, typename C, typename P>
-TF_FORCE_INLINE auto make_max_element_task(B first, E last, T& result, C comp, P&& part) {
+template <typename B, typename E, typename T, typename C, typename P = DefaultPartitioner>
+auto make_max_element_task(B first, E last, T& result, C comp, P part = P()) {
 
   using B_t = std::decay_t<unwrap_ref_decay_t<B>>;
   using E_t = std::decay_t<unwrap_ref_decay_t<E>>;
-  using namespace std::string_literals;
 
-  return 
-  [b=first, e=last, &result, comp, part=std::forward<P>(part)] 
-  (Runtime& rt) mutable {
+  return [=, &result] (Runtime& rt) mutable {
 
     // fetch the iterator values
-    B_t beg = b;
-    E_t end = e;
+    B_t beg = first;
+    E_t end = last;
 
     size_t W = rt.executor().num_workers();
     size_t N = std::distance(beg, end);
 
     // only myself - no need to spawn another graph
     if(W <= 1 || N <= part.chunk_size()) {
-      result = std::max_element(beg, end, comp);
+      launch_loop(part, [&](){
+        result = std::max_element(beg, end, comp);
+      });
       return;
     }
 
     if(N < W) {
       W = N;
     }
 
     std::mutex mutex;
     
     // initialize the result to the first element
     result = beg++;
     N--;
 
     // static partitioner
-    if constexpr(std::is_same_v<std::decay_t<P>, StaticPartitioner>) {
+    if constexpr(part.type() == PartitionerType::STATIC) {
       
       size_t chunk_size;
 
       for(size_t w=0, curr_b=0; w<W && curr_b < N; ++w, curr_b += chunk_size) {
         
         // we force chunk size to be at least two because the temporary
         // variable sum needs to avoid copy at the first step
         chunk_size = std::max(size_t{2}, part.adjusted_chunk_size(N, W, w));
         
-        launch_loop(W, w, rt,
+        launch_loop(W, w, rt, part,
         [beg, curr_b, N, W, chunk_size, &comp, &mutex, &result, &part] () mutable {
-
           std::advance(beg, curr_b);
 
           if(N - curr_b == 1) {
             std::lock_guard<std::mutex> lock(mutex);
             if(comp(*result, *beg)) {
               result = beg;
             }
@@ -420,40 +409,40 @@
 
           auto beg1 = beg++;
           auto beg2 = beg++;
           T largest = comp(*beg1, *beg2) ? beg2 : beg1;
         
           // loop reduce
           part.loop(N, W, curr_b, chunk_size,
-            [&, prev_e=curr_b+2](size_t curr_b, size_t curr_e) mutable {
+            [&, prev_e=curr_b+2](size_t part_b, size_t part_e) mutable {
 
-              if(curr_b > prev_e) {
-                std::advance(beg, curr_b - prev_e);
+              if(part_b > prev_e) {
+                std::advance(beg, part_b - prev_e);
               }
               else {
-                curr_b = prev_e;
+                part_b = prev_e;
               }
 
-              for(size_t x=curr_b; x<curr_e; x++, beg++) {
+              for(size_t x=part_b; x<part_e; x++, beg++) {
                 if(comp(*largest, *beg)) {
                   largest = beg;
                 }
               }
-              prev_e = curr_e;
+              prev_e = part_e;
             }
           ); 
           
           // final reduce
           std::lock_guard<std::mutex> lock(mutex);
           if(comp(*result, *largest)) {
             result = largest;
           }
         });
       }
-      rt.join();
+      rt.corun_all();
     }
     // dynamic partitioner
     else {
       std::atomic<size_t> next(0);
       launch_loop(N, W, rt, next, part,
         [beg, N, W, &next, &comp, &mutex, &result, &part] () mutable {
           // pre-reduce
@@ -476,72 +465,64 @@
           auto beg1 = beg++;
           auto beg2 = beg++;
 
           T largest = comp(*beg1, *beg2) ? beg2 : beg1;
           
           // loop reduce
           part.loop(N, W, next, 
-            [&, prev_e=s0+2](size_t curr_b, size_t curr_e) mutable {
-              std::advance(beg, curr_b - prev_e);
-              for(size_t x=curr_b; x<curr_e; x++, beg++) {
+            [&, prev_e=s0+2](size_t part_b, size_t part_e) mutable {
+              std::advance(beg, part_b - prev_e);
+              for(size_t x=part_b; x<part_e; x++, beg++) {
                 if(comp(*largest, *beg)) {
                   largest = beg;
                 }
               }
-              prev_e = curr_e;
+              prev_e = part_e;
             }
           ); 
           
           // final reduce
           std::lock_guard<std::mutex> lock(mutex);
           if(comp(*result, *largest)) {
             result = largest;
           }
         }
       );
     }
   };
 }
 
-}  // namespace detail --------------------------------------------------------
+
 
 // Function: find_if
 template <typename B, typename E, typename T, typename UOP, typename P>
-Task tf::FlowBuilder::find_if(B first, E last, T& result, UOP predicate, P&& part) {
-  return emplace(detail::make_find_if_task(
-    first, last, result, predicate, std::forward<P>(part)
-  ));
+Task tf::FlowBuilder::find_if(B first, E last, T& result, UOP predicate, P part) {
+  return emplace(make_find_if_task(first, last, result, predicate, part));
 }
 
 // Function: find_if_not
 template <typename B, typename E, typename T, typename UOP, typename P>
-Task tf::FlowBuilder::find_if_not(B first, E last, T& result, UOP predicate, P&& part) {
-  return emplace(detail::make_find_if_not_task(
-    first, last, result, predicate, std::forward<P>(part)
-  ));
+Task tf::FlowBuilder::find_if_not(B first, E last, T& result, UOP predicate, P part) {
+  return emplace(make_find_if_not_task(first, last, result, predicate, part));
 }
 
 // ----------------------------------------------------------------------------
 // min_element
 // ----------------------------------------------------------------------------
 
 // Function: min_element
 template <typename B, typename E, typename T, typename C, typename P>
-Task FlowBuilder::min_element(B first, E last, T& result, C comp, P&& part) {
-  return emplace(detail::make_min_element_task(
-    first, last, result, comp, std::forward<P>(part)
-  ));
+Task FlowBuilder::min_element(B first, E last, T& result, C comp, P part) {
+  return emplace(make_min_element_task(first, last, result, comp, part));
 }
 
 // ----------------------------------------------------------------------------
 // max_element
 // ----------------------------------------------------------------------------
 
 // Function: max_element
 template <typename B, typename E, typename T, typename C, typename P>
-Task FlowBuilder::max_element(B first, E last, T& result, C comp, P&& part) {
-  return emplace(detail::make_max_element_task(
-    first, last, result, comp, std::forward<P>(part)
-  ));
+Task FlowBuilder::max_element(B first, E last, T& result, C comp, P part) {
+  return emplace(make_max_element_task(first, last, result, comp, part));
 }
 
 }  // end of namespace tf -----------------------------------------------------
```

### Comparing `rapidfuzz-3.9.0/extern/taskflow/taskflow/algorithm/for_each.hpp` & `rapidfuzz-3.9.1/extern/taskflow/taskflow/algorithm/for_each.hpp`

 * *Files 22% similar despite different names*

```diff
@@ -1,173 +1,172 @@
 #pragma once
 
 #include "launch.hpp"
 
 namespace tf {
 
-namespace detail {
-
 // Function: make_for_each_task
-template <typename B, typename E, typename C, typename P>
-TF_FORCE_INLINE auto make_for_each_task(B beg, E end, C c, P&& part) {
-  
+template <typename B, typename E, typename C, typename P = DefaultPartitioner>
+auto make_for_each_task(B b, E e, C c, P part = P()) {
+
   using B_t = std::decay_t<unwrap_ref_decay_t<B>>;
   using E_t = std::decay_t<unwrap_ref_decay_t<E>>;
-  using namespace std::string_literals;
 
-  return [b=beg, e=end, c, part=std::forward<P>(part)] (Runtime& rt) mutable {
+  return [=] (Runtime& rt) mutable {
 
     // fetch the stateful values
     B_t beg = b;
     E_t end = e;
 
     size_t W = rt.executor().num_workers();
     size_t N = std::distance(beg, end);
 
     // only myself - no need to spawn another graph
     if(W <= 1 || N <= part.chunk_size()) {
-      std::for_each(beg, end, c);
+      launch_loop(part, [&](){
+        std::for_each(beg, end, c);
+      });
       return;
     }
 
     if(N < W) {
       W = N;
     }
     
     // static partitioner
-    if constexpr(std::is_same_v<std::decay_t<P>, StaticPartitioner>) {
+    if constexpr(part.type() == PartitionerType::STATIC) {
       size_t chunk_size;
       for(size_t w=0, curr_b=0; w<W && curr_b < N; ++w, curr_b += chunk_size) {
         chunk_size = part.adjusted_chunk_size(N, W, w);
-        launch_loop(W, w, rt, [=, &c, &part] () mutable {
+        launch_loop(W, w, rt, part, [=, &c, &part] () mutable {
           part.loop(N, W, curr_b, chunk_size,
-            [&, prev_e=size_t{0}](size_t curr_b, size_t curr_e) mutable {
-              std::advance(beg, curr_b - prev_e);
-              for(size_t x = curr_b; x<curr_e; x++) {
+            [&, prev_e=size_t{0}](size_t part_b, size_t part_e) mutable {
+              std::advance(beg, part_b - prev_e);
+              for(size_t x = part_b; x<part_e; x++) {
                 c(*beg++);
               }
-              prev_e = curr_e;
+              prev_e = part_e;
             }
           ); 
         });
       }
 
-      rt.join();
+      rt.corun_all();
     }
     // dynamic partitioner
     else {
       std::atomic<size_t> next(0);
       launch_loop(N, W, rt, next, part, [=, &c, &next, &part] () mutable {
         part.loop(N, W, next, 
-          [&, prev_e=size_t{0}](size_t curr_b, size_t curr_e) mutable {
-            std::advance(beg, curr_b - prev_e);
-            for(size_t x = curr_b; x<curr_e; x++) {
+          [&, prev_e=size_t{0}](size_t part_b, size_t part_e) mutable {
+            std::advance(beg, part_b - prev_e);
+            for(size_t x = part_b; x<part_e; x++) {
               c(*beg++);
             }
-            prev_e = curr_e;
+            prev_e = part_e;
           }
-        ); 
+        );
       });
     }
   };
 }
 
 // Function: make_for_each_index_task
-template <typename B, typename E, typename S, typename C, typename P>
-TF_FORCE_INLINE auto make_for_each_index_task(B beg, E end, S inc, C c, P&& part){
-
-  using namespace std::string_literals;
+template <typename B, typename E, typename S, typename C, typename P = DefaultPartitioner>
+auto make_for_each_index_task(B b, E e, S s, C c, P part = P()){
 
   using B_t = std::decay_t<unwrap_ref_decay_t<B>>;
   using E_t = std::decay_t<unwrap_ref_decay_t<E>>;
   using S_t = std::decay_t<unwrap_ref_decay_t<S>>;
 
-  return [b=beg, e=end, a=inc, c, part=std::forward<P>(part)] 
-  (Runtime& rt) mutable {
+  return [=] (Runtime& rt) mutable {
 
     // fetch the iterator values
     B_t beg = b;
     E_t end = e;
-    S_t inc = a;
+    S_t inc = s;
+    
+    // nothing to be done if the range is invalid
+    if(is_range_invalid(beg, end, inc)) {
+      return;
+    }
 
     size_t W = rt.executor().num_workers();
     size_t N = distance(beg, end, inc);
 
     // only myself - no need to spawn another graph
     if(W <= 1 || N <= part.chunk_size()) {
-      for(size_t x=0; x<N; x++, beg+=inc) {
-        c(beg);
-      }
+      launch_loop(part, [&](){
+        for(size_t x=0; x<N; x++, beg+=inc) {
+          c(beg);
+        }
+      });
       return;
     }
 
     if(N < W) {
       W = N;
     }
     
     // static partitioner
-    if constexpr(std::is_same_v<std::decay_t<P>, StaticPartitioner>) {
-
+    if constexpr(part.type() == PartitionerType::STATIC) {
       size_t chunk_size;
-
       for(size_t w=0, curr_b=0; w<W && curr_b < N; ++w, curr_b += chunk_size) {
         chunk_size = part.adjusted_chunk_size(N, W, w);
-        launch_loop(W, w, rt, [=, &c, &part] () mutable {
+        launch_loop(W, w, rt, part, [=, &c, &part] () mutable {
           part.loop(N, W, curr_b, chunk_size,
-            [&](size_t curr_b, size_t curr_e) {
-              auto idx = static_cast<B_t>(curr_b) * inc + beg;
-              for(size_t x=curr_b; x<curr_e; x++, idx += inc) {
+            [&](size_t part_b, size_t part_e) {
+              auto idx = static_cast<B_t>(part_b) * inc + beg;
+              for(size_t x=part_b; x<part_e; x++, idx += inc) {
                 c(idx);
               }
             }
-          ); 
+          );
         });
       }
 
-      rt.join();
+      rt.corun_all();
     }
     // dynamic partitioner
     else {
       std::atomic<size_t> next(0);
       launch_loop(N, W, rt, next, part, [=, &c, &next, &part] () mutable {
         part.loop(N, W, next, 
-          [&](size_t curr_b, size_t curr_e) {
-            auto idx = static_cast<B_t>(curr_b) * inc + beg;
-            for(size_t x=curr_b; x<curr_e; x++, idx += inc) {
+          [&](size_t part_b, size_t part_e) {
+            auto idx = static_cast<B_t>(part_b) * inc + beg;
+            for(size_t x=part_b; x<part_e; x++, idx += inc) {
               c(idx);
             }
           }
-        ); 
+        );
       });
     }
   };
 }
 
-}  // end of namespace detail -------------------------------------------------
-
 // ----------------------------------------------------------------------------
 // for_each
 // ----------------------------------------------------------------------------
 
 // Function: for_each
 template <typename B, typename E, typename C, typename P>
-Task FlowBuilder::for_each(B beg, E end, C c, P&& part) {
+Task FlowBuilder::for_each(B beg, E end, C c, P part) {
   return emplace(
-    detail::make_for_each_task(beg, end, c, std::forward<P>(part))
+    make_for_each_task(beg, end, c, part)
   );
 }
 
 // ----------------------------------------------------------------------------
 // for_each_index
 // ----------------------------------------------------------------------------
 
 // Function: for_each_index
 template <typename B, typename E, typename S, typename C, typename P>
-Task FlowBuilder::for_each_index(B beg, E end, S inc, C c, P&& part){
+Task FlowBuilder::for_each_index(B beg, E end, S inc, C c, P part){
   return emplace(
-    detail::make_for_each_index_task(beg, end, inc, c, std::forward<P>(part))
+    make_for_each_index_task(beg, end, inc, c, part)
   );
 }
 
 
 }  // end of namespace tf -----------------------------------------------------
```

### Comparing `rapidfuzz-3.9.0/extern/taskflow/taskflow/algorithm/launch.hpp` & `rapidfuzz-3.9.1/extern/taskflow/taskflow/algorithm/launch.hpp`

 * *Files 18% similar despite different names*

```diff
@@ -1,58 +1,76 @@
 #pragma once
 
+#include <functional>
 #include "../core/async.hpp"
 
 namespace tf {
 
 // Function: launch_loop
+template<typename P, typename Loop>
+TF_FORCE_INLINE void launch_loop(P part, Loop loop) {
+
+  constexpr bool is_default_wrapper_v = std::is_same_v<
+    typename std::decay_t<P>::closure_wrapper_type, DefaultClosureWrapper
+  >;
+  
+  if constexpr(is_default_wrapper_v) {
+    loop();
+  }
+  else {
+    std::invoke(part.closure_wrapper(), loop);
+  }
+}
+
+// Function: launch_loop
 template <typename P, typename Loop>
 TF_FORCE_INLINE void launch_loop(
   size_t N, 
   size_t W, 
   Runtime& rt, 
   std::atomic<size_t>& next, 
-  P&& part, 
-  Loop&& loop
+  P part, 
+  Loop loop
 ) {
 
   //static_assert(std::is_lvalue_reference_v<Loop>, "");
   
   using namespace std::string_literals;
 
   for(size_t w=0; w<W; w++) {
     auto r = N - next.load(std::memory_order_relaxed);
     // no more loop work to do - finished by previous async tasks
     if(!r) {
       break;
     }
     // tail optimization
     if(r <= part.chunk_size() || w == W-1) {
-      loop();
+      launch_loop(part, loop);
       break;
     }
     else {
-      rt.silent_async_unchecked("loop-"s + std::to_string(w), loop);
+      rt.silent_async_unchecked([=](){ launch_loop(part, loop); });
     }
   }
       
-  rt.join();
+  rt.corun_all();
 }
 
 // Function: launch_loop
-template <typename Loop>
+template <typename P, typename Loop>
 TF_FORCE_INLINE void launch_loop(
   size_t W,
   size_t w,
   Runtime& rt, 
-  Loop&& loop 
+  P part,
+  Loop loop 
 ) {
   using namespace std::string_literals;
   if(w == W-1) {
-    loop();
+    launch_loop(part, loop);
   }
   else {
-    rt.silent_async_unchecked("loop-"s + std::to_string(w), loop);
+    rt.silent_async_unchecked([=](){ launch_loop(part, loop); });
   }
 }
 
 }  // end of namespace tf -----------------------------------------------------
```

### Comparing `rapidfuzz-3.9.0/extern/taskflow/taskflow/algorithm/pipeline.hpp` & `rapidfuzz-3.9.1/extern/taskflow/taskflow/algorithm/pipeline.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -1074,14 +1074,15 @@
   /**
   @private
   */
   struct Line {
     std::atomic<size_t> join_counter;
   };
 
+
   public:
 
   /**
   @brief pipe type
   */
   using pipe_t = typename std::iterator_traits<P>::value_type;
 
@@ -1278,14 +1279,15 @@
     TF_THROW("must have at least one line");
   }
 
   reset(first, last);
   _build();
 }
 
+/*
 // move constructor
 template <typename P>
 ScalablePipeline<P>::ScalablePipeline(ScalablePipeline&& rhs) :
   _graph              {std::move(rhs._graph)},
   _num_tokens         {rhs._num_tokens},
   _pipes              {std::move(rhs._pipes)},
   _tasks              {std::move(rhs._tasks)},
@@ -1294,31 +1296,107 @@
   _ready_tokens       {std::move(rhs._ready_tokens)},
   _token_dependencies {std::move(rhs._token_dependencies)},
   _deferred_tokens    {std::move(rhs._deferred_tokens)},
   _longest_deferral   {rhs._longest_deferral}{
 
   rhs._longest_deferral = 0;
   rhs._num_tokens       = 0;
+  std::cout << "scalable move constructor\n";
 }
+*/
+
+// move constructor
+template <typename P>
+ScalablePipeline<P>::ScalablePipeline(ScalablePipeline&& rhs):
+  _num_tokens           {rhs._num_tokens},
+  _pipes                {std::move(rhs._pipes)},
+  _pipeflows            {std::move(rhs._pipeflows)},
+  _lines                {std::move(rhs._lines)},
+  _ready_tokens         {std::move(rhs._ready_tokens)},
+  _token_dependencies   {std::move(rhs._token_dependencies)},
+  _deferred_tokens      {std::move(rhs._deferred_tokens)},
+  _longest_deferral     {rhs._longest_deferral}{
+
+
+  //_num_tokens = rhs._num_tokens;
+
+  //_pipes.resize(rhs.num_pipes());
+  //size_t i=0;
+  //for(auto itr = rhs._pipes.begin(); itr != rhs._pipes.end(); itr++) {
+  //  _pipes[i++] = *itr;
+  //}
+
+
+  //_pipeflows.resize(rhs.num_lines());
+  //for(size_t l = 0; l<rhs.num_lines(); l++) {
+  //  _pipeflows[l]._pipe = rhs._pipeflows[l]._pipe;
+  //  _pipeflows[l]._line = rhs._pipeflows[l]._line;
+  //  _pipeflows[l]._num_deferrals = 0;
+  //  _pipeflows[l]._dependents.clear();
+  //}
+
+  //_lines = std::make_unique<Line[]>(rhs.num_lines() * rhs._pipes.size());
+  //for(size_t l=0; l<num_lines(); l++) {
+  //  for(size_t f=0; f<num_pipes(); f++) {
+  //    _line(l, f).join_counter.store(
+  //      rhs._line(l, f).join_counter, std::memory_order_relaxed
+  //    );
+  //  }
+  //}
+ 
+  //_ready_tokens = std::move(rhs._ready_tokens);
+  //_token_dependencies = std::move(rhs._token_dependencies);
+  //_deferred_tokens = std::move(rhs._deferred_tokens);
+
+  _graph.clear();
+  _tasks.resize(_pipeflows.size()+1);
+  rhs._longest_deferral = 0;
+  rhs._num_tokens       = 0;
+  rhs._tasks.clear();
+  _build();
+}
+
+//// move assignment operator
+//template <typename P>
+//ScalablePipeline<P>& ScalablePipeline<P>::operator = (ScalablePipeline&& rhs) {
+//  _graph                = std::move(rhs._graph);
+//  _num_tokens           = rhs._num_tokens;
+//  _pipes                = std::move(rhs._pipes);
+//  _tasks                = std::move(rhs._tasks);
+//  _pipeflows            = std::move(rhs._pipeflows);
+//  _lines                = std::move(rhs._lines);
+//  rhs._num_tokens       = 0;
+//  _ready_tokens         = std::move(rhs._ready_tokens);
+//  _token_dependencies   = std::move(rhs._token_dependencies);
+//  _deferred_tokens      = std::move(rhs._deferred_tokens);
+//  _longest_deferral     = rhs._longest_deferral;
+//  rhs._longest_deferral = 0;
+//  std::cout << "scalable move assignment\n";
+//  return *this;
+//}
 
 // move assignment operator
 template <typename P>
 ScalablePipeline<P>& ScalablePipeline<P>::operator = (ScalablePipeline&& rhs) {
-  _graph                = std::move(rhs._graph);
-  _num_tokens           = rhs._num_tokens;
-  _pipes                = std::move(rhs._pipes);
-  _tasks                = std::move(rhs._tasks);
-  _pipeflows            = std::move(rhs._pipeflows);
-  _lines                = std::move(rhs._lines);
-  rhs._num_tokens       = 0;
-  _ready_tokens         = std::move(rhs._ready_tokens);
-  _token_dependencies   = std::move(rhs._token_dependencies);
-  _deferred_tokens      = std::move(rhs._deferred_tokens);
-  _longest_deferral     = rhs._longest_deferral;
+  _num_tokens         = rhs._num_tokens;
+  _pipes              = std::move(rhs._pipes);
+  _pipeflows          = std::move(rhs._pipeflows);
+  _lines              = std::move(rhs._lines);
+  _ready_tokens       = std::move(rhs._ready_tokens);
+  _token_dependencies = std::move(rhs._token_dependencies);
+  _deferred_tokens    = std::move(rhs._deferred_tokens);
+  _longest_deferral   = rhs._longest_deferral;
+
+  _graph.clear();
+  _tasks.resize(_pipeflows.size()+1);
+
   rhs._longest_deferral = 0;
+  rhs._num_tokens       = 0;
+  rhs._tasks.clear();
+  _build();
   return *this;
 }
 
 // Function: num_lines
 template <typename P>
 size_t ScalablePipeline<P>::num_lines() const noexcept {
   return _pipeflows.size();
@@ -1521,23 +1599,23 @@
 // Procedure: _build
 template <typename P>
 void ScalablePipeline<P>::_build() {
 
   using namespace std::literals::string_literals;
 
   FlowBuilder fb(_graph);
-
+  
   // init task
   _tasks[0] = fb.emplace([this]() {
     return static_cast<int>(_num_tokens % num_lines());
   }).name("cond");
 
   // line task
   for(size_t l = 0; l < num_lines(); l++) {
-
+    
     _tasks[l + 1] = fb.emplace([this, l] (tf::Runtime& rt) mutable {
 
       auto pf = &_pipeflows[l];
 
       pipeline:
 
       _line(pf->_line, pf->_pipe).join_counter.store(
@@ -1594,19 +1672,19 @@
         if (pf->_token <= _longest_deferral) {
           _resolve_token_dependencies(*pf); 
         }
       }
       else {
         _on_pipe(*pf, rt);
       }
-
+      
       size_t c_f = pf->_pipe;
       size_t n_f = (pf->_pipe + 1) % num_pipes();
       size_t n_l = (pf->_line + 1) % num_lines();
-
+      
       pf->_pipe = n_f;
 
       // ---- scheduling starts here ----
       // Notice that the shared variable f must not be changed after this
       // point because it can result in data race due to the following
       // condition:
       //
```

### Comparing `rapidfuzz-3.9.0/extern/taskflow/taskflow/algorithm/scan.hpp` & `rapidfuzz-3.9.1/extern/taskflow/taskflow/algorithm/scan.hpp`

 * *Files 6% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 
 namespace tf {
 
 namespace detail {
 
 // Function: scan_loop
 template <typename Iterator, typename BufferT, typename B>
-TF_FORCE_INLINE void scan_loop(
+void scan_loop(
   tf::Runtime& rt,
   std::atomic<size_t>& counter, 
   BufferT& buf, 
-  B&& bop, 
+  B bop, 
   Iterator d_beg, 
   size_t W,
   size_t w, 
   size_t chunk_size
 ){
   // whoever finishes the last performs global scan
   if(counter.fetch_add(1, std::memory_order_acq_rel) == W-1) {
@@ -38,23 +38,29 @@
   
   // block addup
   for(size_t i=0; i<chunk_size; i++) {
     *d_beg++ = bop(buf[w-1].data, *d_beg);
   }
 }
 
+}  // end of namespace tf::detail ---------------------------------------------
+
+
 // Function: make_inclusive_scan_task
-template <typename B, typename E, typename D, typename BOP>
-TF_FORCE_INLINE auto make_inclusive_scan_task(B first, E last, D d_first, BOP bop) {
+template <typename B, typename E, typename D, typename BOP, typename P = DefaultPartitioner,
+  std::enable_if_t<is_partitioner_v<std::decay_t<P>>, void>* = nullptr
+>
+auto make_inclusive_scan_task(
+  B first, E last, D d_first, BOP bop, P part = P()
+) {
   
   using B_t = std::decay_t<unwrap_ref_decay_t<B>>;
   using E_t = std::decay_t<unwrap_ref_decay_t<E>>;
   using D_t = std::decay_t<unwrap_ref_decay_t<D>>;
   using value_type = typename std::iterator_traits<B_t>::value_type;
-  using namespace std::string_literals;
   
   return [=] (Runtime& rt) mutable {
 
     // fetch the stateful values
     B_t s_beg = first;
     E_t s_end = last;
     D_t d_beg = d_first;
@@ -64,15 +70,17 @@
     }
 
     size_t W = rt.executor().num_workers();
     size_t N = std::distance(s_beg, s_end);
 
     // only myself - no need to spawn another graph
     if(W <= 1 || N <= 2) {
-      std::inclusive_scan(s_beg, s_end, d_beg, bop);
+      launch_loop(part, [&](){
+        std::inclusive_scan(s_beg, s_end, d_beg, bop);
+      });
       return;
     }
 
     if(N < W) {
       W = N;
     }
     
@@ -86,16 +94,15 @@
     //ExecutionPolicy<StaticPartitioner> policy;
 
     for(size_t w=0, curr_b=0, chunk_size; w<W && curr_b < N; ++w) {
 
       chunk_size = std::min(Q + (w < R), N - curr_b);
 
       // block scan
-      launch_loop(W, w, rt, [=, &rt, &bop, &buf, &counter] () mutable {
-
+      launch_loop(W, w, rt, part, [=, &rt, &bop, &buf, &counter] () mutable {
         auto result = d_beg;
 
         // local scan per worker
         auto& init = buf[w].data;
         *d_beg++ = init = *s_beg++;
 
         for(size_t i=1; i<chunk_size; i++){
@@ -130,27 +137,30 @@
       });
       
       std::advance(s_beg, chunk_size);
       std::advance(d_beg, chunk_size);
       curr_b += chunk_size;
     }
 
-    rt.join();
+    rt.corun_all();
   };
 }
 
 // Function: make_inclusive_scan_task
-template <typename B, typename E, typename D, typename BOP, typename T>
-TF_FORCE_INLINE auto make_inclusive_scan_task(B first, E last, D d_first, BOP bop, T init) {
+template <typename B, typename E, typename D, typename BOP, typename T, typename P = DefaultPartitioner,
+  std::enable_if_t<!is_partitioner_v<std::decay_t<T>>, void>* = nullptr
+>
+auto make_inclusive_scan_task(
+  B first, E last, D d_first, BOP bop, T init, P part = P()
+) {
   
   using B_t = std::decay_t<unwrap_ref_decay_t<B>>;
   using E_t = std::decay_t<unwrap_ref_decay_t<E>>;
   using D_t = std::decay_t<unwrap_ref_decay_t<D>>;
   using value_type = typename std::iterator_traits<B_t>::value_type;
-  using namespace std::string_literals;
   
   return [=] (Runtime& rt) mutable {
 
     // fetch the stateful values
     B_t s_beg = first;
     E_t s_end = last;
     D_t d_beg = d_first;
@@ -160,15 +170,17 @@
     }
 
     size_t W = rt.executor().num_workers();
     size_t N = std::distance(s_beg, s_end);
 
     // only myself - no need to spawn another graph
     if(W <= 1 || N <= 2) {
-      std::inclusive_scan(s_beg, s_end, d_beg, bop, init);
+      launch_loop(part, [&](){
+        std::inclusive_scan(s_beg, s_end, d_beg, bop, init);
+      });
       return;
     }
 
     if(N < W) {
       W = N;
     }
     
@@ -182,54 +194,54 @@
     size_t R = N%W;
 
     for(size_t w=0, curr_b=0, chunk_size; w<W && curr_b < N; ++w) {
 
       chunk_size = std::min(Q + (w < R), N - curr_b);
 
       // block scan
-      launch_loop(W, w, rt, [=, &rt, &bop, &buf, &counter] () mutable {
-
+      launch_loop(W, w, rt, part, [=, &rt, &bop, &buf, &counter] () mutable {
         auto result = d_beg;
 
         // local scan per worker
-        auto& init = buf[w].data;
-        *d_beg++ = init = (w == 0) ? bop(init, *s_beg++) : *s_beg++;
+        auto& local = buf[w].data;
+        *d_beg++ = local = (w == 0) ? bop(local, *s_beg++) : *s_beg++;
 
         for(size_t i=1; i<chunk_size; i++){
-          *d_beg++ = init = bop(init, *s_beg++); 
+          *d_beg++ = local = bop(local, *s_beg++); 
         }
         
         // block scan
         detail::scan_loop(rt, counter, buf, bop, result, W, w, chunk_size);
       });
 
       std::advance(s_beg, chunk_size);
       std::advance(d_beg, chunk_size);
       curr_b += chunk_size;
     }
 
-    rt.join();
+    rt.corun_all();
   };
 }
 
 // ----------------------------------------------------------------------------
 // Transform Inclusive Scan
 // ----------------------------------------------------------------------------
 
 // Function: transform_inclusive_scan
-template <typename B, typename E, typename D, typename BOP, typename UOP>
-TF_FORCE_INLINE auto make_transform_inclusive_scan_task(
-  B first, E last, D d_first, BOP bop, UOP uop
+template <typename B, typename E, typename D, typename BOP, typename UOP, typename P = DefaultPartitioner,
+  std::enable_if_t<is_partitioner_v<std::decay_t<P>>, void>* = nullptr
+>
+auto make_transform_inclusive_scan_task(
+  B first, E last, D d_first, BOP bop, UOP uop, P part = P()
 ) {
   
   using B_t = std::decay_t<unwrap_ref_decay_t<B>>;
   using E_t = std::decay_t<unwrap_ref_decay_t<E>>;
   using D_t = std::decay_t<unwrap_ref_decay_t<D>>;
   using value_type = typename std::iterator_traits<B_t>::value_type;
-  using namespace std::string_literals;
   
   return [=] (Runtime& rt) mutable {
 
     // fetch the stateful values
     B_t s_beg = first;
     E_t s_end = last;
     D_t d_beg = d_first;
@@ -239,15 +251,17 @@
     }
 
     size_t W = rt.executor().num_workers();
     size_t N = std::distance(s_beg, s_end);
 
     // only myself - no need to spawn another graph
     if(W <= 1 || N <= 2) {
-      std::transform_inclusive_scan(s_beg, s_end, d_beg, bop, uop);
+      launch_loop(part, [&](){
+        std::transform_inclusive_scan(s_beg, s_end, d_beg, bop, uop); 
+      });
       return;
     }
 
     if(N < W) {
       W = N;
     }
     
@@ -258,16 +272,15 @@
     size_t R = N%W;
     
     for(size_t w=0, curr_b=0, chunk_size; w<W && curr_b < N; ++w) {
 
       chunk_size = std::min(Q + (w < R), N - curr_b);
 
       // block scan
-      launch_loop(W, w, rt, [=, &rt, &bop, &uop, &buf, &counter] () mutable {
-
+      launch_loop(W, w, rt, part, [=, &rt, &bop, &uop, &buf, &counter] () mutable {
         auto result = d_beg;
 
         // local scan per worker
         auto& init = buf[w].data;
         *d_beg++ = init = uop(*s_beg++);
 
         for(size_t i=1; i<chunk_size; i++){
@@ -279,29 +292,30 @@
       });
       
       std::advance(s_beg, chunk_size);
       std::advance(d_beg, chunk_size);
       curr_b += chunk_size;
     }
 
-    rt.join();
+    rt.corun_all();
   };
 }
 
 // Function: transform_inclusive_scan
-template <typename B, typename E, typename D, typename BOP, typename UOP, typename T>
-TF_FORCE_INLINE auto make_transform_inclusive_scan_task(
-  B first, E last, D d_first, BOP bop, UOP uop, T init
+template <typename B, typename E, typename D, typename BOP, typename UOP, typename T, typename P = DefaultPartitioner,
+  std::enable_if_t<!is_partitioner_v<std::decay_t<T>>, void>* = nullptr
+>
+auto make_transform_inclusive_scan_task(
+  B first, E last, D d_first, BOP bop, UOP uop, T init, P part = P()
 ) {
   
   using B_t = std::decay_t<unwrap_ref_decay_t<B>>;
   using E_t = std::decay_t<unwrap_ref_decay_t<E>>;
   using D_t = std::decay_t<unwrap_ref_decay_t<D>>;
   using value_type = typename std::iterator_traits<B_t>::value_type;
-  using namespace std::string_literals;
   
   return [=] (Runtime& rt) mutable {
 
     // fetch the stateful values
     B_t s_beg = first;
     E_t s_end = last;
     D_t d_beg = d_first;
@@ -311,15 +325,17 @@
     }
 
     size_t W = rt.executor().num_workers();
     size_t N = std::distance(s_beg, s_end);
 
     // only myself - no need to spawn another graph
     if(W <= 1 || N <= 2) {
-      std::transform_inclusive_scan(s_beg, s_end, d_beg, bop, uop, init);
+      launch_loop(part, [&](){
+        std::transform_inclusive_scan(s_beg, s_end, d_beg, bop, uop, init);
+      });
       return;
     }
 
     if(N < W) {
       W = N;
     }
     
@@ -333,55 +349,53 @@
     size_t R = N%W;
 
     for(size_t w=0, curr_b=0, chunk_size; w<W && curr_b < N; ++w) {
 
       chunk_size = std::min(Q + (w < R), N - curr_b);
 
       // block scan
-      launch_loop(W, w, rt, [=, &rt, &bop, &uop, &buf, &counter] () mutable {
-
+      launch_loop(W, w, rt, part, [=, &rt, &bop, &uop, &buf, &counter] () mutable {
         auto result = d_beg;
 
         // local scan per worker
-        auto& init = buf[w].data;
-        *d_beg++ = init = (w == 0) ? bop(init, uop(*s_beg++)) : uop(*s_beg++);
+        auto& local = buf[w].data;
+        *d_beg++ = local = (w == 0) ? bop(local, uop(*s_beg++)) : uop(*s_beg++);
 
         for(size_t i=1; i<chunk_size; i++){
-          *d_beg++ = init = bop(init, uop(*s_beg++)); 
+          *d_beg++ = local = bop(local, uop(*s_beg++)); 
         }
         
         // block scan
         detail::scan_loop(rt, counter, buf, bop, result, W, w, chunk_size);
       });
 
       std::advance(s_beg, chunk_size);
       std::advance(d_beg, chunk_size);
       curr_b += chunk_size;
     }
 
-    rt.join();
+    rt.corun_all();
     
   };
 }
 
 // ----------------------------------------------------------------------------
 // Exclusive Scan
 // ----------------------------------------------------------------------------
 
 // Function: make_exclusive_scan_task
-template <typename B, typename E, typename D, typename T, typename BOP>
-TF_FORCE_INLINE auto make_exclusive_scan_task(
-  B first, E last, D d_first, T init, BOP bop
+template <typename B, typename E, typename D, typename T, typename BOP, typename P = DefaultPartitioner>
+auto make_exclusive_scan_task(
+  B first, E last, D d_first, T init, BOP bop, P part = P()
 ) {
   
   using B_t = std::decay_t<unwrap_ref_decay_t<B>>;
   using E_t = std::decay_t<unwrap_ref_decay_t<E>>;
   using D_t = std::decay_t<unwrap_ref_decay_t<D>>;
   using value_type = typename std::iterator_traits<B_t>::value_type;
-  using namespace std::string_literals;
   
   return [=] (Runtime& rt) mutable {
 
     // fetch the stateful values
     B_t s_beg = first;
     E_t s_end = last;
     D_t d_beg = d_first;
@@ -391,15 +405,17 @@
     }
 
     size_t W = rt.executor().num_workers();
     size_t N = std::distance(s_beg, s_end);
 
     // only myself - no need to spawn another graph
     if(W <= 1 || N <= 2) {
-      std::exclusive_scan(s_beg, s_end, d_beg, init, bop);
+      launch_loop(part, [&](){
+        std::exclusive_scan(s_beg, s_end, d_beg, init, bop);
+      });
       return;
     }
 
     if(N < W) {
       W = N;
     }
     
@@ -419,57 +435,55 @@
     }
     
     for(size_t w=0, curr_b=0, chunk_size; w<W && curr_b < N; ++w) {
 
       chunk_size = std::min(Q + (w < R), N - curr_b);
 
       // block scan
-      launch_loop(W, w, rt, [=, &rt, &bop, &buf, &counter] () mutable {
-
+      launch_loop(W, w, rt, part, [=, &rt, &bop, &buf, &counter] () mutable {
         auto result = d_beg;
 
         // local scan per worker
-        auto& init = buf[w].data;
+        auto& local = buf[w].data;
 
         for(size_t i=1; i<chunk_size; i++) {
-          auto v = init;
-          init = bop(init, *s_beg++);
+          auto v = local;
+          local = bop(local, *s_beg++);
           *d_beg++ = std::move(v);
         }
-        *d_beg++ = init;
+        *d_beg++ = local;
         
         // block scan
         detail::scan_loop(rt, counter, buf, bop, result, W, w, chunk_size);
       });
       
       std::advance(s_beg, chunk_size);
       std::advance(d_beg, chunk_size);
       curr_b += chunk_size;
     }
 
-    rt.join();
+    rt.corun_all();
     
   };
 }
 
 // ----------------------------------------------------------------------------
 // Transform Exclusive Scan
 // ----------------------------------------------------------------------------
 
 // Function: 
-template <typename B, typename E, typename D, typename T, typename BOP, typename UOP>
-TF_FORCE_INLINE auto make_transform_exclusive_scan_task(
-  B first, E last, D d_first, T init, BOP bop, UOP uop
+template <typename B, typename E, typename D, typename T, typename BOP, typename UOP, typename P = DefaultPartitioner>
+auto make_transform_exclusive_scan_task(
+  B first, E last, D d_first, T init, BOP bop, UOP uop, P part = P()
 ) {
   
   using B_t = std::decay_t<unwrap_ref_decay_t<B>>;
   using E_t = std::decay_t<unwrap_ref_decay_t<E>>;
   using D_t = std::decay_t<unwrap_ref_decay_t<D>>;
   using value_type = typename std::iterator_traits<B_t>::value_type;
-  using namespace std::string_literals;
   
   return [=] (Runtime& rt) mutable {
 
     // fetch the stateful values
     B_t s_beg = first;
     E_t s_end = last;
     D_t d_beg = d_first;
@@ -479,15 +493,17 @@
     }
 
     size_t W = rt.executor().num_workers();
     size_t N = std::distance(s_beg, s_end);
 
     // only myself - no need to spawn another graph
     if(W <= 1 || N <= 2) {
-      std::transform_exclusive_scan(s_beg, s_end, d_beg, init, bop, uop);
+      launch_loop(part, [&](){
+        std::transform_exclusive_scan(s_beg, s_end, d_beg, init, bop, uop);
+      });
       return;
     }
 
     if(N < W) {
       W = N;
     }
     
@@ -507,108 +523,111 @@
     }
     
     for(size_t w=0, curr_b=0, chunk_size; w<W && curr_b < N; ++w) {
 
       chunk_size = std::min(Q + (w < R), N - curr_b);
 
       // block scan
-      launch_loop(W, w, rt, [=, &rt, &bop, &uop, &buf, &counter] () mutable {
-
+      launch_loop(W, w, rt, part, [=, &rt, &bop, &uop, &buf, &counter] () mutable {
         auto result = d_beg;
 
         // local scan per worker
-        auto& init = buf[w].data;
+        auto& local = buf[w].data;
 
         for(size_t i=1; i<chunk_size; i++) {
-          auto v = init;
-          init = bop(init, uop(*s_beg++));
+          auto v = local;
+          local = bop(local, uop(*s_beg++));
           *d_beg++ = std::move(v);
         }
-        *d_beg++ = init;
+        *d_beg++ = local;
         
         // block scan
         detail::scan_loop(rt, counter, buf, bop, result, W, w, chunk_size);
       });
       
       std::advance(s_beg, chunk_size);
       std::advance(d_beg, chunk_size);
       curr_b += chunk_size;
     }
 
-    rt.join();
+    rt.corun_all();
     
   };
 }
 
-}  // end of namespace tf::detail ---------------------------------------------
 
 // ----------------------------------------------------------------------------
 // Inclusive Scan
 // ----------------------------------------------------------------------------
 
 // Function: inclusive_scan
-template <typename B, typename E, typename D, typename BOP>
-Task FlowBuilder::inclusive_scan(B first, E last, D d_first, BOP bop) {
-  return emplace(detail::make_inclusive_scan_task(
-    first, last, d_first, bop
-  ));
+template <typename B, typename E, typename D, typename BOP, typename P,
+  std::enable_if_t<is_partitioner_v<std::decay_t<P>>, void>*
+>
+Task FlowBuilder::inclusive_scan(B first, E last, D d_first, BOP bop, P part) {
+  return emplace(make_inclusive_scan_task(first, last, d_first, bop, part));
 }
 
 // Function: inclusive_scan
-template <typename B, typename E, typename D, typename BOP, typename T>
-Task FlowBuilder::inclusive_scan(B first, E last, D d_first, BOP bop, T init) {
-  return emplace(detail::make_inclusive_scan_task(
-    first, last, d_first, bop, init
-  ));
+template <typename B, typename E, typename D, typename BOP, typename T, typename P,
+  std::enable_if_t<!is_partitioner_v<std::decay_t<T>>, void>*
+>
+Task FlowBuilder::inclusive_scan(B first, E last, D d_first, BOP bop, T init, P part) {
+  return emplace(make_inclusive_scan_task(first, last, d_first, bop, init, part));
 }
 
 // ----------------------------------------------------------------------------
 // Transform Inclusive Scan
 // ----------------------------------------------------------------------------
 
 // Function: transform_inclusive_scan
-template <typename B, typename E, typename D, typename BOP, typename UOP>
+template <typename B, typename E, typename D, typename BOP, typename UOP, typename P,
+  std::enable_if_t<is_partitioner_v<std::decay_t<P>>, void>*
+>
 Task FlowBuilder::transform_inclusive_scan(
-  B first, E last, D d_first, BOP bop, UOP uop
+  B first, E last, D d_first, BOP bop, UOP uop, P part
 ) {
-  return emplace(detail::make_transform_inclusive_scan_task(
-    first, last, d_first, bop, uop
+  return emplace(make_transform_inclusive_scan_task(
+    first, last, d_first, bop, uop, part
   ));
 }
 
 // Function: transform_inclusive_scan
-template <typename B, typename E, typename D, typename BOP, typename UOP, typename T>
+template <typename B, typename E, typename D, typename BOP, typename UOP, typename T, typename P,
+  std::enable_if_t<!is_partitioner_v<std::decay_t<T>>, void>*
+>
 Task FlowBuilder::transform_inclusive_scan(
-  B first, E last, D d_first, BOP bop, UOP uop, T init
+  B first, E last, D d_first, BOP bop, UOP uop, T init, P part
 ) {
-  return emplace(detail::make_transform_inclusive_scan_task(
-    first, last, d_first, bop, uop, init
+  return emplace(make_transform_inclusive_scan_task(
+    first, last, d_first, bop, uop, init, part
   ));  
 }
 
 // ----------------------------------------------------------------------------
 // Exclusive Scan
 // ----------------------------------------------------------------------------
 
 // Function: exclusive_scan
-template <typename B, typename E, typename D, typename T, typename BOP>
-Task FlowBuilder::exclusive_scan(B first, E last, D d_first, T init, BOP bop) {
-  return emplace(detail::make_exclusive_scan_task(
-    first, last, d_first, init, bop
+template <typename B, typename E, typename D, typename T, typename BOP, typename P>
+Task FlowBuilder::exclusive_scan(B first, E last, D d_first, T init, BOP bop, P part) {
+  return emplace(make_exclusive_scan_task(
+    first, last, d_first, init, bop, part
   ));
 }
 
 // ----------------------------------------------------------------------------
 // Transform Exclusive Scan
 // ----------------------------------------------------------------------------
 
 // Function: transform_exclusive_scan
-template <typename B, typename E, typename D, typename T, typename BOP, typename UOP>
+template <typename B, typename E, typename D, typename T, typename BOP, typename UOP, typename P>
 Task FlowBuilder::transform_exclusive_scan(
-  B first, E last, D d_first, T init, BOP bop, UOP uop
+  B first, E last, D d_first, T init, BOP bop, UOP uop, P part
 ) {
-  return emplace(detail::make_transform_exclusive_scan_task(
-    first, last, d_first, init, bop, uop
+  return emplace(make_transform_exclusive_scan_task(
+    first, last, d_first, init, bop, uop, part
   )); 
 }
 
 }  // end of namespace tf -----------------------------------------------------
+
```

### Comparing `rapidfuzz-3.9.0/extern/taskflow/taskflow/algorithm/sort.hpp` & `rapidfuzz-3.9.1/extern/taskflow/taskflow/algorithm/sort.hpp`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #pragma once
 
 #include "../core/async.hpp"
 
-namespace tf {
+namespace tf::detail {
 
 // threshold whether or not to perform parallel sort
 template <typename I>
 constexpr size_t parallel_sort_cutoff() {
 
   //using value_type = std::decay_t<decltype(*std::declval<I>())>;
   using value_type = typename std::iterator_traits<I>::value_type;
@@ -591,58 +591,71 @@
     first = r+1;
     goto sort_partition;
   }
 
   //rt.join();
 }
 
-// ----------------------------------------------------------------------------
-// tf::Taskflow::sort
-// ----------------------------------------------------------------------------
+}  // end of namespace tf::detail ---------------------------------------------
 
-// Function: sort
-template <typename B, typename E, typename C>
-Task FlowBuilder::sort(B beg, E end, C cmp) {
+namespace tf { 
 
-  Task task = emplace([b=beg, e=end, cmp] (Runtime& rt) mutable {
+// Function: make_sort_task
+template <typename B, typename E, typename C>
+TF_FORCE_INLINE auto make_sort_task(B b, E e, C cmp) {
+  
+  return [b, e, cmp] (Runtime& rt) mutable {
 
     using B_t = std::decay_t<unwrap_ref_decay_t<B>>;
     using E_t = std::decay_t<unwrap_ref_decay_t<E>>;
 
     // fetch the iterator values
     B_t beg = b;
     E_t end = e;
 
     if(beg == end) {
       return;
     }
 
-    size_t W = rt._executor.num_workers();
+    size_t W = rt.executor().num_workers();
     size_t N = std::distance(beg, end);
 
     // only myself - no need to spawn another graph
-    if(W <= 1 || N <= parallel_sort_cutoff<B_t>()) {
+    if(W <= 1 || N <= detail::parallel_sort_cutoff<B_t>()) {
       std::sort(beg, end, cmp);
       return;
     }
 
     //parallel_3wqsort(rt, beg, end-1, cmp);
-    parallel_pdqsort<B_t, C,
+    detail::parallel_pdqsort<B_t, C,
       is_std_compare_v<std::decay_t<C>> &&
       std::is_arithmetic_v<typename std::iterator_traits<B_t>::value_type>
     >(rt, beg, end, cmp, log2(end - beg));
 
-    rt.join();
-  });
+    rt.corun_all();
+  };
+}
+  
+template <typename B, typename E>
+TF_FORCE_INLINE auto make_sort_task(B beg, E end) {
+  using value_type = std::decay_t<decltype(*std::declval<B>())>;
+  return make_sort_task(beg, end, std::less<value_type>{});
+}
+
+// ----------------------------------------------------------------------------
+// tf::Taskflow::sort
+// ----------------------------------------------------------------------------
 
-  return task;
+// Function: sort
+template <typename B, typename E, typename C>
+Task FlowBuilder::sort(B beg, E end, C cmp) {
+  return emplace(make_sort_task(beg, end, cmp));
 }
 
 // Function: sort
 template <typename B, typename E>
 Task FlowBuilder::sort(B beg, E end) {
-  using value_type = std::decay_t<decltype(*std::declval<B>())>;
-  return sort(beg, end, std::less<value_type>{});
+  return emplace(make_sort_task(beg, end));
 }
 
 }  // namespace tf ------------------------------------------------------------
```

### Comparing `rapidfuzz-3.9.0/extern/taskflow/taskflow/algorithm/transform.hpp` & `rapidfuzz-3.9.1/extern/taskflow/taskflow/algorithm/transform.hpp`

 * *Files 22% similar despite different names*

```diff
@@ -1,198 +1,189 @@
 #pragma once
 
 #include "launch.hpp"
 
 namespace tf {
 
-namespace detail {
-
 // Function: make_transform_task
-template <typename B, typename E, typename O, typename C, typename P>
-TF_FORCE_INLINE auto make_transform_task(
-  B first1, E last1, O d_first, C c, P&& part
-) {
-
-  using namespace std::string_literals;
+template <
+  typename B, typename E, typename O, typename C, typename P = DefaultPartitioner,
+  std::enable_if_t<is_partitioner_v<std::decay_t<P>>, void>* = nullptr
+>
+auto make_transform_task(B first1, E last1, O d_first, C c, P part = P()) {
 
   using B_t = std::decay_t<unwrap_ref_decay_t<B>>;
   using E_t = std::decay_t<unwrap_ref_decay_t<E>>;
   using O_t = std::decay_t<unwrap_ref_decay_t<O>>;
   
-  return
-  [first1, last1, d_first, c, part=std::forward<P>(part)] 
-  (Runtime& rt) mutable {
+  return [=] (Runtime& rt) mutable {
 
     // fetch the stateful values
     B_t beg   = first1;
     E_t end   = last1;
     O_t d_beg = d_first;
 
     size_t W = rt.executor().num_workers();
     size_t N = std::distance(beg, end);
 
     // only myself - no need to spawn another graph
     if(W <= 1 || N <= part.chunk_size()) {
-      std::transform(beg, end, d_beg, c);
+      launch_loop(part, [&](){
+        std::transform(beg, end, d_beg, c);
+      });
       return;
     }
 
     if(N < W) {
       W = N;
     }
 
     // static partitioner
-    if constexpr(std::is_same_v<std::decay_t<P>, StaticPartitioner>) {
+    if constexpr(part.type() == PartitionerType::STATIC) {
       size_t chunk_size;
       for(size_t w=0, curr_b=0; w<W && curr_b < N; ++w, curr_b += chunk_size) {
         chunk_size = part.adjusted_chunk_size(N, W, w);
-        launch_loop(W, w, rt, [=, &part] () mutable {
+        launch_loop(W, w, rt, part, [=, &part] () mutable {
           part.loop(N, W, curr_b, chunk_size,
-            [&, prev_e=size_t{0}](size_t curr_b, size_t curr_e) mutable {
-              std::advance(beg, curr_b - prev_e);
-              std::advance(d_beg, curr_b - prev_e);
-              for(size_t x = curr_b; x<curr_e; x++) {
+            [&, prev_e=size_t{0}](size_t part_b, size_t part_e) mutable {
+              std::advance(beg, part_b - prev_e);
+              std::advance(d_beg, part_b - prev_e);
+              for(size_t x = part_b; x<part_e; x++) {
                 *d_beg++ = c(*beg++);
               }
-              prev_e = curr_e;
+              prev_e = part_e;
             }
-          ); 
+          );
         });
       }
-      rt.join();
+      rt.corun_all();
     }
     // dynamic partitioner
     else {
       std::atomic<size_t> next(0);
-      
       launch_loop(N, W, rt, next, part, [=, &next, &part] () mutable {
         part.loop(N, W, next, 
-          [&, prev_e=size_t{0}](size_t curr_b, size_t curr_e) mutable {
-            std::advance(beg, curr_b - prev_e);
-            std::advance(d_beg, curr_b - prev_e);
-            for(size_t x = curr_b; x<curr_e; x++) {
+          [&, prev_e=size_t{0}](size_t part_b, size_t part_e) mutable {
+            std::advance(beg, part_b - prev_e);
+            std::advance(d_beg, part_b - prev_e);
+            for(size_t x = part_b; x<part_e; x++) {
               *d_beg++ = c(*beg++);
             }
-            prev_e = curr_e;
+            prev_e = part_e;
           }
         ); 
       });
     }
   };
 }
 
 // Function: make_transform_task
 template <
-  typename B1, typename E1, typename B2, typename O, typename C, typename P,
+  typename B1, typename E1, typename B2, typename O, typename C, typename P = DefaultPartitioner,
   std::enable_if_t<!is_partitioner_v<std::decay_t<C>>, void>* = nullptr
 >
-TF_FORCE_INLINE auto make_transform_task(
-  B1 first1, E1 last1, B2 first2, O d_first, C c, P&& part
-) {
-
-  using namespace std::string_literals;
+auto make_transform_task(B1 first1, E1 last1, B2 first2, O d_first, C c, P part = P()) {
 
   using B1_t = std::decay_t<unwrap_ref_decay_t<B1>>;
   using E1_t = std::decay_t<unwrap_ref_decay_t<E1>>;
   using B2_t = std::decay_t<unwrap_ref_decay_t<B2>>;
   using O_t = std::decay_t<unwrap_ref_decay_t<O>>;
 
-  return
-  [first1, last1, first2, d_first, c, part=std::forward<P>(part)] 
-  (Runtime& rt) mutable {
+  return [=] (Runtime& rt) mutable {
 
     // fetch the stateful values
     B1_t beg1 = first1;
     E1_t end1 = last1;
     B2_t beg2 = first2;
     O_t d_beg = d_first;
 
     size_t W = rt.executor().num_workers();
     size_t N = std::distance(beg1, end1);
 
     // only myself - no need to spawn another graph
     if(W <= 1 || N <= part.chunk_size()) {
-      std::transform(beg1, end1, beg2, d_beg, c);
+      launch_loop(part, [&](){
+        std::transform(beg1, end1, beg2, d_beg, c);
+      });
       return;
     }
 
     if(N < W) {
       W = N;
     }
 
     // static partitioner
-    if constexpr(std::is_same_v<std::decay_t<P>, StaticPartitioner>) {
+    if constexpr(part.type() == PartitionerType::STATIC) {
       size_t chunk_size;
       for(size_t w=0, curr_b=0; w<W && curr_b < N; ++w, curr_b += chunk_size) {
         chunk_size = part.adjusted_chunk_size(N, W, w);
-        launch_loop(W, w, rt, [=, &c, &part] () mutable {
+        launch_loop(W, w, rt, part, [=, &c, &part] () mutable {
           part.loop(N, W, curr_b, chunk_size,
-            [&, prev_e=size_t{0}](size_t curr_b, size_t curr_e) mutable {
-              std::advance(beg1, curr_b - prev_e);
-              std::advance(beg2, curr_b - prev_e);
-              std::advance(d_beg, curr_b - prev_e);
-              for(size_t x = curr_b; x<curr_e; x++) {
+            [&, prev_e=size_t{0}](size_t part_b, size_t part_e) mutable {
+              std::advance(beg1, part_b - prev_e);
+              std::advance(beg2, part_b - prev_e);
+              std::advance(d_beg, part_b - prev_e);
+              for(size_t x = part_b; x<part_e; x++) {
                 *d_beg++ = c(*beg1++, *beg2++);
               }
-              prev_e = curr_e;
+              prev_e = part_e;
             }
-          ); 
+          );
         });
       }
-      rt.join();
+      rt.corun_all();
     }
     // dynamic partitioner
     else {
       std::atomic<size_t> next(0);
       launch_loop(N, W, rt, next, part, [=, &c, &next, &part] () mutable {
         part.loop(N, W, next, 
-          [&, prev_e=size_t{0}](size_t curr_b, size_t curr_e) mutable {
-            std::advance(beg1, curr_b - prev_e);
-            std::advance(beg2, curr_b - prev_e);
-            std::advance(d_beg, curr_b - prev_e);
-            for(size_t x = curr_b; x<curr_e; x++) {
+          [&, prev_e=size_t{0}](size_t part_b, size_t part_e) mutable {
+            std::advance(beg1, part_b - prev_e);
+            std::advance(beg2, part_b - prev_e);
+            std::advance(d_beg, part_b - prev_e);
+            for(size_t x = part_b; x<part_e; x++) {
               *d_beg++ = c(*beg1++, *beg2++);
             }
-            prev_e = curr_e;
+            prev_e = part_e;
           }
-        ); 
+        );
       });
     }
   };
 }
 
-}  // end of namespace detail -------------------------------------------------
-
 // ----------------------------------------------------------------------------
 // transform
 // ----------------------------------------------------------------------------
 
 // Function: transform
-template <typename B, typename E, typename O, typename C, typename P>
-Task FlowBuilder::transform(B first1, E last1, O d_first, C c, P&& part) {
+template <typename B, typename E, typename O, typename C, typename P,
+  std::enable_if_t<is_partitioner_v<std::decay_t<P>>, void>*
+>
+Task FlowBuilder::transform(B first1, E last1, O d_first, C c, P part) {
   return emplace(
-    detail::make_transform_task(first1, last1, d_first, c, std::forward<P>(part))
+    make_transform_task(first1, last1, d_first, c, part)
   );
 }
 
 // ----------------------------------------------------------------------------
 // transform2
 // ----------------------------------------------------------------------------
   
 // Function: transform
 template <
   typename B1, typename E1, typename B2, typename O, typename C, typename P,
   std::enable_if_t<!is_partitioner_v<std::decay_t<C>>, void>*
 >
 Task FlowBuilder::transform(
-  B1 first1, E1 last1, B2 first2, O d_first, C c, P&& part
+  B1 first1, E1 last1, B2 first2, O d_first, C c, P part
 ) {
-
-  return emplace(detail::make_transform_task(
-    first1, last1, first2, d_first, c, std::forward<P>(part)
+  return emplace(make_transform_task(
+    first1, last1, first2, d_first, c, part
   ));
 }
 
 
 }  // end of namespace tf -----------------------------------------------------
```

### Comparing `rapidfuzz-3.9.0/extern/taskflow/taskflow/core/async.hpp` & `rapidfuzz-3.9.1/extern/taskflow/taskflow/core/async.hpp`

 * *Files 21% similar despite different names*

```diff
@@ -7,83 +7,71 @@
 namespace tf {
 
 // ----------------------------------------------------------------------------
 // Async
 // ----------------------------------------------------------------------------
 
 // Function: async
-template <typename F>
-auto Executor::async(const std::string& name, F&& f) {
+template <typename P, typename F>
+auto Executor::async(P&& params, F&& f) {
 
   _increment_topology();
 
   using R = std::invoke_result_t<std::decay_t<F>>;
 
-  std::promise<R> p;
+  std::packaged_task<R()> p(std::forward<F>(f));
   auto fu{p.get_future()};
 
   auto node = node_pool.animate(
-    name, 0, nullptr, nullptr, 0,
+    std::forward<P>(params), nullptr, nullptr, 0, 
+    // handle
     std::in_place_type_t<Node::Async>{}, 
-    _make_promised_async(std::move(p), std::forward<F>(f))
+    [p=make_moc(std::move(p))]() mutable { p.object(); }
   );
 
   _schedule_async_task(node);
 
   return fu;
 }
 
 // Function: async
 template <typename F>
 auto Executor::async(F&& f) {
-  return async("", std::forward<F>(f));
+  return async(DefaultTaskParams{}, std::forward<F>(f));
 }
 
 // ----------------------------------------------------------------------------
 // Silent Async
 // ----------------------------------------------------------------------------
 
 // Function: silent_async
-template <typename F>
-void Executor::silent_async(const std::string& name, F&& f) {
+template <typename P, typename F>
+void Executor::silent_async(P&& params, F&& f) {
 
   _increment_topology();
-
+  
   auto node = node_pool.animate(
-    name, 0, nullptr, nullptr, 0,
+    std::forward<P>(params), nullptr, nullptr, 0, 
+    // handle
     std::in_place_type_t<Node::Async>{}, std::forward<F>(f)
   );
 
   _schedule_async_task(node);
 }
 
 // Function: silent_async
 template <typename F>
 void Executor::silent_async(F&& f) {
-  silent_async("", std::forward<F>(f));
+  silent_async(DefaultTaskParams{}, std::forward<F>(f));
 }
 
 // ----------------------------------------------------------------------------
 // Async Helper Methods
 // ----------------------------------------------------------------------------
 
-// Function: _make_promised_async
-template <typename R, typename F>
-auto Executor::_make_promised_async(std::promise<R>&& p, F&& func) {
-  return [p=make_moc(std::move(p)), func=std::forward<F>(func)]() mutable {
-    if constexpr(std::is_same_v<R, void>) {
-      func();
-      p.object.set_value();
-    }
-    else {
-      p.object.set_value(func());
-    }
-  };
-}
-  
 // Procedure: _schedule_async_task
 inline void Executor::_schedule_async_task(Node* node) {  
   if(auto w = _this_worker(); w) {
     _schedule(*w, node);
   }
   else{
     _schedule(node);
@@ -94,302 +82,249 @@
 inline void Executor::_tear_down_async(Node* node) {
   // from runtime
   if(node->_parent) {
     node->_parent->_join_counter.fetch_sub(1, std::memory_order_release);
   }
   // from executor
   else {
-    _decrement_topology_and_notify();
+    _decrement_topology();
   }
   node_pool.recycle(node);
 }
 
 // ----------------------------------------------------------------------------
 // Silent Dependent Async
 // ----------------------------------------------------------------------------
 
 // Function: silent_dependent_async
 template <typename F, typename... Tasks,
   std::enable_if_t<all_same_v<AsyncTask, std::decay_t<Tasks>...>, void>*
 >
 tf::AsyncTask Executor::silent_dependent_async(F&& func, Tasks&&... tasks) {
-  return silent_dependent_async("", std::forward<F>(func), std::forward<Tasks>(tasks)...);
+  return silent_dependent_async(
+    DefaultTaskParams{}, std::forward<F>(func), std::forward<Tasks>(tasks)...
+  );
 }
 
 // Function: silent_dependent_async
-template <typename F, typename... Tasks,
-  std::enable_if_t<all_same_v<AsyncTask, std::decay_t<Tasks>...>, void>*
+template <typename P, typename F, typename... Tasks,
+  std::enable_if_t<is_task_params_v<P> && all_same_v<AsyncTask, std::decay_t<Tasks>...>, void>*
 >
 tf::AsyncTask Executor::silent_dependent_async(
-  const std::string& name, F&& func, Tasks&&... tasks 
+  P&& params, F&& func, Tasks&&... tasks 
 ){
 
   _increment_topology();
 
   size_t num_dependents = sizeof...(Tasks);
   
-  std::shared_ptr<Node> node(
-    node_pool.animate(
-      name, 0, nullptr, nullptr, num_dependents,
-      std::in_place_type_t<Node::DependentAsync>{}, std::forward<F>(func)
-    ),
-    [&](Node* ptr){ node_pool.recycle(ptr); }
-  );
-  
-  {
-    std::scoped_lock lock(_asyncs_mutex);
-    _asyncs.insert(node);
-  }
+  // create a task before scheduling the node to retain a shared ownership first
+  AsyncTask task(node_pool.animate(
+    std::forward<P>(params), nullptr, nullptr, num_dependents,
+    std::in_place_type_t<Node::DependentAsync>{}, std::forward<F>(func)
+  ));
   
   if constexpr(sizeof...(Tasks) > 0) {
-    (_process_async_dependent(node.get(), tasks, num_dependents), ...);
+    (_process_async_dependent(task._node, tasks, num_dependents), ...);
   }
 
   if(num_dependents == 0) {
-    _schedule_async_task(node.get());
+    _schedule_async_task(task._node);
   }
 
-  return AsyncTask(std::move(node));
+  return task;
 }
 
 // Function: silent_dependent_async
 template <typename F, typename I,
   std::enable_if_t<!std::is_same_v<std::decay_t<I>, AsyncTask>, void>*
 >
 tf::AsyncTask Executor::silent_dependent_async(F&& func, I first, I last) {
-  return silent_dependent_async("", std::forward<F>(func), first, last);
+  return silent_dependent_async(DefaultTaskParams{}, std::forward<F>(func), first, last);
 }
 
 // Function: silent_dependent_async
-template <typename F, typename I,
-  std::enable_if_t<!std::is_same_v<std::decay_t<I>, AsyncTask>, void>*
+template <typename P, typename F, typename I,
+  std::enable_if_t<is_task_params_v<P> && !std::is_same_v<std::decay_t<I>, AsyncTask>, void>*
 >
 tf::AsyncTask Executor::silent_dependent_async(
-  const std::string& name, F&& func, I first, I last
+  P&& params, F&& func, I first, I last
 ) {
 
   _increment_topology();
 
   size_t num_dependents = std::distance(first, last);
   
-  std::shared_ptr<Node> node(
-    node_pool.animate(
-      name, 0, nullptr, nullptr, num_dependents,
-      std::in_place_type_t<Node::DependentAsync>{}, std::forward<F>(func)
-    ),
-    [&](Node* ptr){ node_pool.recycle(ptr); }
-  );
-  
-  {
-    std::scoped_lock lock(_asyncs_mutex);
-    _asyncs.insert(node);
-  }
+  AsyncTask task(node_pool.animate(
+    std::forward<P>(params), nullptr, nullptr, num_dependents,
+    std::in_place_type_t<Node::DependentAsync>{}, std::forward<F>(func)
+  ));
   
   for(; first != last; first++){
-    _process_async_dependent(node.get(), *first, num_dependents);
+    _process_async_dependent(task._node, *first, num_dependents);
   }
 
   if(num_dependents == 0) {
-    _schedule_async_task(node.get());
+    _schedule_async_task(task._node);
   }
 
-  return AsyncTask(std::move(node));
+  return task;
 }
 
 // ----------------------------------------------------------------------------
 // Dependent Async
 // ----------------------------------------------------------------------------
 
 // Function: dependent_async
 template <typename F, typename... Tasks,
   std::enable_if_t<all_same_v<AsyncTask, std::decay_t<Tasks>...>, void>*
 >
 auto Executor::dependent_async(F&& func, Tasks&&... tasks) {
-  return dependent_async("", std::forward<F>(func), std::forward<Tasks>(tasks)...);
+  return dependent_async(DefaultTaskParams{}, std::forward<F>(func), std::forward<Tasks>(tasks)...);
 }
 
 // Function: dependent_async
-template <typename F, typename... Tasks,
-  std::enable_if_t<all_same_v<AsyncTask, std::decay_t<Tasks>...>, void>*
+template <typename P, typename F, typename... Tasks,
+  std::enable_if_t<is_task_params_v<P> && all_same_v<AsyncTask, std::decay_t<Tasks>...>, void>*
 >
-auto Executor::dependent_async(
-  const std::string& name, F&& func, Tasks&&... tasks 
-) {
+auto Executor::dependent_async(P&& params, F&& func, Tasks&&... tasks) {
   
   _increment_topology();
   
   using R = std::invoke_result_t<std::decay_t<F>>;
 
-  std::promise<R> p;
+  std::packaged_task<R()> p(std::forward<F>(func));
   auto fu{p.get_future()};
 
   size_t num_dependents = sizeof...(tasks);
 
-  std::shared_ptr<Node> node(
-    node_pool.animate(
-      name, 0, nullptr, nullptr, num_dependents,
-      std::in_place_type_t<Node::DependentAsync>{},
-      _make_promised_async(std::move(p), std::forward<F>(func))
-    ),
-    [&](Node* ptr){ node_pool.recycle(ptr); }
-  );
-  
-  {
-    std::scoped_lock lock(_asyncs_mutex);
-    _asyncs.insert(node);
-  }
+  AsyncTask task(node_pool.animate(
+    std::forward<P>(params), nullptr, nullptr, num_dependents,
+    std::in_place_type_t<Node::DependentAsync>{},
+    [p=make_moc(std::move(p))] () mutable { p.object(); }
+  ));
   
   if constexpr(sizeof...(Tasks) > 0) {
-    (_process_async_dependent(node.get(), tasks, num_dependents), ...);
+    (_process_async_dependent(task._node, tasks, num_dependents), ...);
   }
 
   if(num_dependents == 0) {
-    _schedule_async_task(node.get());
+    _schedule_async_task(task._node);
   }
 
-  return std::make_pair(AsyncTask(std::move(node)), std::move(fu));
+  return std::make_pair(std::move(task), std::move(fu));
 }
 
 // Function: dependent_async
 template <typename F, typename I,
   std::enable_if_t<!std::is_same_v<std::decay_t<I>, AsyncTask>, void>*
 >
 auto Executor::dependent_async(F&& func, I first, I last) {
-  return dependent_async("", std::forward<F>(func), first, last);
+  return dependent_async(DefaultTaskParams{}, std::forward<F>(func), first, last);
 }
 
 // Function: dependent_async
-template <typename F, typename I,
-  std::enable_if_t<!std::is_same_v<std::decay_t<I>, AsyncTask>, void>*
+template <typename P, typename F, typename I,
+  std::enable_if_t<is_task_params_v<P> && !std::is_same_v<std::decay_t<I>, AsyncTask>, void>*
 >
-auto Executor::dependent_async(
-  const std::string& name, F&& func, I first, I last
-) {
+auto Executor::dependent_async(P&& params, F&& func, I first, I last) {
   
   _increment_topology();
   
   using R = std::invoke_result_t<std::decay_t<F>>;
 
-  std::promise<R> p;
+  std::packaged_task<R()> p(std::forward<F>(func));
   auto fu{p.get_future()};
 
   size_t num_dependents = std::distance(first, last);
 
-  std::shared_ptr<Node> node(
-    node_pool.animate(
-      name, 0, nullptr, nullptr, num_dependents,
-      std::in_place_type_t<Node::DependentAsync>{},
-      _make_promised_async(std::move(p), std::forward<F>(func))
-    ),
-    [&](Node* ptr){ node_pool.recycle(ptr); }
-  );
-  
-  {
-    std::scoped_lock lock(_asyncs_mutex);
-    _asyncs.insert(node);
-  }
-  
+  AsyncTask task(node_pool.animate(
+    std::forward<P>(params), nullptr, nullptr, num_dependents,
+    std::in_place_type_t<Node::DependentAsync>{},
+    [p=make_moc(std::move(p))] () mutable { p.object(); }
+  ));
+
   for(; first != last; first++) {
-    _process_async_dependent(node.get(), *first, num_dependents);
+    _process_async_dependent(task._node, *first, num_dependents);
   }
 
   if(num_dependents == 0) {
-    _schedule_async_task(node.get());
+    _schedule_async_task(task._node);
   }
 
-  return std::make_pair(AsyncTask(std::move(node)), std::move(fu));
+  return std::make_pair(std::move(task), std::move(fu));
 }
 
 // ----------------------------------------------------------------------------
 // Dependent Async Helper Functions
 // ----------------------------------------------------------------------------
 
 // Procedure: _process_async_dependent
 inline void Executor::_process_async_dependent(
   Node* node, tf::AsyncTask& task, size_t& num_dependents
 ) {
 
-  std::shared_ptr<Node> dep;
-  {
-    std::scoped_lock lock(_asyncs_mutex);
-    if(auto itr = _asyncs.find(task._node); itr != _asyncs.end()){
-      dep = *itr;
-    }
-  }
+  auto& state = std::get_if<Node::DependentAsync>(&(task._node->_handle))->state;
+
+  add_successor:
+
+  auto target = Node::AsyncState::UNFINISHED;
   
-  // if the dependent task exists
-  if(dep) {
-    auto& state = std::get_if<Node::DependentAsync>(&(dep->_handle))->state;
-
-    add_dependent:
-
-    auto target = Node::AsyncState::UNFINISHED;
-    
-    // acquires the lock
-    if(state.compare_exchange_weak(target, Node::AsyncState::LOCKED,
-                                   std::memory_order_acq_rel,
-                                   std::memory_order_acquire)) {
-      dep->_successors.push_back(node);
-      state.store(Node::AsyncState::UNFINISHED, std::memory_order_release);
-    }
-    // dep's state is FINISHED, which means dep finished its callable already
-    // thus decrement the node's join counter by 1
-    else if (target == Node::AsyncState::FINISHED) {
-      // decrement the counter needs to be the order of acquire and release
-      // to synchronize with the worker
-      num_dependents = node->_join_counter.fetch_sub(1, std::memory_order_acq_rel) - 1;
-    }
-    // another worker adding an async task that shares the same dependent
-    else {
-      goto add_dependent;
-    }
+  // acquires the lock
+  if(state.compare_exchange_weak(target, Node::AsyncState::LOCKED,
+                                 std::memory_order_acq_rel,
+                                 std::memory_order_acquire)) {
+    task._node->_successors.push_back(node);
+    state.store(Node::AsyncState::UNFINISHED, std::memory_order_release);
+  }
+  // dep's state is FINISHED, which means dep finished its callable already
+  // thus decrement the node's join counter by 1
+  else if (target == Node::AsyncState::FINISHED) {
+    num_dependents = node->_join_counter.fetch_sub(1, std::memory_order_acq_rel) - 1;
   }
+  // another worker adding its async task to the same successors of this node
   else {
-    num_dependents = node->_join_counter.fetch_sub(1, std::memory_order_acq_rel) - 1;
+    goto add_successor;
   }
 }
 
+
 // Procedure: _tear_down_dependent_async
 inline void Executor::_tear_down_dependent_async(Worker& worker, Node* node) {
-  
+
+  auto handle = std::get_if<Node::DependentAsync>(&(node->_handle));
+
   // this async task comes from Executor
-  auto& state = std::get_if<Node::DependentAsync>(&(node->_handle))->state;
   auto target = Node::AsyncState::UNFINISHED;
 
-  while(!state.compare_exchange_weak(target, Node::AsyncState::FINISHED,
-                                     std::memory_order_acq_rel,
-                                     std::memory_order_relaxed)) {
+  while(!handle->state.compare_exchange_weak(target, Node::AsyncState::FINISHED,
+                                             std::memory_order_acq_rel,
+                                             std::memory_order_relaxed)) {
     target = Node::AsyncState::UNFINISHED;
   }
   
   // spaw successors whenever their dependencies are resolved
   worker._cache = nullptr;
   for(size_t i=0; i<node->_successors.size(); ++i) {
-    //if(auto s = node->_successors[i]; --(s->_join_counter) == 0) {
     if(auto s = node->_successors[i]; 
       s->_join_counter.fetch_sub(1, std::memory_order_acq_rel) == 1
     ) {
       if(worker._cache) {
         _schedule(worker, worker._cache);
       }
       worker._cache = s;
     }
   }
-    
-  // remove myself from the asyncs using extraction to avoid calling
-  // ~Node inside the lock
-  typename std::unordered_set<std::shared_ptr<Node>>::node_type extracted;
-  {
-    std::shared_ptr<Node> ptr(node, [](Node*){});
-    std::scoped_lock lock(_asyncs_mutex); 
-    extracted = _asyncs.extract(ptr);
-    // assert(extracted.empty() == false);
-  }
   
-  _decrement_topology_and_notify();
+  // now the executor no longer needs to retain ownership
+  if(handle->use_count.fetch_sub(1, std::memory_order_acq_rel) == 1) {
+    node_pool.recycle(node);
+  }
+
+  _decrement_topology();
 }
 
 
 
 
 
 }  // end of namespace tf -----------------------------------------------------
```

### Comparing `rapidfuzz-3.9.0/extern/taskflow/taskflow/core/declarations.hpp` & `rapidfuzz-3.9.1/extern/taskflow/taskflow/core/declarations.hpp`

 * *Files 5% similar despite different names*

```diff
@@ -48,13 +48,19 @@
 // syclFlow
 // ----------------------------------------------------------------------------
 class syclNode;
 class syclGraph;
 class syclTask;
 class syclFlow;
 
+// ----------------------------------------------------------------------------
+// struct 
+// ----------------------------------------------------------------------------
+struct TaskParams;
+struct DefaultTaskParams;
+
 
 }  // end of namespace tf -----------------------------------------------------
```

### Comparing `rapidfuzz-3.9.0/extern/taskflow/taskflow/core/error.hpp` & `rapidfuzz-3.9.1/extern/taskflow/taskflow/core/error.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/extern/taskflow/taskflow/core/executor-module-opt.hpp` & `rapidfuzz-3.9.1/extern/taskflow/taskflow/core/executor-module-opt.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/extern/taskflow/taskflow/core/executor.hpp` & `rapidfuzz-3.9.1/extern/taskflow/taskflow/core/executor.hpp`

 * *Files 4% similar despite different names*

```diff
@@ -55,31 +55,23 @@
   friend class Runtime;
 
   public:
 
   /**
   @brief constructs the executor with @c N worker threads
 
-
-  @param N number of workers (default std::thread::hardware_concurrency)
-  @param wix worker interface class to alter worker (thread) behaviors
+  @param N the number of workers (default std::thread::hardware_concurrency)
   
   The constructor spawns @c N worker threads to run tasks in a
   work-stealing loop. The number of workers must be greater than zero
   or an exception will be thrown.
   By default, the number of worker threads is equal to the maximum
   hardware concurrency returned by std::thread::hardware_concurrency.
-
-  Users can alter the worker behavior, such as changing thread affinity,
-  via deriving an instance from tf::WorkerInterface.
   */
-  explicit Executor(
-    size_t N = std::thread::hardware_concurrency(),
-    std::shared_ptr<WorkerInterface> wix = nullptr 
-  );
+  explicit Executor(size_t N = std::thread::hardware_concurrency());
 
   /**
   @brief destructs the executor
 
   The destructor calls Executor::wait_for_all to wait for all submitted
   taskflows to complete and then notifies all worker threads to stop
   and join these threads.
@@ -595,116 +587,119 @@
   @brief queries the number of observers
   */
   size_t num_observers() const noexcept;
 
   // --------------------------------------------------------------------------
   // Async Task Methods
   // --------------------------------------------------------------------------
-
+  
   /**
-  @brief runs a given function asynchronously
+  @brief creates a parameterized asynchronous task to run the given function
 
+  @tparam P task parameter type
   @tparam F callable type
 
+  @param params task parameters
   @param func callable object
 
   @return a @std_future that will hold the result of the execution
-
-  The method creates an asynchronous task to run the given function
-  and return a @std_future object that eventually will hold the result
-  of the return value.
+  
+  The method creates a parameterized asynchronous task 
+  to run the given function and return a @std_future object 
+  that eventually will hold the result of the execution.
 
   @code{.cpp}
-  std::future<int> future = executor.async([](){
-    std::cout << "create an asynchronous task and returns 1\n";
+  std::future<int> future = executor.async("name", [](){
+    std::cout << "create an asynchronous task with a name and returns 1\n";
     return 1;
   });
   future.get();
   @endcode
 
   This member function is thread-safe.
   */
-  template <typename F>
-  auto async(F&& func);
+  template <typename P, typename F>
+  auto async(P&& params, F&& func);
 
   /**
-  @brief runs a given function asynchronously and gives a name to this task
+  @brief runs a given function asynchronously
 
   @tparam F callable type
 
-  @param name name of the asynchronous task
   @param func callable object
 
   @return a @std_future that will hold the result of the execution
-  
-  The method creates and assigns a name to an asynchronous task 
-  to run the given function, 
-  returning @std_future object that eventually will hold the result
-  Assigned task names will appear in the observers of the executor.
+
+  The method creates an asynchronous task to run the given function
+  and return a @std_future object that eventually will hold the result
+  of the return value.
 
   @code{.cpp}
-  std::future<int> future = executor.async("name", [](){
-    std::cout << "create an asynchronous task with a name and returns 1\n";
+  std::future<int> future = executor.async([](){
+    std::cout << "create an asynchronous task and returns 1\n";
     return 1;
   });
   future.get();
   @endcode
 
   This member function is thread-safe.
   */
   template <typename F>
-  auto async(const std::string& name, F&& func);
+  auto async(F&& func);
 
   /**
   @brief similar to tf::Executor::async but does not return a future object
-  
+
   @tparam F callable type
-  
+
+  @param params task parameters
   @param func callable object
 
-  This member function is more efficient than tf::Executor::async
-  and is encouraged to use when you do not want a @std_future to
-  acquire the result or synchronize the execution.
+  The method creates a parameterized asynchronous task 
+  to run the given function without returning any @std_future object.
+  This member function is more efficient than tf::Executor::async 
+  and is encouraged to use when applications do not need a @std_future to acquire
+  the result or synchronize the execution.
 
   @code{.cpp}
-  executor.silent_async([](){
-    std::cout << "create an asynchronous task with no return\n";
+  executor.silent_async("name", [](){
+    std::cout << "create an asynchronous task with a name and no return\n";
   });
   executor.wait_for_all();
   @endcode
 
   This member function is thread-safe.
   */
-  template <typename F>
-  void silent_async(F&& func);
-
+  template <typename P, typename F>
+  void silent_async(P&& params, F&& func);
+  
   /**
   @brief similar to tf::Executor::async but does not return a future object
-
+  
   @tparam F callable type
-
-  @param name assigned name to the task
+  
   @param func callable object
 
-  This member function is more efficient than tf::Executor::async
-  and is encouraged to use when you do not want a @std_future to
-  acquire the result or synchronize the execution.
-  Assigned task names will appear in the observers of the executor.
+  The method creates an asynchronous task 
+  to run the given function without returning any @std_future object.
+  This member function is more efficient than tf::Executor::async 
+  and is encouraged to use when applications do not need a @std_future to acquire
+  the result or synchronize the execution.
 
   @code{.cpp}
-  executor.silent_async("name", [](){
-    std::cout << "create an asynchronous task with a name and no return\n";
+  executor.silent_async([](){
+    std::cout << "create an asynchronous task with no return\n";
   });
   executor.wait_for_all();
   @endcode
 
   This member function is thread-safe.
   */
   template <typename F>
-  void silent_async(const std::string& name, F&& func);
+  void silent_async(F&& func);
 
   // --------------------------------------------------------------------------
   // Silent Dependent Async Methods
   // --------------------------------------------------------------------------
   
   /**
   @brief runs the given function asynchronously 
@@ -735,21 +730,21 @@
   */
   template <typename F, typename... Tasks,
     std::enable_if_t<all_same_v<AsyncTask, std::decay_t<Tasks>...>, void>* = nullptr
   >
   tf::AsyncTask silent_dependent_async(F&& func, Tasks&&... tasks);
   
   /**
-  @brief names and runs the given function asynchronously 
+  @brief runs the given function asynchronously 
          when the given dependents finish
   
   @tparam F callable type
   @tparam Tasks task types convertible to tf::AsyncTask
 
-  @param name assigned name to the task
+  @param params task parameters
   @param func callable object
   @param tasks asynchronous tasks on which this execution depends
   
   @return a tf::AsyncTask handle 
   
   This member function is more efficient than tf::Executor::dependent_async
   and is encouraged to use when you do not want a @std_future to
@@ -765,18 +760,18 @@
     "C", [](){ printf("C runs after A and B\n"); }, A, B
   );
   executor.wait_for_all();
   @endcode
 
   This member function is thread-safe.
   */
-  template <typename F, typename... Tasks,
-    std::enable_if_t<all_same_v<AsyncTask, std::decay_t<Tasks>...>, void>* = nullptr
+  template <typename P, typename F, typename... Tasks,
+    std::enable_if_t<is_task_params_v<P> && all_same_v<AsyncTask, std::decay_t<Tasks>...>, void>* = nullptr
   >
-  tf::AsyncTask silent_dependent_async(const std::string& name, F&& func, Tasks&&... tasks);
+  tf::AsyncTask silent_dependent_async(P&& params, F&& func, Tasks&&... tasks);
   
   /**
   @brief runs the given function asynchronously 
          when the given range of dependents finish
   
   @tparam F callable type
   @tparam I iterator type 
@@ -808,21 +803,21 @@
   */
   template <typename F, typename I, 
     std::enable_if_t<!std::is_same_v<std::decay_t<I>, AsyncTask>, void>* = nullptr
   >
   tf::AsyncTask silent_dependent_async(F&& func, I first, I last);
   
   /**
-  @brief names and runs the given function asynchronously 
+  @brief runs the given function asynchronously 
          when the given range of dependents finish
   
   @tparam F callable type
   @tparam I iterator type 
 
-  @param name assigned name to the task
+  @param params tasks parameters
   @param func callable object
   @param first iterator to the beginning (inclusive)
   @param last iterator to the end (exclusive)
 
   @return a tf::AsyncTask handle 
   
   This member function is more efficient than tf::Executor::dependent_async
@@ -841,18 +836,18 @@
     "C", [](){ printf("C runs after A and B\n"); }, array.begin(), array.end()
   );
   executor.wait_for_all();
   @endcode
 
   This member function is thread-safe.
   */
-  template <typename F, typename I, 
-    std::enable_if_t<!std::is_same_v<std::decay_t<I>, AsyncTask>, void>* = nullptr
+  template <typename P, typename F, typename I, 
+    std::enable_if_t<is_task_params_v<P> && !std::is_same_v<std::decay_t<I>, AsyncTask>, void>* = nullptr
   >
-  tf::AsyncTask silent_dependent_async(const std::string& name, F&& func, I first, I last);
+  tf::AsyncTask silent_dependent_async(P&& params, F&& func, I first, I last);
   
   // --------------------------------------------------------------------------
   // Dependent Async Methods
   // --------------------------------------------------------------------------
   
   /**
   @brief runs the given function asynchronously 
@@ -893,21 +888,22 @@
   */
   template <typename F, typename... Tasks,
     std::enable_if_t<all_same_v<AsyncTask, std::decay_t<Tasks>...>, void>* = nullptr
   >
   auto dependent_async(F&& func, Tasks&&... tasks);
   
   /**
-  @brief names and runs the given function asynchronously
+  @brief runs the given function asynchronously
          when the given dependents finish
   
+  @tparam P task parameters type
   @tparam F callable type
   @tparam Tasks task types convertible to tf::AsyncTask
   
-  @param name assigned name to the task
+  @param params task parameters
   @param func callable object
   @param tasks asynchronous tasks on which this execution depends
   
   @return a pair of a tf::AsyncTask handle and 
                     a @std_future that holds the result of the execution
   
   The example below creates three named asynchronous tasks, @c A, @c B, and @c C,
@@ -932,18 +928,18 @@
 
   You can mixed the use of tf::AsyncTask handles 
   returned by Executor::dependent_async and Executor::silent_dependent_async
   when specifying task dependencies.
 
   This member function is thread-safe.
   */
-  template <typename F, typename... Tasks,
-    std::enable_if_t<all_same_v<AsyncTask, std::decay_t<Tasks>...>, void>* = nullptr
+  template <typename P, typename F, typename... Tasks,
+    std::enable_if_t<is_task_params_v<P> && all_same_v<AsyncTask, std::decay_t<Tasks>...>, void>* = nullptr
   >
-  auto dependent_async(const std::string& name, F&& func, Tasks&&... tasks);
+  auto dependent_async(P&& params, F&& func, Tasks&&... tasks);
   
   /**
   @brief runs the given function asynchronously 
          when the given range of dependents finish
   
   @tparam F callable type
   @tparam I iterator type 
@@ -983,21 +979,22 @@
   */
   template <typename F, typename I,
     std::enable_if_t<!std::is_same_v<std::decay_t<I>, AsyncTask>, void>* = nullptr
   >
   auto dependent_async(F&& func, I first, I last);
   
   /**
-  @brief names and runs the given function asynchronously 
+  @brief runs the given function asynchronously 
          when the given range of dependents finish
   
+  @tparam P task parameters type
   @tparam F callable type
   @tparam I iterator type 
   
-  @param name assigned name to the task
+  @param params task parameters
   @param func callable object
   @param first iterator to the beginning (inclusive)
   @param last iterator to the end (exclusive)
   
   @return a pair of a tf::AsyncTask handle and 
                     a @std_future that holds the result of the execution
   
@@ -1025,103 +1022,102 @@
 
   You can mixed the use of tf::AsyncTask handles 
   returned by Executor::dependent_async and Executor::silent_dependent_async
   when specifying task dependencies.
 
   This member function is thread-safe.
   */
-  template <typename F, typename I,
-    std::enable_if_t<!std::is_same_v<std::decay_t<I>, AsyncTask>, void>* = nullptr
+  template <typename P, typename F, typename I,
+    std::enable_if_t<is_task_params_v<P> && !std::is_same_v<std::decay_t<I>, AsyncTask>, void>* = nullptr
   >
-  auto dependent_async(const std::string& name, F&& func, I first, I last);
+  auto dependent_async(P&& params, F&& func, I first, I last);
 
   private:
     
   const size_t _MAX_STEALS;
+  
+  std::mutex _wsq_mutex;
+  std::mutex _taskflows_mutex;
 
+#ifdef __cpp_lib_atomic_wait
+  std::atomic<size_t> _num_topologies {0};
+  std::atomic_flag _all_spawned = ATOMIC_FLAG_INIT;
+#else
   std::condition_variable _topology_cv;
-  std::mutex _taskflows_mutex;
   std::mutex _topology_mutex;
-  std::mutex _wsq_mutex;
-  std::mutex _asyncs_mutex;
-
   size_t _num_topologies {0};
+#endif
   
   std::unordered_map<std::thread::id, size_t> _wids;
   std::vector<std::thread> _threads;
   std::vector<Worker> _workers;
   std::list<Taskflow> _taskflows;
 
-  std::unordered_set<std::shared_ptr<Node>> _asyncs;
-
   Notifier _notifier;
 
   TaskQueue<Node*> _wsq;
 
   std::atomic<bool> _done {0};
 
-  std::shared_ptr<WorkerInterface> _worker_interface;
   std::unordered_set<std::shared_ptr<ObserverInterface>> _observers;
 
   Worker* _this_worker();
-
+  
   bool _wait_for_task(Worker&, Node*&);
+  bool _invoke_module_task_internal(Worker&, Node*);
 
   void _observer_prologue(Worker&, Node*);
   void _observer_epilogue(Worker&, Node*);
   void _spawn(size_t);
   void _exploit_task(Worker&, Node*&);
   void _explore_task(Worker&, Node*&);
   void _schedule(Worker&, Node*);
   void _schedule(Node*);
   void _schedule(Worker&, const SmallVector<Node*>&);
   void _schedule(const SmallVector<Node*>&);
   void _set_up_topology(Worker*, Topology*);
+  void _set_up_graph(Graph&, Node*, Topology*, int, SmallVector<Node*>&);
   void _tear_down_topology(Worker&, Topology*);
   void _tear_down_async(Node*);
   void _tear_down_dependent_async(Worker&, Node*);
   void _tear_down_invoke(Worker&, Node*);
   void _increment_topology();
   void _decrement_topology();
-  void _decrement_topology_and_notify();
   void _invoke(Worker&, Node*);
   void _invoke_static_task(Worker&, Node*);
-  void _invoke_dynamic_task(Worker&, Node*);
-  void _consume_graph(Worker&, Node*, Graph&);
-  void _detach_dynamic_task(Worker&, Node*, Graph&);
+  void _invoke_subflow_task(Worker&, Node*);
+  void _detach_subflow_task(Worker&, Node*, Graph&);
   void _invoke_condition_task(Worker&, Node*, SmallVector<int>&);
   void _invoke_multi_condition_task(Worker&, Node*, SmallVector<int>&);
   void _invoke_module_task(Worker&, Node*);
   void _invoke_async_task(Worker&, Node*);
   void _invoke_dependent_async_task(Worker&, Node*);
   void _process_async_dependent(Node*, tf::AsyncTask&, size_t&);
+  void _process_exception(Worker&, Node*);
   void _schedule_async_task(Node*);
+  void _corun_graph(Worker&, Node*, Graph&);
   
   template <typename P>
   void _corun_until(Worker&, P&&);
-  
-  template <typename R, typename F>
-  auto _make_promised_async(std::promise<R>&&, F&&);
 };
 
 // Constructor
-inline Executor::Executor(size_t N, std::shared_ptr<WorkerInterface> wix) :
+inline Executor::Executor(size_t N) :
   _MAX_STEALS {((N+1) << 1)},
   _threads    {N},
   _workers    {N},
-  _notifier   {N},
-  _worker_interface {std::move(wix)} {
+  _notifier   {N} {
 
   if(N == 0) {
-    TF_THROW("no cpu workers to execute taskflows");
+    TF_THROW("executor must define at least one worker");
   }
 
   _spawn(N);
 
-  // instantite the default observer if requested
+  // initialize the default observer if requested
   if(has_env(TF_ENABLE_PROFILER)) {
     TFProfManager::get()._manage(make_observer<TFProfObserver>());
   }
 }
 
 // Destructor
 inline Executor::~Executor() {
@@ -1142,15 +1138,19 @@
 // Function: num_workers
 inline size_t Executor::num_workers() const noexcept {
   return _workers.size();
 }
 
 // Function: num_topologies
 inline size_t Executor::num_topologies() const {
+#ifdef __cpp_lib_atomic_wait
+  return _num_topologies.load(std::memory_order_relaxed);
+#else
   return _num_topologies;
+#endif
 }
 
 // Function: num_taskflows
 inline size_t Executor::num_taskflows() const {
   return _taskflows.size();
 }
 
@@ -1165,87 +1165,84 @@
   auto i = _wids.find(std::this_thread::get_id());
   return i == _wids.end() ? -1 : static_cast<int>(_workers[i->second]._id);
 }
 
 // Procedure: _spawn
 inline void Executor::_spawn(size_t N) {
 
+#ifdef __cpp_lib_atomic_wait
+#else
   std::mutex mutex;
   std::condition_variable cond;
   size_t n=0;
+#endif
 
   for(size_t id=0; id<N; ++id) {
 
     _workers[id]._id = id;
     _workers[id]._vtm = id;
     _workers[id]._executor = this;
     _workers[id]._waiter = &_notifier._waiters[id];
 
-    _threads[id] = std::thread([this] (
-      Worker& w, std::mutex& mutex, std::condition_variable& cond, size_t& n
-    ) -> void {
-      
-      // assign the thread
-      w._thread = &_threads[w._id];
+    _threads[id] = std::thread([&, &w=_workers[id]] () {
 
-      // enables the mapping
+#ifdef __cpp_lib_atomic_wait
+      // wait for the caller thread to initialize the ID mapping
+      _all_spawned.wait(false, std::memory_order_acquire);
+      w._thread = &_threads[w._id];
+#else
+      // update the ID mapping of this thread
+      w._thread = &_threads[w._id];
       {
         std::scoped_lock lock(mutex);
         _wids[std::this_thread::get_id()] = w._id;
         if(n++; n == num_workers()) {
           cond.notify_one();
         }
       }
+#endif
 
       Node* t = nullptr;
       
-      // before entering the scheduler (work-stealing loop), 
-      // call the user-specified prologue function
-      if(_worker_interface) {
-        _worker_interface->scheduler_prologue(w);
-      }
-      
-      // must use 1 as condition instead of !done because
-      // the previous worker may stop while the following workers
-      // are still preparing for entering the scheduling loop
-      std::exception_ptr ptr{nullptr};
-      try {
-        while(1) {
-
-          // execute the tasks.
-          _exploit_task(w, t);
-
-          // wait for tasks
-          if(_wait_for_task(w, t) == false) {
-            break;
-          }
+      while(1) {
+
+        // execute the tasks.
+        _exploit_task(w, t);
+
+        // wait for tasks
+        if(_wait_for_task(w, t) == false) {
+          break;
         }
-      } 
-      catch(...) {
-        ptr = std::current_exception();
-      }
-      
-      // call the user-specified epilogue function
-      if(_worker_interface) {
-        _worker_interface->scheduler_epilogue(w, ptr);
       }
 
-    }, std::ref(_workers[id]), std::ref(mutex), std::ref(cond), std::ref(n));
+    });
     
     // POSIX-like system can use the following to affine threads to cores 
     //cpu_set_t cpuset;
     //CPU_ZERO(&cpuset);
     //CPU_SET(id, &cpuset);
     //pthread_setaffinity_np(
     //  _threads[id].native_handle(), sizeof(cpu_set_t), &cpuset
     //);
-  }
 
+#ifdef __cpp_lib_atomic_wait
+    //_wids[_threads[id].get_id()] = id;
+    _wids.emplace(std::piecewise_construct,
+      std::forward_as_tuple(_threads[id].get_id()), std::forward_as_tuple(id)
+    );
+#endif
+  }
+  
+#ifdef __cpp_lib_atomic_wait
+  _all_spawned.test_and_set(std::memory_order_release);
+  _all_spawned.notify_all();
+#else
   std::unique_lock<std::mutex> lock(mutex);
   cond.wait(lock, [&](){ return n==N; });
+#endif
 }
 
 // Function: _corun_until
 template <typename P>
 void Executor::_corun_until(Worker& w, P&& stop_predicate) {
   
   std::uniform_int_distribution<size_t> rdvtm(0, _workers.size()-1);
@@ -1517,14 +1514,16 @@
 // Procedure: _invoke
 inline void Executor::_invoke(Worker& worker, Node* node) {
 
   // synchronize all outstanding memory operations caused by reordering
   while(!(node->_state.load(std::memory_order_acquire) & Node::READY));
 
   begin_invoke:
+  
+  SmallVector<int> conds;
 
   // no need to do other things if the topology is cancelled
   if(node->_is_cancelled()) {
     _tear_down_invoke(worker, node);
     return;
   }
 
@@ -1536,27 +1535,26 @@
       return;
     }
     node->_state.fetch_or(Node::ACQUIRED, std::memory_order_release);
   }
 
   // condition task
   //int cond = -1;
-  SmallVector<int> conds;
 
   // switch is faster than nested if-else due to jump table
   switch(node->_handle.index()) {
     // static task
     case Node::STATIC:{
       _invoke_static_task(worker, node);
     }
     break;
 
-    // dynamic task
-    case Node::DYNAMIC: {
-      _invoke_dynamic_task(worker, node);
+    // subflow task
+    case Node::SUBFLOW: {
+      _invoke_subflow_task(worker, node);
     }
     break;
 
     // condition task
     case Node::CONDITION: {
       _invoke_condition_task(worker, node, conds);
     }
@@ -1595,14 +1593,16 @@
     break;
 
     // monostate (placeholder)
     default:
     break;
   }
 
+  //invoke_successors:
+
   // if releasing semaphores exist, release them
   if(node->_semaphores && !node->_semaphores->to_release.empty()) {
     _schedule(worker, node->_release_all());
   }
   
   // Reset the join counter to support the cyclic control flow.
   // + We must do this before scheduling the successors to avoid race
@@ -1683,27 +1683,39 @@
   if(worker._cache) {
     node = worker._cache;
     //node->_state.fetch_or(Node::READY, std::memory_order_release);
     goto begin_invoke;
   }
 }
 
-// Proecdure: _tear_down_invoke
+// Procedure: _tear_down_invoke
 inline void Executor::_tear_down_invoke(Worker& worker, Node* node) {
-  // we must check parent first before substracting the join counter,
+  // we must check parent first before subtracting the join counter,
   // or it can introduce data race
-  if(node->_parent == nullptr) {
+  if(auto parent = node->_parent; parent == nullptr) {
     if(node->_topology->_join_counter.fetch_sub(1, std::memory_order_acq_rel) == 1) {
       _tear_down_topology(worker, node->_topology);
     }
   }
-  // joined subflow
-  else {  
-    node->_parent->_join_counter.fetch_sub(1, std::memory_order_release);
+  // Here we asssume the parent is in a busy loop (e.g., corun) waiting for
+  // its join counter to become 0.
+  else {
+    //parent->_join_counter.fetch_sub(1, std::memory_order_acq_rel);
+    parent->_join_counter.fetch_sub(1, std::memory_order_release);
   }
+  //// module task
+  //else {  
+  //  auto id = parent->_handle.index();
+  //  if(parent->_join_counter.fetch_sub(1, std::memory_order_acq_rel) == 1) {
+  //    if(id == Node::MODULE) {
+  //      return parent;
+  //    }
+  //  }
+  //}
+  //return nullptr;
 }
 
 // Procedure: _observer_prologue
 inline void Executor::_observer_prologue(Worker& worker, Node* node) {
   for(auto& observer : _observers) {
     observer->on_entry(WorkerView(worker), TaskView(*node));
   }
@@ -1712,168 +1724,225 @@
 // Procedure: _observer_epilogue
 inline void Executor::_observer_epilogue(Worker& worker, Node* node) {
   for(auto& observer : _observers) {
     observer->on_exit(WorkerView(worker), TaskView(*node));
   }
 }
 
+// Procedure: _process_exception
+inline void Executor::_process_exception(Worker&, Node* node) {
+
+  constexpr static auto flag = Topology::EXCEPTION | Topology::CANCELLED;
+  
+  // if the node has a parent, we store the exception in its parent
+  if(auto parent = node->_parent; parent) { 
+    if ((parent->_state.fetch_or(Node::EXCEPTION, std::memory_order_relaxed) & Node::EXCEPTION) == 0) {
+      parent->_exception_ptr = std::current_exception();
+    }
+    // TODO if the node has a topology, cancel it to enable early stop
+    //if(auto tpg = node->_topology; tpg) {
+    //  tpg->_state.fetch_or(Topology::CANCELLED, std::memory_order_relaxed);
+    //}
+  }
+  // multiple tasks may throw, so we only take the first thrown exception
+  else if(auto tpg = node->_topology; tpg && 
+    ((tpg->_state.fetch_or(flag, std::memory_order_relaxed) & Topology::EXCEPTION) == 0)
+  ) {
+    tpg->_exception_ptr = std::current_exception();
+  }
+  // TODO: skip the exception that is not associated with any taskflows
+}
+
 // Procedure: _invoke_static_task
 inline void Executor::_invoke_static_task(Worker& worker, Node* node) {
   _observer_prologue(worker, node);
-  auto& work = std::get_if<Node::Static>(&node->_handle)->work;
-  switch(work.index()) {
-    case 0:
-      std::get_if<0>(&work)->operator()();
-    break;
+  TF_EXECUTOR_EXCEPTION_HANDLER(worker, node, {
+    auto& work = std::get_if<Node::Static>(&node->_handle)->work;
+    switch(work.index()) {
+      case 0:
+        std::get_if<0>(&work)->operator()();
+      break;
 
-    case 1:
-      Runtime rt(*this, worker, node);
-      std::get_if<1>(&work)->operator()(rt);
-    break;
-  }
+      case 1:
+        Runtime rt(*this, worker, node);
+        std::get_if<1>(&work)->operator()(rt);
+        node->_process_exception();
+      break;
+    }
+  });
   _observer_epilogue(worker, node);
 }
 
-// Procedure: _invoke_dynamic_task
-inline void Executor::_invoke_dynamic_task(Worker& w, Node* node) {
-
+// Procedure: _invoke_subflow_task
+inline void Executor::_invoke_subflow_task(Worker& w, Node* node) {
   _observer_prologue(w, node);
-
-  auto handle = std::get_if<Node::Dynamic>(&node->_handle);
-
-  handle->subgraph._clear();
-
-  Subflow sf(*this, w, node, handle->subgraph);
-
-  handle->work(sf);
-
-  if(sf._joinable) {
-    _consume_graph(w, node, handle->subgraph);
-  }
-
+  TF_EXECUTOR_EXCEPTION_HANDLER(w, node, {
+    auto handle = std::get_if<Node::Subflow>(&node->_handle);
+    handle->subgraph._clear();
+    Subflow sf(*this, w, node, handle->subgraph);
+    handle->work(sf);
+    if(sf._joinable) {
+      _corun_graph(w, node, handle->subgraph);
+    }
+    node->_process_exception();
+  });
   _observer_epilogue(w, node);
 }
 
-// Procedure: _detach_dynamic_task
-inline void Executor::_detach_dynamic_task(
-  Worker& w, Node* p, Graph& g
-) {
+// Procedure: _detach_subflow_task
+inline void Executor::_detach_subflow_task(Worker& w, Node* p, Graph& g) {
 
   // graph is empty and has no async tasks
   if(g.empty() && p->_join_counter.load(std::memory_order_acquire) == 0) {
     return;
   }
 
   SmallVector<Node*> src;
-
-  for(auto n : g._nodes) {
-
-    n->_state.store(Node::DETACHED, std::memory_order_relaxed);
-    n->_set_up_join_counter();
-    n->_topology = p->_topology;
-    n->_parent = nullptr;
-
-    if(n->num_dependents() == 0) {
-      src.push_back(n);
-    }
-  }
+  _set_up_graph(g, nullptr, p->_topology, Node::DETACHED, src);
 
   {
     std::lock_guard<std::mutex> lock(p->_topology->_taskflow._mutex);
     p->_topology->_taskflow._graph._merge(std::move(g));
   }
 
   p->_topology->_join_counter.fetch_add(src.size(), std::memory_order_relaxed);
   _schedule(w, src);
 }
 
-// Procedure: _consume_graph
-inline void Executor::_consume_graph(Worker& w, Node* p, Graph& g) {
+// Procedure: _corun_graph
+inline void Executor::_corun_graph(Worker& w, Node* p, Graph& g) {
 
-  // graph is empty and has no async tasks
+  // assert(p);
+
+  // graph is empty and has no async tasks (subflow)
   if(g.empty() && p->_join_counter.load(std::memory_order_acquire) == 0) {
     return;
   }
 
   SmallVector<Node*> src;
 
-  for(auto n : g._nodes) {
-    n->_state.store(0, std::memory_order_relaxed);
-    n->_set_up_join_counter();
-    n->_topology = p->_topology;
-    n->_parent = p;
-    if(n->num_dependents() == 0) {
-      src.push_back(n);
-    }
-  }
+  _set_up_graph(g, p, p->_topology, 0, src);
   p->_join_counter.fetch_add(src.size(), std::memory_order_relaxed);
   
   _schedule(w, src);
-  _corun_until(w, [p] () -> bool { return p->_join_counter.load(std::memory_order_acquire) == 0; });
+
+  _corun_until(w, [p] () -> bool { 
+    return p->_join_counter.load(std::memory_order_acquire) == 0; }
+  );
 }
 
 // Procedure: _invoke_condition_task
 inline void Executor::_invoke_condition_task(
   Worker& worker, Node* node, SmallVector<int>& conds
 ) {
   _observer_prologue(worker, node);
-  auto& work = std::get_if<Node::Condition>(&node->_handle)->work;
-  switch(work.index()) {
-    case 0:
-      conds = { std::get_if<0>(&work)->operator()() };
-    break;
+  TF_EXECUTOR_EXCEPTION_HANDLER(worker, node, {
+    auto& work = std::get_if<Node::Condition>(&node->_handle)->work;
+    switch(work.index()) {
+      case 0:
+        conds = { std::get_if<0>(&work)->operator()() };
+      break;
 
-    case 1:
-      Runtime rt(*this, worker, node);
-      conds = { std::get_if<1>(&work)->operator()(rt) };
-    break;
-  }
+      case 1:
+        Runtime rt(*this, worker, node);
+        conds = { std::get_if<1>(&work)->operator()(rt) };
+        node->_process_exception();
+      break;
+    }
+  });
   _observer_epilogue(worker, node);
 }
 
 // Procedure: _invoke_multi_condition_task
 inline void Executor::_invoke_multi_condition_task(
   Worker& worker, Node* node, SmallVector<int>& conds
 ) {
   _observer_prologue(worker, node);
-  auto& work = std::get_if<Node::MultiCondition>(&node->_handle)->work;
-  switch(work.index()) {
-    case 0:
-      conds = std::get_if<0>(&work)->operator()();
-    break;
+  TF_EXECUTOR_EXCEPTION_HANDLER(worker, node, {
+    auto& work = std::get_if<Node::MultiCondition>(&node->_handle)->work;
+    switch(work.index()) {
+      case 0:
+        conds = std::get_if<0>(&work)->operator()();
+      break;
 
-    case 1:
-      Runtime rt(*this, worker, node);
-      conds = std::get_if<1>(&work)->operator()(rt);
-    break;
-  }
+      case 1:
+        Runtime rt(*this, worker, node);
+        conds = std::get_if<1>(&work)->operator()(rt);
+        node->_process_exception();
+      break;
+    }
+  });
   _observer_epilogue(worker, node);
 }
 
 // Procedure: _invoke_module_task
 inline void Executor::_invoke_module_task(Worker& w, Node* node) {
   _observer_prologue(w, node);
-  _consume_graph(
-    w, node, std::get_if<Node::Module>(&node->_handle)->graph
-  );
+  TF_EXECUTOR_EXCEPTION_HANDLER(w, node, {
+    _corun_graph(w, node, std::get_if<Node::Module>(&node->_handle)->graph);
+    node->_process_exception();
+  });
   _observer_epilogue(w, node);
 }
 
+//// Function: _invoke_module_task_internal
+//inline bool Executor::_invoke_module_task_internal(Worker& w, Node* p) {
+//  
+//  // acquire the underlying graph
+//  auto& g = std::get_if<Node::Module>(&p->_handle)->graph;
+//
+//  // no need to do anything if the graph is empty
+//  if(g.empty()) {
+//    return false;
+//  }
+//
+//  SmallVector<Node*> src;
+//  _set_up_graph(g, p, p->_topology, 0, src);
+//  p->_join_counter.fetch_add(src.size(), std::memory_order_relaxed);
+//
+//  _schedule(w, src);
+//  return true;
+//}
+
 // Procedure: _invoke_async_task
-inline void Executor::_invoke_async_task(Worker& w, Node* node) {
-  _observer_prologue(w, node);
-  std::get_if<Node::Async>(&node->_handle)->work();
-  _observer_epilogue(w, node);
+inline void Executor::_invoke_async_task(Worker& worker, Node* node) {
+  _observer_prologue(worker, node);
+  TF_EXECUTOR_EXCEPTION_HANDLER(worker, node, {
+    auto& work = std::get_if<Node::Async>(&node->_handle)->work;
+    switch(work.index()) {
+      case 0:
+        std::get_if<0>(&work)->operator()();
+      break;
+
+      case 1:
+        Runtime rt(*this, worker, node);
+        std::get_if<1>(&work)->operator()(rt);
+      break;
+    }
+  });
+  _observer_epilogue(worker, node);
 }
 
 // Procedure: _invoke_dependent_async_task
-inline void Executor::_invoke_dependent_async_task(Worker& w, Node* node) {
-  _observer_prologue(w, node);
-  std::get_if<Node::DependentAsync>(&node->_handle)->work();
-  _observer_epilogue(w, node);
+inline void Executor::_invoke_dependent_async_task(Worker& worker, Node* node) {
+  _observer_prologue(worker, node);
+  TF_EXECUTOR_EXCEPTION_HANDLER(worker, node, {
+    auto& work = std::get_if<Node::DependentAsync>(&node->_handle)->work;
+    switch(work.index()) {
+      case 0:
+        std::get_if<0>(&work)->operator()();
+      break;
+
+      case 1:
+        Runtime rt(*this, worker, node);
+        std::get_if<1>(&work)->operator()(rt);
+      break;
+    }
+  });
+  _observer_epilogue(worker, node);
 }
 
 // Function: run
 inline tf::Future<void> Executor::run(Taskflow& f) {
   return run_n(f, 1, [](){});
 }
 
@@ -1934,29 +2003,29 @@
 
 // Function: run_until
 template <typename P, typename C>
 tf::Future<void> Executor::run_until(Taskflow& f, P&& p, C&& c) {
 
   _increment_topology();
 
-  // Need to check the empty under the lock since dynamic task may
+  // Need to check the empty under the lock since subflow task may
   // define detached blocks that modify the taskflow at the same time
   bool empty;
   {
     std::lock_guard<std::mutex> lock(f._mutex);
     empty = f.empty();
   }
 
   // No need to create a real topology but returns an dummy future
   if(empty || p()) {
     c();
     std::promise<void> promise;
     promise.set_value();
-    _decrement_topology_and_notify();
-    return tf::Future<void>(promise.get_future(), std::monostate{});
+    _decrement_topology();
+    return tf::Future<void>(promise.get_future());
   }
 
   // create a topology for this run
   auto t = std::make_shared<Topology>(f, std::forward<P>(p), std::forward<C>(c));
 
   // need to create future before the topology got torn down quickly
   tf::Future<void> future(t->_promise.get_future(), t);
@@ -1994,98 +2063,115 @@
   
   auto w = _this_worker();
 
   if(w == nullptr) {
     TF_THROW("corun must be called by a worker of the executor");
   }
 
-  Node parent;  // dummy parent
-  _consume_graph(*w, &parent, target.graph());
+  Node parent;  // auxiliary parent
+  _corun_graph(*w, &parent, target.graph());
+  parent._process_exception();
 }
 
 // Function: corun_until
 template <typename P>
 void Executor::corun_until(P&& predicate) {
   
   auto w = _this_worker();
 
   if(w == nullptr) {
     TF_THROW("corun_until must be called by a worker of the executor");
   }
 
   _corun_until(*w, std::forward<P>(predicate));
+
+  // TODO: exception?
 }
 
 // Procedure: _increment_topology
 inline void Executor::_increment_topology() {
+#ifdef __cpp_lib_atomic_wait
+  _num_topologies.fetch_add(1, std::memory_order_relaxed);
+#else
   std::lock_guard<std::mutex> lock(_topology_mutex);
   ++_num_topologies;
+#endif
 }
 
-// Procedure: _decrement_topology_and_notify
-inline void Executor::_decrement_topology_and_notify() {
+// Procedure: _decrement_topology
+inline void Executor::_decrement_topology() {
+#ifdef __cpp_lib_atomic_wait
+  if(_num_topologies.fetch_sub(1, std::memory_order_acq_rel) == 1) {
+    _num_topologies.notify_all();
+  }
+#else
   std::lock_guard<std::mutex> lock(_topology_mutex);
   if(--_num_topologies == 0) {
     _topology_cv.notify_all();
   }
-}
-
-// Procedure: _decrement_topology
-inline void Executor::_decrement_topology() {
-  std::lock_guard<std::mutex> lock(_topology_mutex);
-  --_num_topologies;
+#endif
 }
 
 // Procedure: wait_for_all
 inline void Executor::wait_for_all() {
+#ifdef __cpp_lib_atomic_wait
+  size_t n = _num_topologies.load(std::memory_order_acquire);
+  while(n != 0) {
+    _num_topologies.wait(n, std::memory_order_acquire);
+    n = _num_topologies.load(std::memory_order_acquire);
+  }
+#else
   std::unique_lock<std::mutex> lock(_topology_mutex);
   _topology_cv.wait(lock, [&](){ return _num_topologies == 0; });
+#endif
 }
 
 // Function: _set_up_topology
 inline void Executor::_set_up_topology(Worker* worker, Topology* tpg) {
 
   // ---- under taskflow lock ----
 
   tpg->_sources.clear();
   tpg->_taskflow._graph._clear_detached();
-
-  // scan each node in the graph and build up the links
-  for(auto node : tpg->_taskflow._graph._nodes) {
-
-    node->_topology = tpg;
-    node->_parent = nullptr;
-    node->_state.store(0, std::memory_order_relaxed);
-
-    if(node->num_dependents() == 0) {
-      tpg->_sources.push_back(node);
-    }
-
-    node->_set_up_join_counter();
-  }
-
+  _set_up_graph(tpg->_taskflow._graph, nullptr, tpg, 0, tpg->_sources);
   tpg->_join_counter.store(tpg->_sources.size(), std::memory_order_relaxed);
 
   if(worker) {
     _schedule(*worker, tpg->_sources);
   }
   else {
     _schedule(tpg->_sources);
   }
 }
 
+// Function: _set_up_graph
+inline void Executor::_set_up_graph(
+  Graph& g, Node* parent, Topology* tpg, int state, SmallVector<Node*>& src
+) {
+  for(auto node : g._nodes) {
+    node->_topology = tpg;
+    node->_parent = parent;
+    node->_state.store(state, std::memory_order_relaxed);
+    if(node->num_dependents() == 0) {
+      src.push_back(node);
+    }
+    node->_set_up_join_counter();
+    node->_exception_ptr = nullptr;
+  }
+}
+
 // Function: _tear_down_topology
 inline void Executor::_tear_down_topology(Worker& worker, Topology* tpg) {
 
   auto &f = tpg->_taskflow;
 
   //assert(&tpg == &(f._topologies.front()));
 
   // case 1: we still need to run the topology again
-  if(!tpg->_is_cancelled && !tpg->_pred()) {
+  if(!tpg->_exception_ptr && !tpg->cancelled() && !tpg->_pred()) {
     //assert(tpg->_join_counter == 0);
     std::lock_guard<std::mutex> lock(f._mutex);
     tpg->_join_counter.store(tpg->_sources.size(), std::memory_order_relaxed);
     _schedule(worker, tpg->_sources);
   }
   // case 2: the final run of this topology
   else {
@@ -2110,44 +2196,32 @@
       // set up topology needs to be under the lock or it can
       // introduce memory order error with pop
       _set_up_topology(&worker, tpg);
     }
     else {
       //assert(f._topologies.size() == 1);
 
-      // Need to back up the promise first here becuz taskflow might be
-      // destroy soon after calling get
-      auto p {std::move(tpg->_promise)};
-
-      // Back up lambda capture in case it has the topology pointer,
-      // to avoid it releasing on pop_front ahead of _mutex.unlock &
-      // _promise.set_value. Released safely when leaving scope.
-      auto c {std::move(tpg->_call)};
-
-      // Get the satellite if any
-      auto s {f._satellite};
-
-      // Now we remove the topology from this taskflow
+      auto fetched_tpg {std::move(f._topologies.front())};
       f._topologies.pop();
+      auto satellite {f._satellite};
 
-      //f._mutex.unlock();
       lock.unlock();
+      
+      // Soon after we carry out the promise, there is no longer any guarantee
+      // for the lifetime of the associated taskflow.
+      fetched_tpg->_carry_out_promise();
 
-      // We set the promise in the end in case taskflow leaves the scope.
-      // After set_value, the caller will return from wait
-      p.set_value();
-
-      _decrement_topology_and_notify();
+      _decrement_topology();
 
       // remove the taskflow if it is managed by the executor
       // TODO: in the future, we may need to synchronize on wait
       // (which means the following code should the moved before set_value)
-      if(s) {
-        std::scoped_lock<std::mutex> lock(_taskflows_mutex);
-        _taskflows.erase(*s);
+      if(satellite) {
+        std::scoped_lock<std::mutex> satellite_lock(_taskflows_mutex);
+        _taskflows.erase(*satellite);
       }
     }
   }
 }
 
 // ############################################################################
 // Forward Declaration: Subflow
@@ -2158,28 +2232,32 @@
   // assert(this_worker().worker == &_worker);
 
   if(!_joinable) {
     TF_THROW("subflow not joinable");
   }
 
   // only the parent worker can join the subflow
-  _executor._consume_graph(_worker, _parent, _graph);
+  _executor._corun_graph(_worker, _parent, _graph);
+
+  // if any exception is caught from subflow tasks, rethrow it
+  _parent->_process_exception();
+
   _joinable = false;
 }
 
 inline void Subflow::detach() {
 
   // assert(this_worker().worker == &_worker);
 
   if(!_joinable) {
     TF_THROW("subflow already joined or detached");
   }
 
   // only the parent worker can detach the subflow
-  _executor._detach_dynamic_task(_worker, _parent, _graph);
+  _executor._detach_subflow_task(_worker, _parent, _graph);
   _joinable = false;
 }
 
 // ############################################################################
 // Forward Declaration: Runtime
 // ############################################################################
 
@@ -2197,116 +2275,121 @@
   j.fetch_add(1, std::memory_order_relaxed);
   _executor._schedule(_worker, node);
 }
 
 // Procedure: corun
 template <typename T>
 void Runtime::corun(T&& target) {
-
-  // dynamic task (subflow)
-  if constexpr(is_dynamic_task_v<T>) {
-    Graph graph;
-    Subflow sf(_executor, _worker, _parent, graph);
-    target(sf);
-    if(sf._joinable) {
-      _executor._consume_graph(_worker, _parent, graph);
-    }
-  }
-  // a composable graph object with `tf::Graph& T::graph()` defined
-  else {
-    _executor._consume_graph(_worker, _parent, target.graph());
-  }
+  _executor._corun_graph(_worker, _parent, target.graph());
+  _parent->_process_exception();
 }
 
 // Procedure: corun_until
 template <typename P>
 void Runtime::corun_until(P&& predicate) {
   _executor._corun_until(_worker, std::forward<P>(predicate));
+  // TODO: exception?
+}
+
+// Function: corun_all
+inline void Runtime::corun_all() {
+  _executor._corun_until(_worker, [this] () -> bool { 
+    return _parent->_join_counter.load(std::memory_order_acquire) == 0; 
+  });
+  _parent->_process_exception();
 }
 
+// Destructor
+inline Runtime::~Runtime() {
+  _executor._corun_until(_worker, [this] () -> bool { 
+    return _parent->_join_counter.load(std::memory_order_acquire) == 0; 
+  });
+}
+
+// ------------------------------------
+// Runtime::silent_async series
+// ------------------------------------
+
 // Function: _silent_async
-template <typename F>
-void Runtime::_silent_async(Worker& w, const std::string& name, F&& f) {
+template <typename P, typename F>
+void Runtime::_silent_async(Worker& w, P&& params, F&& f) {
 
   _parent->_join_counter.fetch_add(1, std::memory_order_relaxed);
 
   auto node = node_pool.animate(
-    name, 0, _parent->_topology, _parent, 0,
+    std::forward<P>(params), _parent->_topology, _parent, 0,
     std::in_place_type_t<Node::Async>{}, std::forward<F>(f)
   );
 
   _executor._schedule(w, node);
 }
 
 // Function: silent_async
 template <typename F>
 void Runtime::silent_async(F&& f) {
-  _silent_async(*_executor._this_worker(), "", std::forward<F>(f));
+  _silent_async(*_executor._this_worker(), DefaultTaskParams{}, std::forward<F>(f));
 }
 
 // Function: silent_async
-template <typename F>
-void Runtime::silent_async(const std::string& name, F&& f) {
-  _silent_async(*_executor._this_worker(), name, std::forward<F>(f));
+template <typename P, typename F>
+void Runtime::silent_async(P&& params, F&& f) {
+  _silent_async(*_executor._this_worker(), std::forward<P>(params), std::forward<F>(f));
 }
 
 // Function: silent_async_unchecked
 template <typename F>
-void Runtime::silent_async_unchecked(const std::string& name, F&& f) {
-  _silent_async(_worker, name, std::forward<F>(f));
+void Runtime::silent_async_unchecked(F&& f) {
+  _silent_async(_worker, DefaultTaskParams{}, std::forward<F>(f));
 }
 
+// Function: silent_async_unchecked
+template <typename P, typename F>
+void Runtime::silent_async_unchecked(P&& params, F&& f) {
+  _silent_async(_worker, std::forward<P>(params), std::forward<F>(f));
+}
+
+// ------------------------------------
+// Runtime::async series
+// ------------------------------------
+
 // Function: _async
-template <typename F>
-auto Runtime::_async(Worker& w, const std::string& name, F&& f) {
+template <typename P, typename F>
+auto Runtime::_async(Worker& w, P&& params, F&& f) {
 
   _parent->_join_counter.fetch_add(1, std::memory_order_relaxed);
 
   using R = std::invoke_result_t<std::decay_t<F>>;
 
-  std::promise<R> p;
+  std::packaged_task<R()> p(std::forward<F>(f));
   auto fu{p.get_future()};
 
   auto node = node_pool.animate(
-    name, 0, _parent->_topology, _parent, 0,
+    std::forward<P>(params), _parent->_topology, _parent, 0, 
     std::in_place_type_t<Node::Async>{},
-    [p=make_moc(std::move(p)), f=std::forward<F>(f)] () mutable {
-      if constexpr(std::is_same_v<R, void>) {
-        f();
-        p.object.set_value();
-      }
-      else {
-        p.object.set_value(f());
-      }
-    }
+    [p=make_moc(std::move(p))] () mutable { p.object(); }
   );
 
   _executor._schedule(w, node);
 
   return fu;
 }
 
 // Function: async
 template <typename F>
 auto Runtime::async(F&& f) {
-  return _async(*_executor._this_worker(), "", std::forward<F>(f));
+  return _async(*_executor._this_worker(), DefaultTaskParams{}, std::forward<F>(f));
 }
 
 // Function: async
-template <typename F>
-auto Runtime::async(const std::string& name, F&& f) {
-  return _async(*_executor._this_worker(), name, std::forward<F>(f));
+template <typename P, typename F>
+auto Runtime::async(P&& params, F&& f) {
+  return _async(*_executor._this_worker(), std::forward<P>(params), std::forward<F>(f));
 }
 
-// Function: join
-inline void Runtime::join() {
-  corun_until([this] () -> bool { 
-    return _parent->_join_counter.load(std::memory_order_acquire) == 0; 
-  });
-}
+
 
 }  // end of namespace tf -----------------------------------------------------
```

### Comparing `rapidfuzz-3.9.0/extern/taskflow/taskflow/core/flow_builder.hpp` & `rapidfuzz-3.9.1/extern/taskflow/taskflow/core/flow_builder.hpp`

 * *Files 3% similar despite different names*

```diff
@@ -67,18 +67,18 @@
   @code{.cpp}
   tf::Task dynamic_task = taskflow.emplace([](tf::Subflow& sf){
     tf::Task static_task1 = sf.emplace([](){});
     tf::Task static_task2 = sf.emplace([](){});
   });
   @endcode
 
-  Please refer to @ref DynamicTasking for details.
+  Please refer to @ref SubflowTasking for details.
   */
   template <typename C,
-    std::enable_if_t<is_dynamic_task_v<C>, void>* = nullptr
+    std::enable_if_t<is_subflow_task_v<C>, void>* = nullptr
   >
   Task emplace(C&& callable);
 
   /**
   @brief creates a condition task
 
   @tparam C callable type constructible from std::function<int()>
@@ -217,15 +217,15 @@
   tf::Task init = t2.emplace([](){ std::cout << "t2"; });
   init.precede(comp);
   @endcode
 
   The taskflow object @c t2 is composed of another taskflow object @c t1,
   preceded by another static task @c init.
   When taskflow @c t2 is submitted to an executor,
-  @c init will run first and then @c comp which spwans its definition
+  @c init will run first and then @c comp which spawns its definition
   in taskflow @c t1.
 
   The target @c object being composed must define the method
   <tt>T::graph()</tt> that returns a reference to a graph object of
   type tf::Graph such that it can interact with the executor.
   For example:
 
@@ -309,25 +309,26 @@
   tf::Task C = taskflow.emplace([](){ std::cout << "C"; });
   tf::Task D = taskflow.emplace([](){ std::cout << "D"; });
   taskflow.linearize({A, B, C, D});  // A->B->C->D
   @endcode
   */
   void linearize(std::initializer_list<Task> tasks);
 
+
   // ------------------------------------------------------------------------
   // parallel iterations
   // ------------------------------------------------------------------------
 
   /**
   @brief constructs an STL-styled parallel-for task
 
   @tparam B beginning iterator type
   @tparam E ending iterator type
   @tparam C callable type
-  @tparam P partitioner type (default tf::GuidedPartitioner)
+  @tparam P partitioner type (default tf::DefaultPartitioner)
 
   @param first iterator to the beginning (inclusive)
   @param last iterator to the end (exclusive)
   @param callable callable object to apply to the dereferenced iterator
   @param part partitioning algorithm to schedule parallel iterations
 
   @return a tf::Task handle
@@ -344,25 +345,25 @@
 
   Iterators are templated to enable stateful range using std::reference_wrapper.
   The callable needs to take a single argument of
   the dereferenced iterator type.
 
   Please refer to @ref ParallelIterations for details.
   */
-  template <typename B, typename E, typename C, typename P = GuidedPartitioner>
-  Task for_each(B first, E last, C callable, P&& part = P());
+  template <typename B, typename E, typename C, typename P = DefaultPartitioner>
+  Task for_each(B first, E last, C callable, P part = P());
   
   /**
   @brief constructs an STL-styled index-based parallel-for task 
 
   @tparam B beginning index type (must be integral)
   @tparam E ending index type (must be integral)
   @tparam S step type (must be integral)
   @tparam C callable type
-  @tparam P partitioner type (default tf::GuidedPartitioner)
+  @tparam P partitioner type (default tf::DefaultPartitioner)
 
   @param first index of the beginning (inclusive)
   @param last index of the end (exclusive)
   @param step step size
   @param callable callable object to apply to each valid index
   @param part partitioning algorithm to schedule parallel iterations
 
@@ -385,31 +386,31 @@
   @endcode
 
   Iterators are templated to enable stateful range using std::reference_wrapper.
   The callable needs to take a single argument of the integral index type.
 
   Please refer to @ref ParallelIterations for details.
   */
-  template <typename B, typename E, typename S, typename C, typename P = GuidedPartitioner>
+  template <typename B, typename E, typename S, typename C, typename P = DefaultPartitioner>
   Task for_each_index(
-    B first, E last, S step, C callable, P&& part = P()
+    B first, E last, S step, C callable, P part = P()
   );
 
   // ------------------------------------------------------------------------
   // transform
   // ------------------------------------------------------------------------
 
   /**
   @brief constructs a parallel-transform task
 
   @tparam B beginning input iterator type
   @tparam E ending input iterator type
   @tparam O output iterator type
   @tparam C callable type
-  @tparam P partitioner type (default tf::GuidedPartitioner)
+  @tparam P partitioner type (default tf::DefaultPartitioner)
 
   @param first1 iterator to the beginning of the first range
   @param last1 iterator to the end of the first range
   @param d_first iterator to the beginning of the output range
   @param c an unary callable to apply to dereferenced input elements
   @param part partitioning algorithm to schedule parallel iterations
 
@@ -428,27 +429,28 @@
   Iterators are templated to enable stateful range using std::reference_wrapper.
   The callable needs to take a single argument of the dereferenced
   iterator type.
   
   Please refer to @ref ParallelTransforms for details.
   */
   template <
-    typename B, typename E, typename O, typename C, typename P = GuidedPartitioner
+    typename B, typename E, typename O, typename C, typename P = DefaultPartitioner,
+    std::enable_if_t<is_partitioner_v<std::decay_t<P>>, void>* = nullptr
   >
-  Task transform(B first1, E last1, O d_first, C c, P&& part = P());
+  Task transform(B first1, E last1, O d_first, C c, P part = P());
   
   /**
   @brief constructs a parallel-transform task
 
   @tparam B1 beginning input iterator type for the first input range
   @tparam E1 ending input iterator type for the first input range
   @tparam B2 beginning input iterator type for the first second range
   @tparam O output iterator type
   @tparam C callable type
-  @tparam P partitioner type (default tf::GuidedPartitioner)
+  @tparam P partitioner type (default tf::DefaultPartitioner)
 
   @param first1 iterator to the beginning of the first input range
   @param last1 iterator to the end of the first input range
   @param first2 iterator to the beginning of the second input range
   @param d_first iterator to the beginning of the output range
   @param c a binary operator to apply to dereferenced input elements
   @param part partitioning algorithm to schedule parallel iterations
@@ -468,31 +470,31 @@
   Iterators are templated to enable stateful range using std::reference_wrapper.
   The callable needs to take two arguments of dereferenced elements
   from the two input ranges.
   
   Please refer to @ref ParallelTransforms for details.
   */
   template <
-    typename B1, typename E1, typename B2, typename O, typename C, typename P=GuidedPartitioner,
+    typename B1, typename E1, typename B2, typename O, typename C, typename P=DefaultPartitioner,
     std::enable_if_t<!is_partitioner_v<std::decay_t<C>>, void>* = nullptr
   >
-  Task transform(B1 first1, E1 last1, B2 first2, O d_first, C c, P&& part = P());
+  Task transform(B1 first1, E1 last1, B2 first2, O d_first, C c, P part = P());
   
   // ------------------------------------------------------------------------
   // reduction
   // ------------------------------------------------------------------------
 
   /**
   @brief constructs an STL-styled parallel-reduce task
 
   @tparam B beginning iterator type
   @tparam E ending iterator type
   @tparam T result type
   @tparam O binary reducer type
-  @tparam P partitioner type (default tf::GuidedPartitioner)
+  @tparam P partitioner type (default tf::DefaultPartitioner)
 
   @param first iterator to the beginning (inclusive)
   @param last iterator to the end (exclusive)
   @param init initial value of the reduction and the storage for the reduced result
   @param bop binary operator that will be applied
   @param part partitioning algorithm to schedule parallel iterations
 
@@ -509,30 +511,30 @@
   }
   @endcode
 
   Iterators are templated to enable stateful range using std::reference_wrapper.
 
   Please refer to @ref ParallelReduction for details.
   */
-  template <typename B, typename E, typename T, typename O, typename P = GuidedPartitioner>
-  Task reduce(B first, E last, T& init, O bop, P&& part = P());
+  template <typename B, typename E, typename T, typename O, typename P = DefaultPartitioner>
+  Task reduce(B first, E last, T& init, O bop, P part = P());
   
   // ------------------------------------------------------------------------
-  // transfrom and reduction
+  // transform and reduction
   // ------------------------------------------------------------------------
 
   /**
   @brief constructs an STL-styled parallel transform-reduce task
 
   @tparam B beginning iterator type
   @tparam E ending iterator type
   @tparam T result type
   @tparam BOP binary reducer type
-  @tparam UOP unary transformion type
-  @tparam P partitioner type (default tf::GuidedPartitioner)
+  @tparam UOP unary transformation type
+  @tparam P partitioner type (default tf::DefaultPartitioner)
 
   @param first iterator to the beginning (inclusive)
   @param last iterator to the end (exclusive)
   @param init initial value of the reduction and the storage for the reduced result
   @param bop binary operator that will be applied in unspecified order to the results of @c uop
   @param uop unary operator that will be applied to transform each element in the range to the result type
   @param part partitioning algorithm to schedule parallel iterations
@@ -551,34 +553,82 @@
   @endcode
 
   Iterators are templated to enable stateful range using std::reference_wrapper.
 
   Please refer to @ref ParallelReduction for details.
   */
   template <
-   typename B, typename E, typename T, typename BOP, typename UOP, typename P = GuidedPartitioner
+    typename B, typename E, typename T, typename BOP, typename UOP, typename P = DefaultPartitioner,
+    std::enable_if_t<is_partitioner_v<std::decay_t<P>>, void>* = nullptr
   >
-  Task transform_reduce(B first, E last, T& init, BOP bop, UOP uop, P&& part = P());
+  Task transform_reduce(B first, E last, T& init, BOP bop, UOP uop, P part = P());
+
+  /**
+  @brief constructs an STL-styled parallel transform-reduce task
+  @tparam B1 first beginning iterator type
+  @tparam E1 first ending iterator type
+  @tparam B2 second beginning iterator type
+  @tparam T result type
+  @tparam BOP_R binary reducer type
+  @tparam BOP_T binary transformation type
+  @tparam P partitioner type (default tf::DefaultPartitioner)
+ 
+  @param first1 iterator to the beginning of the first range (inclusive)
+  @param last1 iterator to the end of the first range (exclusive)
+  @param first2 iterator to the beginning of the second range
+  @param init initial value of the reduction and the storage for the reduced result
+  @param bop_r binary operator that will be applied in unspecified order to the results of @c bop_t
+  @param bop_t binary operator that will be applied to transform each element in the range to the result type
+  @param part partitioning algorithm to schedule parallel iterations
+ 
+  @return a tf::Task handle
+ 
+  The task spawns asynchronous tasks to perform parallel reduction over @c init and
+  transformed elements in the range <tt>[first, last)</tt>.
+  The reduced result is store in @c init.
+  This method is equivalent to the parallel execution of the following loop:
+ 
+  @code{.cpp}
+  for(auto itr1=first1, itr2=first2; itr1!=last1; itr1++, itr2++) {
+    init = bop_r(init, bop_t(*itr1, *itr2));
+  }
+  @endcode
+ 
+  Iterators are templated to enable stateful range using std::reference_wrapper.
+
+  Please refer to @ref ParallelReduction for details.
+  */
   
+  template <
+    typename B1, typename E1, typename B2, typename T, typename BOP_R, typename BOP_T, 
+    typename P = DefaultPartitioner,
+    std::enable_if_t<!is_partitioner_v<std::decay_t<BOP_T>>, void>* = nullptr
+  >
+  Task transform_reduce(
+    B1 first1, E1 last1, B2 first2, T& init, BOP_R bop_r, BOP_T bop_t, P part = P()
+  );
+
   // ------------------------------------------------------------------------
   // scan
   // ------------------------------------------------------------------------
   
   /**
   @brief creates an STL-styled parallel inclusive-scan task
 
   @tparam B beginning iterator type
   @tparam E ending iterator type
   @tparam D destination iterator type
   @tparam BOP summation operator type
+  @tparam P partitioner type (default tf::DefaultPartitioner)
 
   @param first start of input range
   @param last end of input range
   @param d_first start of output range (may be the same as input range)
   @param bop function to perform summation
+  @param part partitioning algorithm to schedule parallel iterations
 
   Performs the cumulative sum (aka prefix sum, aka scan) of the input range
   and writes the result to the output range. 
   Each element of the output range contains the
   running total of all earlier elements using the given binary operator
   for summation.
   
@@ -596,31 +646,35 @@
   // input is {1, 3, 6, 10, 15}
   @endcode
   
   Iterators are templated to enable stateful range using std::reference_wrapper.
   
   Please refer to @ref ParallelScan for details.
   */
-  template <typename B, typename E, typename D, typename BOP>
-  Task inclusive_scan(B first, E last, D d_first, BOP bop);
+  template <typename B, typename E, typename D, typename BOP, typename P = DefaultPartitioner,
+    std::enable_if_t<is_partitioner_v<std::decay_t<P>>, void>* = nullptr
+  >
+  Task inclusive_scan(B first, E last, D d_first, BOP bop, P part = P());
   
   /**
   @brief creates an STL-styled parallel inclusive-scan task with an initial value
 
   @tparam B beginning iterator type
   @tparam E ending iterator type
   @tparam D destination iterator type
   @tparam BOP summation operator type
   @tparam T initial value type
+  @tparam P partitioner type (default tf::DefaultPartitioner)
 
   @param first start of input range
   @param last end of input range
   @param d_first start of output range (may be the same as input range)
   @param bop function to perform summation
   @param init initial value
+  @param part partitioning algorithm to schedule parallel iterations
 
   Performs the cumulative sum (aka prefix sum, aka scan) of the input range
   and writes the result to the output range. 
   Each element of the output range contains the
   running total of all earlier elements (and the initial value)
   using the given binary operator for summation.
   
@@ -639,31 +693,35 @@
   @endcode
   
   Iterators are templated to enable stateful range using std::reference_wrapper.
  
   Please refer to @ref ParallelScan for details.
 
   */
-  template <typename B, typename E, typename D, typename BOP, typename T>
-  Task inclusive_scan(B first, E last, D d_first, BOP bop, T init);
+  template <typename B, typename E, typename D, typename BOP, typename T, typename P = DefaultPartitioner,
+    std::enable_if_t<!is_partitioner_v<std::decay_t<T>>, void>* = nullptr
+  >
+  Task inclusive_scan(B first, E last, D d_first, BOP bop, T init, P part = P());
   
   /**
   @brief creates an STL-styled parallel exclusive-scan task
 
   @tparam B beginning iterator type
   @tparam E ending iterator type
   @tparam D destination iterator type
   @tparam T initial value type
   @tparam BOP summation operator type
+  @tparam P partitioner type (default tf::DefaultPartitioner)
 
   @param first start of input range
   @param last end of input range
   @param d_first start of output range (may be the same as input range)
   @param init initial value
   @param bop function to perform summation
+  @param part partitioning algorithm to schedule parallel iterations
 
   Performs the cumulative sum (aka prefix sum, aka scan) of the input range
   and writes the result to the output range. 
   Each element of the output range contains the
   running total of all earlier elements (and the initial value)
   using the given binary operator for summation.
   
@@ -681,35 +739,37 @@
   // input is {-1, 0, 2, 5, 9}
   @endcode
   
   Iterators are templated to enable stateful range using std::reference_wrapper.
   
   Please refer to @ref ParallelScan for details.
   */
-  template <typename B, typename E, typename D, typename T, typename BOP>
-  Task exclusive_scan(B first, E last, D d_first, T init, BOP bop);
+  template <typename B, typename E, typename D, typename T, typename BOP, typename P = DefaultPartitioner>
+  Task exclusive_scan(B first, E last, D d_first, T init, BOP bop, P part = P());
   
   // ------------------------------------------------------------------------
   // transform scan
   // ------------------------------------------------------------------------
   
   /**
   @brief creates an STL-styled parallel transform-inclusive scan task
 
   @tparam B beginning iterator type
   @tparam E ending iterator type
   @tparam D destination iterator type
   @tparam BOP summation operator type
   @tparam UOP transform operator type
+  @tparam P partitioner type (default tf::DefaultPartitioner)
 
   @param first start of input range
   @param last end of input range
   @param d_first start of output range (may be the same as input range)
   @param bop function to perform summation
   @param uop function to transform elements of the input range
+  @param part partitioning algorithm to schedule parallel iterations
 
   Write the cumulative sum (aka prefix sum, aka scan) of the input range
   to the output range. Each element of the output range contains the
   running total of all earlier elements
   using @c uop to transform the input elements
   and using @c bop for summation.
   
@@ -728,33 +788,37 @@
   // input is {-1, -3, -6, -10, -15}
   @endcode
   
   Iterators are templated to enable stateful range using std::reference_wrapper.
   
   Please refer to @ref ParallelScan for details.
   */
-  template <typename B, typename E, typename D, typename BOP, typename UOP>
-  Task transform_inclusive_scan(B first, E last, D d_first, BOP bop, UOP uop);
+  template <typename B, typename E, typename D, typename BOP, typename UOP, typename P = DefaultPartitioner,
+    std::enable_if_t<is_partitioner_v<std::decay_t<P>>, void>* = nullptr
+  >
+  Task transform_inclusive_scan(B first, E last, D d_first, BOP bop, UOP uop, P part = P());
   
   /**
   @brief creates an STL-styled parallel transform-inclusive scan task
 
   @tparam B beginning iterator type
   @tparam E ending iterator type
   @tparam D destination iterator type
   @tparam BOP summation operator type
   @tparam UOP transform operator type
   @tparam T initial value type
+  @tparam P partitioner type (default tf::DefaultPartitioner)
 
   @param first start of input range
   @param last end of input range
   @param d_first start of output range (may be the same as input range)
   @param bop function to perform summation
   @param uop function to transform elements of the input range
   @param init initial value
+  @param part partitioning algorithm to schedule parallel iterations
 
   Write the cumulative sum (aka prefix sum, aka scan) of the input range
   to the output range. Each element of the output range contains the
   running total of all earlier elements (including an initial value)
   using @c uop to transform the input elements
   and using @c bop for summation.
   
@@ -774,33 +838,37 @@
   // input is {-2, -4, -7, -11, -16}
   @endcode
   
   Iterators are templated to enable stateful range using std::reference_wrapper.
   
   Please refer to @ref ParallelScan for details.
   */
-  template <typename B, typename E, typename D, typename BOP, typename UOP, typename T>
-  Task transform_inclusive_scan(B first, E last, D d_first, BOP bop, UOP uop, T init);
+  template <typename B, typename E, typename D, typename BOP, typename UOP, typename T, typename P = DefaultPartitioner,
+    std::enable_if_t<!is_partitioner_v<std::decay_t<T>>, void>* = nullptr
+  >
+  Task transform_inclusive_scan(B first, E last, D d_first, BOP bop, UOP uop, T init, P part = P());
   
   /**
   @brief creates an STL-styled parallel transform-exclusive scan task
 
   @tparam B beginning iterator type
   @tparam E ending iterator type
   @tparam D destination iterator type
   @tparam BOP summation operator type
   @tparam UOP transform operator type
   @tparam T initial value type
+  @tparam P partitioner type (default tf::DefaultPartitioner)
 
   @param first start of input range
   @param last end of input range
   @param d_first start of output range (may be the same as input range)
   @param bop function to perform summation
   @param uop function to transform elements of the input range
   @param init initial value
+  @param part partitioning algorithm to schedule parallel iterations
 
   Write the cumulative sum (aka prefix sum, aka scan) of the input range
   to the output range. Each element of the output range contains the
   running total of all earlier elements (including an initial value)
   using @c uop to transform the input elements
   and using @c bop for summation.
   
@@ -819,16 +887,16 @@
   // input is {-1, -2, -4, -7, -11}
   @endcode
   
   Iterators are templated to enable stateful range using std::reference_wrapper.
   
   Please refer to @ref ParallelScan for details.
   */
-  template <typename B, typename E, typename D, typename T, typename BOP, typename UOP>
-  Task transform_exclusive_scan(B first, E last, D d_first, T init, BOP bop, UOP uop);
+  template <typename B, typename E, typename D, typename T, typename BOP, typename UOP, typename P = DefaultPartitioner>
+  Task transform_exclusive_scan(B first, E last, D d_first, T init, BOP bop, UOP uop, P part = P());
 
   // ------------------------------------------------------------------------
   // find
   // ------------------------------------------------------------------------
  
   /**
   @brief constructs a task to perform STL-styled find-if algorithm
@@ -839,15 +907,15 @@
   @tparam UOP unary predicate type
   @tparam P partitioner type
   
   @param first start of the input range
   @param last end of the input range
   @param result resulting iterator to the found element in the input range
   @param predicate unary predicate which returns @c true for the required element
-  @param part partitioning algorithm (default tf::GuidedPartitioner)
+  @param part partitioning algorithm (default tf::DefaultPartitioner)
 
   Returns an iterator to the first element in the range <tt>[first, last)</tt> 
   that satisfies the given criteria (or last if there is no such iterator).
   This method is equivalent to the parallel execution of the following loop:
 
   @code{.cpp}
   auto find_if(InputIt first, InputIt last, UnaryPredicate p) {
@@ -871,31 +939,31 @@
   );
   executor.run(taskflow).wait();
   assert(*result == 22);
   @endcode
   
   Iterators are templated to enable stateful range using std::reference_wrapper.
   */
-  template <typename B, typename E, typename T, typename UOP, typename P = GuidedPartitioner>
-  Task find_if(B first, E last, T& result, UOP predicate, P&& part = P());
-  
+  template <typename B, typename E, typename T, typename UOP, typename P = DefaultPartitioner>
+  Task find_if(B first, E last, T &result, UOP predicate, P part = P());
+
   /**
   @brief constructs a task to perform STL-styled find-if-not algorithm
 
   @tparam B beginning iterator type
   @tparam E ending iterator type
   @tparam T resulting iterator type
   @tparam UOP unary predicate type
   @tparam P partitioner type
   
   @param first start of the input range
   @param last end of the input range
   @param result resulting iterator to the found element in the input range
   @param predicate unary predicate which returns @c false for the required element
-  @param part partitioning algorithm (default tf::GuidedPartitioner)
+  @param part partitioning algorithm (default tf::DefaultPartitioner)
 
   Returns an iterator to the first element in the range <tt>[first, last)</tt> 
   that satisfies the given criteria (or last if there is no such iterator).
   This method is equivalent to the parallel execution of the following loop:
 
   @code{.cpp}
   auto find_if(InputIt first, InputIt last, UnaryPredicate p) {
@@ -919,31 +987,31 @@
   );
   executor.run(taskflow).wait();
   assert(*result == 22);
   @endcode
   
   Iterators are templated to enable stateful range using std::reference_wrapper.
   */
-  template <typename B, typename E, typename T, typename UOP,typename P = GuidedPartitioner>
-  Task find_if_not(B first, E last, T& result, UOP predicate, P&& part = P());
+  template <typename B, typename E, typename T, typename UOP, typename P = DefaultPartitioner>
+  Task find_if_not(B first, E last, T &result, UOP predicate, P part = P());
 
   /**
   @brief constructs a task to perform STL-styled min-element algorithm
 
   @tparam B beginning iterator type
   @tparam E ending iterator type
   @tparam T resulting iterator type
   @tparam C comparator type
   @tparam P partitioner type
   
   @param first start of the input range
   @param last end of the input range
   @param result resulting iterator to the found element in the input range
   @param comp comparison function object
-  @param part partitioning algorithm (default tf::GuidedPartitioner)
+  @param part partitioning algorithm (default tf::DefaultPartitioner)
 
   Finds the smallest element in the <tt>[first, last)</tt> 
   using the given comparison function object.
   The iterator to that smallest element is stored in @c result.
   This method is equivalent to the parallel execution of the following loop:
 
   @code{.cpp}
@@ -972,30 +1040,30 @@
   executor.run(taskflow).wait();
   assert(*result == -1);
   @endcode
   
   Iterators are templated to enable stateful range using std::reference_wrapper.
   */
   template <typename B, typename E, typename T, typename C, typename P>
-  Task min_element(B first, E last, T& result, C comp, P&& part);
+  Task min_element(B first, E last, T& result, C comp, P part);
   
   /**
   @brief constructs a task to perform STL-styled max-element algorithm
 
   @tparam B beginning iterator type
   @tparam E ending iterator type
   @tparam T resulting iterator type
   @tparam C comparator type
   @tparam P partitioner type
   
   @param first start of the input range
   @param last end of the input range
   @param result resulting iterator to the found element in the input range
   @param comp comparison function object
-  @param part partitioning algorithm (default tf::GuidedPartitioner)
+  @param part partitioning algorithm (default tf::DefaultPartitioner)
 
   Finds the largest element in the <tt>[first, last)</tt> 
   using the given comparison function object.
   The iterator to that largest element is stored in @c result.
   This method is equivalent to the parallel execution of the following loop:
 
   @code{.cpp}
@@ -1024,15 +1092,15 @@
   executor.run(taskflow).wait();
   assert(*result == 2);
   @endcode
   
   Iterators are templated to enable stateful range using std::reference_wrapper.
   */
   template <typename B, typename E, typename T, typename C, typename P>
-  Task max_element(B first, E last, T& result, C comp, P&& part);
+  Task max_element(B first, E last, T& result, C comp, P part);
 
   // ------------------------------------------------------------------------
   // sort
   // ------------------------------------------------------------------------
 
   /**
   @brief constructs a dynamic task to perform STL-styled parallel sort
@@ -1061,15 +1129,15 @@
 
   @tparam B beginning iterator type (random-accessible)
   @tparam E ending iterator type (random-accessible)
 
   @param first iterator to the beginning (inclusive)
   @param last iterator to the end (exclusive)
 
-  The task spawns asynchronous tasks to parallelly sort elements in the range
+  The task spawns asynchronous tasks to parallel sort elements in the range
   <tt>[first, last)</tt> using the @c std::less<T> comparator,
   where @c T is the dereferenced iterator type.
 
   Iterators are templated to enable stateful range using std::reference_wrapper.
 
   Please refer to @ref ParallelSort for details.
    */
@@ -1099,18 +1167,18 @@
 Task FlowBuilder::emplace(C&& c) {
   return Task(_graph._emplace_back("", 0, nullptr, nullptr, 0,
     std::in_place_type_t<Node::Static>{}, std::forward<C>(c)
   ));
 }
 
 // Function: emplace
-template <typename C, std::enable_if_t<is_dynamic_task_v<C>, void>*>
+template <typename C, std::enable_if_t<is_subflow_task_v<C>, void>*>
 Task FlowBuilder::emplace(C&& c) {
   return Task(_graph._emplace_back("", 0, nullptr, nullptr, 0,
-    std::in_place_type_t<Node::Dynamic>{}, std::forward<C>(c)
+    std::in_place_type_t<Node::Subflow>{}, std::forward<C>(c)
   ));
 }
 
 // Function: emplace
 template <typename C, std::enable_if_t<is_condition_task_v<C>, void>*>
 Task FlowBuilder::emplace(C&& c) {
   return Task(_graph._emplace_back("", 0, nullptr, nullptr, 0,
```

### Comparing `rapidfuzz-3.9.0/extern/taskflow/taskflow/core/graph.hpp` & `rapidfuzz-3.9.1/extern/taskflow/taskflow/core/graph.hpp`

 * *Files 10% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 
 namespace tf {
 
 // ----------------------------------------------------------------------------
 // Class: Graph
 // ----------------------------------------------------------------------------
 
+
 /**
 @class Graph
 
 @brief class to create a graph object
 
 A graph is the ultimate storage for a task dependency graph and is the main
 gateway to interact with an executor.
@@ -143,14 +144,22 @@
 */
 class Runtime {
 
   friend class Executor;
   friend class FlowBuilder;
 
   public:
+  
+  /**
+  @brief destroys the runtime object
+
+  Issues a tf::Runtime::corun_all to finish all spawned asynchronous tasks
+  and then destroys the runtime object.
+  */
+  ~Runtime();
 
   /**
   @brief obtains the running executor
 
   The running executor of a runtime task is the executor that runs
   the parent taskflow of that runtime task.
 
@@ -207,17 +216,17 @@
 
   @tparam F callable type
   @param f callable object
     
   The method creates an asynchronous task to launch the given
   function on the given arguments.
   The difference to tf::Executor::async is that the created asynchronous task
-  pertains to the runtime.
-  When the runtime joins, all asynchronous tasks created from the runtime
-  are guaranteed to finish after the join returns.
+  pertains to the runtime object.
+  Applications can explicitly issue tf::Runtime::corun_all
+  to wait for all spawned asynchronous tasks to finish.
   For example:
 
   @code{.cpp}
   std::atomic<int> counter(0);
   taskflow.emplace([&](tf::Runtime& rt){
     auto fu1 = rt.async([&](){ counter++; });
     auto fu2 = rt.async([&](){ counter++; });
@@ -226,16 +235,16 @@
     assert(counter == 2);
     
     // spawn 100 asynchronous tasks from the worker of the runtime
     for(int i=0; i<100; i++) {
       rt.async([&](){ counter++; });
     }
     
-    // explicit join 100 asynchronous tasks
-    rt.join();
+    // wait for the 100 asynchronous tasks to finish
+    rt.corun_all();
     assert(counter == 102);
   });
   @endcode
 
   This method is thread-safe and can be called by multiple workers
   that hold the reference to the runtime.
   For example, the code below spawns 100 tasks from the worker of
@@ -250,41 +259,42 @@
     for(int i=0; i<100; i++) {
       rt.async([&](){ 
         counter++; 
         rt.async([](){ counter++; });
       });
     }
     
-    // explicit join 100 asynchronous tasks
-    rt.join();
+    // wait for the 200 asynchronous tasks to finish
+    rt.corun_all();
     assert(counter == 200);
   });
   @endcode
   */
   template <typename F>
   auto async(F&& f);
   
   /**
-  @brief similar to tf::Runtime::async but assigns the task a name
+  @brief runs the given callable asynchronously
 
   @tparam F callable type
+  @tparam P task parameters type
 
-  @param name assigned name to the task
+  @param params task parameters
   @param f callable
 
   @code{.cpp}
   taskflow.emplace([&](tf::Runtime& rt){
     auto future = rt.async("my task", [](){});
     future.get();
   });
   @endcode
 
   */
-  template <typename F>
-  auto async(const std::string& name, F&& f);
+  template <typename P, typename F>
+  auto async(P&& params, F&& f);
 
   /**
   @brief runs the given function asynchronously without returning any future object
 
   @tparam F callable type
   @param f callable
 
@@ -293,68 +303,90 @@
 
   @code{.cpp}
   std::atomic<int> counter(0);
   taskflow.emplace([&](tf::Runtime& rt){
     for(int i=0; i<100; i++) {
       rt.silent_async([&](){ counter++; });
     }
-    rt.join();
+    rt.corun_all();
     assert(counter == 100);
   });
   @endcode
 
   This member function is thread-safe.
   */
   template <typename F>
   void silent_async(F&& f);
   
   /**
-  @brief similar to tf::Runtime::silent_async but assigns the task a name
+  @brief runs the given function asynchronously without returning any future object
 
   @tparam F callable type
-  @param name assigned name to the task
+  @param params task parameters
   @param f callable
   
   @code{.cpp}
   taskflow.emplace([&](tf::Runtime& rt){
     rt.silent_async("my task", [](){});
-    rt.join();
+    rt.corun_all();
+  });
+  @endcode
+  */
+  template <typename P, typename F>
+  void silent_async(P&& params, F&& f);
+  
+  /**
+  @brief similar to tf::Runtime::silent_async but the caller must be the worker of the runtime
+
+  @tparam F callable type
+
+  @param f callable
+
+  The method bypass the check of the caller worker from the executor 
+  and thus can only called by the worker of this runtime.
+
+  @code{.cpp}
+  taskflow.emplace([&](tf::Runtime& rt){
+    // running by the worker of this runtime
+    rt.silent_async_unchecked([](){});
+    rt.corun_all();
   });
   @endcode
   */
   template <typename F>
-  void silent_async(const std::string& name, F&& f);
+  void silent_async_unchecked(F&& f);
   
   /**
   @brief similar to tf::Runtime::silent_async but the caller must be the worker of the runtime
 
   @tparam F callable type
+  @tparam P task parameters type
 
-  @param name assigned name to the task
+  @param params task parameters
   @param f callable
 
   The method bypass the check of the caller worker from the executor 
   and thus can only called by the worker of this runtime.
 
   @code{.cpp}
   taskflow.emplace([&](tf::Runtime& rt){
     // running by the worker of this runtime
     rt.silent_async_unchecked("my task", [](){});
-    rt.join();
+    rt.corun_all();
   });
   @endcode
   */
-  template <typename F>
-  void silent_async_unchecked(const std::string& name, F&& f);
+  template <typename P, typename F>
+  void silent_async_unchecked(P&& params, F&& f);
 
   /**
   @brief co-runs the given target and waits until it completes
   
   A target can be one of the following forms:
-    + a dynamic task to spawn a subflow or
+    + a subflow task to spawn a subflow or
     + a composable graph object with `tf::Graph& T::graph()` defined
 
   @code{.cpp}
   // co-run a subflow and wait until all tasks complete
   taskflow.emplace([](tf::Runtime& rt){
     rt.corun([](tf::Subflow& sf){
       tf::Task A = sf.emplace([](){});
@@ -372,61 +404,66 @@
   executor.run(taskflow2).wait();
   @endcode
 
   Although tf::Runtime::corun blocks until the operation completes, 
   the caller thread (worker) is not blocked (e.g., sleeping or holding any lock). 
   Instead, the caller thread joins the work-stealing loop of the executor 
   and returns when all tasks in the target completes.
+  
+  @attention
+  Only the worker of this tf::Runtime can issue corun.
   */
   template <typename T>
   void corun(T&& target);
 
   /**
   @brief keeps running the work-stealing loop until the predicate becomes true
   
   @tparam P predicate type
   @param predicate a boolean predicate to indicate when to stop the loop
 
   The method keeps the caller worker running in the work-stealing loop
   until the stop predicate becomes true.
+  
+  @attention
+  Only the worker of this tf::Runtime can issue corun.
   */
   template <typename P>
   void corun_until(P&& predicate);
   
   /**
-  @brief joins all asynchronous tasks spawned by this runtime
+  @brief corun all asynchronous tasks spawned by this runtime with other workers
 
-  Immediately joins all asynchronous tasks (tf::Runtime::async,
-  tf::Runtime::silent_async).
-  Unlike tf::Subflow::join, you can join multiples times from
-  a tf::Runtime object.
+  Coruns all asynchronous tasks (tf::Runtime::async,
+  tf::Runtime::silent_async) with other workers until all those 
+  asynchronous tasks finish.
     
   @code{.cpp}
   std::atomic<size_t> counter{0};
   taskflow.emplace([&](tf::Runtime& rt){
-    // spawn 100 async tasks and join
+    // spawn 100 async tasks and wait
     for(int i=0; i<100; i++) {
       rt.silent_async([&](){ counter++; });
     }
-    rt.join();
+    rt.corun_all();
     assert(counter == 100);
     
-    // spawn another 100 async tasks and join
+    // spawn another 100 async tasks and wait
     for(int i=0; i<100; i++) {
       rt.silent_async([&](){ counter++; });
     }
-    rt.join();
+    rt.corun_all();
     assert(counter == 200);
   });
   @endcode
 
   @attention
-  Only the worker of this tf::Runtime can issue join.
+  Only the worker of this tf::Runtime can issue tf::Runtime::corun_all.
   */
-  inline void join();
+  inline void corun_all();
 
   /**
   @brief acquire a reference to the underlying worker
   */
   inline Worker& worker();
 
   protected:
@@ -450,22 +487,22 @@
   @private
   */
   Node* _parent;
 
   /**
   @private
   */
-  template <typename F>
-  auto _async(Worker& w, const std::string& name, F&& f);
+  template <typename P, typename F>
+  auto _async(Worker& w, P&& params, F&& f);
   
   /**
   @private
   */
-  template <typename F>
-  void _silent_async(Worker& w, const std::string& name, F&& f);
+  template <typename P, typename F>
+  void _silent_async(Worker& w, P&& params, F&& f);
 };
 
 // constructor
 inline Runtime::Runtime(Executor& e, Worker& w, Node* p) :
   _executor{e},
   _worker  {w},
   _parent  {p}{
@@ -478,24 +515,73 @@
 
 // Function: worker
 inline Worker& Runtime::worker() {
   return _worker;
 }
 
 // ----------------------------------------------------------------------------
+// TaskParams
+// ----------------------------------------------------------------------------
+
+/**
+@struct TaskParams
+
+@brief task parameters to use when creating an asynchronous task
+*/
+struct TaskParams {
+  /**
+  @brief name of the task
+  */
+  std::string name;
+
+  /**
+  @brief priority of the tassk
+  */
+  unsigned priority {0};
+
+  /**
+  @brief C-styled pointer to user data
+  */
+  void* data {nullptr};
+};
+
+/**
+@struct DefaultTaskParams
+
+@brief empty task parameter type for compile-time optimization
+*/
+struct DefaultTaskParams {
+};
+
+/**
+@brief determines if the given type is a task parameter type
+
+Task parameters can be specified in one of the following types:
+  + tf::TaskParams: assign the struct of defined parameters
+  + tf::DefaultTaskParams: assign nothing
+  + std::string: assign a name to the task
+*/
+template <typename P>
+constexpr bool is_task_params_v =
+  std::is_same_v<std::decay_t<P>, TaskParams> ||
+  std::is_same_v<std::decay_t<P>, DefaultTaskParams> ||
+  std::is_constructible_v<std::string, P>;
+
+// ----------------------------------------------------------------------------
 // Node
 // ----------------------------------------------------------------------------
 
 /**
 @private
 */
 class Node {
 
   friend class Graph;
   friend class Task;
+  friend class AsyncTask;
   friend class TaskView;
   friend class Taskflow;
   friend class Executor;
   friend class FlowBuilder;
   friend class Subflow;
   friend class Runtime;
 
@@ -508,35 +594,36 @@
   TF_ENABLE_POOLABLE_ON_THIS;
 
   // state bit flag
   constexpr static int CONDITIONED = 1;
   constexpr static int DETACHED    = 2;
   constexpr static int ACQUIRED    = 4;
   constexpr static int READY       = 8;
+  constexpr static int EXCEPTION   = 16;
 
   using Placeholder = std::monostate;
 
   // static work handle
   struct Static {
 
     template <typename C>
     Static(C&&);
 
     std::variant<
       std::function<void()>, std::function<void(Runtime&)>
     > work;
   };
 
-  // dynamic work handle
-  struct Dynamic {
+  // subflow work handle
+  struct Subflow {
 
     template <typename C>
-    Dynamic(C&&);
+    Subflow(C&&);
 
-    std::function<void(Subflow&)> work;
+    std::function<void(tf::Subflow&)> work;
     Graph subgraph;
   };
 
   // condition work handle
   struct Condition {
 
     template <typename C>
@@ -569,60 +656,74 @@
 
   // Async work
   struct Async {
 
     template <typename T>
     Async(T&&);
 
-    std::function<void()> work;
+    std::variant<
+      std::function<void()>, std::function<void(Runtime&)>
+    > work;
   };
   
   // silent dependent async
   struct DependentAsync {
     
     template <typename C>
     DependentAsync(C&&);
     
-    std::function<void()> work;
-    
+    std::variant<
+      std::function<void()>, std::function<void(Runtime&)>
+    > work;
+   
+    std::atomic<size_t> use_count {1};
     std::atomic<AsyncState> state {AsyncState::UNFINISHED};
   };
 
   using handle_t = std::variant<
     Placeholder,      // placeholder
     Static,           // static tasking
-    Dynamic,          // dynamic tasking
+    Subflow,          // subflow tasking
     Condition,        // conditional tasking
     MultiCondition,   // multi-conditional tasking
     Module,           // composable tasking
     Async,            // async tasking
-    DependentAsync    // dependent async tasking (no future)
+    DependentAsync    // dependent async tasking
   >;
 
   struct Semaphores {
     SmallVector<Semaphore*> to_acquire;
     SmallVector<Semaphore*> to_release;
   };
 
   public:
 
   // variant index
   constexpr static auto PLACEHOLDER     = get_index_v<Placeholder, handle_t>;
   constexpr static auto STATIC          = get_index_v<Static, handle_t>;
-  constexpr static auto DYNAMIC         = get_index_v<Dynamic, handle_t>;
+  constexpr static auto SUBFLOW         = get_index_v<Subflow, handle_t>;
   constexpr static auto CONDITION       = get_index_v<Condition, handle_t>;
   constexpr static auto MULTI_CONDITION = get_index_v<MultiCondition, handle_t>;
   constexpr static auto MODULE          = get_index_v<Module, handle_t>;
   constexpr static auto ASYNC           = get_index_v<Async, handle_t>;
   constexpr static auto DEPENDENT_ASYNC = get_index_v<DependentAsync, handle_t>;
 
   Node() = default;
 
   template <typename... Args>
-  Node(const std::string&, unsigned, Topology*, Node*, size_t, Args&&... args);
+  Node(const std::string&, unsigned, Topology*, Node*, size_t, Args&&...);
+  
+  template <typename... Args>
+  Node(const std::string&, Topology*, Node*, size_t, Args&&...);
+  
+  template <typename... Args>
+  Node(const TaskParams&, Topology*, Node*, size_t, Args&&...);
+  
+  template <typename... Args>
+  Node(const DefaultTaskParams&, Topology*, Node*, size_t, Args&&...);
 
   ~Node();
 
   size_t num_successors() const;
   size_t num_dependents() const;
   size_t num_strong_dependents() const;
   size_t num_weak_dependents() const;
@@ -631,31 +732,33 @@
 
   private:
 
   std::string _name;
   
   unsigned _priority {0};
   
+  void* _data {nullptr};
+  
   Topology* _topology {nullptr};
   Node* _parent {nullptr};
 
-  void* _data {nullptr};
-
   SmallVector<Node*> _successors;
   SmallVector<Node*> _dependents;
 
   std::atomic<int> _state {0};
   std::atomic<size_t> _join_counter {0};
 
   std::unique_ptr<Semaphores> _semaphores;
+  std::exception_ptr _exception_ptr {nullptr};
   
   handle_t _handle;
 
   void _precede(Node*);
   void _set_up_join_counter();
+  void _process_exception();
 
   bool _is_cancelled() const;
   bool _is_conditioner() const;
   bool _acquire_all(SmallVector<Node*>&);
 
   SmallVector<Node*> _release_all();
 };
@@ -675,20 +778,20 @@
 
 // Constructor
 template <typename C>
 Node::Static::Static(C&& c) : work {std::forward<C>(c)} {
 }
 
 // ----------------------------------------------------------------------------
-// Definition for Node::Dynamic
+// Definition for Node::Subflow
 // ----------------------------------------------------------------------------
 
 // Constructor
 template <typename C>
-Node::Dynamic::Dynamic(C&& c) : work {std::forward<C>(c)} {
+Node::Subflow::Subflow(C&& c) : work {std::forward<C>(c)} {
 }
 
 // ----------------------------------------------------------------------------
 // Definition for Node::Condition
 // ----------------------------------------------------------------------------
 
 // Constructor
@@ -750,41 +853,87 @@
   _priority     {priority},
   _topology     {topology},
   _parent       {parent},
   _join_counter {join_counter},
   _handle       {std::forward<Args>(args)...} {
 }
 
-//Node::Node(Args&&... args): _handle{std::forward<Args>(args)...} {
-//}
+// Constructor
+template <typename... Args>
+Node::Node(
+  const std::string& name,
+  Topology* topology, 
+  Node* parent, 
+  size_t join_counter,
+  Args&&... args
+) :
+  _name         {name},
+  _topology     {topology},
+  _parent       {parent},
+  _join_counter {join_counter},
+  _handle       {std::forward<Args>(args)...} {
+}
+
+// Constructor
+template <typename... Args>
+Node::Node(
+  const TaskParams& params,
+  Topology* topology, 
+  Node* parent, 
+  size_t join_counter,
+  Args&&... args
+) :
+  _name         {params.name},
+  _priority     {params.priority},
+  _data         {params.data},
+  _topology     {topology},
+  _parent       {parent},
+  _join_counter {join_counter},
+  _handle       {std::forward<Args>(args)...} {
+}
+
+// Constructor
+template <typename... Args>
+Node::Node(
+  const DefaultTaskParams&,
+  Topology* topology, 
+  Node* parent, 
+  size_t join_counter,
+  Args&&... args
+) :
+  _topology     {topology},
+  _parent       {parent},
+  _join_counter {join_counter},
+  _handle       {std::forward<Args>(args)...} {
+}
 
 // Destructor
 inline Node::~Node() {
   // this is to avoid stack overflow
 
-  if(_handle.index() == DYNAMIC) {
+  if(_handle.index() == SUBFLOW) {
     // using std::get_if instead of std::get makes this compatible
     // with older macOS versions
     // the result of std::get_if is guaranteed to be non-null
     // due to the index check above
-    auto& subgraph = std::get_if<Dynamic>(&_handle)->subgraph;
+    auto& subgraph = std::get_if<Subflow>(&_handle)->subgraph;
     std::vector<Node*> nodes;
     nodes.reserve(subgraph.size());
 
     std::move(
       subgraph._nodes.begin(), subgraph._nodes.end(), std::back_inserter(nodes)
     );
     subgraph._nodes.clear();
 
     size_t i = 0;
 
     while(i < nodes.size()) {
 
-      if(nodes[i]->_handle.index() == DYNAMIC) {
-        auto& sbg = std::get_if<Dynamic>(&(nodes[i]->_handle))->subgraph;
+      if(nodes[i]->_handle.index() == SUBFLOW) {
+        auto& sbg = std::get_if<Subflow>(&(nodes[i]->_handle))->subgraph;
         std::move(
           sbg._nodes.begin(), sbg._nodes.end(), std::back_inserter(nodes)
         );
         sbg._nodes.clear();
       }
 
       ++i;
@@ -845,33 +994,44 @@
 // Function: _is_conditioner
 inline bool Node::_is_conditioner() const {
   return _handle.index() == Node::CONDITION ||
          _handle.index() == Node::MULTI_CONDITION;
 }
 
 // Function: _is_cancelled
+// we currently only support cancellation of taskflow (no async task)
 inline bool Node::_is_cancelled() const {
-  return _topology && _topology->_is_cancelled.load(std::memory_order_relaxed);
+  //return _topology && _topology->_is_cancelled.load(std::memory_order_relaxed);
+  return _topology &&
+         (_topology->_state.load(std::memory_order_relaxed) & Topology::CANCELLED);
 }
 
 // Procedure: _set_up_join_counter
 inline void Node::_set_up_join_counter() {
   size_t c = 0;
   for(auto p : _dependents) {
     //if(p->_handle.index() == Node::CONDITION) {
     if(p->_is_conditioner()) {
       _state.fetch_or(Node::CONDITIONED, std::memory_order_relaxed);
     }
     else {
       c++;
     }
   }
-  _join_counter.store(c, std::memory_order_release);
+  _join_counter.store(c, std::memory_order_relaxed);
 }
 
+// Procedure: _process_exception
+inline void Node::_process_exception() {
+  if(_exception_ptr) {
+    auto e = _exception_ptr;
+    _exception_ptr = nullptr;
+    std::rethrow_exception(e);
+  }
+}
 
 // Function: _acquire_all
 inline bool Node::_acquire_all(SmallVector<Node*>& nodes) {
 
   auto& to_acquire = _semaphores->to_acquire;
 
   for(size_t i = 0; i < to_acquire.size(); ++i) {
@@ -991,8 +1151,19 @@
 */
 template <typename ...ArgsT>
 Node* Graph::_emplace_back(ArgsT&&... args) {
   _nodes.push_back(node_pool.animate(std::forward<ArgsT>(args)...));
   return _nodes.back();
 }
 
+
 }  // end of namespace tf. ---------------------------------------------------
+
+
+
+
+
+
+
+
+
+
```

### Comparing `rapidfuzz-3.9.0/extern/taskflow/taskflow/core/notifier.hpp` & `rapidfuzz-3.9.1/extern/taskflow/taskflow/core/notifier.hpp`

 * *Files 14% similar despite different names*

```diff
@@ -66,23 +66,28 @@
 
   friend class Executor;
 
   public:
 
   struct Waiter {
     std::atomic<Waiter*> next;
-    std::mutex mu;
-    std::condition_variable cv;
     uint64_t epoch;
-    unsigned state;
-    enum {
-      kNotSignaled,
+    enum : unsigned {
+      kNotSignaled = 0,
       kWaiting,
       kSignaled,
     };
+
+#ifdef __cpp_lib_atomic_wait
+    std::atomic<unsigned> state {0};
+#else
+    std::mutex mu;
+    std::condition_variable cv;
+    unsigned state;
+#endif
   };
 
   explicit Notifier(size_t N) : _waiters{N} {
     assert(_waiters.size() < (1 << kWaiterBits) - 1);
     // Initialize epoch to something close to overflow to test overflow.
     _state = kStackMask | (kEpochMask - kEpochInc * _waiters.size() * 2);
   }
@@ -97,16 +102,21 @@
   // and call either cancel_wait or commit_wait passing the same Waiter object.
   void prepare_wait(Waiter* w) {
     w->epoch = _state.fetch_add(kWaiterInc, std::memory_order_relaxed);
     std::atomic_thread_fence(std::memory_order_seq_cst);
   }
 
   // commit_wait commits waiting.
+  // only the waiter itself can call
   void commit_wait(Waiter* w) {
+#ifdef __cpp_lib_atomic_wait
+    w->state.store(Waiter::kNotSignaled, std::memory_order_relaxed);
+#else
     w->state = Waiter::kNotSignaled;
+#endif
     // Modification epoch of this waiter.
     uint64_t epoch =
         (w->epoch & kEpochMask) +
         (((w->epoch & kWaiterMask) >> kWaiterShift) << kEpochShift);
     uint64_t state = _state.load(std::memory_order_seq_cst);
     for (;;) {
       if (int64_t((state & kEpochMask) - epoch) < 0) {
@@ -133,16 +143,16 @@
     }
     _park(w);
   }
 
   // cancel_wait cancels effects of the previous prepare_wait call.
   void cancel_wait(Waiter* w) {
     uint64_t epoch =
-        (w->epoch & kEpochMask) +
-        (((w->epoch & kWaiterMask) >> kWaiterShift) << kEpochShift);
+      (w->epoch & kEpochMask) +
+      (((w->epoch & kWaiterMask) >> kWaiterShift) << kEpochShift);
     uint64_t state = _state.load(std::memory_order_relaxed);
     for (;;) {
       if (int64_t((state & kEpochMask) - epoch) < 0) {
         // The preceeding waiter has not decided on its fate. Wait until it
         // calls either cancel_wait or commit_wait, or is notified.
         std::this_thread::yield();
         state = _state.load(std::memory_order_relaxed);
@@ -161,43 +171,48 @@
   // notify wakes one or all waiting threads.
   // Must be called after changing the associated wait predicate.
   void notify(bool all) {
     std::atomic_thread_fence(std::memory_order_seq_cst);
     uint64_t state = _state.load(std::memory_order_acquire);
     for (;;) {
       // Easy case: no waiters.
-      if ((state & kStackMask) == kStackMask && (state & kWaiterMask) == 0)
+      if ((state & kStackMask) == kStackMask && (state & kWaiterMask) == 0) {
         return;
+      }
       uint64_t waiters = (state & kWaiterMask) >> kWaiterShift;
       uint64_t newstate;
       if (all) {
         // Reset prewait counter and empty wait list.
         newstate = (state & kEpochMask) + (kEpochInc * waiters) + kStackMask;
       } else if (waiters) {
         // There is a thread in pre-wait state, unblock it.
         newstate = state + kEpochInc - kWaiterInc;
       } else {
         // Pop a waiter from list and unpark it.
         Waiter* w = &_waiters[state & kStackMask];
         Waiter* wnext = w->next.load(std::memory_order_relaxed);
         uint64_t next = kStackMask;
         //if (wnext != nullptr) next = wnext - &_waiters[0];
-        if (wnext != nullptr) next = static_cast<uint64_t>(wnext - &_waiters[0]);
+        if (wnext != nullptr) {
+          next = static_cast<uint64_t>(wnext - &_waiters[0]);
+        }
         // Note: we don't add kEpochInc here. ABA problem on the lock-free stack
         // can't happen because a waiter is re-pushed onto the stack only after
         // it was in the pre-wait state which inevitably leads to epoch
         // increment.
         newstate = (state & kEpochMask) + next;
       }
       if (_state.compare_exchange_weak(state, newstate,
                                        std::memory_order_acquire)) {
         if (!all && waiters) return;  // unblocked pre-wait thread
         if ((state & kStackMask) == kStackMask) return;
         Waiter* w = &_waiters[state & kStackMask];
-        if (!all) w->next.store(nullptr, std::memory_order_relaxed);
+        if (!all) {
+          w->next.store(nullptr, std::memory_order_relaxed);
+        }
         _unpark(w);
         return;
       }
     }
   }
 
   // notify n workers
@@ -233,33 +248,52 @@
   static const uint64_t kEpochShift = 32;
   static const uint64_t kEpochMask = ((1ull << kEpochBits) - 1) << kEpochShift;
   static const uint64_t kEpochInc = 1ull << kEpochShift;
   std::atomic<uint64_t> _state;
   std::vector<Waiter> _waiters;
 
   void _park(Waiter* w) {
+#ifdef __cpp_lib_atomic_wait
+    unsigned target = Waiter::kNotSignaled;
+    if(w->state.compare_exchange_strong(target, Waiter::kWaiting,
+                                        std::memory_order_relaxed,
+                                        std::memory_order_relaxed)) {
+      w->state.wait(Waiter::kWaiting, std::memory_order_relaxed);
+    }
+#else
     std::unique_lock<std::mutex> lock(w->mu);
     while (w->state != Waiter::kSignaled) {
       w->state = Waiter::kWaiting;
       w->cv.wait(lock);
     }
+#endif
   }
 
   void _unpark(Waiter* waiters) {
     Waiter* next = nullptr;
     for (Waiter* w = waiters; w; w = next) {
       next = w->next.load(std::memory_order_relaxed);
+#ifdef __cpp_lib_atomic_wait
+      // We only notify if the other is waiting - this is why we use tri-state
+      // variable instead of binary-state variable (i.e., atomic_flag)
+      // Performance is about 0.1% faster
+      if(w->state.exchange(Waiter::kSignaled, std::memory_order_relaxed) == 
+         Waiter::kWaiting) {
+        w->state.notify_one();
+      }
+#else
       unsigned state;
       {
         std::unique_lock<std::mutex> lock(w->mu);
         state = w->state;
         w->state = Waiter::kSignaled;
       }
       // Avoid notifying if it wasn't waiting.
       if (state == Waiter::kWaiting) w->cv.notify_one();
+#endif
     }
   }
 
 };
```

### Comparing `rapidfuzz-3.9.0/extern/taskflow/taskflow/core/observer.hpp` & `rapidfuzz-3.9.1/extern/taskflow/taskflow/core/observer.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/extern/taskflow/taskflow/core/semaphore.hpp` & `rapidfuzz-3.9.1/extern/taskflow/taskflow/core/semaphore.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/extern/taskflow/taskflow/core/task.hpp` & `rapidfuzz-3.9.1/extern/taskflow/taskflow/core/task.hpp`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 */
 enum class TaskType : int {
   /** @brief placeholder task type */
   PLACEHOLDER = 0,
   /** @brief static task type */
   STATIC,
   /** @brief dynamic (subflow) task type */
-  DYNAMIC,
+  SUBFLOW,
   /** @brief condition task type */
   CONDITION,
   /** @brief module task type */
   MODULE,
   /** @brief asynchronous task type */
   ASYNC,
   /** @brief undefined task type (for internal use only) */
@@ -38,42 +38,42 @@
 /**
 @private
 @brief array of all task types (used for iterating task types)
 */
 inline constexpr std::array<TaskType, 6> TASK_TYPES = {
   TaskType::PLACEHOLDER,
   TaskType::STATIC,
-  TaskType::DYNAMIC,
+  TaskType::SUBFLOW,
   TaskType::CONDITION,
   TaskType::MODULE,
   TaskType::ASYNC,
 };
 
 /**
 @brief convert a task type to a human-readable string
 
 The name of each task type is the litte-case string of its characters.
 
 @code{.cpp}
 TaskType::PLACEHOLDER     ->  "placeholder"
 TaskType::STATIC          ->  "static"
-TaskType::DYNAMIC         ->  "subflow"
+TaskType::SUBFLOW         ->  "subflow"
 TaskType::CONDITION       ->  "condition"
 TaskType::MODULE          ->  "module"
 TaskType::ASYNC           ->  "async"
 @endcode
 */
 inline const char* to_string(TaskType type) {
 
   const char* val;
 
   switch(type) {
     case TaskType::PLACEHOLDER:      val = "placeholder";     break;
     case TaskType::STATIC:           val = "static";          break;
-    case TaskType::DYNAMIC:          val = "subflow";         break;
+    case TaskType::SUBFLOW:          val = "subflow";         break;
     case TaskType::CONDITION:        val = "condition";       break;
     case TaskType::MODULE:           val = "module";          break;
     case TaskType::ASYNC:            val = "async";           break;
     default:                         val = "undefined";       break;
   }
 
   return val;
@@ -85,54 +85,54 @@
 
 /**
 @brief determines if a callable is a dynamic task
 
 A dynamic task is a callable object constructible from std::function<void(Subflow&)>.
 */
 template <typename C>
-constexpr bool is_dynamic_task_v = 
+constexpr bool is_subflow_task_v = 
   std::is_invocable_r_v<void, C, Subflow&> &&
   !std::is_invocable_r_v<void, C, Runtime&>;
 
 /**
 @brief determines if a callable is a condition task
 
 A condition task is a callable object constructible from std::function<int()>
 or std::function<int(tf::Runtime&)>.
 */
 template <typename C>
 constexpr bool is_condition_task_v = 
   (std::is_invocable_r_v<int, C> || std::is_invocable_r_v<int, C, Runtime&>) &&
-  !is_dynamic_task_v<C>;
+  !is_subflow_task_v<C>;
 
 /**
 @brief determines if a callable is a multi-condition task
 
 A multi-condition task is a callable object constructible from
 std::function<tf::SmallVector<int>()> or
 std::function<tf::SmallVector<int>(tf::Runtime&)>.
 */
 template <typename C>
 constexpr bool is_multi_condition_task_v =
   (std::is_invocable_r_v<SmallVector<int>, C> ||
   std::is_invocable_r_v<SmallVector<int>, C, Runtime&>) &&
-  !is_dynamic_task_v<C>;
+  !is_subflow_task_v<C>;
 
 /**
 @brief determines if a callable is a static task
 
 A static task is a callable object constructible from std::function<void()>
 or std::function<void(tf::Runtime&)>.
 */
 template <typename C>
 constexpr bool is_static_task_v =
   (std::is_invocable_r_v<void, C> || std::is_invocable_r_v<void, C, Runtime&>) &&
   !is_condition_task_v<C> &&
   !is_multi_condition_task_v<C> &&
-  !is_dynamic_task_v<C>;
+  !is_subflow_task_v<C>;
 
 // ----------------------------------------------------------------------------
 // Task
 // ----------------------------------------------------------------------------
 
 /**
 @class Task
@@ -303,15 +303,15 @@
       executor.run(taskflow).wait();
     }
     @endcode
 
     @return @c *this
     */
     Task& data(void* data);
-      
+    
     /**
     @brief assigns a priority value to the task
 
     A priority value can be one of the following three levels, 
     tf::TaskPriority::HIGH (numerically equivalent to 0),
     tf::TaskPriority::NORMAL (numerically equivalent to 1), and
     tf::TaskPriority::LOW (numerically equivalent to 2).
@@ -508,15 +508,15 @@
 }
 
 // Function: task_type
 inline TaskType Task::type() const {
   switch(_node->_handle.index()) {
     case Node::PLACEHOLDER:     return TaskType::PLACEHOLDER;
     case Node::STATIC:          return TaskType::STATIC;
-    case Node::DYNAMIC:         return TaskType::DYNAMIC;
+    case Node::SUBFLOW:         return TaskType::SUBFLOW;
     case Node::CONDITION:       return TaskType::CONDITION;
     case Node::MULTI_CONDITION: return TaskType::CONDITION;
     case Node::MODULE:          return TaskType::MODULE;
     case Node::ASYNC:           return TaskType::ASYNC;
     case Node::DEPENDENT_ASYNC: return TaskType::ASYNC;
     default:                    return TaskType::UNDEFINED;
   }
@@ -554,16 +554,16 @@
 // Function: work
 template <typename C>
 Task& Task::work(C&& c) {
 
   if constexpr(is_static_task_v<C>) {
     _node->_handle.emplace<Node::Static>(std::forward<C>(c));
   }
-  else if constexpr(is_dynamic_task_v<C>) {
-    _node->_handle.emplace<Node::Dynamic>(std::forward<C>(c));
+  else if constexpr(is_subflow_task_v<C>) {
+    _node->_handle.emplace<Node::Subflow>(std::forward<C>(c));
   }
   else if constexpr(is_condition_task_v<C>) {
     _node->_handle.emplace<Node::Condition>(std::forward<C>(c));
   }
   else if constexpr(is_multi_condition_task_v<C>) {
     _node->_handle.emplace<Node::MultiCondition>(std::forward<C>(c));
   }
@@ -707,15 +707,15 @@
 }
 
 // Function: type
 inline TaskType TaskView::type() const {
   switch(_node._handle.index()) {
     case Node::PLACEHOLDER:     return TaskType::PLACEHOLDER;
     case Node::STATIC:          return TaskType::STATIC;
-    case Node::DYNAMIC:         return TaskType::DYNAMIC;
+    case Node::SUBFLOW:         return TaskType::SUBFLOW;
     case Node::CONDITION:       return TaskType::CONDITION;
     case Node::MULTI_CONDITION: return TaskType::CONDITION;
     case Node::MODULE:          return TaskType::MODULE;
     case Node::ASYNC:           return TaskType::ASYNC;
     case Node::DEPENDENT_ASYNC: return TaskType::ASYNC;
     default:                    return TaskType::UNDEFINED;
   }
@@ -738,15 +738,15 @@
 template <typename V>
 void TaskView::for_each_dependent(V&& visitor) const {
   for(size_t i=0; i<_node._dependents.size(); ++i) {
     visitor(TaskView(*_node._dependents[i]));
   }
 }
 
-}  // end of namespace tf. ---------------------------------------------------
+}  // end of namespace tf. ----------------------------------------------------
 
 namespace std {
 
 /**
 @struct hash
 
 @brief hash specialization for std::hash<tf::Task>
```

### Comparing `rapidfuzz-3.9.0/extern/taskflow/taskflow/core/taskflow.hpp` & `rapidfuzz-3.9.1/extern/taskflow/taskflow/core/taskflow.hpp`

 * *Files 8% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 A %taskflow manages a task dependency graph where each task represents a
 callable object (e.g., @std_lambda, @std_function) and an edge represents a
 dependency between two tasks. A task is one of the following types:
 
   1. static task         : the callable constructible from
                            @c std::function<void()>
-  2. dynamic task        : the callable constructible from
+  2. subflow task        : the callable constructible from
                            @c std::function<void(tf::Subflow&)>
   3. condition task      : the callable constructible from
                            @c std::function<int()>
   4. multi-condition task: the callable constructible from
                            @c %std::function<tf::SmallVector<int>()>
   5. module task         : the task constructed from tf::Taskflow::composed_of
                            @c std::function<void(tf::Runtime&)>
@@ -243,14 +243,40 @@
     });
     @endcode
     */
     template <typename V>
     void for_each_task(V&& visitor) const;
 
     /**
+    @brief removes dependencies that go from task @c from to task @c to
+
+    @param from from task (dependent)
+    @param to to task (successor)
+  
+    @code{.cpp}
+    tf::Taskflow taskflow;
+    auto a = taskflow.placeholder().name("a");
+    auto b = taskflow.placeholder().name("b");
+    auto c = taskflow.placeholder().name("c");
+    auto d = taskflow.placeholder().name("d");
+
+    a.precede(b, c, d);
+    assert(a.num_successors() == 3);
+    assert(b.num_dependents() == 1);
+    assert(c.num_dependents() == 1);
+    assert(d.num_dependents() == 1);
+  
+    taskflow.remove_dependency(a, b);
+    assert(a.num_successors() == 2);
+    assert(b.num_dependents() == 0);
+    @endcode
+    */
+    inline void remove_dependency(Task from, Task to);
+
+    /**
     @brief returns a reference to the underlying graph object
 
     A graph object (of type tf::Graph) is the ultimate storage for the
     task dependency graph and should only be used as an opaque
     data structure to interact with the executor (e.g., composition).
     */
     Graph& graph();
@@ -260,15 +286,14 @@
     mutable std::mutex _mutex;
 
     std::string _name;
 
     Graph _graph;
 
     std::queue<std::shared_ptr<Topology>> _topologies;
-
     std::optional<std::list<Taskflow>::iterator> _satellite;
 
     void _dump(std::ostream&, const Graph*) const;
     void _dump(std::ostream&, const Node*, Dumper&) const;
     void _dump(std::ostream&, const Graph*, Dumper&) const;
 };
 
@@ -342,14 +367,29 @@
 template <typename V>
 void Taskflow::for_each_task(V&& visitor) const {
   for(size_t i=0; i<_graph._nodes.size(); ++i) {
     visitor(Task(_graph._nodes[i]));
   }
 }
 
+// Procedure: remove_dependency
+inline void Taskflow::remove_dependency(Task from, Task to) {
+  from._node->_successors.erase(std::remove_if(
+    from._node->_successors.begin(), from._node->_successors.end(), [&](Node* i){
+      return i == to._node;
+    }
+  ), from._node->_successors.end());
+  
+  to._node->_dependents.erase(std::remove_if(
+    to._node->_dependents.begin(), to._node->_dependents.end(), [&](Node* i){
+      return i == from._node;
+    }
+  ), to._node->_dependents.end());
+}
+
 // Procedure: dump
 inline std::string Taskflow::dump() const {
   std::ostringstream oss;
   dump(oss);
   return oss.str();
 }
 
@@ -425,25 +465,25 @@
          << " [style=dashed label=\"" << s << "\"];\n";
     } else {
       os << 'p' << node << " -> p" << node->_successors[s] << ";\n";
     }
   }
 
   // subflow join node
-  if(node->_parent && node->_parent->_handle.index() == Node::DYNAMIC &&
+  if(node->_parent && node->_parent->_handle.index() == Node::SUBFLOW &&
      node->_successors.size() == 0
     ) {
     os << 'p' << node << " -> p" << node->_parent << ";\n";
   }
 
   // node info
   switch(node->_handle.index()) {
 
-    case Node::DYNAMIC: {
-      auto& sbg = std::get_if<Node::Dynamic>(&node->_handle)->subgraph;
+    case Node::SUBFLOW: {
+      auto& sbg = std::get_if<Node::Subflow>(&node->_handle)->subgraph;
       if(!sbg.empty()) {
         os << "subgraph cluster_p" << node << " {\nlabel=\"Subflow: ";
         if(node->_name.empty()) os << 'p' << node;
         else os << node->_name;
 
         os << "\";\n" << "color=blue\n";
         _dump(os, &sbg, dumper);
@@ -498,15 +538,14 @@
 /**
 @class Future
 
 @brief class to access the result of an execution
 
 tf::Future is a derived class from std::future that will eventually hold the
 execution result of a submitted taskflow (tf::Executor::run)
-or an asynchronous task (tf::Executor::async, tf::Executor::silent_async).
 In addition to the base methods inherited from std::future,
 you can call tf::Future::cancel to cancel the execution of the running taskflow
 associated with this future object.
 The following example cancels a submission of a taskflow that contains
 1000 tasks each running one second.
 
 @code{.cpp}
@@ -532,18 +571,14 @@
 template <typename T>
 class Future : public std::future<T>  {
 
   friend class Executor;
   friend class Subflow;
   friend class Runtime;
 
-  using handle_t = std::variant<
-    std::monostate, std::weak_ptr<Topology>
-  >;
-
   public:
 
     /**
     @brief default constructor
     */
     Future() = default;
 
@@ -578,42 +613,31 @@
     any tasks onwards. Tasks that are already running will continue to finish
     (non-preemptive).
     You can call tf::Future::wait to wait for the cancellation to complete.
     */
     bool cancel();
 
   private:
+    
+    std::weak_ptr<Topology> _topology;
 
-    handle_t _handle;
-
-    template <typename P>
-    Future(std::future<T>&&, P&&);
+    Future(std::future<T>&&, std::weak_ptr<Topology> = std::weak_ptr<Topology>());
 };
 
 template <typename T>
-template <typename P>
-Future<T>::Future(std::future<T>&& fu, P&& p) :
-  std::future<T> {std::move(fu)},
-  _handle        {std::forward<P>(p)} {
+Future<T>::Future(std::future<T>&& f, std::weak_ptr<Topology> p) :
+  std::future<T> {std::move(f)},
+  _topology      {std::move(p)} {
 }
 
 // Function: cancel
 template <typename T>
 bool Future<T>::cancel() {
-  return std::visit([](auto&& arg){
-    using P = std::decay_t<decltype(arg)>;
-    if constexpr(std::is_same_v<P, std::monostate>) {
-      return false;
-    }
-    else {
-      auto ptr = arg.lock();
-      if(ptr) {
-        ptr->_is_cancelled.store(true, std::memory_order_relaxed);
-        return true;
-      }
-      return false;
-    }
-  }, _handle);
+  if(auto ptr = _topology.lock(); ptr) {
+    ptr->_state.fetch_or(Topology::CANCELLED, std::memory_order_relaxed);
+    return true;
+  }
+  return false;
 }
 
 
 }  // end of namespace tf. ---------------------------------------------------
```

### Comparing `rapidfuzz-3.9.0/extern/taskflow/taskflow/core/tsq.hpp` & `rapidfuzz-3.9.1/extern/taskflow/taskflow/core/tsq.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/extern/taskflow/taskflow/core/worker.hpp` & `rapidfuzz-3.9.1/extern/taskflow/taskflow/core/worker.hpp`

 * *Files 26% similar despite different names*

```diff
@@ -163,98 +163,10 @@
 
 // Function: queue_capacity
 inline size_t WorkerView::queue_capacity() const {
   return static_cast<size_t>(_worker._wsq.capacity());
 }
 
 
-// ----------------------------------------------------------------------------
-// Class Definition: WorkerInterface
-// ----------------------------------------------------------------------------
-
-/**
-@class WorkerInterface
-
-@brief class to configure worker behavior in an executor
-
-The tf::WorkerInterface class lets users interact with the executor
-to customize the worker behavior,
-such as calling custom methods before and after a worker enters and leaves
-the loop.
-When you create an executor, it spawns a set of workers to run tasks.
-The interaction between the executor and its spawned workers looks like
-the following:
-
-for(size_t n=0; n<num_workers; n++) {
-  create_thread([](Worker& worker)
-  
-    // pre-processing executor-specific worker information
-    // ...
-  
-    // enter the scheduling loop
-    // Here, WorkerInterface::scheduler_prologue is invoked, if any
-    
-    while(1) {
-      perform_work_stealing_algorithm();
-      if(stop) {
-        break; 
-      }
-    }
-  
-    // leaves the scheduling loop and joins this worker thread
-    // Here, WorkerInterface::scheduler_epilogue is invoked, if any
-  );
-}
-
-@note
-Methods defined in tf::WorkerInterface are not thread-safe and may be
-be invoked by multiple workers concurrently.
-
-*/
-class WorkerInterface {
-
-  public:
-  
-  /**
-  @brief default destructor
-  */
-  virtual ~WorkerInterface() = default;
-  
-  /**
-  @brief method to call before a worker enters the scheduling loop
-  @param worker a reference to the worker
-
-  The method is called by the constructor of an executor.
-  */
-  virtual void scheduler_prologue(Worker& worker) = 0;
-  
-  /**
-  @brief method to call after a worker leaves the scheduling loop
-  @param worker a reference to the worker
-  @param ptr an pointer to the exception thrown by the scheduling loop
-
-  The method is called by the constructor of an executor.
-  */
-  virtual void scheduler_epilogue(Worker& worker, std::exception_ptr ptr) = 0;
-
-};
-
-/**
-@brief helper function to create an instance derived from tf::WorkerInterface
-
-@tparam T type derived from tf::WorkerInterface
-@tparam ArgsT argument types to construct @c T
-
-@param args arguments to forward to the constructor of @c T
-*/
-template <typename T, typename... ArgsT>
-std::shared_ptr<T> make_worker_interface(ArgsT&&... args) {
-  static_assert(
-    std::is_base_of_v<WorkerInterface, T>, 
-    "T must be derived from WorkerInterface"
-  );
-  return std::make_shared<T>(std::forward<ArgsT>(args)...);
-}
-
 }  // end of namespact tf -----------------------------------------------------
```

### Comparing `rapidfuzz-3.9.0/extern/taskflow/taskflow/taskflow.hpp` & `rapidfuzz-3.9.1/extern/taskflow/taskflow/taskflow.hpp`

 * *Files 10% similar despite different names*

```diff
@@ -29,16 +29,16 @@
 @brief main taskflow include file
 */
 
 // TF_VERSION % 100 is the patch level
 // TF_VERSION / 100 % 1000 is the minor version
 // TF_VERSION / 100000 is the major version
 
-// current version: 3.6.0
-#define TF_VERSION 300600
+// current version: 3.7.0
+#define TF_VERSION 300700
 
 #define TF_MAJOR_VERSION TF_VERSION/100000
 #define TF_MINOR_VERSION TF_VERSION/100%1000
 #define TF_PATCH_VERSION TF_VERSION%100
 
 /**
 @brief taskflow namespace
@@ -53,15 +53,15 @@
 
 /**
 @brief queries the version information in a string format @c major.minor.patch
 
 Release notes are available here: https://taskflow.github.io/taskflow/Releases.html
 */
 constexpr const char* version() {
-  return "3.6.0";
+  return "3.7.0";
 }
 
 
 }  // end of namespace tf -----------------------------------------------------
```

### Comparing `rapidfuzz-3.9.0/extern/taskflow/taskflow/utility/iterator.hpp` & `rapidfuzz-3.9.1/extern/taskflow/taskflow/utility/iterator.hpp`

 * *Files 15% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 
 namespace tf {
 
 template <typename T>
 constexpr std::enable_if_t<std::is_integral<std::decay_t<T>>::value, bool>
 is_range_invalid(T beg, T end, T step) {
   return ((step == 0 && beg != end) ||
-          (beg < end && step <=  0) ||
-          (beg > end && step >=  0));
+          (beg < end && step <=  0) ||  // positive range
+          (beg > end && step >=  0));   // negative range
 }
 
 template <typename T>
 constexpr std::enable_if_t<std::is_integral<std::decay_t<T>>::value, size_t>
 distance(T beg, T end, T step) {
   return (end - beg + step + (step > 0 ? -1 : 1)) / step;
 }
```

### Comparing `rapidfuzz-3.9.0/extern/taskflow/taskflow/utility/math.hpp` & `rapidfuzz-3.9.1/extern/taskflow/taskflow/utility/math.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/extern/taskflow/taskflow/utility/object_pool.hpp` & `rapidfuzz-3.9.1/extern/taskflow/taskflow/utility/object_pool.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/extern/taskflow/taskflow/utility/os.hpp` & `rapidfuzz-3.9.1/extern/taskflow/taskflow/utility/os.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/extern/taskflow/taskflow/utility/serializer.hpp` & `rapidfuzz-3.9.1/extern/taskflow/taskflow/utility/serializer.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/extern/taskflow/taskflow/utility/singleton.hpp` & `rapidfuzz-3.9.1/extern/taskflow/taskflow/utility/singleton.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/extern/taskflow/taskflow/utility/small_vector.hpp` & `rapidfuzz-3.9.1/extern/taskflow/taskflow/utility/small_vector.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/extern/taskflow/taskflow/utility/stream.hpp` & `rapidfuzz-3.9.1/extern/taskflow/taskflow/utility/stream.hpp`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 #pragma once
 
 #include <iostream>
+#include <sstream>
 #include <string>
 
 namespace tf {
 
 // Procedure: ostreamize
 template <typename T>
 void ostreamize(std::ostream& os, T&& token) {
```

### Comparing `rapidfuzz-3.9.0/extern/taskflow/taskflow/utility/traits.hpp` & `rapidfuzz-3.9.1/extern/taskflow/taskflow/utility/traits.hpp`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 #pragma once
 
+#if __has_include(<version>)
+#  include <version>
+#endif
+
 #include <type_traits>
 #include <iterator>
 #include <iostream>
 #include <fstream>
 #include <mutex>
 #include <stack>
 #include <queue>
```

### Comparing `rapidfuzz-3.9.0/extern/taskflow/taskflow/utility/uuid.hpp` & `rapidfuzz-3.9.1/extern/taskflow/taskflow/utility/uuid.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/pyproject.toml` & `rapidfuzz-3.9.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/setup.py` & `rapidfuzz-3.9.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 
 with open("README.md", encoding="utf8") as f:
     readme = f.read()
 
 setup_args = {
     "name": "rapidfuzz",
-    "version": "3.9.0",
+    "version": "3.9.1",
     "extras_require": {"full": ["numpy"]},
     "url": "https://github.com/rapidfuzz/RapidFuzz",
     "author": "Max Bachmann",
     "author_email": "pypi@maxbachmann.de",
     "description": "rapid fuzzy string matching",
     "long_description": readme,
     "long_description_content_type": "text/markdown",
```

### Comparing `rapidfuzz-3.9.0/src/rapidfuzz/CMakeLists.txt` & `rapidfuzz-3.9.1/src/rapidfuzz/CMakeLists.txt`

 * *Files 2% similar despite different names*

```diff
@@ -53,27 +53,30 @@
 rf_add_library(fuzz_cpp ${fuzz_cpp})
 target_compile_features(fuzz_cpp PUBLIC cxx_std_17)
 target_include_directories(fuzz_cpp PRIVATE ${RF_BASE_DIR}/rapidfuzz)
 target_link_libraries(fuzz_cpp PRIVATE rapidfuzz::rapidfuzz)
 install(TARGETS fuzz_cpp LIBRARY DESTINATION src/rapidfuzz)
 
 if(RAPIDFUZZ_ARCH_X64 OR RAPIDFUZZ_ARCH_X86)
-  create_cython_target(fuzz_cpp_avx2)
-  rf_add_library(fuzz_cpp_avx2 ${fuzz_cpp_avx2})
-  target_compile_features(fuzz_cpp_avx2 PUBLIC cxx_std_17)
+  # on macOs this generates illegal instructions https://github.com/rapidfuzz/RapidFuzz/issues/383
+  if(NOT APPLE)
+    create_cython_target(fuzz_cpp_avx2)
+    rf_add_library(fuzz_cpp_avx2 ${fuzz_cpp_avx2})
+    target_compile_features(fuzz_cpp_avx2 PUBLIC cxx_std_17)
 
-  if(MSVC)
-    set_target_properties(fuzz_cpp_avx2 PROPERTIES COMPILE_FLAGS "/arch:AVX2")
-  else()
-    set_target_properties(fuzz_cpp_avx2 PROPERTIES COMPILE_FLAGS "-mavx2")
-  endif()
+    if(MSVC)
+      set_target_properties(fuzz_cpp_avx2 PROPERTIES COMPILE_FLAGS "/arch:AVX2")
+    else()
+      set_target_properties(fuzz_cpp_avx2 PROPERTIES COMPILE_FLAGS "-mavx2")
+    endif()
 
-  target_include_directories(fuzz_cpp_avx2 PRIVATE ${RF_BASE_DIR}/rapidfuzz)
-  target_link_libraries(fuzz_cpp_avx2 PRIVATE rapidfuzz::rapidfuzz)
-  install(TARGETS fuzz_cpp_avx2 LIBRARY DESTINATION src/rapidfuzz)
+    target_include_directories(fuzz_cpp_avx2 PRIVATE ${RF_BASE_DIR}/rapidfuzz)
+    target_link_libraries(fuzz_cpp_avx2 PRIVATE rapidfuzz::rapidfuzz)
+    install(TARGETS fuzz_cpp_avx2 LIBRARY DESTINATION src/rapidfuzz)
+  endif()
 endif()
 
 if(RAPIDFUZZ_ARCH_X86)
   create_cython_target(fuzz_cpp_sse2)
   rf_add_library(fuzz_cpp_sse2 ${fuzz_cpp_sse2})
   target_compile_features(fuzz_cpp_sse2 PUBLIC cxx_std_17)
```

### Comparing `rapidfuzz-3.9.0/src/rapidfuzz/FeatureDetector/CpuInfo.cpp` & `rapidfuzz-3.9.1/src/rapidfuzz/FeatureDetector/CpuInfo.cpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/src/rapidfuzz/FeatureDetector/CpuInfo.hpp` & `rapidfuzz-3.9.1/src/rapidfuzz/FeatureDetector/CpuInfo.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/src/rapidfuzz/__init__.pxd` & `rapidfuzz-3.9.1/src/rapidfuzz/__init__.pxd`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/src/rapidfuzz/__init__.py` & `rapidfuzz-3.9.1/src/rapidfuzz/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 rapid string matching library
 """
 
 from __future__ import annotations
 
 __author__: str = "Max Bachmann"
 __license__: str = "MIT"
-__version__: str = "3.9.0"
+__version__: str = "3.9.1"
 
 from rapidfuzz import distance, fuzz, process, utils
 
 __all__ = ["distance", "fuzz", "process", "utils", "get_include"]
 
 
 def get_include():
```

### Comparing `rapidfuzz-3.9.0/src/rapidfuzz/__pyinstaller/test_rapidfuzz_packaging.py` & `rapidfuzz-3.9.1/src/rapidfuzz/__pyinstaller/test_rapidfuzz_packaging.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/src/rapidfuzz/_common_py.py` & `rapidfuzz-3.9.1/src/rapidfuzz/_common_py.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/src/rapidfuzz/_feature_detector_cpp.cxx` & `rapidfuzz-3.9.1/src/rapidfuzz/_feature_detector_cpp.cxx`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/src/rapidfuzz/_utils.py` & `rapidfuzz-3.9.1/src/rapidfuzz/_utils.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/src/rapidfuzz/cpp_common.hpp` & `rapidfuzz-3.9.1/src/rapidfuzz/cpp_common.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/src/rapidfuzz/cpp_common.pxd` & `rapidfuzz-3.9.1/src/rapidfuzz/cpp_common.pxd`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/src/rapidfuzz/distance/CMakeLists.txt` & `rapidfuzz-3.9.1/src/rapidfuzz/distance/CMakeLists.txt`

 * *Files 10% similar despite different names*

```diff
@@ -47,30 +47,33 @@
 target_include_directories(
   metrics_cpp PRIVATE ${RF_BASE_DIR}/rapidfuzz
                       ${RF_BASE_DIR}/rapidfuzz/distance)
 target_link_libraries(metrics_cpp PRIVATE rapidfuzz::rapidfuzz)
 install(TARGETS metrics_cpp LIBRARY DESTINATION src/rapidfuzz/distance)
 
 if(RAPIDFUZZ_ARCH_X64 OR RAPIDFUZZ_ARCH_X86)
-  create_cython_target(metrics_cpp_avx2)
-  rf_add_library(metrics_cpp_avx2 ${metrics_cpp_avx2})
-  target_compile_features(metrics_cpp_avx2 PUBLIC cxx_std_17)
+  # on macOs this generates illegal instructions https://github.com/rapidfuzz/RapidFuzz/issues/383
+  if(NOT APPLE)
+    create_cython_target(metrics_cpp_avx2)
+    rf_add_library(metrics_cpp_avx2 ${metrics_cpp_avx2})
+    target_compile_features(metrics_cpp_avx2 PUBLIC cxx_std_17)
 
-  if(MSVC)
-    set_target_properties(metrics_cpp_avx2 PROPERTIES COMPILE_FLAGS
-                                                      "/arch:AVX2")
-  else()
-    set_target_properties(metrics_cpp_avx2 PROPERTIES COMPILE_FLAGS "-mavx2")
-  endif()
+    if(MSVC)
+      set_target_properties(metrics_cpp_avx2 PROPERTIES COMPILE_FLAGS
+                                                        "/arch:AVX2")
+    else()
+      set_target_properties(metrics_cpp_avx2 PROPERTIES COMPILE_FLAGS "-mavx2")
+    endif()
 
-  target_include_directories(
-    metrics_cpp_avx2 PRIVATE ${RF_BASE_DIR}/rapidfuzz
-                             ${RF_BASE_DIR}/rapidfuzz/distance)
-  target_link_libraries(metrics_cpp_avx2 PRIVATE rapidfuzz::rapidfuzz)
-  install(TARGETS metrics_cpp_avx2 LIBRARY DESTINATION src/rapidfuzz/distance)
+    target_include_directories(
+      metrics_cpp_avx2 PRIVATE ${RF_BASE_DIR}/rapidfuzz
+                              ${RF_BASE_DIR}/rapidfuzz/distance)
+    target_link_libraries(metrics_cpp_avx2 PRIVATE rapidfuzz::rapidfuzz)
+    install(TARGETS metrics_cpp_avx2 LIBRARY DESTINATION src/rapidfuzz/distance)
+  endif()
 endif()
 
 if(RAPIDFUZZ_ARCH_X86)
   create_cython_target(metrics_cpp_sse2)
   rf_add_library(metrics_cpp_sse2 ${metrics_cpp_sse2})
   target_compile_features(metrics_cpp_sse2 PUBLIC cxx_std_17)
```

### Comparing `rapidfuzz-3.9.0/src/rapidfuzz/distance/DamerauLevenshtein.py` & `rapidfuzz-3.9.1/src/rapidfuzz/distance/DamerauLevenshtein.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/src/rapidfuzz/distance/DamerauLevenshtein.pyi` & `rapidfuzz-3.9.1/src/rapidfuzz/distance/DamerauLevenshtein.pyi`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/src/rapidfuzz/distance/DamerauLevenshtein_py.py` & `rapidfuzz-3.9.1/src/rapidfuzz/distance/DamerauLevenshtein_py.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/src/rapidfuzz/distance/Hamming.py` & `rapidfuzz-3.9.1/src/rapidfuzz/distance/Hamming.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/src/rapidfuzz/distance/Hamming.pyi` & `rapidfuzz-3.9.1/src/rapidfuzz/distance/Hamming.pyi`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/src/rapidfuzz/distance/Hamming_py.py` & `rapidfuzz-3.9.1/src/rapidfuzz/distance/Hamming_py.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/src/rapidfuzz/distance/Indel.py` & `rapidfuzz-3.9.1/src/rapidfuzz/distance/Indel.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/src/rapidfuzz/distance/Indel.pyi` & `rapidfuzz-3.9.1/src/rapidfuzz/distance/Indel.pyi`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/src/rapidfuzz/distance/Indel_py.py` & `rapidfuzz-3.9.1/src/rapidfuzz/distance/Indel_py.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/src/rapidfuzz/distance/Jaro.pyi` & `rapidfuzz-3.9.1/src/rapidfuzz/distance/Jaro.pyi`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/src/rapidfuzz/distance/JaroWinkler.pyi` & `rapidfuzz-3.9.1/src/rapidfuzz/distance/JaroWinkler.pyi`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/src/rapidfuzz/distance/JaroWinkler_py.py` & `rapidfuzz-3.9.1/src/rapidfuzz/distance/JaroWinkler_py.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/src/rapidfuzz/distance/Jaro_py.py` & `rapidfuzz-3.9.1/src/rapidfuzz/distance/Jaro_py.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/src/rapidfuzz/distance/LCSseq.py` & `rapidfuzz-3.9.1/src/rapidfuzz/distance/LCSseq.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/src/rapidfuzz/distance/LCSseq.pyi` & `rapidfuzz-3.9.1/src/rapidfuzz/distance/LCSseq.pyi`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/src/rapidfuzz/distance/LCSseq_py.py` & `rapidfuzz-3.9.1/src/rapidfuzz/distance/LCSseq_py.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/src/rapidfuzz/distance/Levenshtein.py` & `rapidfuzz-3.9.1/src/rapidfuzz/distance/Levenshtein.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/src/rapidfuzz/distance/Levenshtein.pyi` & `rapidfuzz-3.9.1/src/rapidfuzz/distance/Levenshtein.pyi`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/src/rapidfuzz/distance/Levenshtein_py.py` & `rapidfuzz-3.9.1/src/rapidfuzz/distance/Levenshtein_py.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/src/rapidfuzz/distance/OSA.pyi` & `rapidfuzz-3.9.1/src/rapidfuzz/distance/OSA.pyi`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/src/rapidfuzz/distance/OSA_py.py` & `rapidfuzz-3.9.1/src/rapidfuzz/distance/OSA_py.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/src/rapidfuzz/distance/Postfix.pyi` & `rapidfuzz-3.9.1/src/rapidfuzz/distance/Postfix.pyi`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/src/rapidfuzz/distance/Postfix_py.py` & `rapidfuzz-3.9.1/src/rapidfuzz/distance/Postfix_py.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/src/rapidfuzz/distance/Prefix.pyi` & `rapidfuzz-3.9.1/src/rapidfuzz/distance/Prefix.pyi`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/src/rapidfuzz/distance/Prefix_py.py` & `rapidfuzz-3.9.1/src/rapidfuzz/distance/Prefix_py.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/src/rapidfuzz/distance/__init__.py` & `rapidfuzz-3.9.1/src/rapidfuzz/distance/__init__.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/src/rapidfuzz/distance/__init__.pyi` & `rapidfuzz-3.9.1/src/rapidfuzz/distance/__init__.pyi`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/src/rapidfuzz/distance/_initialize.py` & `rapidfuzz-3.9.1/src/rapidfuzz/distance/_initialize.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/src/rapidfuzz/distance/_initialize.pyi` & `rapidfuzz-3.9.1/src/rapidfuzz/distance/_initialize.pyi`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/src/rapidfuzz/distance/_initialize_cpp.cxx` & `rapidfuzz-3.9.1/src/rapidfuzz/distance/_initialize_cpp.cxx`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/src/rapidfuzz/distance/_initialize_cpp.pyx` & `rapidfuzz-3.9.1/src/rapidfuzz/distance/_initialize_cpp.pyx`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/src/rapidfuzz/distance/_initialize_py.py` & `rapidfuzz-3.9.1/src/rapidfuzz/distance/_initialize_py.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/src/rapidfuzz/distance/metrics.hpp` & `rapidfuzz-3.9.1/src/rapidfuzz/distance/metrics.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/src/rapidfuzz/distance/metrics_cpp.cxx` & `rapidfuzz-3.9.1/src/rapidfuzz/distance/metrics_cpp.cxx`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/src/rapidfuzz/distance/metrics_cpp.pyx` & `rapidfuzz-3.9.1/src/rapidfuzz/distance/metrics_cpp.pyx`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/src/rapidfuzz/distance/metrics_cpp_avx2.cxx` & `rapidfuzz-3.9.1/src/rapidfuzz/distance/metrics_cpp_avx2.cxx`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/src/rapidfuzz/distance/metrics_cpp_sse2.cxx` & `rapidfuzz-3.9.1/src/rapidfuzz/distance/metrics_cpp_sse2.cxx`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/src/rapidfuzz/distance/metrics_py.py` & `rapidfuzz-3.9.1/src/rapidfuzz/distance/metrics_py.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/src/rapidfuzz/fuzz.py` & `rapidfuzz-3.9.1/src/rapidfuzz/fuzz.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/src/rapidfuzz/fuzz.pyi` & `rapidfuzz-3.9.1/src/rapidfuzz/fuzz.pyi`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/src/rapidfuzz/fuzz_cpp.cxx` & `rapidfuzz-3.9.1/src/rapidfuzz/fuzz_cpp.cxx`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/src/rapidfuzz/fuzz_cpp.hpp` & `rapidfuzz-3.9.1/src/rapidfuzz/fuzz_cpp.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/src/rapidfuzz/fuzz_cpp.pyx` & `rapidfuzz-3.9.1/src/rapidfuzz/fuzz_cpp.pyx`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/src/rapidfuzz/fuzz_cpp_avx2.cxx` & `rapidfuzz-3.9.1/src/rapidfuzz/fuzz_cpp_avx2.cxx`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/src/rapidfuzz/fuzz_cpp_sse2.cxx` & `rapidfuzz-3.9.1/src/rapidfuzz/fuzz_cpp_sse2.cxx`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/src/rapidfuzz/fuzz_py.py` & `rapidfuzz-3.9.1/src/rapidfuzz/fuzz_py.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/src/rapidfuzz/process.pyi` & `rapidfuzz-3.9.1/src/rapidfuzz/process.pyi`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/src/rapidfuzz/process_cpp.hpp` & `rapidfuzz-3.9.1/src/rapidfuzz/process_cpp.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/src/rapidfuzz/process_cpp.py` & `rapidfuzz-3.9.1/src/rapidfuzz/process_cpp.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/src/rapidfuzz/process_cpp_impl.cxx` & `rapidfuzz-3.9.1/src/rapidfuzz/process_cpp_impl.cxx`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/src/rapidfuzz/process_cpp_impl.pyx` & `rapidfuzz-3.9.1/src/rapidfuzz/process_cpp_impl.pyx`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/src/rapidfuzz/process_py.py` & `rapidfuzz-3.9.1/src/rapidfuzz/process_py.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/src/rapidfuzz/rapidfuzz.h` & `rapidfuzz-3.9.1/src/rapidfuzz/rapidfuzz.h`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/src/rapidfuzz/unicodetype_db.h` & `rapidfuzz-3.9.1/src/rapidfuzz/unicodetype_db.h`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/src/rapidfuzz/utils.cpp` & `rapidfuzz-3.9.1/src/rapidfuzz/utils.cpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/src/rapidfuzz/utils.hpp` & `rapidfuzz-3.9.1/src/rapidfuzz/utils.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/src/rapidfuzz/utils_cpp.cxx` & `rapidfuzz-3.9.1/src/rapidfuzz/utils_cpp.cxx`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/src/rapidfuzz/utils_cpp.hpp` & `rapidfuzz-3.9.1/src/rapidfuzz/utils_cpp.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/src/rapidfuzz/utils_cpp.pyx` & `rapidfuzz-3.9.1/src/rapidfuzz/utils_cpp.pyx`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/src/rapidfuzz/utils_py.py` & `rapidfuzz-3.9.1/src/rapidfuzz/utils_py.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/src/rapidfuzz.egg-info/PKG-INFO` & `rapidfuzz-3.9.1/src/rapidfuzz.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rapidfuzz
-Version: 3.9.0
+Version: 3.9.1
 Summary: rapid fuzzy string matching
 Home-page: https://github.com/rapidfuzz/RapidFuzz
 Author: Max Bachmann
 Author-email: pypi@maxbachmann.de
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: rapidfuzz Version: 3.9.0 Summary: rapid fuzzy
+Metadata-Version: 2.1 Name: rapidfuzz Version: 3.9.1 Summary: rapid fuzzy
 string matching Home-page: https://github.com/rapidfuzz/RapidFuzz Author: Max
 Bachmann Author-email: pypi@maxbachmann.de License: MIT Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12 Classifier: License :: OSI
 Approved :: MIT License Requires-Python: >=3.8 Description-Content-Type: text/
```

### Comparing `rapidfuzz-3.9.0/src/rapidfuzz.egg-info/SOURCES.txt` & `rapidfuzz-3.9.1/src/rapidfuzz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/tests/common.py` & `rapidfuzz-3.9.1/tests/common.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/tests/distance/common.py` & `rapidfuzz-3.9.1/tests/distance/common.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/tests/distance/test_DamerauLevenshtein.py` & `rapidfuzz-3.9.1/tests/distance/test_DamerauLevenshtein.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/tests/distance/test_Hamming.py` & `rapidfuzz-3.9.1/tests/distance/test_Hamming.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/tests/distance/test_Indel.py` & `rapidfuzz-3.9.1/tests/distance/test_Indel.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/tests/distance/test_Jaro.py` & `rapidfuzz-3.9.1/tests/distance/test_Jaro.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/tests/distance/test_JaroWinkler.py` & `rapidfuzz-3.9.1/tests/distance/test_JaroWinkler.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/tests/distance/test_LCSseq.py` & `rapidfuzz-3.9.1/tests/distance/test_LCSseq.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/tests/distance/test_Levenshtein.py` & `rapidfuzz-3.9.1/tests/distance/test_Levenshtein.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/tests/distance/test_OSA.py` & `rapidfuzz-3.9.1/tests/distance/test_OSA.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/tests/distance/test_Postfix.py` & `rapidfuzz-3.9.1/tests/distance/test_Postfix.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/tests/distance/test_Prefix.py` & `rapidfuzz-3.9.1/tests/distance/test_Prefix.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/tests/distance/test_distance.py` & `rapidfuzz-3.9.1/tests/distance/test_distance.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/tests/distance/test_init.py` & `rapidfuzz-3.9.1/tests/distance/test_init.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/tests/test_fuzz.py` & `rapidfuzz-3.9.1/tests/test_fuzz.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/tests/test_hypothesis.py` & `rapidfuzz-3.9.1/tests/test_hypothesis.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/tests/test_process.py` & `rapidfuzz-3.9.1/tests/test_process.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.0/tests/test_utils.py` & `rapidfuzz-3.9.1/tests/test_utils.py`

 * *Files identical despite different names*

