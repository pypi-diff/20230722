# Comparing `tmp/swarms-0.9.0.tar.gz` & `tmp/swarms-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swarms-0.9.0.tar", last modified: Fri Jul 21 23:09:45 2023, max compression
+gzip compressed data, was "swarms-0.9.1.tar", last modified: Fri Jul 21 23:15:19 2023, max compression
```

## Comparing `swarms-0.9.0.tar` & `swarms-0.9.1.tar`

### file list

```diff
@@ -1,149 +1,149 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 23:09:45.423401 swarms-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-21 23:09:35.000000 swarms-0.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-21 23:09:45.423401 swarms-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15283 2023-07-21 23:09:35.000000 swarms-0.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 23:09:45.407401 swarms-0.9.0/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 23:09:35.000000 swarms-0.9.0/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-07-21 23:09:35.000000 swarms-0.9.0/api/app.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 23:09:45.423401 swarms-0.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-07-21 23:09:35.000000 swarms-0.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 23:09:45.407401 swarms-0.9.0/swarms/
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-21 23:09:35.000000 swarms-0.9.0/swarms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 23:09:45.411401 swarms-0.9.0/swarms/agents/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-21 23:09:35.000000 swarms-0.9.0/swarms/agents/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 23:09:45.411401 swarms-0.9.0/swarms/agents/boss/
--rw-r--r--   0 runner    (1001) docker     (123)     5795 2023-07-21 23:09:35.000000 swarms-0.9.0/swarms/agents/boss/BossNode.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 23:09:35.000000 swarms-0.9.0/swarms/agents/boss/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 23:09:45.411401 swarms-0.9.0/swarms/agents/memory/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 23:09:35.000000 swarms-0.9.0/swarms/agents/memory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18115 2023-07-21 23:09:35.000000 swarms-0.9.0/swarms/agents/memory/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    22333 2023-07-21 23:09:35.000000 swarms-0.9.0/swarms/agents/memory/chroma.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 23:09:45.411401 swarms-0.9.0/swarms/agents/models/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-21 23:09:35.000000 swarms-0.9.0/swarms/agents/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-07-21 23:09:35.000000 swarms-0.9.0/swarms/agents/models/llm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 23:09:45.411401 swarms-0.9.0/swarms/agents/prompts/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-21 23:09:35.000000 swarms-0.9.0/swarms/agents/prompts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-07-21 23:09:35.000000 swarms-0.9.0/swarms/agents/prompts/prompts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 23:09:45.411401 swarms-0.9.0/swarms/agents/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-21 23:09:35.000000 swarms-0.9.0/swarms/agents/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-07-21 23:09:35.000000 swarms-0.9.0/swarms/agents/tools/agent_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-07-21 23:09:35.000000 swarms-0.9.0/swarms/agents/tools/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 23:09:45.411401 swarms-0.9.0/swarms/agents/tools/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 23:09:35.000000 swarms-0.9.0/swarms/agents/tools/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 23:09:45.411401 swarms-0.9.0/swarms/agents/tools/core/code_interpreter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 23:09:35.000000 swarms-0.9.0/swarms/agents/tools/core/code_interpreter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27478 2023-07-21 23:09:35.000000 swarms-0.9.0/swarms/agents/tools/core/code_interpreter/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    73690 2023-07-21 23:09:35.000000 swarms-0.9.0/swarms/agents/tools/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 23:09:45.411401 swarms-0.9.0/swarms/agents/utils/
--rw-r--r--   0 runner    (1001) docker     (123)    19599 2023-07-21 23:09:35.000000 swarms-0.9.0/swarms/agents/utils/Agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     6022 2023-07-21 23:09:35.000000 swarms-0.9.0/swarms/agents/utils/Calback.py
--rw-r--r--   0 runner    (1001) docker     (123)    13661 2023-07-21 23:09:35.000000 swarms-0.9.0/swarms/agents/utils/ChatOpenAI.py
--rw-r--r--   0 runner    (1001) docker     (123)     5508 2023-07-21 23:09:35.000000 swarms-0.9.0/swarms/agents/utils/ConversationalChatAgent.py
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-21 23:09:35.000000 swarms-0.9.0/swarms/agents/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3795 2023-07-21 23:09:35.000000 swarms-0.9.0/swarms/agents/utils/agent_creator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-07-21 23:09:35.000000 swarms-0.9.0/swarms/agents/utils/agent_setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-07-21 23:09:35.000000 swarms-0.9.0/swarms/agents/utils/output_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     6348 2023-07-21 23:09:35.000000 swarms-0.9.0/swarms/agents/utils/prompts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 23:09:45.411401 swarms-0.9.0/swarms/agents/workers/
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-21 23:09:35.000000 swarms-0.9.0/swarms/agents/workers/MultiModalVisualAgentTool.py
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-21 23:09:35.000000 swarms-0.9.0/swarms/agents/workers/OmniWorkerAgent.py
--rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-07-21 23:09:35.000000 swarms-0.9.0/swarms/agents/workers/PromptWorker.py
--rw-r--r--   0 runner    (1001) docker     (123)     6132 2023-07-21 23:09:35.000000 swarms-0.9.0/swarms/agents/workers/WorkerNode.py
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-21 23:09:35.000000 swarms-0.9.0/swarms/agents/workers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22410 2023-07-21 23:09:35.000000 swarms-0.9.0/swarms/agents/workers/generative_worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 23:09:45.415401 swarms-0.9.0/swarms/agents/workers/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 23:09:45.415401 swarms-0.9.0/swarms/agents/workers/models/GroundingDINO/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-21 23:09:36.000000 swarms-0.9.0/swarms/agents/workers/models/GroundingDINO/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 23:09:45.415401 swarms-0.9.0/swarms/agents/workers/models/GroundingDINO/groundingdino/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 23:09:36.000000 swarms-0.9.0/swarms/agents/workers/models/GroundingDINO/groundingdino/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 23:09:45.415401 swarms-0.9.0/swarms/agents/workers/models/GroundingDINO/groundingdino/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-07-21 23:09:36.000000 swarms-0.9.0/swarms/agents/workers/models/GroundingDINO/groundingdino/config/GroundingDINO_SwinB_cfg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-21 23:09:36.000000 swarms-0.9.0/swarms/agents/workers/models/GroundingDINO/groundingdino/config/GroundingDINO_SwinT_OGC.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 23:09:36.000000 swarms-0.9.0/swarms/agents/workers/models/GroundingDINO/groundingdino/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 23:09:45.415401 swarms-0.9.0/swarms/agents/workers/models/GroundingDINO/groundingdino/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 23:09:36.000000 swarms-0.9.0/swarms/agents/workers/models/GroundingDINO/groundingdino/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9398 2023-07-21 23:09:36.000000 swarms-0.9.0/swarms/agents/workers/models/GroundingDINO/groundingdino/datasets/cocogrounding_eval.py
--rw-r--r--   0 runner    (1001) docker     (123)     9711 2023-07-21 23:09:36.000000 swarms-0.9.0/swarms/agents/workers/models/GroundingDINO/groundingdino/datasets/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 23:09:45.415401 swarms-0.9.0/swarms/agents/workers/models/GroundingDINO/groundingdino/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 23:09:45.415401 swarms-0.9.0/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-07-21 23:09:36.000000 swarms-0.9.0/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 23:09:45.415401 swarms-0.9.0/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-21 23:09:36.000000 swarms-0.9.0/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7972 2023-07-21 23:09:36.000000 swarms-0.9.0/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/backbone.py
--rw-r--r--   0 runner    (1001) docker     (123)     6866 2023-07-21 23:09:36.000000 swarms-0.9.0/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/position_encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)    29339 2023-07-21 23:09:36.000000 swarms-0.9.0/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/swin_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    12242 2023-07-21 23:09:36.000000 swarms-0.9.0/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/bertwarper.py
--rw-r--r--   0 runner    (1001) docker     (123)    11825 2023-07-21 23:09:36.000000 swarms-0.9.0/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/fuse_modules.py
--rw-r--r--   0 runner    (1001) docker     (123)    16669 2023-07-21 23:09:36.000000 swarms-0.9.0/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/groundingdino.py
--rw-r--r--   0 runner    (1001) docker     (123)    15482 2023-07-21 23:09:36.000000 swarms-0.9.0/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/ms_deform_attn.py
--rw-r--r--   0 runner    (1001) docker     (123)    36805 2023-07-21 23:09:36.000000 swarms-0.9.0/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4020 2023-07-21 23:09:36.000000 swarms-0.9.0/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/transformer_vanilla.py
--rw-r--r--   0 runner    (1001) docker     (123)    10087 2023-07-21 23:09:36.000000 swarms-0.9.0/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-07-21 23:09:36.000000 swarms-0.9.0/swarms/agents/workers/models/GroundingDINO/groundingdino/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-07-21 23:09:36.000000 swarms-0.9.0/swarms/agents/workers/models/GroundingDINO/groundingdino/models/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 23:09:45.419401 swarms-0.9.0/swarms/agents/workers/models/GroundingDINO/groundingdino/util/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-21 23:09:36.000000 swarms-0.9.0/swarms/agents/workers/models/GroundingDINO/groundingdino/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-07-21 23:09:36.000000 swarms-0.9.0/swarms/agents/workers/models/GroundingDINO/groundingdino/util/box_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-07-21 23:09:36.000000 swarms-0.9.0/swarms/agents/workers/models/GroundingDINO/groundingdino/util/get_tokenlizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8745 2023-07-21 23:09:36.000000 swarms-0.9.0/swarms/agents/workers/models/GroundingDINO/groundingdino/util/inference.py
--rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-07-21 23:09:36.000000 swarms-0.9.0/swarms/agents/workers/models/GroundingDINO/groundingdino/util/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    23348 2023-07-21 23:09:36.000000 swarms-0.9.0/swarms/agents/workers/models/GroundingDINO/groundingdino/util/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)    14380 2023-07-21 23:09:36.000000 swarms-0.9.0/swarms/agents/workers/models/GroundingDINO/groundingdino/util/slconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     5377 2023-07-21 23:09:36.000000 swarms-0.9.0/swarms/agents/workers/models/GroundingDINO/groundingdino/util/slio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-07-21 23:09:36.000000 swarms-0.9.0/swarms/agents/workers/models/GroundingDINO/groundingdino/util/time_counter.py
--rw-r--r--   0 runner    (1001) docker     (123)    17828 2023-07-21 23:09:36.000000 swarms-0.9.0/swarms/agents/workers/models/GroundingDINO/groundingdino/util/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    12047 2023-07-21 23:09:36.000000 swarms-0.9.0/swarms/agents/workers/models/GroundingDINO/groundingdino/util/visualizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-07-21 23:09:36.000000 swarms-0.9.0/swarms/agents/workers/models/GroundingDINO/groundingdino/util/vl_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7179 2023-07-21 23:09:36.000000 swarms-0.9.0/swarms/agents/workers/models/GroundingDINO/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-07-21 23:09:36.000000 swarms-0.9.0/swarms/agents/workers/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 23:09:45.419401 swarms-0.9.0/swarms/agents/workers/models/segment_anything/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-21 23:09:36.000000 swarms-0.9.0/swarms/agents/workers/models/segment_anything/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 23:09:45.419401 swarms-0.9.0/swarms/agents/workers/models/segment_anything/segment_anything/
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-07-21 23:09:36.000000 swarms-0.9.0/swarms/agents/workers/models/segment_anything/segment_anything/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15148 2023-07-21 23:09:36.000000 swarms-0.9.0/swarms/agents/workers/models/segment_anything/segment_anything/automatic_mask_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-07-21 23:09:36.000000 swarms-0.9.0/swarms/agents/workers/models/segment_anything/segment_anything/build_sam.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 23:09:45.419401 swarms-0.9.0/swarms/agents/workers/models/segment_anything/segment_anything/modeling/
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-21 23:09:36.000000 swarms-0.9.0/swarms/agents/workers/models/segment_anything/segment_anything/modeling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-07-21 23:09:36.000000 swarms-0.9.0/swarms/agents/workers/models/segment_anything/segment_anything/modeling/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    14420 2023-07-21 23:09:36.000000 swarms-0.9.0/swarms/agents/workers/models/segment_anything/segment_anything/modeling/image_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     6615 2023-07-21 23:09:36.000000 swarms-0.9.0/swarms/agents/workers/models/segment_anything/segment_anything/modeling/mask_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     8594 2023-07-21 23:09:36.000000 swarms-0.9.0/swarms/agents/workers/models/segment_anything/segment_anything/modeling/prompt_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-07-21 23:09:36.000000 swarms-0.9.0/swarms/agents/workers/models/segment_anything/segment_anything/modeling/sam.py
--rw-r--r--   0 runner    (1001) docker     (123)     8397 2023-07-21 23:09:36.000000 swarms-0.9.0/swarms/agents/workers/models/segment_anything/segment_anything/modeling/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11649 2023-07-21 23:09:36.000000 swarms-0.9.0/swarms/agents/workers/models/segment_anything/segment_anything/predictor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 23:09:45.419401 swarms-0.9.0/swarms/agents/workers/models/segment_anything/segment_anything/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-21 23:09:36.000000 swarms-0.9.0/swarms/agents/workers/models/segment_anything/segment_anything/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12712 2023-07-21 23:09:36.000000 swarms-0.9.0/swarms/agents/workers/models/segment_anything/segment_anything/utils/amg.py
--rw-r--r--   0 runner    (1001) docker     (123)     5812 2023-07-21 23:09:36.000000 swarms-0.9.0/swarms/agents/workers/models/segment_anything/segment_anything/utils/onnx.py
--rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-07-21 23:09:36.000000 swarms-0.9.0/swarms/agents/workers/models/segment_anything/segment_anything/utils/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-07-21 23:09:36.000000 swarms-0.9.0/swarms/agents/workers/models/segment_anything/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 23:09:45.419401 swarms-0.9.0/swarms/agents/workers/multi_modal_workers/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-21 23:09:36.000000 swarms-0.9.0/swarms/agents/workers/multi_modal_workers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    79584 2023-07-21 23:09:36.000000 swarms-0.9.0/swarms/agents/workers/multi_modal_workers/multi_modal_agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 23:09:45.419401 swarms-0.9.0/swarms/agents/workers/multi_modal_workers/omni_agent/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 23:09:36.000000 swarms-0.9.0/swarms/agents/workers/multi_modal_workers/omni_agent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-07-21 23:09:36.000000 swarms-0.9.0/swarms/agents/workers/multi_modal_workers/omni_agent/get_token_ids.py
--rw-r--r--   0 runner    (1001) docker     (123)    31378 2023-07-21 23:09:36.000000 swarms-0.9.0/swarms/agents/workers/multi_modal_workers/omni_agent/model_server.py
--rw-r--r--   0 runner    (1001) docker     (123)    45882 2023-07-21 23:09:36.000000 swarms-0.9.0/swarms/agents/workers/multi_modal_workers/omni_agent/omni_chat.py
--rw-r--r--   0 runner    (1001) docker     (123)     6904 2023-07-21 23:09:36.000000 swarms-0.9.0/swarms/agents/workers/worker_agent_ultra.py
--rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-07-21 23:09:36.000000 swarms-0.9.0/swarms/agents/workers/worker_ultra_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-07-21 23:09:36.000000 swarms-0.9.0/swarms/hivemind.py
--rw-r--r--   0 runner    (1001) docker     (123)     9240 2023-07-21 23:09:36.000000 swarms-0.9.0/swarms/swarms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 23:09:45.419401 swarms-0.9.0/swarms/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-21 23:09:36.000000 swarms-0.9.0/swarms/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 23:09:45.423401 swarms-0.9.0/swarms/utils/embeddings/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-21 23:09:36.000000 swarms-0.9.0/swarms/utils/embeddings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-21 23:09:36.000000 swarms-0.9.0/swarms/utils/embeddings/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-21 23:09:36.000000 swarms-0.9.0/swarms/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    11292 2023-07-21 23:09:36.000000 swarms-0.9.0/swarms/utils/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 23:09:45.423401 swarms-0.9.0/swarms/utils/schema/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 23:09:36.000000 swarms-0.9.0/swarms/utils/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 23:09:36.000000 swarms-0.9.0/swarms/utils/schema/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-07-21 23:09:36.000000 swarms-0.9.0/swarms/utils/static.py
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-21 23:09:36.000000 swarms-0.9.0/swarms/utils/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 23:09:45.407401 swarms-0.9.0/swarms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-21 23:09:45.000000 swarms-0.9.0/swarms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6369 2023-07-21 23:09:45.000000 swarms-0.9.0/swarms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 23:09:45.000000 swarms-0.9.0/swarms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-07-21 23:09:45.000000 swarms-0.9.0/swarms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-21 23:09:45.000000 swarms-0.9.0/swarms.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 23:15:19.190427 swarms-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-21 23:15:09.000000 swarms-0.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-21 23:15:19.190427 swarms-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15283 2023-07-21 23:15:09.000000 swarms-0.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 23:15:19.174427 swarms-0.9.1/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 23:15:09.000000 swarms-0.9.1/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-07-21 23:15:09.000000 swarms-0.9.1/api/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 23:15:19.190427 swarms-0.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-07-21 23:15:09.000000 swarms-0.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 23:15:19.174427 swarms-0.9.1/swarms/
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-21 23:15:09.000000 swarms-0.9.1/swarms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 23:15:19.174427 swarms-0.9.1/swarms/agents/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-21 23:15:09.000000 swarms-0.9.1/swarms/agents/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 23:15:19.174427 swarms-0.9.1/swarms/agents/boss/
+-rw-r--r--   0 runner    (1001) docker     (123)     5795 2023-07-21 23:15:09.000000 swarms-0.9.1/swarms/agents/boss/BossNode.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 23:15:09.000000 swarms-0.9.1/swarms/agents/boss/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 23:15:19.178427 swarms-0.9.1/swarms/agents/memory/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 23:15:09.000000 swarms-0.9.1/swarms/agents/memory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18115 2023-07-21 23:15:09.000000 swarms-0.9.1/swarms/agents/memory/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22333 2023-07-21 23:15:09.000000 swarms-0.9.1/swarms/agents/memory/chroma.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 23:15:19.178427 swarms-0.9.1/swarms/agents/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-21 23:15:09.000000 swarms-0.9.1/swarms/agents/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-07-21 23:15:09.000000 swarms-0.9.1/swarms/agents/models/llm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 23:15:19.178427 swarms-0.9.1/swarms/agents/prompts/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-21 23:15:09.000000 swarms-0.9.1/swarms/agents/prompts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-07-21 23:15:09.000000 swarms-0.9.1/swarms/agents/prompts/prompts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 23:15:19.178427 swarms-0.9.1/swarms/agents/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-21 23:15:09.000000 swarms-0.9.1/swarms/agents/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-07-21 23:15:09.000000 swarms-0.9.1/swarms/agents/tools/agent_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-07-21 23:15:09.000000 swarms-0.9.1/swarms/agents/tools/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 23:15:19.178427 swarms-0.9.1/swarms/agents/tools/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 23:15:09.000000 swarms-0.9.1/swarms/agents/tools/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 23:15:19.178427 swarms-0.9.1/swarms/agents/tools/core/code_interpreter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 23:15:09.000000 swarms-0.9.1/swarms/agents/tools/core/code_interpreter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27478 2023-07-21 23:15:09.000000 swarms-0.9.1/swarms/agents/tools/core/code_interpreter/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    73698 2023-07-21 23:15:09.000000 swarms-0.9.1/swarms/agents/tools/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 23:15:19.178427 swarms-0.9.1/swarms/agents/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)    19599 2023-07-21 23:15:09.000000 swarms-0.9.1/swarms/agents/utils/Agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6022 2023-07-21 23:15:09.000000 swarms-0.9.1/swarms/agents/utils/Calback.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13661 2023-07-21 23:15:09.000000 swarms-0.9.1/swarms/agents/utils/ChatOpenAI.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5508 2023-07-21 23:15:09.000000 swarms-0.9.1/swarms/agents/utils/ConversationalChatAgent.py
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-21 23:15:09.000000 swarms-0.9.1/swarms/agents/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3795 2023-07-21 23:15:09.000000 swarms-0.9.1/swarms/agents/utils/agent_creator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-07-21 23:15:09.000000 swarms-0.9.1/swarms/agents/utils/agent_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-07-21 23:15:09.000000 swarms-0.9.1/swarms/agents/utils/output_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6348 2023-07-21 23:15:09.000000 swarms-0.9.1/swarms/agents/utils/prompts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 23:15:19.178427 swarms-0.9.1/swarms/agents/workers/
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-21 23:15:09.000000 swarms-0.9.1/swarms/agents/workers/MultiModalVisualAgentTool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-21 23:15:09.000000 swarms-0.9.1/swarms/agents/workers/OmniWorkerAgent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-07-21 23:15:09.000000 swarms-0.9.1/swarms/agents/workers/PromptWorker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6132 2023-07-21 23:15:09.000000 swarms-0.9.1/swarms/agents/workers/WorkerNode.py
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-21 23:15:09.000000 swarms-0.9.1/swarms/agents/workers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22410 2023-07-21 23:15:09.000000 swarms-0.9.1/swarms/agents/workers/generative_worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 23:15:19.182427 swarms-0.9.1/swarms/agents/workers/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 23:15:19.182427 swarms-0.9.1/swarms/agents/workers/models/GroundingDINO/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-21 23:15:09.000000 swarms-0.9.1/swarms/agents/workers/models/GroundingDINO/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 23:15:19.182427 swarms-0.9.1/swarms/agents/workers/models/GroundingDINO/groundingdino/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 23:15:09.000000 swarms-0.9.1/swarms/agents/workers/models/GroundingDINO/groundingdino/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 23:15:19.182427 swarms-0.9.1/swarms/agents/workers/models/GroundingDINO/groundingdino/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-07-21 23:15:09.000000 swarms-0.9.1/swarms/agents/workers/models/GroundingDINO/groundingdino/config/GroundingDINO_SwinB_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-21 23:15:09.000000 swarms-0.9.1/swarms/agents/workers/models/GroundingDINO/groundingdino/config/GroundingDINO_SwinT_OGC.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 23:15:09.000000 swarms-0.9.1/swarms/agents/workers/models/GroundingDINO/groundingdino/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 23:15:19.182427 swarms-0.9.1/swarms/agents/workers/models/GroundingDINO/groundingdino/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 23:15:09.000000 swarms-0.9.1/swarms/agents/workers/models/GroundingDINO/groundingdino/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9398 2023-07-21 23:15:09.000000 swarms-0.9.1/swarms/agents/workers/models/GroundingDINO/groundingdino/datasets/cocogrounding_eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9711 2023-07-21 23:15:09.000000 swarms-0.9.1/swarms/agents/workers/models/GroundingDINO/groundingdino/datasets/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 23:15:19.182427 swarms-0.9.1/swarms/agents/workers/models/GroundingDINO/groundingdino/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 23:15:19.182427 swarms-0.9.1/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-07-21 23:15:09.000000 swarms-0.9.1/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 23:15:19.182427 swarms-0.9.1/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-21 23:15:09.000000 swarms-0.9.1/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7972 2023-07-21 23:15:09.000000 swarms-0.9.1/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/backbone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6866 2023-07-21 23:15:09.000000 swarms-0.9.1/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/position_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29339 2023-07-21 23:15:09.000000 swarms-0.9.1/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/swin_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12242 2023-07-21 23:15:09.000000 swarms-0.9.1/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/bertwarper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11825 2023-07-21 23:15:09.000000 swarms-0.9.1/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/fuse_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16669 2023-07-21 23:15:09.000000 swarms-0.9.1/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/groundingdino.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15482 2023-07-21 23:15:09.000000 swarms-0.9.1/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/ms_deform_attn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36805 2023-07-21 23:15:09.000000 swarms-0.9.1/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4020 2023-07-21 23:15:09.000000 swarms-0.9.1/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/transformer_vanilla.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10087 2023-07-21 23:15:09.000000 swarms-0.9.1/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-07-21 23:15:09.000000 swarms-0.9.1/swarms/agents/workers/models/GroundingDINO/groundingdino/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-07-21 23:15:09.000000 swarms-0.9.1/swarms/agents/workers/models/GroundingDINO/groundingdino/models/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 23:15:19.186427 swarms-0.9.1/swarms/agents/workers/models/GroundingDINO/groundingdino/util/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-21 23:15:09.000000 swarms-0.9.1/swarms/agents/workers/models/GroundingDINO/groundingdino/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-07-21 23:15:09.000000 swarms-0.9.1/swarms/agents/workers/models/GroundingDINO/groundingdino/util/box_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-07-21 23:15:09.000000 swarms-0.9.1/swarms/agents/workers/models/GroundingDINO/groundingdino/util/get_tokenlizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8745 2023-07-21 23:15:09.000000 swarms-0.9.1/swarms/agents/workers/models/GroundingDINO/groundingdino/util/inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-07-21 23:15:09.000000 swarms-0.9.1/swarms/agents/workers/models/GroundingDINO/groundingdino/util/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23348 2023-07-21 23:15:09.000000 swarms-0.9.1/swarms/agents/workers/models/GroundingDINO/groundingdino/util/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14380 2023-07-21 23:15:09.000000 swarms-0.9.1/swarms/agents/workers/models/GroundingDINO/groundingdino/util/slconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5377 2023-07-21 23:15:09.000000 swarms-0.9.1/swarms/agents/workers/models/GroundingDINO/groundingdino/util/slio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-07-21 23:15:09.000000 swarms-0.9.1/swarms/agents/workers/models/GroundingDINO/groundingdino/util/time_counter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17828 2023-07-21 23:15:09.000000 swarms-0.9.1/swarms/agents/workers/models/GroundingDINO/groundingdino/util/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12047 2023-07-21 23:15:09.000000 swarms-0.9.1/swarms/agents/workers/models/GroundingDINO/groundingdino/util/visualizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-07-21 23:15:09.000000 swarms-0.9.1/swarms/agents/workers/models/GroundingDINO/groundingdino/util/vl_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7179 2023-07-21 23:15:09.000000 swarms-0.9.1/swarms/agents/workers/models/GroundingDINO/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-07-21 23:15:09.000000 swarms-0.9.1/swarms/agents/workers/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 23:15:19.186427 swarms-0.9.1/swarms/agents/workers/models/segment_anything/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-21 23:15:09.000000 swarms-0.9.1/swarms/agents/workers/models/segment_anything/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 23:15:19.186427 swarms-0.9.1/swarms/agents/workers/models/segment_anything/segment_anything/
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-07-21 23:15:09.000000 swarms-0.9.1/swarms/agents/workers/models/segment_anything/segment_anything/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15148 2023-07-21 23:15:09.000000 swarms-0.9.1/swarms/agents/workers/models/segment_anything/segment_anything/automatic_mask_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-07-21 23:15:09.000000 swarms-0.9.1/swarms/agents/workers/models/segment_anything/segment_anything/build_sam.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 23:15:19.186427 swarms-0.9.1/swarms/agents/workers/models/segment_anything/segment_anything/modeling/
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-21 23:15:09.000000 swarms-0.9.1/swarms/agents/workers/models/segment_anything/segment_anything/modeling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-07-21 23:15:09.000000 swarms-0.9.1/swarms/agents/workers/models/segment_anything/segment_anything/modeling/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14420 2023-07-21 23:15:09.000000 swarms-0.9.1/swarms/agents/workers/models/segment_anything/segment_anything/modeling/image_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6615 2023-07-21 23:15:09.000000 swarms-0.9.1/swarms/agents/workers/models/segment_anything/segment_anything/modeling/mask_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8594 2023-07-21 23:15:09.000000 swarms-0.9.1/swarms/agents/workers/models/segment_anything/segment_anything/modeling/prompt_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-07-21 23:15:09.000000 swarms-0.9.1/swarms/agents/workers/models/segment_anything/segment_anything/modeling/sam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8397 2023-07-21 23:15:09.000000 swarms-0.9.1/swarms/agents/workers/models/segment_anything/segment_anything/modeling/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11649 2023-07-21 23:15:09.000000 swarms-0.9.1/swarms/agents/workers/models/segment_anything/segment_anything/predictor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 23:15:19.186427 swarms-0.9.1/swarms/agents/workers/models/segment_anything/segment_anything/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-21 23:15:09.000000 swarms-0.9.1/swarms/agents/workers/models/segment_anything/segment_anything/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12712 2023-07-21 23:15:09.000000 swarms-0.9.1/swarms/agents/workers/models/segment_anything/segment_anything/utils/amg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5812 2023-07-21 23:15:09.000000 swarms-0.9.1/swarms/agents/workers/models/segment_anything/segment_anything/utils/onnx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-07-21 23:15:09.000000 swarms-0.9.1/swarms/agents/workers/models/segment_anything/segment_anything/utils/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-07-21 23:15:09.000000 swarms-0.9.1/swarms/agents/workers/models/segment_anything/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 23:15:19.186427 swarms-0.9.1/swarms/agents/workers/multi_modal_workers/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-21 23:15:09.000000 swarms-0.9.1/swarms/agents/workers/multi_modal_workers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79584 2023-07-21 23:15:09.000000 swarms-0.9.1/swarms/agents/workers/multi_modal_workers/multi_modal_agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 23:15:19.190427 swarms-0.9.1/swarms/agents/workers/multi_modal_workers/omni_agent/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 23:15:09.000000 swarms-0.9.1/swarms/agents/workers/multi_modal_workers/omni_agent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-07-21 23:15:09.000000 swarms-0.9.1/swarms/agents/workers/multi_modal_workers/omni_agent/get_token_ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31378 2023-07-21 23:15:09.000000 swarms-0.9.1/swarms/agents/workers/multi_modal_workers/omni_agent/model_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45882 2023-07-21 23:15:09.000000 swarms-0.9.1/swarms/agents/workers/multi_modal_workers/omni_agent/omni_chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6904 2023-07-21 23:15:09.000000 swarms-0.9.1/swarms/agents/workers/worker_agent_ultra.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-07-21 23:15:09.000000 swarms-0.9.1/swarms/agents/workers/worker_ultra_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-07-21 23:15:09.000000 swarms-0.9.1/swarms/hivemind.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9240 2023-07-21 23:15:09.000000 swarms-0.9.1/swarms/swarms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 23:15:19.190427 swarms-0.9.1/swarms/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-21 23:15:09.000000 swarms-0.9.1/swarms/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 23:15:19.190427 swarms-0.9.1/swarms/utils/embeddings/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-21 23:15:09.000000 swarms-0.9.1/swarms/utils/embeddings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-21 23:15:09.000000 swarms-0.9.1/swarms/utils/embeddings/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-21 23:15:09.000000 swarms-0.9.1/swarms/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11292 2023-07-21 23:15:09.000000 swarms-0.9.1/swarms/utils/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 23:15:19.190427 swarms-0.9.1/swarms/utils/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 23:15:09.000000 swarms-0.9.1/swarms/utils/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 23:15:09.000000 swarms-0.9.1/swarms/utils/schema/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-07-21 23:15:09.000000 swarms-0.9.1/swarms/utils/static.py
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-21 23:15:09.000000 swarms-0.9.1/swarms/utils/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 23:15:19.174427 swarms-0.9.1/swarms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-21 23:15:19.000000 swarms-0.9.1/swarms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6369 2023-07-21 23:15:19.000000 swarms-0.9.1/swarms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 23:15:19.000000 swarms-0.9.1/swarms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-07-21 23:15:19.000000 swarms-0.9.1/swarms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-21 23:15:19.000000 swarms-0.9.1/swarms.egg-info/top_level.txt
```

### Comparing `swarms-0.9.0/LICENSE` & `swarms-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `swarms-0.9.0/PKG-INFO` & `swarms-0.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swarms
-Version: 0.9.0
+Version: 0.9.1
 Summary: Swarms - Pytorch
 Home-page: https://github.com/kyegomez/swarms
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `swarms-0.9.0/README.md` & `swarms-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `swarms-0.9.0/api/app.py` & `swarms-0.9.1/api/app.py`

 * *Files identical despite different names*

