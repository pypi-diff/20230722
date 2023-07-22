# Comparing `tmp/swarms-1.0.6.tar.gz` & `tmp/swarms-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swarms-1.0.6.tar", last modified: Sat Jul 22 19:17:58 2023, max compression
+gzip compressed data, was "swarms-1.9.0.tar", last modified: Sat Jul 22 15:53:41 2023, max compression
```

## Comparing `swarms-1.0.6.tar` & `swarms-1.9.0.tar`

### file list

```diff
@@ -1,152 +1,149 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 19:17:58.786649 swarms-1.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-22 19:17:45.000000 swarms-1.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-22 19:17:58.786649 swarms-1.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15283 2023-07-22 19:17:45.000000 swarms-1.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 19:17:58.770649 swarms-1.0.6/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 19:17:45.000000 swarms-1.0.6/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-07-22 19:17:45.000000 swarms-1.0.6/api/app.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-22 19:17:58.786649 swarms-1.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-07-22 19:17:45.000000 swarms-1.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 19:17:58.770649 swarms-1.0.6/swarms/
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-22 19:17:45.000000 swarms-1.0.6/swarms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 19:17:58.774649 swarms-1.0.6/swarms/agents/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-22 19:17:45.000000 swarms-1.0.6/swarms/agents/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 19:17:58.774649 swarms-1.0.6/swarms/agents/memory/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 19:17:45.000000 swarms-1.0.6/swarms/agents/memory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18115 2023-07-22 19:17:45.000000 swarms-1.0.6/swarms/agents/memory/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    22333 2023-07-22 19:17:45.000000 swarms-1.0.6/swarms/agents/memory/chroma.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 19:17:58.774649 swarms-1.0.6/swarms/agents/models/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-22 19:17:45.000000 swarms-1.0.6/swarms/agents/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-07-22 19:17:45.000000 swarms-1.0.6/swarms/agents/models/llm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 19:17:58.774649 swarms-1.0.6/swarms/agents/prompts/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-22 19:17:45.000000 swarms-1.0.6/swarms/agents/prompts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 19:17:58.774649 swarms-1.0.6/swarms/agents/prompts/chains/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 19:17:45.000000 swarms-1.0.6/swarms/agents/prompts/chains/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12136 2023-07-22 19:17:45.000000 swarms-1.0.6/swarms/agents/prompts/chains/llm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-07-22 19:17:45.000000 swarms-1.0.6/swarms/agents/prompts/prompts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 19:17:58.774649 swarms-1.0.6/swarms/agents/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-22 19:17:45.000000 swarms-1.0.6/swarms/agents/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-07-22 19:17:45.000000 swarms-1.0.6/swarms/agents/tools/agent_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-07-22 19:17:45.000000 swarms-1.0.6/swarms/agents/tools/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 19:17:58.774649 swarms-1.0.6/swarms/agents/tools/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 19:17:45.000000 swarms-1.0.6/swarms/agents/tools/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 19:17:58.774649 swarms-1.0.6/swarms/agents/tools/core/code_interpreter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 19:17:45.000000 swarms-1.0.6/swarms/agents/tools/core/code_interpreter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27478 2023-07-22 19:17:45.000000 swarms-1.0.6/swarms/agents/tools/core/code_interpreter/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    73698 2023-07-22 19:17:45.000000 swarms-1.0.6/swarms/agents/tools/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 19:17:58.774649 swarms-1.0.6/swarms/agents/utils/
--rw-r--r--   0 runner    (1001) docker     (123)    19599 2023-07-22 19:17:45.000000 swarms-1.0.6/swarms/agents/utils/Agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     6022 2023-07-22 19:17:45.000000 swarms-1.0.6/swarms/agents/utils/Calback.py
--rw-r--r--   0 runner    (1001) docker     (123)    13661 2023-07-22 19:17:45.000000 swarms-1.0.6/swarms/agents/utils/ChatOpenAI.py
--rw-r--r--   0 runner    (1001) docker     (123)     5529 2023-07-22 19:17:45.000000 swarms-1.0.6/swarms/agents/utils/ConversationalChatAgent.py
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-22 19:17:45.000000 swarms-1.0.6/swarms/agents/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3795 2023-07-22 19:17:45.000000 swarms-1.0.6/swarms/agents/utils/agent_creator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-07-22 19:17:45.000000 swarms-1.0.6/swarms/agents/utils/agent_setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-07-22 19:17:45.000000 swarms-1.0.6/swarms/agents/utils/output_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     6348 2023-07-22 19:17:45.000000 swarms-1.0.6/swarms/agents/utils/prompts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 19:17:58.774649 swarms-1.0.6/swarms/boss/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 19:17:45.000000 swarms-1.0.6/swarms/boss/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5834 2023-07-22 19:17:45.000000 swarms-1.0.6/swarms/boss/boss_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-07-22 19:17:45.000000 swarms-1.0.6/swarms/hivemind.py
--rw-r--r--   0 runner    (1001) docker     (123)     9763 2023-07-22 19:17:45.000000 swarms-1.0.6/swarms/swarms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 19:17:58.778649 swarms-1.0.6/swarms/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-22 19:17:45.000000 swarms-1.0.6/swarms/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 19:17:58.778649 swarms-1.0.6/swarms/utils/embeddings/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-22 19:17:45.000000 swarms-1.0.6/swarms/utils/embeddings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-22 19:17:45.000000 swarms-1.0.6/swarms/utils/embeddings/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-22 19:17:45.000000 swarms-1.0.6/swarms/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    11292 2023-07-22 19:17:45.000000 swarms-1.0.6/swarms/utils/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 19:17:58.778649 swarms-1.0.6/swarms/utils/schema/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 19:17:45.000000 swarms-1.0.6/swarms/utils/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 19:17:45.000000 swarms-1.0.6/swarms/utils/schema/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-07-22 19:17:45.000000 swarms-1.0.6/swarms/utils/static.py
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-22 19:17:45.000000 swarms-1.0.6/swarms/utils/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 19:17:58.778649 swarms-1.0.6/swarms/workers/
--rw-r--r--   0 runner    (1001) docker     (123)     6132 2023-07-22 19:17:45.000000 swarms-1.0.6/swarms/workers/WorkerNode.py
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-22 19:17:45.000000 swarms-1.0.6/swarms/workers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10799 2023-07-22 19:17:45.000000 swarms-1.0.6/swarms/workers/character_generative.py
--rw-r--r--   0 runner    (1001) docker     (123)    22410 2023-07-22 19:17:45.000000 swarms-1.0.6/swarms/workers/generative_worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 19:17:58.778649 swarms-1.0.6/swarms/workers/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 19:17:58.778649 swarms-1.0.6/swarms/workers/models/GroundingDINO/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-22 19:17:45.000000 swarms-1.0.6/swarms/workers/models/GroundingDINO/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 19:17:58.778649 swarms-1.0.6/swarms/workers/models/GroundingDINO/groundingdino/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 19:17:46.000000 swarms-1.0.6/swarms/workers/models/GroundingDINO/groundingdino/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 19:17:58.778649 swarms-1.0.6/swarms/workers/models/GroundingDINO/groundingdino/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-07-22 19:17:46.000000 swarms-1.0.6/swarms/workers/models/GroundingDINO/groundingdino/config/GroundingDINO_SwinB_cfg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-22 19:17:46.000000 swarms-1.0.6/swarms/workers/models/GroundingDINO/groundingdino/config/GroundingDINO_SwinT_OGC.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 19:17:46.000000 swarms-1.0.6/swarms/workers/models/GroundingDINO/groundingdino/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 19:17:58.778649 swarms-1.0.6/swarms/workers/models/GroundingDINO/groundingdino/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 19:17:46.000000 swarms-1.0.6/swarms/workers/models/GroundingDINO/groundingdino/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9398 2023-07-22 19:17:46.000000 swarms-1.0.6/swarms/workers/models/GroundingDINO/groundingdino/datasets/cocogrounding_eval.py
--rw-r--r--   0 runner    (1001) docker     (123)     9711 2023-07-22 19:17:46.000000 swarms-1.0.6/swarms/workers/models/GroundingDINO/groundingdino/datasets/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 19:17:58.778649 swarms-1.0.6/swarms/workers/models/GroundingDINO/groundingdino/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 19:17:58.782649 swarms-1.0.6/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-07-22 19:17:46.000000 swarms-1.0.6/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 19:17:58.782649 swarms-1.0.6/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-22 19:17:46.000000 swarms-1.0.6/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7972 2023-07-22 19:17:46.000000 swarms-1.0.6/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/backbone.py
--rw-r--r--   0 runner    (1001) docker     (123)     6866 2023-07-22 19:17:46.000000 swarms-1.0.6/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/position_encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)    29339 2023-07-22 19:17:46.000000 swarms-1.0.6/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/swin_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    12242 2023-07-22 19:17:46.000000 swarms-1.0.6/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/bertwarper.py
--rw-r--r--   0 runner    (1001) docker     (123)    11825 2023-07-22 19:17:46.000000 swarms-1.0.6/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/fuse_modules.py
--rw-r--r--   0 runner    (1001) docker     (123)    16669 2023-07-22 19:17:46.000000 swarms-1.0.6/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/groundingdino.py
--rw-r--r--   0 runner    (1001) docker     (123)    15482 2023-07-22 19:17:46.000000 swarms-1.0.6/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/ms_deform_attn.py
--rw-r--r--   0 runner    (1001) docker     (123)    36805 2023-07-22 19:17:46.000000 swarms-1.0.6/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4020 2023-07-22 19:17:46.000000 swarms-1.0.6/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/transformer_vanilla.py
--rw-r--r--   0 runner    (1001) docker     (123)    10087 2023-07-22 19:17:46.000000 swarms-1.0.6/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-07-22 19:17:46.000000 swarms-1.0.6/swarms/workers/models/GroundingDINO/groundingdino/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-07-22 19:17:46.000000 swarms-1.0.6/swarms/workers/models/GroundingDINO/groundingdino/models/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 19:17:58.782649 swarms-1.0.6/swarms/workers/models/GroundingDINO/groundingdino/util/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-22 19:17:46.000000 swarms-1.0.6/swarms/workers/models/GroundingDINO/groundingdino/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-07-22 19:17:46.000000 swarms-1.0.6/swarms/workers/models/GroundingDINO/groundingdino/util/box_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-07-22 19:17:46.000000 swarms-1.0.6/swarms/workers/models/GroundingDINO/groundingdino/util/get_tokenlizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8745 2023-07-22 19:17:46.000000 swarms-1.0.6/swarms/workers/models/GroundingDINO/groundingdino/util/inference.py
--rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-07-22 19:17:46.000000 swarms-1.0.6/swarms/workers/models/GroundingDINO/groundingdino/util/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    23348 2023-07-22 19:17:46.000000 swarms-1.0.6/swarms/workers/models/GroundingDINO/groundingdino/util/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)    14380 2023-07-22 19:17:46.000000 swarms-1.0.6/swarms/workers/models/GroundingDINO/groundingdino/util/slconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     5377 2023-07-22 19:17:46.000000 swarms-1.0.6/swarms/workers/models/GroundingDINO/groundingdino/util/slio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-07-22 19:17:46.000000 swarms-1.0.6/swarms/workers/models/GroundingDINO/groundingdino/util/time_counter.py
--rw-r--r--   0 runner    (1001) docker     (123)    17828 2023-07-22 19:17:46.000000 swarms-1.0.6/swarms/workers/models/GroundingDINO/groundingdino/util/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    12047 2023-07-22 19:17:46.000000 swarms-1.0.6/swarms/workers/models/GroundingDINO/groundingdino/util/visualizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-07-22 19:17:46.000000 swarms-1.0.6/swarms/workers/models/GroundingDINO/groundingdino/util/vl_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7179 2023-07-22 19:17:46.000000 swarms-1.0.6/swarms/workers/models/GroundingDINO/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-07-22 19:17:46.000000 swarms-1.0.6/swarms/workers/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 19:17:58.782649 swarms-1.0.6/swarms/workers/models/segment_anything/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-22 19:17:46.000000 swarms-1.0.6/swarms/workers/models/segment_anything/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 19:17:58.782649 swarms-1.0.6/swarms/workers/models/segment_anything/segment_anything/
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-07-22 19:17:46.000000 swarms-1.0.6/swarms/workers/models/segment_anything/segment_anything/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15148 2023-07-22 19:17:46.000000 swarms-1.0.6/swarms/workers/models/segment_anything/segment_anything/automatic_mask_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-07-22 19:17:46.000000 swarms-1.0.6/swarms/workers/models/segment_anything/segment_anything/build_sam.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 19:17:58.782649 swarms-1.0.6/swarms/workers/models/segment_anything/segment_anything/modeling/
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-22 19:17:46.000000 swarms-1.0.6/swarms/workers/models/segment_anything/segment_anything/modeling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-07-22 19:17:46.000000 swarms-1.0.6/swarms/workers/models/segment_anything/segment_anything/modeling/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    14420 2023-07-22 19:17:46.000000 swarms-1.0.6/swarms/workers/models/segment_anything/segment_anything/modeling/image_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     6615 2023-07-22 19:17:46.000000 swarms-1.0.6/swarms/workers/models/segment_anything/segment_anything/modeling/mask_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     8594 2023-07-22 19:17:46.000000 swarms-1.0.6/swarms/workers/models/segment_anything/segment_anything/modeling/prompt_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-07-22 19:17:46.000000 swarms-1.0.6/swarms/workers/models/segment_anything/segment_anything/modeling/sam.py
--rw-r--r--   0 runner    (1001) docker     (123)     8397 2023-07-22 19:17:46.000000 swarms-1.0.6/swarms/workers/models/segment_anything/segment_anything/modeling/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11649 2023-07-22 19:17:46.000000 swarms-1.0.6/swarms/workers/models/segment_anything/segment_anything/predictor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 19:17:58.786649 swarms-1.0.6/swarms/workers/models/segment_anything/segment_anything/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-22 19:17:46.000000 swarms-1.0.6/swarms/workers/models/segment_anything/segment_anything/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12712 2023-07-22 19:17:46.000000 swarms-1.0.6/swarms/workers/models/segment_anything/segment_anything/utils/amg.py
--rw-r--r--   0 runner    (1001) docker     (123)     5812 2023-07-22 19:17:46.000000 swarms-1.0.6/swarms/workers/models/segment_anything/segment_anything/utils/onnx.py
--rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-07-22 19:17:46.000000 swarms-1.0.6/swarms/workers/models/segment_anything/segment_anything/utils/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-07-22 19:17:46.000000 swarms-1.0.6/swarms/workers/models/segment_anything/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-22 19:17:46.000000 swarms-1.0.6/swarms/workers/multi_modal_worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 19:17:58.786649 swarms-1.0.6/swarms/workers/multi_modal_workers/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-22 19:17:46.000000 swarms-1.0.6/swarms/workers/multi_modal_workers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    79542 2023-07-22 19:17:46.000000 swarms-1.0.6/swarms/workers/multi_modal_workers/multi_modal_agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 19:17:58.786649 swarms-1.0.6/swarms/workers/multi_modal_workers/omni_agent/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 19:17:46.000000 swarms-1.0.6/swarms/workers/multi_modal_workers/omni_agent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-07-22 19:17:46.000000 swarms-1.0.6/swarms/workers/multi_modal_workers/omni_agent/get_token_ids.py
--rw-r--r--   0 runner    (1001) docker     (123)    31378 2023-07-22 19:17:46.000000 swarms-1.0.6/swarms/workers/multi_modal_workers/omni_agent/model_server.py
--rw-r--r--   0 runner    (1001) docker     (123)    45875 2023-07-22 19:17:46.000000 swarms-1.0.6/swarms/workers/multi_modal_workers/omni_agent/omni_chat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-22 19:17:46.000000 swarms-1.0.6/swarms/workers/omni_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     6904 2023-07-22 19:17:46.000000 swarms-1.0.6/swarms/workers/worker_agent_ultra.py
--rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-07-22 19:17:46.000000 swarms-1.0.6/swarms/workers/worker_ultra_node.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 19:17:58.774649 swarms-1.0.6/swarms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-22 19:17:58.000000 swarms-1.0.6/swarms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5961 2023-07-22 19:17:58.000000 swarms-1.0.6/swarms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 19:17:58.000000 swarms-1.0.6/swarms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-07-22 19:17:58.000000 swarms-1.0.6/swarms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-22 19:17:58.000000 swarms-1.0.6/swarms.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 15:53:41.726630 swarms-1.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-22 15:53:28.000000 swarms-1.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-22 15:53:41.726630 swarms-1.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15283 2023-07-22 15:53:28.000000 swarms-1.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 15:53:41.702630 swarms-1.9.0/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 15:53:28.000000 swarms-1.9.0/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-07-22 15:53:28.000000 swarms-1.9.0/api/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-22 15:53:41.726630 swarms-1.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-07-22 15:53:28.000000 swarms-1.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 15:53:41.702630 swarms-1.9.0/swarms/
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-22 15:53:28.000000 swarms-1.9.0/swarms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 15:53:41.702630 swarms-1.9.0/swarms/agents/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-22 15:53:28.000000 swarms-1.9.0/swarms/agents/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 15:53:41.702630 swarms-1.9.0/swarms/agents/boss/
+-rw-r--r--   0 runner    (1001) docker     (123)     5795 2023-07-22 15:53:28.000000 swarms-1.9.0/swarms/agents/boss/BossNode.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 15:53:28.000000 swarms-1.9.0/swarms/agents/boss/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 15:53:41.702630 swarms-1.9.0/swarms/agents/memory/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 15:53:28.000000 swarms-1.9.0/swarms/agents/memory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18115 2023-07-22 15:53:28.000000 swarms-1.9.0/swarms/agents/memory/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22333 2023-07-22 15:53:28.000000 swarms-1.9.0/swarms/agents/memory/chroma.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 15:53:41.706630 swarms-1.9.0/swarms/agents/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-22 15:53:28.000000 swarms-1.9.0/swarms/agents/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-07-22 15:53:28.000000 swarms-1.9.0/swarms/agents/models/llm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 15:53:41.706630 swarms-1.9.0/swarms/agents/prompts/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-22 15:53:28.000000 swarms-1.9.0/swarms/agents/prompts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-07-22 15:53:28.000000 swarms-1.9.0/swarms/agents/prompts/prompts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 15:53:41.706630 swarms-1.9.0/swarms/agents/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-22 15:53:28.000000 swarms-1.9.0/swarms/agents/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-07-22 15:53:28.000000 swarms-1.9.0/swarms/agents/tools/agent_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-07-22 15:53:28.000000 swarms-1.9.0/swarms/agents/tools/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 15:53:41.706630 swarms-1.9.0/swarms/agents/tools/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 15:53:28.000000 swarms-1.9.0/swarms/agents/tools/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 15:53:41.706630 swarms-1.9.0/swarms/agents/tools/core/code_interpreter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 15:53:28.000000 swarms-1.9.0/swarms/agents/tools/core/code_interpreter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27478 2023-07-22 15:53:28.000000 swarms-1.9.0/swarms/agents/tools/core/code_interpreter/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    73676 2023-07-22 15:53:28.000000 swarms-1.9.0/swarms/agents/tools/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 15:53:41.710630 swarms-1.9.0/swarms/agents/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)    19599 2023-07-22 15:53:28.000000 swarms-1.9.0/swarms/agents/utils/Agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6022 2023-07-22 15:53:28.000000 swarms-1.9.0/swarms/agents/utils/Calback.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13661 2023-07-22 15:53:28.000000 swarms-1.9.0/swarms/agents/utils/ChatOpenAI.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5529 2023-07-22 15:53:28.000000 swarms-1.9.0/swarms/agents/utils/ConversationalChatAgent.py
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-22 15:53:28.000000 swarms-1.9.0/swarms/agents/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3795 2023-07-22 15:53:28.000000 swarms-1.9.0/swarms/agents/utils/agent_creator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-07-22 15:53:28.000000 swarms-1.9.0/swarms/agents/utils/agent_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-07-22 15:53:28.000000 swarms-1.9.0/swarms/agents/utils/output_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6348 2023-07-22 15:53:28.000000 swarms-1.9.0/swarms/agents/utils/prompts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 15:53:41.710630 swarms-1.9.0/swarms/agents/workers/
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-22 15:53:28.000000 swarms-1.9.0/swarms/agents/workers/MultiModalVisualAgentTool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-22 15:53:28.000000 swarms-1.9.0/swarms/agents/workers/OmniWorkerAgent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-07-22 15:53:28.000000 swarms-1.9.0/swarms/agents/workers/PromptWorker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6132 2023-07-22 15:53:28.000000 swarms-1.9.0/swarms/agents/workers/WorkerNode.py
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-22 15:53:28.000000 swarms-1.9.0/swarms/agents/workers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22410 2023-07-22 15:53:28.000000 swarms-1.9.0/swarms/agents/workers/generative_worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 15:53:41.710630 swarms-1.9.0/swarms/agents/workers/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 15:53:41.710630 swarms-1.9.0/swarms/agents/workers/models/GroundingDINO/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-22 15:53:28.000000 swarms-1.9.0/swarms/agents/workers/models/GroundingDINO/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 15:53:41.710630 swarms-1.9.0/swarms/agents/workers/models/GroundingDINO/groundingdino/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 15:53:28.000000 swarms-1.9.0/swarms/agents/workers/models/GroundingDINO/groundingdino/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 15:53:41.710630 swarms-1.9.0/swarms/agents/workers/models/GroundingDINO/groundingdino/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-07-22 15:53:28.000000 swarms-1.9.0/swarms/agents/workers/models/GroundingDINO/groundingdino/config/GroundingDINO_SwinB_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-22 15:53:28.000000 swarms-1.9.0/swarms/agents/workers/models/GroundingDINO/groundingdino/config/GroundingDINO_SwinT_OGC.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 15:53:28.000000 swarms-1.9.0/swarms/agents/workers/models/GroundingDINO/groundingdino/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 15:53:41.714630 swarms-1.9.0/swarms/agents/workers/models/GroundingDINO/groundingdino/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 15:53:28.000000 swarms-1.9.0/swarms/agents/workers/models/GroundingDINO/groundingdino/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9398 2023-07-22 15:53:28.000000 swarms-1.9.0/swarms/agents/workers/models/GroundingDINO/groundingdino/datasets/cocogrounding_eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9711 2023-07-22 15:53:28.000000 swarms-1.9.0/swarms/agents/workers/models/GroundingDINO/groundingdino/datasets/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 15:53:41.714630 swarms-1.9.0/swarms/agents/workers/models/GroundingDINO/groundingdino/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 15:53:41.714630 swarms-1.9.0/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-07-22 15:53:28.000000 swarms-1.9.0/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 15:53:41.714630 swarms-1.9.0/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-22 15:53:28.000000 swarms-1.9.0/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7972 2023-07-22 15:53:28.000000 swarms-1.9.0/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/backbone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6866 2023-07-22 15:53:28.000000 swarms-1.9.0/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/position_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29339 2023-07-22 15:53:28.000000 swarms-1.9.0/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/swin_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12242 2023-07-22 15:53:28.000000 swarms-1.9.0/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/bertwarper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11825 2023-07-22 15:53:28.000000 swarms-1.9.0/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/fuse_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16669 2023-07-22 15:53:28.000000 swarms-1.9.0/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/groundingdino.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15482 2023-07-22 15:53:28.000000 swarms-1.9.0/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/ms_deform_attn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36805 2023-07-22 15:53:28.000000 swarms-1.9.0/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4020 2023-07-22 15:53:28.000000 swarms-1.9.0/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/transformer_vanilla.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10087 2023-07-22 15:53:28.000000 swarms-1.9.0/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-07-22 15:53:28.000000 swarms-1.9.0/swarms/agents/workers/models/GroundingDINO/groundingdino/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-07-22 15:53:28.000000 swarms-1.9.0/swarms/agents/workers/models/GroundingDINO/groundingdino/models/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 15:53:41.718630 swarms-1.9.0/swarms/agents/workers/models/GroundingDINO/groundingdino/util/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-22 15:53:28.000000 swarms-1.9.0/swarms/agents/workers/models/GroundingDINO/groundingdino/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-07-22 15:53:28.000000 swarms-1.9.0/swarms/agents/workers/models/GroundingDINO/groundingdino/util/box_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-07-22 15:53:28.000000 swarms-1.9.0/swarms/agents/workers/models/GroundingDINO/groundingdino/util/get_tokenlizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8745 2023-07-22 15:53:28.000000 swarms-1.9.0/swarms/agents/workers/models/GroundingDINO/groundingdino/util/inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-07-22 15:53:28.000000 swarms-1.9.0/swarms/agents/workers/models/GroundingDINO/groundingdino/util/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23348 2023-07-22 15:53:28.000000 swarms-1.9.0/swarms/agents/workers/models/GroundingDINO/groundingdino/util/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14380 2023-07-22 15:53:28.000000 swarms-1.9.0/swarms/agents/workers/models/GroundingDINO/groundingdino/util/slconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5377 2023-07-22 15:53:28.000000 swarms-1.9.0/swarms/agents/workers/models/GroundingDINO/groundingdino/util/slio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-07-22 15:53:28.000000 swarms-1.9.0/swarms/agents/workers/models/GroundingDINO/groundingdino/util/time_counter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17828 2023-07-22 15:53:28.000000 swarms-1.9.0/swarms/agents/workers/models/GroundingDINO/groundingdino/util/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12047 2023-07-22 15:53:28.000000 swarms-1.9.0/swarms/agents/workers/models/GroundingDINO/groundingdino/util/visualizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-07-22 15:53:28.000000 swarms-1.9.0/swarms/agents/workers/models/GroundingDINO/groundingdino/util/vl_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7179 2023-07-22 15:53:28.000000 swarms-1.9.0/swarms/agents/workers/models/GroundingDINO/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-07-22 15:53:28.000000 swarms-1.9.0/swarms/agents/workers/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 15:53:41.718630 swarms-1.9.0/swarms/agents/workers/models/segment_anything/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-22 15:53:28.000000 swarms-1.9.0/swarms/agents/workers/models/segment_anything/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 15:53:41.718630 swarms-1.9.0/swarms/agents/workers/models/segment_anything/segment_anything/
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-07-22 15:53:28.000000 swarms-1.9.0/swarms/agents/workers/models/segment_anything/segment_anything/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15148 2023-07-22 15:53:28.000000 swarms-1.9.0/swarms/agents/workers/models/segment_anything/segment_anything/automatic_mask_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-07-22 15:53:28.000000 swarms-1.9.0/swarms/agents/workers/models/segment_anything/segment_anything/build_sam.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 15:53:41.722630 swarms-1.9.0/swarms/agents/workers/models/segment_anything/segment_anything/modeling/
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-22 15:53:28.000000 swarms-1.9.0/swarms/agents/workers/models/segment_anything/segment_anything/modeling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-07-22 15:53:28.000000 swarms-1.9.0/swarms/agents/workers/models/segment_anything/segment_anything/modeling/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14420 2023-07-22 15:53:28.000000 swarms-1.9.0/swarms/agents/workers/models/segment_anything/segment_anything/modeling/image_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6615 2023-07-22 15:53:28.000000 swarms-1.9.0/swarms/agents/workers/models/segment_anything/segment_anything/modeling/mask_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8594 2023-07-22 15:53:28.000000 swarms-1.9.0/swarms/agents/workers/models/segment_anything/segment_anything/modeling/prompt_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-07-22 15:53:28.000000 swarms-1.9.0/swarms/agents/workers/models/segment_anything/segment_anything/modeling/sam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8397 2023-07-22 15:53:28.000000 swarms-1.9.0/swarms/agents/workers/models/segment_anything/segment_anything/modeling/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11649 2023-07-22 15:53:28.000000 swarms-1.9.0/swarms/agents/workers/models/segment_anything/segment_anything/predictor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 15:53:41.722630 swarms-1.9.0/swarms/agents/workers/models/segment_anything/segment_anything/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-22 15:53:28.000000 swarms-1.9.0/swarms/agents/workers/models/segment_anything/segment_anything/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12712 2023-07-22 15:53:28.000000 swarms-1.9.0/swarms/agents/workers/models/segment_anything/segment_anything/utils/amg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5812 2023-07-22 15:53:28.000000 swarms-1.9.0/swarms/agents/workers/models/segment_anything/segment_anything/utils/onnx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-07-22 15:53:28.000000 swarms-1.9.0/swarms/agents/workers/models/segment_anything/segment_anything/utils/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-07-22 15:53:28.000000 swarms-1.9.0/swarms/agents/workers/models/segment_anything/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 15:53:41.722630 swarms-1.9.0/swarms/agents/workers/multi_modal_workers/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-22 15:53:28.000000 swarms-1.9.0/swarms/agents/workers/multi_modal_workers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79584 2023-07-22 15:53:28.000000 swarms-1.9.0/swarms/agents/workers/multi_modal_workers/multi_modal_agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 15:53:41.722630 swarms-1.9.0/swarms/agents/workers/multi_modal_workers/omni_agent/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 15:53:28.000000 swarms-1.9.0/swarms/agents/workers/multi_modal_workers/omni_agent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-07-22 15:53:28.000000 swarms-1.9.0/swarms/agents/workers/multi_modal_workers/omni_agent/get_token_ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31378 2023-07-22 15:53:28.000000 swarms-1.9.0/swarms/agents/workers/multi_modal_workers/omni_agent/model_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45882 2023-07-22 15:53:28.000000 swarms-1.9.0/swarms/agents/workers/multi_modal_workers/omni_agent/omni_chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6904 2023-07-22 15:53:28.000000 swarms-1.9.0/swarms/agents/workers/worker_agent_ultra.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-07-22 15:53:28.000000 swarms-1.9.0/swarms/agents/workers/worker_ultra_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-07-22 15:53:28.000000 swarms-1.9.0/swarms/hivemind.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9296 2023-07-22 15:53:28.000000 swarms-1.9.0/swarms/swarms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 15:53:41.726630 swarms-1.9.0/swarms/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-22 15:53:28.000000 swarms-1.9.0/swarms/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 15:53:41.726630 swarms-1.9.0/swarms/utils/embeddings/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-22 15:53:28.000000 swarms-1.9.0/swarms/utils/embeddings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-22 15:53:28.000000 swarms-1.9.0/swarms/utils/embeddings/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-22 15:53:28.000000 swarms-1.9.0/swarms/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11292 2023-07-22 15:53:28.000000 swarms-1.9.0/swarms/utils/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 15:53:41.726630 swarms-1.9.0/swarms/utils/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 15:53:28.000000 swarms-1.9.0/swarms/utils/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 15:53:28.000000 swarms-1.9.0/swarms/utils/schema/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-07-22 15:53:28.000000 swarms-1.9.0/swarms/utils/static.py
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-22 15:53:28.000000 swarms-1.9.0/swarms/utils/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 15:53:41.702630 swarms-1.9.0/swarms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-22 15:53:41.000000 swarms-1.9.0/swarms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6369 2023-07-22 15:53:41.000000 swarms-1.9.0/swarms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 15:53:41.000000 swarms-1.9.0/swarms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-07-22 15:53:41.000000 swarms-1.9.0/swarms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-22 15:53:41.000000 swarms-1.9.0/swarms.egg-info/top_level.txt
```

### Comparing `swarms-1.0.6/LICENSE` & `swarms-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `swarms-1.0.6/PKG-INFO` & `swarms-1.9.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swarms
-Version: 1.0.6
+Version: 1.9.0
 Summary: Swarms - Pytorch
 Home-page: https://github.com/kyegomez/swarms
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `swarms-1.0.6/README.md` & `swarms-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `swarms-1.0.6/api/app.py` & `swarms-1.9.0/api/app.py`

 * *Files identical despite different names*

