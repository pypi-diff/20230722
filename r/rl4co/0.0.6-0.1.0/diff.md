# Comparing `tmp/rl4co-0.0.6.tar.gz` & `tmp/rl4co-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rl4co-0.0.6.tar", last modified: Mon Jul 10 19:04:52 2023, max compression
+gzip compressed data, was "rl4co-0.1.0.tar", last modified: Sat Jul 22 20:09:57 2023, max compression
```

## Comparing `rl4co-0.0.6.tar` & `rl4co-0.1.0.tar`

### file list

```diff
@@ -1,130 +1,145 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:04:52.302782 rl4co-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)    11372 2023-07-10 19:04:40.000000 rl4co-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    21176 2023-07-10 19:04:52.302782 rl4co-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7287 2023-07-10 19:04:40.000000 rl4co-0.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2981 2023-07-10 19:04:40.000000 rl4co-0.0.6/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:04:52.286781 rl4co-0.0.6/rl4co/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:04:52.286781 rl4co-0.0.6/rl4co/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/data/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    12329 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/data/generate_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/data/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:04:52.290781 rl4co-0.0.6/rl4co/envs/
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/envs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8078 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/envs/atsp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:04:52.290781 rl4co-0.0.6/rl4co/envs/common/
--rw-r--r--   0 runner    (1001) docker     (123)     6061 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/envs/common/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/envs/common/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    15110 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/envs/cvrp.py
--rw-r--r--   0 runner    (1001) docker     (123)    14006 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/envs/dpp.py
--rw-r--r--   0 runner    (1001) docker     (123)    13205 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/envs/ffsp.py
--rw-r--r--   0 runner    (1001) docker     (123)    12232 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/envs/mdpp.py
--rw-r--r--   0 runner    (1001) docker     (123)    12670 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/envs/mtsp.py
--rw-r--r--   0 runner    (1001) docker     (123)    15062 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/envs/op.py
--rw-r--r--   0 runner    (1001) docker     (123)    16473 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/envs/pctsp.py
--rw-r--r--   0 runner    (1001) docker     (123)    10231 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/envs/pdp.py
--rw-r--r--   0 runner    (1001) docker     (123)     8457 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/envs/sdvrp.py
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/envs/spctsp.py
--rw-r--r--   0 runner    (1001) docker     (123)     7238 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/envs/tsp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:04:52.290781 rl4co-0.0.6/rl4co/models/
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:04:52.290781 rl4co-0.0.6/rl4co/models/nn/
--rw-r--r--   0 runner    (1001) docker     (123)    10127 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/models/nn/attention.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:04:52.290781 rl4co-0.0.6/rl4co/models/nn/env_embeddings/
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/models/nn/env_embeddings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7793 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/models/nn/env_embeddings/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/models/nn/env_embeddings/dynamic.py
--rw-r--r--   0 runner    (1001) docker     (123)     9582 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/models/nn/env_embeddings/init.py
--rw-r--r--   0 runner    (1001) docker     (123)    29517 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/models/nn/flash_attention.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:04:52.290781 rl4co-0.0.6/rl4co/models/nn/graph/
--rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/models/nn/graph/gat.py
--rw-r--r--   0 runner    (1001) docker     (123)     3014 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/models/nn/graph/gcn.py
--rw-r--r--   0 runner    (1001) docker     (123)     5573 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/models/nn/graph/mpnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/models/nn/mlp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/models/nn/ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/models/nn/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:04:52.282781 rl4co-0.0.6/rl4co/models/rl/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:04:52.290781 rl4co-0.0.6/rl4co/models/rl/ppo/
--rw-r--r--   0 runner    (1001) docker     (123)     4931 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/models/rl/ppo/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/models/rl/ppo/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:04:52.290781 rl4co-0.0.6/rl4co/models/rl/reinforce/
--rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/models/rl/reinforce/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7402 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/models/rl/reinforce/baselines.py
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/models/rl/reinforce/critic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:04:52.282781 rl4co-0.0.6/rl4co/models/zoo/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:04:52.294782 rl4co-0.0.6/rl4co/models/zoo/am/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/models/zoo/am/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6295 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/models/zoo/am/decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/models/zoo/am/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/models/zoo/am/policy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:04:52.294782 rl4co-0.0.6/rl4co/models/zoo/amppo/
--rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/models/zoo/amppo/decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/models/zoo/amppo/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3865 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/models/zoo/amppo/policy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:04:52.294782 rl4co-0.0.6/rl4co/models/zoo/ham/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/models/zoo/ham/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18979 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/models/zoo/ham/attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/models/zoo/ham/encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/models/zoo/ham/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/models/zoo/ham/policy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:04:52.294782 rl4co-0.0.6/rl4co/models/zoo/mdam/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/models/zoo/mdam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12183 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/models/zoo/mdam/decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     9144 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/models/zoo/mdam/encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/models/zoo/mdam/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4211 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/models/zoo/mdam/policy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:04:52.294782 rl4co-0.0.6/rl4co/models/zoo/pomo/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/models/zoo/pomo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/models/zoo/pomo/augmentations.py
--rw-r--r--   0 runner    (1001) docker     (123)     5826 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/models/zoo/pomo/decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4577 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/models/zoo/pomo/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/models/zoo/pomo/policy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:04:52.298782 rl4co-0.0.6/rl4co/models/zoo/ptrnet/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/models/zoo/ptrnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/models/zoo/ptrnet/critic.py
--rw-r--r--   0 runner    (1001) docker     (123)     6254 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/models/zoo/ptrnet/decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/models/zoo/ptrnet/encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/models/zoo/ptrnet/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/models/zoo/ptrnet/policy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:04:52.298782 rl4co-0.0.6/rl4co/models/zoo/symnco/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/models/zoo/symnco/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/models/zoo/symnco/augmentations.py
--rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/models/zoo/symnco/decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/models/zoo/symnco/losses.py
--rw-r--r--   0 runner    (1001) docker     (123)     5195 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/models/zoo/symnco/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/models/zoo/symnco/policy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:04:52.298782 rl4co-0.0.6/rl4co/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)    13869 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/tasks/eval.py
--rw-r--r--   0 runner    (1001) docker     (123)     8881 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/tasks/rl4co.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:04:52.302782 rl4co-0.0.6/rl4co/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:04:52.302782 rl4co-0.0.6/rl4co/utils/callbacks/
--rw-r--r--   0 runner    (1001) docker     (123)     3975 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/utils/callbacks/speed_monitor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:04:52.302782 rl4co-0.0.6/rl4co/utils/download/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/utils/download/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     9470 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/utils/download/downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     4628 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/utils/download/gdrive.py
--rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/utils/download/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/utils/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/utils/instantiators.py
--rw-r--r--   0 runner    (1001) docker     (123)     4660 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/utils/lightning.py
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/utils/logging_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4177 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/utils/ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     5565 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/utils/param_grouping.py
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/utils/pylogger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/utils/rich_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/utils/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/utils/transfer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6508 2023-07-10 19:04:40.000000 rl4co-0.0.6/rl4co/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:04:52.286781 rl4co-0.0.6/rl4co.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21176 2023-07-10 19:04:52.000000 rl4co-0.0.6/rl4co.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-07-10 19:04:52.000000 rl4co-0.0.6/rl4co.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 19:04:52.000000 rl4co-0.0.6/rl4co.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-10 19:04:52.000000 rl4co-0.0.6/rl4co.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-10 19:04:52.000000 rl4co-0.0.6/rl4co.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 19:04:52.302782 rl4co-0.0.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:04:52.302782 rl4co-0.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-07-10 19:04:40.000000 rl4co-0.0.6/tests/test_envs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-07-10 19:04:40.000000 rl4co-0.0.6/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-07-10 19:04:40.000000 rl4co-0.0.6/tests/test_ops.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 20:09:57.069568 rl4co-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11372 2023-07-22 20:09:42.000000 rl4co-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20850 2023-07-22 20:09:57.069568 rl4co-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6965 2023-07-22 20:09:42.000000 rl4co-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-07-22 20:09:42.000000 rl4co-0.1.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 20:09:57.045568 rl4co-0.1.0/rl4co/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 20:09:57.049568 rl4co-0.1.0/rl4co/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/data/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12329 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/data/generate_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4091 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/data/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/data/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 20:09:57.049568 rl4co-0.1.0/rl4co/envs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/envs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8210 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/envs/atsp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 20:09:57.049568 rl4co-0.1.0/rl4co/envs/common/
+-rw-r--r--   0 runner    (1001) docker     (123)     6065 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/envs/common/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/envs/common/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15077 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/envs/cvrp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15199 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/envs/dpp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13577 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/envs/ffsp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12449 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/envs/mdpp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20158 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/envs/mpdp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13117 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/envs/mtsp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15062 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/envs/op.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16426 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/envs/pctsp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10011 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/envs/pdp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8390 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/envs/sdvrp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/envs/spctsp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7352 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/envs/tsp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 20:09:57.049568 rl4co-0.1.0/rl4co/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 20:09:57.053568 rl4co-0.1.0/rl4co/models/nn/
+-rw-r--r--   0 runner    (1001) docker     (123)     8414 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/models/nn/attention.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 20:09:57.053568 rl4co-0.1.0/rl4co/models/nn/env_embeddings/
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/models/nn/env_embeddings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7793 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/models/nn/env_embeddings/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/models/nn/env_embeddings/dynamic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9582 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/models/nn/env_embeddings/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29517 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/models/nn/flash_attention.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 20:09:57.053568 rl4co-0.1.0/rl4co/models/nn/graph/
+-rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/models/nn/graph/attnnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3451 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/models/nn/graph/gcn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5573 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/models/nn/graph/mpnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/models/nn/mlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/models/nn/ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/models/nn/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 20:09:57.053568 rl4co-0.1.0/rl4co/models/rl/
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/models/rl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 20:09:57.053568 rl4co-0.1.0/rl4co/models/rl/common/
+-rw-r--r--   0 runner    (1001) docker     (123)    11799 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/models/rl/common/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/models/rl/common/critic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 20:09:57.053568 rl4co-0.1.0/rl4co/models/rl/ppo/
+-rw-r--r--   0 runner    (1001) docker     (123)     9029 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/models/rl/ppo/ppo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 20:09:57.057568 rl4co-0.1.0/rl4co/models/rl/reinforce/
+-rw-r--r--   0 runner    (1001) docker     (123)    10438 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/models/rl/reinforce/baselines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5425 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/models/rl/reinforce/reinforce.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 20:09:57.041568 rl4co-0.1.0/rl4co/models/zoo/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 20:09:57.057568 rl4co-0.1.0/rl4co/models/zoo/am/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/models/zoo/am/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/models/zoo/am/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/models/zoo/am/policy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 20:09:57.041568 rl4co-0.1.0/rl4co/models/zoo/common/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 20:09:57.057568 rl4co-0.1.0/rl4co/models/zoo/common/autoregressive/
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/models/zoo/common/autoregressive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10108 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/models/zoo/common/autoregressive/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/models/zoo/common/autoregressive/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6036 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/models/zoo/common/autoregressive/policy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 20:09:57.057568 rl4co-0.1.0/rl4co/models/zoo/et/
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/models/zoo/et/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/models/zoo/et/policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/models/zoo/et/positional_encoding.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 20:09:57.057568 rl4co-0.1.0/rl4co/models/zoo/ham/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/models/zoo/ham/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18979 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/models/zoo/ham/attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/models/zoo/ham/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/models/zoo/ham/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/models/zoo/ham/policy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 20:09:57.061568 rl4co-0.1.0/rl4co/models/zoo/mdam/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/models/zoo/mdam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12401 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/models/zoo/mdam/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9144 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/models/zoo/mdam/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/models/zoo/mdam/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/models/zoo/mdam/policy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 20:09:57.061568 rl4co-0.1.0/rl4co/models/zoo/pomo/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/models/zoo/pomo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/models/zoo/pomo/augmentations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5826 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/models/zoo/pomo/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4582 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/models/zoo/pomo/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/models/zoo/pomo/policy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 20:09:57.061568 rl4co-0.1.0/rl4co/models/zoo/ppo/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/models/zoo/ppo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/models/zoo/ppo/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/models/zoo/ppo/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/models/zoo/ppo/policy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 20:09:57.061568 rl4co-0.1.0/rl4co/models/zoo/ptrnet/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/models/zoo/ptrnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/models/zoo/ptrnet/critic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6254 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/models/zoo/ptrnet/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/models/zoo/ptrnet/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/models/zoo/ptrnet/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/models/zoo/ptrnet/policy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 20:09:57.065568 rl4co-0.1.0/rl4co/models/zoo/symnco/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/models/zoo/symnco/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/models/zoo/symnco/losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5227 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/models/zoo/symnco/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/models/zoo/symnco/policy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 20:09:57.065568 rl4co-0.1.0/rl4co/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13869 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/tasks/eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3696 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/tasks/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 20:09:57.065568 rl4co-0.1.0/rl4co/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 20:09:57.065568 rl4co-0.1.0/rl4co/utils/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (123)     3975 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/utils/callbacks/speed_monitor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 20:09:57.069568 rl4co-0.1.0/rl4co/utils/download/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/utils/download/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9470 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/utils/download/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4628 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/utils/download/gdrive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/utils/download/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/utils/instantiators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/utils/lightning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/utils/ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/utils/optim_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5565 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/utils/param_grouping.py
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/utils/pylogger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/utils/rich_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/utils/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/utils/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/utils/transfer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6626 2023-07-22 20:09:42.000000 rl4co-0.1.0/rl4co/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 20:09:57.045568 rl4co-0.1.0/rl4co.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20850 2023-07-22 20:09:57.000000 rl4co-0.1.0/rl4co.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-07-22 20:09:57.000000 rl4co-0.1.0/rl4co.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 20:09:57.000000 rl4co-0.1.0/rl4co.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-22 20:09:57.000000 rl4co-0.1.0/rl4co.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-22 20:09:57.000000 rl4co-0.1.0/rl4co.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-22 20:09:57.069568 rl4co-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 20:09:57.069568 rl4co-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-07-22 20:09:42.000000 rl4co-0.1.0/tests/test_envs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-07-22 20:09:42.000000 rl4co-0.1.0/tests/test_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-07-22 20:09:42.000000 rl4co-0.1.0/tests/test_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-07-22 20:09:42.000000 rl4co-0.1.0/tests/test_training.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-07-22 20:09:42.000000 rl4co-0.1.0/tests/test_utils.py
```

### Comparing `rl4co-0.0.6/LICENSE` & `rl4co-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.6/PKG-INFO` & `rl4co-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rl4co
-Version: 0.0.6
+Version: 0.1.0
 Summary: RL4CO: an Extensive Reinforcement Learning for Combinatorial Optimization Benchmark
 Author-email: Federico Berto <berto.federico2@gmail.com>, Chuanbo Hua <cbhua@kaist.ac.kr>, Junyoung Park <junyoungpark.ml@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -214,27 +214,28 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: graph
 Provides-Extra: testing
-Provides-Extra: linting
+Provides-Extra: dev
 License-File: LICENSE
 
 <div align="center">
 
-# RL4CO
+<img src="https://github.com/kaist-silab/rl4co/assets/34462374/249462ea-b15d-4358-8a11-6508903dae58" style="width:40%">
+</br></br>
 
 
 <a href="https://pytorch.org/get-started/locally/"><img alt="PyTorch" src="https://img.shields.io/badge/PyTorch-ee4c2c?logo=pytorch&logoColor=white"></a>
 <a href="https://pytorchlightning.ai/"><img alt="Lightning" src="https://img.shields.io/badge/-Lightning-792ee5?logo=pytorchlightning&logoColor=white"></a>
 <a href="https://github.com/pytorch/rl"><img alt="base: TorchRL" src="https://img.shields.io/badge/base-TorchRL-red">
