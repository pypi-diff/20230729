# Comparing `tmp/swarms-1.1.2.tar.gz` & `tmp/swarms-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swarms-1.1.2.tar", last modified: Fri Jul 28 17:16:26 2023, max compression
+gzip compressed data, was "swarms-1.1.3.tar", last modified: Sat Jul 29 14:56:55 2023, max compression
```

## Comparing `swarms-1.1.2.tar` & `swarms-1.1.3.tar`

### file list

```diff
@@ -1,160 +1,160 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:16:26.485408 swarms-1.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-28 17:16:14.000000 swarms-1.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-28 17:16:26.485408 swarms-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14777 2023-07-28 17:16:14.000000 swarms-1.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:16:26.465408 swarms-1.1.2/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 17:16:14.000000 swarms-1.1.2/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-07-28 17:16:14.000000 swarms-1.1.2/api/app.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 17:16:26.485408 swarms-1.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-07-28 17:16:14.000000 swarms-1.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:16:26.465408 swarms-1.1.2/swarms/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:16:26.465408 swarms-1.1.2/swarms/agents/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/agents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7667 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/agents/agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/agents/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:16:26.465408 swarms-1.1.2/swarms/agents/memory/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/agents/memory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18113 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/agents/memory/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    22333 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/agents/memory/chroma.py
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/agents/memory/ocean.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/agents/memory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:16:26.469408 swarms-1.1.2/swarms/agents/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/agents/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/agents/models/hf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/agents/models/llm.py
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/agents/models/petals_hf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:16:26.469408 swarms-1.1.2/swarms/agents/prompts/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/agents/prompts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/agents/prompts/agent_prompt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:16:26.469408 swarms-1.1.2/swarms/agents/prompts/chains/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/agents/prompts/chains/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12127 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/agents/prompts/chains/llm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/agents/prompts/prompts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:16:26.469408 swarms-1.1.2/swarms/agents/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/agents/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/agents/tools/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:16:26.469408 swarms-1.1.2/swarms/agents/tools/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/agents/tools/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:16:26.469408 swarms-1.1.2/swarms/agents/tools/core/code_interpreter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/agents/tools/core/code_interpreter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27427 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/agents/tools/core/code_interpreter/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    73260 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/agents/tools/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:16:26.469408 swarms-1.1.2/swarms/agents/utils/
--rw-r--r--   0 runner    (1001) docker     (123)    19268 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/agents/utils/Agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     6020 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/agents/utils/Calback.py
--rw-r--r--   0 runner    (1001) docker     (123)    13650 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/agents/utils/ChatOpenAI.py
--rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/agents/utils/ConversationalChatAgent.py
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/agents/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/agents/utils/agent_creator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/agents/utils/agent_setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/agents/utils/output_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     6348 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/agents/utils/prompts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:16:26.469408 swarms-1.1.2/swarms/boss/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/boss/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6114 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/boss/boss_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/hivemind.py
--rw-r--r--   0 runner    (1001) docker     (123)     6470 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/orchestrate.py
--rw-r--r--   0 runner    (1001) docker     (123)    11311 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/swarms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:16:26.473408 swarms-1.1.2/swarms/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:16:26.473408 swarms-1.1.2/swarms/utils/embeddings/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/utils/embeddings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/utils/embeddings/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/utils/embeddings/pegasus.py
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    11292 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/utils/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:16:26.473408 swarms-1.1.2/swarms/utils/schema/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/utils/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/utils/schema/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/utils/static.py
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/utils/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:16:26.473408 swarms-1.1.2/swarms/workers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/workers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10799 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/workers/character_generative.py
--rw-r--r--   0 runner    (1001) docker     (123)    12475 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/workers/generative_worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:16:26.473408 swarms-1.1.2/swarms/workers/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:16:26.473408 swarms-1.1.2/swarms/workers/models/GroundingDINO/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/workers/models/GroundingDINO/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:16:26.473408 swarms-1.1.2/swarms/workers/models/GroundingDINO/groundingdino/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/workers/models/GroundingDINO/groundingdino/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:16:26.473408 swarms-1.1.2/swarms/workers/models/GroundingDINO/groundingdino/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/workers/models/GroundingDINO/groundingdino/config/GroundingDINO_SwinB_cfg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/workers/models/GroundingDINO/groundingdino/config/GroundingDINO_SwinT_OGC.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/workers/models/GroundingDINO/groundingdino/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:16:26.477408 swarms-1.1.2/swarms/workers/models/GroundingDINO/groundingdino/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/workers/models/GroundingDINO/groundingdino/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9398 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/workers/models/GroundingDINO/groundingdino/datasets/cocogrounding_eval.py
--rw-r--r--   0 runner    (1001) docker     (123)     9711 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/workers/models/GroundingDINO/groundingdino/datasets/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:16:26.477408 swarms-1.1.2/swarms/workers/models/GroundingDINO/groundingdino/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:16:26.477408 swarms-1.1.2/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:16:26.477408 swarms-1.1.2/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7954 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/backbone.py
--rw-r--r--   0 runner    (1001) docker     (123)     6866 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/position_encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)    29339 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/swin_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    12052 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/bertwarper.py
--rw-r--r--   0 runner    (1001) docker     (123)    11825 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/fuse_modules.py
--rw-r--r--   0 runner    (1001) docker     (123)    16158 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/groundingdino.py
--rw-r--r--   0 runner    (1001) docker     (123)    15482 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/ms_deform_attn.py
--rw-r--r--   0 runner    (1001) docker     (123)    36750 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3889 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/transformer_vanilla.py
--rw-r--r--   0 runner    (1001) docker     (123)    10087 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/workers/models/GroundingDINO/groundingdino/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/workers/models/GroundingDINO/groundingdino/models/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:16:26.481408 swarms-1.1.2/swarms/workers/models/GroundingDINO/groundingdino/util/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/workers/models/GroundingDINO/groundingdino/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/workers/models/GroundingDINO/groundingdino/util/box_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/workers/models/GroundingDINO/groundingdino/util/get_tokenlizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8745 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/workers/models/GroundingDINO/groundingdino/util/inference.py
--rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/workers/models/GroundingDINO/groundingdino/util/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    23348 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/workers/models/GroundingDINO/groundingdino/util/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)    14380 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/workers/models/GroundingDINO/groundingdino/util/slconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     5377 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/workers/models/GroundingDINO/groundingdino/util/slio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/workers/models/GroundingDINO/groundingdino/util/time_counter.py
--rw-r--r--   0 runner    (1001) docker     (123)    17839 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/workers/models/GroundingDINO/groundingdino/util/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    12036 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/workers/models/GroundingDINO/groundingdino/util/visualizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/workers/models/GroundingDINO/groundingdino/util/vl_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7179 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/workers/models/GroundingDINO/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/workers/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:16:26.481408 swarms-1.1.2/swarms/workers/models/segment_anything/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/workers/models/segment_anything/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:16:26.481408 swarms-1.1.2/swarms/workers/models/segment_anything/segment_anything/
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/workers/models/segment_anything/segment_anything/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15148 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/workers/models/segment_anything/segment_anything/automatic_mask_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/workers/models/segment_anything/segment_anything/build_sam.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:16:26.481408 swarms-1.1.2/swarms/workers/models/segment_anything/segment_anything/modeling/
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/workers/models/segment_anything/segment_anything/modeling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/workers/models/segment_anything/segment_anything/modeling/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    14420 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/workers/models/segment_anything/segment_anything/modeling/image_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     6615 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/workers/models/segment_anything/segment_anything/modeling/mask_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     8594 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/workers/models/segment_anything/segment_anything/modeling/prompt_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/workers/models/segment_anything/segment_anything/modeling/sam.py
--rw-r--r--   0 runner    (1001) docker     (123)     8397 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/workers/models/segment_anything/segment_anything/modeling/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11649 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/workers/models/segment_anything/segment_anything/predictor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:16:26.481408 swarms-1.1.2/swarms/workers/models/segment_anything/segment_anything/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/workers/models/segment_anything/segment_anything/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12712 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/workers/models/segment_anything/segment_anything/utils/amg.py
--rw-r--r--   0 runner    (1001) docker     (123)     5812 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/workers/models/segment_anything/segment_anything/utils/onnx.py
--rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/workers/models/segment_anything/segment_anything/utils/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/workers/models/segment_anything/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/workers/multi_modal_worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:16:26.481408 swarms-1.1.2/swarms/workers/multi_modal_workers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/workers/multi_modal_workers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    79017 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/workers/multi_modal_workers/multi_modal_agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:16:26.481408 swarms-1.1.2/swarms/workers/multi_modal_workers/omni_agent/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/workers/multi_modal_workers/omni_agent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/workers/multi_modal_workers/omni_agent/get_token_ids.py
--rw-r--r--   0 runner    (1001) docker     (123)    31031 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/workers/multi_modal_workers/omni_agent/model_server.py
--rw-r--r--   0 runner    (1001) docker     (123)    45794 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/workers/multi_modal_workers/omni_agent/omni_chat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/workers/omni_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     6650 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/workers/worker_agent_ultra.py
--rw-r--r--   0 runner    (1001) docker     (123)     6547 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/workers/worker_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-07-28 17:16:14.000000 swarms-1.1.2/swarms/workers/worker_ultra_node.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:16:26.465408 swarms-1.1.2/swarms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-28 17:16:26.000000 swarms-1.1.2/swarms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6182 2023-07-28 17:16:26.000000 swarms-1.1.2/swarms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 17:16:26.000000 swarms-1.1.2/swarms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-07-28 17:16:26.000000 swarms-1.1.2/swarms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-28 17:16:26.000000 swarms-1.1.2/swarms.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:56:55.770467 swarms-1.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-29 14:56:45.000000 swarms-1.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-29 14:56:55.770467 swarms-1.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15788 2023-07-29 14:56:45.000000 swarms-1.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:56:55.746467 swarms-1.1.3/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 14:56:45.000000 swarms-1.1.3/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-07-29 14:56:45.000000 swarms-1.1.3/api/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 14:56:55.770467 swarms-1.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-07-29 14:56:45.000000 swarms-1.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:56:55.746467 swarms-1.1.3/swarms/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:56:55.746467 swarms-1.1.3/swarms/agents/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/agents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7667 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/agents/agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/agents/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:56:55.750467 swarms-1.1.3/swarms/agents/memory/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/agents/memory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18113 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/agents/memory/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22333 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/agents/memory/chroma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/agents/memory/ocean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/agents/memory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:56:55.750467 swarms-1.1.3/swarms/agents/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/agents/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/agents/models/hf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/agents/models/llm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/agents/models/petals_hf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:56:55.750467 swarms-1.1.3/swarms/agents/prompts/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/agents/prompts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/agents/prompts/agent_prompt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:56:55.750467 swarms-1.1.3/swarms/agents/prompts/chains/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/agents/prompts/chains/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12127 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/agents/prompts/chains/llm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/agents/prompts/prompts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:56:55.750467 swarms-1.1.3/swarms/agents/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/agents/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/agents/tools/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:56:55.754467 swarms-1.1.3/swarms/agents/tools/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/agents/tools/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:56:55.754467 swarms-1.1.3/swarms/agents/tools/core/code_interpreter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/agents/tools/core/code_interpreter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27427 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/agents/tools/core/code_interpreter/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    73260 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/agents/tools/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:56:55.754467 swarms-1.1.3/swarms/agents/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)    19268 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/agents/utils/Agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6020 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/agents/utils/Calback.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13650 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/agents/utils/ChatOpenAI.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/agents/utils/ConversationalChatAgent.py
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/agents/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/agents/utils/agent_creator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/agents/utils/agent_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/agents/utils/output_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6348 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/agents/utils/prompts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:56:55.754467 swarms-1.1.3/swarms/boss/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/boss/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6114 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/boss/boss_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/hivemind.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6470 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/orchestrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10449 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/swarms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:56:55.754467 swarms-1.1.3/swarms/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:56:55.758468 swarms-1.1.3/swarms/utils/embeddings/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/utils/embeddings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/utils/embeddings/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/utils/embeddings/pegasus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11292 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/utils/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:56:55.758468 swarms-1.1.3/swarms/utils/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/utils/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/utils/schema/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/utils/static.py
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/utils/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:56:55.758468 swarms-1.1.3/swarms/workers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/workers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10799 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/workers/character_generative.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12475 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/workers/generative_worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:56:55.758468 swarms-1.1.3/swarms/workers/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:56:55.758468 swarms-1.1.3/swarms/workers/models/GroundingDINO/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/workers/models/GroundingDINO/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:56:55.758468 swarms-1.1.3/swarms/workers/models/GroundingDINO/groundingdino/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/workers/models/GroundingDINO/groundingdino/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:56:55.758468 swarms-1.1.3/swarms/workers/models/GroundingDINO/groundingdino/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/workers/models/GroundingDINO/groundingdino/config/GroundingDINO_SwinB_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/workers/models/GroundingDINO/groundingdino/config/GroundingDINO_SwinT_OGC.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/workers/models/GroundingDINO/groundingdino/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:56:55.758468 swarms-1.1.3/swarms/workers/models/GroundingDINO/groundingdino/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/workers/models/GroundingDINO/groundingdino/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9398 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/workers/models/GroundingDINO/groundingdino/datasets/cocogrounding_eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9711 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/workers/models/GroundingDINO/groundingdino/datasets/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:56:55.758468 swarms-1.1.3/swarms/workers/models/GroundingDINO/groundingdino/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:56:55.762467 swarms-1.1.3/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:56:55.762467 swarms-1.1.3/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7954 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/backbone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6866 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/position_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29339 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/swin_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12052 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/bertwarper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11825 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/fuse_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16158 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/groundingdino.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15482 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/ms_deform_attn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36750 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3889 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/transformer_vanilla.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10087 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/workers/models/GroundingDINO/groundingdino/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/workers/models/GroundingDINO/groundingdino/models/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:56:55.766467 swarms-1.1.3/swarms/workers/models/GroundingDINO/groundingdino/util/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/workers/models/GroundingDINO/groundingdino/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/workers/models/GroundingDINO/groundingdino/util/box_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/workers/models/GroundingDINO/groundingdino/util/get_tokenlizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8745 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/workers/models/GroundingDINO/groundingdino/util/inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/workers/models/GroundingDINO/groundingdino/util/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23348 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/workers/models/GroundingDINO/groundingdino/util/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14380 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/workers/models/GroundingDINO/groundingdino/util/slconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5377 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/workers/models/GroundingDINO/groundingdino/util/slio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/workers/models/GroundingDINO/groundingdino/util/time_counter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17839 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/workers/models/GroundingDINO/groundingdino/util/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12036 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/workers/models/GroundingDINO/groundingdino/util/visualizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/workers/models/GroundingDINO/groundingdino/util/vl_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7179 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/workers/models/GroundingDINO/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/workers/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:56:55.766467 swarms-1.1.3/swarms/workers/models/segment_anything/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/workers/models/segment_anything/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:56:55.766467 swarms-1.1.3/swarms/workers/models/segment_anything/segment_anything/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/workers/models/segment_anything/segment_anything/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15148 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/workers/models/segment_anything/segment_anything/automatic_mask_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/workers/models/segment_anything/segment_anything/build_sam.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:56:55.766467 swarms-1.1.3/swarms/workers/models/segment_anything/segment_anything/modeling/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/workers/models/segment_anything/segment_anything/modeling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/workers/models/segment_anything/segment_anything/modeling/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14420 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/workers/models/segment_anything/segment_anything/modeling/image_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6615 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/workers/models/segment_anything/segment_anything/modeling/mask_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8594 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/workers/models/segment_anything/segment_anything/modeling/prompt_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/workers/models/segment_anything/segment_anything/modeling/sam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8397 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/workers/models/segment_anything/segment_anything/modeling/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11649 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/workers/models/segment_anything/segment_anything/predictor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:56:55.770467 swarms-1.1.3/swarms/workers/models/segment_anything/segment_anything/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/workers/models/segment_anything/segment_anything/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12712 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/workers/models/segment_anything/segment_anything/utils/amg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5812 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/workers/models/segment_anything/segment_anything/utils/onnx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/workers/models/segment_anything/segment_anything/utils/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/workers/models/segment_anything/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/workers/multi_modal_worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:56:55.770467 swarms-1.1.3/swarms/workers/multi_modal_workers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/workers/multi_modal_workers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79017 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/workers/multi_modal_workers/multi_modal_agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:56:55.770467 swarms-1.1.3/swarms/workers/multi_modal_workers/omni_agent/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/workers/multi_modal_workers/omni_agent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/workers/multi_modal_workers/omni_agent/get_token_ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31031 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/workers/multi_modal_workers/omni_agent/model_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45794 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/workers/multi_modal_workers/omni_agent/omni_chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/workers/omni_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6650 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/workers/worker_agent_ultra.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6547 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/workers/worker_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-07-29 14:56:45.000000 swarms-1.1.3/swarms/workers/worker_ultra_node.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 14:56:55.746467 swarms-1.1.3/swarms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-29 14:56:55.000000 swarms-1.1.3/swarms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6182 2023-07-29 14:56:55.000000 swarms-1.1.3/swarms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 14:56:55.000000 swarms-1.1.3/swarms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-07-29 14:56:55.000000 swarms-1.1.3/swarms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-29 14:56:55.000000 swarms-1.1.3/swarms.egg-info/top_level.txt
```

### Comparing `swarms-1.1.2/LICENSE` & `swarms-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `swarms-1.1.2/PKG-INFO` & `swarms-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swarms
-Version: 1.1.2
+Version: 1.1.3
 Summary: Swarms - Pytorch
 Home-page: https://github.com/kyegomez/swarms
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `swarms-1.1.2/README.md` & `swarms-1.1.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,21 @@
-## Swarms of Autonomous AI Agents 
+<div align="center">
+
+
+# Swarms of Autonomous AI Agents  🤖 🤖 🤖
 