### Comparing `swarms-1.0.6/setup.py` & `swarms-1.9.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 ##
 
 setup(
   name = 'swarms',
   packages = find_packages(exclude=[]),
-  version = '1.0.6',
+  version = '1.9.0',
   license='MIT',
   description = 'Swarms - Pytorch',
   author = 'Kye Gomez',
   author_email = 'kye@apac.ai',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/kyegomez/swarms',
   keywords = [
```

### Comparing `swarms-1.0.6/swarms/agents/memory/base.py` & `swarms-1.9.0/swarms/agents/memory/base.py`

 * *Files identical despite different names*

### Comparing `swarms-1.0.6/swarms/agents/memory/chroma.py` & `swarms-1.9.0/swarms/agents/memory/chroma.py`

 * *Files identical despite different names*

### Comparing `swarms-1.0.6/swarms/agents/models/llm.py` & `swarms-1.9.0/swarms/agents/models/llm.py`

 * *Files identical despite different names*

### Comparing `swarms-1.0.6/swarms/agents/prompts/prompts.py` & `swarms-1.9.0/swarms/agents/prompts/prompts.py`

 * *Files identical despite different names*

### Comparing `swarms-1.0.6/swarms/agents/tools/agent_tools.py` & `swarms-1.9.0/swarms/agents/tools/agent_tools.py`

 * *Files identical despite different names*

### Comparing `swarms-1.0.6/swarms/agents/tools/base.py` & `swarms-1.9.0/swarms/agents/tools/base.py`

 * *Files identical despite different names*

### Comparing `swarms-1.0.6/swarms/agents/tools/core/code_interpreter/main.py` & `swarms-1.9.0/swarms/agents/tools/core/code_interpreter/main.py`

 * *Files identical despite different names*

### Comparing `swarms-1.0.6/swarms/agents/tools/main.py` & `swarms-1.9.0/swarms/agents/tools/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -2299,27 +2299,27 @@
 #         compute_type: str = "float16",
 #         run_manager: Optional[AsyncCallbackManagerForToolRun] = None,
 #     ) -> str:
 #         """Use the tool asynchronously."""
 #         raise NotImplementedError("transcribe_audio does not support async")
 ###########=========================>
 
-# #======> Calculator
-# from langchain import LLMMathChain
+#======> Calculator
+from langchain import LLMMathChain
 
-# llm_math_chain = LLMMathChain.from_llm(llm=llm, verbose=True)
-# math_tool = Tool(
-#         name="Calculator",
-#         func=llm_math_chain.run,
-#         description="useful for when you need to answer questions about math"
-#     ),
-
-# #####==========================================================================> TOOLS
-# from langchain.tools.human.tool import HumanInputRun
-# from langchain.tools import BaseTool, DuckDuckGoSearchRun
+llm_math_chain = LLMMathChain.from_llm(llm=llm, verbose=True)
+math_tool = Tool(
+        name="Calculator",
+        func=llm_math_chain.run,
+        description="useful for when you need to answer questions about math"
+    ),
+
+#####==========================================================================> TOOLS
+from langchain.tools.human.tool import HumanInputRun
+from langchain.tools import BaseTool, DuckDuckGoSearchRun
```

### Comparing `swarms-1.0.6/swarms/agents/utils/Agent.py` & `swarms-1.9.0/swarms/agents/utils/Agent.py`

 * *Files identical despite different names*

### Comparing `swarms-1.0.6/swarms/agents/utils/Calback.py` & `swarms-1.9.0/swarms/agents/utils/Calback.py`

 * *Files identical despite different names*

### Comparing `swarms-1.0.6/swarms/agents/utils/ChatOpenAI.py` & `swarms-1.9.0/swarms/agents/utils/ChatOpenAI.py`

 * *Files identical despite different names*

### Comparing `swarms-1.0.6/swarms/agents/utils/ConversationalChatAgent.py` & `swarms-1.9.0/swarms/agents/utils/ConversationalChatAgent.py`

 * *Files identical despite different names*

### Comparing `swarms-1.0.6/swarms/agents/utils/agent_creator.py` & `swarms-1.9.0/swarms/agents/utils/agent_creator.py`

 * *Files identical despite different names*

### Comparing `swarms-1.0.6/swarms/agents/utils/agent_setup.py` & `swarms-1.9.0/swarms/agents/utils/agent_setup.py`

 * *Files identical despite different names*

### Comparing `swarms-1.0.6/swarms/agents/utils/output_parser.py` & `swarms-1.9.0/swarms/agents/utils/output_parser.py`

 * *Files identical despite different names*

### Comparing `swarms-1.0.6/swarms/agents/utils/prompts.py` & `swarms-1.9.0/swarms/agents/utils/prompts.py`

 * *Files identical despite different names*

### Comparing `swarms-1.0.6/swarms/boss/boss_node.py` & `swarms-1.9.0/swarms/agents/boss/BossNode.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 
         try:
             self.baby_agi = BabyAGI.from_llm(
                 llm=self.llm,
                 vectorstore=self.vectorstore,
                 task_execution_chain=self.agent_executor,
                 max_iterations=self.max_iterations,
-                human_in_the_loop=True
             )
         except ValidationError as e:
             logging.error(f"Validation Error while initializing BabyAGI: {e}")
             raise
         except Exception as e:
             logging.error(f"Unexpected Error while initializing BabyAGI: {e}")
             raise
```

### Comparing `swarms-1.0.6/swarms/hivemind.py` & `swarms-1.9.0/swarms/hivemind.py`

 * *Files identical despite different names*

### Comparing `swarms-1.0.6/swarms/swarms.py` & `swarms-1.9.0/swarms/swarms.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,31 @@
 import logging
 import asyncio
 
 # from swarms.agents.tools.agent_tools import *
 from swarms.agents.tools.agent_tools import *
-from swarms.workers.WorkerNode import WorkerNodeInitializer, worker_node
-from swarms.boss.boss_node import BossNodeInitializer as BossNode
-from swarms.workers.worker_ultra_node import WorkerUltra
-
-from langchain import LLMMathChain
-
+from swarms.agents.workers.WorkerNode import WorkerNodeInitializer, worker_node
+from swarms.agents.boss.BossNode import BossNodeInitializer as BossNode
+from swarms.agents.workers.worker_ultra_node import WorkerUltra
 
 logging.basicConfig(level=logging.INFO, format='%(asctime)s - %(levelname)s - %(message)s')
 
 
 from swarms.utils.task import Task
 
 class Swarms:
-    def __init__(self, openai_api_key="", use_vectorstore=True, use_async=True, human_in_the_loop=True):
+    def __init__(self, openai_api_key="", use_vectorstore=True, use_async=True):
         #openai_api_key: the openai key. Default is empty
         if not openai_api_key:
             logging.error("OpenAI key is not provided")
             raise ValueError("OpenAI API key is required")
         
         self.openai_api_key = openai_api_key
         self.use_vectorstore = use_vectorstore
         self.use_async = use_async
-        self.human_in_the_loop = human_in_the_loop
 
     def initialize_llm(self, llm_class, temperature=0.5):
         """
         Init LLM 
 
         Params:
             llm_class(class): The Language model class. Default is OpenAI.
@@ -88,15 +84,15 @@
             index = faiss.IndexFlatL2(embedding_size)
 
             return FAISS(embeddings_model.embed_query, index, InMemoryDocstore({}), {})
         except Exception as e:
             logging.error(f"Failed to initialize vector store: {e}")
             return None
 
-    def initialize_worker_node(self, worker_tools, vectorstore, llm_class=ChatOpenAI, ai_name="Swarm Worker AI Assistant", human_in_the_loop=True):
+    def initialize_worker_node(self, worker_tools, vectorstore, llm_class=ChatOpenAI, ai_name="Swarm Worker AI Assistant"):
         """
         Init WorkerNode
 
         Params:
             worker_tools (list): The list of worker tools.
             vectorstore (object): The vector store object
             llm_class (class): The Language model class. Default is ChatOpenAI
@@ -104,15 +100,15 @@
         """
 
         try:
                 
             # Initialize worker node
             llm = self.initialize_llm(ChatOpenAI)
             worker_node = WorkerNodeInitializer(llm=llm, tools=worker_tools, vectorstore=vectorstore)
-            worker_node.create_agent(ai_name=ai_name, ai_role="Assistant", search_kwargs={}, human_in_the_loop=self.human_in_the_loop) # add search kwargs
+            worker_node.create_agent(ai_name=ai_name, ai_role="Assistant", human_in_the_loop=False, search_kwargs={}) # add search kwargs
 
             worker_node_tool = Tool(name="WorkerNode AI Agent", func=worker_node.run, description="Input: an objective with a todo list for that objective. Output: your task completed: Please be very clear what the objective and task instructions are. The Swarm worker agent is Useful for when you need to spawn an autonomous agent instance as a worker to accomplish any complex tasks, it can search the internet or write code or spawn child multi-modality models to process and generate images and text or audio and so on")
             return worker_node_tool
         except Exception as e:
             logging.error(f"Failed to initialize worker node: {e}")
             raise
 
@@ -131,28 +127,18 @@
         try:
 
             # Initialize boss node
             llm = self.initialize_llm(llm_class)
             todo_prompt = PromptTemplate.from_template("You are a boss planer in a swarm who is an expert at coming up with a todo list for a given objective and then creating an worker to help you accomplish your task. Rate every task on the importance of it's probability to complete the main objective on a scale from 0 to 1, an integer. Come up with a todo list for this objective: {objective} and then spawn a worker agent to complete the task for you. Always spawn an worker agent after creating a plan and pass the objective and plan to the worker agent.")
             todo_chain = LLMChain(llm=llm, prompt=todo_prompt)
 
-            #math tool
-            llm_math_chain = LLMMathChain.from_llm(llm=llm, verbose=True)
-            math_tool = Tool(
-                name="Calculator",
-                func=llm_math_chain.run,
-                description="useful for when you need to answer questions about math"
-            )
-
             tools = [
                 Tool(name="TODO", func=todo_chain.run, description="useful for when you need to come up with todo lists. Input: an objective to create a todo list for your objective. Note create a todo list then assign a ranking from 0.0 to 1.0 to each task, then sort the tasks based on the tasks most likely to achieve the objective. The Output: a todo list for that objective with rankings for each step from 0.1 Please be very clear what the objective is!"),
-                worker_node,
-                math_tool
+                worker_node
             ]
-
             suffix = """Question: {task}\n{agent_scratchpad}"""
             prefix = """You are an Boss in a swarm who performs one task based on the following objective: {objective}. Take into account these previously completed tasks: {context}.\n """
             
             prompt = ZeroShotAgent.create_prompt(tools, prefix=prefix, suffix=suffix, input_variables=["objective", "task", "context", "agent_scratchpad"],)
             llm_chain = LLMChain(llm=llm, prompt=prompt)
             agent = ZeroShotAgent(llm_chain=llm_chain, allowed_tools=[tool.name for tool in tools])
 
@@ -221,9 +207,7 @@
             logging.error("Failed to run swarms")
         else:
             logging.info(f"Successfully ran swarms with results: {result}")
         return result
     except Exception as e:
         logging.error(f"An error occured in swarm: {e}")
         return None
-
-
```

### Comparing `swarms-1.0.6/swarms/utils/embeddings/base.py` & `swarms-1.9.0/swarms/utils/embeddings/base.py`

 * *Files identical despite different names*

### Comparing `swarms-1.0.6/swarms/utils/main.py` & `swarms-1.9.0/swarms/utils/main.py`

 * *Files identical despite different names*

### Comparing `swarms-1.0.6/swarms/utils/static.py` & `swarms-1.9.0/swarms/utils/static.py`

 * *Files identical despite different names*

### Comparing `swarms-1.0.6/swarms/workers/WorkerNode.py` & `swarms-1.9.0/swarms/agents/workers/WorkerNode.py`

 * *Files identical despite different names*

### Comparing `swarms-1.0.6/swarms/workers/generative_worker.py` & `swarms-1.9.0/swarms/agents/workers/generative_worker.py`

 * *Files identical despite different names*

### Comparing `swarms-1.0.6/swarms/workers/models/GroundingDINO/groundingdino/config/GroundingDINO_SwinB_cfg.py` & `swarms-1.9.0/swarms/agents/workers/models/GroundingDINO/groundingdino/config/GroundingDINO_SwinB_cfg.py`

 * *Files identical despite different names*

### Comparing `swarms-1.0.6/swarms/workers/models/GroundingDINO/groundingdino/config/GroundingDINO_SwinT_OGC.py` & `swarms-1.9.0/swarms/agents/workers/models/GroundingDINO/groundingdino/config/GroundingDINO_SwinT_OGC.py`

 * *Files identical despite different names*

### Comparing `swarms-1.0.6/swarms/workers/models/GroundingDINO/groundingdino/datasets/cocogrounding_eval.py` & `swarms-1.9.0/swarms/agents/workers/models/GroundingDINO/groundingdino/datasets/cocogrounding_eval.py`

 * *Files identical despite different names*

### Comparing `swarms-1.0.6/swarms/workers/models/GroundingDINO/groundingdino/datasets/transforms.py` & `swarms-1.9.0/swarms/agents/workers/models/GroundingDINO/groundingdino/datasets/transforms.py`

 * *Files identical despite different names*

### Comparing `swarms-1.0.6/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/__init__.py` & `swarms-1.9.0/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/__init__.py`

 * *Files identical despite different names*

### Comparing `swarms-1.0.6/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/backbone.py` & `swarms-1.9.0/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/backbone.py`

 * *Files identical despite different names*

### Comparing `swarms-1.0.6/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/position_encoding.py` & `swarms-1.9.0/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/position_encoding.py`

 * *Files identical despite different names*

### Comparing `swarms-1.0.6/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/swin_transformer.py` & `swarms-1.9.0/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/swin_transformer.py`

 * *Files identical despite different names*

### Comparing `swarms-1.0.6/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/bertwarper.py` & `swarms-1.9.0/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/bertwarper.py`

 * *Files identical despite different names*

### Comparing `swarms-1.0.6/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/fuse_modules.py` & `swarms-1.9.0/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/fuse_modules.py`

 * *Files identical despite different names*

### Comparing `swarms-1.0.6/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/groundingdino.py` & `swarms-1.9.0/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/groundingdino.py`

 * *Files identical despite different names*

### Comparing `swarms-1.0.6/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/ms_deform_attn.py` & `swarms-1.9.0/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/ms_deform_attn.py`

 * *Files identical despite different names*

### Comparing `swarms-1.0.6/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/transformer.py` & `swarms-1.9.0/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/transformer.py`

 * *Files identical despite different names*

### Comparing `swarms-1.0.6/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/transformer_vanilla.py` & `swarms-1.9.0/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/transformer_vanilla.py`

 * *Files identical despite different names*

### Comparing `swarms-1.0.6/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/utils.py` & `swarms-1.9.0/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/utils.py`

 * *Files identical despite different names*

### Comparing `swarms-1.0.6/swarms/workers/models/GroundingDINO/groundingdino/models/__init__.py` & `swarms-1.9.0/swarms/agents/workers/models/GroundingDINO/groundingdino/models/__init__.py`

 * *Files identical despite different names*

### Comparing `swarms-1.0.6/swarms/workers/models/GroundingDINO/groundingdino/models/registry.py` & `swarms-1.9.0/swarms/agents/workers/models/GroundingDINO/groundingdino/models/registry.py`

 * *Files identical despite different names*

### Comparing `swarms-1.0.6/swarms/workers/models/GroundingDINO/groundingdino/util/box_ops.py` & `swarms-1.9.0/swarms/agents/workers/models/GroundingDINO/groundingdino/util/box_ops.py`

 * *Files identical despite different names*

### Comparing `swarms-1.0.6/swarms/workers/models/GroundingDINO/groundingdino/util/get_tokenlizer.py` & `swarms-1.9.0/swarms/agents/workers/models/GroundingDINO/groundingdino/util/get_tokenlizer.py`

 * *Files identical despite different names*

### Comparing `swarms-1.0.6/swarms/workers/models/GroundingDINO/groundingdino/util/inference.py` & `swarms-1.9.0/swarms/agents/workers/models/GroundingDINO/groundingdino/util/inference.py`

 * *Files identical despite different names*

### Comparing `swarms-1.0.6/swarms/workers/models/GroundingDINO/groundingdino/util/logger.py` & `swarms-1.9.0/swarms/agents/workers/models/GroundingDINO/groundingdino/util/logger.py`

 * *Files identical despite different names*

### Comparing `swarms-1.0.6/swarms/workers/models/GroundingDINO/groundingdino/util/misc.py` & `swarms-1.9.0/swarms/agents/workers/models/GroundingDINO/groundingdino/util/misc.py`

 * *Files identical despite different names*

### Comparing `swarms-1.0.6/swarms/workers/models/GroundingDINO/groundingdino/util/slconfig.py` & `swarms-1.9.0/swarms/agents/workers/models/GroundingDINO/groundingdino/util/slconfig.py`

 * *Files identical despite different names*

### Comparing `swarms-1.0.6/swarms/workers/models/GroundingDINO/groundingdino/util/slio.py` & `swarms-1.9.0/swarms/agents/workers/models/GroundingDINO/groundingdino/util/slio.py`

 * *Files identical despite different names*

### Comparing `swarms-1.0.6/swarms/workers/models/GroundingDINO/groundingdino/util/time_counter.py` & `swarms-1.9.0/swarms/agents/workers/models/GroundingDINO/groundingdino/util/time_counter.py`

 * *Files identical despite different names*

### Comparing `swarms-1.0.6/swarms/workers/models/GroundingDINO/groundingdino/util/utils.py` & `swarms-1.9.0/swarms/agents/workers/models/GroundingDINO/groundingdino/util/utils.py`

 * *Files identical despite different names*

### Comparing `swarms-1.0.6/swarms/workers/models/GroundingDINO/groundingdino/util/visualizer.py` & `swarms-1.9.0/swarms/agents/workers/models/GroundingDINO/groundingdino/util/visualizer.py`

 * *Files identical despite different names*

### Comparing `swarms-1.0.6/swarms/workers/models/GroundingDINO/groundingdino/util/vl_utils.py` & `swarms-1.9.0/swarms/agents/workers/models/GroundingDINO/groundingdino/util/vl_utils.py`

 * *Files identical despite different names*

### Comparing `swarms-1.0.6/swarms/workers/models/GroundingDINO/setup.py` & `swarms-1.9.0/swarms/agents/workers/models/GroundingDINO/setup.py`

 * *Files identical despite different names*

### Comparing `swarms-1.0.6/swarms/workers/models/__init__.py` & `swarms-1.9.0/swarms/agents/workers/models/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # from .GroundingDINO.groundingdino.datasets.transforms import T
 # from .GroundingDINO.groundingdino.models import build_model
 # from .GroundingDINO.groundingdino.util import box_ops, SLConfig
 # from .GroundingDINO.groundingdino.util.utils import clean_state_dict, get_phrases_from_posmap
 # from .segment_anything.segment_anything import build_sam, SamPredictor, SamAutomaticMaskGenerator
-from swarms.workers.models.GroundingDINO.groundingdino.datasets.transforms import (
+from swarms.agents.workers.models.GroundingDINO.groundingdino.datasets.transforms import (
     Compose,
     Normalize,
     ToTensor,
     crop,
     hflip,
     resize,
     pad,
@@ -17,13 +17,13 @@
     CenterCrop,
     RandomHorizontalFlip,
     RandomResize,
     RandomPad,
     RandomSelect
 )
 
-from swarms.workers.models.GroundingDINO.groundingdino.models import build_model
-from swarms.workers.models.GroundingDINO.groundingdino.util import box_ops
-from swarms.workers.models.GroundingDINO.groundingdino.util.slconfig import SLConfig
-from swarms.workers.models.GroundingDINO.groundingdino.util.utils import clean_state_dict, get_phrases_from_posmap
+from swarms.agents.workers.models.GroundingDINO.groundingdino.models import build_model
+from swarms.agents.workers.models.GroundingDINO.groundingdino.util import box_ops
+from swarms.agents.workers.models.GroundingDINO.groundingdino.util.slconfig import SLConfig
+from swarms.agents.workers.models.GroundingDINO.groundingdino.util.utils import clean_state_dict, get_phrases_from_posmap
 
-from swarms.workers.models.segment_anything import build_sam, SamPredictor, SamAutomaticMaskGenerator
+from swarms.agents.workers.models.segment_anything import build_sam, SamPredictor, SamAutomaticMaskGenerator
```

### Comparing `swarms-1.0.6/swarms/workers/models/segment_anything/segment_anything/automatic_mask_generator.py` & `swarms-1.9.0/swarms/agents/workers/models/segment_anything/segment_anything/automatic_mask_generator.py`

 * *Files identical despite different names*

### Comparing `swarms-1.0.6/swarms/workers/models/segment_anything/segment_anything/build_sam.py` & `swarms-1.9.0/swarms/agents/workers/models/segment_anything/segment_anything/build_sam.py`

 * *Files identical despite different names*

### Comparing `swarms-1.0.6/swarms/workers/models/segment_anything/segment_anything/modeling/common.py` & `swarms-1.9.0/swarms/agents/workers/models/segment_anything/segment_anything/modeling/common.py`

 * *Files identical despite different names*

### Comparing `swarms-1.0.6/swarms/workers/models/segment_anything/segment_anything/modeling/image_encoder.py` & `swarms-1.9.0/swarms/agents/workers/models/segment_anything/segment_anything/modeling/image_encoder.py`

 * *Files identical despite different names*

### Comparing `swarms-1.0.6/swarms/workers/models/segment_anything/segment_anything/modeling/mask_decoder.py` & `swarms-1.9.0/swarms/agents/workers/models/segment_anything/segment_anything/modeling/mask_decoder.py`

 * *Files identical despite different names*

### Comparing `swarms-1.0.6/swarms/workers/models/segment_anything/segment_anything/modeling/prompt_encoder.py` & `swarms-1.9.0/swarms/agents/workers/models/segment_anything/segment_anything/modeling/prompt_encoder.py`

 * *Files identical despite different names*

### Comparing `swarms-1.0.6/swarms/workers/models/segment_anything/segment_anything/modeling/sam.py` & `swarms-1.9.0/swarms/agents/workers/models/segment_anything/segment_anything/modeling/sam.py`

 * *Files identical despite different names*

### Comparing `swarms-1.0.6/swarms/workers/models/segment_anything/segment_anything/modeling/transformer.py` & `swarms-1.9.0/swarms/agents/workers/models/segment_anything/segment_anything/modeling/transformer.py`

 * *Files identical despite different names*

### Comparing `swarms-1.0.6/swarms/workers/models/segment_anything/segment_anything/predictor.py` & `swarms-1.9.0/swarms/agents/workers/models/segment_anything/segment_anything/predictor.py`

 * *Files identical despite different names*

### Comparing `swarms-1.0.6/swarms/workers/models/segment_anything/segment_anything/utils/amg.py` & `swarms-1.9.0/swarms/agents/workers/models/segment_anything/segment_anything/utils/amg.py`

 * *Files identical despite different names*

### Comparing `swarms-1.0.6/swarms/workers/models/segment_anything/segment_anything/utils/onnx.py` & `swarms-1.9.0/swarms/agents/workers/models/segment_anything/segment_anything/utils/onnx.py`

 * *Files identical despite different names*

### Comparing `swarms-1.0.6/swarms/workers/models/segment_anything/segment_anything/utils/transforms.py` & `swarms-1.9.0/swarms/agents/workers/models/segment_anything/segment_anything/utils/transforms.py`

 * *Files identical despite different names*

### Comparing `swarms-1.0.6/swarms/workers/models/segment_anything/setup.py` & `swarms-1.9.0/swarms/agents/workers/models/segment_anything/setup.py`

 * *Files identical despite different names*

### Comparing `swarms-1.0.6/swarms/workers/multi_modal_worker.py` & `swarms-1.9.0/swarms/agents/workers/MultiModalVisualAgentTool.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-# from swarms.workers.multi_modal_workers.multi_modal_agent import MultiModalVisualAgent
-from swarms.workers.multi_modal_workers.multi_modal_agent import MultiModalVisualAgent
+from swarms.agents.workers.multi_modal_workers.multi_modal_agent import MultiModalVisualAgent
 from langchain.tools import BaseTool
 
 class MultiModalVisualAgentTool(BaseTool):
     name = "multi_visual_agent"
     description = "Multi-Modal Visual agent tool"
 
     def __init__(self, agent: MultiModalVisualAgent):
```

### Comparing `swarms-1.0.6/swarms/workers/multi_modal_workers/multi_modal_agent.py` & `swarms-1.9.0/swarms/agents/workers/multi_modal_workers/multi_modal_agent.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 from langchain.agents.initialize import initialize_agent
 from langchain.agents.tools import Tool
 from langchain.chains.conversation.memory import ConversationBufferMemory
 from langchain.llms.openai import OpenAI
 
 # Grounding DINO
 # import groundingdino.datasets.transforms as T
-from swarms.workers.models import (
+from swarms.agents.workers.models import (
     Compose,
     Normalize,
     ToTensor,
     crop,
     hflip,
     resize,
     pad,
@@ -44,20 +44,20 @@
     CenterCrop,
     RandomHorizontalFlip,
     RandomResize,
     RandomPad,
     RandomSelect
 )
 
-from swarms.workers.models import build_model
-from swarms.workers.models  import box_ops
-from swarms.workers.models import SLConfig
-from swarms.workers.models import clean_state_dict, get_phrases_from_posmap
+from swarms.agents.workers.models import build_model
+from swarms.agents.workers.models  import box_ops
+from swarms.agents.workers.models import SLConfig
+from swarms.agents.workers.models import clean_state_dict, get_phrases_from_posmap
 
-from swarms.workers.models.segment_anything import build_sam, SamPredictor, SamAutomaticMaskGenerator
+from swarms.agents.workers.models.segment_anything import build_sam, SamPredictor, SamAutomaticMaskGenerator
 import cv2
 import numpy as np
 import matplotlib.pyplot as plt
 import wget
 
 VISUAL_AGENT_PREFIX = """Worker Multi-Modal Agent is designed to be able to assist with a wide range of text and visual related tasks, from answering simple questions to providing in-depth explanations and discussions on a wide range of topics. Worker Multi-Modal Agent is able to generate human-like text based on the input it receives, allowing it to engage in natural-sounding conversations and provide responses that are coherent and relevant to the topic at hand.
```

### Comparing `swarms-1.0.6/swarms/workers/multi_modal_workers/omni_agent/get_token_ids.py` & `swarms-1.9.0/swarms/agents/workers/multi_modal_workers/omni_agent/get_token_ids.py`

 * *Files identical despite different names*

### Comparing `swarms-1.0.6/swarms/workers/multi_modal_workers/omni_agent/model_server.py` & `swarms-1.9.0/swarms/agents/workers/multi_modal_workers/omni_agent/model_server.py`

 * *Files identical despite different names*

### Comparing `swarms-1.0.6/swarms/workers/multi_modal_workers/omni_agent/omni_chat.py` & `swarms-1.9.0/swarms/agents/workers/multi_modal_workers/omni_agent/omni_chat.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from pydub import AudioSegment
 import threading
 from queue import Queue
 # import flask
 # from flask import request, jsonify
 import waitress
 # from flask_cors import CORS, cross_origin
-from swarms.workers.multi_modal_workers.omni_agent.get_token_ids import get_token_ids_for_task_parsing, get_token_ids_for_choose_model, count_tokens, get_max_context_length
+from swarms.agents.workers.multi_modal_workers.omni_agent.get_token_ids import get_token_ids_for_task_parsing, get_token_ids_for_choose_model, count_tokens, get_max_context_length
 from huggingface_hub.inference_api import InferenceApi
 from huggingface_hub.inference_api import ALL_TASKS
 
 parser = argparse.ArgumentParser()
 parser.add_argument("--config", type=str, default="swarms/agents/workers/multi_modal_workers/omni_agent/config.yml")
 parser.add_argument("--mode", type=str, default="cli")
 args = parser.parse_args()
```

### Comparing `swarms-1.0.6/swarms/workers/omni_worker.py` & `swarms-1.9.0/swarms/agents/workers/OmniWorkerAgent.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 #boss node -> worker agent -> omni agent [worker of the worker]
 from langchain.tools import tool
-# from swarms.workers.multi_modal_workers.omni_agent.omni_chat import chat_huggingface
-from swarms.workers.multi_modal_workers.omni_agent.omni_chat import chat_huggingface
+from swarms.agents.workers.multi_modal_workers.omni_agent.omni_chat import chat_huggingface
 
 class OmniWorkerAgent:
     def __init__(self, api_key, api_endpoint, api_type):
         self.api_key = api_key
         self.api_endpoint = api_endpoint
         self.api_type = api_type
```

### Comparing `swarms-1.0.6/swarms/workers/worker_agent_ultra.py` & `swarms-1.9.0/swarms/agents/workers/worker_agent_ultra.py`

 * *Files identical despite different names*

### Comparing `swarms-1.0.6/swarms/workers/worker_ultra_node.py` & `swarms-1.9.0/swarms/agents/workers/worker_ultra_node.py`

 * *Files identical despite different names*

### Comparing `swarms-1.0.6/swarms.egg-info/PKG-INFO` & `swarms-1.9.0/swarms.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swarms
-Version: 1.0.6
+Version: 1.9.0
 Summary: Swarms - Pytorch
 Home-page: https://github.com/kyegomez/swarms
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `swarms-1.0.6/swarms.egg-info/SOURCES.txt` & `swarms-1.9.0/swarms.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -8,23 +8,23 @@
 swarms/swarms.py
 swarms.egg-info/PKG-INFO
 swarms.egg-info/SOURCES.txt
 swarms.egg-info/dependency_links.txt
 swarms.egg-info/requires.txt
 swarms.egg-info/top_level.txt
 swarms/agents/__init__.py
+swarms/agents/boss/BossNode.py
+swarms/agents/boss/__init__.py
 swarms/agents/memory/__init__.py
 swarms/agents/memory/base.py
 swarms/agents/memory/chroma.py
 swarms/agents/models/__init__.py
 swarms/agents/models/llm.py
 swarms/agents/prompts/__init__.py
 swarms/agents/prompts/prompts.py
-swarms/agents/prompts/chains/__init__.py
-swarms/agents/prompts/chains/llm.py
 swarms/agents/tools/__init__.py
 swarms/agents/tools/agent_tools.py
 swarms/agents/tools/base.py
 swarms/agents/tools/main.py
 swarms/agents/tools/core/__init__.py
 swarms/agents/tools/core/code_interpreter/__init__.py
 swarms/agents/tools/core/code_interpreter/main.py
@@ -33,85 +33,83 @@
 swarms/agents/utils/ChatOpenAI.py
 swarms/agents/utils/ConversationalChatAgent.py
 swarms/agents/utils/__init__.py
 swarms/agents/utils/agent_creator.py
 swarms/agents/utils/agent_setup.py
 swarms/agents/utils/output_parser.py
 swarms/agents/utils/prompts.py
-swarms/boss/__init__.py
-swarms/boss/boss_node.py
+swarms/agents/workers/MultiModalVisualAgentTool.py
+swarms/agents/workers/OmniWorkerAgent.py
+swarms/agents/workers/PromptWorker.py
+swarms/agents/workers/WorkerNode.py
+swarms/agents/workers/__init__.py
+swarms/agents/workers/generative_worker.py
+swarms/agents/workers/worker_agent_ultra.py
+swarms/agents/workers/worker_ultra_node.py
+swarms/agents/workers/models/__init__.py
+swarms/agents/workers/models/GroundingDINO/__init__.py
+swarms/agents/workers/models/GroundingDINO/setup.py
+swarms/agents/workers/models/GroundingDINO/groundingdino/__init__.py
+swarms/agents/workers/models/GroundingDINO/groundingdino/config/GroundingDINO_SwinB_cfg.py
+swarms/agents/workers/models/GroundingDINO/groundingdino/config/GroundingDINO_SwinT_OGC.py
+swarms/agents/workers/models/GroundingDINO/groundingdino/config/__init__.py
+swarms/agents/workers/models/GroundingDINO/groundingdino/datasets/__init__.py
+swarms/agents/workers/models/GroundingDINO/groundingdino/datasets/cocogrounding_eval.py
+swarms/agents/workers/models/GroundingDINO/groundingdino/datasets/transforms.py
+swarms/agents/workers/models/GroundingDINO/groundingdino/models/__init__.py
+swarms/agents/workers/models/GroundingDINO/groundingdino/models/registry.py
+swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/__init__.py
+swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/bertwarper.py
+swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/fuse_modules.py
+swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/groundingdino.py
+swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/ms_deform_attn.py
+swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/transformer.py
+swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/transformer_vanilla.py
+swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/utils.py
+swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/__init__.py
+swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/backbone.py
+swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/position_encoding.py
+swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/swin_transformer.py
+swarms/agents/workers/models/GroundingDINO/groundingdino/util/__init__.py
+swarms/agents/workers/models/GroundingDINO/groundingdino/util/box_ops.py
+swarms/agents/workers/models/GroundingDINO/groundingdino/util/get_tokenlizer.py
+swarms/agents/workers/models/GroundingDINO/groundingdino/util/inference.py
+swarms/agents/workers/models/GroundingDINO/groundingdino/util/logger.py
+swarms/agents/workers/models/GroundingDINO/groundingdino/util/misc.py
+swarms/agents/workers/models/GroundingDINO/groundingdino/util/slconfig.py
+swarms/agents/workers/models/GroundingDINO/groundingdino/util/slio.py
+swarms/agents/workers/models/GroundingDINO/groundingdino/util/time_counter.py
+swarms/agents/workers/models/GroundingDINO/groundingdino/util/utils.py
+swarms/agents/workers/models/GroundingDINO/groundingdino/util/visualizer.py
+swarms/agents/workers/models/GroundingDINO/groundingdino/util/vl_utils.py
+swarms/agents/workers/models/segment_anything/__init__.py
+swarms/agents/workers/models/segment_anything/setup.py
+swarms/agents/workers/models/segment_anything/segment_anything/__init__.py
+swarms/agents/workers/models/segment_anything/segment_anything/automatic_mask_generator.py
+swarms/agents/workers/models/segment_anything/segment_anything/build_sam.py
+swarms/agents/workers/models/segment_anything/segment_anything/predictor.py
+swarms/agents/workers/models/segment_anything/segment_anything/modeling/__init__.py
+swarms/agents/workers/models/segment_anything/segment_anything/modeling/common.py
+swarms/agents/workers/models/segment_anything/segment_anything/modeling/image_encoder.py
+swarms/agents/workers/models/segment_anything/segment_anything/modeling/mask_decoder.py
+swarms/agents/workers/models/segment_anything/segment_anything/modeling/prompt_encoder.py
+swarms/agents/workers/models/segment_anything/segment_anything/modeling/sam.py
+swarms/agents/workers/models/segment_anything/segment_anything/modeling/transformer.py
+swarms/agents/workers/models/segment_anything/segment_anything/utils/__init__.py
+swarms/agents/workers/models/segment_anything/segment_anything/utils/amg.py
+swarms/agents/workers/models/segment_anything/segment_anything/utils/onnx.py
+swarms/agents/workers/models/segment_anything/segment_anything/utils/transforms.py
+swarms/agents/workers/multi_modal_workers/__init__.py
+swarms/agents/workers/multi_modal_workers/multi_modal_agent.py
+swarms/agents/workers/multi_modal_workers/omni_agent/__init__.py
+swarms/agents/workers/multi_modal_workers/omni_agent/get_token_ids.py
+swarms/agents/workers/multi_modal_workers/omni_agent/model_server.py
+swarms/agents/workers/multi_modal_workers/omni_agent/omni_chat.py
 swarms/utils/__init__.py
 swarms/utils/logger.py
 swarms/utils/main.py
 swarms/utils/static.py
 swarms/utils/task.py
 swarms/utils/embeddings/__init__.py
 swarms/utils/embeddings/base.py
 swarms/utils/schema/__init__.py
-swarms/utils/schema/base.py
-swarms/workers/WorkerNode.py
-swarms/workers/__init__.py
-swarms/workers/character_generative.py
-swarms/workers/generative_worker.py
-swarms/workers/multi_modal_worker.py
-swarms/workers/omni_worker.py
-swarms/workers/worker_agent_ultra.py
-swarms/workers/worker_ultra_node.py
-swarms/workers/models/__init__.py
-swarms/workers/models/GroundingDINO/__init__.py
-swarms/workers/models/GroundingDINO/setup.py
-swarms/workers/models/GroundingDINO/groundingdino/__init__.py
-swarms/workers/models/GroundingDINO/groundingdino/config/GroundingDINO_SwinB_cfg.py
-swarms/workers/models/GroundingDINO/groundingdino/config/GroundingDINO_SwinT_OGC.py
-swarms/workers/models/GroundingDINO/groundingdino/config/__init__.py
-swarms/workers/models/GroundingDINO/groundingdino/datasets/__init__.py
-swarms/workers/models/GroundingDINO/groundingdino/datasets/cocogrounding_eval.py
-swarms/workers/models/GroundingDINO/groundingdino/datasets/transforms.py
-swarms/workers/models/GroundingDINO/groundingdino/models/__init__.py
-swarms/workers/models/GroundingDINO/groundingdino/models/registry.py
-swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/__init__.py
-swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/bertwarper.py
-swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/fuse_modules.py
-swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/groundingdino.py
-swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/ms_deform_attn.py
-swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/transformer.py
-swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/transformer_vanilla.py
-swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/utils.py
-swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/__init__.py
-swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/backbone.py
-swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/position_encoding.py
-swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/swin_transformer.py
-swarms/workers/models/GroundingDINO/groundingdino/util/__init__.py
-swarms/workers/models/GroundingDINO/groundingdino/util/box_ops.py
-swarms/workers/models/GroundingDINO/groundingdino/util/get_tokenlizer.py
-swarms/workers/models/GroundingDINO/groundingdino/util/inference.py
-swarms/workers/models/GroundingDINO/groundingdino/util/logger.py
-swarms/workers/models/GroundingDINO/groundingdino/util/misc.py
-swarms/workers/models/GroundingDINO/groundingdino/util/slconfig.py
-swarms/workers/models/GroundingDINO/groundingdino/util/slio.py
-swarms/workers/models/GroundingDINO/groundingdino/util/time_counter.py
-swarms/workers/models/GroundingDINO/groundingdino/util/utils.py
-swarms/workers/models/GroundingDINO/groundingdino/util/visualizer.py
-swarms/workers/models/GroundingDINO/groundingdino/util/vl_utils.py
-swarms/workers/models/segment_anything/__init__.py
-swarms/workers/models/segment_anything/setup.py
-swarms/workers/models/segment_anything/segment_anything/__init__.py
-swarms/workers/models/segment_anything/segment_anything/automatic_mask_generator.py
-swarms/workers/models/segment_anything/segment_anything/build_sam.py
-swarms/workers/models/segment_anything/segment_anything/predictor.py
-swarms/workers/models/segment_anything/segment_anything/modeling/__init__.py
-swarms/workers/models/segment_anything/segment_anything/modeling/common.py
-swarms/workers/models/segment_anything/segment_anything/modeling/image_encoder.py
-swarms/workers/models/segment_anything/segment_anything/modeling/mask_decoder.py
-swarms/workers/models/segment_anything/segment_anything/modeling/prompt_encoder.py
-swarms/workers/models/segment_anything/segment_anything/modeling/sam.py
-swarms/workers/models/segment_anything/segment_anything/modeling/transformer.py
-swarms/workers/models/segment_anything/segment_anything/utils/__init__.py
-swarms/workers/models/segment_anything/segment_anything/utils/amg.py
-swarms/workers/models/segment_anything/segment_anything/utils/onnx.py
-swarms/workers/models/segment_anything/segment_anything/utils/transforms.py
-swarms/workers/multi_modal_workers/__init__.py
-swarms/workers/multi_modal_workers/multi_modal_agent.py
-swarms/workers/multi_modal_workers/omni_agent/__init__.py
-swarms/workers/multi_modal_workers/omni_agent/get_token_ids.py
-swarms/workers/multi_modal_workers/omni_agent/model_server.py
-swarms/workers/multi_modal_workers/omni_agent/omni_chat.py
+swarms/utils/schema/base.py
```

### Comparing `swarms-1.0.6/swarms.egg-info/requires.txt` & `swarms-1.9.0/swarms.egg-info/requires.txt`

 * *Files identical despite different names*

