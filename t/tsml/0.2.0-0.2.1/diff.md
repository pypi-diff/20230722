# Comparing `tmp/tsml-0.2.0.tar.gz` & `tmp/tsml-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tsml-0.2.0.tar", last modified: Fri Jul 21 13:23:30 2023, max compression
+gzip compressed data, was "tsml-0.2.1.tar", last modified: Sat Jul 22 15:43:35 2023, max compression
```

## Comparing `tsml-0.2.0.tar` & `tsml-0.2.1.tar`

### file list

```diff
@@ -1,124 +1,125 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:23:30.817438 tsml-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-07-21 13:23:15.000000 tsml-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-21 13:23:15.000000 tsml-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-07-21 13:23:30.817438 tsml-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-21 13:23:15.000000 tsml-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-07-21 13:23:15.000000 tsml-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 13:23:30.817438 tsml-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:23:30.793438 tsml-0.2.0/tsml/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11349 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:23:30.797438 tsml-0.2.0/tsml/compose/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/compose/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20638 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/compose/_channel_ensemble.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:23:30.797438 tsml-0.2.0/tsml/compose/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/compose/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/compose/tests/test_channel_ensemble.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:23:30.797438 tsml-0.2.0/tsml/datasets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:23:30.797438 tsml-0.2.0/tsml/datasets/EqualMinimalJapaneseVowels/
--rw-r--r--   0 runner    (1001) docker     (123)   120661 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/datasets/EqualMinimalJapaneseVowels/EqualMinimalJapaneseVowels_TEST.ts
--rw-r--r--   0 runner    (1001) docker     (123)   120799 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/datasets/EqualMinimalJapaneseVowels/EqualMinimalJapaneseVowels_TRAIN.ts
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:23:30.797438 tsml-0.2.0/tsml/datasets/MinimalChinatown/
--rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/datasets/MinimalChinatown/MinimalChinatown_TEST.ts
--rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/datasets/MinimalChinatown/MinimalChinatown_TRAIN.ts
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:23:30.797438 tsml-0.2.0/tsml/datasets/MinimalGasPrices/
--rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/datasets/MinimalGasPrices/MinimalGasPrices_TEST.ts
--rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/datasets/MinimalGasPrices/MinimalGasPrices_TRAIN.ts
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:23:30.801438 tsml-0.2.0/tsml/datasets/MinimalJapaneseVowels/
--rw-r--r--   0 runner    (1001) docker     (123)    36247 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/datasets/MinimalJapaneseVowels/MinimalJapaneseVowels_TEST.ts
--rw-r--r--   0 runner    (1001) docker     (123)    38758 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/datasets/MinimalJapaneseVowels/MinimalJapaneseVowels_TRAIN.ts
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:23:30.801438 tsml-0.2.0/tsml/datasets/UnequalMinimalChinatown/
--rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/datasets/UnequalMinimalChinatown/UnequalMinimalChinatown_TEST.ts
--rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/datasets/UnequalMinimalChinatown/UnequalMinimalChinatown_TRAIN.ts
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:23:30.801438 tsml-0.2.0/tsml/datasets/UnequalMinimalGasPrices/
--rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/datasets/UnequalMinimalGasPrices/UnequalMinimalGasPrices_TEST.ts
--rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/datasets/UnequalMinimalGasPrices/UnequalMinimalGasPrices_TRAIN.ts
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24932 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/datasets/_data_io.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:23:30.801438 tsml-0.2.0/tsml/datasets/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/datasets/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   286342 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/datasets/tests/_expected_data_io_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/datasets/tests/test_data_io.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:23:30.801438 tsml-0.2.0/tsml/distance_based/
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/distance_based/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5308 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/distance_based/_mpdist.py
--rw-r--r--   0 runner    (1001) docker     (123)     6156 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/distance_based/_pf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:23:30.801438 tsml-0.2.0/tsml/distances/
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/distances/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/distances/_manhattan.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:23:30.801438 tsml-0.2.0/tsml/dummy/
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/dummy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18023 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/dummy/_dummy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:23:30.805438 tsml-0.2.0/tsml/feature_based/
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/feature_based/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20217 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/feature_based/_catch22.py
--rw-r--r--   0 runner    (1001) docker     (123)    13708 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/feature_based/_fpca.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:23:30.805438 tsml-0.2.0/tsml/hybrid/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/hybrid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22124 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/hybrid/_rist.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:23:30.805438 tsml-0.2.0/tsml/interval_based/
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/interval_based/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    48835 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/interval_based/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    41948 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/interval_based/_cif.py
--rw-r--r--   0 runner    (1001) docker     (123)    21846 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/interval_based/_interval_forest.py
--rw-r--r--   0 runner    (1001) docker     (123)    26649 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/interval_based/_interval_pipelines.py
--rw-r--r--   0 runner    (1001) docker     (123)    16744 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/interval_based/_rise.py
--rw-r--r--   0 runner    (1001) docker     (123)    17244 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/interval_based/_stsf.py
--rw-r--r--   0 runner    (1001) docker     (123)    16955 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/interval_based/_tsf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:23:30.805438 tsml-0.2.0/tsml/interval_based/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/interval_based/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5515 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/interval_based/tests/test_interval_forest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:23:30.809438 tsml-0.2.0/tsml/shapelet_based/
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/shapelet_based/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8152 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/shapelet_based/_mrsqm.py
--rw-r--r--   0 runner    (1001) docker     (123)    20841 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/shapelet_based/_rdst.py
--rw-r--r--   0 runner    (1001) docker     (123)    11162 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/shapelet_based/_rsf.py
--rw-r--r--   0 runner    (1001) docker     (123)    12293 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/shapelet_based/_stc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:23:30.809438 tsml-0.2.0/tsml/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/tests/test_all_estimators.py
--rw-r--r--   0 runner    (1001) docker     (123)     9679 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/tests/test_estimator_checks.py
--rw-r--r--   0 runner    (1001) docker     (123)    47622 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/tests/test_estimators_sklearn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/tests/test_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:23:30.809438 tsml-0.2.0/tsml/transformations/
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/transformations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4798 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/transformations/_acf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3839 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/transformations/_ar_coefficient.py
--rw-r--r--   0 runner    (1001) docker     (123)    43348 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/transformations/_catch22.py
--rw-r--r--   0 runner    (1001) docker     (123)     6741 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/transformations/_fpca.py
--rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/transformations/_function_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    37045 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/transformations/_interval_extraction.py
--rw-r--r--   0 runner    (1001) docker     (123)     3963 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/transformations/_periodogram.py
--rw-r--r--   0 runner    (1001) docker     (123)    41527 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/transformations/_sfa.py
--rw-r--r--   0 runner    (1001) docker     (123)    56382 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/transformations/_shapelet_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     3717 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/transformations/_summary_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     4472 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/transformations/_transform_concatenator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:23:30.813438 tsml-0.2.0/tsml/transformations/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/transformations/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/transformations/tests/test_function_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/transformations/tests/test_interval_extraction.py
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/transformations/tests/test_periodogram.py
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/transformations/tests/test_transform_concatenator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:23:30.813438 tsml-0.2.0/tsml/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/utils/_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     4358 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/utils/discovery.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:23:30.813438 tsml-0.2.0/tsml/utils/numba_functions/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/utils/numba_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15812 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/utils/numba_functions/general.py
--rw-r--r--   0 runner    (1001) docker     (123)    21053 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/utils/numba_functions/stats.py
--rw-r--r--   0 runner    (1001) docker     (123)    10603 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/utils/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)    22415 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/utils/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:23:30.813438 tsml-0.2.0/tsml/vector/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/vector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15847 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/vector/_cit.py
--rw-r--r--   0 runner    (1001) docker     (123)    29766 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/vector/_rotation_forest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:23:30.813438 tsml-0.2.0/tsml/vector/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/vector/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-07-21 13:23:15.000000 tsml-0.2.0/tsml/vector/tests/test_rotation_forest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:23:30.797438 tsml-0.2.0/tsml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-07-21 13:23:30.000000 tsml-0.2.0/tsml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-07-21 13:23:30.000000 tsml-0.2.0/tsml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 13:23:30.000000 tsml-0.2.0/tsml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-21 13:23:30.000000 tsml-0.2.0/tsml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-21 13:23:30.000000 tsml-0.2.0/tsml.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 15:43:35.034697 tsml-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-07-22 15:43:25.000000 tsml-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-22 15:43:25.000000 tsml-0.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-07-22 15:43:35.034697 tsml-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-22 15:43:25.000000 tsml-0.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-07-22 15:43:25.000000 tsml-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-22 15:43:35.034697 tsml-0.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 15:43:35.018697 tsml-0.2.1/tsml/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-22 15:43:25.000000 tsml-0.2.1/tsml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11349 2023-07-22 15:43:25.000000 tsml-0.2.1/tsml/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 15:43:35.022697 tsml-0.2.1/tsml/compose/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-07-22 15:43:25.000000 tsml-0.2.1/tsml/compose/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20638 2023-07-22 15:43:25.000000 tsml-0.2.1/tsml/compose/_channel_ensemble.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 15:43:35.022697 tsml-0.2.1/tsml/compose/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-22 15:43:25.000000 tsml-0.2.1/tsml/compose/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-07-22 15:43:25.000000 tsml-0.2.1/tsml/compose/tests/test_channel_ensemble.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 15:43:35.022697 tsml-0.2.1/tsml/datasets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 15:43:35.022697 tsml-0.2.1/tsml/datasets/EqualMinimalJapaneseVowels/
+-rw-r--r--   0 runner    (1001) docker     (123)   120661 2023-07-22 15:43:25.000000 tsml-0.2.1/tsml/datasets/EqualMinimalJapaneseVowels/EqualMinimalJapaneseVowels_TEST.ts
+-rw-r--r--   0 runner    (1001) docker     (123)   120799 2023-07-22 15:43:25.000000 tsml-0.2.1/tsml/datasets/EqualMinimalJapaneseVowels/EqualMinimalJapaneseVowels_TRAIN.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 15:43:35.022697 tsml-0.2.1/tsml/datasets/MinimalChinatown/
+-rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-07-22 15:43:25.000000 tsml-0.2.1/tsml/datasets/MinimalChinatown/MinimalChinatown_TEST.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-07-22 15:43:25.000000 tsml-0.2.1/tsml/datasets/MinimalChinatown/MinimalChinatown_TRAIN.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 15:43:35.022697 tsml-0.2.1/tsml/datasets/MinimalGasPrices/
+-rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-07-22 15:43:25.000000 tsml-0.2.1/tsml/datasets/MinimalGasPrices/MinimalGasPrices_TEST.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-07-22 15:43:25.000000 tsml-0.2.1/tsml/datasets/MinimalGasPrices/MinimalGasPrices_TRAIN.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 15:43:35.022697 tsml-0.2.1/tsml/datasets/MinimalJapaneseVowels/
+-rw-r--r--   0 runner    (1001) docker     (123)    36247 2023-07-22 15:43:25.000000 tsml-0.2.1/tsml/datasets/MinimalJapaneseVowels/MinimalJapaneseVowels_TEST.ts
+-rw-r--r--   0 runner    (1001) docker     (123)    38758 2023-07-22 15:43:25.000000 tsml-0.2.1/tsml/datasets/MinimalJapaneseVowels/MinimalJapaneseVowels_TRAIN.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 15:43:35.022697 tsml-0.2.1/tsml/datasets/UnequalMinimalChinatown/
+-rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-07-22 15:43:25.000000 tsml-0.2.1/tsml/datasets/UnequalMinimalChinatown/UnequalMinimalChinatown_TEST.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-07-22 15:43:25.000000 tsml-0.2.1/tsml/datasets/UnequalMinimalChinatown/UnequalMinimalChinatown_TRAIN.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 15:43:35.022697 tsml-0.2.1/tsml/datasets/UnequalMinimalGasPrices/
+-rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-07-22 15:43:25.000000 tsml-0.2.1/tsml/datasets/UnequalMinimalGasPrices/UnequalMinimalGasPrices_TEST.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-07-22 15:43:25.000000 tsml-0.2.1/tsml/datasets/UnequalMinimalGasPrices/UnequalMinimalGasPrices_TRAIN.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-07-22 15:43:25.000000 tsml-0.2.1/tsml/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24932 2023-07-22 15:43:25.000000 tsml-0.2.1/tsml/datasets/_data_io.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 15:43:35.022697 tsml-0.2.1/tsml/datasets/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-22 15:43:25.000000 tsml-0.2.1/tsml/datasets/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   286342 2023-07-22 15:43:25.000000 tsml-0.2.1/tsml/datasets/tests/_expected_data_io_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-07-22 15:43:25.000000 tsml-0.2.1/tsml/datasets/tests/test_data_io.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 15:43:35.022697 tsml-0.2.1/tsml/distance_based/
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-22 15:43:25.000000 tsml-0.2.1/tsml/distance_based/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5308 2023-07-22 15:43:25.000000 tsml-0.2.1/tsml/distance_based/_mpdist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6156 2023-07-22 15:43:25.000000 tsml-0.2.1/tsml/distance_based/_pf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 15:43:35.022697 tsml-0.2.1/tsml/distances/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-22 15:43:25.000000 tsml-0.2.1/tsml/distances/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-07-22 15:43:25.000000 tsml-0.2.1/tsml/distances/_manhattan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 15:43:35.026697 tsml-0.2.1/tsml/dummy/
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-22 15:43:25.000000 tsml-0.2.1/tsml/dummy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18023 2023-07-22 15:43:25.000000 tsml-0.2.1/tsml/dummy/_dummy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 15:43:35.026697 tsml-0.2.1/tsml/feature_based/
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-22 15:43:25.000000 tsml-0.2.1/tsml/feature_based/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20217 2023-07-22 15:43:25.000000 tsml-0.2.1/tsml/feature_based/_catch22.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13708 2023-07-22 15:43:25.000000 tsml-0.2.1/tsml/feature_based/_fpca.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 15:43:35.026697 tsml-0.2.1/tsml/hybrid/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-22 15:43:25.000000 tsml-0.2.1/tsml/hybrid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22124 2023-07-22 15:43:25.000000 tsml-0.2.1/tsml/hybrid/_rist.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 15:43:35.026697 tsml-0.2.1/tsml/interval_based/
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-07-22 15:43:25.000000 tsml-0.2.1/tsml/interval_based/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48835 2023-07-22 15:43:25.000000 tsml-0.2.1/tsml/interval_based/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41948 2023-07-22 15:43:25.000000 tsml-0.2.1/tsml/interval_based/_cif.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21846 2023-07-22 15:43:25.000000 tsml-0.2.1/tsml/interval_based/_interval_forest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30448 2023-07-22 15:43:25.000000 tsml-0.2.1/tsml/interval_based/_interval_pipelines.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16744 2023-07-22 15:43:25.000000 tsml-0.2.1/tsml/interval_based/_rise.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17244 2023-07-22 15:43:25.000000 tsml-0.2.1/tsml/interval_based/_stsf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16955 2023-07-22 15:43:25.000000 tsml-0.2.1/tsml/interval_based/_tsf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 15:43:35.026697 tsml-0.2.1/tsml/interval_based/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-22 15:43:25.000000 tsml-0.2.1/tsml/interval_based/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5515 2023-07-22 15:43:25.000000 tsml-0.2.1/tsml/interval_based/tests/test_interval_forest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-07-22 15:43:25.000000 tsml-0.2.1/tsml/interval_based/tests/test_interval_pipelines.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 15:43:35.026697 tsml-0.2.1/tsml/shapelet_based/
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-22 15:43:25.000000 tsml-0.2.1/tsml/shapelet_based/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8152 2023-07-22 15:43:25.000000 tsml-0.2.1/tsml/shapelet_based/_mrsqm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20841 2023-07-22 15:43:25.000000 tsml-0.2.1/tsml/shapelet_based/_rdst.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11162 2023-07-22 15:43:25.000000 tsml-0.2.1/tsml/shapelet_based/_rsf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12293 2023-07-22 15:43:25.000000 tsml-0.2.1/tsml/shapelet_based/_stc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 15:43:35.026697 tsml-0.2.1/tsml/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-22 15:43:25.000000 tsml-0.2.1/tsml/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-22 15:43:25.000000 tsml-0.2.1/tsml/tests/test_all_estimators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9679 2023-07-22 15:43:25.000000 tsml-0.2.1/tsml/tests/test_estimator_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47622 2023-07-22 15:43:25.000000 tsml-0.2.1/tsml/tests/test_estimators_sklearn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-07-22 15:43:25.000000 tsml-0.2.1/tsml/tests/test_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 15:43:35.030697 tsml-0.2.1/tsml/transformations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-07-22 15:43:25.000000 tsml-0.2.1/tsml/transformations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4798 2023-07-22 15:43:25.000000 tsml-0.2.1/tsml/transformations/_acf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3839 2023-07-22 15:43:25.000000 tsml-0.2.1/tsml/transformations/_ar_coefficient.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43348 2023-07-22 15:43:25.000000 tsml-0.2.1/tsml/transformations/_catch22.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6741 2023-07-22 15:43:25.000000 tsml-0.2.1/tsml/transformations/_fpca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-07-22 15:43:25.000000 tsml-0.2.1/tsml/transformations/_function_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37313 2023-07-22 15:43:25.000000 tsml-0.2.1/tsml/transformations/_interval_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3963 2023-07-22 15:43:25.000000 tsml-0.2.1/tsml/transformations/_periodogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41527 2023-07-22 15:43:25.000000 tsml-0.2.1/tsml/transformations/_sfa.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56382 2023-07-22 15:43:25.000000 tsml-0.2.1/tsml/transformations/_shapelet_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3717 2023-07-22 15:43:25.000000 tsml-0.2.1/tsml/transformations/_summary_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4472 2023-07-22 15:43:25.000000 tsml-0.2.1/tsml/transformations/_transform_concatenator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 15:43:35.030697 tsml-0.2.1/tsml/transformations/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 15:43:25.000000 tsml-0.2.1/tsml/transformations/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-22 15:43:25.000000 tsml-0.2.1/tsml/transformations/tests/test_function_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-07-22 15:43:25.000000 tsml-0.2.1/tsml/transformations/tests/test_interval_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-07-22 15:43:25.000000 tsml-0.2.1/tsml/transformations/tests/test_periodogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-07-22 15:43:25.000000 tsml-0.2.1/tsml/transformations/tests/test_transform_concatenator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 15:43:35.030697 tsml-0.2.1/tsml/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-22 15:43:25.000000 tsml-0.2.1/tsml/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-07-22 15:43:25.000000 tsml-0.2.1/tsml/utils/_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4358 2023-07-22 15:43:25.000000 tsml-0.2.1/tsml/utils/discovery.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 15:43:35.030697 tsml-0.2.1/tsml/utils/numba_functions/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-22 15:43:25.000000 tsml-0.2.1/tsml/utils/numba_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15812 2023-07-22 15:43:25.000000 tsml-0.2.1/tsml/utils/numba_functions/general.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21053 2023-07-22 15:43:25.000000 tsml-0.2.1/tsml/utils/numba_functions/stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10603 2023-07-22 15:43:25.000000 tsml-0.2.1/tsml/utils/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22415 2023-07-22 15:43:25.000000 tsml-0.2.1/tsml/utils/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 15:43:35.030697 tsml-0.2.1/tsml/vector/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-22 15:43:25.000000 tsml-0.2.1/tsml/vector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15847 2023-07-22 15:43:25.000000 tsml-0.2.1/tsml/vector/_cit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29766 2023-07-22 15:43:25.000000 tsml-0.2.1/tsml/vector/_rotation_forest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 15:43:35.034697 tsml-0.2.1/tsml/vector/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-22 15:43:25.000000 tsml-0.2.1/tsml/vector/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-07-22 15:43:25.000000 tsml-0.2.1/tsml/vector/tests/test_rotation_forest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 15:43:35.022697 tsml-0.2.1/tsml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-07-22 15:43:35.000000 tsml-0.2.1/tsml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-07-22 15:43:35.000000 tsml-0.2.1/tsml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 15:43:35.000000 tsml-0.2.1/tsml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-22 15:43:35.000000 tsml-0.2.1/tsml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-22 15:43:35.000000 tsml-0.2.1/tsml.egg-info/top_level.txt
```

### Comparing `tsml-0.2.0/LICENSE` & `tsml-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tsml-0.2.0/PKG-INFO` & `tsml-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsml
-Version: 0.2.0
+Version: 0.2.1
 Summary: A toolkit for time series machine learning algorithms.
 Author-email: Matthew Middlehurst <m.middlehurst@uea.ac.uk>, Tony Bagnall <ajb@uea.ac.uk>
 License: BSD 3-Clause License
         
         Copyright (c) The Time Series Machine Learning (tsml) developers.
         All rights reserved.
