# Comparing `tmp/scope-rl-0.1.1.tar.gz` & `tmp/scope-rl-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scope-rl-0.1.1.tar", last modified: Thu Jun 29 01:48:01 2023, max compression
+gzip compressed data, was "scope-rl-0.1.2.tar", last modified: Sat Jul 22 01:34:31 2023, max compression
```

## Comparing `scope-rl-0.1.1.tar` & `scope-rl-0.1.2.tar`

### file list

```diff
@@ -1,96 +1,96 @@
-drwxr-xr-x   0 haruka     (501) staff       (20)        0 2023-06-29 01:48:01.223026 scope-rl-0.1.1/
--rw-r--r--   0 haruka     (501) staff       (20)     1483 2023-06-16 01:19:44.000000 scope-rl-0.1.1/CONTRIBUTING.md
--rw-r--r--   0 haruka     (501) staff       (20)     1290 2023-06-16 01:19:44.000000 scope-rl-0.1.1/FrequentlyAskedQuestions.md
--rw-r--r--   0 haruka     (501) staff       (20)    11420 2023-06-16 01:19:44.000000 scope-rl-0.1.1/LICENSE
--rw-r--r--   0 haruka     (501) staff       (20)       42 2023-06-16 01:19:44.000000 scope-rl-0.1.1/MANIFEST.in
--rw-r--r--   0 haruka     (501) staff       (20)    29865 2023-06-29 01:48:01.223125 scope-rl-0.1.1/PKG-INFO
--rw-r--r--   0 haruka     (501) staff       (20)    28806 2023-06-28 23:25:00.000000 scope-rl-0.1.1/README.md
-drwxr-xr-x   0 haruka     (501) staff       (20)        0 2023-06-29 01:48:01.204825 scope-rl-0.1.1/basicgym/
--rw-r--r--   0 haruka     (501) staff       (20)     1013 2023-06-16 01:19:44.000000 scope-rl-0.1.1/basicgym/__init__.py
-drwxr-xr-x   0 haruka     (501) staff       (20)        0 2023-06-29 01:48:01.205207 scope-rl-0.1.1/basicgym/envs/
--rw-r--r--   0 haruka     (501) staff       (20)      249 2023-06-16 01:19:44.000000 scope-rl-0.1.1/basicgym/envs/__init__.py
-drwxr-xr-x   0 haruka     (501) staff       (20)        0 2023-06-29 01:48:01.205623 scope-rl-0.1.1/basicgym/envs/simulator/
--rw-r--r--   0 haruka     (501) staff       (20)      339 2023-06-16 01:19:44.000000 scope-rl-0.1.1/basicgym/envs/simulator/__init__.py
--rw-r--r--   0 haruka     (501) staff       (20)     2341 2023-06-16 01:19:44.000000 scope-rl-0.1.1/basicgym/envs/simulator/base.py
--rw-r--r--   0 haruka     (501) staff       (20)     5633 2023-06-16 01:19:44.000000 scope-rl-0.1.1/basicgym/envs/simulator/function.py
--rw-r--r--   0 haruka     (501) staff       (20)    12192 2023-06-16 01:19:44.000000 scope-rl-0.1.1/basicgym/envs/synthetic.py
--rw-r--r--   0 haruka     (501) staff       (20)      306 2023-06-16 01:19:44.000000 scope-rl-0.1.1/basicgym/types.py
--rw-r--r--   0 haruka     (501) staff       (20)     2051 2023-06-16 01:19:44.000000 scope-rl-0.1.1/basicgym/utils.py
--rw-r--r--   0 haruka     (501) staff       (20)      194 2023-06-16 01:19:44.000000 scope-rl-0.1.1/basicgym/version.py
-drwxr-xr-x   0 haruka     (501) staff       (20)        0 2023-06-29 01:48:01.206529 scope-rl-0.1.1/recgym/
--rw-r--r--   0 haruka     (501) staff       (20)      548 2023-06-16 01:19:45.000000 scope-rl-0.1.1/recgym/__init__.py
-drwxr-xr-x   0 haruka     (501) staff       (20)        0 2023-06-29 01:48:01.206821 scope-rl-0.1.1/recgym/envs/
--rw-r--r--   0 haruka     (501) staff       (20)      237 2023-06-16 01:19:45.000000 scope-rl-0.1.1/recgym/envs/__init__.py
--rw-r--r--   0 haruka     (501) staff       (20)    12828 2023-06-16 01:19:45.000000 scope-rl-0.1.1/recgym/envs/rec.py
-drwxr-xr-x   0 haruka     (501) staff       (20)        0 2023-06-29 01:48:01.207235 scope-rl-0.1.1/recgym/envs/simulator/
--rw-r--r--   0 haruka     (501) staff       (20)      257 2023-06-16 01:19:45.000000 scope-rl-0.1.1/recgym/envs/simulator/__init__.py
--rw-r--r--   0 haruka     (501) staff       (20)     2757 2023-06-16 01:19:45.000000 scope-rl-0.1.1/recgym/envs/simulator/base.py
--rw-r--r--   0 haruka     (501) staff       (20)     5363 2023-06-16 01:19:45.000000 scope-rl-0.1.1/recgym/envs/simulator/function.py
--rw-r--r--   0 haruka     (501) staff       (20)      333 2023-06-16 01:19:45.000000 scope-rl-0.1.1/recgym/types.py
--rw-r--r--   0 haruka     (501) staff       (20)     2052 2023-06-16 01:19:45.000000 scope-rl-0.1.1/recgym/utils.py
--rw-r--r--   0 haruka     (501) staff       (20)      194 2023-06-16 01:19:45.000000 scope-rl-0.1.1/recgym/version.py
--rw-r--r--   0 haruka     (501) staff       (20)      193 2023-06-26 23:52:14.000000 scope-rl-0.1.1/requirements.txt
-drwxr-xr-x   0 haruka     (501) staff       (20)        0 2023-06-29 01:48:01.207777 scope-rl-0.1.1/rtbgym/
--rw-r--r--   0 haruka     (501) staff       (20)     1264 2023-06-16 01:19:45.000000 scope-rl-0.1.1/rtbgym/__init__.py
-drwxr-xr-x   0 haruka     (501) staff       (20)        0 2023-06-29 01:48:01.208438 scope-rl-0.1.1/rtbgym/envs/
--rw-r--r--   0 haruka     (501) staff       (20)      314 2023-06-16 01:19:45.000000 scope-rl-0.1.1/rtbgym/envs/__init__.py
--rw-r--r--   0 haruka     (501) staff       (20)    18863 2023-06-27 00:32:37.000000 scope-rl-0.1.1/rtbgym/envs/rtb.py
-drwxr-xr-x   0 haruka     (501) staff       (20)        0 2023-06-29 01:48:01.209348 scope-rl-0.1.1/rtbgym/envs/simulator/
--rw-r--r--   0 haruka     (501) staff       (20)      621 2023-06-16 01:19:45.000000 scope-rl-0.1.1/rtbgym/envs/simulator/__init__.py
--rw-r--r--   0 haruka     (501) staff       (20)     7529 2023-06-16 01:19:45.000000 scope-rl-0.1.1/rtbgym/envs/simulator/base.py
--rw-r--r--   0 haruka     (501) staff       (20)    16332 2023-06-16 01:19:45.000000 scope-rl-0.1.1/rtbgym/envs/simulator/bidder.py
--rw-r--r--   0 haruka     (501) staff       (20)    20994 2023-06-27 04:53:01.000000 scope-rl-0.1.1/rtbgym/envs/simulator/function.py
--rw-r--r--   0 haruka     (501) staff       (20)    21598 2023-06-27 00:32:44.000000 scope-rl-0.1.1/rtbgym/envs/simulator/rtb_synthetic.py
--rw-r--r--   0 haruka     (501) staff       (20)    13398 2023-06-16 01:19:45.000000 scope-rl-0.1.1/rtbgym/envs/wrapper_rtb.py
--rw-r--r--   0 haruka     (501) staff       (20)      411 2023-06-16 01:19:45.000000 scope-rl-0.1.1/rtbgym/types.py
--rw-r--r--   0 haruka     (501) staff       (20)     4788 2023-06-16 01:19:45.000000 scope-rl-0.1.1/rtbgym/utils.py
--rw-r--r--   0 haruka     (501) staff       (20)      194 2023-06-16 01:19:45.000000 scope-rl-0.1.1/rtbgym/version.py
-drwxr-xr-x   0 haruka     (501) staff       (20)        0 2023-06-29 01:48:01.210856 scope-rl-0.1.1/scope_rl/
--rw-r--r--   0 haruka     (501) staff       (20)      213 2023-06-16 01:19:45.000000 scope-rl-0.1.1/scope_rl/__init__.py
-drwxr-xr-x   0 haruka     (501) staff       (20)        0 2023-06-29 01:48:01.212076 scope-rl-0.1.1/scope_rl/dataset/
--rw-r--r--   0 haruka     (501) staff       (20)      332 2023-06-16 01:19:45.000000 scope-rl-0.1.1/scope_rl/dataset/__init__.py
--rw-r--r--   0 haruka     (501) staff       (20)     7018 2023-06-16 01:19:45.000000 scope-rl-0.1.1/scope_rl/dataset/base.py
--rw-r--r--   0 haruka     (501) staff       (20)    49546 2023-06-27 05:43:29.000000 scope-rl-0.1.1/scope_rl/dataset/synthetic.py
-drwxr-xr-x   0 haruka     (501) staff       (20)        0 2023-06-29 01:48:01.215244 scope-rl-0.1.1/scope_rl/ope/
--rw-r--r--   0 haruka     (501) staff       (20)     1046 2023-06-16 01:19:45.000000 scope-rl-0.1.1/scope_rl/ope/__init__.py
-drwxr-xr-x   0 haruka     (501) staff       (20)        0 2023-06-29 01:48:01.217632 scope-rl-0.1.1/scope_rl/ope/continuous/
--rw-r--r--   0 haruka     (501) staff       (20)     2233 2023-06-16 01:19:45.000000 scope-rl-0.1.1/scope_rl/ope/continuous/__init__.py
--rw-r--r--   0 haruka     (501) staff       (20)    70031 2023-06-27 08:03:25.000000 scope-rl-0.1.1/scope_rl/ope/continuous/basic_estimators.py
--rw-r--r--   0 haruka     (501) staff       (20)    73299 2023-06-16 01:19:45.000000 scope-rl-0.1.1/scope_rl/ope/continuous/cumulative_distribution_estimators.py
--rw-r--r--   0 haruka     (501) staff       (20)   131052 2023-06-27 08:00:33.000000 scope-rl-0.1.1/scope_rl/ope/continuous/marginal_estimators.py
-drwxr-xr-x   0 haruka     (501) staff       (20)        0 2023-06-29 01:48:01.218811 scope-rl-0.1.1/scope_rl/ope/discrete/
--rw-r--r--   0 haruka     (501) staff       (20)     2227 2023-06-16 01:19:45.000000 scope-rl-0.1.1/scope_rl/ope/discrete/__init__.py
--rw-r--r--   0 haruka     (501) staff       (20)    62995 2023-06-16 01:19:45.000000 scope-rl-0.1.1/scope_rl/ope/discrete/basic_estimators.py
--rw-r--r--   0 haruka     (501) staff       (20)    68685 2023-06-16 01:19:45.000000 scope-rl-0.1.1/scope_rl/ope/discrete/cumulative_distribution_estimators.py
--rw-r--r--   0 haruka     (501) staff       (20)   125009 2023-06-27 07:57:09.000000 scope-rl-0.1.1/scope_rl/ope/discrete/marginal_estimators.py
--rw-r--r--   0 haruka     (501) staff       (20)    37164 2023-06-16 01:19:45.000000 scope-rl-0.1.1/scope_rl/ope/estimators_base.py
--rw-r--r--   0 haruka     (501) staff       (20)   129251 2023-06-27 06:29:10.000000 scope-rl-0.1.1/scope_rl/ope/input.py
--rw-r--r--   0 haruka     (501) staff       (20)    54713 2023-06-16 01:19:45.000000 scope-rl-0.1.1/scope_rl/ope/online.py
--rw-r--r--   0 haruka     (501) staff       (20)   292304 2023-06-27 06:12:50.000000 scope-rl-0.1.1/scope_rl/ope/ope.py
--rw-r--r--   0 haruka     (501) staff       (20)   523679 2023-06-27 06:27:20.000000 scope-rl-0.1.1/scope_rl/ope/ops.py
-drwxr-xr-x   0 haruka     (501) staff       (20)        0 2023-06-29 01:48:01.222074 scope-rl-0.1.1/scope_rl/ope/weight_value_learning/
--rw-r--r--   0 haruka     (501) staff       (20)     2492 2023-06-16 01:19:45.000000 scope-rl-0.1.1/scope_rl/ope/weight_value_learning/__init__.py
--rw-r--r--   0 haruka     (501) staff       (20)    49122 2023-06-16 01:19:45.000000 scope-rl-0.1.1/scope_rl/ope/weight_value_learning/augmented_lagrangian_learning_continuous.py
--rw-r--r--   0 haruka     (501) staff       (20)    50800 2023-06-16 01:19:45.000000 scope-rl-0.1.1/scope_rl/ope/weight_value_learning/augmented_lagrangian_learning_discrete.py
--rw-r--r--   0 haruka     (501) staff       (20)      985 2023-06-16 01:19:45.000000 scope-rl-0.1.1/scope_rl/ope/weight_value_learning/base.py
--rw-r--r--   0 haruka     (501) staff       (20)     7892 2023-06-16 01:19:45.000000 scope-rl-0.1.1/scope_rl/ope/weight_value_learning/function.py
--rw-r--r--   0 haruka     (501) staff       (20)    34834 2023-06-16 01:19:45.000000 scope-rl-0.1.1/scope_rl/ope/weight_value_learning/minimax_value_learning_continuous.py
--rw-r--r--   0 haruka     (501) staff       (20)    36314 2023-06-16 01:19:45.000000 scope-rl-0.1.1/scope_rl/ope/weight_value_learning/minimax_value_learning_discrete.py
--rw-r--r--   0 haruka     (501) staff       (20)    41939 2023-06-16 01:19:45.000000 scope-rl-0.1.1/scope_rl/ope/weight_value_learning/minimax_weight_learning_continuous.py
--rw-r--r--   0 haruka     (501) staff       (20)    42102 2023-06-16 01:19:45.000000 scope-rl-0.1.1/scope_rl/ope/weight_value_learning/minimax_weight_learning_discrete.py
-drwxr-xr-x   0 haruka     (501) staff       (20)        0 2023-06-29 01:48:01.222782 scope-rl-0.1.1/scope_rl/policy/
--rw-r--r--   0 haruka     (501) staff       (20)      981 2023-06-16 01:19:45.000000 scope-rl-0.1.1/scope_rl/policy/__init__.py
--rw-r--r--   0 haruka     (501) staff       (20)     9256 2023-06-16 01:19:45.000000 scope-rl-0.1.1/scope_rl/policy/encoder.py
--rw-r--r--   0 haruka     (501) staff       (20)    32731 2023-06-16 01:19:45.000000 scope-rl-0.1.1/scope_rl/policy/head.py
--rw-r--r--   0 haruka     (501) staff       (20)    25869 2023-06-16 01:19:45.000000 scope-rl-0.1.1/scope_rl/policy/orl.py
--rw-r--r--   0 haruka     (501) staff       (20)      334 2023-06-16 01:19:45.000000 scope-rl-0.1.1/scope_rl/types.py
--rw-r--r--   0 haruka     (501) staff       (20)    30939 2023-06-16 01:19:45.000000 scope-rl-0.1.1/scope_rl/utils.py
--rw-r--r--   0 haruka     (501) staff       (20)      194 2023-06-28 23:30:27.000000 scope-rl-0.1.1/scope_rl/version.py
-drwxr-xr-x   0 haruka     (501) staff       (20)        0 2023-06-29 01:48:01.211562 scope-rl-0.1.1/scope_rl.egg-info/
--rw-r--r--   0 haruka     (501) staff       (20)    29865 2023-06-29 01:48:01.000000 scope-rl-0.1.1/scope_rl.egg-info/PKG-INFO
--rw-r--r--   0 haruka     (501) staff       (20)     2374 2023-06-29 01:48:01.000000 scope-rl-0.1.1/scope_rl.egg-info/SOURCES.txt
--rw-r--r--   0 haruka     (501) staff       (20)        1 2023-06-29 01:48:01.000000 scope-rl-0.1.1/scope_rl.egg-info/dependency_links.txt
--rw-r--r--   0 haruka     (501) staff       (20)      194 2023-06-29 01:48:01.000000 scope-rl-0.1.1/scope_rl.egg-info/requires.txt
--rw-r--r--   0 haruka     (501) staff       (20)       32 2023-06-29 01:48:01.000000 scope-rl-0.1.1/scope_rl.egg-info/top_level.txt
--rw-r--r--   0 haruka     (501) staff       (20)       74 2023-06-29 01:48:01.223391 scope-rl-0.1.1/setup.cfg
--rw-r--r--   0 haruka     (501) staff       (20)     1729 2023-06-28 23:03:04.000000 scope-rl-0.1.1/setup.py
+drwxr-xr-x   0 haruka     (501) staff       (20)        0 2023-07-22 01:34:31.841663 scope-rl-0.1.2/
+-rw-r--r--   0 haruka     (501) staff       (20)     1483 2023-06-16 01:19:44.000000 scope-rl-0.1.2/CONTRIBUTING.md
+-rw-r--r--   0 haruka     (501) staff       (20)     1318 2023-07-21 11:27:55.000000 scope-rl-0.1.2/FrequentlyAskedQuestions.md
+-rw-r--r--   0 haruka     (501) staff       (20)    11420 2023-06-16 01:19:44.000000 scope-rl-0.1.2/LICENSE
+-rw-r--r--   0 haruka     (501) staff       (20)       42 2023-06-16 01:19:44.000000 scope-rl-0.1.2/MANIFEST.in
+-rw-r--r--   0 haruka     (501) staff       (20)    30919 2023-07-22 01:34:31.841778 scope-rl-0.1.2/PKG-INFO
+-rw-r--r--   0 haruka     (501) staff       (20)    29860 2023-07-21 23:24:19.000000 scope-rl-0.1.2/README.md
+drwxr-xr-x   0 haruka     (501) staff       (20)        0 2023-07-22 01:34:31.825568 scope-rl-0.1.2/basicgym/
+-rw-r--r--   0 haruka     (501) staff       (20)     1013 2023-06-16 01:19:44.000000 scope-rl-0.1.2/basicgym/__init__.py
+drwxr-xr-x   0 haruka     (501) staff       (20)        0 2023-07-22 01:34:31.825972 scope-rl-0.1.2/basicgym/envs/
+-rw-r--r--   0 haruka     (501) staff       (20)      249 2023-06-16 01:19:44.000000 scope-rl-0.1.2/basicgym/envs/__init__.py
+drwxr-xr-x   0 haruka     (501) staff       (20)        0 2023-07-22 01:34:31.826410 scope-rl-0.1.2/basicgym/envs/simulator/
+-rw-r--r--   0 haruka     (501) staff       (20)      339 2023-06-16 01:19:44.000000 scope-rl-0.1.2/basicgym/envs/simulator/__init__.py
+-rw-r--r--   0 haruka     (501) staff       (20)     2341 2023-06-16 01:19:44.000000 scope-rl-0.1.2/basicgym/envs/simulator/base.py
+-rw-r--r--   0 haruka     (501) staff       (20)     5633 2023-06-16 01:19:44.000000 scope-rl-0.1.2/basicgym/envs/simulator/function.py
+-rw-r--r--   0 haruka     (501) staff       (20)    12192 2023-06-16 01:19:44.000000 scope-rl-0.1.2/basicgym/envs/synthetic.py
+-rw-r--r--   0 haruka     (501) staff       (20)      306 2023-06-16 01:19:44.000000 scope-rl-0.1.2/basicgym/types.py
+-rw-r--r--   0 haruka     (501) staff       (20)     2051 2023-06-16 01:19:44.000000 scope-rl-0.1.2/basicgym/utils.py
+-rw-r--r--   0 haruka     (501) staff       (20)      194 2023-06-16 01:19:44.000000 scope-rl-0.1.2/basicgym/version.py
+drwxr-xr-x   0 haruka     (501) staff       (20)        0 2023-07-22 01:34:31.827327 scope-rl-0.1.2/recgym/
+-rw-r--r--   0 haruka     (501) staff       (20)      548 2023-06-16 01:19:45.000000 scope-rl-0.1.2/recgym/__init__.py
+drwxr-xr-x   0 haruka     (501) staff       (20)        0 2023-07-22 01:34:31.827596 scope-rl-0.1.2/recgym/envs/
+-rw-r--r--   0 haruka     (501) staff       (20)      237 2023-06-16 01:19:45.000000 scope-rl-0.1.2/recgym/envs/__init__.py
+-rw-r--r--   0 haruka     (501) staff       (20)    12828 2023-06-16 01:19:45.000000 scope-rl-0.1.2/recgym/envs/rec.py
+drwxr-xr-x   0 haruka     (501) staff       (20)        0 2023-07-22 01:34:31.828164 scope-rl-0.1.2/recgym/envs/simulator/
+-rw-r--r--   0 haruka     (501) staff       (20)      257 2023-06-16 01:19:45.000000 scope-rl-0.1.2/recgym/envs/simulator/__init__.py
+-rw-r--r--   0 haruka     (501) staff       (20)     2757 2023-06-16 01:19:45.000000 scope-rl-0.1.2/recgym/envs/simulator/base.py
+-rw-r--r--   0 haruka     (501) staff       (20)     5363 2023-06-16 01:19:45.000000 scope-rl-0.1.2/recgym/envs/simulator/function.py
+-rw-r--r--   0 haruka     (501) staff       (20)      333 2023-06-16 01:19:45.000000 scope-rl-0.1.2/recgym/types.py
+-rw-r--r--   0 haruka     (501) staff       (20)     2052 2023-06-16 01:19:45.000000 scope-rl-0.1.2/recgym/utils.py
+-rw-r--r--   0 haruka     (501) staff       (20)      194 2023-06-16 01:19:45.000000 scope-rl-0.1.2/recgym/version.py
+-rw-r--r--   0 haruka     (501) staff       (20)      193 2023-07-21 11:27:56.000000 scope-rl-0.1.2/requirements.txt
+drwxr-xr-x   0 haruka     (501) staff       (20)        0 2023-07-22 01:34:31.828795 scope-rl-0.1.2/rtbgym/
+-rw-r--r--   0 haruka     (501) staff       (20)     1264 2023-06-16 01:19:45.000000 scope-rl-0.1.2/rtbgym/__init__.py
+drwxr-xr-x   0 haruka     (501) staff       (20)        0 2023-07-22 01:34:31.829573 scope-rl-0.1.2/rtbgym/envs/
+-rw-r--r--   0 haruka     (501) staff       (20)      314 2023-06-16 01:19:45.000000 scope-rl-0.1.2/rtbgym/envs/__init__.py
+-rw-r--r--   0 haruka     (501) staff       (20)    18863 2023-07-21 11:27:56.000000 scope-rl-0.1.2/rtbgym/envs/rtb.py
+drwxr-xr-x   0 haruka     (501) staff       (20)        0 2023-07-22 01:34:31.830322 scope-rl-0.1.2/rtbgym/envs/simulator/
+-rw-r--r--   0 haruka     (501) staff       (20)      621 2023-06-16 01:19:45.000000 scope-rl-0.1.2/rtbgym/envs/simulator/__init__.py
+-rw-r--r--   0 haruka     (501) staff       (20)     7529 2023-06-16 01:19:45.000000 scope-rl-0.1.2/rtbgym/envs/simulator/base.py
+-rw-r--r--   0 haruka     (501) staff       (20)    16332 2023-06-16 01:19:45.000000 scope-rl-0.1.2/rtbgym/envs/simulator/bidder.py
+-rw-r--r--   0 haruka     (501) staff       (20)    20994 2023-07-21 11:27:56.000000 scope-rl-0.1.2/rtbgym/envs/simulator/function.py
+-rw-r--r--   0 haruka     (501) staff       (20)    21598 2023-07-21 11:27:56.000000 scope-rl-0.1.2/rtbgym/envs/simulator/rtb_synthetic.py
+-rw-r--r--   0 haruka     (501) staff       (20)    13398 2023-06-16 01:19:45.000000 scope-rl-0.1.2/rtbgym/envs/wrapper_rtb.py
+-rw-r--r--   0 haruka     (501) staff       (20)      411 2023-06-16 01:19:45.000000 scope-rl-0.1.2/rtbgym/types.py
+-rw-r--r--   0 haruka     (501) staff       (20)     4788 2023-06-16 01:19:45.000000 scope-rl-0.1.2/rtbgym/utils.py
+-rw-r--r--   0 haruka     (501) staff       (20)      194 2023-06-16 01:19:45.000000 scope-rl-0.1.2/rtbgym/version.py
+drwxr-xr-x   0 haruka     (501) staff       (20)        0 2023-07-22 01:34:31.831298 scope-rl-0.1.2/scope_rl/
+-rw-r--r--   0 haruka     (501) staff       (20)      213 2023-06-16 01:19:45.000000 scope-rl-0.1.2/scope_rl/__init__.py
+drwxr-xr-x   0 haruka     (501) staff       (20)        0 2023-07-22 01:34:31.832373 scope-rl-0.1.2/scope_rl/dataset/
+-rw-r--r--   0 haruka     (501) staff       (20)      332 2023-06-16 01:19:45.000000 scope-rl-0.1.2/scope_rl/dataset/__init__.py
+-rw-r--r--   0 haruka     (501) staff       (20)     7018 2023-06-16 01:19:45.000000 scope-rl-0.1.2/scope_rl/dataset/base.py
+-rw-r--r--   0 haruka     (501) staff       (20)    49548 2023-07-21 11:27:56.000000 scope-rl-0.1.2/scope_rl/dataset/synthetic.py
+drwxr-xr-x   0 haruka     (501) staff       (20)        0 2023-07-22 01:34:31.834889 scope-rl-0.1.2/scope_rl/ope/
+-rw-r--r--   0 haruka     (501) staff       (20)     1046 2023-06-16 01:19:45.000000 scope-rl-0.1.2/scope_rl/ope/__init__.py
+drwxr-xr-x   0 haruka     (501) staff       (20)        0 2023-07-22 01:34:31.836983 scope-rl-0.1.2/scope_rl/ope/continuous/
+-rw-r--r--   0 haruka     (501) staff       (20)     2233 2023-06-16 01:19:45.000000 scope-rl-0.1.2/scope_rl/ope/continuous/__init__.py
+-rw-r--r--   0 haruka     (501) staff       (20)    69911 2023-07-21 11:27:56.000000 scope-rl-0.1.2/scope_rl/ope/continuous/basic_estimators.py
+-rw-r--r--   0 haruka     (501) staff       (20)    73299 2023-06-16 01:19:45.000000 scope-rl-0.1.2/scope_rl/ope/continuous/cumulative_distribution_estimators.py
+-rw-r--r--   0 haruka     (501) staff       (20)   130872 2023-07-21 11:27:56.000000 scope-rl-0.1.2/scope_rl/ope/continuous/marginal_estimators.py
+drwxr-xr-x   0 haruka     (501) staff       (20)        0 2023-07-22 01:34:31.837949 scope-rl-0.1.2/scope_rl/ope/discrete/
+-rw-r--r--   0 haruka     (501) staff       (20)     2227 2023-06-16 01:19:45.000000 scope-rl-0.1.2/scope_rl/ope/discrete/__init__.py
+-rw-r--r--   0 haruka     (501) staff       (20)    62875 2023-07-21 11:27:56.000000 scope-rl-0.1.2/scope_rl/ope/discrete/basic_estimators.py
+-rw-r--r--   0 haruka     (501) staff       (20)    68685 2023-06-16 01:19:45.000000 scope-rl-0.1.2/scope_rl/ope/discrete/cumulative_distribution_estimators.py
+-rw-r--r--   0 haruka     (501) staff       (20)   124829 2023-07-21 11:27:56.000000 scope-rl-0.1.2/scope_rl/ope/discrete/marginal_estimators.py
+-rw-r--r--   0 haruka     (501) staff       (20)    37164 2023-06-16 01:19:45.000000 scope-rl-0.1.2/scope_rl/ope/estimators_base.py
+-rw-r--r--   0 haruka     (501) staff       (20)   129251 2023-07-21 11:27:56.000000 scope-rl-0.1.2/scope_rl/ope/input.py
+-rw-r--r--   0 haruka     (501) staff       (20)    54713 2023-06-16 01:19:45.000000 scope-rl-0.1.2/scope_rl/ope/online.py
+-rw-r--r--   0 haruka     (501) staff       (20)   292304 2023-07-21 11:27:56.000000 scope-rl-0.1.2/scope_rl/ope/ope.py
+-rw-r--r--   0 haruka     (501) staff       (20)   523702 2023-07-21 11:27:56.000000 scope-rl-0.1.2/scope_rl/ope/ops.py
+drwxr-xr-x   0 haruka     (501) staff       (20)        0 2023-07-22 01:34:31.840714 scope-rl-0.1.2/scope_rl/ope/weight_value_learning/
+-rw-r--r--   0 haruka     (501) staff       (20)     2492 2023-06-16 01:19:45.000000 scope-rl-0.1.2/scope_rl/ope/weight_value_learning/__init__.py
+-rw-r--r--   0 haruka     (501) staff       (20)    49122 2023-06-16 01:19:45.000000 scope-rl-0.1.2/scope_rl/ope/weight_value_learning/augmented_lagrangian_learning_continuous.py
+-rw-r--r--   0 haruka     (501) staff       (20)    50800 2023-06-16 01:19:45.000000 scope-rl-0.1.2/scope_rl/ope/weight_value_learning/augmented_lagrangian_learning_discrete.py
+-rw-r--r--   0 haruka     (501) staff       (20)      985 2023-06-16 01:19:45.000000 scope-rl-0.1.2/scope_rl/ope/weight_value_learning/base.py
+-rw-r--r--   0 haruka     (501) staff       (20)     7892 2023-06-16 01:19:45.000000 scope-rl-0.1.2/scope_rl/ope/weight_value_learning/function.py
+-rw-r--r--   0 haruka     (501) staff       (20)    34834 2023-06-16 01:19:45.000000 scope-rl-0.1.2/scope_rl/ope/weight_value_learning/minimax_value_learning_continuous.py
+-rw-r--r--   0 haruka     (501) staff       (20)    36314 2023-06-16 01:19:45.000000 scope-rl-0.1.2/scope_rl/ope/weight_value_learning/minimax_value_learning_discrete.py
+-rw-r--r--   0 haruka     (501) staff       (20)    41939 2023-06-16 01:19:45.000000 scope-rl-0.1.2/scope_rl/ope/weight_value_learning/minimax_weight_learning_continuous.py
+-rw-r--r--   0 haruka     (501) staff       (20)    42102 2023-06-16 01:19:45.000000 scope-rl-0.1.2/scope_rl/ope/weight_value_learning/minimax_weight_learning_discrete.py
+drwxr-xr-x   0 haruka     (501) staff       (20)        0 2023-07-22 01:34:31.841454 scope-rl-0.1.2/scope_rl/policy/
+-rw-r--r--   0 haruka     (501) staff       (20)      981 2023-06-16 01:19:45.000000 scope-rl-0.1.2/scope_rl/policy/__init__.py
+-rw-r--r--   0 haruka     (501) staff       (20)     9256 2023-06-16 01:19:45.000000 scope-rl-0.1.2/scope_rl/policy/encoder.py
+-rw-r--r--   0 haruka     (501) staff       (20)    32731 2023-06-16 01:19:45.000000 scope-rl-0.1.2/scope_rl/policy/head.py
+-rw-r--r--   0 haruka     (501) staff       (20)    25869 2023-06-16 01:19:45.000000 scope-rl-0.1.2/scope_rl/policy/orl.py
+-rw-r--r--   0 haruka     (501) staff       (20)      334 2023-06-16 01:19:45.000000 scope-rl-0.1.2/scope_rl/types.py
+-rw-r--r--   0 haruka     (501) staff       (20)    30944 2023-07-09 08:34:30.000000 scope-rl-0.1.2/scope_rl/utils.py
+-rw-r--r--   0 haruka     (501) staff       (20)      194 2023-07-21 11:29:43.000000 scope-rl-0.1.2/scope_rl/version.py
+drwxr-xr-x   0 haruka     (501) staff       (20)        0 2023-07-22 01:34:31.831982 scope-rl-0.1.2/scope_rl.egg-info/
+-rw-r--r--   0 haruka     (501) staff       (20)    30919 2023-07-22 01:34:31.000000 scope-rl-0.1.2/scope_rl.egg-info/PKG-INFO
+-rw-r--r--   0 haruka     (501) staff       (20)     2374 2023-07-22 01:34:31.000000 scope-rl-0.1.2/scope_rl.egg-info/SOURCES.txt
+-rw-r--r--   0 haruka     (501) staff       (20)        1 2023-07-22 01:34:31.000000 scope-rl-0.1.2/scope_rl.egg-info/dependency_links.txt
+-rw-r--r--   0 haruka     (501) staff       (20)      194 2023-07-22 01:34:31.000000 scope-rl-0.1.2/scope_rl.egg-info/requires.txt
+-rw-r--r--   0 haruka     (501) staff       (20)       32 2023-07-22 01:34:31.000000 scope-rl-0.1.2/scope_rl.egg-info/top_level.txt
+-rw-r--r--   0 haruka     (501) staff       (20)       74 2023-07-22 01:34:31.842031 scope-rl-0.1.2/setup.cfg
+-rw-r--r--   0 haruka     (501) staff       (20)     1729 2023-07-21 12:05:09.000000 scope-rl-0.1.2/setup.py
```

### Comparing `scope-rl-0.1.1/CONTRIBUTING.md` & `scope-rl-0.1.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `scope-rl-0.1.1/FrequentlyAskedQuestions.md` & `scope-rl-0.1.2/FrequentlyAskedQuestions.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Frequently Asked Questions
 
-Q. xxx environment does not work on OFRL. How should we fix it?
+Q. xxx environment does not work on SCOPE-RL. How should we fix it?
 
-A. OFRL is compatible to Open AI Gym API, specifically for `gym>=0.26.0`, which works as follows.
+A. SCOPE-RL is compatible with OpenAI Gym API, specifically for `gym>=0.26.0`, which works as follows.
 ```Python
 obs, info = env.reset(), False
 while not done:
     action = agent.act(obs)
     obs, reward, done, truncated, info = env.step(action)
 ```
 
@@ -20,15 +20,15 @@
 
 To solve this incompatibility, please use `NewGymAPIWrapper` provided in `scope_rl/utils.py`. It should be used as follows.
 ```Python
 from scope_rl.utils import NewGymAPIWrapper
 env = NewGymAPIWrapper(env)
 ```
 
-Q. xxx environment does not work on d3rlpy, which is used for model training. How should we fix it? (d3rlpy and OFRL is compatible to different version of Open AI Gym.)
+Q. xxx environment does not work on d3rlpy, which is used for model training. How should we fix it? (d3rlpy and SCOPE-RL are compatible with different version of OpenAI Gym.)
 
-A. While OFRL is compatible to the latest API of Open AI Gym, d3rlpy is not. Therefore, please use `OldGymAPIWrapper` provided in `scope_rl/utils.py` to enable the use of d3rlpy.
+A. While SCOPE-RL is compatible with the latest API of OpenAI Gym, d3rlpy is not. Therefore, please use `OldGymAPIWrapper` provided in `scope_rl/utils.py` to enable the use of d3rlpy.
 ```Python
 from scope_rl.utils import OldGymAPIWrapper