-<a href="https://hydra.cc/"><img alt="config: Hydra" src="https://img.shields.io/badge/config-Hydra-89b8cd"></a> [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)[![Slack](https://img.shields.io/badge/slack-chat-611f69.svg?logo=slack)](https://join.slack.com/t/rl4co/shared_invite/zt-1ytz2c1v4-0IkQ8NQH4TRXIX8PrRmDhQ)
-![license](https://img.shields.io/badge/license-Apache%202.0-green.svg?)<a href="https://colab.research.google.com/github/kaist-silab/rl4co/blob/main/notebooks/1-quickstart.ipynb"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"></a>[![PyPI](https://img.shields.io/pypi/v/rl4co?logo=pypi)](https://pypi.org/project/rl4co)
+<a href="https://hydra.cc/"><img alt="config: Hydra" src="https://img.shields.io/badge/config-Hydra-89b8cd"></a> [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![Slack](https://img.shields.io/badge/slack-chat-611f69.svg?logo=slack)](https://join.slack.com/t/rl4co/shared_invite/zt-1ytz2c1v4-0IkQ8NQH4TRXIX8PrRmDhQ)
+![license](https://img.shields.io/badge/license-Apache%202.0-green.svg?) <a href="https://colab.research.google.com/github/kaist-silab/rl4co/blob/main/notebooks/1-quickstart.ipynb"> <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"></a> [![PyPI](https://img.shields.io/pypi/v/rl4co?logo=pypi)](https://pypi.org/project/rl4co)
 [![Test](https://github.com/kaist-silab/rl4co/actions/workflows/tests.yml/badge.svg)](https://github.com/kaist-silab/rl4co/actions/workflows/tests.yml)
 <!-- ![testing](https://github.com/kaist-silab/ncobench/actions/workflows/tests.yml/badge.svg) -->
 
 [**Documentation**](https://rl4co.readthedocs.io/) |  [**Getting Started**](#getting-started) | [**Usage**](#usage) | [**Contributing**](#contributing) | [**Paper**](https://arxiv.org/abs/2306.17100) | [**Citation**](#cite-us)
 
 </div>
 
@@ -246,16 +247,15 @@
 
 RL4CO is built upon:
 - [TorchRL](https://github.com/pytorch/rl): official PyTorch framework for RL algorithms and vectorized environments on GPUs
 - [TensorDict](https://github.com/pytorch-labs/tensordict): a library to easily handle heterogeneous data such as states, actions and rewards
 - [PyTorch Lightning](https://github.com/Lightning-AI/lightning): a lightweight PyTorch wrapper for high-performance AI research
 - [Hydra](https://github.com/facebookresearch/hydra): a framework for elegantly configuring complex applications
 
-![image](https://github.com/kaist-silab/rl4co/assets/48984123/0db4efdd-1c93-4991-8f09-f3c6c1f35d60)
-
+![RL4CO Overview](https://github.com/kaist-silab/rl4co/assets/34462374/4d9a670f-ab7c-4fc8-9135-82d17cb6d0ee)
 
 ## Getting started
 <a href="https://colab.research.google.com/github/kaist-silab/rl4co/blob/main/notebooks/1-quickstart.ipynb"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"></a>
 
 RL4CO is now available for installation on `pip`!
 ```bash
 pip install rl4co
@@ -325,49 +325,38 @@
 ```
 </details>
 
 
 
 ### Minimalistic Example
 
-Here is a minimalistic example training the Attention Model with greedy rollout baseline on TSP in less than 50 lines of code:
+Here is a minimalistic example training the Attention Model with greedy rollout baseline on TSP in less than 30 lines of code:
 
 ```python
-from omegaconf import DictConfig
-import lightning as L
 from rl4co.envs import TSPEnv
-from rl4co.models.zoo.am import AttentionModel
-from rl4co.tasks.rl4co import RL4COLitModule
-
-config = DictConfig(
-    {"data": {
-            "train_size": 100000,
-            "val_size": 10000,
-            "batch_size": 512,
-        },
-    "optimizer": {"lr": 1e-4}}
-)
+from rl4co.models import AttentionModel
+from rl4co.utils import RL4COTrainer
 
 # Environment, Model, and Lightning Module
 env = TSPEnv(num_loc=20)
-model = AttentionModel(env)
-lit_module = RL4COLitModule(config, env, model)
+model = AttentionModel(env,
+                       baseline="rollout",
+                       train_data_size=100_000,
+                       test_data_size=10_000,
+                       optimizer_kwargs={'lr': 1e-4}
+                       )
 
 # Trainer
-trainer = L.Trainer(
-    max_epochs=3, # only few epochs
-    accelerator="gpu", # use GPU if available, else you can use others as "cpu"
-    logger=None, # can replace with WandbLogger, TensorBoardLogger, etc.
-    precision="16-mixed", # Lightning will handle faster training with mixed precision
-    gradient_clip_val=1.0, # clip gradients to avoid exploding gradients
-    reload_dataloaders_every_n_epochs=1, # necessary for sampling new data
-)
+trainer = RL4COTrainer(max_epochs=3)
 
 # Fit the model
-trainer.fit(lit_module)
+trainer.fit(model)
+
+# Test the model
+trainer.test(model)
 ```
 
 
 ### Testing
 
 Run tests with `pytest` from the root directory:
```

### Comparing `rl4co-0.0.6/README.md` & `rl4co-0.1.0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 <div align="center">
 
-# RL4CO
+<img src="https://github.com/kaist-silab/rl4co/assets/34462374/249462ea-b15d-4358-8a11-6508903dae58" style="width:40%">
+</br></br>
 
 
 <a href="https://pytorch.org/get-started/locally/"><img alt="PyTorch" src="https://img.shields.io/badge/PyTorch-ee4c2c?logo=pytorch&logoColor=white"></a>
 <a href="https://pytorchlightning.ai/"><img alt="Lightning" src="https://img.shields.io/badge/-Lightning-792ee5?logo=pytorchlightning&logoColor=white"></a>
 <a href="https://github.com/pytorch/rl"><img alt="base: TorchRL" src="https://img.shields.io/badge/base-TorchRL-red">
-<a href="https://hydra.cc/"><img alt="config: Hydra" src="https://img.shields.io/badge/config-Hydra-89b8cd"></a> [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)[![Slack](https://img.shields.io/badge/slack-chat-611f69.svg?logo=slack)](https://join.slack.com/t/rl4co/shared_invite/zt-1ytz2c1v4-0IkQ8NQH4TRXIX8PrRmDhQ)
-![license](https://img.shields.io/badge/license-Apache%202.0-green.svg?)<a href="https://colab.research.google.com/github/kaist-silab/rl4co/blob/main/notebooks/1-quickstart.ipynb"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"></a>[![PyPI](https://img.shields.io/pypi/v/rl4co?logo=pypi)](https://pypi.org/project/rl4co)
+<a href="https://hydra.cc/"><img alt="config: Hydra" src="https://img.shields.io/badge/config-Hydra-89b8cd"></a> [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![Slack](https://img.shields.io/badge/slack-chat-611f69.svg?logo=slack)](https://join.slack.com/t/rl4co/shared_invite/zt-1ytz2c1v4-0IkQ8NQH4TRXIX8PrRmDhQ)
+![license](https://img.shields.io/badge/license-Apache%202.0-green.svg?) <a href="https://colab.research.google.com/github/kaist-silab/rl4co/blob/main/notebooks/1-quickstart.ipynb"> <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"></a> [![PyPI](https://img.shields.io/pypi/v/rl4co?logo=pypi)](https://pypi.org/project/rl4co)
 [![Test](https://github.com/kaist-silab/rl4co/actions/workflows/tests.yml/badge.svg)](https://github.com/kaist-silab/rl4co/actions/workflows/tests.yml)
 <!-- ![testing](https://github.com/kaist-silab/ncobench/actions/workflows/tests.yml/badge.svg) -->
 
 [**Documentation**](https://rl4co.readthedocs.io/) |  [**Getting Started**](#getting-started) | [**Usage**](#usage) | [**Contributing**](#contributing) | [**Paper**](https://arxiv.org/abs/2306.17100) | [**Citation**](#cite-us)
 
 </div>
 
@@ -23,16 +24,15 @@
 
 RL4CO is built upon:
 - [TorchRL](https://github.com/pytorch/rl): official PyTorch framework for RL algorithms and vectorized environments on GPUs
 - [TensorDict](https://github.com/pytorch-labs/tensordict): a library to easily handle heterogeneous data such as states, actions and rewards
 - [PyTorch Lightning](https://github.com/Lightning-AI/lightning): a lightweight PyTorch wrapper for high-performance AI research
 - [Hydra](https://github.com/facebookresearch/hydra): a framework for elegantly configuring complex applications
 
-![image](https://github.com/kaist-silab/rl4co/assets/48984123/0db4efdd-1c93-4991-8f09-f3c6c1f35d60)
-
+![RL4CO Overview](https://github.com/kaist-silab/rl4co/assets/34462374/4d9a670f-ab7c-4fc8-9135-82d17cb6d0ee)
 
 ## Getting started
 <a href="https://colab.research.google.com/github/kaist-silab/rl4co/blob/main/notebooks/1-quickstart.ipynb"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"></a>
 
 RL4CO is now available for installation on `pip`!
 ```bash
 pip install rl4co
@@ -102,49 +102,38 @@
 ```
 </details>
 
 
 
 ### Minimalistic Example
 
-Here is a minimalistic example training the Attention Model with greedy rollout baseline on TSP in less than 50 lines of code:
+Here is a minimalistic example training the Attention Model with greedy rollout baseline on TSP in less than 30 lines of code:
 
 ```python
-from omegaconf import DictConfig
-import lightning as L
 from rl4co.envs import TSPEnv
-from rl4co.models.zoo.am import AttentionModel
-from rl4co.tasks.rl4co import RL4COLitModule
-
-config = DictConfig(
-    {"data": {
-            "train_size": 100000,
-            "val_size": 10000,
-            "batch_size": 512,
-        },
-    "optimizer": {"lr": 1e-4}}
-)
+from rl4co.models import AttentionModel
+from rl4co.utils import RL4COTrainer
 
 # Environment, Model, and Lightning Module
 env = TSPEnv(num_loc=20)
-model = AttentionModel(env)
-lit_module = RL4COLitModule(config, env, model)
+model = AttentionModel(env,
+                       baseline="rollout",
+                       train_data_size=100_000,
+                       test_data_size=10_000,
+                       optimizer_kwargs={'lr': 1e-4}
+                       )
 
 # Trainer
-trainer = L.Trainer(
-    max_epochs=3, # only few epochs
-    accelerator="gpu", # use GPU if available, else you can use others as "cpu"
-    logger=None, # can replace with WandbLogger, TensorBoardLogger, etc.
-    precision="16-mixed", # Lightning will handle faster training with mixed precision
-    gradient_clip_val=1.0, # clip gradients to avoid exploding gradients
-    reload_dataloaders_every_n_epochs=1, # necessary for sampling new data
-)
+trainer = RL4COTrainer(max_epochs=3)
 
 # Fit the model
-trainer.fit(lit_module)
+trainer.fit(model)
+
+# Test the model
+trainer.test(model)
 ```
 
 
 ### Testing
 
 Run tests with `pytest` from the root directory:
```

#### html2text {}

```diff
@@ -1,79 +1,73 @@
- # RL4CO [PyTorch] [Lightning] [base:_TorchRL]_[config:_Hydra]_[![Code_style:
- black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://
-    github.com/psf/black)[![Slack](https://img.shields.io/badge/slack-chat-
-   611f69.svg?logo=slack)](https://join.slack.com/t/rl4co/shared_invite/zt-
+[https://github.com/kaist-silab/rl4co/assets/34462374/249462ea-b15d-4358-8a11-
+ 6508903dae58]  [PyTorch] [Lightning] [base:_TorchRL]_[config:_Hydra]_[![Code
+  style:_black](https://img.shields.io/badge/code%20style-black-000000.svg)]
+ (https://github.com/psf/black)_[![Slack](https://img.shields.io/badge/slack-
+ chat-611f69.svg?logo=slack)](https://join.slack.com/t/rl4co/shared_invite/zt-
   1ytz2c1v4-0IkQ8NQH4TRXIX8PrRmDhQ)_![license](https://img.shields.io/badge/
-license-Apache%202.0-green.svg?)[Open_In_Colab][![PyPI](https://img.shields.io/
-  pypi/v/rl4co?logo=pypi)](https://pypi.org/project/rl4co)_[![Test](https://
- github.com/kaist-silab/rl4co/actions/workflows/tests.yml/badge.svg)](https://
-github.com/kaist-silab/rl4co/actions/workflows/tests.yml)__[**Documentation**]
- (https://rl4co.readthedocs.io/)_|_[**Getting_Started**](#getting-started)_|_
-[**Usage**](#usage)_|_[**Contributing**](#contributing)_|_[**Paper**](https://
-             arxiv.org/abs/2306.17100)_|_[**Citation**](#cite-us)
+      license-Apache%202.0-green.svg?)_[Open_In_Colab]_[![PyPI](https://
+  img.shields.io/pypi/v/rl4co?logo=pypi)](https://pypi.org/project/rl4co)_[!
+   [Test](https://github.com/kaist-silab/rl4co/actions/workflows/tests.yml/
+badge.svg)](https://github.com/kaist-silab/rl4co/actions/workflows/tests.yml)__
+  [**Documentation**](https://rl4co.readthedocs.io/)_|_[**Getting_Started**]
+(#getting-started)_|_[**Usage**](#usage)_|_[**Contributing**](#contributing)_|_
+   [**Paper**](https://arxiv.org/abs/2306.17100)_|_[**Citation**](#cite-us)
 --- An extensive Reinforcement Learning (RL) for Combinatorial Optimization
 (CO) benchmark. Our goal is to provide a unified framework for RL-based CO
 algorithms, and to facilitate reproducible research in this field, decoupling
 the science from the engineering. RL4CO is built upon: - [TorchRL](https://
 github.com/pytorch/rl): official PyTorch framework for RL algorithms and
 vectorized environments on GPUs - [TensorDict](https://github.com/pytorch-labs/
 tensordict): a library to easily handle heterogeneous data such as states,
 actions and rewards - [PyTorch Lightning](https://github.com/Lightning-AI/
 lightning): a lightweight PyTorch wrapper for high-performance AI research -
 [Hydra](https://github.com/facebookresearch/hydra): a framework for elegantly
-configuring complex applications ![image](https://github.com/kaist-silab/rl4co/
-assets/48984123/0db4efdd-1c93-4991-8f09-f3c6c1f35d60) ## Getting started [Open
-In_Colab] RL4CO is now available for installation on `pip`! ```bash pip install
-rl4co ``` ### Local install and development If you want to develop RL4CO or
-access the latest builds, we recommend you to install it locally with `pip` in
-editable mode: ```bash git clone https://github.com/kaist-silab/rl4co && cd
-rl4co pip install -e . ```  [Optional] Automatically install PyTorch with
-correct CUDA version These commands will [automatically install](https://
-github.com/pmeier/light-the-torch) PyTorch with the right GPU version for your
-system: ```bash pip install light-the-torch python3 -m light_the_torch install
--r --upgrade torch ``` > Note: `conda` is also a good candidate for hassle-free
-installation of PyTorch: check out the [PyTorch website](https://pytorch.org/
-get-started/locally/) for more details.  To get started, we recommend checking
-out our [quickstart notebook](notebooks/1-quickstart.ipynb) or the
-[minimalistic example](#minimalistic-example) below. ## Usage Train model with
-default configuration (AM on TSP environment): ```bash python run.py ```
-Change experiment Train model with chosen experiment configuration from
-[configs/experiment/](configs/experiment/) (e.g. tsp/am, and environment with
-42 cities) ```bash python run.py experiment=tsp/am env.num_loc=42 ```   Disable
-logging ```bash python run.py experiment=test/am logger=none
-'~callbacks.learning_rate_monitor' ``` Note that `~` is used to disable a
-callback that would need a logger.   Create a sweep over hyperparameters (-
-m for multirun) ```bash python run.py -m experiment=tsp/am
+configuring complex applications ![RL4CO Overview](https://github.com/kaist-
+silab/rl4co/assets/34462374/4d9a670f-ab7c-4fc8-9135-82d17cb6d0ee) ## Getting
+started [Open_In_Colab] RL4CO is now available for installation on `pip`!
+```bash pip install rl4co ``` ### Local install and development If you want to
+develop RL4CO or access the latest builds, we recommend you to install it
+locally with `pip` in editable mode: ```bash git clone https://github.com/
+kaist-silab/rl4co && cd rl4co pip install -e . ```  [Optional] Automatically
+install PyTorch with correct CUDA version These commands will [automatically
+install](https://github.com/pmeier/light-the-torch) PyTorch with the right GPU
+version for your system: ```bash pip install light-the-torch python3 -
+m light_the_torch install -r --upgrade torch ``` > Note: `conda` is also a good
+candidate for hassle-free installation of PyTorch: check out the [PyTorch
+website](https://pytorch.org/get-started/locally/) for more details.  To get
+started, we recommend checking out our [quickstart notebook](notebooks/1-
+quickstart.ipynb) or the [minimalistic example](#minimalistic-example) below.
+## Usage Train model with default configuration (AM on TSP environment):
+```bash python run.py ```  Change experiment Train model with chosen experiment
+configuration from [configs/experiment/](configs/experiment/) (e.g. tsp/am, and
+environment with 42 cities) ```bash python run.py experiment=tsp/am
+env.num_loc=42 ```   Disable logging ```bash python run.py experiment=test/am
+logger=none '~callbacks.learning_rate_monitor' ``` Note that `~` is used to
+disable a callback that would need a logger.   Create a sweep over
+hyperparameters (-m for multirun) ```bash python run.py -m experiment=tsp/am
 train.optimizer.lr=1e-3,1e-4,1e-5 ```  ### Minimalistic Example Here is a
 minimalistic example training the Attention Model with greedy rollout baseline
-on TSP in less than 50 lines of code: ```python from omegaconf import
-DictConfig import lightning as L from rl4co.envs import TSPEnv from
-rl4co.models.zoo.am import AttentionModel from rl4co.tasks.rl4co import
-RL4COLitModule config = DictConfig( {"data": { "train_size": 100000,
-"val_size": 10000, "batch_size": 512, }, "optimizer": {"lr": 1e-4}} ) #
+on TSP in less than 30 lines of code: ```python from rl4co.envs import TSPEnv
+from rl4co.models import AttentionModel from rl4co.utils import RL4COTrainer #
 Environment, Model, and Lightning Module env = TSPEnv(num_loc=20) model =
-AttentionModel(env) lit_module = RL4COLitModule(config, env, model) # Trainer
-trainer = L.Trainer( max_epochs=3, # only few epochs accelerator="gpu", # use
-GPU if available, else you can use others as "cpu" logger=None, # can replace
-with WandbLogger, TensorBoardLogger, etc. precision="16-mixed", # Lightning
-will handle faster training with mixed precision gradient_clip_val=1.0, # clip
-gradients to avoid exploding gradients reload_dataloaders_every_n_epochs=1, #
-necessary for sampling new data ) # Fit the model trainer.fit(lit_module) ```
-### Testing Run tests with `pytest` from the root directory: ```bash pytest
-tests ``` ## Contributing [![Slack](https://img.shields.io/badge/slack-chat-
-611f69.svg?logo=slack)](https://join.slack.com/t/rl4co/shared_invite/zt-
-1ytz2c1v4-0IkQ8NQH4TRXIX8PrRmDhQ) Have a suggestion, request, or found a bug?
-Feel free to [open an issue](https://github.com/kaist-silab/rl4co/issues) or
-[submit a pull request](https://github.com/kaist-silab/rl4co/pulls). If you
-would like to contribute, please check out our contribution guidelines [here]
-(.github/CONTRIBUTING.md). We welcome and look forward to all contributions to
-RL4CO! We are also on [Slack](https://join.slack.com/t/rl4co/shared_invite/zt-
-1ytz2c1v4-0IkQ8NQH4TRXIX8PrRmDhQ) if you have any questions or would like to
-discuss RL4CO with us. We are open to collaborations and would love to hear
-from you ð ### Contributors [https://contrib.rocks/image?repo=kaist-silab/
-rl4co] ## Cite us If you find RL4CO valuable for your research or applied
-projects: ```bibtex @article{berto2023rl4co, title = {{RL4CO}: an Extensive
-Reinforcement Learning for Combinatorial Optimization Benchmark}, author=
-{Federico Berto and Chuanbo Hua and Junyoung Park and Minsu Kim and Hyeonah Kim
-and Jiwoo Son and Haeyeon Kim and Joungho Kim and Jinkyoo Park}, journal={arXiv
-preprint arXiv:2306.17100}, year={2023}, url = {https://github.com/kaist-silab/
-rl4co} } ```
+AttentionModel(env, baseline="rollout", train_data_size=100_000,
+test_data_size=10_000, optimizer_kwargs={'lr': 1e-4} ) # Trainer trainer =
+RL4COTrainer(max_epochs=3) # Fit the model trainer.fit(model) # Test the model
+trainer.test(model) ``` ### Testing Run tests with `pytest` from the root
+directory: ```bash pytest tests ``` ## Contributing [![Slack](https://
+img.shields.io/badge/slack-chat-611f69.svg?logo=slack)](https://join.slack.com/
+t/rl4co/shared_invite/zt-1ytz2c1v4-0IkQ8NQH4TRXIX8PrRmDhQ) Have a suggestion,
+request, or found a bug? Feel free to [open an issue](https://github.com/kaist-
+silab/rl4co/issues) or [submit a pull request](https://github.com/kaist-silab/
+rl4co/pulls). If you would like to contribute, please check out our
+contribution guidelines [here](.github/CONTRIBUTING.md). We welcome and look
+forward to all contributions to RL4CO! We are also on [Slack](https://
+join.slack.com/t/rl4co/shared_invite/zt-1ytz2c1v4-0IkQ8NQH4TRXIX8PrRmDhQ) if
+you have any questions or would like to discuss RL4CO with us. We are open to
+collaborations and would love to hear from you ð ### Contributors [https://
+contrib.rocks/image?repo=kaist-silab/rl4co] ## Cite us If you find RL4CO
+valuable for your research or applied projects: ```bibtex @article
+{berto2023rl4co, title = {{RL4CO}: an Extensive Reinforcement Learning for
+Combinatorial Optimization Benchmark}, author={Federico Berto and Chuanbo Hua
+and Junyoung Park and Minsu Kim and Hyeonah Kim and Jiwoo Son and Haeyeon Kim
+and Joungho Kim and Jinkyoo Park}, journal={arXiv preprint arXiv:2306.17100},
+year={2023}, url = {https://github.com/kaist-silab/rl4co} } ```
```

### Comparing `rl4co-0.0.6/pyproject.toml` & `rl4co-0.1.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -33,33 +33,30 @@
     "Programming Language :: Python"
 ]
 
 dependencies = [
     "torch>=2.0.0",
     "torchrl>=0.1.1",
     "tensordict>=0.1.1",
-    "lightning>=2.0.0",
+    "lightning>=2.0.5",
     "hydra-core",
     "hydra-colorlog",
     "omegaconf",
     "pyrootutils",
     "rich",
-    "numpy",
     "einops",
     "wandb",
-    "pre-commit>=3.3.3",
     "matplotlib",
     "scipy",
-    "pydantic<2.0.0" # Temporary bugfix https://github.com/Lightning-AI/lightning/pull/18022
 ]
 
 [project.optional-dependencies]
 graph = ["torch_geometric"]
-testing = ["pytest"]
-linting = ["black", "ruff"]
+testing = ["pytest", "pytest-cov"]
+dev = ["black", "ruff", "pre-commit>=3.3.3"]
 
 [project.urls]
 "Homepage" = "https://github.com/kaist-silab/rl4co"
 "Bug Tracker" = "https://github.com/kaist-silab/rl4co/issues"
 
 # Ruff + Black + isort combo for code formatting
 # Adapted from https://github.com/AntonOsika/gpt-engineer (kudos!)
@@ -124,7 +121,17 @@
     | build
     | dist
     | venv
   )/
 )
 '''
 
+[tool.coverage]
+include = ["rl4co.*"]
+
+[tool.coverage.report]
+show_missing = true
+exclude_lines = [
+    # Lines to exclude from coverage report (e.g., comments, debug statements)
+    "pragma: no cover",
+    "if __name__ == .__main__.:",
+]
```

### Comparing `rl4co-0.0.6/rl4co/data/dataset.py` & `rl4co-0.1.0/rl4co/data/dataset.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.6/rl4co/data/generate_data.py` & `rl4co-0.1.0/rl4co/data/generate_data.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.6/rl4co/data/utils.py` & `rl4co-0.1.0/rl4co/data/utils.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.6/rl4co/envs/atsp.py` & `rl4co-0.1.0/rl4co/envs/atsp.py`

 * *Files 7% similar despite different names*

```diff
@@ -187,30 +187,35 @@
                 dms, _ = (
                     dms[..., :, None, :] + dms[..., None, :, :].transpose(-2, -1)
                 ).min(dim=-1)
                 if (dms == old_dms).all():
                     break
         return TensorDict({"cost_matrix": dms}, batch_size=batch_size)
 
-    def render(self, td):
+    @staticmethod
+    def render(td, actions=None, ax=None):
         try:
             import networkx as nx
         except ImportError:
             log.warn(
                 "Networkx is not installed. Please install it with `pip install networkx`"
             )
             return
 
         td = td.detach().cpu()
+        if actions is None:
+            actions = td.get("action", None)
+
         # if batch_size greater than 0 , we need to select the first batch element
         if td.batch_size != torch.Size([]):
             td = td[0]
+            actions = actions[0]
 
-        src_nodes = td["action"]
-        tgt_nodes = torch.roll(td["action"], 1, dims=0)
+        src_nodes = actions
+        tgt_nodes = torch.roll(actions, 1, dims=0)
 
         # Plot with networkx
         G = nx.DiGraph(td["cost_matrix"].numpy())
         pos = nx.spring_layout(G)
         nx.draw(
             G,
             pos,
```

### Comparing `rl4co-0.0.6/rl4co/envs/common/base.py` & `rl4co-0.1.0/rl4co/envs/common/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,21 +13,21 @@
 log = get_pylogger(__name__)
 
 
 class RL4COEnvBase(EnvBase):
     """Base class for RL4CO environments based on TorchRL EnvBase
 
     Args:
-        data_dir (str): Root directory for the dataset
-        train_file (str): Name of the training file
-        val_file (str): Name of the validation file
-        test_file (str): Name of the test file
-        check_solution (bool): Whether to check the validity of the solution at the end of the episode
-        seed (int): Seed for the environment
-        device (str): Device to use. Generally, no need to set as tensors are updated on the fly
+        data_dir: Root directory for the dataset
+        train_file: Name of the training file
+        val_file: Name of the validation file
+        test_file: Name of the test file
+        check_solution: Whether to check the validity of the solution at the end of the episode
+        seed: Seed for the environment
+        device: Device to use. Generally, no need to set as tensors are updated on the fly
     """
 
     batch_locked = False
 
     def __init__(
         self,
         *,
@@ -99,18 +99,20 @@
                 log.warning(
                     "Loading training dataset from file. This may not be desired in RL since "
                     "the dataset is fixed and the agent will not be able to explore new states"
                 )
             try:
                 td = self.load_data(f, batch_size)
             except FileNotFoundError:
-                raise Exception(
+                log.error(
                     f"Provided file name {f} not found. Make sure to provide a file in the right path first or "
                     f"unset {phase}_file to generate data automatically instead"
                 )
+                td = self.generate_data(batch_size)
+
         return TensorDictDataset(td)
 
     def generate_data(self, batch_size):
         """Dataset generation"""
         raise NotImplementedError
 
     def transform(self):
```

### Comparing `rl4co-0.0.6/rl4co/envs/common/utils.py` & `rl4co-0.1.0/rl4co/envs/common/utils.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.6/rl4co/envs/cvrp.py` & `rl4co-0.1.0/rl4co/envs/cvrp.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,22 +41,22 @@
     """Capacitated Vehicle Routing Problem (CVRP) environment.
     At each step, the agent chooses a customer to visit depending on the current location and the remaining capacity.
     When the agent visits a customer, the remaining capacity is updated. If the remaining capacity is not enough to
     visit any customer, the agent must go back to the depot. The reward is the -infinite unless the agent visits all the cities.
     In that case, the reward is (-)length of the path: maximizing the reward is equivalent to minimizing the path length.
 
     Args:
-        num_loc (int): number of locations (cities) in the VRP, without the depot. (e.g. 10 means 10 locs + 1 depot)
-        min_loc (float): minimum value for the location coordinates
-        max_loc (float): maximum value for the location coordinates
-        min_demand (float): minimum value for the demand of each customer
-        max_demand (float): maximum value for the demand of each customer
-        vehicle_capacity (float): capacity of the vehicle
-        capacity (float): capacity of the vehicle
-        td_params (TensorDict): parameters of the environment
+        num_loc: number of locations (cities) in the VRP, without the depot. (e.g. 10 means 10 locs + 1 depot)
+        min_loc: minimum value for the location coordinates
+        max_loc: maximum value for the location coordinates
+        min_demand: minimum value for the demand of each customer
+        max_demand: maximum value for the demand of each customer
+        vehicle_capacity: capacity of the vehicle
+        capacity: capacity of the vehicle
+        td_params: parameters of the environment
     """
 
     name = "cvrp"
 
     def __init__(
         self,
         num_loc: int = 20,
@@ -310,25 +310,27 @@
         out = base.from_list(cmap_name, color_list, num_routine)
 
         if ax is None:
             # Create a plot of the nodes
             _, ax = plt.subplots()
 
         td = td.detach().cpu()
+
+        if actions is None:
+            actions = td.get("action", None)
+
         # if batch_size greater than 0 , we need to select the first batch element
         if td.batch_size != torch.Size([]):
             td = td[0]
+            actions = actions[0]
 
         locs = td["locs"]
         scale = CAPACITIES.get(td["locs"].size(-2) - 1, 1)
         demands = td["demand"] * scale
 
-        if actions is None:
-            actions = td.get("action", None)
-
         # add the depot at the first action and the end action
         actions = torch.cat([torch.tensor([0]), actions, torch.tensor([0])])
 
         # gather locs in order of action if available
         if actions is None:
             log.warning("No action in TensorDict, rendering unsorted locs")
         else:
```

### Comparing `rl4co-0.0.6/rl4co/envs/dpp.py` & `rl4co-0.1.0/rl4co/envs/dpp.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,17 +19,33 @@
 from rl4co.utils.download.downloader import download_url
 from rl4co.utils.pylogger import get_pylogger
 
 log = get_pylogger(__name__)
 
 
 class DPPEnv(RL4COEnvBase):
-    """Decap placement problem as done in DevFormer paper
+    """Decap placement problem as done in DevFormer paper: https://arxiv.org/abs/2205.13225
 
-    https://arxiv.org/abs/2205.13225
+    The environment is a 10x10 grid with 100 locations containing either a probing port or a keepout region.
+    The goal is to place decaps (decoupling capacitors) to maximize the impedance suppression at the probing port.
+    Decaps cannot be placed in keepout regions or at the probing port and the number of decaps is limited.
+
+    Args:
+        min_loc: Minimum location value. Defaults to 0.
+        max_loc: Maximum location value. Defaults to 1.
+        num_keepout_min: Minimum number of keepout regions. Defaults to 1.
+        num_keepout_max: Maximum number of keepout regions. Defaults to 50.
+        max_decaps: Maximum number of decaps. Defaults to 20.
+        data_dir: Directory to store data. Defaults to "data/dpp/".
+            This can be downloaded from this [url](https://drive.google.com/uc?id=1IEuR2v8Le-mtHWHxwTAbTOPIkkQszI95).
+        chip_file: Name of the chip file. Defaults to "10x10_pkg_chip.npy".
+        decap_file: Name of the decap file. Defaults to "01nF_decap.npy".
+        freq_file: Name of the frequency file. Defaults to "freq_201.npy".
+        url: URL to download data from. Defaults to None.
+        td_params: TensorDict parameters. Defaults to None.
     """
 
     name = "dpp"
 
     def __init__(
         self,
         *,
```

### Comparing `rl4co-0.0.6/rl4co/envs/ffsp.py` & `rl4co-0.1.0/rl4co/envs/ffsp.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,16 +10,24 @@
     UnboundedDiscreteTensorSpec,
 )
 
 from rl4co.envs.common.base import RL4COEnvBase
 
 
 class FFSPEnv(RL4COEnvBase):
-    """Flexible Flow Shop Problem (FFSP) Environment
+    """Flexible Flow Shop Problem (FFSP) environment.
+    The goal is to schedule a set of jobs on a set of machines such that the makespan is minimized.
+
     Args:
+        num_stage: number of stages
+        num_machine: number of machines in each stage
+        num_job: number of jobs
+        min_time: minimum processing time of a job
+        max_time: maximum processing time of a job
+        batch_size: batch size of the problem
 
     Note:
         - [IMPORTANT] This version of ffsp requires the number of machines in each stage to be the same
     """
 
     name = "ffsp"
```

### Comparing `rl4co-0.0.6/rl4co/envs/mdpp.py` & `rl4co-0.1.0/rl4co/envs/mdpp.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,20 @@
 class MDPPEnv(DPPEnv):
     """Multiple decap placement problem (mDPP) environment
     This is a modified version of the DPP environment where we allow multiple probing ports
     The reward can be calculated as:
         - minmax: min of the max of the decap scores
         - meansum: mean of the sum of the decap scores
     The minmax is more challenging as it requires to find the best decap location for the worst case
+
+    Args:
+        num_probes_min: minimum number of probes
+        num_probes_max: maximum number of probes
+        reward_type: reward type, either minmax or meansum
+        td_params: TensorDict parameters
     """
 
     name = "mdpp"
 
     def __init__(
         self,
         *,
@@ -325,12 +331,12 @@
                 plt.Rectangle(
                     (0, 0), 1, 1, color=c, edgecolor="k", linestyle="-", linewidth=1
                 )
                 for c in colors
             ]
             ax.legend(
                 handles,
-                [l for l in labels],
+                [label for label in labels],
                 ncol=len(colors),
                 loc="upper center",
                 bbox_to_anchor=(0.5, 1.1),
             )
```

### Comparing `rl4co-0.0.6/rl4co/envs/mtsp.py` & `rl4co-0.1.0/rl4co/envs/mtsp.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,24 +9,33 @@
     CompositeSpec,
     UnboundedContinuousTensorSpec,
     UnboundedDiscreteTensorSpec,
 )
 
 from rl4co.envs.common.base import RL4COEnvBase
 from rl4co.envs.common.utils import batch_to_scalar
-from rl4co.utils.ops import get_distance, gather_by_index, get_tour_length
+from rl4co.utils.ops import gather_by_index, get_distance, get_tour_length
 
 
 class MTSPEnv(RL4COEnvBase):
     """Multiple Traveling Salesman Problem environment
     At each step, an agent chooses to visit a city. A maximum of `num_agents` agents can be employed to visit the cities.
     The cost can be defined in two ways:
         - `minmax`: (default) the reward is the maximum of the path lengths of all the agents
         - `sum`: the cost is the sum of the path lengths of all the agents
     Reward is - cost, so the goal is to maximize the reward (minimize the cost).
+
+    Args:
+        num_loc: number of locations (cities) to visit
+        min_loc: minimum value of the locations
+        max_loc: maximum value of the locations
+        min_num_agents: minimum number of agents
+        max_num_agents: maximum number of agents
+        cost_type: type of cost to use, either `minmax` or `sum`
+        td_params: parameters for the TensorDict specs
     """
 
     name = "mtsp"
 
     def __init__(
         self,
         num_loc: int = 20,
@@ -258,34 +267,35 @@
                 "locs": locs,
                 "num_agents": num_agents,
             },
             batch_size=batch_size,
         )
 
     @staticmethod
-    def render(td):
+    def render(td, actions=None, ax=None):
         import matplotlib.pyplot as plt
 
         from matplotlib import colormaps
 
         def discrete_cmap(num, base_cmap="nipy_spectral"):
             """Create an N-bin discrete colormap from the specified input map"""
             base = colormaps[base_cmap]
             color_list = base(np.linspace(0, 1, num))
             cmap_name = base.name + str(num)
             return base.from_list(cmap_name, color_list, num)
 
-        td = td.detach().cpu()
+        if actions is None:
+            actions = td.get("action", None)
         # if batch_size greater than 0 , we need to select the first batch element
         if td.batch_size != torch.Size([]):
             td = td[0]
+            actions = actions[0]
 
         num_agents = td["num_agents"]
         locs = td["locs"]
-        actions = td["action"]
         cmap = discrete_cmap(num_agents, "rainbow")
 
         fig, ax = plt.subplots()
 
         # Add depot action = 0 to before first action and after last action
         actions = torch.cat(
             [
```

### Comparing `rl4co-0.0.6/rl4co/envs/op.py` & `rl4co-0.1.0/rl4co/envs/op.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.6/rl4co/envs/pctsp.py` & `rl4co-0.1.0/rl4co/envs/pctsp.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,26 +24,26 @@
 # The expected total (uniform) penalty of half of the nodes (since approx half will be visited by the constraint)
 # is (n / 2) / 2 = n / 4 so divide by this means multiply by 4 / n,
 # However instead of 4 we use penalty_factor (3 works well) so we can make them larger or smaller
 MAX_LENGTHS = {20: 2.0, 50: 3.0, 100: 4.0}
 
 
 class PCTSPEnv(RL4COEnvBase):
-    """Prize-collecting TSP environment
-    The goal is to collect as much prize as possible while minimizing the total travel cost
-    The environment is stochastic, the prize is only revealed when the node is visited
+    """Prize-collecting TSP (PCTSP) environment.
+    The goal is to collect as much prize as possible while minimizing the total travel cost.
+    The environment is stochastic, the prize is only revealed when the node is visited.
 
     Args:
-        num_loc (int): Number of locations
-        min_loc (float): Minimum location value
-        max_loc (float): Maximum location value
-        penalty_factor (float): Penalty factor
-        prize_required (float): Minimum prize required to visit a node
-        check_solution (bool): Set to False by default for small bug happening around 0.01% of the time (TODO: fix)
-        td_params (TensorDict): Parameters of the environment
+        num_loc: Number of locations
+        min_loc: Minimum location value
+        max_loc: Maximum location value
+        penalty_factor: Penalty factor
+        prize_required: Minimum prize required to visit a node
+        check_solution: Set to False by default for small bug happening around 0.01% of the time (TODO: fix)
+        td_params: Parameters of the environment
     """
 
     name = "pctsp"
     _stochastic = False
 
     def __init__(
         self,
```

### Comparing `rl4co-0.0.6/rl4co/envs/pdp.py` & `rl4co-0.1.0/rl4co/envs/pdp.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,19 +11,19 @@
 )
 
 from rl4co.envs.common.base import RL4COEnvBase
 from rl4co.utils.ops import gather_by_index, get_tour_length
 
 
 class PDPEnv(RL4COEnvBase):
-    """Pickup and Delivery Problem (PDP) environment
+    """Pickup and Delivery Problem (PDP) environment.
     The environment is made of num_loc + 1 locations (cities):
-    - 1 depot
-    - num_loc / 2 pickup locations
-    - num_loc / 2 delivery locations
+        - 1 depot
+        - `num_loc` / 2 pickup locations
+        - `num_loc` / 2 delivery locations
     The goal is to visit all the pickup and delivery locations in the shortest path possible starting from the depot
     The conditions is that the agent must visit a pickup location before visiting its corresponding delivery location
 
     Args:
         num_loc: number of locations (cities) in the TSP
         td_params: parameters of the environment
         seed: seed for the environment
@@ -217,15 +217,15 @@
                 "locs": locs_with_depot[..., 1:, :],
                 "depot": locs_with_depot[..., 0, :],
             },
             batch_size=batch_size,
         )
 
     @staticmethod
-    def render(td, actions=None):
+    def render(td: TensorDict, actions=None, ax=None):
         import matplotlib.pyplot as plt
 
         markersize = 8
 
         td = td.detach().cpu()
         # if batch_size greater than 0 , we need to select the first batch element
         if td.batch_size != torch.Size([]):
@@ -287,18 +287,11 @@
                 delivery_loc[1],
                 "b",
                 marker="v",
                 markersize=markersize,
                 label="Delivery" if i == 0 else None,
             )
 
-        # Legend
-        # plt.legend(['Actions', 'Depot', 'Delivery', 'Pickup'])
-        # get handles
-        handles, labels = ax.get_legend_handles_labels()
-
-        # plot legend
-        ax.legend(handles, labels)
-        ax.set_title("Pickup and Delivery Problem Solution")
-        ax.set_xlabel("x-coordinate")
-        ax.set_ylabel("y-coordinate")
+        # Setup limits and show
+        ax.set_xlim(-0.05, 1.05)
+        ax.set_ylim(-0.05, 1.05)
         plt.show()
```

### Comparing `rl4co-0.0.6/rl4co/envs/sdvrp.py` & `rl4co-0.1.0/rl4co/envs/sdvrp.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,22 +22,22 @@
     SDVRP is a generalization of CVRP, where nodes can be visited multiple times and a fraction of the demand can be met.
     At each step, the agent chooses a customer to visit depending on the current location and the remaining capacity.
     When the agent visits a customer, the remaining capacity is updated. If the remaining capacity is not enough to
     visit any customer, the agent must go back to the depot. The reward is the -infinite unless the agent visits all the cities.
     In that case, the reward is (-)length of the path: maximizing the reward is equivalent to minimizing the path length.
 
     Args:
-        num_loc (int): number of locations (cities) in the VRP, without the depot. (e.g. 10 means 10 locs + 1 depot)
-        min_loc (float): minimum value for the location coordinates
-        max_loc (float): maximum value for the location coordinates
-        min_demand (float): minimum value for the demand of each customer
-        max_demand (float): maximum value for the demand of each customer
-        vehicle_capacity (float): capacity of the vehicle
-        capacity (float): capacity of the vehicle
-        td_params (TensorDict): parameters of the environment
+        num_loc: number of locations (cities) in the VRP, without the depot. (e.g. 10 means 10 locs + 1 depot)
+        min_loc: minimum value for the location coordinates
+        max_loc: maximum value for the location coordinates
+        min_demand: minimum value for the demand of each customer
+        max_demand: maximum value for the demand of each customer
+        vehicle_capacity: capacity of the vehicle
+        capacity: capacity of the vehicle
+        td_params: parameters of the environment
     """
 
     name = "sdvrp"
 
     def __init__(
         self,
         num_loc: int = 20,
```

### Comparing `rl4co-0.0.6/rl4co/envs/spctsp.py` & `rl4co-0.1.0/rl4co/envs/spctsp.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,14 +1,21 @@
 from rl4co.envs.pctsp import PCTSPEnv
 from rl4co.utils.pylogger import get_pylogger
 
 log = get_pylogger(__name__)
 
 
 class SPCTSPEnv(PCTSPEnv):
+    """Stochastic Prize Collecting Traveling Salesman Problem (SPCTSP) environment.
+
+    Note:
+        The only difference with deterministic PCTSP is that the prizes are stochastic
+        (i.e. the expected prize is not the same as the real prize).
+    """
+
     name = "spctsp"
     _stochastic = True
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
 
     @property
```

### Comparing `rl4co-0.0.6/rl4co/envs/tsp.py` & `rl4co-0.1.0/rl4co/envs/tsp.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,14 +83,15 @@
         # Initialize locations
         init_locs = td["locs"] if td is not None else None
         if batch_size is None:
             batch_size = self.batch_size if init_locs is None else init_locs.shape[:-2]
         self.device = device = init_locs.device if init_locs is not None else self.device
         if init_locs is None:
             init_locs = self.generate_data(batch_size=batch_size).to(device)["locs"]
+        batch_size = [batch_size] if isinstance(batch_size, int) else batch_size
 
         # We do not enforce loading from self for flexibility
         num_loc = init_locs.shape[-2]
 
         # Other variables
         current_node = torch.zeros((batch_size), dtype=torch.int64, device=device)
         available = torch.ones(
@@ -175,23 +176,24 @@
         import numpy as np
 
         if ax is None:
             # Create a plot of the nodes
             _, ax = plt.subplots()
 
         td = td.detach().cpu()
+
+        if actions is None:
+            actions = td.get("action", None)
         # if batch_size greater than 0 , we need to select the first batch element
         if td.batch_size != torch.Size([]):
             td = td[0]
+            actions = actions[0]
 
         locs = td["locs"]
 
-        if actions is None:
-            actions = td.get("action", None)
-
         # gather locs in order of action if available
         if actions is None:
             log.warning("No action in TensorDict, rendering unsorted locs")
         else:
             locs = gather_by_index(locs, actions, dim=0)
 
         # Cat the first node to the end to complete the tour
```

### Comparing `rl4co-0.0.6/rl4co/models/nn/attention.py` & `rl4co-0.1.0/rl4co/models/nn/attention.py`

 * *Files 20% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     )
 
     def scaled_dot_product_attention(
         Q, K, V, attn_mask=None, dropout_p=0.0, is_causal=False, scale=None
     ):
         """Simple Scaled Dot-Product Attention in PyTorch without Flash Attention"""
         if scale is None:
-            scale = Q.size(-1) ** -0.5  # scale factor
+            scale = math.sqrt(Q.size(-1))  # scale factor
         # compute the attention scores
         attn_scores = torch.matmul(Q, K.transpose(-2, -1)) / scale
         # apply causal masking if required
         if is_causal:
             mask = torch.triu(torch.ones_like(attn_scores), diagonal=1)
             attn_scores = attn_scores.masked_fill(mask == 0, float("-inf"))
         # apply attention mask if provided
@@ -49,27 +49,43 @@
         args = [arg.half() for arg in args if isinstance(arg, torch.Tensor)]
         out = func(*args, **kwargs)
         return out.to(original_dtype)
     else:
         return func(*args, **kwargs)
 
 
-class NativeFlashMHA(nn.Module):
-    """PyTorch native implementation of Flash Multi-Head Attention with automatic mixed precision support."""
+class MultiHeadAttention(nn.Module):
+    """PyTorch native implementation of Flash Multi-Head Attention with automatic mixed precision support.
+    Uses PyTorch's native `scaled_dot_product_attention` implementation, available from 2.0
+
+    Note:
+        If `scaled_dot_product_attention` is not available, use custom implementation of `scaled_dot_product_attention` without Flash Attention.
+        In case you want to use Flash Attention, you may have a look at the MHA module under `rl4co.models.nn.flash_attention.MHA`.
+
+    Args:
+        embed_dim: total dimension of the model
+        num_heads: number of heads
+        bias: whether to use bias
+        attention_dropout: dropout rate for attention weights
+        causal: whether to apply causal mask to attention scores
+        device: torch device
+        dtype: torch dtype
+        force_flash_attn: whether to force flash attention. If True, then we automatically cast to fp16
+    """
 
     def __init__(
         self,
-        embed_dim,
-        num_heads,
-        bias=True,
-        attention_dropout=0.0,
-        causal=False,
+        embed_dim: int,
+        num_heads: int,
+        bias: bool = True,
+        attention_dropout: float = 0.0,
+        causal: bool = False,
         device=None,
         dtype=None,
-        force_flash_attn=False,
+        force_flash_attn: bool = False,
     ) -> None:
         factory_kwargs = {"device": device, "dtype": dtype}
         super().__init__()
         self.embed_dim = embed_dim
         self.causal = causal
         self.force_flash_attn = force_flash_attn
         self.attention_dropout = attention_dropout
@@ -103,115 +119,46 @@
             dropout_p=self.attention_dropout,
         )
         return self.out_proj(rearrange(out, "b h s d -> b s (h d)"))
 
     flash_attn_wrapper = flash_attn_wrapper
 
 
-class MultiHeadAttention(nn.Module):
-    """Multi-Head Attention module following Kool et al. (2019)"""
-
-    def __init__(self, embed_dim, num_heads, **kwargs):
-        super(MultiHeadAttention, self).__init__()
-
-        self.num_heads = num_heads
-        self.embed_dim = embed_dim
-        self.hdim = embed_dim // num_heads
-
-        self.norm_factor = 1 / math.sqrt(self.hdim)  # See Attention is all you need
-
-        self.Wq = nn.Parameter(torch.Tensor(num_heads, embed_dim, self.hdim))
-        self.Wk = nn.Parameter(torch.Tensor(num_heads, embed_dim, self.hdim))
-        self.Wv = nn.Parameter(torch.Tensor(num_heads, embed_dim, self.hdim))
-
-        self.Wout = nn.Parameter(torch.Tensor(num_heads, self.hdim, embed_dim))
-
-        self.init_parameters()
-
-    def init_parameters(self):
-        for param in self.parameters():
-            stdv = 1.0 / math.sqrt(param.size(-1))
-            param.data.uniform_(-stdv, stdv)
-
-    def forward(self, q, h=None, mask=None):
-        """q: queries (batch_size, n_query, input_dim)
-        h: data (batch_size, graph_size, input_dim)
-        mask: mask (batch_size, n_query, graph_size) or viewable as that (i.e. can be 2 dim if n_query == 1)
-        Mask should contain 1 if attention is not possible (i.e. mask is negative adjacency)
-        """
-
-        if h is None:
-            h = q  # compute self-attention
-
-        batch_size, graph_size, input_dim = h.size()
-        n_query = q.size(1)
-        assert q.size(0) == batch_size
-        assert q.size(2) == input_dim
-
-        hflat = h.contiguous().view(-1, input_dim)
-        qflat = q.contiguous().view(-1, input_dim)
-
-        # Last dimension can be different for keys and values
-        shp = (self.num_heads, batch_size, graph_size, -1)
-        shp_q = (self.num_heads, batch_size, n_query, -1)
-
-        # Calculate queries, (num_heads, n_query, graph_size, key/val_size)
-        Q = torch.matmul(qflat, self.Wq).view(shp_q)
-        # Calculate keys and values (num_heads, batch_size, graph_size, key/val_size)
-        K = torch.matmul(hflat, self.Wk).view(shp)
-        V = torch.matmul(hflat, self.Wv).view(shp)
-
-        # Calculate compatibility (num_heads, batch_size, n_query, graph_size)
-        compatibility = self.norm_factor * torch.matmul(Q, K.transpose(2, 3))
-
-        # Optionally apply mask to prevent attention
-        if mask is not None:
-            mask = mask.view(1, batch_size, n_query, graph_size).expand_as(compatibility)
-            compatibility[mask] = float("-inf")  # -np.inf
-
-        attn = torch.softmax(compatibility, dim=-1)
-
-        # If there are nodes with no neighbours then softmax returns nan so we fix them to 0
-        if mask is not None:
-            attnc = attn.clone()
-            attnc[mask] = 0
-            attn = attnc
-
-        heads = torch.matmul(attn, V)
-
-        out = torch.mm(
-            heads.permute(1, 2, 0, 3).contiguous().view(-1, self.num_heads * self.hdim),
-            self.Wout.view(-1, self.embed_dim),
-        ).view(batch_size, n_query, self.embed_dim)
-
-        return out
-
-
 class LogitAttention(nn.Module):
     """Calculate logits given query, key and value and logit key
     If we use Flash Attention, then we automatically move to fp16 for inner computations
     Note: with Flash Attention, masking is not supported
 
     Perform the following:
         1. Apply cross attention to get the heads
         2. Project heads to get glimpse
         3. Compute attention score between glimpse and logit key
         4. Normalize and mask
+
+    Args:
+        embed_dim: total dimension of the model
+        num_heads: number of heads
+        tanh_clipping: tanh clipping value
+        mask_inner: whether to mask inner attention
+        mask_logits: whether to mask logits
+        normalize: whether to normalize logits
+        softmax_temp: softmax temperature
+        force_flash_attn: whether to force flash attention. If True, then we automatically cast to fp16
     """
 
     def __init__(
         self,
-        embed_dim,
-        num_heads,
-        tanh_clipping=10.0,
-        mask_inner=True,
-        mask_logits=True,
-        normalize=True,
-        softmax_temp=1.0,
-        force_flash_attn=False,
+        embed_dim: int,
+        num_heads: int,
+        tanh_clipping: float = 10.0,
+        mask_inner: bool = True,
+        mask_logits: bool = True,
+        normalize: bool = True,
+        softmax_temp: float = 1.0,
+        force_flash_attn: bool = False,
     ):
         super(LogitAttention, self).__init__()
         self.num_heads = num_heads
         self.mask_logits = mask_logits
         self.mask_inner = mask_inner
         self.tanh_clipping = tanh_clipping
         self.normalize = normalize
```

### Comparing `rl4co-0.0.6/rl4co/models/nn/env_embeddings/context.py` & `rl4co-0.1.0/rl4co/models/nn/env_embeddings/context.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.6/rl4co/models/nn/env_embeddings/dynamic.py` & `rl4co-0.1.0/rl4co/models/nn/env_embeddings/dynamic.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.6/rl4co/models/nn/env_embeddings/init.py` & `rl4co-0.1.0/rl4co/models/nn/env_embeddings/init.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.6/rl4co/models/nn/flash_attention.py` & `rl4co-0.1.0/rl4co/models/nn/flash_attention.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.6/rl4co/models/nn/graph/gat.py` & `rl4co-0.1.0/rl4co/models/rl/common/critic.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,89 +1,77 @@
-import torch.nn as nn
+from typing import Union
 
-from rl4co.models.nn.attention import MultiHeadAttention, NativeFlashMHA
-from rl4co.models.nn.env_embeddings import env_init_embedding
-from rl4co.models.nn.ops import Normalization, SkipConnection
-from rl4co.utils.pylogger import get_pylogger
-
-log = get_pylogger(__name__)
+from tensordict import TensorDict
+from torch import Tensor, nn
 
-
-class MultiHeadAttentionLayer(nn.Sequential):
-    def __init__(
-        self,
-        num_heads,
-        embed_dim,
-        feed_forward_hidden=512,
-        normalization="batch",
-        use_native_sdpa=False,
-        force_flash_attn=False,
-    ):
-        MHA = NativeFlashMHA if use_native_sdpa else MultiHeadAttention
-        super(MultiHeadAttentionLayer, self).__init__(
-            SkipConnection(MHA(embed_dim, num_heads, force_flash_attn=force_flash_attn)),
-            Normalization(embed_dim, normalization),
-            SkipConnection(
-                nn.Sequential(
-                    nn.Linear(embed_dim, feed_forward_hidden),
-                    nn.ReLU(),
-                    nn.Linear(feed_forward_hidden, embed_dim),
-                )
-                if feed_forward_hidden > 0
-                else nn.Linear(embed_dim, embed_dim)
-            ),
-            Normalization(embed_dim, normalization),
-        )
+from rl4co.models.nn.env_embeddings import env_init_embedding
+from rl4co.models.nn.graph.attnnet import GraphAttentionNetwork
 
 
-class GraphAttentionEncoder(nn.Module):
-    """Graph Attention Encoder with a series of MHA layers
-    Multi-Head Attention Layer with normalization and feed-forward layer
-    If use_native_sdpa is True, use NativeFlashMHA instead of MultiHeadAttention:
-    native PyTorch `scaled_dot_product_attention` implementation, available from 2.0
-    You may force FlashAttention by setting force_flash_attn to True (move to half precision)
+class CriticNetwork(nn.Module):
+    """We make the critic network compatible with any problem by using encoder for any environment
+    Refactored from Kool et al. (2019) which only worked for TSP. In our case, we make it
+    compatible with any problem by using the environment init embedding.
+
+    Args:
+        env_name: environment name to solve
+        encoder: Encoder to use for the critic
+        embedding_dim: Dimension of the embeddings
+        hidden_dim: Hidden dimension for the feed-forward network
+        num_layers: Number of layers for the encoder
+        num_heads: Number of heads for the attention
+        normalization: Normalization to use for the attention
+        force_flash_attn: Whether to force the use of flash attention. If True, cast to fp16
     """
 
     def __init__(
         self,
-        num_heads,
-        embedding_dim,
-        num_layers,
-        env=None,
-        normalization="batch",
-        feed_forward_hidden=512,
-        use_native_sdpa=False,
-        force_flash_attn=False,
-        disable_init_embedding=False,
+        env_name: str = None,
+        encoder: nn.Module = None,
+        embedding_dim: int = 128,
+        hidden_dim: int = 512,
+        num_layers: int = 3,
+        num_heads: int = 8,
+        normalization: str = "batch",
+        force_flash_attn: bool = False,
+        **unused_kwargs,
     ):
-        super(GraphAttentionEncoder, self).__init__()
+        super(CriticNetwork, self).__init__()
 
-        # To map input to embedding space
-        if not disable_init_embedding:
+        if env_name is None:
+            self.init_embedding = nn.Identity()
+        else:
             self.init_embedding = env_init_embedding(
-                env.name, {"embedding_dim": embedding_dim}
+                env_name, {"embedding_dim": embedding_dim}
             )
-        else:
-            log.warning("Disabling init embedding manually for GraphAttentionEncoder")
-            self.init_embedding = nn.Identity()  # do nothing
 
-        self.layers = nn.Sequential(
-            *(
-                MultiHeadAttentionLayer(
-                    num_heads,
-                    embedding_dim,
-                    feed_forward_hidden=feed_forward_hidden,
-                    normalization=normalization,
-                    use_native_sdpa=use_native_sdpa,
-                    force_flash_attn=force_flash_attn,
-                )
-                for _ in range(num_layers)
+        self.encoder = (
+            GraphAttentionNetwork(
+                num_heads=num_heads,
+                embedding_dim=embedding_dim,
+                num_layers=num_layers,
+                normalization=normalization,
+                feed_forward_hidden=hidden_dim,
+                force_flash_attn=force_flash_attn,
             )
+            if encoder is None
+            else encoder
         )
 
-    def forward(self, x, mask=None):
-        assert mask is None, "Mask not yet supported!"
-        # initial Embedding from features
-        init_embeds = self.init_embedding(x)
-        # layers  (batch_size, graph_size, embed_dim)
-        embeds = self.layers(init_embeds)
-        return embeds, init_embeds
+        self.value_head = nn.Sequential(
+            nn.Linear(embedding_dim, hidden_dim), nn.ReLU(), nn.Linear(hidden_dim, 1)
+        )
+
+    def forward(self, x: Union[Tensor, TensorDict]) -> Tensor:
+        """Forward pass of the critic network: encode the imput in embedding space and return the value
+
+        Args:
+            x: Input containing the environment state. Can be a Tensor or a TensorDict
+
+        Returns:
+            Value of the input state
+        """
+
+        # Initial embedding of x. This is the identity function if env_name is None.
+        x = self.init_embedding(x)
+        x = self.encoder(x)
+        return self.value_head(x).mean(1)
```

### Comparing `rl4co-0.0.6/rl4co/models/nn/graph/gcn.py` & `rl4co-0.1.0/rl4co/models/nn/graph/gcn.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,35 +1,39 @@
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 
 from torch_geometric.data import Batch, Data
 from torch_geometric.nn import GCNConv
 
-from rl4co.models.nn.env_embeddings import env_init_embedding
 from rl4co.utils.pylogger import get_pylogger
 
 log = get_pylogger(__name__)
 
 
 class GCNEncoder(nn.Module):
+    """Graph Convolutional Network to encode embeddings with a series of GCN layers
+
+    Args:
+        embedding_dim: dimension of the embeddings
+        num_nodes: number of nodes in the graph
+        num_gcn_layer: number of GCN layers
+        self_loop: whether to add self loop in the graph
+        residual: whether to use residual connection
+    """
+
     def __init__(
         self,
-        env,
-        embedding_dim,
-        num_nodes,
-        num_gcn_layer,
-        self_loop=False,
-        residual=True,
+        embedding_dim: int,
+        num_nodes: int,
+        num_gcn_layer: int,
+        self_loop: bool = False,
+        residual: bool = True,
     ):
         super(GCNEncoder, self).__init__()
-        # Define the init embedding
-        self.init_embedding = env_init_embedding(
-            env.name, {"embedding_dim": embedding_dim}
-        )
 
         # Generate edge index for a fully connected graph
         adj_matrix = torch.ones(num_nodes, num_nodes)
         if self_loop:
             adj_matrix.fill_diagonal_(0)  # No self-loops
         self.edge_index = torch.permute(torch.nonzero(adj_matrix), (1, 0))
 
@@ -38,18 +42,25 @@
             [GCNConv(embedding_dim, embedding_dim) for _ in range(num_gcn_layer)]
         )
 
         # Record parameters
         self.residual = residual
         self.self_loop = self_loop
 
-    def forward(self, x, mask=None):
+    def forward(self, x, node_feature, mask=None):
+        """Forward pass of the GCN encoder
+
+        Args:
+            x: [batch_size, graph_size, embed_dim] initial embeddings to process
+            node_feature: [batch_size, graph_size, embed_dim] node features, i.e. raw ones
+            mask: [batch_size, graph_size] mask for valid nodes
+        """
+
         assert mask is None, "Mask not yet supported!"
         # initial Embedding from features
-        node_feature = self.init_embedding(x)
 
         # Check to update the edge index with different number of node
         if node_feature.size(1) != self.edge_index.max().item() + 1:
             adj_matrix = torch.ones(x.size(1), x.size(1))
             if self.self_loop:
                 adj_matrix.fill_diagonal_(0)
             edge_index = torch.permute(torch.nonzero(adj_matrix), (1, 0))
```

### Comparing `rl4co-0.0.6/rl4co/models/nn/graph/mpnn.py` & `rl4co-0.1.0/rl4co/models/nn/graph/mpnn.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.6/rl4co/models/nn/mlp.py` & `rl4co-0.1.0/rl4co/models/nn/mlp.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.6/rl4co/models/nn/ops.py` & `rl4co-0.1.0/rl4co/models/nn/ops.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.6/rl4co/models/nn/utils.py` & `rl4co-0.1.0/rl4co/models/nn/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -60,8 +60,12 @@
     over envs when done with `env.rollout()`. We need this because for environements that complete at different steps.
     """
     actions = []
     while not td["done"].all():
         td = policy(td)
         actions.append(td["action"])
         td = env.step(td)["next"]
-    return env.get_reward(td, torch.stack(actions, dim=1))
+    return (
+        env.get_reward(td, torch.stack(actions, dim=1)),
+        td,
+        torch.stack(actions, dim=1),
+    )
```

### Comparing `rl4co-0.0.6/rl4co/models/rl/reinforce/baselines.py` & `rl4co-0.1.0/rl4co/models/rl/reinforce/baselines.py`

 * *Files 23% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 from scipy.stats import ttest_rel
 from torch.utils.data import DataLoader
 from tqdm.auto import tqdm
 
 from rl4co import utils
 from rl4co.data.dataset import ExtraKeyDataset, tensordict_collate_fn
+from rl4co.models.rl.common.critic import CriticNetwork
 
 log = utils.get_pylogger(__name__)
 
 
 class REINFORCEBaseline(nn.Module):
     """Base class for REINFORCE baselines"""
 
@@ -21,15 +22,15 @@
         super().__init__()
         pass
 
     def wrap_dataset(self, dataset, *args, **kw):
         """Wrap dataset with baseline-specific functionality"""
         return dataset
 
-    def eval(self, td, reward):
+    def eval(self, td, reward, env=None):
         """Evaluate baseline"""
         pass
 
     def epoch_callback(self, *args, **kw):
         """Callback at the end of each epoch
         For example, update baseline parameters and obtain baseline values
         """
@@ -39,46 +40,59 @@
         """To be called before training during setup phase
         This follow PyTorch Lightning's setup() convention
         """
         pass
 
 
 class NoBaseline(REINFORCEBaseline):
-    def eval(self, td, reward):
+    """No baseline: return 0 for baseline and neg_los"""
+
+    def eval(self, td, reward, env=None):
         return 0, 0  # No baseline, no neg_los
 
 
 class SharedBaseline(REINFORCEBaseline):
-    def eval(self, td, reward, on_dim=1):  # e.g. [batch, pomo, ...]
+    """Shared baseline: return mean of reward as baseline"""
+
+    def eval(self, td, reward, env=None, on_dim=1):  # e.g. [batch, pomo, ...]
         return reward.mean(dim=on_dim, keepdims=True), 0
 
 
 class ExponentialBaseline(REINFORCEBaseline):
-    def __init__(self, beta=0.8):
+    """Exponential baseline: return exponential moving average of reward as baseline
+
+    Args:
+        beta: Beta value for the exponential moving average
+    """
+
+    def __init__(self, beta=0.8, **kw):
         super(REINFORCEBaseline, self).__init__()
 
         self.beta = beta
         self.v = None
 
-    def eval(self, td, reward):
+    def eval(self, td, reward, env=None):
         if self.v is None:
             v = reward.mean()
         else:
             v = self.beta * self.v + (1.0 - self.beta) * reward.mean()
         self.v = v.detach()  # Detach since we never want to backprop
         return self.v, 0  # No loss
 
 
 class WarmupBaseline(REINFORCEBaseline):
-    def __init__(
-        self,
-        baseline,
-        n_epochs=1,
-        warmup_exp_beta=0.8,
-    ):
+    """Warmup baseline: return convex combination of baseline and exponential baseline
+
+    Args:
+        baseline: Baseline to use after warmup
+        n_epochs: Number of epochs to warmup
+        warmup_exp_beta: Beta value for the exponential baseline during warmup
+    """
+
+    def __init__(self, baseline, n_epochs=1, warmup_exp_beta=0.8, **kw):
         super(REINFORCEBaseline, self).__init__()
 
         self.baseline = baseline
         assert n_epochs > 0, "n_epochs to warmup must be positive"
         self.warmup_baseline = ExponentialBaseline(warmup_exp_beta)
         self.alpha = 0
         self.n_epochs = n_epochs
@@ -87,72 +101,96 @@
         if self.alpha > 0:
             return self.baseline.wrap_dataset(dataset, *args, **kw)
         return self.warmup_baseline.wrap_dataset(dataset, *args, **kw)
 
     def setup(self, *args, **kw):
         self.baseline.setup(*args, **kw)
 
-    def eval(self, td, reward):
+    def eval(self, td, reward, env=None):
         if self.alpha == 1:
-            return self.baseline.eval(td, reward)
+            return self.baseline.eval(td, reward, env)
         if self.alpha == 0:
-            return self.warmup_baseline.eval(td, reward)
-        v_b, l_b = self.baseline.eval(td, reward)
-        v_wb, l_wb = self.warmup_baseline.eval(td, reward)
+            return self.warmup_baseline.eval(td, reward, env)
+        v_b, l_b = self.baseline.eval(td, reward, env)
+        v_wb, l_wb = self.warmup_baseline.eval(td, reward, env)
         # Return convex combination of baseline and of loss
         return self.alpha * v_b + (1 - self.alpha) * v_wb, self.alpha * l_b + (
             1 - self.alpha * l_wb
         )
 
     def epoch_callback(self, *args, **kw):
         # Need to call epoch callback of inner model (also after first epoch if we have not used it)
         self.baseline.epoch_callback(*args, **kw)
         self.alpha = (kw["epoch"] + 1) / float(self.n_epochs)
         if kw["epoch"] < self.n_epochs:
             log.info("Set warmup alpha = {}".format(self.alpha))
 
 
 class CriticBaseline(REINFORCEBaseline):
-    def __init__(self, critic, **unused_kw):
+    """Critic baseline: use critic network as baseline
+
+    Args:
+        critic: Critic network to use as baseline. If None, create a new critic network based on the environment
+    """
+
+    def __init__(self, critic: nn.Module = None, **unused_kw):
         super(CriticBaseline, self).__init__()
         self.critic = critic
 
-    def eval(self, x, c):
+    def setup(self, model, env, **kwargs):
+        if self.critic is None:
+            log.info("Creating critic network for {}".format(env.name))
+            self.critic = CriticNetwork(env.name, **kwargs)
+
+    def eval(self, x, c, env=None):
         v = self.critic(x)
         # detach v since actor should not backprop through baseline, only for neg_loss
         return v.detach(), -F.mse_loss(v, c.detach())
 
 
 class RolloutBaseline(REINFORCEBaseline):
-    def __init__(self, bl_alpha=0.05, progress_bar=False):
+    """Rollout baseline: use greedy rollout as baseline
+
+    Args:
+        bl_alpha: Alpha value for the baseline T-test
+        progress_bar: Whether to show progress bar for rollout
+    """
+
+    def __init__(self, bl_alpha=0.05, progress_bar=False, **kw):
         super(RolloutBaseline, self).__init__()
         self.bl_alpha = bl_alpha
         self.progress_bar = progress_bar
 
     def setup(self, *args, **kw):
         self._update_model(*args, **kw)
 
     def _update_model(
         self, model, env, batch_size=64, device="cpu", dataset_size=None, dataset=None
     ):
+        """Update model and rollout baseline values"""
         self.model = copy.deepcopy(model).to(device)
         if dataset is None:
             log.info("Creating evaluation dataset for rollout baseline")
             self.dataset = env.dataset(batch_size=[dataset_size])
 
         log.info("Evaluating baseline model on evaluation dataset")
         self.bl_vals = (
             self.rollout(self.model, env, batch_size, device, self.dataset).cpu().numpy()
         )
         self.mean = self.bl_vals.mean()
 
-    def eval(self, td, reward):
-        # Use volatile mode for efficient inference (single batch so we do not use rollout function)
+    def eval(self, td, reward, env):
+        """Evaluate rollout baseline
+
+        Warning:
+            This is not differentiable and should only be used for evaluation.
+            Also, it is recommended to use the `rollout` method directly instead of this method.
+        """
         with torch.no_grad():
-            reward = self.model(td)["reward"]
+            reward = self.model(td, env)["reward"]
         return reward, 0
 
     def epoch_callback(
         self, model, env, batch_size=64, device="cpu", epoch=None, dataset_size=None
     ):
         """Challenges the current baseline with the model and replaces the baseline model if it is improved"""
         log.info("Evaluating candidate model on evaluation dataset")
@@ -171,36 +209,43 @@
             p_val = p / 2  # one-sided
             assert t < 0, "T-statistic should be negative"
             log.info("p-value: {:.3f}".format(p_val))
             if p_val < self.bl_alpha:
                 log.info("Updating baseline")
                 self._update_model(model, env, batch_size, device, dataset_size)
 
-    def rollout(self, model, env=None, batch_size=64, device="cpu", dataset=None):
+    def rollout(self, model, env, batch_size=64, device="cpu", dataset=None):
         """Rollout the model on the given dataset"""
+
         # if dataset is None, use the dataset of the baseline
         dataset = self.dataset if dataset is None else dataset
 
         model.eval()
         model = model.to(device)
 
         def eval_model(batch):
             with torch.no_grad():
                 batch = env.reset(batch.to(device))
-                return model(batch, decode_type="greedy")["reward"].data.cpu()
+                return model(batch, env, decode_type="greedy")["reward"].data.cpu()
 
         dl = DataLoader(dataset, batch_size=batch_size, collate_fn=tensordict_collate_fn)
 
         retval = torch.cat(
             [eval_model(batch) for batch in tqdm(dl, disable=not self.progress_bar)], 0
         )
         return retval
 
     def wrap_dataset(self, dataset, env, batch_size=64, device="cpu", **kw):
-        """Wrap the dataset in a baseline dataset"""
+        """Wrap the dataset in a baseline dataset
+
+        Note:
+            This is an alternative to `eval` that does not require the model to be passed
+            at every call but just once. Values are added to the dataset. This also allows for
+            larger batch sizes since we evauate the model without gradients.
+        """
         rewards = (
             self.rollout(self.model, env, batch_size, device, dataset=dataset)
             .detach()
             .cpu()
         )
         return ExtraKeyDataset(dataset, rewards)
 
@@ -213,7 +258,43 @@
             pass
         return state
 
     def __setstate__(self, state):
         """Restore datasets after unpickling. Will be restored in setup"""
         self.__dict__.update(state)
         self.dataset = None
+
+
+REINFORCE_BASELINES_REGISTRY = {
+    "no": NoBaseline,
+    "shared": SharedBaseline,
+    "exponential": ExponentialBaseline,
+    "critic": CriticBaseline,
+    "rollout_only": RolloutBaseline,
+    "warmup": WarmupBaseline,
+}
+
+
+def get_reinforce_baseline(name, **kw):
+    """Get a REINFORCE baseline by name
+    The rollout baseline default to warmup baseline with one epoch of
+    exponential baseline and the greedy rollout
+    """
+    if name == "warmup":
+        inner_baseline = kw.get("baseline", "rollout")
+        if not isinstance(inner_baseline, REINFORCEBaseline):
+            inner_baseline = get_reinforce_baseline(inner_baseline, **kw)
+        return WarmupBaseline(inner_baseline, **kw)
+    elif name == "rollout":
+        warmup_epochs = kw.get("n_epochs", 1)
+        warmup_exp_beta = kw.get("exp_beta", 0.8)
+        bl_alpha = kw.get("bl_alpha", 0.05)
+        return WarmupBaseline(
+            RolloutBaseline(bl_alpha=bl_alpha), warmup_epochs, warmup_exp_beta
+        )
+
+    baseline_cls = REINFORCE_BASELINES_REGISTRY.get(name, None)
+    if baseline_cls is None:
+        raise ValueError(
+            f"Unknown baseline {baseline_cls}. Available baselines: {REINFORCE_BASELINES_REGISTRY.keys()}"
+        )
+    return baseline_cls(**kw)
```

### Comparing `rl4co-0.0.6/rl4co/models/rl/reinforce/critic.py` & `rl4co-0.1.0/rl4co/models/zoo/ham/encoder.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,60 +1,68 @@
-from torch import nn
+import torch.nn as nn
 
-from rl4co.models.nn.graph.gat import GraphAttentionEncoder
+from rl4co.models.nn.env_embeddings import env_init_embedding
+from rl4co.models.nn.graph.attnnet import Normalization, SkipConnection
+from rl4co.models.zoo.ham.attention import HeterogenousMHA
 
 
-class CriticNetwork(nn.Module):
-    """We make the critic network compatible with any problem by using encoder for any environment
-    Refactored from Kool et al. (2019) which only worked for TSP
-    Reference: https://github.com/wouterkool/attention-learn-to-route
-
-    Args:
-        env (EnvBase): environment
-        encoder (nn.Module, optional): encoder. Defaults to None. Initialized with GraphAttentionEncoder.
-        embedding_dim (int, optional): embedding dimension. Defaults to 128.
-        hidden_dim (int, optional): hidden dimension. Defaults to 512.
-        n_layers (int, optional): number of encoder layers. Defaults to 3.
-        num_heads (int, optional): number of attention heads. Defaults to 8.
-        encoder_normalization (str, optional): normalization. Defaults to "batch".
-    """
+class HeterogeneuousMHALayer(nn.Sequential):
+    def __init__(
+        self,
+        num_heads,
+        embed_dim,
+        feed_forward_hidden=512,
+        normalization="batch",
+    ):
+        super(HeterogeneuousMHALayer, self).__init__(
+            SkipConnection(HeterogenousMHA(num_heads, embed_dim, embed_dim)),
+            Normalization(embed_dim, normalization),
+            SkipConnection(
+                nn.Sequential(
+                    nn.Linear(embed_dim, feed_forward_hidden),
+                    nn.ReLU(),
+                    nn.Linear(feed_forward_hidden, embed_dim),
+                )
+                if feed_forward_hidden > 0
+                else nn.Linear(embed_dim, embed_dim)
+            ),
+            Normalization(embed_dim, normalization),
+        )
 
+
+class GraphHeterogeneousAttentionEncoder(nn.Module):
     def __init__(
         self,
-        env=None,
-        encoder=None,
-        embedding_dim=128,
-        hidden_dim=512,
-        num_layers=3,
-        num_heads=8,
-        encoder_normalization="batch",
-        use_native_sdpa=False,
+        num_heads,
+        embedding_dim,
+        num_encoder_layers,
+        env_name=None,
+        normalization="batch",
+        feed_forward_hidden=512,
         force_flash_attn=False,
     ):
-        super(CriticNetwork, self).__init__()
+        super(GraphHeterogeneousAttentionEncoder, self).__init__()
 
-        self.encoder = (
-            GraphAttentionEncoder(
-                num_heads=num_heads,
-                embedding_dim=embedding_dim,
-                num_layers=num_layers,
-                env=env,
-                normalization=encoder_normalization,
-                feed_forward_hidden=hidden_dim,
-                use_native_sdpa=use_native_sdpa,
-                force_flash_attn=force_flash_attn,
-            )
-            if encoder is None
-            else encoder
+        # Map input to embedding space
+        self.init_embedding = env_init_embedding(
+            env_name, {"embedding_dim": embedding_dim}
         )
 
-        self.value_head = nn.Sequential(
-            nn.Linear(embedding_dim, hidden_dim), nn.ReLU(), nn.Linear(hidden_dim, 1)
+        self.layers = nn.Sequential(
+            *(
+                HeterogeneuousMHALayer(
+                    num_heads,
+                    embedding_dim,
+                    feed_forward_hidden,
+                    normalization,
+                )
+                for _ in range(num_encoder_layers)
+            )
         )
 
-    def forward(self, td):
-        graph_embeddings, _ = self.encoder(td)
-        # graph_embedings: [batch_size, graph_size, input_dim]
-        # return self.value_head(graph_embeddings.mean(1))
-
-        # L2D style
-        return self.value_head(graph_embeddings).mean(1)
+    def forward(self, x, mask=None):
+        assert mask is None, "Mask not yet supported!"
+        # initial Embedding from features
+        init_embeds = self.init_embedding(x)  # (batch_size, graph_size, embed_dim)
+        # layers  (batch_size, graph_size, embed_dim)
+        embeds = self.layers(init_embeds)
+        return embeds, init_embeds
```

### Comparing `rl4co-0.0.6/rl4co/models/zoo/am/decoder.py` & `rl4co-0.1.0/rl4co/models/zoo/pomo/decoder.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,37 +4,30 @@
 import torch.nn as nn
 
 from einops import rearrange
 
 from rl4co.models.nn.attention import LogitAttention
 from rl4co.models.nn.env_embeddings import env_context_embedding, env_dynamic_embedding
 from rl4co.models.nn.utils import decode_probs
+from rl4co.utils import get_pylogger
 from rl4co.utils.ops import batchify, select_start_nodes, unbatchify
 
+log = get_pylogger(__name__)
+
 
 @dataclass
 class PrecomputedCache:
     node_embeddings: torch.Tensor
-    graph_context: torch.Tensor
     glimpse_key: torch.Tensor
     glimpse_val: torch.Tensor
     logit_key: torch.Tensor
 
 
 class Decoder(nn.Module):
-    """Auto-regressive decoder for the Attention Model for constructing solutions
-    We additionally include support for greedy multi-starts during inference (as in POMO)
-
-    Args:
-        env: Environment to solve
-        embedding_dim: Dimension of the embeddings
-        num_heads: Number of heads for the attention
-    """
-
-    def __init__(self, env, embedding_dim, num_heads, **logit_attn_kwargs):
+    def __init__(self, env, embedding_dim, num_heads, num_starts=20, **logit_attn_kwargs):
         super(Decoder, self).__init__()
 
         self.env = env
         self.embedding_dim = embedding_dim
         self.num_heads = num_heads
 
         assert embedding_dim % num_heads == 0
@@ -53,38 +46,43 @@
         self.project_fixed_context = nn.Linear(embedding_dim, embedding_dim, bias=False)
 
         # MHA
         self.logit_attention = LogitAttention(
             embedding_dim, num_heads, **logit_attn_kwargs
         )
 
+        # POMO multi-start sampling
+        self.num_starts = max(num_starts, 0)  # num_starts = 0 is just normal REINFORCE
+
     def forward(
         self,
         td,
         embeddings,
         decode_type="sampling",
         softmax_temp=None,
+        single_traj=False,
         num_starts=None,
-        calc_reward=True,
     ):
         # Greedy multi-start decoding if num_starts > 1
-        num_starts = 0 if num_starts is None else num_starts
+        num_starts = (
+            self.num_starts if num_starts is None else num_starts
+        )  # substitute self.num_starts with num_starts
         assert not (
             "multistart" in decode_type and num_starts <= 1
         ), "Multi-start decoding requires `num_starts` > 1"
 
         # Compute keys, values for the glimpse and keys for the logits once as they can be reused in every step
-        cached_embeds = self._precompute(embeddings, num_starts=num_starts)
+        cached_embeds = self._precompute(embeddings)
 
         # Collect outputs
         outputs = []
         actions = []
 
-        # Multi-start decoding: first action is chosen by ad-hoc node selection
-        if num_starts > 1 or "multistart" in decode_type:
+        if num_starts > 1 and not single_traj or "multistart" in decode_type:
+            # POMO: first action is decided via select_start_nodes
             action = select_start_nodes(td, num_starts, self.env)
 
             # Expand td to batch_size * num_starts
             td = batchify(td, num_starts)
 
             td.set("action", action)
             td = self.env.step(td)["next"]
@@ -106,53 +104,43 @@
             td = self.env.step(td)["next"]
 
             # Collect output of step
             outputs.append(log_p)
             actions.append(action)
 
         outputs, actions = torch.stack(outputs, 1), torch.stack(actions, 1)
-        if calc_reward:
-            td.set("reward", self.env.get_reward(td, actions))
-
+        td.set("reward", self.env.get_reward(td, actions))
         return outputs, actions, td
 
-    def _precompute(self, embeddings, num_starts=0):
+    def _precompute(self, embeddings):
         # The projection of the node embeddings for the attention is calculated once up front
         (
             glimpse_key_fixed,
             glimpse_val_fixed,
             logit_key_fixed,
         ) = self.project_node_embeddings(embeddings).chunk(3, dim=-1)
 
-        # Batchify and unbatchify have no effect if num_starts = 0.
-        # Otherwise, we need to batchify the embeddings to modify key value (i.e. for the lenght of queries)
-        graph_context = unbatchify(
-            batchify(self.project_fixed_context(embeddings.mean(1)), num_starts),
-            num_starts,
-        )
-
         # Organize in a dataclass for easy access
         cached_embeds = PrecomputedCache(
             node_embeddings=embeddings,
-            graph_context=graph_context,
             glimpse_key=glimpse_key_fixed,
             glimpse_val=glimpse_val_fixed,
             logit_key=logit_key_fixed,
         )
 
         return cached_embeds
 
     def _get_log_p(self, cached, td, softmax_temp=None, num_starts=0):
         # Compute the query based on the context (computes automatically the first and last node context)
 
         # Unbatchify to [batch_size, num_starts, ...]. Has no effect if num_starts = 0
         td_unbatch = unbatchify(td, num_starts)
 
         step_context = self.context(cached.node_embeddings, td_unbatch)
-        glimpse_q = step_context + cached.graph_context
+        glimpse_q = step_context  # in POMO, no graph context is used to compute query
         glimpse_q = glimpse_q.unsqueeze(1) if glimpse_q.ndim == 2 else glimpse_q
 
         # Compute keys and values for the nodes
         (
             glimpse_key_dynamic,
             glimpse_val_dynamic,
             logit_key_dynamic,
```

### Comparing `rl4co-0.0.6/rl4co/models/zoo/am/model.py` & `rl4co-0.1.0/rl4co/models/zoo/et/model.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,25 +1,29 @@
-from rl4co.models.rl.reinforce.base import REINFORCE
-from rl4co.models.rl.reinforce.baselines import RolloutBaseline, WarmupBaseline
+from typing import Optional, Union
+
+from rl4co.envs.common.base import RL4COEnvBase
+from rl4co.models.rl import REINFORCE
+from rl4co.models.rl.reinforce.baselines import REINFORCEBaseline
 from rl4co.models.zoo.am.policy import AttentionModelPolicy
 
 
-class AttentionModel(REINFORCE):
-    """
-    Attention Model for neural combinatorial optimization based on REINFORCE
-    Based on Wouter Kool et al. (2018) https://arxiv.org/abs/1803.08475
-    Refactored from reference implementation: https://github.com/wouterkool/attention-learn-to-route
-
-    Args:
-        env: TorchRL Environment
-        policy: Policy
-        baseline: REINFORCE Baseline
+class EquityTransformer(REINFORCE):
+    """Equity Transformer from Son et al., 2023.
+    Reference: https://arxiv.org/abs/2306.02689
+
+    Warning:
+        This implementation is under development and subject to change.
     """
 
-    def __init__(self, env, policy=None, baseline=None, **policy_kwargs):
-        super(AttentionModel, self).__init__(env, policy, baseline)
-        self.policy = (
-            AttentionModelPolicy(self.env, **policy_kwargs) if policy is None else policy
-        )
-        self.baseline = (
-            WarmupBaseline(RolloutBaseline()) if baseline is None else baseline
-        )
+    def __init__(
+        self,
+        env: RL4COEnvBase,
+        policy: Optional(AttentionModelPolicy) = None,
+        baseline: Union[REINFORCEBaseline, str] = "rollout",
+        policy_kwargs={},
+        baseline_kwargs={},
+        **kwargs,
+    ):
+        if policy is None:
+            policy = AttentionModelPolicy(env.name, **policy_kwargs)
+
+        super().__init__(env, policy, baseline, baseline_kwargs, **kwargs)
```

### Comparing `rl4co-0.0.6/rl4co/models/zoo/am/policy.py` & `rl4co-0.1.0/rl4co/models/zoo/pomo/policy.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 import torch.nn as nn
 
 from tensordict.tensordict import TensorDict
 from torchrl.envs import EnvBase
 
-from rl4co.models.nn.graph.gat import GraphAttentionEncoder
+from rl4co.models.nn.graph.attnnet import GraphAttentionEncoder
 from rl4co.models.nn.utils import get_log_likelihood
-from rl4co.models.zoo.am.decoder import Decoder
+from rl4co.models.zoo.pomo.decoder import Decoder
 from rl4co.utils.pylogger import get_pylogger
 
 log = get_pylogger(__name__)
 
 
-class AttentionModelPolicy(nn.Module):
+class POMOPolicy(nn.Module):
     def __init__(
         self,
         env: EnvBase,
         encoder: nn.Module = None,
         decoder: nn.Module = None,
         embedding_dim: int = 128,
-        num_encoder_layers: int = 3,
+        num_starts: int = 10,
+        num_encoder_layers: int = 6,
+        normalization: str = "instance",
         num_heads: int = 8,
-        normalization: str = "batch",
         mask_inner: bool = True,
         use_native_sdpa: bool = False,
         force_flash_attn: bool = False,
         train_decode_type: str = "sampling",
         val_decode_type: str = "greedy",
         test_decode_type: str = "greedy",
         **unused_kw,
     ):
-        super(AttentionModelPolicy, self).__init__()
+        super(POMOPolicy, self).__init__()
         if len(unused_kw) > 0:
             log.warn(f"Unused kwargs: {unused_kw}")
 
         self.env = env
 
         self.encoder = (
             GraphAttentionEncoder(
@@ -47,55 +48,48 @@
             )
             if encoder is None
             else encoder
         )
 
         self.decoder = (
             Decoder(
-                env,
+                self.env,
                 embedding_dim,
                 num_heads,
+                num_starts=num_starts,
                 mask_inner=mask_inner,
                 force_flash_attn=force_flash_attn,
             )
             if decoder is None
             else decoder
         )
-
         self.train_decode_type = train_decode_type
         self.val_decode_type = val_decode_type
         self.test_decode_type = test_decode_type
 
     def forward(
         self,
         td: TensorDict,
         phase: str = "train",
         return_actions: bool = False,
-        return_entropy: bool = False,
         **decoder_kwargs,
     ) -> dict:
         # Encode inputs
         embeddings, _ = self.encoder(td)
 
         # Get decode type depending on phase
         if decoder_kwargs.get("decode_type", None) is None:
             decoder_kwargs["decode_type"] = getattr(self, f"{phase}_decode_type")
 
         # Main rollout: autoregressive decoding
         log_p, actions, td_out = self.decoder(td, embeddings, **decoder_kwargs)
 
-        # Log likelihood is calculated within the model since returning it per action does not work well with
+        # Log likelyhood is calculated within the model since returning it per action does not work well with
         ll = get_log_likelihood(log_p, actions, td_out.get("mask", None))
-
         out = {
             "reward": td_out["reward"],
             "log_likelihood": ll,
         }
         if return_actions:
             out["actions"] = actions
 
-        if return_entropy:
-            entropy = -(log_p.exp() * log_p).nansum(dim=1)  # [batch, decoder steps]
-            entropy = entropy.sum(dim=1)  # [batch]
-            out["entropy"] = entropy
-
         return out
```

### Comparing `rl4co-0.0.6/rl4co/models/zoo/ham/attention.py` & `rl4co-0.1.0/rl4co/models/zoo/ham/attention.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.6/rl4co/models/zoo/ham/policy.py` & `rl4co-0.1.0/rl4co/models/zoo/mdam/policy.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,91 +1,87 @@
 import torch.nn as nn
+from typing import Union
 
-from tensordict.tensordict import TensorDict
-from torchrl.envs import EnvBase
+from tensordict import TensorDict
+from rl4co.envs import RL4COEnvBase, get_env
 
-from rl4co.models.nn.utils import get_log_likelihood
-from rl4co.models.zoo.am.decoder import Decoder
-from rl4co.models.zoo.ham.encoder import GraphHeterogeneousAttentionEncoder
+from rl4co.models.nn.env_embeddings import env_init_embedding
+from rl4co.models.zoo.mdam.decoder import Decoder
+from rl4co.models.zoo.mdam.encoder import GraphAttentionEncoder
+from rl4co.models.zoo.common.autoregressive import AutoregressivePolicy
 from rl4co.utils.pylogger import get_pylogger
 
 log = get_pylogger(__name__)
 
 
-class HeterogeneousAttentionModelPolicy(nn.Module):
+class MDAMPolicy(AutoregressivePolicy):
+    """ Multi-Decoder Attention Model (MDAM) policy.
+    Args:
+
+    """
+    
     def __init__(
-        self,
-        env: EnvBase,
-        encoder: nn.Module = None,
-        decoder: nn.Module = None,
+        self, 
+        env_name: str,
         embedding_dim: int = 128,
         num_encoder_layers: int = 3,
         num_heads: int = 8,
         normalization: str = "batch",
-        mask_inner: bool = True,
-        force_flash_attn: bool = False,
-        train_decode_type: str = "sampling",
-        val_decode_type: str = "greedy",
-        test_decode_type: str = "greedy",
-        **unused_kw,
+        **kwargs,
     ):
-        super(HeterogeneousAttentionModelPolicy, self).__init__()
-        if len(unused_kw) > 0:
-            log.warn(f"Unused kwargs: {unused_kw}")
-
-        self.env = env
-
-        self.encoder = (
-            GraphHeterogeneousAttentionEncoder(
+        super(MDAMPolicy, self).__init__(
+            env_name=env_name,
+            encoder=GraphAttentionEncoder(
                 num_heads=num_heads,
-                embedding_dim=embedding_dim,
+                embed_dim=embedding_dim,
                 num_layers=num_encoder_layers,
-                env=self.env,
                 normalization=normalization,
-            )
-            if encoder is None
-            else encoder
+                **kwargs
+            ),
+            decoder=Decoder(
+                env_name=env_name,
+                embedding_dim=embedding_dim,
+                num_heads=num_heads,
+                **kwargs
+            ),
+            embedding_dim=embedding_dim,
+            num_encoder_layers=num_encoder_layers,
+            num_heads=num_heads,
+            normalization=normalization,
+            **kwargs,
         )
 
-        self.decoder = (
-            Decoder(
-                self.env,
-                embedding_dim,
-                num_heads,
-                mask_inner=mask_inner,
-                force_flash_attn=force_flash_attn,
-            )
-            if decoder is None
-            else decoder
+        self.init_embedding = env_init_embedding(
+            env_name, {"embedding_dim": embedding_dim}
         )
 
-        self.train_decode_type = train_decode_type
-        self.val_decode_type = val_decode_type
-        self.test_decode_type = test_decode_type
-
     def forward(
         self,
         td: TensorDict,
+        env: Union[str, RL4COEnvBase] = None,
         phase: str = "train",
         return_actions: bool = False,
         **decoder_kwargs,
     ) -> TensorDict:
-        # Encode inputs
-        embeddings, _ = self.encoder(td)
+        embedding = self.init_embedding(td)
+        encoded_inputs, _, attn, V, h_old = self.encoder(embedding)
+
+        # Instantiate environment if needed
+        if isinstance(env, str) or env is None:
+            env_name = self.env_name if env is None else env
+            log.info(f"Instantiated environment not provided; instantiating {env_name}")
+            env = get_env(env_name)
 
         # Get decode type depending on phase
         if decoder_kwargs.get("decode_type", None) is None:
             decoder_kwargs["decode_type"] = getattr(self, f"{phase}_decode_type")
 
-        # Main rollout: autoregressive decoding
-        log_p, actions, td_out = self.decoder(td, embeddings, **decoder_kwargs)
-
-        # Log likelyhood is calculated within the model since returning it per action does not work well with
-        ll = get_log_likelihood(log_p, actions, td_out.get("mask", None))
+        reward, log_likelihood, kl_divergence, actions = self.decoder(
+            td, encoded_inputs, env, attn, V, h_old, **decoder_kwargs
+        )
         out = {
-            "reward": td_out["reward"],
-            "log_likelihood": ll,
+            "reward": reward,
+            "log_likelihood": log_likelihood,
+            "entropy": kl_divergence,
+            "actions": actions if return_actions else None,
         }
-        if return_actions:
-            out["actions"] = actions
-
-        return out
+        return out
```

### Comparing `rl4co-0.0.6/rl4co/models/zoo/mdam/decoder.py` & `rl4co-0.1.0/rl4co/models/zoo/mdam/decoder.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 import math
+from typing import Union
 
 from dataclasses import dataclass
+from tensordict import TensorDict
 
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 
+from rl4co.envs import RL4COEnvBase
+
 from rl4co.models.nn.attention import LogitAttention
 from rl4co.models.nn.env_embeddings import env_context_embedding, env_dynamic_embedding
 from rl4co.models.nn.utils import decode_probs, get_log_likelihood
 
 
 @dataclass
 class PrecomputedCache:
@@ -19,15 +23,15 @@
     glimpse_val: torch.Tensor
     logit_key: torch.Tensor
 
 
 class Decoder(nn.Module):
     def __init__(
         self,
-        env,
+        env_name,
         embedding_dim,
         num_heads,
         num_paths: int = 5,
         mask_inner: bool = True,
         mask_logits: bool = True,
         eg_step_gap: int = 200,
         tanh_clipping: float = 10.0,
@@ -35,83 +39,92 @@
         shrink_size=None,
         train_decode_type: str = "sampling",
         val_decode_type: str = "greedy",
         test_decode_type: str = "greedy",
     ):
         super(Decoder, self).__init__()
         self.dynamic_embedding = env_dynamic_embedding(
-            env, {"embedding_dim": embedding_dim}
+            env_name, {"embedding_dim": embedding_dim}
         )
 
         self.train_decode_type = train_decode_type
         self.val_decode_type = val_decode_type
         self.test_decode_type = test_decode_type
 
         self.W_placeholder = nn.Parameter(torch.Tensor(2 * embedding_dim))
         self.W_placeholder.data.uniform_(
             -1, 1
         )  # Placeholder should be in range of activations
 
         self.context = [
-            env_context_embedding(env.name, {"embedding_dim": embedding_dim})
+            env_context_embedding(env_name, {"embedding_dim": embedding_dim})
             for _ in range(num_paths)
         ]
 
         self.project_node_embeddings = [
-            nn.Linear(embedding_dim, 3 * embedding_dim, device=env.device, bias=False)
+            nn.Linear(embedding_dim, 3 * embedding_dim, bias=False)
             for _ in range(num_paths)
         ]
         self.project_node_embeddings = nn.ModuleList(self.project_node_embeddings)
 
         self.project_fixed_context = [
-            nn.Linear(embedding_dim, embedding_dim, device=env.device, bias=False)
+            nn.Linear(embedding_dim, embedding_dim, bias=False)
             for _ in range(num_paths)
         ]
         self.project_fixed_context = nn.ModuleList(self.project_fixed_context)
 
         self.project_step_context = [
-            nn.Linear(2 * embedding_dim, embedding_dim, device=env.device, bias=False)
+            nn.Linear(2 * embedding_dim, embedding_dim, bias=False)
             for _ in range(num_paths)
         ]
         self.project_step_context = nn.ModuleList(self.project_step_context)
 
         self.project_out = [
-            nn.Linear(embedding_dim, embedding_dim, device=env.device, bias=False)
+            nn.Linear(embedding_dim, embedding_dim, bias=False)
             for _ in range(num_paths)
         ]
         self.project_out = nn.ModuleList(self.project_out)
 
         self.dynamic_embedding = env_dynamic_embedding(
-            env.name, {"embedding_dim": embedding_dim}
+            env_name, {"embedding_dim": embedding_dim}
         )
 
         self.logit_attention = [
             LogitAttention(
                 embedding_dim,
                 num_heads,
                 mask_inner=mask_inner,
                 force_flash_attn=force_flash_attn,
             )
             for _ in range(num_paths)
         ]
 
-        self.env = env
+        self.env_name = env_name
         self.mask_inner = mask_inner
         self.mask_logits = mask_logits
         self.num_heads = num_heads
         self.num_paths = num_paths
         self.eg_step_gap = eg_step_gap
         self.tanh_clipping = tanh_clipping
         self.shrink_size = shrink_size
 
-    def forward(self, td, encoded_inputs, attn, V, h_old, **decoder_kwargs):
+    def forward(
+            self, 
+            td: TensorDict, 
+            encoded_inputs: torch.Tensor, 
+            env: Union[str, RL4COEnvBase],
+            attn, 
+            V,
+            h_old,
+            **decoder_kwargs
+        ):
         # SECTION: Decoder first step: calculate for the decoder divergence loss
         # Cost list and log likelihood list along with path
         output_list = []
-        td_list = [self.env.reset(td) for i in range(self.num_paths)]
+        td_list = [env.reset(td) for i in range(self.num_paths)]
         for i in range(self.num_paths):
             # Clone the encoded features for this path
             _encoded_inputs = encoded_inputs.clone()
 
             # Compute keys, values for the glimpse and keys for the logits once as they can be reused in every step
             fixed = self._precompute(_encoded_inputs, path_index=i)
             log_p, _ = self._get_log_p(fixed, td_list[i], i)
@@ -143,15 +156,15 @@
 
         # SECTION: Decoder rest step: calculate for other decoder divergence loss
         # Cost list and log likelihood list along with path
         reward_list = []
         output_list = []
         action_list = []
         ll_list = []
-        td_list = [self.env.reset(td) for _ in range(self.num_paths)]
+        td_list = [env.reset(td) for _ in range(self.num_paths)]
         for i in range(self.num_paths):
             # Clone the encoded features for this path
             _encoded_inputs = encoded_inputs.clone()
             _attn = attn.clone()
             _V = V.clone()
             _h_old = h_old.clone()
 
@@ -178,23 +191,23 @@
                 action = decode_probs(
                     log_p.exp()[:, 0, :],
                     mask,
                     decode_type=decoder_kwargs["decode_type"],
                 )
 
                 td_list[i].set("action", action)
-                td_list[i] = self.env.step(td_list[i])["next"]
+                td_list[i] = env.step(td_list[i])["next"]
 
                 # Collect output of step
                 outputs.append(log_p[:, 0, :])
                 actions.append(action)
                 j += 1
 
             outputs, actions = torch.stack(outputs, 1), torch.stack(actions, 1)
-            reward = self.env.get_reward(td, actions)
+            reward = env.get_reward(td, actions)
             ll = get_log_likelihood(outputs, actions, mask)
 
             reward_list.append(reward)
             output_list.append(outputs)
             action_list.append(actions)
             ll_list.append(ll)
 
@@ -244,15 +257,15 @@
             )  # (n_heads, batch_size, num_steps, graph_size, head_dim)
         )
 
     def _get_log_p(self, fixed, td, path_index, normalize=True):
         step_context = self.context[path_index](
             fixed.node_embeddings, td
         )  # [batch, embed_dim]
-        glimpse_q = fixed.graph_context + step_context.unsqueeze(1)
+        glimpse_q = fixed.graph_context + step_context.unsqueeze(1).to(fixed.graph_context.device)
 
         # Compute keys and values for the nodes
         (
             glimpse_key_dynamic,
             glimpse_val_dynamic,
             logit_key_dynamic,
         ) = self.dynamic_embedding(td)
```

### Comparing `rl4co-0.0.6/rl4co/models/zoo/mdam/encoder.py` & `rl4co-0.1.0/rl4co/models/zoo/mdam/encoder.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.6/rl4co/models/zoo/pomo/augmentations.py` & `rl4co-0.1.0/rl4co/models/zoo/pomo/augmentations.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.6/rl4co/models/zoo/pomo/model.py` & `rl4co-0.1.0/rl4co/models/zoo/pomo/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from tensordict import TensorDict
 
-from rl4co.models.rl.reinforce.base import REINFORCE
+from rl4co.models.rl.reinforce.reinforce import REINFORCE
 from rl4co.models.rl.reinforce.baselines import SharedBaseline
 from rl4co.models.zoo.pomo.augmentations import StateAugmentation
 from rl4co.models.zoo.pomo.policy import POMOPolicy
 from rl4co.utils.ops import gather_by_index, unbatchify
 
 
 class POMO(REINFORCE):
```

### Comparing `rl4co-0.0.6/rl4co/models/zoo/ptrnet/critic.py` & `rl4co-0.1.0/rl4co/models/zoo/ptrnet/critic.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.6/rl4co/models/zoo/ptrnet/decoder.py` & `rl4co-0.1.0/rl4co/models/zoo/ptrnet/decoder.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.6/rl4co/models/zoo/ptrnet/encoder.py` & `rl4co-0.1.0/rl4co/models/zoo/ptrnet/encoder.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.6/rl4co/models/zoo/ptrnet/policy.py` & `rl4co-0.1.0/rl4co/models/zoo/ptrnet/policy.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,27 +10,27 @@
 
 log = get_pylogger(__name__)
 
 
 class PointerNetworkPolicy(nn.Module):
     def __init__(
         self,
-        env,
+        env_name,
         embedding_dim: int = 128,
         hidden_dim: int = 128,
         tanh_clipping=10.0,
         mask_inner=True,
         mask_logits=True,
         **kwargs,
     ):
         super(PointerNetworkPolicy, self).__init__()
 
         # torch.backends.cudnn.enabled=False
-        self.env = env
-        assert self.env.name == "tsp", "Only the Euclidean TSP env supported"
+        assert env_name == "tsp", "Only the Euclidean TSP env supported"
+        self.env_name = env_name
 
         self.input_dim = 2
 
         self.encoder = Encoder(embedding_dim, hidden_dim)
 
         self.decoder = Decoder(
             embedding_dim,
@@ -49,14 +49,15 @@
 
         self.embedding = nn.Parameter(torch.FloatTensor(self.input_dim, embedding_dim))
         self.embedding.data.uniform_(-std, std)
 
     def forward(
         self,
         td,
+        env,
         phase: str = "train",
         decode_type="sampling",
         eval_tours=None,
         **unused_kwargs,
     ):
         if len(unused_kwargs) > 0:
             log.info(f"Unused kwargs for {self.__class__.__name__}: {unused_kwargs}")
@@ -75,15 +76,15 @@
             self.embedding,
         ).view(graph_size, batch_size, -1)
 
         # query the actor net for the input indices
         # making up the output, and the pointer attn
         _log_p, actions = self._inner(embedded_inputs, decode_type, eval_tours)
 
-        reward = self.env.get_reward(td, actions)
+        reward = env.get_reward(td, actions)
 
         # Log likelyhood is calculated within the model since returning it per action does not work well with
         # DataParallel since sequences can be of different lengths
         ll = get_log_likelihood(_log_p, actions, td.get("mask", None))
 
         out = {"reward": reward, "log_likelihood": ll, "actions": actions}
         return out
```

### Comparing `rl4co-0.0.6/rl4co/models/zoo/symnco/decoder.py` & `rl4co-0.1.0/rl4co/models/zoo/common/autoregressive/decoder.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,105 +1,153 @@
 from dataclasses import dataclass
+from typing import Tuple, Union
 
 import torch
 import torch.nn as nn
 
 from einops import rearrange
+from tensordict import TensorDict
+from torch import Tensor
 
+from rl4co.envs import RL4COEnvBase, get_env
 from rl4co.models.nn.attention import LogitAttention
 from rl4co.models.nn.env_embeddings import env_context_embedding, env_dynamic_embedding
 from rl4co.models.nn.utils import decode_probs
-from rl4co.utils import get_pylogger
 from rl4co.utils.ops import batchify, select_start_nodes, unbatchify
 
-log = get_pylogger(__name__)
-
 
 @dataclass
 class PrecomputedCache:
-    node_embeddings: torch.Tensor
-    graph_context: torch.Tensor
-    glimpse_key: torch.Tensor
-    glimpse_val: torch.Tensor
-    logit_key: torch.Tensor
-
+    node_embeddings: Tensor
+    graph_context: Union[Tensor, float]
+    glimpse_key: Tensor
+    glimpse_val: Tensor
+    logit_key: Tensor
+
+
+class AutoregressiveDecoder(nn.Module):
+    """Auto-regressive decoder for constructing solutions for combinatorial optimization problems.
+    Given the environment state and the embeddings, compute the logits and sample actions autoregressively until
+    all the environments in the batch have reached a terminal state.
+    We additionally include support for multi-starts as it is more efficient to do so in the decoder as we can
+    natively perform the attention computation.
+
+    Note:
+        There are major differences between this decoding and most RL problems. The most important one is
+        that reward is not defined for partial solutions, hence we have to wait for the environment to reach a terminal
+        state before we can compute the reward with `env.get_reward()`.
+
+    Warning:
+        We suppose environments in the `done` state are still available for sampling. This is because in NCO we need to
+        wait for all the environments to reach a terminal state before we can stop the decoding process. This is in
+        contrast with the TorchRL framework (at the moment) where the `env.rollout` function automatically resets.
+        You may follow tighter integration with TorchRL here: https://github.com/kaist-silab/rl4co/issues/72.
+
+    Args:
+        env_name: environment name to solve
+        embedding_dim: Dimension of the embeddings
+        num_heads: Number of heads for the attention
+        use_graph_context: Whether to use the initial graph context to modify the query
+    """
 
-class Decoder(nn.Module):
     def __init__(
         self,
-        env,
-        embedding_dim,
-        num_heads,
-        num_starts=20,
-        use_graph_context=True,
+        env_name: str,
+        embedding_dim: int,
+        num_heads: int,
+        use_graph_context: bool = True,
         **logit_attn_kwargs,
     ):
-        super(Decoder, self).__init__()
+        super().__init__()
 
-        self.env = env
+        self.env_name = env_name
         self.embedding_dim = embedding_dim
         self.num_heads = num_heads
 
         assert embedding_dim % num_heads == 0
 
-        self.context = env_context_embedding(
-            self.env.name, {"embedding_dim": embedding_dim}
+        self.context_embedding = env_context_embedding(
+            self.env_name, {"embedding_dim": embedding_dim}
         )
         self.dynamic_embedding = env_dynamic_embedding(
-            self.env.name, {"embedding_dim": embedding_dim}
+            self.env_name, {"embedding_dim": embedding_dim}
         )
+        self.use_graph_context = use_graph_context
 
         # For each node we compute (glimpse key, glimpse value, logit key) so 3 * embedding_dim
         self.project_node_embeddings = nn.Linear(
             embedding_dim, 3 * embedding_dim, bias=False
         )
         self.project_fixed_context = nn.Linear(embedding_dim, embedding_dim, bias=False)
 
         # MHA
         self.logit_attention = LogitAttention(
             embedding_dim, num_heads, **logit_attn_kwargs
         )
 
-        # POMO
-        self.num_starts = num_starts  # POMO = 1 is just normal REINFORCE
-        self.use_graph_context = use_graph_context  # disabling makes it like in POMO
-
     def forward(
         self,
-        td,
-        embeddings,
-        decode_type="sampling",
-        softmax_temp=None,
-        single_traj=False,
-        num_starts=None,
-    ):
+        td: TensorDict,
+        embeddings: Tensor,
+        env: Union[str, RL4COEnvBase] = None,
+        decode_type: str = "sampling",
+        num_starts: int = None,
+        softmax_temp: float = None,
+        calc_reward: bool = True,
+    ) -> Tuple[Tensor, Tensor, TensorDict]:
+        """Forward pass of the decoder
+        Given the environment state and the pre-computed embeddings, compute the logits and sample actions
+
+        Args:
+            td: Input TensorDict containing the environment state
+            embeddings: Precomputed embeddings for the nodes
+            env: Environment to use for decoding. If None, the environment is instantiated from `env_name`. Note that
+                it is more efficient to pass an already instantiated environment each time for fine-grained control
+            decode_type: Type of decoding to use. Can be one of:
+                - "sampling": sample from the logits
+                - "greedy": take the argmax of the logits
+                - "multistart_sampling": sample as sampling, but with multi-start decoding
+                - "multistart_greedy": sample as greedy, but with multi-start decoding
+            num_starts: Number of multi-starts to use. If None, no multi-start decoding is used
+            softmax_temp: Temperature for the softmax. If None, default softmax is used from the `LogitAttention` module
+            calc_reward: Whether to calculate the reward for the decoded sequence
+
+        Returns:
+            outputs: Tensor of shape (batch_size, seq_len, num_nodes) containing the logits
+            actions: Tensor of shape (batch_size, seq_len) containing the sampled actions
+            td: TensorDict containing the environment state after decoding
+        """
+
         # Greedy multi-start decoding if num_starts > 1
-        num_starts = (
-            self.num_starts if num_starts is None else num_starts
-        )  # substitute self.num_starts with num_starts
+        num_starts = 0 if num_starts is None else num_starts
         assert not (
             "multistart" in decode_type and num_starts <= 1
         ), "Multi-start decoding requires `num_starts` > 1"
 
         # Compute keys, values for the glimpse and keys for the logits once as they can be reused in every step
-        cached_embeds = self._precompute(embeddings, num_starts=num_starts)
+        cached_embeds = self._precompute_cache(embeddings, num_starts=num_starts)
 
         # Collect outputs
         outputs = []
         actions = []
 
+        # Instantiate environment if needed
+        if isinstance(env, str):
+            env_name = self.env_name if env is None else env
+            env = get_env(env_name)
+
         # Multi-start decoding: first action is chosen by ad-hoc node selection
-        if num_starts > 1 and not single_traj or "multistart" in decode_type:
-            action = select_start_nodes(td, num_starts, self.env)
+        if num_starts > 1 or "multistart" in decode_type:
+            action = select_start_nodes(td, num_starts, env)
 
             # Expand td to batch_size * num_starts
             td = batchify(td, num_starts)
 
             td.set("action", action)
-            td = self.env.step(td)["next"]
+            td = env.step(td)["next"]
             log_p = torch.zeros_like(
                 td["action_mask"], device=td.device
             )  # first log_p is 0, so p = log_p.exp() = 1
 
             outputs.append(log_p)
             actions.append(action)
 
@@ -107,34 +155,42 @@
         while not td["done"].all():
             log_p, mask = self._get_log_p(cached_embeds, td, softmax_temp, num_starts)
 
             # Select the indices of the next nodes in the sequences, result (batch_size) long
             action = decode_probs(log_p.exp(), mask, decode_type=decode_type)
 
             td.set("action", action)
-            td = self.env.step(td)["next"]
+            td = env.step(td)["next"]
 
             # Collect output of step
             outputs.append(log_p)
             actions.append(action)
 
         outputs, actions = torch.stack(outputs, 1), torch.stack(actions, 1)
-        td.set("reward", self.env.get_reward(td, actions))
+        if calc_reward:
+            td.set("reward", env.get_reward(td, actions))
+
         return outputs, actions, td
 
-    def _precompute(self, embeddings, num_starts=0):
+    def _precompute_cache(self, embeddings: Tensor, num_starts: int = 0):
+        """Compute the cached embeddings for the attention
+
+        Args:
+            embeddings: Precomputed embeddings for the nodes
+            num_starts: Number of multi-starts to use. If 0, no multi-start decoding is used
+        """
+
         # The projection of the node embeddings for the attention is calculated once up front
         (
             glimpse_key_fixed,
             glimpse_val_fixed,
             logit_key_fixed,
         ) = self.project_node_embeddings(embeddings).chunk(3, dim=-1)
 
-        # By default, the query is modified with the graph context.
-        # In POMO, the graph context is not used
+        # Optionally disable the graph context from the initial embedding as done in POMO
         if self.use_graph_context:
             graph_context = unbatchify(
                 batchify(self.project_fixed_context(embeddings.mean(1)), num_starts),
                 num_starts,
             )
         else:
             graph_context = 0
@@ -146,21 +202,33 @@
             glimpse_key=glimpse_key_fixed,
             glimpse_val=glimpse_val_fixed,
             logit_key=logit_key_fixed,
         )
 
         return cached_embeds
 
-    def _get_log_p(self, cached, td, softmax_temp=None, num_starts=0):
-        # Compute the query based on the context (computes automatically the first and last node context)
+    def _get_log_p(
+        self,
+        cached: PrecomputedCache,
+        td: TensorDict,
+        softmax_temp: float = None,
+        num_starts: int = 0,
+    ):
+        """Compute the log probabilities of the next actions given the current state
+
+        Args:
+            cache: Precomputed embeddings
+            td: TensorDict with the current environment state
+            softmax_temp: Temperature for the softmax
+            num_starts: Number of starts for the multi-start decoding
+        """
 
         # Unbatchify to [batch_size, num_starts, ...]. Has no effect if num_starts = 0
         td_unbatch = unbatchify(td, num_starts)
-
-        step_context = self.context(cached.node_embeddings, td_unbatch)
+        step_context = self.context_embedding(cached.node_embeddings, td_unbatch)
         glimpse_q = step_context + cached.graph_context
         glimpse_q = glimpse_q.unsqueeze(1) if glimpse_q.ndim == 2 else glimpse_q
 
         # Compute keys and values for the nodes
         (
             glimpse_key_dynamic,
             glimpse_val_dynamic,
```

### Comparing `rl4co-0.0.6/rl4co/models/zoo/symnco/losses.py` & `rl4co-0.1.0/rl4co/models/zoo/symnco/losses.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.6/rl4co/models/zoo/symnco/model.py` & `rl4co-0.1.0/rl4co/models/zoo/symnco/model.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,135 +1,133 @@
-from tensordict import TensorDict
+from typing import Any
 
-from rl4co.models.rl.reinforce.base import REINFORCE
-from rl4co.models.rl.reinforce.baselines import NoBaseline
-from rl4co.models.zoo.symnco.augmentations import StateAugmentation
+from rl4co.data.transforms import StateAugmentation
+from rl4co.envs.common.base import RL4COEnvBase
+from rl4co.models.rl.reinforce.reinforce import REINFORCE
 from rl4co.models.zoo.symnco.losses import (
     invariance_loss,
     problem_symmetricity_loss,
     solution_symmetricity_loss,
 )
 from rl4co.models.zoo.symnco.policy import SymNCOPolicy
 from rl4co.utils.ops import gather_by_index, unbatchify
 from rl4co.utils.pylogger import get_pylogger
 
 log = get_pylogger(__name__)
 
 
 class SymNCO(REINFORCE):
-    """SymNCO Model for neural combinatorial optimization based on REINFORCE
-    Based on Kim et al. (2022) https://arxiv.org/abs/2205.13209
+    """SymNCO Model for neural combinatorial optimization based on REINFORCE with shared baselines
+    based on Kim et al. (2022) https://arxiv.org/abs/2205.13209
+
 
     Args:
-        env: TorchRL Environment
-        policy: Policy
-        baseline: REINFORCE Baseline
-        num_augment: Number of augmentations (default: 8)
+        env: Environment to use for the algorithm
+        policy: Policy to use for the algorithm
+        policy_kwargs: Keyword arguments for policy
+        num_starts: Number of starts
+        num_augment: Number of augmentations
         alpha: weight for invariance loss
         beta: weight for solution symmetricity loss
-        augment_test: whether to augment data during testing as well
+        **kwargs: Keyword arguments passed to the superclass
     """
 
     def __init__(
         self,
-        env,
-        policy=None,
-        baseline=None,
-        num_starts=10,
-        num_augment=4,
-        alpha=0.2,
-        beta=1,
-        augment_test=True,
-        **policy_kwargs,
+        env: RL4COEnvBase,
+        policy: SymNCOPolicy = None,
+        policy_kwargs={},
+        num_augment: int = 4,
+        num_starts: int = 1,
+        alpha: float = 0.2,
+        beta: float = 1,
+        **kwargs,
     ):
-        super(SymNCO, self).__init__(env, policy, baseline)
+        self.save_hyperparameters(logger=False)
+
+        if policy is None:
+            policy = SymNCOPolicy(env.name, **policy_kwargs)
 
-        self.policy = (
-            SymNCOPolicy(self.env, num_starts=num_starts, **policy_kwargs)
-            if policy is None
-            else policy
-        )
-        if baseline is not None:
-            log.warn(
-                "SymNCO uses shared baselines in the loss functions. Baseline argument will be ignored"
-            )
-        self.baseline = NoBaseline()  # baseline is calculated in the loss function
+        # Pass no baseline to superclass since there are multiple custom baselines
+        super().__init__(env, policy, "no", **kwargs)
 
-        # Multi-start parameters from policy, default to 1
+        self.num_starts = num_starts
         self.num_augment = num_augment
-        self.augment = StateAugmentation(self.env.name)
-        self.augment_test = augment_test
+        self.augment = StateAugmentation(self.env.name, num_augment=self.num_augment)
         self.alpha = alpha  # weight for invariance loss
         self.beta = beta  # weight for solution symmetricity loss
 
-    def forward(self, td: TensorDict, phase: str = "train", extra=None, **policy_kwargs):
-        """Evaluate model, get costs and log probabilities and compare with baseline"""
-
-        # Get num_starts from policy. If single_traj, set num_starts and num_augment to 0
-        num_starts = getattr(self.policy.decoder, "num_starts", 0)
-        num_augment = self.num_augment
-
-        if policy_kwargs.get("single_traj", False):
-            num_starts, num_augment = 0, 0
+        # Add `_multistart` to decode type for train, val and test in policy if num_starts > 1
+        if self.num_starts > 1:
+            for phase in ["train", "val", "test"]:
+                attribute = f"{phase}_decode_type"
+                attr_get = getattr(self.policy, attribute)
+                # If does not exist, log error
+                if attr_get is None:
+                    log.error(
+                        f"Decode type for {phase} is None. Cannot add `_multistart`."
+                    )
+                    continue
+                elif "multistart" in attr_get:
+                    continue
+                else:
+                    setattr(self.policy, attribute, f"{attr_get}_multistart")
+
+    def shared_step(self, batch: Any, batch_idx: int, phase: str):
+        n_aug, n_start = self.num_augment, self.num_starts
+        td = self.env.reset(batch)
+        out = self.policy(td, self.env, phase=phase, num_starts=n_start)
+
+        # Run augmentation
+        if n_aug > 1:
+            td = self.augment(td)
 
-        if num_augment > 1:
-            td = self.augment(td, num_augment)
-
-        # Evaluate model, get costs and log probabilities
-        out = self.policy(td, phase, **policy_kwargs)
-
-        # Unbatchify reward to [batch_size, num_starts, num_augment].
-        reward = unbatchify(out["reward"], (num_starts, num_augment))
+        # Unbatchify reward to [batch_size, n_start, n_aug].
+        reward = unbatchify(out["reward"], (n_start, n_aug))
 
         # Get multi-start (=POMO) rewards and best actions
-        if num_starts > 1:
+        if n_start > 1:
             # max multi-start reward
             max_reward, max_idxs = reward.max(dim=1)
             out.update({"max_reward": max_reward})
 
-            # Reshape batch to [batch, num_starts, num_augment]
+            # Reshape batch to [batch, n_start, n_aug]
             if out.get("actions", None) is not None:
                 # TODO: actions are not unbatchified correctly
-                actions = unbatchify(out["actions"], (num_starts, num_augment))
+                actions = unbatchify(out["actions"], (n_start, n_aug))
                 out.update(
                     {"best_multistart_actions": gather_by_index(actions, max_idxs)}
                 )
                 out["actions"] = actions
 
         # Get augmentation score only during inference
-        if num_augment > 1:
+        if n_aug > 1:
             # If multistart is enabled, we use the best multistart rewards
-            reward_ = max_reward if num_starts > 1 else reward
-            # [batch, num_augment]
+            reward_ = max_reward if n_start > 1 else reward
+            # [batch, n_aug]
             max_aug_reward, max_idxs = reward_.max(dim=1)
             out.update({"max_aug_reward": max_aug_reward})
             if out.get("best_multistart_actions", None) is not None:
                 out.update(
                     {
                         "best_aug_actions": gather_by_index(
                             out["best_multistart_actions"], max_idxs
                         )
                     }
                 )
 
-        # Get best actions and rewards
         # Main training loss
         if phase == "train":
-            # [batch_size, num_starts, num_augment]
-            ll = unbatchify(out["log_likelihood"], (num_starts, num_augment))
+            # [batch_size, n_start, n_aug]
+            ll = unbatchify(out["log_likelihood"], (n_start, n_aug))
 
             # Calculate losses: problem symmetricity, solution symmetricity, invariance
-
-            loss_ps = problem_symmetricity_loss(reward, ll) if num_starts > 1 else 0
-            loss_ss = solution_symmetricity_loss(reward, ll) if num_augment > 1 else 0
-            loss_inv = (
-                invariance_loss(out["proj_embeddings"], num_augment)
-                if num_augment > 1
-                else 0
-            )
+            loss_ps = problem_symmetricity_loss(reward, ll) if n_start > 1 else 0
+            loss_ss = solution_symmetricity_loss(reward, ll) if n_aug > 1 else 0
+            loss_inv = invariance_loss(out["proj_embeddings"], n_aug) if n_aug > 1 else 0
             loss = loss_ps + self.beta * loss_ss + self.alpha * loss_inv
             out.update(
                 {
                     "loss": loss,
                     "loss_ss": loss_ss,
                     "loss_ps": loss_ps,
                     "loss_inv": loss_inv,
```

### Comparing `rl4co-0.0.6/rl4co/tasks/eval.py` & `rl4co-0.1.0/rl4co/tasks/eval.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.6/rl4co/utils/callbacks/speed_monitor.py` & `rl4co-0.1.0/rl4co/utils/callbacks/speed_monitor.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.6/rl4co/utils/download/downloader.py` & `rl4co-0.1.0/rl4co/utils/download/downloader.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.6/rl4co/utils/download/gdrive.py` & `rl4co-0.1.0/rl4co/utils/download/gdrive.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.6/rl4co/utils/download/s3.py` & `rl4co-0.1.0/rl4co/utils/download/s3.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.6/rl4co/utils/instantiators.py` & `rl4co-0.1.0/rl4co/utils/instantiators.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.6/rl4co/utils/ops.py` & `rl4co-0.1.0/rl4co/utils/ops.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,25 +90,25 @@
     Args:
         ordered_locs: Tensor of shape [batch_size, num_nodes, 2] containing the ordered locations of the tour
     """
     ordered_locs_next = torch.roll(ordered_locs, 1, dims=-2)
     return get_distance(ordered_locs_next, ordered_locs).sum(-1)
 
 
-def select_start_nodes(td, num_nodes, env=None):
+def select_start_nodes(td, num_nodes, env):
     """Node selection strategy as proposed in POMO (Kwon et al. 2020)
     and extended in SymNCO (Kim et al. 2022).
     Selects different start nodes for each batch element
 
     Args:
         td: TensorDict containing the data. We may need to access the available actions to select the start nodes
         num_nodes: Number of nodes to select
         env: (TODO) Environment may determine the node selection strategy
     """
-    if env.name != "pctsp":
+    if env.name not in ["pctsp", "spctsp", "mtsp"]:
         selected = torch.arange(num_nodes, device=td.device).repeat_interleave(
             td.shape[0]
         )
     else:
         selected = torch.arange(1, num_nodes + 1, device=td.device).repeat_interleave(
             td.shape[0]
         )
```

### Comparing `rl4co-0.0.6/rl4co/utils/param_grouping.py` & `rl4co-0.1.0/rl4co/utils/param_grouping.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.6/rl4co/utils/pylogger.py` & `rl4co-0.1.0/rl4co/utils/pylogger.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.6/rl4co/utils/rich_utils.py` & `rl4co-0.1.0/rl4co/utils/rich_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 log = pylogger.get_pylogger(__name__)
 
 
 @rank_zero_only
 def print_config_tree(
     cfg: DictConfig,
     print_order: Sequence[str] = (
-        "data",
+        # "data", # note: data is dealt with in model
         "model",
         "callbacks",
         "logger",
         "trainer",
         "paths",
         "extras",
     ),
```

### Comparing `rl4co-0.0.6/rl4co/utils/test_utils.py` & `rl4co-0.1.0/rl4co/utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.6/rl4co/utils/transfer.py` & `rl4co-0.1.0/rl4co/utils/transfer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import torch.nn as nn
 
 
-def transplant_weights(
+# Work in progress on transfer learning between models
+def transfer_learning_weights(
     source: nn.Module,
     target: nn.Module,
     load_encoder: bool = True,
     load_decoder: bool = True,
     reset_norms: bool = True,
     freeze_encoder: bool = True,
 ):
```

### Comparing `rl4co-0.0.6/rl4co/utils/utils.py` & `rl4co-0.1.0/rl4co/utils/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -150,15 +150,17 @@
     hparams["model/params/trainable"] = sum(
         p.numel() for p in model.parameters() if p.requires_grad
     )
     hparams["model/params/non_trainable"] = sum(
         p.numel() for p in model.parameters() if not p.requires_grad
     )
 
-    hparams["data"] = cfg["data"]
+    ## Note: we do not use the data config, since it is dealt with in the model
+    ## which is a `LightningModule`
+    # hparams["data"] = cfg["data"]
     hparams["trainer"] = cfg["trainer"]
 
     hparams["callbacks"] = cfg.get("callbacks")
     hparams["extras"] = cfg.get("extras")
 
     hparams["task_name"] = cfg.get("task_name")
     hparams["tags"] = cfg.get("tags")
```

### Comparing `rl4co-0.0.6/rl4co.egg-info/PKG-INFO` & `rl4co-0.1.0/rl4co.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rl4co
-Version: 0.0.6
+Version: 0.1.0
 Summary: RL4CO: an Extensive Reinforcement Learning for Combinatorial Optimization Benchmark
 Author-email: Federico Berto <berto.federico2@gmail.com>, Chuanbo Hua <cbhua@kaist.ac.kr>, Junyoung Park <junyoungpark.ml@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -214,27 +214,28 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: graph
 Provides-Extra: testing
-Provides-Extra: linting
+Provides-Extra: dev
 License-File: LICENSE
 
 <div align="center">
 
-# RL4CO
+<img src="https://github.com/kaist-silab/rl4co/assets/34462374/249462ea-b15d-4358-8a11-6508903dae58" style="width:40%">
+</br></br>
 
 
 <a href="https://pytorch.org/get-started/locally/"><img alt="PyTorch" src="https://img.shields.io/badge/PyTorch-ee4c2c?logo=pytorch&logoColor=white"></a>
 <a href="https://pytorchlightning.ai/"><img alt="Lightning" src="https://img.shields.io/badge/-Lightning-792ee5?logo=pytorchlightning&logoColor=white"></a>
 <a href="https://github.com/pytorch/rl"><img alt="base: TorchRL" src="https://img.shields.io/badge/base-TorchRL-red">
-<a href="https://hydra.cc/"><img alt="config: Hydra" src="https://img.shields.io/badge/config-Hydra-89b8cd"></a> [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)[![Slack](https://img.shields.io/badge/slack-chat-611f69.svg?logo=slack)](https://join.slack.com/t/rl4co/shared_invite/zt-1ytz2c1v4-0IkQ8NQH4TRXIX8PrRmDhQ)
-![license](https://img.shields.io/badge/license-Apache%202.0-green.svg?)<a href="https://colab.research.google.com/github/kaist-silab/rl4co/blob/main/notebooks/1-quickstart.ipynb"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"></a>[![PyPI](https://img.shields.io/pypi/v/rl4co?logo=pypi)](https://pypi.org/project/rl4co)
+<a href="https://hydra.cc/"><img alt="config: Hydra" src="https://img.shields.io/badge/config-Hydra-89b8cd"></a> [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![Slack](https://img.shields.io/badge/slack-chat-611f69.svg?logo=slack)](https://join.slack.com/t/rl4co/shared_invite/zt-1ytz2c1v4-0IkQ8NQH4TRXIX8PrRmDhQ)
+![license](https://img.shields.io/badge/license-Apache%202.0-green.svg?) <a href="https://colab.research.google.com/github/kaist-silab/rl4co/blob/main/notebooks/1-quickstart.ipynb"> <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"></a> [![PyPI](https://img.shields.io/pypi/v/rl4co?logo=pypi)](https://pypi.org/project/rl4co)
 [![Test](https://github.com/kaist-silab/rl4co/actions/workflows/tests.yml/badge.svg)](https://github.com/kaist-silab/rl4co/actions/workflows/tests.yml)
 <!-- ![testing](https://github.com/kaist-silab/ncobench/actions/workflows/tests.yml/badge.svg) -->
 
 [**Documentation**](https://rl4co.readthedocs.io/) |  [**Getting Started**](#getting-started) | [**Usage**](#usage) | [**Contributing**](#contributing) | [**Paper**](https://arxiv.org/abs/2306.17100) | [**Citation**](#cite-us)
 
 </div>
 
@@ -246,16 +247,15 @@
 
 RL4CO is built upon:
 - [TorchRL](https://github.com/pytorch/rl): official PyTorch framework for RL algorithms and vectorized environments on GPUs
 - [TensorDict](https://github.com/pytorch-labs/tensordict): a library to easily handle heterogeneous data such as states, actions and rewards
 - [PyTorch Lightning](https://github.com/Lightning-AI/lightning): a lightweight PyTorch wrapper for high-performance AI research
 - [Hydra](https://github.com/facebookresearch/hydra): a framework for elegantly configuring complex applications
 
-![image](https://github.com/kaist-silab/rl4co/assets/48984123/0db4efdd-1c93-4991-8f09-f3c6c1f35d60)
-
+![RL4CO Overview](https://github.com/kaist-silab/rl4co/assets/34462374/4d9a670f-ab7c-4fc8-9135-82d17cb6d0ee)
 
 ## Getting started
 <a href="https://colab.research.google.com/github/kaist-silab/rl4co/blob/main/notebooks/1-quickstart.ipynb"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"></a>
 
 RL4CO is now available for installation on `pip`!
 ```bash
 pip install rl4co
@@ -325,49 +325,38 @@
 ```
 </details>
 
 
 
 ### Minimalistic Example
 
-Here is a minimalistic example training the Attention Model with greedy rollout baseline on TSP in less than 50 lines of code:
+Here is a minimalistic example training the Attention Model with greedy rollout baseline on TSP in less than 30 lines of code:
 
 ```python
-from omegaconf import DictConfig
-import lightning as L
 from rl4co.envs import TSPEnv
-from rl4co.models.zoo.am import AttentionModel
-from rl4co.tasks.rl4co import RL4COLitModule
-
-config = DictConfig(
-    {"data": {
-            "train_size": 100000,
-            "val_size": 10000,
-            "batch_size": 512,
-        },
-    "optimizer": {"lr": 1e-4}}
-)
+from rl4co.models import AttentionModel
+from rl4co.utils import RL4COTrainer
 
 # Environment, Model, and Lightning Module
 env = TSPEnv(num_loc=20)
-model = AttentionModel(env)
-lit_module = RL4COLitModule(config, env, model)
+model = AttentionModel(env,
+                       baseline="rollout",
+                       train_data_size=100_000,
+                       test_data_size=10_000,
+                       optimizer_kwargs={'lr': 1e-4}
+                       )
 
 # Trainer
-trainer = L.Trainer(
-    max_epochs=3, # only few epochs
-    accelerator="gpu", # use GPU if available, else you can use others as "cpu"
-    logger=None, # can replace with WandbLogger, TensorBoardLogger, etc.
-    precision="16-mixed", # Lightning will handle faster training with mixed precision
-    gradient_clip_val=1.0, # clip gradients to avoid exploding gradients
-    reload_dataloaders_every_n_epochs=1, # necessary for sampling new data
-)
+trainer = RL4COTrainer(max_epochs=3)
 
 # Fit the model
-trainer.fit(lit_module)
+trainer.fit(model)
+
+# Test the model
+trainer.test(model)
 ```
 
 
 ### Testing
 
 Run tests with `pytest` from the root directory:
```

### Comparing `rl4co-0.0.6/rl4co.egg-info/SOURCES.txt` & `rl4co-0.1.0/rl4co.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -6,21 +6,23 @@
 rl4co.egg-info/SOURCES.txt
 rl4co.egg-info/dependency_links.txt
 rl4co.egg-info/requires.txt
 rl4co.egg-info/top_level.txt
 rl4co/data/__init__.py
 rl4co/data/dataset.py
 rl4co/data/generate_data.py
+rl4co/data/transforms.py
 rl4co/data/utils.py
 rl4co/envs/__init__.py
 rl4co/envs/atsp.py
 rl4co/envs/cvrp.py
 rl4co/envs/dpp.py
 rl4co/envs/ffsp.py
 rl4co/envs/mdpp.py
+rl4co/envs/mpdp.py
 rl4co/envs/mtsp.py
 rl4co/envs/op.py
 rl4co/envs/pctsp.py
 rl4co/envs/pdp.py
 rl4co/envs/sdvrp.py
 rl4co/envs/spctsp.py
 rl4co/envs/tsp.py
@@ -32,29 +34,33 @@
 rl4co/models/nn/mlp.py
 rl4co/models/nn/ops.py
 rl4co/models/nn/utils.py
 rl4co/models/nn/env_embeddings/__init__.py
 rl4co/models/nn/env_embeddings/context.py
 rl4co/models/nn/env_embeddings/dynamic.py
 rl4co/models/nn/env_embeddings/init.py
-rl4co/models/nn/graph/gat.py
+rl4co/models/nn/graph/attnnet.py
 rl4co/models/nn/graph/gcn.py
 rl4co/models/nn/graph/mpnn.py
-rl4co/models/rl/ppo/model.py
-rl4co/models/rl/ppo/task.py
-rl4co/models/rl/reinforce/base.py
+rl4co/models/rl/__init__.py
+rl4co/models/rl/common/base.py
+rl4co/models/rl/common/critic.py
+rl4co/models/rl/ppo/ppo.py
 rl4co/models/rl/reinforce/baselines.py
-rl4co/models/rl/reinforce/critic.py
+rl4co/models/rl/reinforce/reinforce.py
 rl4co/models/zoo/am/__init__.py
-rl4co/models/zoo/am/decoder.py
 rl4co/models/zoo/am/model.py
 rl4co/models/zoo/am/policy.py
-rl4co/models/zoo/amppo/decoder.py
-rl4co/models/zoo/amppo/model.py
-rl4co/models/zoo/amppo/policy.py
+rl4co/models/zoo/common/autoregressive/__init__.py
+rl4co/models/zoo/common/autoregressive/decoder.py
+rl4co/models/zoo/common/autoregressive/encoder.py
+rl4co/models/zoo/common/autoregressive/policy.py
+rl4co/models/zoo/et/model.py
+rl4co/models/zoo/et/policy.py
+rl4co/models/zoo/et/positional_encoding.py
 rl4co/models/zoo/ham/__init__.py
 rl4co/models/zoo/ham/attention.py
 rl4co/models/zoo/ham/encoder.py
 rl4co/models/zoo/ham/model.py
 rl4co/models/zoo/ham/policy.py
 rl4co/models/zoo/mdam/__init__.py
 rl4co/models/zoo/mdam/decoder.py
@@ -62,41 +68,46 @@
 rl4co/models/zoo/mdam/model.py
 rl4co/models/zoo/mdam/policy.py
 rl4co/models/zoo/pomo/__init__.py
 rl4co/models/zoo/pomo/augmentations.py
 rl4co/models/zoo/pomo/decoder.py
 rl4co/models/zoo/pomo/model.py
 rl4co/models/zoo/pomo/policy.py
+rl4co/models/zoo/ppo/__init__.py
+rl4co/models/zoo/ppo/decoder.py
+rl4co/models/zoo/ppo/model.py
+rl4co/models/zoo/ppo/policy.py
 rl4co/models/zoo/ptrnet/__init__.py
 rl4co/models/zoo/ptrnet/critic.py
 rl4co/models/zoo/ptrnet/decoder.py
 rl4co/models/zoo/ptrnet/encoder.py
 rl4co/models/zoo/ptrnet/model.py
 rl4co/models/zoo/ptrnet/policy.py
 rl4co/models/zoo/symnco/__init__.py
-rl4co/models/zoo/symnco/augmentations.py
-rl4co/models/zoo/symnco/decoder.py
 rl4co/models/zoo/symnco/losses.py
 rl4co/models/zoo/symnco/model.py
 rl4co/models/zoo/symnco/policy.py
+rl4co/tasks/__init__.py
 rl4co/tasks/eval.py
-rl4co/tasks/rl4co.py
+rl4co/tasks/train.py
 rl4co/utils/__init__.py
-rl4co/utils/helpers.py
 rl4co/utils/instantiators.py
 rl4co/utils/lightning.py
-rl4co/utils/logging_utils.py
 rl4co/utils/ops.py
+rl4co/utils/optim_helpers.py
 rl4co/utils/param_grouping.py
 rl4co/utils/pylogger.py
 rl4co/utils/rich_utils.py
 rl4co/utils/test_utils.py
+rl4co/utils/trainer.py
 rl4co/utils/transfer.py
 rl4co/utils/utils.py
 rl4co/utils/callbacks/speed_monitor.py
 rl4co/utils/download/constants.py
 rl4co/utils/download/downloader.py
 rl4co/utils/download/gdrive.py
 rl4co/utils/download/s3.py
 tests/test_envs.py
-tests/test_models.py
-tests/test_ops.py
+tests/test_policy.py
+tests/test_tasks.py
+tests/test_training.py
+tests/test_utils.py
```

### Comparing `rl4co-0.0.6/tests/test_ops.py` & `rl4co-0.1.0/tests/test_utils.py`

 * *Files identical despite different names*