```

### Comparing `tsml-0.2.0/pyproject.toml` & `tsml-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61", "wheel", "toml", "build"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "tsml"
-version = "0.2.0"
+version = "0.2.1"
 description = "A toolkit for time series machine learning algorithms."
 authors = [
     {name = "Matthew Middlehurst", email = "m.middlehurst@uea.ac.uk"},
     {name = "Tony Bagnall", email = "ajb@uea.ac.uk"},
 ]
 readme = "README.md"
 requires-python = ">=3.8,<3.12"
```

### Comparing `tsml-0.2.0/tsml/base.py` & `tsml-0.2.1/tsml/base.py`

 * *Files identical despite different names*

### Comparing `tsml-0.2.0/tsml/compose/_channel_ensemble.py` & `tsml-0.2.1/tsml/compose/_channel_ensemble.py`

 * *Files identical despite different names*

### Comparing `tsml-0.2.0/tsml/compose/tests/test_channel_ensemble.py` & `tsml-0.2.1/tsml/compose/tests/test_channel_ensemble.py`

 * *Files identical despite different names*

### Comparing `tsml-0.2.0/tsml/datasets/EqualMinimalJapaneseVowels/EqualMinimalJapaneseVowels_TEST.ts` & `tsml-0.2.1/tsml/datasets/EqualMinimalJapaneseVowels/EqualMinimalJapaneseVowels_TEST.ts`

 * *Files identical despite different names*

### Comparing `tsml-0.2.0/tsml/datasets/EqualMinimalJapaneseVowels/EqualMinimalJapaneseVowels_TRAIN.ts` & `tsml-0.2.1/tsml/datasets/EqualMinimalJapaneseVowels/EqualMinimalJapaneseVowels_TRAIN.ts`

 * *Files identical despite different names*

### Comparing `tsml-0.2.0/tsml/datasets/MinimalChinatown/MinimalChinatown_TEST.ts` & `tsml-0.2.1/tsml/datasets/MinimalChinatown/MinimalChinatown_TEST.ts`

 * *Files identical despite different names*

### Comparing `tsml-0.2.0/tsml/datasets/MinimalChinatown/MinimalChinatown_TRAIN.ts` & `tsml-0.2.1/tsml/datasets/MinimalChinatown/MinimalChinatown_TRAIN.ts`

 * *Files identical despite different names*

### Comparing `tsml-0.2.0/tsml/datasets/MinimalGasPrices/MinimalGasPrices_TEST.ts` & `tsml-0.2.1/tsml/datasets/MinimalGasPrices/MinimalGasPrices_TEST.ts`

 * *Files identical despite different names*

### Comparing `tsml-0.2.0/tsml/datasets/MinimalGasPrices/MinimalGasPrices_TRAIN.ts` & `tsml-0.2.1/tsml/datasets/MinimalGasPrices/MinimalGasPrices_TRAIN.ts`

 * *Files identical despite different names*

### Comparing `tsml-0.2.0/tsml/datasets/MinimalJapaneseVowels/MinimalJapaneseVowels_TEST.ts` & `tsml-0.2.1/tsml/datasets/MinimalJapaneseVowels/MinimalJapaneseVowels_TEST.ts`

 * *Files identical despite different names*

### Comparing `tsml-0.2.0/tsml/datasets/MinimalJapaneseVowels/MinimalJapaneseVowels_TRAIN.ts` & `tsml-0.2.1/tsml/datasets/MinimalJapaneseVowels/MinimalJapaneseVowels_TRAIN.ts`

 * *Files identical despite different names*

### Comparing `tsml-0.2.0/tsml/datasets/UnequalMinimalChinatown/UnequalMinimalChinatown_TEST.ts` & `tsml-0.2.1/tsml/datasets/UnequalMinimalChinatown/UnequalMinimalChinatown_TEST.ts`

 * *Files identical despite different names*

### Comparing `tsml-0.2.0/tsml/datasets/UnequalMinimalChinatown/UnequalMinimalChinatown_TRAIN.ts` & `tsml-0.2.1/tsml/datasets/UnequalMinimalChinatown/UnequalMinimalChinatown_TRAIN.ts`

 * *Files identical despite different names*

### Comparing `tsml-0.2.0/tsml/datasets/UnequalMinimalGasPrices/UnequalMinimalGasPrices_TEST.ts` & `tsml-0.2.1/tsml/datasets/UnequalMinimalGasPrices/UnequalMinimalGasPrices_TEST.ts`

 * *Files identical despite different names*

### Comparing `tsml-0.2.0/tsml/datasets/UnequalMinimalGasPrices/UnequalMinimalGasPrices_TRAIN.ts` & `tsml-0.2.1/tsml/datasets/UnequalMinimalGasPrices/UnequalMinimalGasPrices_TRAIN.ts`

 * *Files identical despite different names*

### Comparing `tsml-0.2.0/tsml/datasets/__init__.py` & `tsml-0.2.1/tsml/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `tsml-0.2.0/tsml/datasets/_data_io.py` & `tsml-0.2.1/tsml/datasets/_data_io.py`

 * *Files identical despite different names*