-env = gym.make("xxx_v0")  # compatible to gym>=0.26.2 and OFRL
-env_ = OldGymAPIWrapper(env)  # compatible to gym<0.26.2 and d3rlpy
+env = gym.make("xxx_v0")  # compatible with gym>=0.26.2 and SCOPE-RL
+env_ = OldGymAPIWrapper(env)  # compatible with gym<0.26.2 and d3rlpy
 ```
```

### Comparing `scope-rl-0.1.1/LICENSE` & `scope-rl-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `scope-rl-0.1.1/PKG-INFO` & `scope-rl-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scope-rl
-Version: 0.1.1
+Version: 0.1.2
 Summary: SCOPE-RL: A pipeline for offline reinforcement learning research and applications
 Home-page: https://github.com/hakuhodo-technologies/scope-rl
 Author: Haruka Kiyohara
 Author-email: hk844@cornell.edu
 License: Apache License 2.0
 Keywords: off-policy evaluation,offline reinforcement learning,risk assessment
 Platform: UNKNOWN
@@ -45,35 +45,37 @@
 - [Contact](#contact)
 - [Reference](#reference)
 
 </details>
 
 **Documentation is available [here](https://scope-rl.readthedocs.io/en/latest/)**
 
+**Stable versions are available at [PyPI](https://pypi.org/project/scope-rl/)**
+
 ## Overview
 
 *SCOPE-RL* is an open-source Python Software for implementing the end-to-end procedure regarding **offline Reinforcement Learning (offline RL)**, from data collection to offline policy learning, off-policy performance evaluation, and policy selection. Our software includes a series of modules to implement synthetic dataset generation, dataset preprocessing, estimators for Off-Policy Evaluation (OPE), and Off-Policy Selection (OPS) methods.
 
-This software is also compatible with [d3rlpy](https://github.com/takuseno/d3rlpy), which implements a range of online and offline RL methods. SCOPE-RL enables an easy, transparent, and reliable experiment in offline RL research on any environment with [OpenAI Gym](https://gym.openai.com) and [Gymnasium](https://gymnasium.farama.org/)-like interface. It also facilitates implementation of offline RL in practice on a variety of customized datasets and on real-world datasets.
+This software is also compatible with [d3rlpy](https://github.com/takuseno/d3rlpy), which implements a range of online and offline RL methods. SCOPE-RL enables an easy, transparent, and reliable experiment in offline RL research on any environment with [OpenAI Gym](https://gym.openai.com) and [Gymnasium](https://gymnasium.farama.org/)-like interface. It also facilitates the implementation of offline RL in practice on a variety of customized datasets and real-world datasets.
 
 In particular, SCOPE-RL enables and facilitates evaluation and algorithm comparison related to the following research topics:
 
-- **Offline Reinforcement Learning**: Offline RL aims at learning a new policy from only offline logged data collected by a behavior policy. SCOPE-RL enables flexible experiment using customized dataset collected by various behavior policies and on a variety of environment.
+- **Offline Reinforcement Learning**: Offline RL aims at learning a new policy from only offline logged data collected by a behavior policy. SCOPE-RL enables flexible experiments using customized datasets collected by various behavior policies and environments.
 
 - **Off-Policy Evaluation**: OPE aims at evaluating the performance of a counterfactual policy using only offline logged data. SCOPE-RL supports many OPE estimators and streamlines the experimental procedure to evaluate and compare OPE estimators. Moreover, we also implement advanced OPE methods, such as estimators based on state-action density estimation and cumulative distribution estimation.
 
 - **Off-Policy Selection**: OPS aims at identifying the best-performing policy from a pool of several candidate policies using offline logged data. SCOPE-RL supports some basic OPS methods and provides several metrics to evaluate the OPS accuracy.
 
 This software is inspired by [Open Bandit Pipeline](https://github.com/st-tech/zr-obp), which is a library for OPE in contextual bandits. However, SCOPE-RL also implements a set of OPE estimators and tools to facilitate experiments about OPE for the contextual bandit setup by itself as well as those for RL.
 
 ### Implementations
 
 *SCOPE-RL* mainly consists of the following three modules.
 - [**dataset module**](./_gym/dataset): This module provides tools to generate synthetic data from any environment on top of [OpenAI Gym](http://gym.openai.com/) and [Gymnasium](https://gymnasium.farama.org/)-like interface. It also provides tools to pre-process the logged data.
-- [**policy module**](./_gym/policy): This module provides a wrapper class for [d3rlpy](https://github.com/takuseno/d3rlpy) to enable a flexible data collection.
+- [**policy module**](./_gym/policy): This module provides a wrapper class for [d3rlpy](https://github.com/takuseno/d3rlpy) to enable flexible data collection.
 - [**ope module**](./_gym/ope): This module provides a generic abstract class to implement OPE estimators. It also provides some tools useful for performing OPS.
 
 <details>
 <summary><strong>Behavior Policy </strong>(click to expand)</summary>
 
 - Discrete
   - Epsilon Greedy
@@ -129,38 +131,39 @@
 <details>
 <summary><strong>Evaluation Metrics of OPS </strong>(click to expand)</summary>
 
 - Mean Squared Error
 - Spearman's Rank Correlation Coefficient
 - Regret
 - Type I and Type II Error Rates
-- {Best/Worst/Mean} performances of top-k policies
+- {Best/Worst/Mean/Std} performances of top-k policies
 - Safety violation rate of top-k policies
+- SharpeRatio@k
 
 </details>
 
-Note that in addition to the above OPE and OPS methods, researcher can easily implement and compare their own estimators through a generic abstract class implemented in SCOPE-RL. Moreover, practitioners can apply the above methods to their real-world data to evaluate and choose counterfactual policies for their own practical situations.
+Note that in addition to the above OPE and OPS methods, researchers can easily implement and compare their own estimators through a generic abstract class implemented in SCOPE-RL. Moreover, practitioners can apply the above methods to their real-world data to evaluate and choose counterfactual policies for their own practical situations.
 
 To provide an example of performing a customized experiment imitating a practical setup, we also provide [RTBGym](./rtbgym) and [RecGym](./recgym), RL environments for Real-Time Bidding (RTB) and Recommender Systems.
 
 ## Installation
 
 You can install SCOPE-RL using Python's package manager `pip`.
 ```
 pip install scope-rl
 ```
 
-You can also install SCOPE-RL from source.
+You can also install SCOPE-RL from the source.
 ```bash
 git clone https://github.com/hakuhodo-technologies/scope-rl
 cd scope-rl
 python setup.py install
 ```
 
-SCOPE-RL supports Python 3.9 or newer. See [requirements.txt](./requirements.txt) for other requirements.
+SCOPE-RL supports Python 3.9 or newer. See [requirements.txt](./requirements.txt) for other requirements. Please also refer to issue [#17](https://github.com/hakuhodo-technologies/scope-rl/issues/17) when you encounter some dependency conflicts.
 
 ## Usage
 
 Here, we provide an example workflow to perform offline RL, OPE, and OPS using SCOPE-RL on [RTBGym](./rtbgym).
 
 ### Synthetic Dataset Generation and Data Preprocessing
 
@@ -258,15 +261,15 @@
     n_steps=10000,
     scorers={},
 )
 ```
 
 ### Basic Off-Policy Evaluation
 
-Then, we evaluate the performance of several evaluation policy (ddqn, cql, and random) using offline logged data collected by the behavior policy. Specifically, we compare the estimation results of various OPE estimators, including Direct Method (DM), Trajectory-wise Importance Sampling (TIS), Per-Decision Importance Sampling (PDIS), and Doubly Robust (DR) below.
+Then, we evaluate the performance of several evaluation policies (ddqn, cql, and random) using offline logged data collected by the behavior policy. Specifically, we compare the estimation results of various OPE estimators, including Direct Method (DM), Trajectory-wise Importance Sampling (TIS), Per-Decision Importance Sampling (PDIS), and Doubly Robust (DR) below.
 
 ```Python
 # implement a basic OPE procedure using SCOPE-RL
 
 # import SCOPE-RL modules
 from scope_rl.ope import CreateOPEInput
 from scope_rl.ope import OffPolicyEvaluation as OPE
@@ -325,15 +328,15 @@
 <div align="center"><img src="https://raw.githubusercontent.com/hakuhodo-technologies/scope-rl/main/images/ope_policy_value_basic.png" width="100%"/></div>
 <figcaption>
 <p align="center">
   Policy Value Estimated by OPE Estimators
 </p>
 </figcaption>
 
-More formal example implementations with RTBGym is available at [./examples/quickstart/rtb/](./examples/quickstart/rtb). Those with RecGym are also available at [./examples/quickstart/rec/](./examples/quickstart/rec).
+More formal example implementations with RTBGym are available at [./examples/quickstart/rtb/](./examples/quickstart/rtb). Those with RecGym are also available at [./examples/quickstart/rec/](./examples/quickstart/rec).
 
 ### Advanced Off-Policy Evaluation
 
 We can also estimate various statics of the evaluation policy, beyond just its expected performance, including variance and conditional value at risk (CVaR) via estimating the cumulative distribution function (CDF) of the reward under the evaluation policy.
 
 ```Python
 # implement a cumulative distribution estimation procedure using SCOPE-RL
@@ -373,15 +376,15 @@
 </p>
 </figcaption>
 
 For more extensive examples, please refer to [quickstart/rtb/rtb_synthetic_discrete_advanced.ipynb](./examples/quickstart/rtb/rtb_synthetic_discrete_advanced.ipynb).
 
 ### Off-Policy Selection and Evaluation of OPE/OPS
 
-We can also select the best-performing policy among a set of candidate policies based on the OPE results using the OPS class. It is also possible to evaluate the reliability of OPE/OPS using various metrics such as mean-squared-error, rank correlation, regret, and type I and type II error rates.
+We can also select the best-performing policy among a set of candidate policies based on the OPE results using the OPS class. It is also possible to evaluate the reliability of OPE/OPS using various metrics such as mean squaredberror, rank correlation, regret, and type I and type II error rates.
 
 ```Python
 # perform off-policy selection based on the OPE results
 
 # import SCOPE-RL modules
 from scope_rl.ope import OffPolicySelection
 
@@ -436,31 +439,52 @@
 [quickstart/rtb/rtb_synthetic_continuous_advanced.ipynb](./examples/quickstart/rtb/rtb_synthetic_continuous_advanced.ipynb) for continuous actions.
 
 ## Citation
 
 If you use our software in your work, please cite our paper:
 
 Haruka Kiyohara, Ren Kishimoto, Kosuke Kawakami, Ken Kobayashi, Kazuhide Nakata, Yuta Saito.<br>
+**SCOPE-RL: A Python Library for Offline Reinforcement Learning, Off-Policy Evaluation, and Policy Selection**<br>
+[link]() (a preprint coming soon..)
+
+Bibtex:
+```
+@article{kiyohara2023towards,
+  author = {Kiyohara, Haruka and Kishimoto, Ren and Kawakami, Kosuke and Kobayashi, Ken and Nataka, Kazuhide and Saito, Yuta},
+  title = {SCOPE-RL: A Python Library for Offline Reinforcement Learning, Off-Policy Evaluation, and Policy Selection},
+  journal={arXiv preprint arXiv:23xx.xxxxx},
+  year={2023},
+}
+```
+
+If you use our proposed metric "SharpeRatio@k" in your work, please cite our paper:
+
+Haruka Kiyohara, Ren Kishimoto, Kosuke Kawakami, Ken Kobayashi, Kazuhide Nakata, Yuta Saito.<br>
 **Towards Assessing and Benchmarking Risk-Return Tradeoff of Off-Policy Evaluation in Reinforcement Learning**<br>
 [link]() (a preprint coming soon..)
 
 Bibtex:
 ```
 @article{kiyohara2023towards,
   author = {Kiyohara, Haruka and Kishimoto, Ren and Kawakami, Kosuke and Kobayashi, Ken and Nataka, Kazuhide and Saito, Yuta},
   title = {Towards Assessing and Benchmarking Risk-Return Tradeoff of Off-Policy Evaluation in Reinforcement Learning},
-  journal = {A github repository},
-  pages = {xxx--xxx},
-  year = {2023},
+  journal={arXiv preprint arXiv:23xx.xxxxx},
+  year={2023},
 }
 ```
 
+## Google Group
+
+If you are interested in SCOPE-RL, please follow its updates via the google group:
+https://groups.google.com/g/scope-rl
+
+
 ## Contribution
 Any contributions to SCOPE-RL are more than welcome!
-Please refer to [CONTRIBUTING.md](./CONTRIBUTING.md) for general guidelines how to contribute the project.
+Please refer to [CONTRIBUTING.md](./CONTRIBUTING.md) for general guidelines on how to contribute to the project.
 
 ## License
 
 This project is licensed under Apache 2.0 license - see [LICENSE](LICENSE) file for details.
 
 ## Project Team
 
@@ -469,15 +493,15 @@
 - Kosuke Kawakami (HAKUHODO Technologies Inc.)
 - Ken Kobayashi (Tokyo Institute of Technology)
 - Kazuhide Nakata (Tokyo Institute of Technology)
 - [Yuta Saito](https://usait0.com/en/) (Cornell University)
 
 ## Contact
 
-For any question about the paper and software, feel free to contact: hk844@cornell.edu
+For any questions about the paper and software, feel free to contact: hk844@cornell.edu
 
 ## References
 
 <details>
 <summary><strong>Papers </strong>(click to expand)</summary>
 
 1. Alina Beygelzimer and John Langford. [The Offset Tree for Learning with Partial Labels](https://arxiv.org/abs/0812.4044). In *Proceedings of the 15th ACM SIGKDD International Conference on Knowledge Discovery and Data Mining*, 129-138, 2009.
@@ -526,15 +550,15 @@
 
 24. Tom Le Paine, Cosmin Paduraru, Andrea Michi, Caglar Gulcehre, Konrad Zolna, Alexander Novikov, Ziyu Wang, and Nando de Freitas. [Hyperparameter Selection for Offline Reinforcement Learning](https://arxiv.org/abs/2007.090550). *arXiv preprint arXiv:2007.09055*, 2020.
 
 25. Doina Precup, Richard S. Sutton, and Satinder P. Singh. [Eligibility Traces for Off-Policy Policy Evaluation](https://scholarworks.umass.edu/cgi/viewcontent.cgi?article=1079&context=cs_faculty_pubs). In *Proceedings of the 17th International Conference on Machine Learning*, 759–766, 2000.
 
 26. Rafael Figueiredo Prudencio, Marcos R. O. A. Maximo, and Esther Luna Colombini. [A Survey on Offline Reinforcement Learning: Taxonomy, Review, and Open Problems](https://arxiv.org/abs/2203.01387). *arXiv preprint arXiv:2203.01387*, 2022.
 
-27. Yuta Saito, Shunsuke Aihara, Megumi Matsutani, and Yusuke Narita. [Open Bandit Dataset and Pipeline: Towards Realistic and Reproducible Off-Policy Evaluation](https://arxiv.org/abs/2008.07146). In *Advances in Neural Information Processing Systems*, , 2021.
+27. Yuta Saito, Shunsuke Aihara, Megumi Matsutani, and Yusuke Narita. [Open Bandit Dataset and Pipeline: Towards Realistic and Reproducible Off-Policy Evaluation](https://arxiv.org/abs/2008.07146). In *Advances in Neural Information Processing Systems*, 2021.
 
 28. Takuma Seno and Michita Imai. [d3rlpy: An Offline Deep Reinforcement Library](https://arxiv.org/abs/2111.03788), *arXiv preprint arXiv:2111.03788*, 2021.
 
 29. Alex Strehl, John Langford, Sham Kakade, and Lihong Li. [Learning from Logged Implicit Exploration Data](https://arxiv.org/abs/1003.0120). In *Advances in Neural Information Processing Systems*, 2217-2225, 2010.
 
 30. Adith Swaminathan and Thorsten Joachims. [The Self-Normalized Estimator for Counterfactual Learning](https://papers.nips.cc/paper/2015/hash/39027dfad5138c9ca0c474d71db915c3-Abstract.html). In *Advances in Neural Information Processing Systems*, 3231-3239, 2015.
 
@@ -562,12 +586,12 @@
 
 <details>
 <summary><strong>Projects </strong>(click to expand)</summary>
 
 This project is strongly inspired by the following three packages.
 - **Open Bandit Pipeline**  -- a pipeline implementation of OPE in contextual bandits: [[github](https://github.com/st-tech/zr-obp)] [[documentation](https://zr-obp.readthedocs.io/en/latest/)] [[paper](https://arxiv.org/abs/2008.07146)]
 - **d3rlpy** -- a set of implementations of offline RL algorithms: [[github](https://github.com/takuseno/d3rlpy)] [[documentation](https://d3rlpy.readthedocs.io/en/v0.91/)] [[paper](https://arxiv.org/abs/2111.03788)]
-- **Spinning Up** -- an educational resource for learning deepl RL: [[github](https://github.com/openai/spinningup)] [[documentation](https://spinningup.openai.com/en/latest/)]
+- **Spinning Up** -- an educational resource for learning deep RL: [[github](https://github.com/openai/spinningup)] [[documentation](https://spinningup.openai.com/en/latest/)]
 
 </details>
```

### Comparing `scope-rl-0.1.1/README.md` & `scope-rl-0.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -21,35 +21,37 @@
 - [Contact](#contact)
 - [Reference](#reference)
 
 </details>
 
 **Documentation is available [here](https://scope-rl.readthedocs.io/en/latest/)**
 
+**Stable versions are available at [PyPI](https://pypi.org/project/scope-rl/)**
+
 ## Overview
 
 *SCOPE-RL* is an open-source Python Software for implementing the end-to-end procedure regarding **offline Reinforcement Learning (offline RL)**, from data collection to offline policy learning, off-policy performance evaluation, and policy selection. Our software includes a series of modules to implement synthetic dataset generation, dataset preprocessing, estimators for Off-Policy Evaluation (OPE), and Off-Policy Selection (OPS) methods.
 
-This software is also compatible with [d3rlpy](https://github.com/takuseno/d3rlpy), which implements a range of online and offline RL methods. SCOPE-RL enables an easy, transparent, and reliable experiment in offline RL research on any environment with [OpenAI Gym](https://gym.openai.com) and [Gymnasium](https://gymnasium.farama.org/)-like interface. It also facilitates implementation of offline RL in practice on a variety of customized datasets and on real-world datasets.
+This software is also compatible with [d3rlpy](https://github.com/takuseno/d3rlpy), which implements a range of online and offline RL methods. SCOPE-RL enables an easy, transparent, and reliable experiment in offline RL research on any environment with [OpenAI Gym](https://gym.openai.com) and [Gymnasium](https://gymnasium.farama.org/)-like interface. It also facilitates the implementation of offline RL in practice on a variety of customized datasets and real-world datasets.
 
 In particular, SCOPE-RL enables and facilitates evaluation and algorithm comparison related to the following research topics:
 
-- **Offline Reinforcement Learning**: Offline RL aims at learning a new policy from only offline logged data collected by a behavior policy. SCOPE-RL enables flexible experiment using customized dataset collected by various behavior policies and on a variety of environment.
+- **Offline Reinforcement Learning**: Offline RL aims at learning a new policy from only offline logged data collected by a behavior policy. SCOPE-RL enables flexible experiments using customized datasets collected by various behavior policies and environments.
 
 - **Off-Policy Evaluation**: OPE aims at evaluating the performance of a counterfactual policy using only offline logged data. SCOPE-RL supports many OPE estimators and streamlines the experimental procedure to evaluate and compare OPE estimators. Moreover, we also implement advanced OPE methods, such as estimators based on state-action density estimation and cumulative distribution estimation.
 
 - **Off-Policy Selection**: OPS aims at identifying the best-performing policy from a pool of several candidate policies using offline logged data. SCOPE-RL supports some basic OPS methods and provides several metrics to evaluate the OPS accuracy.
 
 This software is inspired by [Open Bandit Pipeline](https://github.com/st-tech/zr-obp), which is a library for OPE in contextual bandits. However, SCOPE-RL also implements a set of OPE estimators and tools to facilitate experiments about OPE for the contextual bandit setup by itself as well as those for RL.
 
 ### Implementations
 
 *SCOPE-RL* mainly consists of the following three modules.
 - [**dataset module**](./_gym/dataset): This module provides tools to generate synthetic data from any environment on top of [OpenAI Gym](http://gym.openai.com/) and [Gymnasium](https://gymnasium.farama.org/)-like interface. It also provides tools to pre-process the logged data.
-- [**policy module**](./_gym/policy): This module provides a wrapper class for [d3rlpy](https://github.com/takuseno/d3rlpy) to enable a flexible data collection.
+- [**policy module**](./_gym/policy): This module provides a wrapper class for [d3rlpy](https://github.com/takuseno/d3rlpy) to enable flexible data collection.
 - [**ope module**](./_gym/ope): This module provides a generic abstract class to implement OPE estimators. It also provides some tools useful for performing OPS.
 
 <details>
 <summary><strong>Behavior Policy </strong>(click to expand)</summary>
 
 - Discrete
   - Epsilon Greedy
@@ -105,38 +107,39 @@
 <details>
 <summary><strong>Evaluation Metrics of OPS </strong>(click to expand)</summary>
 
 - Mean Squared Error
 - Spearman's Rank Correlation Coefficient
 - Regret
 - Type I and Type II Error Rates
-- {Best/Worst/Mean} performances of top-k policies
+- {Best/Worst/Mean/Std} performances of top-k policies
 - Safety violation rate of top-k policies
+- SharpeRatio@k
 
 </details>
 
-Note that in addition to the above OPE and OPS methods, researcher can easily implement and compare their own estimators through a generic abstract class implemented in SCOPE-RL. Moreover, practitioners can apply the above methods to their real-world data to evaluate and choose counterfactual policies for their own practical situations.
+Note that in addition to the above OPE and OPS methods, researchers can easily implement and compare their own estimators through a generic abstract class implemented in SCOPE-RL. Moreover, practitioners can apply the above methods to their real-world data to evaluate and choose counterfactual policies for their own practical situations.
 
 To provide an example of performing a customized experiment imitating a practical setup, we also provide [RTBGym](./rtbgym) and [RecGym](./recgym), RL environments for Real-Time Bidding (RTB) and Recommender Systems.
 
 ## Installation
 
 You can install SCOPE-RL using Python's package manager `pip`.
 ```
 pip install scope-rl
 ```
 
-You can also install SCOPE-RL from source.
+You can also install SCOPE-RL from the source.
 ```bash
 git clone https://github.com/hakuhodo-technologies/scope-rl
 cd scope-rl
 python setup.py install
 ```
 
-SCOPE-RL supports Python 3.9 or newer. See [requirements.txt](./requirements.txt) for other requirements.
+SCOPE-RL supports Python 3.9 or newer. See [requirements.txt](./requirements.txt) for other requirements. Please also refer to issue [#17](https://github.com/hakuhodo-technologies/scope-rl/issues/17) when you encounter some dependency conflicts.
 
 ## Usage
 
 Here, we provide an example workflow to perform offline RL, OPE, and OPS using SCOPE-RL on [RTBGym](./rtbgym).
 
 ### Synthetic Dataset Generation and Data Preprocessing
 
@@ -234,15 +237,15 @@
     n_steps=10000,
     scorers={},
 )
 ```
 
 ### Basic Off-Policy Evaluation
 
-Then, we evaluate the performance of several evaluation policy (ddqn, cql, and random) using offline logged data collected by the behavior policy. Specifically, we compare the estimation results of various OPE estimators, including Direct Method (DM), Trajectory-wise Importance Sampling (TIS), Per-Decision Importance Sampling (PDIS), and Doubly Robust (DR) below.
+Then, we evaluate the performance of several evaluation policies (ddqn, cql, and random) using offline logged data collected by the behavior policy. Specifically, we compare the estimation results of various OPE estimators, including Direct Method (DM), Trajectory-wise Importance Sampling (TIS), Per-Decision Importance Sampling (PDIS), and Doubly Robust (DR) below.
 
 ```Python
 # implement a basic OPE procedure using SCOPE-RL
 
 # import SCOPE-RL modules
 from scope_rl.ope import CreateOPEInput
 from scope_rl.ope import OffPolicyEvaluation as OPE
@@ -301,15 +304,15 @@
 <div align="center"><img src="https://raw.githubusercontent.com/hakuhodo-technologies/scope-rl/main/images/ope_policy_value_basic.png" width="100%"/></div>
 <figcaption>
 <p align="center">
   Policy Value Estimated by OPE Estimators
 </p>
 </figcaption>
 
-More formal example implementations with RTBGym is available at [./examples/quickstart/rtb/](./examples/quickstart/rtb). Those with RecGym are also available at [./examples/quickstart/rec/](./examples/quickstart/rec).
+More formal example implementations with RTBGym are available at [./examples/quickstart/rtb/](./examples/quickstart/rtb). Those with RecGym are also available at [./examples/quickstart/rec/](./examples/quickstart/rec).
 
 ### Advanced Off-Policy Evaluation
 
 We can also estimate various statics of the evaluation policy, beyond just its expected performance, including variance and conditional value at risk (CVaR) via estimating the cumulative distribution function (CDF) of the reward under the evaluation policy.
 
 ```Python
 # implement a cumulative distribution estimation procedure using SCOPE-RL
@@ -349,15 +352,15 @@
 </p>
 </figcaption>
 
 For more extensive examples, please refer to [quickstart/rtb/rtb_synthetic_discrete_advanced.ipynb](./examples/quickstart/rtb/rtb_synthetic_discrete_advanced.ipynb).
 
 ### Off-Policy Selection and Evaluation of OPE/OPS
 
-We can also select the best-performing policy among a set of candidate policies based on the OPE results using the OPS class. It is also possible to evaluate the reliability of OPE/OPS using various metrics such as mean-squared-error, rank correlation, regret, and type I and type II error rates.
+We can also select the best-performing policy among a set of candidate policies based on the OPE results using the OPS class. It is also possible to evaluate the reliability of OPE/OPS using various metrics such as mean squaredberror, rank correlation, regret, and type I and type II error rates.
 
 ```Python
 # perform off-policy selection based on the OPE results
 
 # import SCOPE-RL modules
 from scope_rl.ope import OffPolicySelection
 
@@ -412,31 +415,52 @@
 [quickstart/rtb/rtb_synthetic_continuous_advanced.ipynb](./examples/quickstart/rtb/rtb_synthetic_continuous_advanced.ipynb) for continuous actions.
 
 ## Citation
 
 If you use our software in your work, please cite our paper:
 
 Haruka Kiyohara, Ren Kishimoto, Kosuke Kawakami, Ken Kobayashi, Kazuhide Nakata, Yuta Saito.<br>
+**SCOPE-RL: A Python Library for Offline Reinforcement Learning, Off-Policy Evaluation, and Policy Selection**<br>
+[link]() (a preprint coming soon..)
+
+Bibtex:
+```
+@article{kiyohara2023towards,
+  author = {Kiyohara, Haruka and Kishimoto, Ren and Kawakami, Kosuke and Kobayashi, Ken and Nataka, Kazuhide and Saito, Yuta},
+  title = {SCOPE-RL: A Python Library for Offline Reinforcement Learning, Off-Policy Evaluation, and Policy Selection},
+  journal={arXiv preprint arXiv:23xx.xxxxx},
+  year={2023},
+}
+```
+
+If you use our proposed metric "SharpeRatio@k" in your work, please cite our paper:
+
+Haruka Kiyohara, Ren Kishimoto, Kosuke Kawakami, Ken Kobayashi, Kazuhide Nakata, Yuta Saito.<br>
 **Towards Assessing and Benchmarking Risk-Return Tradeoff of Off-Policy Evaluation in Reinforcement Learning**<br>
 [link]() (a preprint coming soon..)
 
 Bibtex:
 ```
 @article{kiyohara2023towards,
   author = {Kiyohara, Haruka and Kishimoto, Ren and Kawakami, Kosuke and Kobayashi, Ken and Nataka, Kazuhide and Saito, Yuta},
   title = {Towards Assessing and Benchmarking Risk-Return Tradeoff of Off-Policy Evaluation in Reinforcement Learning},
-  journal = {A github repository},
-  pages = {xxx--xxx},
-  year = {2023},
+  journal={arXiv preprint arXiv:23xx.xxxxx},
+  year={2023},
 }
 ```
 
+## Google Group
+
+If you are interested in SCOPE-RL, please follow its updates via the google group:
+https://groups.google.com/g/scope-rl
+
+
 ## Contribution
 Any contributions to SCOPE-RL are more than welcome!
-Please refer to [CONTRIBUTING.md](./CONTRIBUTING.md) for general guidelines how to contribute the project.
+Please refer to [CONTRIBUTING.md](./CONTRIBUTING.md) for general guidelines on how to contribute to the project.
 
 ## License
 
 This project is licensed under Apache 2.0 license - see [LICENSE](LICENSE) file for details.
 
 ## Project Team
 
@@ -445,15 +469,15 @@
 - Kosuke Kawakami (HAKUHODO Technologies Inc.)
 - Ken Kobayashi (Tokyo Institute of Technology)
 - Kazuhide Nakata (Tokyo Institute of Technology)
 - [Yuta Saito](https://usait0.com/en/) (Cornell University)
 
 ## Contact
 
-For any question about the paper and software, feel free to contact: hk844@cornell.edu
+For any questions about the paper and software, feel free to contact: hk844@cornell.edu
 
 ## References
 
 <details>
 <summary><strong>Papers </strong>(click to expand)</summary>
 
 1. Alina Beygelzimer and John Langford. [The Offset Tree for Learning with Partial Labels](https://arxiv.org/abs/0812.4044). In *Proceedings of the 15th ACM SIGKDD International Conference on Knowledge Discovery and Data Mining*, 129-138, 2009.
@@ -502,15 +526,15 @@
 
 24. Tom Le Paine, Cosmin Paduraru, Andrea Michi, Caglar Gulcehre, Konrad Zolna, Alexander Novikov, Ziyu Wang, and Nando de Freitas. [Hyperparameter Selection for Offline Reinforcement Learning](https://arxiv.org/abs/2007.090550). *arXiv preprint arXiv:2007.09055*, 2020.
 
 25. Doina Precup, Richard S. Sutton, and Satinder P. Singh. [Eligibility Traces for Off-Policy Policy Evaluation](https://scholarworks.umass.edu/cgi/viewcontent.cgi?article=1079&context=cs_faculty_pubs). In *Proceedings of the 17th International Conference on Machine Learning*, 759–766, 2000.
 
 26. Rafael Figueiredo Prudencio, Marcos R. O. A. Maximo, and Esther Luna Colombini. [A Survey on Offline Reinforcement Learning: Taxonomy, Review, and Open Problems](https://arxiv.org/abs/2203.01387). *arXiv preprint arXiv:2203.01387*, 2022.
 
-27. Yuta Saito, Shunsuke Aihara, Megumi Matsutani, and Yusuke Narita. [Open Bandit Dataset and Pipeline: Towards Realistic and Reproducible Off-Policy Evaluation](https://arxiv.org/abs/2008.07146). In *Advances in Neural Information Processing Systems*, , 2021.
+27. Yuta Saito, Shunsuke Aihara, Megumi Matsutani, and Yusuke Narita. [Open Bandit Dataset and Pipeline: Towards Realistic and Reproducible Off-Policy Evaluation](https://arxiv.org/abs/2008.07146). In *Advances in Neural Information Processing Systems*, 2021.
 
 28. Takuma Seno and Michita Imai. [d3rlpy: An Offline Deep Reinforcement Library](https://arxiv.org/abs/2111.03788), *arXiv preprint arXiv:2111.03788*, 2021.
 
 29. Alex Strehl, John Langford, Sham Kakade, and Lihong Li. [Learning from Logged Implicit Exploration Data](https://arxiv.org/abs/1003.0120). In *Advances in Neural Information Processing Systems*, 2217-2225, 2010.
 
 30. Adith Swaminathan and Thorsten Joachims. [The Self-Normalized Estimator for Counterfactual Learning](https://papers.nips.cc/paper/2015/hash/39027dfad5138c9ca0c474d71db915c3-Abstract.html). In *Advances in Neural Information Processing Systems*, 3231-3239, 2015.
 
@@ -538,10 +562,10 @@
 
 <details>
 <summary><strong>Projects </strong>(click to expand)</summary>
 
 This project is strongly inspired by the following three packages.
 - **Open Bandit Pipeline**  -- a pipeline implementation of OPE in contextual bandits: [[github](https://github.com/st-tech/zr-obp)] [[documentation](https://zr-obp.readthedocs.io/en/latest/)] [[paper](https://arxiv.org/abs/2008.07146)]
 - **d3rlpy** -- a set of implementations of offline RL algorithms: [[github](https://github.com/takuseno/d3rlpy)] [[documentation](https://d3rlpy.readthedocs.io/en/v0.91/)] [[paper](https://arxiv.org/abs/2111.03788)]
-- **Spinning Up** -- an educational resource for learning deepl RL: [[github](https://github.com/openai/spinningup)] [[documentation](https://spinningup.openai.com/en/latest/)]
+- **Spinning Up** -- an educational resource for learning deep RL: [[github](https://github.com/openai/spinningup)] [[documentation](https://spinningup.openai.com/en/latest/)]
 
 </details>
```

### Comparing `scope-rl-0.1.1/basicgym/__init__.py` & `scope-rl-0.1.2/basicgym/__init__.py`

 * *Files identical despite different names*

### Comparing `scope-rl-0.1.1/basicgym/envs/simulator/base.py` & `scope-rl-0.1.2/basicgym/envs/simulator/base.py`

 * *Files identical despite different names*

### Comparing `scope-rl-0.1.1/basicgym/envs/simulator/function.py` & `scope-rl-0.1.2/basicgym/envs/simulator/function.py`

 * *Files identical despite different names*

### Comparing `scope-rl-0.1.1/basicgym/envs/synthetic.py` & `scope-rl-0.1.2/basicgym/envs/synthetic.py`

 * *Files identical despite different names*

### Comparing `scope-rl-0.1.1/basicgym/utils.py` & `scope-rl-0.1.2/basicgym/utils.py`

 * *Files identical despite different names*

### Comparing `scope-rl-0.1.1/recgym/__init__.py` & `scope-rl-0.1.2/recgym/__init__.py`

 * *Files identical despite different names*

### Comparing `scope-rl-0.1.1/recgym/envs/rec.py` & `scope-rl-0.1.2/recgym/envs/rec.py`

 * *Files identical despite different names*

### Comparing `scope-rl-0.1.1/recgym/envs/simulator/base.py` & `scope-rl-0.1.2/recgym/envs/simulator/base.py`

 * *Files identical despite different names*

### Comparing `scope-rl-0.1.1/recgym/envs/simulator/function.py` & `scope-rl-0.1.2/recgym/envs/simulator/function.py`

 * *Files identical despite different names*

### Comparing `scope-rl-0.1.1/recgym/utils.py` & `scope-rl-0.1.2/recgym/utils.py`

 * *Files identical despite different names*

### Comparing `scope-rl-0.1.1/rtbgym/__init__.py` & `scope-rl-0.1.2/rtbgym/__init__.py`

 * *Files identical despite different names*

### Comparing `scope-rl-0.1.1/rtbgym/envs/rtb.py` & `scope-rl-0.1.2/rtbgym/envs/rtb.py`

 * *Files identical despite different names*

### Comparing `scope-rl-0.1.1/rtbgym/envs/simulator/__init__.py` & `scope-rl-0.1.2/rtbgym/envs/simulator/__init__.py`

 * *Files identical despite different names*

### Comparing `scope-rl-0.1.1/rtbgym/envs/simulator/base.py` & `scope-rl-0.1.2/rtbgym/envs/simulator/base.py`

 * *Files identical despite different names*

### Comparing `scope-rl-0.1.1/rtbgym/envs/simulator/bidder.py` & `scope-rl-0.1.2/rtbgym/envs/simulator/bidder.py`

 * *Files identical despite different names*

### Comparing `scope-rl-0.1.1/rtbgym/envs/simulator/function.py` & `scope-rl-0.1.2/rtbgym/envs/simulator/function.py`

 * *Files identical despite different names*

### Comparing `scope-rl-0.1.1/rtbgym/envs/simulator/rtb_synthetic.py` & `scope-rl-0.1.2/rtbgym/envs/simulator/rtb_synthetic.py`

 * *Files identical despite different names*

### Comparing `scope-rl-0.1.1/rtbgym/envs/wrapper_rtb.py` & `scope-rl-0.1.2/rtbgym/envs/wrapper_rtb.py`

 * *Files identical despite different names*

### Comparing `scope-rl-0.1.1/rtbgym/utils.py` & `scope-rl-0.1.2/rtbgym/utils.py`

 * *Files identical despite different names*

### Comparing `scope-rl-0.1.1/scope_rl/dataset/base.py` & `scope-rl-0.1.2/scope_rl/dataset/base.py`

 * *Files identical despite different names*

### Comparing `scope-rl-0.1.1/scope_rl/dataset/synthetic.py` & `scope-rl-0.1.2/scope_rl/dataset/synthetic.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     Bases: :class:`scope_rl.dataset.BaseDataset`
 
     Imported as: :class:`scope_rl.dataset.SyntheticDataset`
 
     Note
     -------
     Logged dataset is directly used for Off-Policy Evaluation (OPE).
-    Moreover, it is also compatible to `d3rlpy <https://github.com/takuseno/d3rlpy>`_ (offline RL library) with the following command.
+    Moreover, it is also compatible with `d3rlpy <https://github.com/takuseno/d3rlpy>`_ (offline RL library) with the following command.
 
     .. code-block:: python
 
         d3rlpy_dataset = MDPDataset(
             observations=logged_datasets["state"],
             actions=logged_datasets["action"],
             rewards=logged_datasets["reward"],
```

### Comparing `scope-rl-0.1.1/scope_rl/ope/__init__.py` & `scope-rl-0.1.2/scope_rl/ope/__init__.py`

 * *Files identical despite different names*

### Comparing `scope-rl-0.1.1/scope_rl/ope/continuous/__init__.py` & `scope-rl-0.1.2/scope_rl/ope/continuous/__init__.py`

 * *Files identical despite different names*

### Comparing `scope-rl-0.1.1/scope_rl/ope/continuous/basic_estimators.py` & `scope-rl-0.1.2/scope_rl/ope/continuous/basic_estimators.py`

 * *Files 0% similar despite different names*

```diff
@@ -109,15 +109,15 @@
 
         state_action_value_prediction: array-like of shape (n_trajectories * step_per_trajectory, 2)
             :math:`\\hat{Q}` for the observed action and that chosen by the evaluation policy,
             i.e., (row 0) :math:`\\hat{Q}(s_t, a_t)` and (row 2) :math:`\\hat{Q}(s_t, \\pi(a | s_t))`.
 
         Return
         -------
-        V_hat: ndarray of shape (n_trajectories, )
+        V_hat: float
             Estimated policy value.
 
         """
         check_scalar(
             step_per_trajectory,
             name="step_per_trajectory",
             target_type=int,
@@ -391,15 +391,15 @@
             Bandwidth hyperparameter of the kernel function.
 
         action_scaler: d3rlpy.preprocessing.ActionScaler, default=None
             Scaling factor of action.
 
         Return
         -------
-        V_hat: ndarray of shape (n_trajectories, )
+        V_hat: float
             Estimated policy value.
 
         """
         check_scalar(
             step_per_trajectory,
             name="step_per_trajectory",
             target_type=int,
@@ -785,15 +785,15 @@
             Bandwidth hyperparameter of the kernel function.
 
         action_scaler: d3rlpy.preprocessing.ActionScaler, default=None
             Scaling factor of action.
 
         Return
         -------
-        V_hat: ndarray of shape (n_trajectories, )
+        V_hat: float
             Estimated policy value.
 
         """
         check_scalar(
             step_per_trajectory,
             name="step_per_trajectory",
             target_type=int,
@@ -1203,15 +1203,15 @@
             Bandwidth hyperparameter of the kernel function.
 
         action_scaler: d3rlpy.preprocessing.ActionScaler, default=None
             Scaling factor of action.
 
         Return
         -------
-        V_hat: ndarray of shape (n_trajectories, )
+        V_hat: float
             Estimated policy value.
 
         """
         check_scalar(
             step_per_trajectory,
             name="step_per_trajectory",
             target_type=int,
```

### Comparing `scope-rl-0.1.1/scope_rl/ope/continuous/cumulative_distribution_estimators.py` & `scope-rl-0.1.2/scope_rl/ope/continuous/cumulative_distribution_estimators.py`

 * *Files identical despite different names*

### Comparing `scope-rl-0.1.1/scope_rl/ope/continuous/marginal_estimators.py` & `scope-rl-0.1.2/scope_rl/ope/continuous/marginal_estimators.py`

 * *Files 1% similar despite different names*

```diff
@@ -147,15 +147,15 @@
 
         state_action_value_prediction: array-like of shape (n_trajectories * step_per_trajectory, 2)
             :math:`\\hat{Q}` for the observed action and that chosen by the evaluation policy,
             i.e., (row 0) :math:`\\hat{Q}(s_t, a_t)` and (row 2) :math:`\\hat{Q}(s_t, \\pi(a | s_t))`.
 
         Return
         -------
-        V_hat: ndarray of shape (n_trajectories, )
+        V_hat: float
             Estimated policy value.
 
         """
         check_scalar(
             step_per_trajectory,
             name="step_per_trajectory",
             target_type=int,
@@ -390,15 +390,15 @@
         Parameters
         -------
         initial_state_value_prediction: array-like of shape (n_trajectories, )
             Estimated initial state value.
 
         Return
         -------
-        V_hat: ndarray of shape (n_trajectories, )
+        V_hat: float
             Estimated policy value.
 
         """
         check_array(
             initial_state_value_prediction,
             name="initial_state_value_prediction",
             expected_dim=1,
@@ -680,15 +680,15 @@
             Bandwidth hyperparameter of the kernel function.
 
         action_scaler: d3rlpy.preprocessing.ActionScaler, default=None
             Scaling factor of action.
 
         Return
         -------
-        V_hat: ndarray of shape (n_trajectories, )
+        V_hat: float
             Estimated policy value.
 
         """
         check_scalar(
             n_step_pdis,
             name="n_step_pdis",
             target_type=int,
@@ -1185,15 +1185,15 @@
             Bandwidth hyperparameter of the kernel function.
 
         action_scaler: d3rlpy.preprocessing.ActionScaler, default=None
             Scaling factor of action.
 
         Return
         -------
-        V_hat: ndarray of shape (n_trajectories, )
+        V_hat: float
             Estimated policy value.
 
         """
         check_scalar(
             n_step_pdis,
             name="n_step_pdis",
             target_type=int,
@@ -2040,15 +2040,15 @@
             Bandwidth hyperparameter of the kernel function.
 
         action_scaler: d3rlpy.preprocessing.ActionScaler, default=None
             Scaling factor of action.
 
         Return
         -------
-        V_hat: ndarray of shape (n_trajectories, )
+        V_hat: float
             Estimated policy value.
 
         """
         check_scalar(
             n_step_pdis,
             name="n_step_pdis",
             target_type=int,
@@ -2542,15 +2542,15 @@
             Bandwidth hyperparameter of the kernel function.
 
         action_scaler: d3rlpy.preprocessing.ActionScaler, default=None
             Scaling factor of action.
 
         Return
         -------
-        V_hat: ndarray of shape (n_trajectories, )
+        V_hat: float
             Estimated policy value.
 
         """
         check_scalar(
             n_step_pdis,
             name="n_step_pdis",
             target_type=int,
```

### Comparing `scope-rl-0.1.1/scope_rl/ope/discrete/__init__.py` & `scope-rl-0.1.2/scope_rl/ope/discrete/__init__.py`

 * *Files identical despite different names*

### Comparing `scope-rl-0.1.1/scope_rl/ope/discrete/basic_estimators.py` & `scope-rl-0.1.2/scope_rl/ope/discrete/basic_estimators.py`

 * *Files 0% similar despite different names*

```diff
@@ -117,15 +117,15 @@
             i.e., :math:`\\pi(a | s_t) \\forall a \\in \\mathcal{A}`
 
         state_action_value_prediction: array-like of shape (n_trajectories * step_per_trajectory, n_action)
             :math:`\\hat{Q}` for all actions, i.e., :math:`\\hat{Q}(s_t, a) \\forall a \\in \\mathcal{A}`.
 
         Return
         -------
-        V_hat: ndarray of shape (n_trajectories, )
+        V_hat: float
             Estimated policy value.
 
         """
         check_scalar(
             step_per_trajectory,
             name="step_per_trajectory",
             target_type=int,
@@ -425,15 +425,15 @@
             i.e., :math:`\\pi(a | s_t) \\forall a \\in \\mathcal{A}`
 
         gamma: float, default=1.0
             Discount factor. The value should be within (0, 1].
 
         Return
         -------
-        V_hat: ndarray of shape (n_trajectories, )
+        V_hat: float
             Estimated policy value.
 
         """
         check_scalar(
             step_per_trajectory,
             name="step_per_trajectory",
             target_type=int,
@@ -770,15 +770,15 @@
             i.e., :math:`\\pi(a | s_t) \\forall a \\in \\mathcal{A}`
 
         gamma: float, default=1.0
             Discount factor. The value should be within (0, 1].
 
         Return
         -------
-        V_hat: ndarray of shape (n_trajectories, )
+        V_hat: float
             Estimated policy value.
 
         """
         check_scalar(
             step_per_trajectory,
             name="step_per_trajectory",
             target_type=int,
@@ -1144,15 +1144,15 @@
             :math:`\\hat{Q}` for all actions, i.e., :math:`\\hat{Q}(s_t, a) \\forall a \\in \\mathcal{A}`.
 
         gamma: float, default=1.0
             Discount factor. The value should be within (0, 1].
 
         Return
         -------
-        V_hat: ndarray of shape (n_trajectories, )
+        V_hat: float
             Estimated policy value.
 
         """
         check_scalar(
             step_per_trajectory,
             name="step_per_trajectory",
             target_type=int,
```

### Comparing `scope-rl-0.1.1/scope_rl/ope/discrete/cumulative_distribution_estimators.py` & `scope-rl-0.1.2/scope_rl/ope/discrete/cumulative_distribution_estimators.py`

 * *Files identical despite different names*

### Comparing `scope-rl-0.1.1/scope_rl/ope/discrete/marginal_estimators.py` & `scope-rl-0.1.2/scope_rl/ope/discrete/marginal_estimators.py`

 * *Files 1% similar despite different names*

```diff
@@ -164,15 +164,15 @@
             i.e., :math:`\\pi(a | s) \\forall a \\in \\mathcal{A}`
 
         state_action_value_prediction: array-like of shape (n_trajectories * step_per_trajectory, n_action)
             :math:`\\hat{Q}` for all actions, i.e., :math:`\\hat{Q}(s_t, a) \\forall a \\in \\mathcal{A}`.
 
         Return
         -------
-        V_hat: ndarray of shape (n_trajectories, )
+        V_hat: float
             Estimated policy value.
 
         """
         check_scalar(
             step_per_trajectory,
             name="step_per_trajectory",
             target_type=int,
@@ -477,15 +477,15 @@
         Parameters
         -------
         initial_state_value_prediction: array-like of shape (n_trajectories, )
             Estimated initial state value.
 
         Return
         -------
-        V_hat: ndarray of shape (n_trajectories, )
+        V_hat: float
             Estimated policy value.
 
         """
         check_array(
             initial_state_value_prediction,
             name="initial_state_value_prediction",
             expected_dim=1,
@@ -738,15 +738,15 @@
             i.e., :math:`\\pi(a | s) \\forall a \\in \\mathcal{A}`
 
         gamma: float, default=1.0
             Discount factor. The value should be within (0, 1].
 
         Return
         -------
-        V_hat: ndarray of shape (n_trajectories, )
+        V_hat: float
             Estimated policy value.
 
         """
         check_scalar(
             n_step_pdis,
             name="n_step_pdis",
             target_type=int,
@@ -1208,15 +1208,15 @@
             Estimated initial state value.
 
         gamma: float, default=1.0
             Discount factor. The value should be within (0, 1].
 
         Return
         -------
-        V_hat: ndarray of shape (n_trajectories, )
+        V_hat: float
             Estimated policy value.
 
         """
         check_scalar(
             n_step_pdis,
             name="n_step_pdis",
             target_type=int,
@@ -2010,15 +2010,15 @@
             i.e., :math:`\\pi(a | s) \\forall a \\in \\mathcal{A}`
 
         gamma: float, default=1.0
             Discount factor. The value should be within (0, 1].
 
         Return
         -------
-        V_hat: ndarray of shape (n_trajectories, )
+        V_hat: float
             Estimated policy value.
 
         """
         check_scalar(
             n_step_pdis,
             name="n_step_pdis",
             target_type=int,
@@ -2474,15 +2474,15 @@
             Estimated initial state value.
 
         gamma: float, default=1.0
             Discount factor. The value should be within (0, 1].
 
         Return
         -------
-        V_hat: ndarray of shape (n_trajectories, )
+        V_hat: float
             Estimated policy value.
 
         """
         check_scalar(
             n_step_pdis,
             name="n_step_pdis",
             target_type=int,
```

### Comparing `scope-rl-0.1.1/scope_rl/ope/estimators_base.py` & `scope-rl-0.1.2/scope_rl/ope/estimators_base.py`

 * *Files identical despite different names*

### Comparing `scope-rl-0.1.1/scope_rl/ope/input.py` & `scope-rl-0.1.2/scope_rl/ope/input.py`

 * *Files identical despite different names*

### Comparing `scope-rl-0.1.1/scope_rl/ope/online.py` & `scope-rl-0.1.2/scope_rl/ope/online.py`

 * *Files identical despite different names*

### Comparing `scope-rl-0.1.1/scope_rl/ope/ope.py` & `scope-rl-0.1.2/scope_rl/ope/ope.py`

 * *Files identical despite different names*

### Comparing `scope-rl-0.1.1/scope_rl/ope/ops.py` & `scope-rl-0.1.2/scope_rl/ope/ops.py`

 * *Files 0% similar despite different names*

```diff
@@ -5326,15 +5326,15 @@
         return_safety_violation_rate: bool, default=False.
             Whether to calculate and return the safety violate.
 
         safety_threshold: float, default=0.0 (>= 0)
             The conditional value at risk required to be considered a safe policy.
 
         clip_sharpe_ratio: bool, default=False
-            Whether to clip a large value of SharpRatio with 1e2.
+            Whether to clip a large value of SharpeRatio with 1e2.
 
         return_by_dataframe: bool, default=False
             Whether to return the result in a dataframe format.
 
         Return
         -------
         topk_metric_dict/topk_metric_df: dict or dataframe
@@ -6278,15 +6278,15 @@
 
         relative_safety_criteria: float, default=None
             The relative policy value required to be considered a safe policy.
             For example, when 0.9 is given, candidate policy must exceed 90\\% of the behavior policy performance.
             Only applicable when using a single behavior policy.
 
         clip_sharpe_ratio: bool, default=False
-            Whether to clip a large value of SharpRatio with 1e2.
+            Whether to clip a large value of SharpeRatio with 1e2.
 
         cis: list of {"bootstrap", "hoeffding", "bernstein", "ttest"}, default=["bootstrap"]
             Estimation methods for confidence intervals.
 
         ope_alpha: float, default=0.05
             Significance level. The value should be within `[0, 1)`.
 
@@ -6776,15 +6776,15 @@
         return_safety_violation_rate: bool, default=False.
             Whether to calculate and return the safety violate.
 
         safety_threshold: float, default=None.
             A policy whose policy value is below the given threshold is to be considered unsafe.
 
         clip_sharpe_ratio: bool, default=False
-            Whether to clip a large value of SharpRatio with 1e2.
+            Whether to clip a large value of SharpeRatio with 1e2.
 
         return_by_dataframe: bool, default=False
             Whether to return the result in a dataframe format.
 
         Return
         -------
         topk_metric_dict/topk_metric_df: dict or dataframe
@@ -6938,15 +6938,15 @@
         return_safety_violation_rate: bool, default=False.
             Whether to calculate and return the safety violate.
 
         safety_threshold: float, default=None.
             A policy whose policy value is below the given threshold is to be considered unsafe.
 
         clip_sharpe_ratio: bool, default=False
-            Whether to clip a large value of SharpRatio with 1e2.
+            Whether to clip a large value of SharpeRatio with 1e2.
 
         return_by_dataframe: bool, default=False
             Whether to return the result in a dataframe format.
 
         Return
         -------
         topk_metric_dict/topk_metric_df: dict or dataframe
@@ -7101,15 +7101,15 @@
         return_safety_violation_rate: bool, default=False.
             Whether to calculate and return the safety violate.
 
         safety_threshold: float, default=None.
             A policy whose policy value is below the given threshold is to be considered unsafe.
 
         clip_sharpe_ratio: bool, default=False
-            Whether to clip a large value of SharpRatio with 1e2.
+            Whether to clip a large value of SharpeRatio with 1e2.
 
         return_by_dataframe: bool, default=False
             Whether to return the result in a dataframe format.
 
         Return
         -------
         topk_metric_dict/topk_metric_df: dict or dataframe
@@ -7263,15 +7263,15 @@
         return_safety_violation_rate: bool, default=False.
             Whether to calculate and return the safety violate.
 
         safety_threshold: float, default=None.
             A policy whose policy value is below the given threshold is to be considered unsafe.
 
         clip_sharpe_ratio: bool, default=False
-            Whether to clip a large value of SharpRatio with 1e2.
+            Whether to clip a large value of SharpeRatio with 1e2.
 
         return_by_dataframe: bool, default=False
             Whether to return the result in a dataframe format.
 
         Return
         -------
         topk_metric_dict/topk_metric_df: dict or dataframe
@@ -7578,15 +7578,15 @@
         legend: bool, default=True
             Whether to include a legend in the figure.
 
         ylabel: str, default="policy performance"
             Label of the y-axis.
 
         ymax_sharp_ratio: float, default=None
-            Maximum value in y-axis of the plot of SharpRatio.
+            Maximum value in y-axis of the plot of SharpeRatio.
 
         fig_dir: Path, default=None
             Path to store the bar figure.
             If `None` is given, the figure will not be saved.
 
         fig_name: str, default="topk_policy_value_standard_ope.png"
             Name of the bar figure.
@@ -7872,18 +7872,18 @@
 
         relative_safety_criteria: float, default=None
             The relative policy value required to be considered a safe policy.
             For example, when 0.9 is given, candidate policy must exceed 90\\% of the behavior policy performance.
             Only applicable when using a single behavior policy.
 
         clip_sharpe_ratio: bool, default=False
-            Whether to clip a large value of SharpRatio with 1e2.
+            Whether to clip a large value of SharpeRatio with 1e2.
 
         ymax_sharp_ratio: float, default=None
-            Maximum value in y-axis of the plot of SharpRatio.
+            Maximum value in y-axis of the plot of SharpeRatio.
 
         visualize_ci: bool, default=False
             Whether to visualize ci. (Only applicable when :class:`MultipleInputDict` is given.)
 
         plot_ci: {"bootstrap", "hoeffding", "bernstein", "ttest"}, default="bootstrap"
             Method to estimate the confidence interval.
 
@@ -8076,18 +8076,18 @@
             A policy whose policy value is below the given threshold is to be considered unsafe.
 
         relative_safety_criteria: float, default=None
             The relative policy value required to be considered a safe policy.
             For example, when 0.9 is given, candidate policy must exceed 90\\% of the behavior policy performance.
 
         clip_sharpe_ratio: bool, default=False
-            Whether to clip a large value of SharpRatio with 1e2.
+            Whether to clip a large value of SharpeRatio with 1e2.
 
         ymax_sharp_ratio: float, default=None
-            Maximum value in y-axis of the plot of SharpRatio.
+            Maximum value in y-axis of the plot of SharpeRatio.
 
         visualize_ci: bool, default=False
             Whether to visualize ci. (Only applicable when :class:`MultipleInputDict` is given.)
 
         plot_ci: {"bootstrap", "hoeffding", "bernstein", "ttest"}, default="bootstrap"
             Method to estimate the confidence interval.
 
@@ -8283,18 +8283,18 @@
             A policy whose policy value is below the given threshold is to be considered unsafe.
 
         relative_safety_criteria: float, default=None
             The relative policy value required to be considered a safe policy.
             For example, when 0.9 is given, candidate policy must exceed 90\\% of the behavior policy performance.
 
         clip_sharpe_ratio: bool, default=False
-            Whether to clip a large value of SharpRatio with 1e2.
+            Whether to clip a large value of SharpeRatio with 1e2.
 
         ymax_sharp_ratio: float, default=None
-            Maximum value in y-axis of the plot of SharpRatio.
+            Maximum value in y-axis of the plot of SharpeRatio.
 
         ope_cis: list of {"bootstrap", "hoeffding", "bernstein", "ttest"}, default=["bootstrap"]
             Estimation methods for confidence intervals.
 
         ope_alpha: float, default=0.05
             Significance level. The value should be within `[0, 1)`.
 
@@ -8900,18 +8900,18 @@
             Maximum number of policies to be deployed.
             If `None` is given, all the policies will be deployed.
 
         safety_threshold: float, default=0.0 (>= 0)
             The conditional value at risk required to be considered a safe policy.
 
         clip_sharpe_ratio: bool, default=False
-            Whether to clip a large value of SharpRatio with 1e2.
+            Whether to clip a large value of SharpeRatio with 1e2.
 
         ymax_sharp_ratio: float, default=None
-            Maximum value in y-axis of the plot of SharpRatio.
+            Maximum value in y-axis of the plot of SharpeRatio.
 
         visualize_ci: bool, default=False
             Whether to visualize ci. (Only applicable when :class:`MultipleInputDict` is given.)
 
         plot_ci: {"bootstrap", "hoeffding", "bernstein", "ttest"}, default="bootstrap"
             Method to estimate the confidence interval.
 
@@ -8921,15 +8921,15 @@
         plot_n_bootstrap_samples: int, default=10000 (> 0)
             Number of resampling performed in the bootstrap procedure.
 
         random_state: int, default=None (>= 0)
             Random state.
 
         ymax_sharp_ratio: float, default=None
-            Maximum value in y-axis of the plot of SharpRatio.
+            Maximum value in y-axis of the plot of SharpeRatio.
 
         legend: bool, default=True
             Whether to include a legend in the figure.
 
         fig_dir: Path, default=None
             Path to store the bar figure.
             If `None` is given, the figure will not be saved.
@@ -9108,18 +9108,18 @@
             Maximum number of policies to be deployed.
             If `None` is given, all the policies will be deployed.
 
         safety_threshold: float, default=0.0 (>= 0)
             The conditional value at risk required to be considered a safe policy.
 
         clip_sharpe_ratio: bool, default=False
-            Whether to clip a large value of SharpRatio with 1e2.
+            Whether to clip a large value of SharpeRatio with 1e2.
 
         ymax_sharp_ratio: float, default=None
-            Maximum value in y-axis of the plot of SharpRatio.
+            Maximum value in y-axis of the plot of SharpeRatio.
 
         visualize_ci: bool, default=False
             Whether to visualize ci. (Only applicable when :class:`MultipleInputDict` is given.)
 
         plot_ci: {"bootstrap", "hoeffding", "bernstein", "ttest"}, default="bootstrap"
             Method to estimate the confidence interval.
 
@@ -9314,18 +9314,18 @@
             Maximum number of policies to be deployed.
             If `None` is given, all the policies will be deployed.
 
         safety_threshold: float, default=0.0 (>= 0)
             The conditional value at risk required to be considered a safe policy.
 
         clip_sharpe_ratio: bool, default=False
-            Whether to clip a large value of SharpRatio with 1e2.
+            Whether to clip a large value of SharpeRatio with 1e2.
 
         ymax_sharp_ratio: float, default=None
-            Maximum value in y-axis of the plot of SharpRatio.
+            Maximum value in y-axis of the plot of SharpeRatio.
 
         visualize_ci: bool, default=False
             Whether to visualize ci. (Only applicable when :class:`MultipleInputDict` is given.)
 
         plot_ci: {"bootstrap", "hoeffding", "bernstein", "ttest"}, default="bootstrap"
             Method to estimate the confidence interval.
 
@@ -9519,18 +9519,18 @@
             Maximum number of policies to be deployed.
             If `None` is given, all the policies will be deployed.
 
         safety_threshold: float, default=0.0 (>= 0)
             The conditional value at risk required to be considered a safe policy.
 
         clip_sharpe_ratio: bool, default=False
-            Whether to clip a large value of SharpRatio with 1e2.
+            Whether to clip a large value of SharpeRatio with 1e2.
 
         ymax_sharp_ratio: float, default=None
-            Maximum value in y-axis of the plot of SharpRatio.
+            Maximum value in y-axis of the plot of SharpeRatio.
 
         visualize_ci: bool, default=False
             Whether to visualize ci. (Only applicable when :class:`MultipleInputDict` is given.)
 
         plot_ci: {"bootstrap", "hoeffding", "bernstein", "ttest"}, default="bootstrap"
             Method to estimate the confidence interval.
 
@@ -9540,15 +9540,15 @@
         plot_n_bootstrap_samples: int, default=10000 (> 0)
             Number of resampling performed in the bootstrap procedure.
 
         random_state: int, default=None (>= 0)
             Random state.
 
         ymax_sharp_ratio: float, default=None
-            Maximum value in y-axis of the plot of SharpRatio.
+            Maximum value in y-axis of the plot of SharpeRatio.
 
         legend: bool, default=True
             Whether to include a legend in the figure.
 
         fig_dir: Path, default=None
             Path to store the bar figure.
             If `None` is given, the figure will not be saved.
```

### Comparing `scope-rl-0.1.1/scope_rl/ope/weight_value_learning/__init__.py` & `scope-rl-0.1.2/scope_rl/ope/weight_value_learning/__init__.py`

 * *Files identical despite different names*

### Comparing `scope-rl-0.1.1/scope_rl/ope/weight_value_learning/augmented_lagrangian_learning_continuous.py` & `scope-rl-0.1.2/scope_rl/ope/weight_value_learning/augmented_lagrangian_learning_continuous.py`

 * *Files identical despite different names*

### Comparing `scope-rl-0.1.1/scope_rl/ope/weight_value_learning/augmented_lagrangian_learning_discrete.py` & `scope-rl-0.1.2/scope_rl/ope/weight_value_learning/augmented_lagrangian_learning_discrete.py`

 * *Files identical despite different names*

### Comparing `scope-rl-0.1.1/scope_rl/ope/weight_value_learning/base.py` & `scope-rl-0.1.2/scope_rl/ope/weight_value_learning/base.py`

 * *Files identical despite different names*

### Comparing `scope-rl-0.1.1/scope_rl/ope/weight_value_learning/function.py` & `scope-rl-0.1.2/scope_rl/ope/weight_value_learning/function.py`

 * *Files identical despite different names*

### Comparing `scope-rl-0.1.1/scope_rl/ope/weight_value_learning/minimax_value_learning_continuous.py` & `scope-rl-0.1.2/scope_rl/ope/weight_value_learning/minimax_value_learning_continuous.py`

 * *Files identical despite different names*

### Comparing `scope-rl-0.1.1/scope_rl/ope/weight_value_learning/minimax_value_learning_discrete.py` & `scope-rl-0.1.2/scope_rl/ope/weight_value_learning/minimax_value_learning_discrete.py`

 * *Files identical despite different names*

### Comparing `scope-rl-0.1.1/scope_rl/ope/weight_value_learning/minimax_weight_learning_continuous.py` & `scope-rl-0.1.2/scope_rl/ope/weight_value_learning/minimax_weight_learning_continuous.py`

 * *Files identical despite different names*

### Comparing `scope-rl-0.1.1/scope_rl/ope/weight_value_learning/minimax_weight_learning_discrete.py` & `scope-rl-0.1.2/scope_rl/ope/weight_value_learning/minimax_weight_learning_discrete.py`

 * *Files identical despite different names*

### Comparing `scope-rl-0.1.1/scope_rl/policy/__init__.py` & `scope-rl-0.1.2/scope_rl/policy/__init__.py`

 * *Files identical despite different names*

### Comparing `scope-rl-0.1.1/scope_rl/policy/encoder.py` & `scope-rl-0.1.2/scope_rl/policy/encoder.py`

 * *Files identical despite different names*

### Comparing `scope-rl-0.1.1/scope_rl/policy/head.py` & `scope-rl-0.1.2/scope_rl/policy/head.py`

 * *Files identical despite different names*

### Comparing `scope-rl-0.1.1/scope_rl/policy/orl.py` & `scope-rl-0.1.2/scope_rl/policy/orl.py`

 * *Files identical despite different names*

### Comparing `scope-rl-0.1.1/scope_rl/utils.py` & `scope-rl-0.1.2/scope_rl/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -800,15 +800,15 @@
     def render(self, mode: str = "human"):
         self.env.render()
 
     def close(self):
         self.env.close()
 
     def seed(self, seed: Optional[int] = None):
-        self.env.reset(seed)
+        self.env.reset(seed=seed)
 
     def __getattr__(self, key) -> Any:
         return object.__getattribute__(self.env, key)
 
 
 class MinMaxActionScaler(ActionScaler):
     r"""Min-Max normalization action preprocessing (temporally supported).
```

### Comparing `scope-rl-0.1.1/scope_rl.egg-info/PKG-INFO` & `scope-rl-0.1.2/scope_rl.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scope-rl
-Version: 0.1.1
+Version: 0.1.2
 Summary: SCOPE-RL: A pipeline for offline reinforcement learning research and applications
 Home-page: https://github.com/hakuhodo-technologies/scope-rl
 Author: Haruka Kiyohara
 Author-email: hk844@cornell.edu
 License: Apache License 2.0
 Keywords: off-policy evaluation,offline reinforcement learning,risk assessment
 Platform: UNKNOWN
@@ -45,35 +45,37 @@
 - [Contact](#contact)
 - [Reference](#reference)
 
 </details>
 
 **Documentation is available [here](https://scope-rl.readthedocs.io/en/latest/)**
 
+**Stable versions are available at [PyPI](https://pypi.org/project/scope-rl/)**
+
 ## Overview
 
 *SCOPE-RL* is an open-source Python Software for implementing the end-to-end procedure regarding **offline Reinforcement Learning (offline RL)**, from data collection to offline policy learning, off-policy performance evaluation, and policy selection. Our software includes a series of modules to implement synthetic dataset generation, dataset preprocessing, estimators for Off-Policy Evaluation (OPE), and Off-Policy Selection (OPS) methods.
 
-This software is also compatible with [d3rlpy](https://github.com/takuseno/d3rlpy), which implements a range of online and offline RL methods. SCOPE-RL enables an easy, transparent, and reliable experiment in offline RL research on any environment with [OpenAI Gym](https://gym.openai.com) and [Gymnasium](https://gymnasium.farama.org/)-like interface. It also facilitates implementation of offline RL in practice on a variety of customized datasets and on real-world datasets.
+This software is also compatible with [d3rlpy](https://github.com/takuseno/d3rlpy), which implements a range of online and offline RL methods. SCOPE-RL enables an easy, transparent, and reliable experiment in offline RL research on any environment with [OpenAI Gym](https://gym.openai.com) and [Gymnasium](https://gymnasium.farama.org/)-like interface. It also facilitates the implementation of offline RL in practice on a variety of customized datasets and real-world datasets.
 
 In particular, SCOPE-RL enables and facilitates evaluation and algorithm comparison related to the following research topics:
 
-- **Offline Reinforcement Learning**: Offline RL aims at learning a new policy from only offline logged data collected by a behavior policy. SCOPE-RL enables flexible experiment using customized dataset collected by various behavior policies and on a variety of environment.
+- **Offline Reinforcement Learning**: Offline RL aims at learning a new policy from only offline logged data collected by a behavior policy. SCOPE-RL enables flexible experiments using customized datasets collected by various behavior policies and environments.
 
 - **Off-Policy Evaluation**: OPE aims at evaluating the performance of a counterfactual policy using only offline logged data. SCOPE-RL supports many OPE estimators and streamlines the experimental procedure to evaluate and compare OPE estimators. Moreover, we also implement advanced OPE methods, such as estimators based on state-action density estimation and cumulative distribution estimation.
 
 - **Off-Policy Selection**: OPS aims at identifying the best-performing policy from a pool of several candidate policies using offline logged data. SCOPE-RL supports some basic OPS methods and provides several metrics to evaluate the OPS accuracy.
 
 This software is inspired by [Open Bandit Pipeline](https://github.com/st-tech/zr-obp), which is a library for OPE in contextual bandits. However, SCOPE-RL also implements a set of OPE estimators and tools to facilitate experiments about OPE for the contextual bandit setup by itself as well as those for RL.
 
 ### Implementations
 
 *SCOPE-RL* mainly consists of the following three modules.
 - [**dataset module**](./_gym/dataset): This module provides tools to generate synthetic data from any environment on top of [OpenAI Gym](http://gym.openai.com/) and [Gymnasium](https://gymnasium.farama.org/)-like interface. It also provides tools to pre-process the logged data.
-- [**policy module**](./_gym/policy): This module provides a wrapper class for [d3rlpy](https://github.com/takuseno/d3rlpy) to enable a flexible data collection.
+- [**policy module**](./_gym/policy): This module provides a wrapper class for [d3rlpy](https://github.com/takuseno/d3rlpy) to enable flexible data collection.
 - [**ope module**](./_gym/ope): This module provides a generic abstract class to implement OPE estimators. It also provides some tools useful for performing OPS.
 
 <details>
 <summary><strong>Behavior Policy </strong>(click to expand)</summary>
 
 - Discrete
   - Epsilon Greedy
@@ -129,38 +131,39 @@
 <details>
 <summary><strong>Evaluation Metrics of OPS </strong>(click to expand)</summary>
 
 - Mean Squared Error
 - Spearman's Rank Correlation Coefficient
 - Regret
 - Type I and Type II Error Rates
-- {Best/Worst/Mean} performances of top-k policies
+- {Best/Worst/Mean/Std} performances of top-k policies
 - Safety violation rate of top-k policies
+- SharpeRatio@k
 
 </details>
 
-Note that in addition to the above OPE and OPS methods, researcher can easily implement and compare their own estimators through a generic abstract class implemented in SCOPE-RL. Moreover, practitioners can apply the above methods to their real-world data to evaluate and choose counterfactual policies for their own practical situations.
+Note that in addition to the above OPE and OPS methods, researchers can easily implement and compare their own estimators through a generic abstract class implemented in SCOPE-RL. Moreover, practitioners can apply the above methods to their real-world data to evaluate and choose counterfactual policies for their own practical situations.
 
 To provide an example of performing a customized experiment imitating a practical setup, we also provide [RTBGym](./rtbgym) and [RecGym](./recgym), RL environments for Real-Time Bidding (RTB) and Recommender Systems.
 
 ## Installation
 
 You can install SCOPE-RL using Python's package manager `pip`.
 ```
 pip install scope-rl
 ```
 
-You can also install SCOPE-RL from source.
+You can also install SCOPE-RL from the source.
 ```bash
 git clone https://github.com/hakuhodo-technologies/scope-rl
 cd scope-rl
 python setup.py install
 ```
 
-SCOPE-RL supports Python 3.9 or newer. See [requirements.txt](./requirements.txt) for other requirements.
+SCOPE-RL supports Python 3.9 or newer. See [requirements.txt](./requirements.txt) for other requirements. Please also refer to issue [#17](https://github.com/hakuhodo-technologies/scope-rl/issues/17) when you encounter some dependency conflicts.
 
 ## Usage
 
 Here, we provide an example workflow to perform offline RL, OPE, and OPS using SCOPE-RL on [RTBGym](./rtbgym).
 
 ### Synthetic Dataset Generation and Data Preprocessing
 
@@ -258,15 +261,15 @@
     n_steps=10000,
     scorers={},
 )
 ```
 
 ### Basic Off-Policy Evaluation
 
-Then, we evaluate the performance of several evaluation policy (ddqn, cql, and random) using offline logged data collected by the behavior policy. Specifically, we compare the estimation results of various OPE estimators, including Direct Method (DM), Trajectory-wise Importance Sampling (TIS), Per-Decision Importance Sampling (PDIS), and Doubly Robust (DR) below.
+Then, we evaluate the performance of several evaluation policies (ddqn, cql, and random) using offline logged data collected by the behavior policy. Specifically, we compare the estimation results of various OPE estimators, including Direct Method (DM), Trajectory-wise Importance Sampling (TIS), Per-Decision Importance Sampling (PDIS), and Doubly Robust (DR) below.
 
 ```Python
 # implement a basic OPE procedure using SCOPE-RL
 
 # import SCOPE-RL modules
 from scope_rl.ope import CreateOPEInput
 from scope_rl.ope import OffPolicyEvaluation as OPE
@@ -325,15 +328,15 @@
 <div align="center"><img src="https://raw.githubusercontent.com/hakuhodo-technologies/scope-rl/main/images/ope_policy_value_basic.png" width="100%"/></div>
 <figcaption>
 <p align="center">
   Policy Value Estimated by OPE Estimators
 </p>
 </figcaption>
 
-More formal example implementations with RTBGym is available at [./examples/quickstart/rtb/](./examples/quickstart/rtb). Those with RecGym are also available at [./examples/quickstart/rec/](./examples/quickstart/rec).
+More formal example implementations with RTBGym are available at [./examples/quickstart/rtb/](./examples/quickstart/rtb). Those with RecGym are also available at [./examples/quickstart/rec/](./examples/quickstart/rec).
 
 ### Advanced Off-Policy Evaluation
 
 We can also estimate various statics of the evaluation policy, beyond just its expected performance, including variance and conditional value at risk (CVaR) via estimating the cumulative distribution function (CDF) of the reward under the evaluation policy.
 
 ```Python
 # implement a cumulative distribution estimation procedure using SCOPE-RL
@@ -373,15 +376,15 @@
 </p>
 </figcaption>
 
 For more extensive examples, please refer to [quickstart/rtb/rtb_synthetic_discrete_advanced.ipynb](./examples/quickstart/rtb/rtb_synthetic_discrete_advanced.ipynb).
 
 ### Off-Policy Selection and Evaluation of OPE/OPS
 
-We can also select the best-performing policy among a set of candidate policies based on the OPE results using the OPS class. It is also possible to evaluate the reliability of OPE/OPS using various metrics such as mean-squared-error, rank correlation, regret, and type I and type II error rates.
+We can also select the best-performing policy among a set of candidate policies based on the OPE results using the OPS class. It is also possible to evaluate the reliability of OPE/OPS using various metrics such as mean squaredberror, rank correlation, regret, and type I and type II error rates.
 
 ```Python
 # perform off-policy selection based on the OPE results
 
 # import SCOPE-RL modules
 from scope_rl.ope import OffPolicySelection
 
@@ -436,31 +439,52 @@
 [quickstart/rtb/rtb_synthetic_continuous_advanced.ipynb](./examples/quickstart/rtb/rtb_synthetic_continuous_advanced.ipynb) for continuous actions.
 
 ## Citation
 
 If you use our software in your work, please cite our paper:
 
 Haruka Kiyohara, Ren Kishimoto, Kosuke Kawakami, Ken Kobayashi, Kazuhide Nakata, Yuta Saito.<br>
+**SCOPE-RL: A Python Library for Offline Reinforcement Learning, Off-Policy Evaluation, and Policy Selection**<br>
+[link]() (a preprint coming soon..)
+
+Bibtex:
+```
+@article{kiyohara2023towards,
+  author = {Kiyohara, Haruka and Kishimoto, Ren and Kawakami, Kosuke and Kobayashi, Ken and Nataka, Kazuhide and Saito, Yuta},
+  title = {SCOPE-RL: A Python Library for Offline Reinforcement Learning, Off-Policy Evaluation, and Policy Selection},
+  journal={arXiv preprint arXiv:23xx.xxxxx},
+  year={2023},
+}
+```
+
+If you use our proposed metric "SharpeRatio@k" in your work, please cite our paper:
+
+Haruka Kiyohara, Ren Kishimoto, Kosuke Kawakami, Ken Kobayashi, Kazuhide Nakata, Yuta Saito.<br>
 **Towards Assessing and Benchmarking Risk-Return Tradeoff of Off-Policy Evaluation in Reinforcement Learning**<br>
 [link]() (a preprint coming soon..)
 
 Bibtex:
 ```
 @article{kiyohara2023towards,
   author = {Kiyohara, Haruka and Kishimoto, Ren and Kawakami, Kosuke and Kobayashi, Ken and Nataka, Kazuhide and Saito, Yuta},
   title = {Towards Assessing and Benchmarking Risk-Return Tradeoff of Off-Policy Evaluation in Reinforcement Learning},
-  journal = {A github repository},
-  pages = {xxx--xxx},
-  year = {2023},
+  journal={arXiv preprint arXiv:23xx.xxxxx},
+  year={2023},
 }
 ```
 
+## Google Group
+
+If you are interested in SCOPE-RL, please follow its updates via the google group:
+https://groups.google.com/g/scope-rl
+
+
 ## Contribution
 Any contributions to SCOPE-RL are more than welcome!
-Please refer to [CONTRIBUTING.md](./CONTRIBUTING.md) for general guidelines how to contribute the project.
+Please refer to [CONTRIBUTING.md](./CONTRIBUTING.md) for general guidelines on how to contribute to the project.
 
 ## License
 
 This project is licensed under Apache 2.0 license - see [LICENSE](LICENSE) file for details.
 
 ## Project Team
 
@@ -469,15 +493,15 @@
 - Kosuke Kawakami (HAKUHODO Technologies Inc.)
 - Ken Kobayashi (Tokyo Institute of Technology)
 - Kazuhide Nakata (Tokyo Institute of Technology)
 - [Yuta Saito](https://usait0.com/en/) (Cornell University)
 
 ## Contact
 
-For any question about the paper and software, feel free to contact: hk844@cornell.edu
+For any questions about the paper and software, feel free to contact: hk844@cornell.edu
 
 ## References
 
 <details>
 <summary><strong>Papers </strong>(click to expand)</summary>
 
 1. Alina Beygelzimer and John Langford. [The Offset Tree for Learning with Partial Labels](https://arxiv.org/abs/0812.4044). In *Proceedings of the 15th ACM SIGKDD International Conference on Knowledge Discovery and Data Mining*, 129-138, 2009.
@@ -526,15 +550,15 @@
 
 24. Tom Le Paine, Cosmin Paduraru, Andrea Michi, Caglar Gulcehre, Konrad Zolna, Alexander Novikov, Ziyu Wang, and Nando de Freitas. [Hyperparameter Selection for Offline Reinforcement Learning](https://arxiv.org/abs/2007.090550). *arXiv preprint arXiv:2007.09055*, 2020.
 
 25. Doina Precup, Richard S. Sutton, and Satinder P. Singh. [Eligibility Traces for Off-Policy Policy Evaluation](https://scholarworks.umass.edu/cgi/viewcontent.cgi?article=1079&context=cs_faculty_pubs). In *Proceedings of the 17th International Conference on Machine Learning*, 759–766, 2000.
 
 26. Rafael Figueiredo Prudencio, Marcos R. O. A. Maximo, and Esther Luna Colombini. [A Survey on Offline Reinforcement Learning: Taxonomy, Review, and Open Problems](https://arxiv.org/abs/2203.01387). *arXiv preprint arXiv:2203.01387*, 2022.
 
-27. Yuta Saito, Shunsuke Aihara, Megumi Matsutani, and Yusuke Narita. [Open Bandit Dataset and Pipeline: Towards Realistic and Reproducible Off-Policy Evaluation](https://arxiv.org/abs/2008.07146). In *Advances in Neural Information Processing Systems*, , 2021.
+27. Yuta Saito, Shunsuke Aihara, Megumi Matsutani, and Yusuke Narita. [Open Bandit Dataset and Pipeline: Towards Realistic and Reproducible Off-Policy Evaluation](https://arxiv.org/abs/2008.07146). In *Advances in Neural Information Processing Systems*, 2021.
 
 28. Takuma Seno and Michita Imai. [d3rlpy: An Offline Deep Reinforcement Library](https://arxiv.org/abs/2111.03788), *arXiv preprint arXiv:2111.03788*, 2021.
 
 29. Alex Strehl, John Langford, Sham Kakade, and Lihong Li. [Learning from Logged Implicit Exploration Data](https://arxiv.org/abs/1003.0120). In *Advances in Neural Information Processing Systems*, 2217-2225, 2010.
 
 30. Adith Swaminathan and Thorsten Joachims. [The Self-Normalized Estimator for Counterfactual Learning](https://papers.nips.cc/paper/2015/hash/39027dfad5138c9ca0c474d71db915c3-Abstract.html). In *Advances in Neural Information Processing Systems*, 3231-3239, 2015.
 
@@ -562,12 +586,12 @@
 
 <details>
 <summary><strong>Projects </strong>(click to expand)</summary>
 
 This project is strongly inspired by the following three packages.
 - **Open Bandit Pipeline**  -- a pipeline implementation of OPE in contextual bandits: [[github](https://github.com/st-tech/zr-obp)] [[documentation](https://zr-obp.readthedocs.io/en/latest/)] [[paper](https://arxiv.org/abs/2008.07146)]
 - **d3rlpy** -- a set of implementations of offline RL algorithms: [[github](https://github.com/takuseno/d3rlpy)] [[documentation](https://d3rlpy.readthedocs.io/en/v0.91/)] [[paper](https://arxiv.org/abs/2111.03788)]
-- **Spinning Up** -- an educational resource for learning deepl RL: [[github](https://github.com/openai/spinningup)] [[documentation](https://spinningup.openai.com/en/latest/)]
+- **Spinning Up** -- an educational resource for learning deep RL: [[github](https://github.com/openai/spinningup)] [[documentation](https://spinningup.openai.com/en/latest/)]
 
 </details>
```

### Comparing `scope-rl-0.1.1/scope_rl.egg-info/SOURCES.txt` & `scope-rl-0.1.2/scope_rl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scope-rl-0.1.1/setup.py` & `scope-rl-0.1.2/setup.py`

 * *Files identical despite different names*

