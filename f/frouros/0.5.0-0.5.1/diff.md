# Comparing `tmp/frouros-0.5.0.tar.gz` & `tmp/frouros-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frouros-0.5.0.tar", last modified: Tue Jul 18 10:24:07 2023, max compression
+gzip compressed data, was "frouros-0.5.1.tar", last modified: Sat Jul 22 14:52:29 2023, max compression
```

## Comparing `frouros-0.5.0.tar` & `frouros-0.5.1.tar`

### file list

```diff
@@ -1,134 +1,135 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 10:24:07.517669 frouros-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (122)     1548 2023-07-18 10:23:52.000000 frouros-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       15 2023-07-18 10:23:52.000000 frouros-0.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    23673 2023-07-18 10:24:07.517669 frouros-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    22052 2023-07-18 10:23:52.000000 frouros-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 10:24:07.509668 frouros-0.5.0/frouros/
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 10:24:07.509668 frouros-0.5.0/frouros/callbacks/
--rw-r--r--   0 runner    (1001) docker     (122)      312 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2047 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/callbacks/base.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 10:24:07.509668 frouros-0.5.0/frouros/callbacks/batch/
--rw-r--r--   0 runner    (1001) docker     (122)      207 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/callbacks/batch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      735 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/callbacks/batch/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     5629 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/callbacks/batch/permutation_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     2118 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/callbacks/batch/reset.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 10:24:07.509668 frouros-0.5.0/frouros/callbacks/streaming/
--rw-r--r--   0 runner    (1001) docker     (122)      232 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/callbacks/streaming/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      743 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/callbacks/streaming/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     2647 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/callbacks/streaming/history.py
--rw-r--r--   0 runner    (1001) docker     (122)     6295 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/callbacks/streaming/msprt.py
--rw-r--r--   0 runner    (1001) docker     (122)     2009 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/callbacks/streaming/warning_samples.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 10:24:07.509668 frouros-0.5.0/frouros/common/
--rw-r--r--   0 runner    (1001) docker     (122)       19 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      240 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/common/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 10:24:07.509668 frouros-0.5.0/frouros/datasets/
--rw-r--r--   0 runner    (1001) docker     (122)       21 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5703 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/datasets/base.py
--rw-r--r--   0 runner    (1001) docker     (122)      466 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/datasets/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     1214 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/datasets/real.py
--rw-r--r--   0 runner    (1001) docker     (122)     3041 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/datasets/synthetic.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 10:24:07.509668 frouros-0.5.0/frouros/detectors/
--rw-r--r--   0 runner    (1001) docker     (122)       30 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/detectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2331 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/detectors/base.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 10:24:07.513669 frouros-0.5.0/frouros/detectors/concept_drift/
--rw-r--r--   0 runner    (1001) docker     (122)      943 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/detectors/concept_drift/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6598 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/detectors/concept_drift/base.py
--rw-r--r--   0 runner    (1001) docker     (122)      285 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/detectors/concept_drift/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 10:24:07.513669 frouros-0.5.0/frouros/detectors/concept_drift/streaming/
--rw-r--r--   0 runner    (1001) docker     (122)     1112 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/detectors/concept_drift/streaming/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      566 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/detectors/concept_drift/streaming/base.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 10:24:07.513669 frouros-0.5.0/frouros/detectors/concept_drift/streaming/change_detection/
--rw-r--r--   0 runner    (1001) docker     (122)      513 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/detectors/concept_drift/streaming/change_detection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5856 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/detectors/concept_drift/streaming/change_detection/base.py
--rw-r--r--   0 runner    (1001) docker     (122)    10325 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/detectors/concept_drift/streaming/change_detection/bocd.py
--rw-r--r--   0 runner    (1001) docker     (122)     1572 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/detectors/concept_drift/streaming/change_detection/cusum.py
--rw-r--r--   0 runner    (1001) docker     (122)     1824 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/detectors/concept_drift/streaming/change_detection/geometric_moving_average.py
--rw-r--r--   0 runner    (1001) docker     (122)     1732 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/detectors/concept_drift/streaming/change_detection/page_hinkley.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 10:24:07.513669 frouros-0.5.0/frouros/detectors/concept_drift/streaming/statistical_process_control/
--rw-r--r--   0 runner    (1001) docker     (122)      479 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/detectors/concept_drift/streaming/statistical_process_control/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10975 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/detectors/concept_drift/streaming/statistical_process_control/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     2752 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/detectors/concept_drift/streaming/statistical_process_control/ddm.py
--rw-r--r--   0 runner    (1001) docker     (122)     4920 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/detectors/concept_drift/streaming/statistical_process_control/ecdd.py
--rw-r--r--   0 runner    (1001) docker     (122)    12526 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/detectors/concept_drift/streaming/statistical_process_control/eddm.py
--rw-r--r--   0 runner    (1001) docker     (122)    23271 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/detectors/concept_drift/streaming/statistical_process_control/hddm.py
--rw-r--r--   0 runner    (1001) docker     (122)     9767 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/detectors/concept_drift/streaming/statistical_process_control/rddm.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 10:24:07.513669 frouros-0.5.0/frouros/detectors/concept_drift/streaming/window_based/
--rw-r--r--   0 runner    (1001) docker     (122)      285 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/detectors/concept_drift/streaming/window_based/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    19431 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/detectors/concept_drift/streaming/window_based/adwin.py
--rw-r--r--   0 runner    (1001) docker     (122)      581 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/detectors/concept_drift/streaming/window_based/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     6066 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/detectors/concept_drift/streaming/window_based/kswin.py
--rw-r--r--   0 runner    (1001) docker     (122)     7985 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/detectors/concept_drift/streaming/window_based/stepd.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 10:24:07.513669 frouros-0.5.0/frouros/detectors/data_drift/
--rw-r--r--   0 runner    (1001) docker     (122)      689 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/detectors/data_drift/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6567 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/detectors/data_drift/base.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 10:24:07.513669 frouros-0.5.0/frouros/detectors/data_drift/batch/
--rw-r--r--   0 runner    (1001) docker     (122)      613 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/detectors/data_drift/batch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3754 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/detectors/data_drift/batch/base.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 10:24:07.513669 frouros-0.5.0/frouros/detectors/data_drift/batch/distance_based/
--rw-r--r--   0 runner    (1001) docker     (122)      486 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/detectors/data_drift/batch/distance_based/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8889 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/detectors/data_drift/batch/distance_based/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     1929 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/detectors/data_drift/batch/distance_based/bhattacharyya_distance.py
--rw-r--r--   0 runner    (1001) docker     (122)     1831 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/detectors/data_drift/batch/distance_based/emd.py
--rw-r--r--   0 runner    (1001) docker     (122)     2189 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/detectors/data_drift/batch/distance_based/hellinger_distance.py
--rw-r--r--   0 runner    (1001) docker     (122)     2340 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/detectors/data_drift/batch/distance_based/hi_normalized_complement.py
--rw-r--r--   0 runner    (1001) docker     (122)     2187 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/detectors/data_drift/batch/distance_based/js.py
--rw-r--r--   0 runner    (1001) docker     (122)     2199 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/detectors/data_drift/batch/distance_based/kl.py
--rw-r--r--   0 runner    (1001) docker     (122)     8198 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/detectors/data_drift/batch/distance_based/mmd.py
--rw-r--r--   0 runner    (1001) docker     (122)     2403 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/detectors/data_drift/batch/distance_based/psi.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 10:24:07.517669 frouros-0.5.0/frouros/detectors/data_drift/batch/statistical_test/
--rw-r--r--   0 runner    (1001) docker     (122)      417 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/detectors/data_drift/batch/statistical_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1840 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/detectors/data_drift/batch/statistical_test/anderson_darling.py
--rw-r--r--   0 runner    (1001) docker     (122)     1110 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/detectors/data_drift/batch/statistical_test/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     2558 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/detectors/data_drift/batch/statistical_test/chisquare.py
--rw-r--r--   0 runner    (1001) docker     (122)     2489 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/detectors/data_drift/batch/statistical_test/cvm.py
--rw-r--r--   0 runner    (1001) docker     (122)     1625 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/detectors/data_drift/batch/statistical_test/ks.py
--rw-r--r--   0 runner    (1001) docker     (122)     1701 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/detectors/data_drift/batch/statistical_test/mann_whitney_u.py
--rw-r--r--   0 runner    (1001) docker     (122)     1651 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/detectors/data_drift/batch/statistical_test/welch_t_test.py
--rw-r--r--   0 runner    (1001) docker     (122)      428 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/detectors/data_drift/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 10:24:07.517669 frouros-0.5.0/frouros/detectors/data_drift/streaming/
--rw-r--r--   0 runner    (1001) docker     (122)      183 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/detectors/data_drift/streaming/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2952 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/detectors/data_drift/streaming/base.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 10:24:07.517669 frouros-0.5.0/frouros/detectors/data_drift/streaming/distance_based/
--rw-r--r--   0 runner    (1001) docker     (122)      115 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/detectors/data_drift/streaming/distance_based/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2019 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/detectors/data_drift/streaming/distance_based/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     3224 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/detectors/data_drift/streaming/distance_based/mmd.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 10:24:07.517669 frouros-0.5.0/frouros/detectors/data_drift/streaming/statistical_test/
--rw-r--r--   0 runner    (1001) docker     (122)      144 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/detectors/data_drift/streaming/statistical_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2288 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/detectors/data_drift/streaming/statistical_test/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     7430 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/detectors/data_drift/streaming/statistical_test/ks.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 10:24:07.517669 frouros-0.5.0/frouros/metrics/
--rw-r--r--   0 runner    (1001) docker     (122)      135 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1456 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/metrics/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     3758 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/metrics/prequential_error.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 10:24:07.517669 frouros-0.5.0/frouros/tests/
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12875 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 10:24:07.517669 frouros-0.5.0/frouros/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (122)       30 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9163 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/tests/integration/test_callback.py
--rw-r--r--   0 runner    (1001) docker     (122)     7832 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/tests/integration/test_concept_drift.py
--rw-r--r--   0 runner    (1001) docker     (122)    15055 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/tests/integration/test_data_drift.py
--rw-r--r--   0 runner    (1001) docker     (122)     1351 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/tests/integration/test_real.py
--rw-r--r--   0 runner    (1001) docker     (122)     1620 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/tests/integration/test_synthetic.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 10:24:07.517669 frouros-0.5.0/frouros/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (122)       23 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/tests/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 10:24:07.517669 frouros-0.5.0/frouros/tests/unit/metrics/
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/tests/unit/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1493 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/tests/unit/metrics/test_prequential_error.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 10:24:07.517669 frouros-0.5.0/frouros/utils/
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      833 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/utils/checks.py
--rw-r--r--   0 runner    (1001) docker     (122)    21163 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/utils/data_structures.py
--rw-r--r--   0 runner    (1001) docker     (122)      140 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (122)     7750 2023-07-18 10:23:53.000000 frouros-0.5.0/frouros/utils/stats.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 10:24:07.509668 frouros-0.5.0/frouros.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    23673 2023-07-18 10:24:07.000000 frouros-0.5.0/frouros.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     4937 2023-07-18 10:24:07.000000 frouros-0.5.0/frouros.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-18 10:24:07.000000 frouros-0.5.0/frouros.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-18 10:24:07.000000 frouros-0.5.0/frouros.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      343 2023-07-18 10:24:07.000000 frouros-0.5.0/frouros.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        8 2023-07-18 10:24:07.000000 frouros-0.5.0/frouros.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)     2139 2023-07-18 10:23:53.000000 frouros-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-18 10:24:07.517669 frouros-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1854 2023-07-18 10:23:53.000000 frouros-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-22 14:52:29.180122 frouros-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (122)     1548 2023-07-22 14:52:16.000000 frouros-0.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       15 2023-07-22 14:52:16.000000 frouros-0.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    23673 2023-07-22 14:52:29.180122 frouros-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    22052 2023-07-22 14:52:16.000000 frouros-0.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-22 14:52:29.168121 frouros-0.5.1/frouros/
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-22 14:52:29.168121 frouros-0.5.1/frouros/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (122)      312 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2047 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/callbacks/base.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-22 14:52:29.168121 frouros-0.5.1/frouros/callbacks/batch/
+-rw-r--r--   0 runner    (1001) docker     (122)      207 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/callbacks/batch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      735 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/callbacks/batch/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5358 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/callbacks/batch/permutation_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2118 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/callbacks/batch/reset.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-22 14:52:29.172121 frouros-0.5.1/frouros/callbacks/streaming/
+-rw-r--r--   0 runner    (1001) docker     (122)      232 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/callbacks/streaming/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      743 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/callbacks/streaming/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2647 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/callbacks/streaming/history.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6295 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/callbacks/streaming/msprt.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2009 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/callbacks/streaming/warning_samples.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-22 14:52:29.172121 frouros-0.5.1/frouros/common/
+-rw-r--r--   0 runner    (1001) docker     (122)       19 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      240 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/common/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-22 14:52:29.172121 frouros-0.5.1/frouros/datasets/
+-rw-r--r--   0 runner    (1001) docker     (122)       21 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5703 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/datasets/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)      466 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/datasets/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1214 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/datasets/real.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3041 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/datasets/synthetic.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-22 14:52:29.172121 frouros-0.5.1/frouros/detectors/
+-rw-r--r--   0 runner    (1001) docker     (122)       30 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/detectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2331 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/detectors/base.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-22 14:52:29.172121 frouros-0.5.1/frouros/detectors/concept_drift/
+-rw-r--r--   0 runner    (1001) docker     (122)      943 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/detectors/concept_drift/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6598 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/detectors/concept_drift/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)      285 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/detectors/concept_drift/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-22 14:52:29.172121 frouros-0.5.1/frouros/detectors/concept_drift/streaming/
+-rw-r--r--   0 runner    (1001) docker     (122)     1112 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/detectors/concept_drift/streaming/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      566 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/detectors/concept_drift/streaming/base.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-22 14:52:29.172121 frouros-0.5.1/frouros/detectors/concept_drift/streaming/change_detection/
+-rw-r--r--   0 runner    (1001) docker     (122)      513 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/detectors/concept_drift/streaming/change_detection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5856 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/detectors/concept_drift/streaming/change_detection/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10325 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/detectors/concept_drift/streaming/change_detection/bocd.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1572 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/detectors/concept_drift/streaming/change_detection/cusum.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1824 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/detectors/concept_drift/streaming/change_detection/geometric_moving_average.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1732 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/detectors/concept_drift/streaming/change_detection/page_hinkley.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-22 14:52:29.172121 frouros-0.5.1/frouros/detectors/concept_drift/streaming/statistical_process_control/
+-rw-r--r--   0 runner    (1001) docker     (122)      479 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/detectors/concept_drift/streaming/statistical_process_control/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10975 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/detectors/concept_drift/streaming/statistical_process_control/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2752 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/detectors/concept_drift/streaming/statistical_process_control/ddm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4920 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/detectors/concept_drift/streaming/statistical_process_control/ecdd.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12526 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/detectors/concept_drift/streaming/statistical_process_control/eddm.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23271 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/detectors/concept_drift/streaming/statistical_process_control/hddm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9767 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/detectors/concept_drift/streaming/statistical_process_control/rddm.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-22 14:52:29.172121 frouros-0.5.1/frouros/detectors/concept_drift/streaming/window_based/
+-rw-r--r--   0 runner    (1001) docker     (122)      285 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/detectors/concept_drift/streaming/window_based/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19431 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/detectors/concept_drift/streaming/window_based/adwin.py
+-rw-r--r--   0 runner    (1001) docker     (122)      581 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/detectors/concept_drift/streaming/window_based/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6066 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/detectors/concept_drift/streaming/window_based/kswin.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7985 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/detectors/concept_drift/streaming/window_based/stepd.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-22 14:52:29.172121 frouros-0.5.1/frouros/detectors/data_drift/
+-rw-r--r--   0 runner    (1001) docker     (122)      689 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/detectors/data_drift/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6567 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/detectors/data_drift/base.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-22 14:52:29.172121 frouros-0.5.1/frouros/detectors/data_drift/batch/
+-rw-r--r--   0 runner    (1001) docker     (122)      613 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/detectors/data_drift/batch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3754 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/detectors/data_drift/batch/base.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-22 14:52:29.176121 frouros-0.5.1/frouros/detectors/data_drift/batch/distance_based/
+-rw-r--r--   0 runner    (1001) docker     (122)      486 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/detectors/data_drift/batch/distance_based/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8889 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/detectors/data_drift/batch/distance_based/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1929 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/detectors/data_drift/batch/distance_based/bhattacharyya_distance.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1831 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/detectors/data_drift/batch/distance_based/emd.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2189 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/detectors/data_drift/batch/distance_based/hellinger_distance.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2340 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/detectors/data_drift/batch/distance_based/hi_normalized_complement.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2187 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/detectors/data_drift/batch/distance_based/js.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2199 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/detectors/data_drift/batch/distance_based/kl.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7281 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/detectors/data_drift/batch/distance_based/mmd.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2403 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/detectors/data_drift/batch/distance_based/psi.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-22 14:52:29.176121 frouros-0.5.1/frouros/detectors/data_drift/batch/statistical_test/
+-rw-r--r--   0 runner    (1001) docker     (122)      417 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/detectors/data_drift/batch/statistical_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1840 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/detectors/data_drift/batch/statistical_test/anderson_darling.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1110 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/detectors/data_drift/batch/statistical_test/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2558 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/detectors/data_drift/batch/statistical_test/chisquare.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2489 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/detectors/data_drift/batch/statistical_test/cvm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1625 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/detectors/data_drift/batch/statistical_test/ks.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1701 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/detectors/data_drift/batch/statistical_test/mann_whitney_u.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1651 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/detectors/data_drift/batch/statistical_test/welch_t_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)      428 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/detectors/data_drift/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-22 14:52:29.176121 frouros-0.5.1/frouros/detectors/data_drift/streaming/
+-rw-r--r--   0 runner    (1001) docker     (122)      183 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/detectors/data_drift/streaming/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2952 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/detectors/data_drift/streaming/base.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-22 14:52:29.176121 frouros-0.5.1/frouros/detectors/data_drift/streaming/distance_based/
+-rw-r--r--   0 runner    (1001) docker     (122)      115 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/detectors/data_drift/streaming/distance_based/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2019 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/detectors/data_drift/streaming/distance_based/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3224 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/detectors/data_drift/streaming/distance_based/mmd.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-22 14:52:29.176121 frouros-0.5.1/frouros/detectors/data_drift/streaming/statistical_test/
+-rw-r--r--   0 runner    (1001) docker     (122)      144 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/detectors/data_drift/streaming/statistical_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2288 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/detectors/data_drift/streaming/statistical_test/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7430 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/detectors/data_drift/streaming/statistical_test/ks.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-22 14:52:29.176121 frouros-0.5.1/frouros/metrics/
+-rw-r--r--   0 runner    (1001) docker     (122)      135 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1456 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/metrics/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3758 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/metrics/prequential_error.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-22 14:52:29.176121 frouros-0.5.1/frouros/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12875 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-22 14:52:29.176121 frouros-0.5.1/frouros/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (122)       30 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9068 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/tests/integration/test_callback.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7832 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/tests/integration/test_concept_drift.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15055 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/tests/integration/test_data_drift.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1351 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/tests/integration/test_real.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1620 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/tests/integration/test_synthetic.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-22 14:52:29.176121 frouros-0.5.1/frouros/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (122)       23 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-22 14:52:29.176121 frouros-0.5.1/frouros/tests/unit/metrics/
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/tests/unit/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1493 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/tests/unit/metrics/test_prequential_error.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-22 14:52:29.180122 frouros-0.5.1/frouros/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      833 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/utils/checks.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21163 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/utils/data_structures.py
+-rw-r--r--   0 runner    (1001) docker     (122)      614 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/utils/kernels.py
+-rw-r--r--   0 runner    (1001) docker     (122)      140 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7360 2023-07-22 14:52:16.000000 frouros-0.5.1/frouros/utils/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-22 14:52:29.168121 frouros-0.5.1/frouros.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    23673 2023-07-22 14:52:28.000000 frouros-0.5.1/frouros.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4962 2023-07-22 14:52:29.000000 frouros-0.5.1/frouros.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-22 14:52:28.000000 frouros-0.5.1/frouros.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-22 14:52:28.000000 frouros-0.5.1/frouros.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      343 2023-07-22 14:52:29.000000 frouros-0.5.1/frouros.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        8 2023-07-22 14:52:29.000000 frouros-0.5.1/frouros.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     2139 2023-07-22 14:52:16.000000 frouros-0.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-22 14:52:29.180122 frouros-0.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1854 2023-07-22 14:52:16.000000 frouros-0.5.1/setup.py
```

### Comparing `frouros-0.5.0/LICENSE` & `frouros-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `frouros-0.5.0/PKG-INFO` & `frouros-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frouros
-Version: 0.5.0
+Version: 0.5.1
 Summary: An open-source Python library for drift detection in machine learning systems
 Home-page: https://github.com/IFCA/frouros
 Author: Jaime Céspedes Sisniega
 Author-email: cespedes@ifca.unican.es
 Maintainer: Jaime Céspedes Sisniega
 Maintainer-email: cespedes@ifca.unican.es
 License: BSD-3-Clause
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: frouros Version: 0.5.0 Summary: An open-source
+Metadata-Version: 2.1 Name: frouros Version: 0.5.1 Summary: An open-source
 Python library for drift detection in machine learning systems Home-page:
 https://github.com/IFCA/frouros Author: Jaime CÃ©spedes Sisniega Author-email:
 cespedes@ifca.unican.es Maintainer: Jaime CÃ©spedes Sisniega Maintainer-email:
 cespedes@ifca.unican.es License: BSD-3-Clause Project-URL: homepage, https://
 frouros.readthedocs.io Project-URL: repository, https://github.com/IFCA/frouros
 Project-URL: documentation, https://frouros.readthedocs.io Project-URL:
 download, https://pypi.org/project/frouros/ Keywords: drift-detection,concept-
```