### Comparing `tsml-0.2.0/tsml/datasets/tests/_expected_data_io_output.py` & `tsml-0.2.1/tsml/datasets/tests/_expected_data_io_output.py`

 * *Files identical despite different names*

### Comparing `tsml-0.2.0/tsml/datasets/tests/test_data_io.py` & `tsml-0.2.1/tsml/datasets/tests/test_data_io.py`

 * *Files identical despite different names*

### Comparing `tsml-0.2.0/tsml/distance_based/_mpdist.py` & `tsml-0.2.1/tsml/distance_based/_mpdist.py`

 * *Files identical despite different names*

### Comparing `tsml-0.2.0/tsml/distance_based/_pf.py` & `tsml-0.2.1/tsml/distance_based/_pf.py`

 * *Files identical despite different names*

### Comparing `tsml-0.2.0/tsml/distances/_manhattan.py` & `tsml-0.2.1/tsml/distances/_manhattan.py`

 * *Files identical despite different names*

### Comparing `tsml-0.2.0/tsml/dummy/_dummy.py` & `tsml-0.2.1/tsml/dummy/_dummy.py`

 * *Files identical despite different names*

### Comparing `tsml-0.2.0/tsml/feature_based/_catch22.py` & `tsml-0.2.1/tsml/feature_based/_catch22.py`

 * *Files identical despite different names*