### Comparing `swarms-0.9.0/setup.py` & `swarms-0.9.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 ##
 
 setup(
   name = 'swarms',
   packages = find_packages(exclude=[]),
-  version = '0.9.0',
+  version = '0.9.1',
   license='MIT',
   description = 'Swarms - Pytorch',
   author = 'Kye Gomez',
   author_email = 'kye@apac.ai',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/kyegomez/swarms',
   keywords = [
```

### Comparing `swarms-0.9.0/swarms/agents/boss/BossNode.py` & `swarms-0.9.1/swarms/agents/boss/BossNode.py`

 * *Files identical despite different names*

### Comparing `swarms-0.9.0/swarms/agents/memory/base.py` & `swarms-0.9.1/swarms/agents/memory/base.py`

 * *Files identical despite different names*

### Comparing `swarms-0.9.0/swarms/agents/memory/chroma.py` & `swarms-0.9.1/swarms/agents/memory/chroma.py`

 * *Files identical despite different names*

### Comparing `swarms-0.9.0/swarms/agents/models/llm.py` & `swarms-0.9.1/swarms/agents/models/llm.py`

 * *Files identical despite different names*

### Comparing `swarms-0.9.0/swarms/agents/prompts/prompts.py` & `swarms-0.9.1/swarms/agents/prompts/prompts.py`

 * *Files identical despite different names*

### Comparing `swarms-0.9.0/swarms/agents/tools/agent_tools.py` & `swarms-0.9.1/swarms/agents/tools/agent_tools.py`

 * *Files identical despite different names*

### Comparing `swarms-0.9.0/swarms/agents/tools/base.py` & `swarms-0.9.1/swarms/agents/tools/base.py`

 * *Files identical despite different names*

### Comparing `swarms-0.9.0/swarms/agents/tools/core/code_interpreter/main.py` & `swarms-0.9.1/swarms/agents/tools/core/code_interpreter/main.py`

 * *Files identical despite different names*

### Comparing `swarms-0.9.0/swarms/agents/tools/main.py` & `swarms-0.9.1/swarms/agents/tools/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -1304,15 +1304,15 @@
 #========================> handlers/image
 import torch
 from PIL import Image
 from transformers import BlipForConditionalGeneration, BlipProcessor
 
 # from core.prompts.file import IMAGE_PROMPT
 # from swarms.agents.prompts import IMAGE_PROMPT
-from swarms.agents.prompts import IMAGE_PROMPT
+from swarms.agents.prompts.prompts import IMAGE_PROMPT
 
 from swarms.utils.main import BaseHandler
 
 class ImageCaptioning(BaseHandler):
     def __init__(self, device):
         print("Initializing ImageCaptioning to %s" % device)
         self.device = device
```

### Comparing `swarms-0.9.0/swarms/agents/utils/Agent.py` & `swarms-0.9.1/swarms/agents/utils/Agent.py`

 * *Files identical despite different names*

### Comparing `swarms-0.9.0/swarms/agents/utils/Calback.py` & `swarms-0.9.1/swarms/agents/utils/Calback.py`

 * *Files identical despite different names*

### Comparing `swarms-0.9.0/swarms/agents/utils/ChatOpenAI.py` & `swarms-0.9.1/swarms/agents/utils/ChatOpenAI.py`

 * *Files identical despite different names*

### Comparing `swarms-0.9.0/swarms/agents/utils/ConversationalChatAgent.py` & `swarms-0.9.1/swarms/agents/utils/ConversationalChatAgent.py`

 * *Files identical despite different names*

### Comparing `swarms-0.9.0/swarms/agents/utils/agent_creator.py` & `swarms-0.9.1/swarms/agents/utils/agent_creator.py`

 * *Files identical despite different names*

### Comparing `swarms-0.9.0/swarms/agents/utils/agent_setup.py` & `swarms-0.9.1/swarms/agents/utils/agent_setup.py`

 * *Files identical despite different names*

### Comparing `swarms-0.9.0/swarms/agents/utils/output_parser.py` & `swarms-0.9.1/swarms/agents/utils/output_parser.py`

 * *Files identical despite different names*

### Comparing `swarms-0.9.0/swarms/agents/utils/prompts.py` & `swarms-0.9.1/swarms/agents/utils/prompts.py`

 * *Files identical despite different names*

### Comparing `swarms-0.9.0/swarms/agents/workers/MultiModalVisualAgentTool.py` & `swarms-0.9.1/swarms/agents/workers/MultiModalVisualAgentTool.py`

 * *Files identical despite different names*

### Comparing `swarms-0.9.0/swarms/agents/workers/OmniWorkerAgent.py` & `swarms-0.9.1/swarms/agents/workers/OmniWorkerAgent.py`

 * *Files identical despite different names*

### Comparing `swarms-0.9.0/swarms/agents/workers/PromptWorker.py` & `swarms-0.9.1/swarms/agents/workers/PromptWorker.py`

 * *Files identical despite different names*

### Comparing `swarms-0.9.0/swarms/agents/workers/WorkerNode.py` & `swarms-0.9.1/swarms/agents/workers/WorkerNode.py`

 * *Files identical despite different names*

### Comparing `swarms-0.9.0/swarms/agents/workers/generative_worker.py` & `swarms-0.9.1/swarms/agents/workers/generative_worker.py`

 * *Files identical despite different names*

### Comparing `swarms-0.9.0/swarms/agents/workers/models/GroundingDINO/groundingdino/config/GroundingDINO_SwinB_cfg.py` & `swarms-0.9.1/swarms/agents/workers/models/GroundingDINO/groundingdino/config/GroundingDINO_SwinB_cfg.py`

 * *Files identical despite different names*

### Comparing `swarms-0.9.0/swarms/agents/workers/models/GroundingDINO/groundingdino/config/GroundingDINO_SwinT_OGC.py` & `swarms-0.9.1/swarms/agents/workers/models/GroundingDINO/groundingdino/config/GroundingDINO_SwinT_OGC.py`

 * *Files identical despite different names*

### Comparing `swarms-0.9.0/swarms/agents/workers/models/GroundingDINO/groundingdino/datasets/cocogrounding_eval.py` & `swarms-0.9.1/swarms/agents/workers/models/GroundingDINO/groundingdino/datasets/cocogrounding_eval.py`

 * *Files identical despite different names*

### Comparing `swarms-0.9.0/swarms/agents/workers/models/GroundingDINO/groundingdino/datasets/transforms.py` & `swarms-0.9.1/swarms/agents/workers/models/GroundingDINO/groundingdino/datasets/transforms.py`

 * *Files identical despite different names*

### Comparing `swarms-0.9.0/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/__init__.py` & `swarms-0.9.1/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/__init__.py`

 * *Files identical despite different names*

### Comparing `swarms-0.9.0/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/backbone.py` & `swarms-0.9.1/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/backbone.py`

 * *Files identical despite different names*

### Comparing `swarms-0.9.0/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/position_encoding.py` & `swarms-0.9.1/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/position_encoding.py`

 * *Files identical despite different names*

### Comparing `swarms-0.9.0/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/swin_transformer.py` & `swarms-0.9.1/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/swin_transformer.py`

 * *Files identical despite different names*

### Comparing `swarms-0.9.0/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/bertwarper.py` & `swarms-0.9.1/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/bertwarper.py`

 * *Files identical despite different names*

### Comparing `swarms-0.9.0/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/fuse_modules.py` & `swarms-0.9.1/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/fuse_modules.py`

 * *Files identical despite different names*

### Comparing `swarms-0.9.0/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/groundingdino.py` & `swarms-0.9.1/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/groundingdino.py`

 * *Files identical despite different names*

### Comparing `swarms-0.9.0/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/ms_deform_attn.py` & `swarms-0.9.1/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/ms_deform_attn.py`

 * *Files identical despite different names*

### Comparing `swarms-0.9.0/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/transformer.py` & `swarms-0.9.1/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/transformer.py`

 * *Files identical despite different names*

### Comparing `swarms-0.9.0/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/transformer_vanilla.py` & `swarms-0.9.1/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/transformer_vanilla.py`

 * *Files identical despite different names*

### Comparing `swarms-0.9.0/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/utils.py` & `swarms-0.9.1/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/utils.py`

 * *Files identical despite different names*

### Comparing `swarms-0.9.0/swarms/agents/workers/models/GroundingDINO/groundingdino/models/__init__.py` & `swarms-0.9.1/swarms/agents/workers/models/GroundingDINO/groundingdino/models/__init__.py`

 * *Files identical despite different names*

### Comparing `swarms-0.9.0/swarms/agents/workers/models/GroundingDINO/groundingdino/models/registry.py` & `swarms-0.9.1/swarms/agents/workers/models/GroundingDINO/groundingdino/models/registry.py`

 * *Files identical despite different names*

### Comparing `swarms-0.9.0/swarms/agents/workers/models/GroundingDINO/groundingdino/util/box_ops.py` & `swarms-0.9.1/swarms/agents/workers/models/GroundingDINO/groundingdino/util/box_ops.py`

 * *Files identical despite different names*

### Comparing `swarms-0.9.0/swarms/agents/workers/models/GroundingDINO/groundingdino/util/get_tokenlizer.py` & `swarms-0.9.1/swarms/agents/workers/models/GroundingDINO/groundingdino/util/get_tokenlizer.py`

 * *Files identical despite different names*

### Comparing `swarms-0.9.0/swarms/agents/workers/models/GroundingDINO/groundingdino/util/inference.py` & `swarms-0.9.1/swarms/agents/workers/models/GroundingDINO/groundingdino/util/inference.py`

 * *Files identical despite different names*

### Comparing `swarms-0.9.0/swarms/agents/workers/models/GroundingDINO/groundingdino/util/logger.py` & `swarms-0.9.1/swarms/agents/workers/models/GroundingDINO/groundingdino/util/logger.py`

 * *Files identical despite different names*

### Comparing `swarms-0.9.0/swarms/agents/workers/models/GroundingDINO/groundingdino/util/misc.py` & `swarms-0.9.1/swarms/agents/workers/models/GroundingDINO/groundingdino/util/misc.py`

 * *Files identical despite different names*

### Comparing `swarms-0.9.0/swarms/agents/workers/models/GroundingDINO/groundingdino/util/slconfig.py` & `swarms-0.9.1/swarms/agents/workers/models/GroundingDINO/groundingdino/util/slconfig.py`

 * *Files identical despite different names*

### Comparing `swarms-0.9.0/swarms/agents/workers/models/GroundingDINO/groundingdino/util/slio.py` & `swarms-0.9.1/swarms/agents/workers/models/GroundingDINO/groundingdino/util/slio.py`

 * *Files identical despite different names*

### Comparing `swarms-0.9.0/swarms/agents/workers/models/GroundingDINO/groundingdino/util/time_counter.py` & `swarms-0.9.1/swarms/agents/workers/models/GroundingDINO/groundingdino/util/time_counter.py`

 * *Files identical despite different names*

### Comparing `swarms-0.9.0/swarms/agents/workers/models/GroundingDINO/groundingdino/util/utils.py` & `swarms-0.9.1/swarms/agents/workers/models/GroundingDINO/groundingdino/util/utils.py`

 * *Files identical despite different names*

### Comparing `swarms-0.9.0/swarms/agents/workers/models/GroundingDINO/groundingdino/util/visualizer.py` & `swarms-0.9.1/swarms/agents/workers/models/GroundingDINO/groundingdino/util/visualizer.py`

 * *Files identical despite different names*

### Comparing `swarms-0.9.0/swarms/agents/workers/models/GroundingDINO/groundingdino/util/vl_utils.py` & `swarms-0.9.1/swarms/agents/workers/models/GroundingDINO/groundingdino/util/vl_utils.py`

 * *Files identical despite different names*

### Comparing `swarms-0.9.0/swarms/agents/workers/models/GroundingDINO/setup.py` & `swarms-0.9.1/swarms/agents/workers/models/GroundingDINO/setup.py`

 * *Files identical despite different names*

### Comparing `swarms-0.9.0/swarms/agents/workers/models/__init__.py` & `swarms-0.9.1/swarms/agents/workers/models/__init__.py`

 * *Files identical despite different names*

### Comparing `swarms-0.9.0/swarms/agents/workers/models/segment_anything/segment_anything/automatic_mask_generator.py` & `swarms-0.9.1/swarms/agents/workers/models/segment_anything/segment_anything/automatic_mask_generator.py`

 * *Files identical despite different names*

### Comparing `swarms-0.9.0/swarms/agents/workers/models/segment_anything/segment_anything/build_sam.py` & `swarms-0.9.1/swarms/agents/workers/models/segment_anything/segment_anything/build_sam.py`

 * *Files identical despite different names*

### Comparing `swarms-0.9.0/swarms/agents/workers/models/segment_anything/segment_anything/modeling/common.py` & `swarms-0.9.1/swarms/agents/workers/models/segment_anything/segment_anything/modeling/common.py`

 * *Files identical despite different names*

### Comparing `swarms-0.9.0/swarms/agents/workers/models/segment_anything/segment_anything/modeling/image_encoder.py` & `swarms-0.9.1/swarms/agents/workers/models/segment_anything/segment_anything/modeling/image_encoder.py`

 * *Files identical despite different names*

### Comparing `swarms-0.9.0/swarms/agents/workers/models/segment_anything/segment_anything/modeling/mask_decoder.py` & `swarms-0.9.1/swarms/agents/workers/models/segment_anything/segment_anything/modeling/mask_decoder.py`

 * *Files identical despite different names*

### Comparing `swarms-0.9.0/swarms/agents/workers/models/segment_anything/segment_anything/modeling/prompt_encoder.py` & `swarms-0.9.1/swarms/agents/workers/models/segment_anything/segment_anything/modeling/prompt_encoder.py`

 * *Files identical despite different names*

### Comparing `swarms-0.9.0/swarms/agents/workers/models/segment_anything/segment_anything/modeling/sam.py` & `swarms-0.9.1/swarms/agents/workers/models/segment_anything/segment_anything/modeling/sam.py`

 * *Files identical despite different names*

### Comparing `swarms-0.9.0/swarms/agents/workers/models/segment_anything/segment_anything/modeling/transformer.py` & `swarms-0.9.1/swarms/agents/workers/models/segment_anything/segment_anything/modeling/transformer.py`

 * *Files identical despite different names*

### Comparing `swarms-0.9.0/swarms/agents/workers/models/segment_anything/segment_anything/predictor.py` & `swarms-0.9.1/swarms/agents/workers/models/segment_anything/segment_anything/predictor.py`

 * *Files identical despite different names*

### Comparing `swarms-0.9.0/swarms/agents/workers/models/segment_anything/segment_anything/utils/amg.py` & `swarms-0.9.1/swarms/agents/workers/models/segment_anything/segment_anything/utils/amg.py`

 * *Files identical despite different names*

### Comparing `swarms-0.9.0/swarms/agents/workers/models/segment_anything/segment_anything/utils/onnx.py` & `swarms-0.9.1/swarms/agents/workers/models/segment_anything/segment_anything/utils/onnx.py`

 * *Files identical despite different names*

### Comparing `swarms-0.9.0/swarms/agents/workers/models/segment_anything/segment_anything/utils/transforms.py` & `swarms-0.9.1/swarms/agents/workers/models/segment_anything/segment_anything/utils/transforms.py`

 * *Files identical despite different names*

### Comparing `swarms-0.9.0/swarms/agents/workers/models/segment_anything/setup.py` & `swarms-0.9.1/swarms/agents/workers/models/segment_anything/setup.py`

 * *Files identical despite different names*

### Comparing `swarms-0.9.0/swarms/agents/workers/multi_modal_workers/multi_modal_agent.py` & `swarms-0.9.1/swarms/agents/workers/multi_modal_workers/multi_modal_agent.py`

 * *Files identical despite different names*

### Comparing `swarms-0.9.0/swarms/agents/workers/multi_modal_workers/omni_agent/get_token_ids.py` & `swarms-0.9.1/swarms/agents/workers/multi_modal_workers/omni_agent/get_token_ids.py`

 * *Files identical despite different names*

### Comparing `swarms-0.9.0/swarms/agents/workers/multi_modal_workers/omni_agent/model_server.py` & `swarms-0.9.1/swarms/agents/workers/multi_modal_workers/omni_agent/model_server.py`

 * *Files identical despite different names*

### Comparing `swarms-0.9.0/swarms/agents/workers/multi_modal_workers/omni_agent/omni_chat.py` & `swarms-0.9.1/swarms/agents/workers/multi_modal_workers/omni_agent/omni_chat.py`

 * *Files identical despite different names*

### Comparing `swarms-0.9.0/swarms/agents/workers/worker_agent_ultra.py` & `swarms-0.9.1/swarms/agents/workers/worker_agent_ultra.py`

 * *Files identical despite different names*

### Comparing `swarms-0.9.0/swarms/agents/workers/worker_ultra_node.py` & `swarms-0.9.1/swarms/agents/workers/worker_ultra_node.py`

 * *Files identical despite different names*

### Comparing `swarms-0.9.0/swarms/hivemind.py` & `swarms-0.9.1/swarms/hivemind.py`

 * *Files identical despite different names*

### Comparing `swarms-0.9.0/swarms/swarms.py` & `swarms-0.9.1/swarms/swarms.py`

 * *Files identical despite different names*

### Comparing `swarms-0.9.0/swarms/utils/embeddings/base.py` & `swarms-0.9.1/swarms/utils/embeddings/base.py`

 * *Files identical despite different names*

### Comparing `swarms-0.9.0/swarms/utils/main.py` & `swarms-0.9.1/swarms/utils/main.py`

 * *Files identical despite different names*

### Comparing `swarms-0.9.0/swarms/utils/static.py` & `swarms-0.9.1/swarms/utils/static.py`

 * *Files identical despite different names*

### Comparing `swarms-0.9.0/swarms.egg-info/PKG-INFO` & `swarms-0.9.1/swarms.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swarms
-Version: 0.9.0
+Version: 0.9.1
 Summary: Swarms - Pytorch
 Home-page: https://github.com/kyegomez/swarms
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `swarms-0.9.0/swarms.egg-info/SOURCES.txt` & `swarms-0.9.1/swarms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `swarms-0.9.0/swarms.egg-info/requires.txt` & `swarms-0.9.1/swarms.egg-info/requires.txt`

 * *Files identical despite different names*