-![Swarming banner](images/swarms.png)
+<!-- ![Swarming banner icon](images/swarmsbannernew.png) -->
 
 Introducing Swarms, automating all digital activities with multi-agent collaboration, get started in 30 seconds in a seamless onboarding experience.
 
----
+</div>
 
-![Join the Agora discord](https://img.shields.io/discord/1110910277110743103?label=Discord&logo=discord&logoColor=white&style=plastic&color=d7b023)
+---
+<!-- 
+![Join the Agora discord](https://img.shields.io/discord/1110910277110743103?label=Discord&logo=discord&logoColor=white&style=plastic&color=d7b023) -->
 
 
 [![GitHub issues](https://img.shields.io/github/issues/kyegomez/swarms)](https://github.com/kyegomez/swarms/issues) [![GitHub forks](https://img.shields.io/github/forks/kyegomez/swarms)](https://github.com/kyegomez/swarms/network) [![GitHub stars](https://img.shields.io/github/stars/kyegomez/swarms)](https://github.com/kyegomez/swarms/stargazers) [![GitHub license](https://img.shields.io/github/license/kyegomez/swarms)](https://github.com/kyegomez/swarms/blob/main/LICENSE)[![GitHub star chart](https://img.shields.io/github/stars/kyegomez/swarms?style=social)](https://star-history.com/#kyegomez/swarms)
 [![Dependency Status](https://img.shields.io/librariesio/github/kyegomez/swarms)](https://libraries.io/github/kyegomez/swarms) [![Downloads](https://static.pepy.tech/badge/swarms/month)](https://pepy.tech/project/swarms)
 
 
 <div align="center">
@@ -143,15 +148,35 @@
 Here are some agents in the swarm you can use!
 
 | Agent        | Import Statement                                   | Example Usage                                           |
 |--------------|----------------------------------------------------|---------------------------------------------------------|
 | WorkerNode   | `from swarms import worker_node`                   | ```python api_key = "sksdsds" node = worker_node(api_key) objective = "Please make a web GUI for using HTTP API server..." task = node.run(objective) print(task)``` |
 | Swarms       | `from swarms.swarms import Swarms`                 | ```python import os from swarms.swarms import Swarms api_key = os.getenv("OPENAI_API_KEY") swarm = Swarms(openai_api_key=api_key) objective = "Please make a web GUI for using HTTP API server..." task = swarm.run(objective) print(task)``` |
 
+## Hierarhical Swarm
+
+```python
+from swarms import HierarchicalSwarm
+
+swarm = HierarchicalSwarm(
+    openai_api_key="your_openai_api_key", 
+    use_vectorstore=True, 
+    embedding_size=768, 
+    use_async=True, 
+    worker_name="My Custom Worker", 
+    human_in_the_loop=True, 
+    boss_prompt="You are a custom boss in a swarm who performs one task based on the following objective: {objective}. Take into account these previously completed tasks: {context}.\n ", 
+    worker_prompt="You are a custom worker in a swarm who performs one task based on the following objective: {objective}. Take into account these previously completed tasks: {context}.\n ", 
+    temperature=0.5, 
+    max_iterations=5, 
+    logging_enabled=True
+)
+result = swarm.run("your_objective")
 
+```
 ---
 
 
 # Docker Setup
 
 * Build the Docker image
 
@@ -282,15 +307,9 @@
 
 ## Swarm Video Demo {Click for more}
 
 [![Watch the swarm video](https://img.youtube.com/vi/Br62cDMYXgc/maxresdefault.jpg)](https://youtu.be/Br62cDMYXgc)
 
 ---
 
-
-
-
-
-
-
-
-
+# Contact 
+For enterprise and production ready deployments, allow us to discover more about you and your story, [book a call with us here](https://www.apac.ai/Setup-Call)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `swarms-1.1.2/api/app.py` & `swarms-1.1.3/api/app.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.2/setup.py` & `swarms-1.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 ##
 
 setup(
   name = 'swarms',
   packages = find_packages(exclude=[]),
-  version = '1.1.2',
+  version = '1.1.3',
   license='MIT',
   description = 'Swarms - Pytorch',
   author = 'Kye Gomez',
   author_email = 'kye@apac.ai',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/kyegomez/swarms',
   keywords = [
```

### Comparing `swarms-1.1.2/swarms/agents/agent.py` & `swarms-1.1.3/swarms/agents/agent.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.2/swarms/agents/base.py` & `swarms-1.1.3/swarms/agents/base.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.2/swarms/agents/memory/base.py` & `swarms-1.1.3/swarms/agents/memory/base.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.2/swarms/agents/memory/chroma.py` & `swarms-1.1.3/swarms/agents/memory/chroma.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.2/swarms/agents/memory/ocean.py` & `swarms-1.1.3/swarms/agents/memory/ocean.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.2/swarms/agents/memory.py` & `swarms-1.1.3/swarms/agents/memory.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.2/swarms/agents/models/hf.py` & `swarms-1.1.3/swarms/agents/models/hf.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.2/swarms/agents/models/llm.py` & `swarms-1.1.3/swarms/agents/models/llm.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.2/swarms/agents/prompts/agent_prompt.py` & `swarms-1.1.3/swarms/agents/prompts/agent_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.2/swarms/agents/prompts/chains/llm.py` & `swarms-1.1.3/swarms/agents/prompts/chains/llm.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.2/swarms/agents/prompts/prompts.py` & `swarms-1.1.3/swarms/agents/prompts/prompts.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.2/swarms/agents/tools/base.py` & `swarms-1.1.3/swarms/agents/tools/base.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.2/swarms/agents/tools/core/code_interpreter/main.py` & `swarms-1.1.3/swarms/agents/tools/core/code_interpreter/main.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.2/swarms/agents/tools/main.py` & `swarms-1.1.3/swarms/agents/tools/main.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.2/swarms/agents/utils/Agent.py` & `swarms-1.1.3/swarms/agents/utils/Agent.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.2/swarms/agents/utils/Calback.py` & `swarms-1.1.3/swarms/agents/utils/Calback.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.2/swarms/agents/utils/ChatOpenAI.py` & `swarms-1.1.3/swarms/agents/utils/ChatOpenAI.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.2/swarms/agents/utils/ConversationalChatAgent.py` & `swarms-1.1.3/swarms/agents/utils/ConversationalChatAgent.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.2/swarms/agents/utils/agent_creator.py` & `swarms-1.1.3/swarms/agents/utils/agent_creator.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.2/swarms/agents/utils/agent_setup.py` & `swarms-1.1.3/swarms/agents/utils/agent_setup.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.2/swarms/agents/utils/output_parser.py` & `swarms-1.1.3/swarms/agents/utils/output_parser.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.2/swarms/agents/utils/prompts.py` & `swarms-1.1.3/swarms/agents/utils/prompts.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.2/swarms/boss/boss_node.py` & `swarms-1.1.3/swarms/boss/boss_node.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.2/swarms/hivemind.py` & `swarms-1.1.3/swarms/hivemind.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.2/swarms/orchestrate.py` & `swarms-1.1.3/swarms/orchestrate.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.2/swarms/swarms.py` & `swarms-1.1.3/swarms/swarms.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,20 +11,18 @@
 from langchain.embeddings import OpenAIEmbeddings
 from langchain.tools import DuckDuckGoSearchRun
 from langchain.tools.file_management.read import ReadFileTool
 from langchain.tools.file_management.write import WriteFileTool
 from langchain.vectorstores import FAISS
 
 
-# from langchain.tools.human.tool import HumanInputRun
 from swarms.agents.tools.main import WebpageQATool, process_csv
 from swarms.boss.boss_node import BossNodeInitializer as BossNode
 from swarms.workers.worker_node import WorkerNodeInitializer
 
-# from langchain import LLMMathChain
 logging.basicConfig(level=logging.INFO, format='%(asctime)s - %(levelname)s - %(message)s')
 
 
 # TODO: Pass in abstract LLM class that can utilize Hf or Anthropic models, Move away from OPENAI
 # TODO: ADD Universal Communication Layer, a ocean vectorstore instance
 # TODO: BE MORE EXPLICIT ON TOOL USE, TASK DECOMPOSITION AND TASK COMPLETETION AND ALLOCATION
 # TODO: Add RLHF Data collection, ask user how the swarm is performing
@@ -38,17 +36,18 @@
     def __init__(
         self, 
         openai_api_key: Optional[str] = "", 
 
         use_vectorstore: Optional[bool] = True, 
         embedding_size: Optional[int] = None, 
         use_async: Optional[bool] = True, 
+        worker_name: Optional[str] = "Swarm Worker AI Assistant",
 
         human_in_the_loop: Optional[bool] = True, 
-        boss_prompt: Optional[str] = None,
+        boss_prompt: Optional[str] = "You are an Boss in a swarm who performs one task based on the following objective: {objective}. Take into account these previously completed tasks: {context}.\n",
 
         worker_prompt: Optional[str] = None,
         temperature: Optional[float] = None,
         max_iterations: Optional[int] = None,
         logging_enabled: Optional[bool] = True):
             
         self.openai_api_key = openai_api_key
@@ -128,31 +127,19 @@
             index = faiss.IndexFlatL2(embedding_size)
 
             return FAISS(embeddings_model.embed_query, index, InMemoryDocstore({}), {})
         except Exception as e:
             logging.error(f"Failed to initialize vector store: {e}")
             return None
 
-    def initialize_worker_node(self, worker_tools, vectorstore, llm_class=ChatOpenAI, ai_name="Swarm Worker AI Assistant",):
-        """
-        Init WorkerNode
-
-        Params:
-            worker_tools (list): The list of worker tools.
-            vectorstore (object): The vector store object
-            llm_class (class): The Language model class. Default is ChatOpenAI
-            ai_name (str): The AI name. Default is "Swarms worker AI assistant"        
-        """
+    def initialize_worker_node(self, worker_tools, vectorstore, llm_class=ChatOpenAI):
         try:    
-            # Initialize worker node
-            llm = self.initialize_llm(ChatOpenAI)
-            worker_node = WorkerNodeInitializer(llm=llm, tools=worker_tools, vectorstore=vectorstore)
-            worker_node.create_agent(ai_name=ai_name, ai_role="Assistant", search_kwargs={}, human_in_the_loop=self.human_in_the_loop) # add search kwargs
+            worker_node = WorkerNodeInitializer(llm=self.llm, tools=worker_tools, vectorstore=vectorstore)
+            worker_node.create_agent(ai_name=self.worker_name, ai_role="Assistant", search_kwargs={}, human_in_the_loop=self.human_in_the_loop)
             worker_description = self.worker_prompt
-
             worker_node_tool = Tool(name="WorkerNode AI Agent", func=worker_node.run, description= worker_description or "Input: an objective with a todo list for that objective. Output: your task completed: Please be very clear what the objective and task instructions are. The Swarm worker agent is Useful for when you need to spawn an autonomous agent instance as a worker to accomplish any complex tasks, it can search the internet or write code or spawn child multi-modality models to process and generate images and text or audio and so on")
             return worker_node_tool
         except Exception as e:
             logging.error(f"Failed to initialize worker node: {e}")
             raise
 
     def initialize_boss_node(self, vectorstore, worker_node, llm_class=OpenAI, max_iterations=None, verbose=False):
@@ -169,15 +156,15 @@
         """
         try:
 
             # Initialize boss node
             llm = self.initialize_llm(llm_class)
             
             # prompt = self.boss_prompt
-            todo_prompt = PromptTemplate.from_template({self.boss_prompt} or "You are a boss planer in a swarm who is an expert at coming up with a todo list for a given objective and then creating an worker to help you accomplish your task. Rate every task on the importance of it's probability to complete the main objective on a scale from 0 to 1, an integer. Come up with a todo list for this objective: {objective} and then spawn a worker agent to complete the task for you. Always spawn an worker agent after creating a plan and pass the objective and plan to the worker agent.")
+            todo_prompt = PromptTemplate.from_template(self.boss_prompt)
             todo_chain = LLMChain(llm=llm, prompt=todo_prompt)
 
             tools = [
                 Tool(name="TODO", func=todo_chain.run, description="useful for when you need to come up with todo lists. Input: an objective to create a todo list for your objective. Note create a todo list then assign a ranking from 0.0 to 1.0 to each task, then sort the tasks based on the tasks most likely to achieve the objective. The Output: a todo list for that objective with rankings for each step from 0.1 Please be very clear what the objective is!"),
                 worker_node,
             ]
```

### Comparing `swarms-1.1.2/swarms/utils/embeddings/base.py` & `swarms-1.1.3/swarms/utils/embeddings/base.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.2/swarms/utils/embeddings/pegasus.py` & `swarms-1.1.3/swarms/utils/embeddings/pegasus.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.2/swarms/utils/main.py` & `swarms-1.1.3/swarms/utils/main.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.2/swarms/utils/static.py` & `swarms-1.1.3/swarms/utils/static.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.2/swarms/workers/character_generative.py` & `swarms-1.1.3/swarms/workers/character_generative.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.2/swarms/workers/generative_worker.py` & `swarms-1.1.3/swarms/workers/generative_worker.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.2/swarms/workers/models/GroundingDINO/groundingdino/config/GroundingDINO_SwinB_cfg.py` & `swarms-1.1.3/swarms/workers/models/GroundingDINO/groundingdino/config/GroundingDINO_SwinB_cfg.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.2/swarms/workers/models/GroundingDINO/groundingdino/config/GroundingDINO_SwinT_OGC.py` & `swarms-1.1.3/swarms/workers/models/GroundingDINO/groundingdino/config/GroundingDINO_SwinT_OGC.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.2/swarms/workers/models/GroundingDINO/groundingdino/datasets/cocogrounding_eval.py` & `swarms-1.1.3/swarms/workers/models/GroundingDINO/groundingdino/datasets/cocogrounding_eval.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.2/swarms/workers/models/GroundingDINO/groundingdino/datasets/transforms.py` & `swarms-1.1.3/swarms/workers/models/GroundingDINO/groundingdino/datasets/transforms.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.2/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/__init__.py` & `swarms-1.1.3/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/__init__.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.2/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/backbone.py` & `swarms-1.1.3/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/backbone.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.2/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/position_encoding.py` & `swarms-1.1.3/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/position_encoding.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.2/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/swin_transformer.py` & `swarms-1.1.3/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/swin_transformer.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.2/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/bertwarper.py` & `swarms-1.1.3/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/bertwarper.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.2/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/fuse_modules.py` & `swarms-1.1.3/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/fuse_modules.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.2/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/groundingdino.py` & `swarms-1.1.3/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/groundingdino.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.2/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/ms_deform_attn.py` & `swarms-1.1.3/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/ms_deform_attn.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.2/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/transformer.py` & `swarms-1.1.3/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/transformer.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.2/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/transformer_vanilla.py` & `swarms-1.1.3/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/transformer_vanilla.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.2/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/utils.py` & `swarms-1.1.3/swarms/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/utils.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.2/swarms/workers/models/GroundingDINO/groundingdino/models/__init__.py` & `swarms-1.1.3/swarms/workers/models/GroundingDINO/groundingdino/models/__init__.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.2/swarms/workers/models/GroundingDINO/groundingdino/models/registry.py` & `swarms-1.1.3/swarms/workers/models/GroundingDINO/groundingdino/models/registry.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.2/swarms/workers/models/GroundingDINO/groundingdino/util/box_ops.py` & `swarms-1.1.3/swarms/workers/models/GroundingDINO/groundingdino/util/box_ops.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.2/swarms/workers/models/GroundingDINO/groundingdino/util/get_tokenlizer.py` & `swarms-1.1.3/swarms/workers/models/GroundingDINO/groundingdino/util/get_tokenlizer.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.2/swarms/workers/models/GroundingDINO/groundingdino/util/inference.py` & `swarms-1.1.3/swarms/workers/models/GroundingDINO/groundingdino/util/inference.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.2/swarms/workers/models/GroundingDINO/groundingdino/util/logger.py` & `swarms-1.1.3/swarms/workers/models/GroundingDINO/groundingdino/util/logger.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.2/swarms/workers/models/GroundingDINO/groundingdino/util/misc.py` & `swarms-1.1.3/swarms/workers/models/GroundingDINO/groundingdino/util/misc.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.2/swarms/workers/models/GroundingDINO/groundingdino/util/slconfig.py` & `swarms-1.1.3/swarms/workers/models/GroundingDINO/groundingdino/util/slconfig.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.2/swarms/workers/models/GroundingDINO/groundingdino/util/slio.py` & `swarms-1.1.3/swarms/workers/models/GroundingDINO/groundingdino/util/slio.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.2/swarms/workers/models/GroundingDINO/groundingdino/util/time_counter.py` & `swarms-1.1.3/swarms/workers/models/GroundingDINO/groundingdino/util/time_counter.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.2/swarms/workers/models/GroundingDINO/groundingdino/util/utils.py` & `swarms-1.1.3/swarms/workers/models/GroundingDINO/groundingdino/util/utils.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.2/swarms/workers/models/GroundingDINO/groundingdino/util/visualizer.py` & `swarms-1.1.3/swarms/workers/models/GroundingDINO/groundingdino/util/visualizer.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.2/swarms/workers/models/GroundingDINO/groundingdino/util/vl_utils.py` & `swarms-1.1.3/swarms/workers/models/GroundingDINO/groundingdino/util/vl_utils.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.2/swarms/workers/models/GroundingDINO/setup.py` & `swarms-1.1.3/swarms/workers/models/GroundingDINO/setup.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.2/swarms/workers/models/segment_anything/segment_anything/automatic_mask_generator.py` & `swarms-1.1.3/swarms/workers/models/segment_anything/segment_anything/automatic_mask_generator.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.2/swarms/workers/models/segment_anything/segment_anything/build_sam.py` & `swarms-1.1.3/swarms/workers/models/segment_anything/segment_anything/build_sam.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.2/swarms/workers/models/segment_anything/segment_anything/modeling/common.py` & `swarms-1.1.3/swarms/workers/models/segment_anything/segment_anything/modeling/common.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.2/swarms/workers/models/segment_anything/segment_anything/modeling/image_encoder.py` & `swarms-1.1.3/swarms/workers/models/segment_anything/segment_anything/modeling/image_encoder.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.2/swarms/workers/models/segment_anything/segment_anything/modeling/mask_decoder.py` & `swarms-1.1.3/swarms/workers/models/segment_anything/segment_anything/modeling/mask_decoder.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.2/swarms/workers/models/segment_anything/segment_anything/modeling/prompt_encoder.py` & `swarms-1.1.3/swarms/workers/models/segment_anything/segment_anything/modeling/prompt_encoder.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.2/swarms/workers/models/segment_anything/segment_anything/modeling/sam.py` & `swarms-1.1.3/swarms/workers/models/segment_anything/segment_anything/modeling/sam.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.2/swarms/workers/models/segment_anything/segment_anything/modeling/transformer.py` & `swarms-1.1.3/swarms/workers/models/segment_anything/segment_anything/modeling/transformer.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.2/swarms/workers/models/segment_anything/segment_anything/predictor.py` & `swarms-1.1.3/swarms/workers/models/segment_anything/segment_anything/predictor.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.2/swarms/workers/models/segment_anything/segment_anything/utils/amg.py` & `swarms-1.1.3/swarms/workers/models/segment_anything/segment_anything/utils/amg.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.2/swarms/workers/models/segment_anything/segment_anything/utils/onnx.py` & `swarms-1.1.3/swarms/workers/models/segment_anything/segment_anything/utils/onnx.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.2/swarms/workers/models/segment_anything/segment_anything/utils/transforms.py` & `swarms-1.1.3/swarms/workers/models/segment_anything/segment_anything/utils/transforms.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.2/swarms/workers/models/segment_anything/setup.py` & `swarms-1.1.3/swarms/workers/models/segment_anything/setup.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.2/swarms/workers/multi_modal_worker.py` & `swarms-1.1.3/swarms/workers/multi_modal_worker.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.2/swarms/workers/multi_modal_workers/multi_modal_agent.py` & `swarms-1.1.3/swarms/workers/multi_modal_workers/multi_modal_agent.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.2/swarms/workers/multi_modal_workers/omni_agent/get_token_ids.py` & `swarms-1.1.3/swarms/workers/multi_modal_workers/omni_agent/get_token_ids.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.2/swarms/workers/multi_modal_workers/omni_agent/model_server.py` & `swarms-1.1.3/swarms/workers/multi_modal_workers/omni_agent/model_server.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.2/swarms/workers/multi_modal_workers/omni_agent/omni_chat.py` & `swarms-1.1.3/swarms/workers/multi_modal_workers/omni_agent/omni_chat.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.2/swarms/workers/omni_worker.py` & `swarms-1.1.3/swarms/workers/omni_worker.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.2/swarms/workers/worker_agent_ultra.py` & `swarms-1.1.3/swarms/workers/worker_agent_ultra.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.2/swarms/workers/worker_node.py` & `swarms-1.1.3/swarms/workers/worker_node.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.2/swarms/workers/worker_ultra_node.py` & `swarms-1.1.3/swarms/workers/worker_ultra_node.py`

 * *Files identical despite different names*

### Comparing `swarms-1.1.2/swarms.egg-info/PKG-INFO` & `swarms-1.1.3/swarms.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swarms
-Version: 1.1.2
+Version: 1.1.3
 Summary: Swarms - Pytorch
 Home-page: https://github.com/kyegomez/swarms
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `swarms-1.1.2/swarms.egg-info/SOURCES.txt` & `swarms-1.1.3/swarms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `swarms-1.1.2/swarms.egg-info/requires.txt` & `swarms-1.1.3/swarms.egg-info/requires.txt`

 * *Files identical despite different names*