### Comparing `tsml-0.2.0/tsml/feature_based/_fpca.py` & `tsml-0.2.1/tsml/feature_based/_fpca.py`

 * *Files identical despite different names*

### Comparing `tsml-0.2.0/tsml/hybrid/_rist.py` & `tsml-0.2.1/tsml/hybrid/_rist.py`

 * *Files identical despite different names*

### Comparing `tsml-0.2.0/tsml/interval_based/__init__.py` & `tsml-0.2.1/tsml/interval_based/__init__.py`

 * *Files identical despite different names*

### Comparing `tsml-0.2.0/tsml/interval_based/_base.py` & `tsml-0.2.1/tsml/interval_based/_base.py`

 * *Files identical despite different names*

### Comparing `tsml-0.2.0/tsml/interval_based/_cif.py` & `tsml-0.2.1/tsml/interval_based/_cif.py`

 * *Files identical despite different names*

### Comparing `tsml-0.2.0/tsml/interval_based/_interval_forest.py` & `tsml-0.2.1/tsml/interval_based/_interval_forest.py`

 * *Files identical despite different names*

### Comparing `tsml-0.2.0/tsml/interval_based/_interval_pipelines.py` & `tsml-0.2.1/tsml/interval_based/_interval_pipelines.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,15 +12,16 @@
 ]
 
 from typing import List, Union
 
 import numpy as np
 from sklearn.base import ClassifierMixin, RegressorMixin
 from sklearn.ensemble import RandomForestClassifier, RandomForestRegressor