### Comparing `frouros-0.5.0/README.md` & `frouros-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `frouros-0.5.0/frouros/callbacks/base.py` & `frouros-0.5.1/frouros/callbacks/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.5.0/frouros/callbacks/batch/base.py` & `frouros-0.5.1/frouros/callbacks/batch/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.5.0/frouros/callbacks/batch/permutation_test.py` & `frouros-0.5.1/frouros/callbacks/batch/permutation_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 """Permutation test batch callback module."""
 
 import multiprocessing
 from typing import Any, Callable, Dict, List, Optional, Tuple
 
 import numpy as np  # type: ignore
-from scipy.stats import norm  # type: ignore
 
 from frouros.callbacks.batch.base import BaseCallbackBatch
-from frouros.utils.stats import permutation, z_score
+from frouros.utils.stats import permutation
 
 
 class PermutationTestDistanceBased(BaseCallbackBatch):
     """Permutation test on distance based batch callback class."""
 
     def __init__(
         self,
@@ -118,21 +117,15 @@
             statistical_args=statistic_args,
             num_permutations=num_permutations,
             num_jobs=num_jobs,
             random_state=random_state,
             verbose=verbose,
         )
         permuted_statistic = np.array(permuted_statistic)
-        # Use z-score to calculate p-value
-        observed_z_score = z_score(
-            value=observed_statistic,
-            mean=permuted_statistic.mean(),  # type: ignore
-            std=permuted_statistic.std(),  # type: ignore
-        )
-        p_value = norm.sf(np.abs(observed_z_score)) * 2
+        p_value = (permuted_statistic >= observed_statistic).mean()  # type: ignore
         return permuted_statistic, p_value
 
     def on_compare_end(self, **kwargs) -> None:
         """On compare end method."""
         X_ref, X_test = kwargs["X_ref"], kwargs["X_test"]  # noqa: N806
         observed_statistic = kwargs["result"][0]
         permuted_statistics, p_value = self._calculate_p_value(
```

### Comparing `frouros-0.5.0/frouros/callbacks/batch/reset.py` & `frouros-0.5.1/frouros/callbacks/batch/reset.py`

 * *Files identical despite different names*

### Comparing `frouros-0.5.0/frouros/callbacks/streaming/base.py` & `frouros-0.5.1/frouros/callbacks/streaming/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.5.0/frouros/callbacks/streaming/history.py` & `frouros-0.5.1/frouros/callbacks/streaming/history.py`

 * *Files identical despite different names*

### Comparing `frouros-0.5.0/frouros/callbacks/streaming/msprt.py` & `frouros-0.5.1/frouros/callbacks/streaming/msprt.py`

 * *Files identical despite different names*

### Comparing `frouros-0.5.0/frouros/callbacks/streaming/warning_samples.py` & `frouros-0.5.1/frouros/callbacks/streaming/warning_samples.py`

 * *Files identical despite different names*

### Comparing `frouros-0.5.0/frouros/datasets/base.py` & `frouros-0.5.1/frouros/datasets/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.5.0/frouros/datasets/real.py` & `frouros-0.5.1/frouros/datasets/real.py`

 * *Files identical despite different names*

### Comparing `frouros-0.5.0/frouros/datasets/synthetic.py` & `frouros-0.5.1/frouros/datasets/synthetic.py`

 * *Files identical despite different names*

### Comparing `frouros-0.5.0/frouros/detectors/base.py` & `frouros-0.5.1/frouros/detectors/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.5.0/frouros/detectors/concept_drift/__init__.py` & `frouros-0.5.1/frouros/detectors/concept_drift/__init__.py`

 * *Files identical despite different names*

### Comparing `frouros-0.5.0/frouros/detectors/concept_drift/base.py` & `frouros-0.5.1/frouros/detectors/concept_drift/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.5.0/frouros/detectors/concept_drift/streaming/__init__.py` & `frouros-0.5.1/frouros/detectors/concept_drift/streaming/__init__.py`

 * *Files identical despite different names*

### Comparing `frouros-0.5.0/frouros/detectors/concept_drift/streaming/base.py` & `frouros-0.5.1/frouros/detectors/concept_drift/streaming/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.5.0/frouros/detectors/concept_drift/streaming/change_detection/__init__.py` & `frouros-0.5.1/frouros/detectors/concept_drift/streaming/change_detection/__init__.py`

 * *Files identical despite different names*

### Comparing `frouros-0.5.0/frouros/detectors/concept_drift/streaming/change_detection/base.py` & `frouros-0.5.1/frouros/detectors/concept_drift/streaming/change_detection/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.5.0/frouros/detectors/concept_drift/streaming/change_detection/bocd.py` & `frouros-0.5.1/frouros/detectors/concept_drift/streaming/change_detection/bocd.py`

 * *Files identical despite different names*

### Comparing `frouros-0.5.0/frouros/detectors/concept_drift/streaming/change_detection/cusum.py` & `frouros-0.5.1/frouros/detectors/concept_drift/streaming/change_detection/cusum.py`

 * *Files identical despite different names*

### Comparing `frouros-0.5.0/frouros/detectors/concept_drift/streaming/change_detection/geometric_moving_average.py` & `frouros-0.5.1/frouros/detectors/concept_drift/streaming/change_detection/geometric_moving_average.py`

 * *Files identical despite different names*

### Comparing `frouros-0.5.0/frouros/detectors/concept_drift/streaming/change_detection/page_hinkley.py` & `frouros-0.5.1/frouros/detectors/concept_drift/streaming/change_detection/page_hinkley.py`

 * *Files identical despite different names*

### Comparing `frouros-0.5.0/frouros/detectors/concept_drift/streaming/statistical_process_control/base.py` & `frouros-0.5.1/frouros/detectors/concept_drift/streaming/statistical_process_control/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.5.0/frouros/detectors/concept_drift/streaming/statistical_process_control/ddm.py` & `frouros-0.5.1/frouros/detectors/concept_drift/streaming/statistical_process_control/ddm.py`

 * *Files identical despite different names*

### Comparing `frouros-0.5.0/frouros/detectors/concept_drift/streaming/statistical_process_control/ecdd.py` & `frouros-0.5.1/frouros/detectors/concept_drift/streaming/statistical_process_control/ecdd.py`

 * *Files identical despite different names*

### Comparing `frouros-0.5.0/frouros/detectors/concept_drift/streaming/statistical_process_control/eddm.py` & `frouros-0.5.1/frouros/detectors/concept_drift/streaming/statistical_process_control/eddm.py`

 * *Files identical despite different names*

### Comparing `frouros-0.5.0/frouros/detectors/concept_drift/streaming/statistical_process_control/hddm.py` & `frouros-0.5.1/frouros/detectors/concept_drift/streaming/statistical_process_control/hddm.py`

 * *Files identical despite different names*

### Comparing `frouros-0.5.0/frouros/detectors/concept_drift/streaming/statistical_process_control/rddm.py` & `frouros-0.5.1/frouros/detectors/concept_drift/streaming/statistical_process_control/rddm.py`

 * *Files identical despite different names*

### Comparing `frouros-0.5.0/frouros/detectors/concept_drift/streaming/window_based/adwin.py` & `frouros-0.5.1/frouros/detectors/concept_drift/streaming/window_based/adwin.py`

 * *Files identical despite different names*

### Comparing `frouros-0.5.0/frouros/detectors/concept_drift/streaming/window_based/base.py` & `frouros-0.5.1/frouros/detectors/concept_drift/streaming/window_based/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.5.0/frouros/detectors/concept_drift/streaming/window_based/kswin.py` & `frouros-0.5.1/frouros/detectors/concept_drift/streaming/window_based/kswin.py`

 * *Files identical despite different names*

### Comparing `frouros-0.5.0/frouros/detectors/concept_drift/streaming/window_based/stepd.py` & `frouros-0.5.1/frouros/detectors/concept_drift/streaming/window_based/stepd.py`

 * *Files identical despite different names*

### Comparing `frouros-0.5.0/frouros/detectors/data_drift/__init__.py` & `frouros-0.5.1/frouros/detectors/data_drift/__init__.py`

 * *Files identical despite different names*

### Comparing `frouros-0.5.0/frouros/detectors/data_drift/base.py` & `frouros-0.5.1/frouros/detectors/data_drift/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.5.0/frouros/detectors/data_drift/batch/__init__.py` & `frouros-0.5.1/frouros/detectors/data_drift/batch/__init__.py`

 * *Files identical despite different names*

### Comparing `frouros-0.5.0/frouros/detectors/data_drift/batch/base.py` & `frouros-0.5.1/frouros/detectors/data_drift/batch/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.5.0/frouros/detectors/data_drift/batch/distance_based/base.py` & `frouros-0.5.1/frouros/detectors/data_drift/batch/distance_based/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.5.0/frouros/detectors/data_drift/batch/distance_based/bhattacharyya_distance.py` & `frouros-0.5.1/frouros/detectors/data_drift/batch/distance_based/bhattacharyya_distance.py`

 * *Files identical despite different names*

### Comparing `frouros-0.5.0/frouros/detectors/data_drift/batch/distance_based/emd.py` & `frouros-0.5.1/frouros/detectors/data_drift/batch/distance_based/emd.py`

 * *Files identical despite different names*

### Comparing `frouros-0.5.0/frouros/detectors/data_drift/batch/distance_based/hellinger_distance.py` & `frouros-0.5.1/frouros/detectors/data_drift/batch/distance_based/hellinger_distance.py`

 * *Files identical despite different names*

### Comparing `frouros-0.5.0/frouros/detectors/data_drift/batch/distance_based/hi_normalized_complement.py` & `frouros-0.5.1/frouros/detectors/data_drift/batch/distance_based/hi_normalized_complement.py`

 * *Files identical despite different names*

### Comparing `frouros-0.5.0/frouros/detectors/data_drift/batch/distance_based/js.py` & `frouros-0.5.1/frouros/detectors/data_drift/batch/distance_based/js.py`

 * *Files identical despite different names*

### Comparing `frouros-0.5.0/frouros/detectors/data_drift/batch/distance_based/kl.py` & `frouros-0.5.1/frouros/detectors/data_drift/batch/distance_based/kl.py`

 * *Files identical despite different names*

### Comparing `frouros-0.5.0/frouros/detectors/data_drift/batch/distance_based/mmd.py` & `frouros-0.5.1/frouros/detectors/data_drift/batch/distance_based/mmd.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,39 +2,22 @@
 
 import itertools
 import math
 from typing import Callable, Generator, Optional, List, Union
 
 import numpy as np  # type: ignore
 import tqdm  # type: ignore
-from scipy.spatial.distance import cdist  # type: ignore
 
 from frouros.callbacks.batch.base import BaseCallbackBatch
 from frouros.detectors.data_drift.base import MultivariateData
 from frouros.detectors.data_drift.batch.distance_based.base import (
     BaseDistanceBased,
     DistanceResult,
 )
-
-
-def rbf_kernel(
-    X: np.ndarray, Y: np.ndarray, std: float = 1.0  # noqa: N803
-) -> np.ndarray:
-    """Radial basis function kernel between X and Y matrices.
-
-    :param X: X matrix
-    :type X: numpy.ndarray
-    :param Y: Y matrix
-    :type Y: numpy.ndarray
-    :param std: standard deviation value
-    :type std: float
-    :return: Radial basis kernel matrix
-    :rtype: numpy.ndarray
-    """
-    return np.exp(-cdist(X, Y, "sqeuclidean") / 2 * std**2)
+from frouros.utils.kernels import rbf_kernel
 
 
 class MMD(BaseDistanceBased):
     """MMD (Maximum Mean Discrepancy) [gretton2012kernel]_ detector.
 
     :References:
 
@@ -64,18 +47,14 @@
             statistical_kwargs={
                 "kernel": kernel,
             },
             callbacks=callbacks,
         )
         self.kernel = kernel
         self.chunk_size = chunk_size
-        self._chunk_size_x = None
-        self.X_chunks_combinations = None
-        self.X_num_samples = None
-        self.expected_k_xx = None
 
     @property
     def chunk_size(self) -> Optional[int]:
         """Chunk size property.
 
         :return: chunk size to use
         :rtype: int
@@ -121,137 +100,129 @@
 
     def _distance_measure(
         self,
         X_ref: np.ndarray,  # noqa: N803
         X: np.ndarray,  # noqa: N803
         **kwargs,
     ) -> DistanceResult:
-        mmd = self._mmd(X=X_ref, Y=X, kernel=self.kernel, **kwargs)
+        mmd = self._mmd(
+            X=X_ref,
+            Y=X,
+            kernel=self.kernel,
+            chunk_size=self.chunk_size,
+            **kwargs,
+        )
         distance_test = DistanceResult(distance=mmd)
         return distance_test
 
-    def _fit(
-        self,
-        X: np.ndarray,  # noqa: N803
-        **kwargs,
-    ) -> None:
-        super()._fit(X=X)
-        # Add dimension only for the kernel calculation (if dim == 1)
-        if X.ndim == 1:
-            X = np.expand_dims(X, axis=1)  # noqa: N806
-        self.X_num_samples = len(self.X_ref)  # type: ignore # noqa: N806
-
-        self._chunk_size_x = (
-            self.X_num_samples
-            if self.chunk_size is None
-            else self.chunk_size  # type: ignore
-        )
-
-        X_chunks = self._get_chunks(  # noqa: N806
-            data=X,
-            chunk_size=self._chunk_size_x,  # type: ignore
-        )
-        xx_chunks_combinations = itertools.product(X_chunks, repeat=2)  # noqa: N806
-
-        if kwargs.get("verbose", False):
-            num_chunks = (
-                math.ceil(self.X_num_samples / self._chunk_size_x) ** 2  # type: ignore
-            )
-            xx_chunks_combinations = tqdm.tqdm(
-                xx_chunks_combinations,
-                total=num_chunks,
-            )
-
-        k_xx_sum = (
-            self._compute_kernel(
-                chunk_combinations=xx_chunks_combinations,  # type: ignore
-                kernel=self.kernel,
-            )
-            # Remove diagonal (j!=i case)
-            - self.X_num_samples  # type: ignore
-        )
-
-        self.expected_k_xx = k_xx_sum / (  # type: ignore
-            self.X_num_samples * (self.X_num_samples - 1)  # type: ignore
-        )
-
     @staticmethod
     def _compute_kernel(chunk_combinations: Generator, kernel: Callable) -> float:
         k_sum = np.array([kernel(*chunk).sum() for chunk in chunk_combinations]).sum()
         return k_sum
 
     @staticmethod
     def _get_chunks(data: np.ndarray, chunk_size: int) -> Generator:
         chunks = (
             data[i : i + chunk_size]  # noqa: E203
             for i in range(0, len(data), chunk_size)
         )
         return chunks
 
+    @staticmethod
     def _mmd(  # pylint: disable=too-many-locals
-        self,
         X: np.ndarray,  # noqa: N803
         Y: np.ndarray,
         *,
         kernel: Callable,
         **kwargs,
     ) -> float:  # noqa: N803
         # Only check for X dimension (X == Y dim comparison has been already made)
         if X.ndim == 1:
             X = np.expand_dims(X, axis=1)  # noqa: N806
             Y = np.expand_dims(Y, axis=1)  # noqa: N806
 
-        X_chunks = self._get_chunks(  # noqa: N806
-            data=X,
-            chunk_size=self._chunk_size_x,  # type: ignore
+        x_num_samples = len(X)  # noqa: N806
+        chunk_size_x = (
+            kwargs["chunk_size"]
+            if "chunk_size" in kwargs and kwargs["chunk_size"] is not None
+            else x_num_samples
+        )
+        x_chunks, x_chunks_copy = itertools.tee(  # noqa: N806
+            MMD._get_chunks(
+                data=X,
+                chunk_size=chunk_size_x,  # type: ignore
+            ),
+            2,
         )
         y_num_samples = len(Y)  # noqa: N806
-        chunk_size_y = y_num_samples if self.chunk_size is None else self.chunk_size
+        chunk_size_y = (
+            kwargs["chunk_size"]
+            if "chunk_size" in kwargs and kwargs["chunk_size"] is not None
+            else y_num_samples
+        )
         y_chunks, y_chunks_copy = itertools.tee(  # noqa: N806
-            self._get_chunks(
+            MMD._get_chunks(
                 data=Y,
                 chunk_size=chunk_size_y,  # type: ignore
             ),
             2,
         )
+        x_chunks_combinations = itertools.product(  # noqa: N806
+            x_chunks,
+            repeat=2,
+        )
         y_chunks_combinations = itertools.product(  # noqa: N806
             y_chunks,
             repeat=2,
         )
         xy_chunks_combinations = itertools.product(  # noqa: N806
-            X_chunks,
+            x_chunks_copy,
             y_chunks_copy,
         )
 
         if kwargs.get("verbose", False):
+            num_chunks_x = math.ceil(x_num_samples / chunk_size_x)  # type: ignore
             num_chunks_y = math.ceil(y_num_samples / chunk_size_y)  # type: ignore
+            num_chunks_x_combinations = num_chunks_x**2
             num_chunks_y_combinations = num_chunks_y**2
             num_chunks_xy = (
-                math.ceil(len(X) / self._chunk_size_x) * num_chunks_y  # type: ignore
+                math.ceil(len(X) / chunk_size_x) * num_chunks_y  # type: ignore
+            )
+            x_chunks_combinations = tqdm.tqdm(
+                x_chunks_combinations,
+                total=num_chunks_x_combinations,
             )
             y_chunks_combinations = tqdm.tqdm(
                 y_chunks_combinations,
                 total=num_chunks_y_combinations,
             )
             xy_chunks_combinations = tqdm.tqdm(
                 xy_chunks_combinations,
                 total=num_chunks_xy,
             )
 
+        k_xx_sum = (
+            MMD._compute_kernel(
+                chunk_combinations=x_chunks_combinations,  # type: ignore
+                kernel=kernel,
+            )
+            # Remove diagonal (j!=i case)
+            - x_num_samples  # type: ignore
+        )
         k_yy_sum = (
-            self._compute_kernel(
+            MMD._compute_kernel(
                 chunk_combinations=y_chunks_combinations,  # type: ignore
                 kernel=kernel,
             )
             # Remove diagonal (j!=i case)
             - y_num_samples  # type: ignore
         )
-        k_xy_sum = self._compute_kernel(
+        k_xy_sum = MMD._compute_kernel(
             chunk_combinations=xy_chunks_combinations,  # type: ignore
             kernel=kernel,
         )
         mmd = (
-            self.expected_k_xx  # type: ignore
+            +k_xx_sum / (x_num_samples * (x_num_samples - 1))
             + k_yy_sum / (y_num_samples * (y_num_samples - 1))
-            - 2 * k_xy_sum / (self.X_num_samples * y_num_samples)  # type: ignore
+            - 2 * k_xy_sum / (x_num_samples * y_num_samples)  # type: ignore
         )
         return mmd
```

### Comparing `frouros-0.5.0/frouros/detectors/data_drift/batch/distance_based/psi.py` & `frouros-0.5.1/frouros/detectors/data_drift/batch/distance_based/psi.py`

 * *Files identical despite different names*

### Comparing `frouros-0.5.0/frouros/detectors/data_drift/batch/statistical_test/anderson_darling.py` & `frouros-0.5.1/frouros/detectors/data_drift/batch/statistical_test/anderson_darling.py`

 * *Files identical despite different names*

### Comparing `frouros-0.5.0/frouros/detectors/data_drift/batch/statistical_test/base.py` & `frouros-0.5.1/frouros/detectors/data_drift/batch/statistical_test/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.5.0/frouros/detectors/data_drift/batch/statistical_test/chisquare.py` & `frouros-0.5.1/frouros/detectors/data_drift/batch/statistical_test/chisquare.py`

 * *Files identical despite different names*

### Comparing `frouros-0.5.0/frouros/detectors/data_drift/batch/statistical_test/cvm.py` & `frouros-0.5.1/frouros/detectors/data_drift/batch/statistical_test/cvm.py`

 * *Files identical despite different names*

### Comparing `frouros-0.5.0/frouros/detectors/data_drift/batch/statistical_test/ks.py` & `frouros-0.5.1/frouros/detectors/data_drift/batch/statistical_test/ks.py`

 * *Files identical despite different names*

### Comparing `frouros-0.5.0/frouros/detectors/data_drift/batch/statistical_test/mann_whitney_u.py` & `frouros-0.5.1/frouros/detectors/data_drift/batch/statistical_test/mann_whitney_u.py`

 * *Files identical despite different names*

### Comparing `frouros-0.5.0/frouros/detectors/data_drift/batch/statistical_test/welch_t_test.py` & `frouros-0.5.1/frouros/detectors/data_drift/batch/statistical_test/welch_t_test.py`

 * *Files identical despite different names*

### Comparing `frouros-0.5.0/frouros/detectors/data_drift/streaming/base.py` & `frouros-0.5.1/frouros/detectors/data_drift/streaming/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.5.0/frouros/detectors/data_drift/streaming/distance_based/base.py` & `frouros-0.5.1/frouros/detectors/data_drift/streaming/distance_based/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.5.0/frouros/detectors/data_drift/streaming/distance_based/mmd.py` & `frouros-0.5.1/frouros/detectors/data_drift/streaming/distance_based/mmd.py`

 * *Files identical despite different names*

### Comparing `frouros-0.5.0/frouros/detectors/data_drift/streaming/statistical_test/base.py` & `frouros-0.5.1/frouros/detectors/data_drift/streaming/statistical_test/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.5.0/frouros/detectors/data_drift/streaming/statistical_test/ks.py` & `frouros-0.5.1/frouros/detectors/data_drift/streaming/statistical_test/ks.py`

 * *Files identical despite different names*

### Comparing `frouros-0.5.0/frouros/metrics/base.py` & `frouros-0.5.1/frouros/metrics/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.5.0/frouros/metrics/prequential_error.py` & `frouros-0.5.1/frouros/metrics/prequential_error.py`

 * *Files identical despite different names*

### Comparing `frouros-0.5.0/frouros/tests/conftest.py` & `frouros-0.5.1/frouros/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `frouros-0.5.0/frouros/tests/integration/test_callback.py` & `frouros-0.5.1/frouros/tests/integration/test_callback.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,21 +50,21 @@
 from frouros.detectors.data_drift.streaming import MMD as MMDStreaming  # noqa: N811
 
 
 @pytest.mark.parametrize(
     "detector_class, expected_distance, expected_p_value",
     [
         (BhattacharyyaDistance, 0.55516059, 0.0),
-        (EMD, 3.85346006, 9.21632493e-101),
-        (HellingerDistance, 0.74509099, 3.13808126e-50),
-        (HINormalizedComplement, 0.78, 1.31340683e-55),
-        (JS, 0.67010107, 2.30485343e-63),
-        (KL, np.inf, np.nan),
-        (MMD, 0.69509004, 2.53277069e-137),
-        (PSI, 461.20379435, 4.45088795e-238),
+        (EMD, 3.85346006, 0.0),
+        (HellingerDistance, 0.74509099, 0.0),
+        (HINormalizedComplement, 0.78, 0.0),
+        (JS, 0.67010107, 0.0),
+        (KL, np.inf, 0.06),
+        (MMD, 0.69509004, 0.0),
+        (PSI, 461.20379435, 0.0),
     ],
 )
 def test_batch_permutation_test_data_univariate_different_distribution(
     X_ref_univariate: np.ndarray,  # noqa: N803
     X_test_univariate: np.ndarray,
     detector_class: BaseDataDriftBatch,
     expected_distance: float,
@@ -99,15 +99,14 @@
     _ = detector.fit(X=X_ref_univariate)
     distance, callback_logs = detector.compare(X=X_test_univariate)
 
     assert np.isclose(distance, expected_distance)
     assert np.isclose(
         callback_logs[permutation_test_name]["p_value"],
         expected_p_value,
-        equal_nan=True,
     )
 
 
 @pytest.mark.parametrize(
     "detector_class",
     [CVMTest, KSTest, WelchTTest],
 )
```

### Comparing `frouros-0.5.0/frouros/tests/integration/test_concept_drift.py` & `frouros-0.5.1/frouros/tests/integration/test_concept_drift.py`

 * *Files identical despite different names*

### Comparing `frouros-0.5.0/frouros/tests/integration/test_data_drift.py` & `frouros-0.5.1/frouros/tests/integration/test_data_drift.py`

 * *Files identical despite different names*

### Comparing `frouros-0.5.0/frouros/tests/integration/test_real.py` & `frouros-0.5.1/frouros/tests/integration/test_real.py`

 * *Files identical despite different names*

### Comparing `frouros-0.5.0/frouros/tests/integration/test_synthetic.py` & `frouros-0.5.1/frouros/tests/integration/test_synthetic.py`

 * *Files identical despite different names*

### Comparing `frouros-0.5.0/frouros/tests/unit/metrics/test_prequential_error.py` & `frouros-0.5.1/frouros/tests/unit/metrics/test_prequential_error.py`

 * *Files identical despite different names*

### Comparing `frouros-0.5.0/frouros/utils/checks.py` & `frouros-0.5.1/frouros/utils/checks.py`

 * *Files identical despite different names*

### Comparing `frouros-0.5.0/frouros/utils/data_structures.py` & `frouros-0.5.1/frouros/utils/data_structures.py`

 * *Files identical despite different names*

### Comparing `frouros-0.5.0/frouros/utils/stats.py` & `frouros-0.5.1/frouros/utils/stats.py`

 * *Files 4% similar despite different names*

```diff
@@ -259,26 +259,7 @@
     with Pool(processes=num_jobs) as pool:
         permuted_statistics = pool.starmap_async(
             partial(statistic, **statistical_args),
             iterable=tqdm(permuted_data) if verbose else permuted_data,
         ).get()
 
     return permuted_statistics
-
-
-def z_score(
-    value: np.ndarray,
-    mean: float,
-    std: float,
-) -> np.ndarray:
-    """Z-score method.
-
-    :param value: value to use to compute the z-score
-    :type value: np.ndarray
-    :param mean: mean value
-    :type mean: float
-    :param std: standard deviation value
-    :type std: float
-    :return: z-score
-    :rtype: np.ndarray
-    """
-    return (value - mean) / std
```

### Comparing `frouros-0.5.0/frouros.egg-info/PKG-INFO` & `frouros-0.5.1/frouros.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frouros
-Version: 0.5.0
+Version: 0.5.1
 Summary: An open-source Python library for drift detection in machine learning systems
 Home-page: https://github.com/IFCA/frouros
 Author: Jaime Céspedes Sisniega
 Author-email: cespedes@ifca.unican.es
 Maintainer: Jaime Céspedes Sisniega
 Maintainer-email: cespedes@ifca.unican.es
 License: BSD-3-Clause
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: frouros Version: 0.5.0 Summary: An open-source
+Metadata-Version: 2.1 Name: frouros Version: 0.5.1 Summary: An open-source
 Python library for drift detection in machine learning systems Home-page:
 https://github.com/IFCA/frouros Author: Jaime CÃ©spedes Sisniega Author-email:
 cespedes@ifca.unican.es Maintainer: Jaime CÃ©spedes Sisniega Maintainer-email:
 cespedes@ifca.unican.es License: BSD-3-Clause Project-URL: homepage, https://
 frouros.readthedocs.io Project-URL: repository, https://github.com/IFCA/frouros
 Project-URL: documentation, https://frouros.readthedocs.io Project-URL:
 download, https://pypi.org/project/frouros/ Keywords: drift-detection,concept-
```

### Comparing `frouros-0.5.0/frouros.egg-info/SOURCES.txt` & `frouros-0.5.1/frouros.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -97,9 +97,10 @@
 frouros/tests/integration/test_synthetic.py
 frouros/tests/unit/__init__.py
 frouros/tests/unit/metrics/__init__.py
 frouros/tests/unit/metrics/test_prequential_error.py
 frouros/utils/__init__.py
 frouros/utils/checks.py
 frouros/utils/data_structures.py
+frouros/utils/kernels.py
 frouros/utils/logger.py
 frouros/utils/stats.py
```

### Comparing `frouros-0.5.0/pyproject.toml` & `frouros-0.5.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "frouros"
-version = "0.5.0"
+version = "0.5.1"
 description = "An open-source Python library for drift detection in machine learning systems"
 authors = [
     {name = "Jaime Céspedes Sisniega", email = "cespedes@ifca.unican.es"}
 ]
 maintainers = [
     {name = "Jaime Céspedes Sisniega", email = "cespedes@ifca.unican.es"}
 ]
```

### Comparing `frouros-0.5.0/setup.py` & `frouros-0.5.1/setup.py`

 * *Files identical despite different names*