-from sklearn.utils.validation import check_is_fitted
+from sklearn.ensemble._base import _set_random_states
+from sklearn.utils.validation import check_is_fitted, check_random_state
 
 from tsml.base import BaseTimeSeriesEstimator, _clone_estimator
 from tsml.transformations._interval_extraction import (
     RandomIntervalTransformer,
     SupervisedIntervalTransformer,
 )
 from tsml.utils.validation import check_n_jobs
@@ -31,25 +32,33 @@
 
     Extracts multiple intervals with random length, position and dimension from series
     qnd concatenates them into a feature vector. Builds an estimator on the
     transformed data.
 
     Parameters
     ----------
-    n_intervals : int, default=100,
+    n_intervals : int or callable, default=100,
         The number of intervals of random length, position and dimension to be
-        extracted.
+        extracted.  Input should be an int or a function that takes a 3D np.ndarray
+        input and returns an int.
     min_interval_length : int, default=3
         The minimum length of extracted intervals. Minimum value of 3.
     max_interval_length : int, default=3
         The maximum length of extracted intervals. Minimum value of min_interval_length.
     features : TransformerMixin, a function taking a 2d numpy array parameter, or list
             of said transformers and functions, default=None
         Transformers and functions used to extract features from selected intervals.
         If None, defaults to [mean, median, min, max, std, 25% quantile, 75% quantile]
+    series_transformers : TransformerMixin, list, tuple, or None, default=None
+        The transformers to apply to the series before extracting intervals and
+        shapelets. If None, use the series as is.
+
+        A list or tuple of transformers will extract intervals from
+        all transformations concatenate the output. Including None in the list or tuple
+        will use the series as is for interval extraction.
     dilation : int, list or None, default=None
         Add dilation to extracted intervals. No dilation is added if None or 1. If a
         list of ints, a random dilation value is selected from the list for each
         interval.
 
         The dilation value is selected after the interval star and end points. If the
         number of values in the dilated interval is less than the min_interval_length,
@@ -70,17 +79,17 @@
         Valid options are "loky", "multiprocessing", "threading" or a custom backend.
         See the joblib Parallel documentation for more details.
 
     Attributes
     ----------
     n_instances_ : int
         The number of train cases in the training set.
-    n_channels : int
+    n_channels_ : int
         The number of dimensions per case in the training set.
-    n_timepoints : int
+    n_timepoints_ : int
         The length of each series in the training set.
     n_classes_ : int
         Number of classes. Extracted from the data.
     classes_ : ndarray of shape (n_classes_)
         Holds the label for each class.
     class_dictionary_ : dict
         A dictionary mapping class labels to class indices in classes_.
@@ -105,24 +114,26 @@
 
     def __init__(
         self,
         n_intervals=100,
         min_interval_length=3,
         max_interval_length=np.inf,
         features=None,
+        series_transformers=None,
         dilation=None,
         estimator=None,
         n_jobs=1,
         random_state=None,
         parallel_backend=None,
     ):
         self.n_intervals = n_intervals
         self.min_interval_length = min_interval_length
         self.max_interval_length = max_interval_length
         self.features = features
+        self.series_transformers = series_transformers
         self.dilation = dilation
         self.estimator = estimator
         self.random_state = random_state
         self.n_jobs = n_jobs
         self.parallel_backend = parallel_backend
 
         super(RandomIntervalClassifier, self).__init__()
@@ -154,38 +165,62 @@
         for index, class_val in enumerate(self.classes_):
             self.class_dictionary_[class_val] = index
 
         if self.n_classes_ == 1:
             return self
 
         self._n_jobs = check_n_jobs(self.n_jobs)
+        rng = check_random_state(self.random_state)
 
-        self._transformer = RandomIntervalTransformer(
-            n_intervals=self.n_intervals,
-            min_interval_length=self.min_interval_length,
-            max_interval_length=self.max_interval_length,
-            features=self.features,
-            dilation=self.dilation,
-            random_state=self.random_state,
-            n_jobs=self._n_jobs,
-            parallel_backend=self.parallel_backend,
-        )
+        if isinstance(self.series_transformers, (list, tuple)):
+            self._series_transformers = [
+                None if st is None else _clone_estimator(st, random_state=rng)
+                for st in self.series_transformers
+            ]
+        else:
+            self._series_transformers = [
+                None
+                if self.series_transformers is None
+                else _clone_estimator(self.series_transformers, random_state=rng)
+            ]
+
+        X_t = np.empty((X.shape[0], 0))
+        self._transformers = []
+        for st in self._series_transformers:
+            if st is not None:
+                s = st.fit_transform(X, y)
+            else:
+                s = X
+
+            ct = RandomIntervalTransformer(
+                n_intervals=self.n_intervals,
+                min_interval_length=self.min_interval_length,
+                max_interval_length=self.max_interval_length,
+                features=self.features,
+                dilation=self.dilation,
+                n_jobs=self._n_jobs,
+                parallel_backend=self.parallel_backend,
+            )
+            _set_random_states(ct, rng)
+            self._transformers.append(ct)
+            t = ct.fit_transform(s, y)
+
+            X_t = np.hstack((X_t, t))
 
         self._estimator = _clone_estimator(
             RandomForestClassifier(n_estimators=200)
             if self.estimator is None
             else self.estimator,
             self.random_state,
         )
 
         m = getattr(self._estimator, "n_jobs", None)
         if m is not None:
             self._estimator.n_jobs = self._n_jobs
 
-        X_t = self._transformer.fit_transform(X, y)
         self._estimator.fit(X_t, y)
 
         return self
 
     def predict(self, X: Union[np.ndarray, List[np.ndarray]]) -> np.ndarray:
         """Predicts labels for sequences in X.
 
@@ -204,15 +239,25 @@
         # treat case of single class seen in fit
         if self.n_classes_ == 1:
             return np.repeat(list(self.class_dictionary_.keys()), X.shape[0], axis=0)
 
         X = self._validate_data(X=X, reset=False, ensure_min_series_length=3)
         X = self._convert_X(X)
 
-        return self._estimator.predict(self._transformer.transform(X))
+        X_t = np.empty((X.shape[0], 0))
+        for i, st in enumerate(self._series_transformers):
+            if st is not None:
+                s = st.transform(X)
+            else:
+                s = X
+
+            t = self._transformers[i].transform(s)
+            X_t = np.hstack((X_t, t))
+
+        return self._estimator.predict(X_t)
 
     def predict_proba(self, X: Union[np.ndarray, List[np.ndarray]]) -> np.ndarray:
         """Predicts labels probabilities for sequences in X.
 
         Parameters
         ----------
         X : 3D np.array of shape (n_instances, n_channels, n_timepoints)
@@ -228,20 +273,30 @@
         # treat case of single class seen in fit
         if self.n_classes_ == 1:
             return np.repeat([[1]], X.shape[0], axis=0)
 
         X = self._validate_data(X=X, reset=False, ensure_min_series_length=3)
         X = self._convert_X(X)
 
+        X_t = np.empty((X.shape[0], 0))
+        for i, st in enumerate(self._series_transformers):
+            if st is not None:
+                s = st.transform(X)
+            else:
+                s = X
+
+            t = self._transformers[i].transform(s)
+            X_t = np.hstack((X_t, t))
+
         m = getattr(self._estimator, "predict_proba", None)
         if callable(m):
-            return self._estimator.predict_proba(self._transformer.transform(X))
+            return self._estimator.predict_proba(X_t)
         else:
             dists = np.zeros((X.shape[0], self.n_classes_))
-            preds = self._estimator.predict(self._transformer.transform(X))
+            preds = self._estimator.predict(X_t)
             for i in range(0, X.shape[0]):
                 dists[i, self.class_dictionary_[preds[i]]] = 1
             return dists
 
     @classmethod
     def get_test_params(
         cls, parameter_set: Union[str, None] = None
@@ -273,25 +328,33 @@
 
     Extracts multiple intervals with random length, position and dimension from series
     and concatenates them into a feature vector. Builds an estimator on the
     transformed data.
 
     Parameters
     ----------
-    n_intervals : int, default=100,
+    n_intervals : int or callable, default=100,
         The number of intervals of random length, position and dimension to be
-        extracted.
+        extracted.  Input should be an int or a function that takes a 3D np.ndarray
+        input and returns an int.
     min_interval_length : int, default=3
         The minimum length of extracted intervals. Minimum value of 3.
     max_interval_length : int, default=3
         The maximum length of extracted intervals. Minimum value of min_interval_length.
     features : TransformerMixin, a function taking a 2d numpy array parameter, or list
             of said transformers and functions, default=None
         Transformers and functions used to extract features from selected intervals.
         If None, defaults to [mean, median, min, max, std, 25% quantile, 75% quantile]
+    series_transformers : TransformerMixin, list, tuple, or None, default=None
+        The transformers to apply to the series before extracting intervals and
+        shapelets. If None, use the series as is.
+
+        A list or tuple of transformers will extract intervals from
+        all transformations concatenate the output. Including None in the list or tuple
+        will use the series as is for interval extraction.
     dilation : int, list or None, default=None
         Add dilation to extracted intervals. No dilation is added if None or 1. If a
         list of ints, a random dilation value is selected from the list for each
         interval.
 
         The dilation value is selected after the interval star and end points. If the
         number of values in the dilated interval is less than the min_interval_length,
@@ -332,34 +395,36 @@
     >>> from tsml.utils.testing import generate_3d_test_data
     >>> X, y = generate_3d_test_data(n_samples=8, series_length=10,
     ...                              regression_target=True, random_state=0)
     >>> reg = RandomIntervalRegressor(random_state=0)
     >>> reg.fit(X, y)
     RandomIntervalRegressor(...)
     >>> reg.predict(X)
-    array([0.46836751, 1.32023847, 1.13355919, 0.63979608, 0.58309353,
-           1.18197903, 0.57859747, 1.0772939 ])
+    array([0.44924979, 1.31424037, 1.11951504, 0.63780969, 0.58123516,
+           1.17135463, 0.56450198, 1.10128837])
     """
 
     def __init__(
         self,
         n_intervals=100,
         min_interval_length=3,
         max_interval_length=np.inf,
         features=None,
+        series_transformers=None,
         dilation=None,
         estimator=None,
         n_jobs=1,
         random_state=None,
         parallel_backend=None,
     ):
         self.n_intervals = n_intervals
         self.min_interval_length = min_interval_length
         self.max_interval_length = max_interval_length
         self.features = features
+        self.series_transformers = series_transformers
         self.dilation = dilation
         self.estimator = estimator
         self.random_state = random_state
         self.n_jobs = n_jobs
         self.parallel_backend = parallel_backend
 
         super(RandomIntervalRegressor, self).__init__()
@@ -383,38 +448,62 @@
             X=X, y=y, ensure_min_samples=2, ensure_min_series_length=3
         )
         X = self._convert_X(X)
 
         self.n_instances_, self.n_channels_, self.n_timepoints_ = X.shape
 
         self._n_jobs = check_n_jobs(self.n_jobs)
+        rng = check_random_state(self.random_state)
 
-        self._transformer = RandomIntervalTransformer(
-            n_intervals=self.n_intervals,
-            min_interval_length=self.min_interval_length,
-            max_interval_length=self.max_interval_length,
-            features=self.features,
-            dilation=self.dilation,
-            random_state=self.random_state,
-            n_jobs=self._n_jobs,
-            parallel_backend=self.parallel_backend,
-        )
+        if isinstance(self.series_transformers, (list, tuple)):
+            self._series_transformers = [
+                None if st is None else _clone_estimator(st, random_state=rng)
+                for st in self.series_transformers
+            ]
+        else:
+            self._series_transformers = [
+                None
+                if self.series_transformers is None
+                else _clone_estimator(self.series_transformers, random_state=rng)
+            ]
+
+        X_t = np.empty((X.shape[0], 0))
+        self._transformers = []
+        for st in self._series_transformers:
+            if st is not None:
+                s = st.fit_transform(X, y)
+            else:
+                s = X
+
+            ct = RandomIntervalTransformer(
+                n_intervals=self.n_intervals,
+                min_interval_length=self.min_interval_length,
+                max_interval_length=self.max_interval_length,
+                features=self.features,
+                dilation=self.dilation,
+                n_jobs=self._n_jobs,
+                parallel_backend=self.parallel_backend,
+            )
+            _set_random_states(ct, rng)
+            self._transformers.append(ct)
+            t = ct.fit_transform(s, y)
+
+            X_t = np.hstack((X_t, t))
 
         self._estimator = _clone_estimator(
             RandomForestRegressor(n_estimators=200)
             if self.estimator is None
             else self.estimator,
             self.random_state,
         )
 
         m = getattr(self._estimator, "n_jobs", None)
         if m is not None:
             self._estimator.n_jobs = self._n_jobs
 
-        X_t = self._transformer.fit_transform(X, y)
         self._estimator.fit(X_t, y)
 
         return self
 
     def predict(self, X: Union[np.ndarray, List[np.ndarray]]) -> np.ndarray:
         """Predicts labels for sequences in X.
 
@@ -429,15 +518,25 @@
             Predicted target labels.
         """
         check_is_fitted(self)
 
         X = self._validate_data(X=X, reset=False, ensure_min_series_length=3)
         X = self._convert_X(X)
 
-        return self._estimator.predict(self._transformer.transform(X))
+        X_t = np.empty((X.shape[0], 0))
+        for i, st in enumerate(self._series_transformers):
+            if st is not None:
+                s = st.transform(X)
+            else:
+                s = X
+
+            t = self._transformers[i].transform(s)
+            X_t = np.hstack((X_t, t))
+
+        return self._estimator.predict(X_t)
 
     @classmethod
     def get_test_params(
         cls, parameter_set: Union[str, None] = None
     ) -> Union[dict, List[dict]]:
         """Return unit test parameter settings for the estimator.
```

### Comparing `tsml-0.2.0/tsml/interval_based/_rise.py` & `tsml-0.2.1/tsml/interval_based/_rise.py`

 * *Files identical despite different names*

### Comparing `tsml-0.2.0/tsml/interval_based/_stsf.py` & `tsml-0.2.1/tsml/interval_based/_stsf.py`

 * *Files identical despite different names*

### Comparing `tsml-0.2.0/tsml/interval_based/_tsf.py` & `tsml-0.2.1/tsml/interval_based/_tsf.py`

 * *Files identical despite different names*

### Comparing `tsml-0.2.0/tsml/interval_based/tests/test_interval_forest.py` & `tsml-0.2.1/tsml/interval_based/tests/test_interval_forest.py`

 * *Files identical despite different names*

### Comparing `tsml-0.2.0/tsml/shapelet_based/__init__.py` & `tsml-0.2.1/tsml/shapelet_based/__init__.py`

 * *Files identical despite different names*

### Comparing `tsml-0.2.0/tsml/shapelet_based/_mrsqm.py` & `tsml-0.2.1/tsml/shapelet_based/_mrsqm.py`

 * *Files identical despite different names*

### Comparing `tsml-0.2.0/tsml/shapelet_based/_rdst.py` & `tsml-0.2.1/tsml/shapelet_based/_rdst.py`

 * *Files identical despite different names*

### Comparing `tsml-0.2.0/tsml/shapelet_based/_rsf.py` & `tsml-0.2.1/tsml/shapelet_based/_rsf.py`

 * *Files identical despite different names*

### Comparing `tsml-0.2.0/tsml/shapelet_based/_stc.py` & `tsml-0.2.1/tsml/shapelet_based/_stc.py`

 * *Files identical despite different names*

### Comparing `tsml-0.2.0/tsml/tests/test_estimator_checks.py` & `tsml-0.2.1/tsml/tests/test_estimator_checks.py`

 * *Files identical despite different names*

### Comparing `tsml-0.2.0/tsml/tests/test_estimators_sklearn.py` & `tsml-0.2.1/tsml/tests/test_estimators_sklearn.py`

 * *Files identical despite different names*

### Comparing `tsml-0.2.0/tsml/tests/test_interface.py` & `tsml-0.2.1/tsml/tests/test_interface.py`

 * *Files identical despite different names*

### Comparing `tsml-0.2.0/tsml/transformations/__init__.py` & `tsml-0.2.1/tsml/transformations/__init__.py`

 * *Files identical despite different names*

### Comparing `tsml-0.2.0/tsml/transformations/_acf.py` & `tsml-0.2.1/tsml/transformations/_acf.py`

 * *Files identical despite different names*

### Comparing `tsml-0.2.0/tsml/transformations/_ar_coefficient.py` & `tsml-0.2.1/tsml/transformations/_ar_coefficient.py`

 * *Files identical despite different names*

### Comparing `tsml-0.2.0/tsml/transformations/_catch22.py` & `tsml-0.2.1/tsml/transformations/_catch22.py`

 * *Files identical despite different names*

### Comparing `tsml-0.2.0/tsml/transformations/_fpca.py` & `tsml-0.2.1/tsml/transformations/_fpca.py`

 * *Files identical despite different names*

### Comparing `tsml-0.2.0/tsml/transformations/_function_transformer.py` & `tsml-0.2.1/tsml/transformations/_function_transformer.py`

 * *Files identical despite different names*

### Comparing `tsml-0.2.0/tsml/transformations/_interval_extraction.py` & `tsml-0.2.1/tsml/transformations/_interval_extraction.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,17 +44,18 @@
     concatenates them into a feature vector in transform.
 
     Identical intervals are pruned at the end of fit, as such the number of features may
     be less than expected from n_intervals.
 
     Parameters
     ----------
-    n_intervals : int, default=100,
+    n_intervals : int or callable, default=100,
         The number of intervals of random length, position and dimension to be
-        extracted.
+        extracted.  Input should be an int or a function that takes a 3D np.ndarray
+        input and returns an int.
     min_interval_length : int, default=3
         The minimum length of extracted intervals. Minimum value of 3.
     max_interval_length : int, default=3
         The maximum length of extracted intervals. Minimum value of min_interval_length.
     features : BaseTransformer, a function taking a 2d numpy array parameter, or list
             of said transformers and functions, default=None
         Transformers and functions used to extract features from selected intervals.
@@ -146,15 +147,15 @@
         )(
             delayed(self._generate_interval)(
                 X,
                 y,
                 rng.randint(np.iinfo(np.int32).max),
                 True,
             )
-            for _ in range(self.n_intervals)
+            for _ in range(self._n_intervals)
         )
 
         (
             intervals,
             transformed_intervals,
         ) = zip(*fit)
 
@@ -172,15 +173,15 @@
                 current.append(new_interval)
                 self.intervals_.extend(interval)
                 self.n_intervals_ += 1
             else:
                 removed_idx.append(i)
 
         Xt = transformed_intervals[0]
-        for i in range(1, self.n_intervals):
+        for i in range(1, self._n_intervals):
             if i not in removed_idx:
                 Xt = np.hstack((Xt, transformed_intervals[i]))
 
         return Xt
 
     def fit(self, X, y=None):
         X, rng = self._fit_setup(X)
@@ -257,14 +258,19 @@
         X = self._convert_X(X)
 
         self.intervals_ = []
         self._transform_features = None
 
         self.n_instances_, self.n_dims_, self.series_length_ = X.shape
 
+        if callable(self.n_intervals):
+            self._n_intervals = self.n_intervals(X)
+        else:
+            self._n_intervals = self.n_intervals
+
         self._min_interval_length = self.min_interval_length
         if self.min_interval_length < 3:
             self._min_interval_length = 3
 
         self._max_interval_length = self.max_interval_length
         if self.max_interval_length < self._min_interval_length:
             self._max_interval_length = self._min_interval_length
```

### Comparing `tsml-0.2.0/tsml/transformations/_periodogram.py` & `tsml-0.2.1/tsml/transformations/_periodogram.py`

 * *Files identical despite different names*

### Comparing `tsml-0.2.0/tsml/transformations/_sfa.py` & `tsml-0.2.1/tsml/transformations/_sfa.py`

 * *Files identical despite different names*

### Comparing `tsml-0.2.0/tsml/transformations/_shapelet_transform.py` & `tsml-0.2.1/tsml/transformations/_shapelet_transform.py`

 * *Files identical despite different names*

### Comparing `tsml-0.2.0/tsml/transformations/_summary_features.py` & `tsml-0.2.1/tsml/transformations/_summary_features.py`

 * *Files identical despite different names*

### Comparing `tsml-0.2.0/tsml/transformations/_transform_concatenator.py` & `tsml-0.2.1/tsml/transformations/_transform_concatenator.py`

 * *Files identical despite different names*

### Comparing `tsml-0.2.0/tsml/transformations/tests/test_function_transformer.py` & `tsml-0.2.1/tsml/transformations/tests/test_function_transformer.py`

 * *Files identical despite different names*

### Comparing `tsml-0.2.0/tsml/transformations/tests/test_interval_extraction.py` & `tsml-0.2.1/tsml/transformations/tests/test_interval_extraction.py`

 * *Files identical despite different names*

### Comparing `tsml-0.2.0/tsml/transformations/tests/test_transform_concatenator.py` & `tsml-0.2.1/tsml/transformations/tests/test_transform_concatenator.py`

 * *Files identical despite different names*

### Comparing `tsml-0.2.0/tsml/utils/_tags.py` & `tsml-0.2.1/tsml/utils/_tags.py`

 * *Files identical despite different names*

### Comparing `tsml-0.2.0/tsml/utils/discovery.py` & `tsml-0.2.1/tsml/utils/discovery.py`

 * *Files identical despite different names*

### Comparing `tsml-0.2.0/tsml/utils/numba_functions/general.py` & `tsml-0.2.1/tsml/utils/numba_functions/general.py`

 * *Files identical despite different names*

### Comparing `tsml-0.2.0/tsml/utils/numba_functions/stats.py` & `tsml-0.2.1/tsml/utils/numba_functions/stats.py`

 * *Files identical despite different names*

### Comparing `tsml-0.2.0/tsml/utils/testing.py` & `tsml-0.2.1/tsml/utils/testing.py`

 * *Files identical despite different names*

### Comparing `tsml-0.2.0/tsml/utils/validation.py` & `tsml-0.2.1/tsml/utils/validation.py`

 * *Files identical despite different names*

### Comparing `tsml-0.2.0/tsml/vector/_cit.py` & `tsml-0.2.1/tsml/vector/_cit.py`

 * *Files identical despite different names*

### Comparing `tsml-0.2.0/tsml/vector/_rotation_forest.py` & `tsml-0.2.1/tsml/vector/_rotation_forest.py`

 * *Files identical despite different names*

### Comparing `tsml-0.2.0/tsml/vector/tests/test_rotation_forest.py` & `tsml-0.2.1/tsml/vector/tests/test_rotation_forest.py`

 * *Files identical despite different names*

### Comparing `tsml-0.2.0/tsml.egg-info/PKG-INFO` & `tsml-0.2.1/tsml.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsml
-Version: 0.2.0
+Version: 0.2.1
 Summary: A toolkit for time series machine learning algorithms.
 Author-email: Matthew Middlehurst <m.middlehurst@uea.ac.uk>, Tony Bagnall <ajb@uea.ac.uk>
 License: BSD 3-Clause License
         
         Copyright (c) The Time Series Machine Learning (tsml) developers.
         All rights reserved.
```

### Comparing `tsml-0.2.0/tsml.egg-info/SOURCES.txt` & `tsml-0.2.1/tsml.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -48,14 +48,15 @@
 tsml/interval_based/_interval_forest.py
 tsml/interval_based/_interval_pipelines.py
 tsml/interval_based/_rise.py
 tsml/interval_based/_stsf.py
 tsml/interval_based/_tsf.py
 tsml/interval_based/tests/__init__.py
 tsml/interval_based/tests/test_interval_forest.py
+tsml/interval_based/tests/test_interval_pipelines.py
 tsml/shapelet_based/__init__.py
 tsml/shapelet_based/_mrsqm.py
 tsml/shapelet_based/_rdst.py
 tsml/shapelet_based/_rsf.py
 tsml/shapelet_based/_stc.py
 tsml/tests/__init__.py
 tsml/tests/test_all_estimators.py
```

### Comparing `tsml-0.2.0/tsml.egg-info/requires.txt` & `tsml-0.2.1/tsml.egg-info/requires.txt`

 * *Files identical despite different names*

