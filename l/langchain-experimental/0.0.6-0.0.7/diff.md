# Comparing `tmp/langchain_experimental-0.0.6.tar.gz` & `tmp/langchain_experimental-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_experimental-0.0.6.tar", max compression
+gzip compressed data, was "langchain_experimental-0.0.7.tar", max compression
```

## Comparing `langchain_experimental-0.0.6.tar` & `langchain_experimental-0.0.7.tar`

### file list

```diff
@@ -1,64 +1,64 @@
--rw-r--r--   0        0        0       93 2023-07-28 08:18:51.192045 langchain_experimental-0.0.6/README.md
--rw-r--r--   0        0        0        0 2023-07-28 08:18:51.192045 langchain_experimental-0.0.6/langchain_experimental/__init__.py
--rw-r--r--   0        0        0      288 2023-07-28 08:18:51.192045 langchain_experimental-0.0.6/langchain_experimental/autonomous_agents/__init__.py
--rw-r--r--   0        0        0        0 2023-07-28 08:18:51.192045 langchain_experimental-0.0.6/langchain_experimental/autonomous_agents/autogpt/__init__.py
--rw-r--r--   0        0        0     5244 2023-07-28 08:18:51.192045 langchain_experimental-0.0.6/langchain_experimental/autonomous_agents/autogpt/agent.py
--rw-r--r--   0        0        0     1072 2023-07-28 08:18:51.192045 langchain_experimental-0.0.6/langchain_experimental/autonomous_agents/autogpt/memory.py
--rw-r--r--   0        0        0     1950 2023-07-28 08:18:51.192045 langchain_experimental-0.0.6/langchain_experimental/autonomous_agents/autogpt/output_parser.py
--rw-r--r--   0        0        0     3305 2023-07-28 08:18:51.192045 langchain_experimental-0.0.6/langchain_experimental/autonomous_agents/autogpt/prompt.py
--rw-r--r--   0        0        0     6572 2023-07-28 08:18:51.192045 langchain_experimental-0.0.6/langchain_experimental/autonomous_agents/autogpt/prompt_generator.py
--rw-r--r--   0        0        0      514 2023-07-28 08:18:51.192045 langchain_experimental-0.0.6/langchain_experimental/autonomous_agents/baby_agi/__init__.py
--rw-r--r--   0        0        0     7469 2023-07-28 08:18:51.192045 langchain_experimental-0.0.6/langchain_experimental/autonomous_agents/baby_agi/baby_agi.py
--rw-r--r--   0        0        0     1284 2023-07-28 08:18:51.192045 langchain_experimental-0.0.6/langchain_experimental/autonomous_agents/baby_agi/task_creation.py
--rw-r--r--   0        0        0      835 2023-07-28 08:18:51.192045 langchain_experimental-0.0.6/langchain_experimental/autonomous_agents/baby_agi/task_execution.py
--rw-r--r--   0        0        0     1076 2023-07-28 08:18:51.192045 langchain_experimental-0.0.6/langchain_experimental/autonomous_agents/baby_agi/task_prioritization.py
--rw-r--r--   0        0        0        0 2023-07-28 08:18:51.192045 langchain_experimental-0.0.6/langchain_experimental/autonomous_agents/hugginggpt/__init__.py
--rw-r--r--   0        0        0     1083 2023-07-28 08:18:51.192045 langchain_experimental-0.0.6/langchain_experimental/autonomous_agents/hugginggpt/hugginggpt.py
--rw-r--r--   0        0        0     1450 2023-07-28 08:18:51.192045 langchain_experimental-0.0.6/langchain_experimental/autonomous_agents/hugginggpt/repsonse_generator.py
--rw-r--r--   0        0        0     4551 2023-07-28 08:18:51.192045 langchain_experimental-0.0.6/langchain_experimental/autonomous_agents/hugginggpt/task_executor.py
--rw-r--r--   0        0        0     6439 2023-07-28 08:18:51.192045 langchain_experimental-0.0.6/langchain_experimental/autonomous_agents/hugginggpt/task_planner.py
--rw-r--r--   0        0        0      100 2023-07-28 08:18:51.192045 langchain_experimental-0.0.6/langchain_experimental/cpal/README.md
--rw-r--r--   0        0        0        0 2023-07-28 08:18:51.192045 langchain_experimental-0.0.6/langchain_experimental/cpal/__init__.py
--rw-r--r--   0        0        0     9041 2023-07-28 08:18:51.192045 langchain_experimental-0.0.6/langchain_experimental/cpal/base.py
--rw-r--r--   0        0        0      246 2023-07-28 08:18:51.192045 langchain_experimental-0.0.6/langchain_experimental/cpal/constants.py
--rw-r--r--   0        0        0     8322 2023-07-28 08:18:51.192045 langchain_experimental-0.0.6/langchain_experimental/cpal/models.py
--rw-r--r--   0        0        0        0 2023-07-28 08:18:51.192045 langchain_experimental-0.0.6/langchain_experimental/cpal/templates/__init__.py
--rw-r--r--   0        0        0        0 2023-07-28 08:18:51.192045 langchain_experimental-0.0.6/langchain_experimental/cpal/templates/univariate/__init__.py
--rw-r--r--   0        0        0     2175 2023-07-28 08:18:51.192045 langchain_experimental-0.0.6/langchain_experimental/cpal/templates/univariate/causal.py
--rw-r--r--   0        0        0      706 2023-07-28 08:18:51.192045 langchain_experimental-0.0.6/langchain_experimental/cpal/templates/univariate/intervention.py
--rw-r--r--   0        0        0     1750 2023-07-28 08:18:51.192045 langchain_experimental-0.0.6/langchain_experimental/cpal/templates/univariate/narrative.py
--rw-r--r--   0        0        0     4503 2023-07-28 08:18:51.192045 langchain_experimental-0.0.6/langchain_experimental/cpal/templates/univariate/query.py
--rw-r--r--   0        0        0      260 2023-07-28 08:18:51.192045 langchain_experimental-0.0.6/langchain_experimental/generative_agents/__init__.py
--rw-r--r--   0        0        0    10150 2023-07-28 08:18:51.192045 langchain_experimental-0.0.6/langchain_experimental/generative_agents/generative_agent.py
--rw-r--r--   0        0        0    12461 2023-07-28 08:18:51.192045 langchain_experimental-0.0.6/langchain_experimental/generative_agents/memory.py
--rw-r--r--   0        0        0      277 2023-07-28 08:18:51.192045 langchain_experimental-0.0.6/langchain_experimental/llms/__init__.py
--rw-r--r--   0        0        0     1838 2023-07-28 08:18:51.192045 langchain_experimental-0.0.6/langchain_experimental/llms/jsonformer_decoder.py
--rw-r--r--   0        0        0     4279 2023-07-28 08:18:51.192045 langchain_experimental-0.0.6/langchain_experimental/llms/llamaapi.py
--rw-r--r--   0        0        0     2027 2023-07-28 08:18:51.192045 langchain_experimental-0.0.6/langchain_experimental/llms/rellm_decoder.py
--rw-r--r--   0        0        0      277 2023-07-28 08:18:51.192045 langchain_experimental-0.0.6/langchain_experimental/pal_chain/__init__.py
--rw-r--r--   0        0        0    12482 2023-07-28 08:18:51.192045 langchain_experimental-0.0.6/langchain_experimental/pal_chain/base.py
--rw-r--r--   0        0        0     2645 2023-07-28 08:18:51.192045 langchain_experimental-0.0.6/langchain_experimental/pal_chain/colored_object_prompt.py
--rw-r--r--   0        0        0     4301 2023-07-28 08:18:51.192045 langchain_experimental-0.0.6/langchain_experimental/pal_chain/math_prompt.py
--rw-r--r--   0        0        0      363 2023-07-28 08:18:51.192045 langchain_experimental-0.0.6/langchain_experimental/plan_and_execute/__init__.py
--rw-r--r--   0        0        0     3400 2023-07-28 08:18:51.192045 langchain_experimental-0.0.6/langchain_experimental/plan_and_execute/agent_executor.py
--rw-r--r--   0        0        0        0 2023-07-28 08:18:51.192045 langchain_experimental-0.0.6/langchain_experimental/plan_and_execute/executors/__init__.py
--rw-r--r--   0        0        0     1464 2023-07-28 08:18:51.192045 langchain_experimental-0.0.6/langchain_experimental/plan_and_execute/executors/agent_executor.py
--rw-r--r--   0        0        0     1156 2023-07-28 08:18:51.192045 langchain_experimental-0.0.6/langchain_experimental/plan_and_execute/executors/base.py
--rw-r--r--   0        0        0        0 2023-07-28 08:18:51.192045 langchain_experimental-0.0.6/langchain_experimental/plan_and_execute/planners/__init__.py
--rw-r--r--   0        0        0     1362 2023-07-28 08:18:51.192045 langchain_experimental-0.0.6/langchain_experimental/plan_and_execute/planners/base.py
--rw-r--r--   0        0        0     1800 2023-07-28 08:18:51.192045 langchain_experimental-0.0.6/langchain_experimental/plan_and_execute/planners/chat_planner.py
--rw-r--r--   0        0        0     1149 2023-07-28 08:18:51.192045 langchain_experimental-0.0.6/langchain_experimental/plan_and_execute/schema.py
--rw-r--r--   0        0        0       87 2023-07-28 08:18:51.192045 langchain_experimental-0.0.6/langchain_experimental/prompts/__init__.py
--rw-r--r--   0        0        0     1873 2023-07-28 08:18:51.192045 langchain_experimental-0.0.6/langchain_experimental/prompts/load.py
--rw-r--r--   0        0        0      140 2023-07-28 08:18:51.192045 langchain_experimental-0.0.6/langchain_experimental/sql/__init__.py
--rw-r--r--   0        0        0    11413 2023-07-28 08:18:51.192045 langchain_experimental-0.0.6/langchain_experimental/sql/base.py
--rw-r--r--   0        0        0      149 2023-07-28 08:18:51.192045 langchain_experimental-0.0.6/langchain_experimental/tot/__init__.py
--rw-r--r--   0        0        0     5087 2023-07-28 08:18:51.192045 langchain_experimental-0.0.6/langchain_experimental/tot/base.py
--rw-r--r--   0        0        0     1405 2023-07-28 08:18:51.192045 langchain_experimental-0.0.6/langchain_experimental/tot/checker.py
--rw-r--r--   0        0        0     1666 2023-07-28 08:18:51.192045 langchain_experimental-0.0.6/langchain_experimental/tot/controller.py
--rw-r--r--   0        0        0     1456 2023-07-28 08:18:51.192045 langchain_experimental-0.0.6/langchain_experimental/tot/memory.py
--rw-r--r--   0        0        0     3534 2023-07-28 08:18:51.192045 langchain_experimental-0.0.6/langchain_experimental/tot/prompts.py
--rw-r--r--   0        0        0      398 2023-07-28 08:18:51.192045 langchain_experimental-0.0.6/langchain_experimental/tot/thought.py
--rw-r--r--   0        0        0     3026 2023-07-28 08:18:51.192045 langchain_experimental-0.0.6/langchain_experimental/tot/thought_generation.py
--rw-r--r--   0        0        0     1904 2023-07-28 08:18:51.196045 langchain_experimental-0.0.6/pyproject.toml
--rw-r--r--   0        0        0      717 1970-01-01 00:00:00.000000 langchain_experimental-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0       93 2023-07-29 00:17:08.308358 langchain_experimental-0.0.7/README.md
+-rw-r--r--   0        0        0        0 2023-07-29 00:17:08.308358 langchain_experimental-0.0.7/langchain_experimental/__init__.py
+-rw-r--r--   0        0        0      288 2023-07-29 00:17:08.312358 langchain_experimental-0.0.7/langchain_experimental/autonomous_agents/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-29 00:17:08.312358 langchain_experimental-0.0.7/langchain_experimental/autonomous_agents/autogpt/__init__.py
+-rw-r--r--   0        0        0     5244 2023-07-29 00:17:08.312358 langchain_experimental-0.0.7/langchain_experimental/autonomous_agents/autogpt/agent.py
+-rw-r--r--   0        0        0     1103 2023-07-29 00:17:08.312358 langchain_experimental-0.0.7/langchain_experimental/autonomous_agents/autogpt/memory.py
+-rw-r--r--   0        0        0     1882 2023-07-29 00:17:08.312358 langchain_experimental-0.0.7/langchain_experimental/autonomous_agents/autogpt/output_parser.py
+-rw-r--r--   0        0        0     3305 2023-07-29 00:17:08.312358 langchain_experimental-0.0.7/langchain_experimental/autonomous_agents/autogpt/prompt.py
+-rw-r--r--   0        0        0     6573 2023-07-29 00:17:08.312358 langchain_experimental-0.0.7/langchain_experimental/autonomous_agents/autogpt/prompt_generator.py
+-rw-r--r--   0        0        0      514 2023-07-29 00:17:08.312358 langchain_experimental-0.0.7/langchain_experimental/autonomous_agents/baby_agi/__init__.py
+-rw-r--r--   0        0        0     7469 2023-07-29 00:17:08.312358 langchain_experimental-0.0.7/langchain_experimental/autonomous_agents/baby_agi/baby_agi.py
+-rw-r--r--   0        0        0     1282 2023-07-29 00:17:08.312358 langchain_experimental-0.0.7/langchain_experimental/autonomous_agents/baby_agi/task_creation.py
+-rw-r--r--   0        0        0      835 2023-07-29 00:17:08.312358 langchain_experimental-0.0.7/langchain_experimental/autonomous_agents/baby_agi/task_execution.py
+-rw-r--r--   0        0        0     1076 2023-07-29 00:17:08.312358 langchain_experimental-0.0.7/langchain_experimental/autonomous_agents/baby_agi/task_prioritization.py
+-rw-r--r--   0        0        0        0 2023-07-29 00:17:08.312358 langchain_experimental-0.0.7/langchain_experimental/autonomous_agents/hugginggpt/__init__.py
+-rw-r--r--   0        0        0     1083 2023-07-29 00:17:08.312358 langchain_experimental-0.0.7/langchain_experimental/autonomous_agents/hugginggpt/hugginggpt.py
+-rw-r--r--   0        0        0     1450 2023-07-29 00:17:08.312358 langchain_experimental-0.0.7/langchain_experimental/autonomous_agents/hugginggpt/repsonse_generator.py
+-rw-r--r--   0        0        0     4551 2023-07-29 00:17:08.312358 langchain_experimental-0.0.7/langchain_experimental/autonomous_agents/hugginggpt/task_executor.py
+-rw-r--r--   0        0        0     6439 2023-07-29 00:17:08.312358 langchain_experimental-0.0.7/langchain_experimental/autonomous_agents/hugginggpt/task_planner.py
+-rw-r--r--   0        0        0      100 2023-07-29 00:17:08.312358 langchain_experimental-0.0.7/langchain_experimental/cpal/README.md
+-rw-r--r--   0        0        0        0 2023-07-29 00:17:08.312358 langchain_experimental-0.0.7/langchain_experimental/cpal/__init__.py
+-rw-r--r--   0        0        0     9041 2023-07-29 00:17:08.312358 langchain_experimental-0.0.7/langchain_experimental/cpal/base.py
+-rw-r--r--   0        0        0      246 2023-07-29 00:17:08.312358 langchain_experimental-0.0.7/langchain_experimental/cpal/constants.py
+-rw-r--r--   0        0        0     8322 2023-07-29 00:17:08.312358 langchain_experimental-0.0.7/langchain_experimental/cpal/models.py
+-rw-r--r--   0        0        0        0 2023-07-29 00:17:08.312358 langchain_experimental-0.0.7/langchain_experimental/cpal/templates/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-29 00:17:08.312358 langchain_experimental-0.0.7/langchain_experimental/cpal/templates/univariate/__init__.py
+-rw-r--r--   0        0        0     2175 2023-07-29 00:17:08.312358 langchain_experimental-0.0.7/langchain_experimental/cpal/templates/univariate/causal.py
+-rw-r--r--   0        0        0      706 2023-07-29 00:17:08.312358 langchain_experimental-0.0.7/langchain_experimental/cpal/templates/univariate/intervention.py
+-rw-r--r--   0        0        0     1750 2023-07-29 00:17:08.312358 langchain_experimental-0.0.7/langchain_experimental/cpal/templates/univariate/narrative.py
+-rw-r--r--   0        0        0     4503 2023-07-29 00:17:08.312358 langchain_experimental-0.0.7/langchain_experimental/cpal/templates/univariate/query.py
+-rw-r--r--   0        0        0      260 2023-07-29 00:17:08.312358 langchain_experimental-0.0.7/langchain_experimental/generative_agents/__init__.py
+-rw-r--r--   0        0        0    10158 2023-07-29 00:17:08.312358 langchain_experimental-0.0.7/langchain_experimental/generative_agents/generative_agent.py
+-rw-r--r--   0        0        0    12500 2023-07-29 00:17:08.312358 langchain_experimental-0.0.7/langchain_experimental/generative_agents/memory.py
+-rw-r--r--   0        0        0      277 2023-07-29 00:17:08.312358 langchain_experimental-0.0.7/langchain_experimental/llms/__init__.py
+-rw-r--r--   0        0        0     1965 2023-07-29 00:17:08.312358 langchain_experimental-0.0.7/langchain_experimental/llms/jsonformer_decoder.py
+-rw-r--r--   0        0        0     4279 2023-07-29 00:17:08.312358 langchain_experimental-0.0.7/langchain_experimental/llms/llamaapi.py
+-rw-r--r--   0        0        0     2089 2023-07-29 00:17:08.312358 langchain_experimental-0.0.7/langchain_experimental/llms/rellm_decoder.py
+-rw-r--r--   0        0        0      277 2023-07-29 00:17:08.312358 langchain_experimental-0.0.7/langchain_experimental/pal_chain/__init__.py
+-rw-r--r--   0        0        0    11672 2023-07-29 00:17:08.312358 langchain_experimental-0.0.7/langchain_experimental/pal_chain/base.py
+-rw-r--r--   0        0        0     2645 2023-07-29 00:17:08.312358 langchain_experimental-0.0.7/langchain_experimental/pal_chain/colored_object_prompt.py
+-rw-r--r--   0        0        0     4301 2023-07-29 00:17:08.312358 langchain_experimental-0.0.7/langchain_experimental/pal_chain/math_prompt.py
+-rw-r--r--   0        0        0      363 2023-07-29 00:17:08.312358 langchain_experimental-0.0.7/langchain_experimental/plan_and_execute/__init__.py
+-rw-r--r--   0        0        0     3544 2023-07-29 00:17:08.312358 langchain_experimental-0.0.7/langchain_experimental/plan_and_execute/agent_executor.py
+-rw-r--r--   0        0        0        0 2023-07-29 00:17:08.312358 langchain_experimental-0.0.7/langchain_experimental/plan_and_execute/executors/__init__.py
+-rw-r--r--   0        0        0     1464 2023-07-29 00:17:08.312358 langchain_experimental-0.0.7/langchain_experimental/plan_and_execute/executors/agent_executor.py
+-rw-r--r--   0        0        0     1243 2023-07-29 00:17:08.312358 langchain_experimental-0.0.7/langchain_experimental/plan_and_execute/executors/base.py
+-rw-r--r--   0        0        0        0 2023-07-29 00:17:08.312358 langchain_experimental-0.0.7/langchain_experimental/plan_and_execute/planners/__init__.py
+-rw-r--r--   0        0        0     1541 2023-07-29 00:17:08.312358 langchain_experimental-0.0.7/langchain_experimental/plan_and_execute/planners/base.py
+-rw-r--r--   0        0        0     1836 2023-07-29 00:17:08.312358 langchain_experimental-0.0.7/langchain_experimental/plan_and_execute/planners/chat_planner.py
+-rw-r--r--   0        0        0     1391 2023-07-29 00:17:08.312358 langchain_experimental-0.0.7/langchain_experimental/plan_and_execute/schema.py
+-rw-r--r--   0        0        0       87 2023-07-29 00:17:08.312358 langchain_experimental-0.0.7/langchain_experimental/prompts/__init__.py
+-rw-r--r--   0        0        0     1873 2023-07-29 00:17:08.312358 langchain_experimental-0.0.7/langchain_experimental/prompts/load.py
+-rw-r--r--   0        0        0      140 2023-07-29 00:17:08.312358 langchain_experimental-0.0.7/langchain_experimental/sql/__init__.py
+-rw-r--r--   0        0        0    11413 2023-07-29 00:17:08.312358 langchain_experimental-0.0.7/langchain_experimental/sql/base.py
+-rw-r--r--   0        0        0      149 2023-07-29 00:17:08.312358 langchain_experimental-0.0.7/langchain_experimental/tot/__init__.py
+-rw-r--r--   0        0        0     5087 2023-07-29 00:17:08.312358 langchain_experimental-0.0.7/langchain_experimental/tot/base.py
+-rw-r--r--   0        0        0     1405 2023-07-29 00:17:08.312358 langchain_experimental-0.0.7/langchain_experimental/tot/checker.py
+-rw-r--r--   0        0        0     1666 2023-07-29 00:17:08.312358 langchain_experimental-0.0.7/langchain_experimental/tot/controller.py
+-rw-r--r--   0        0        0     1456 2023-07-29 00:17:08.312358 langchain_experimental-0.0.7/langchain_experimental/tot/memory.py
+-rw-r--r--   0        0        0     3534 2023-07-29 00:17:08.312358 langchain_experimental-0.0.7/langchain_experimental/tot/prompts.py
+-rw-r--r--   0        0        0      398 2023-07-29 00:17:08.312358 langchain_experimental-0.0.7/langchain_experimental/tot/thought.py
+-rw-r--r--   0        0        0     3026 2023-07-29 00:17:08.312358 langchain_experimental-0.0.7/langchain_experimental/tot/thought_generation.py
+-rw-r--r--   0        0        0     1904 2023-07-29 00:17:08.328358 langchain_experimental-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0      717 1970-01-01 00:00:00.000000 langchain_experimental-0.0.7/PKG-INFO
```

### Comparing `langchain_experimental-0.0.6/langchain_experimental/autonomous_agents/autogpt/agent.py` & `langchain_experimental-0.0.7/langchain_experimental/autonomous_agents/autogpt/agent.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.6/langchain_experimental/autonomous_agents/autogpt/memory.py` & `langchain_experimental-0.0.7/langchain_experimental/autonomous_agents/autogpt/memory.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 
 from langchain.memory.chat_memory import BaseChatMemory, get_prompt_input_key
 from langchain.vectorstores.base import VectorStoreRetriever
 from pydantic import Field
 
 
 class AutoGPTMemory(BaseChatMemory):
+    """Memory for AutoGPT."""
+
     retriever: VectorStoreRetriever = Field(exclude=True)
     """VectorStoreRetriever object to connect to."""
 
     @property
     def memory_variables(self) -> List[str]:
         return ["chat_history", "relevant_context"]
```

### Comparing `langchain_experimental-0.0.6/langchain_experimental/autonomous_agents/autogpt/output_parser.py` & `langchain_experimental-0.0.7/langchain_experimental/autonomous_agents/autogpt/output_parser.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,28 +3,26 @@
 from abc import abstractmethod
 from typing import Dict, NamedTuple
 
 from langchain.schema import BaseOutputParser
 
 
 class AutoGPTAction(NamedTuple):
-    """Action for AutoGPT."""
+    """Action returned by AutoGPTOutputParser."""
 
     name: str
-    """Name of the action."""
     args: Dict
-    """Arguments for the action."""
 
 
 class BaseAutoGPTOutputParser(BaseOutputParser):
-    """Base class for AutoGPT output parsers."""
+    """Base Output parser for AutoGPT."""
 
     @abstractmethod
     def parse(self, text: str) -> AutoGPTAction:
-        """Parse text and return AutoGPTAction"""
+        """Return AutoGPTAction"""
 
 
 def preprocess_json_input(input_str: str) -> str:
     """Preprocesses a string to be parsed as json.
 
     Replace single backslashes with double backslashes,
     while leaving already escaped ones intact.
```

### Comparing `langchain_experimental-0.0.6/langchain_experimental/autonomous_agents/autogpt/prompt.py` & `langchain_experimental-0.0.7/langchain_experimental/autonomous_agents/autogpt/prompt.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.6/langchain_experimental/autonomous_agents/autogpt/prompt_generator.py` & `langchain_experimental-0.0.7/langchain_experimental/autonomous_agents/autogpt/prompt_generator.py`

 * *Files 0% similar despite different names*

```diff
@@ -119,15 +119,15 @@
             f"\nEnsure the response can be parsed by Python json.loads"
         )
 
         return prompt_string
 
 
 def get_prompt(tools: List[BaseTool]) -> str:
-    """Generate a prompt string.
+    """Generates a prompt string.
 
     It includes various constraints, commands, resources, and performance evaluations.
 
     Returns:
         str: The generated prompt string.
     """
```

### Comparing `langchain_experimental-0.0.6/langchain_experimental/autonomous_agents/baby_agi/__init__.py` & `langchain_experimental-0.0.7/langchain_experimental/autonomous_agents/baby_agi/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.6/langchain_experimental/autonomous_agents/baby_agi/baby_agi.py` & `langchain_experimental-0.0.7/langchain_experimental/autonomous_agents/baby_agi/baby_agi.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.6/langchain_experimental/autonomous_agents/baby_agi/task_creation.py` & `langchain_experimental-0.0.7/langchain_experimental/autonomous_agents/baby_agi/task_creation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from langchain.chains import LLMChain
 from langchain.prompts import PromptTemplate
 from langchain.schema.language_model import BaseLanguageModel
 
 
 class TaskCreationChain(LLMChain):
-    """Chain to generates tasks."""
+    """Chain generating tasks."""
 
     @classmethod
     def from_llm(cls, llm: BaseLanguageModel, verbose: bool = True) -> LLMChain:
         """Get the response parser."""
         task_creation_template = (
             "You are an task creation AI that uses the result of an execution agent"
             " to create new tasks with the following objective: {objective},"
```

### Comparing `langchain_experimental-0.0.6/langchain_experimental/autonomous_agents/baby_agi/task_execution.py` & `langchain_experimental-0.0.7/langchain_experimental/autonomous_agents/baby_agi/task_execution.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.6/langchain_experimental/autonomous_agents/baby_agi/task_prioritization.py` & `langchain_experimental-0.0.7/langchain_experimental/autonomous_agents/baby_agi/task_prioritization.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.6/langchain_experimental/autonomous_agents/hugginggpt/hugginggpt.py` & `langchain_experimental-0.0.7/langchain_experimental/autonomous_agents/hugginggpt/hugginggpt.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.6/langchain_experimental/autonomous_agents/hugginggpt/repsonse_generator.py` & `langchain_experimental-0.0.7/langchain_experimental/autonomous_agents/hugginggpt/repsonse_generator.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.6/langchain_experimental/autonomous_agents/hugginggpt/task_executor.py` & `langchain_experimental-0.0.7/langchain_experimental/autonomous_agents/hugginggpt/task_executor.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.6/langchain_experimental/autonomous_agents/hugginggpt/task_planner.py` & `langchain_experimental-0.0.7/langchain_experimental/autonomous_agents/hugginggpt/task_planner.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.6/langchain_experimental/cpal/base.py` & `langchain_experimental-0.0.7/langchain_experimental/cpal/base.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.6/langchain_experimental/cpal/models.py` & `langchain_experimental-0.0.7/langchain_experimental/cpal/models.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.6/langchain_experimental/cpal/templates/univariate/causal.py` & `langchain_experimental-0.0.7/langchain_experimental/cpal/templates/univariate/causal.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.6/langchain_experimental/cpal/templates/univariate/intervention.py` & `langchain_experimental-0.0.7/langchain_experimental/cpal/templates/univariate/intervention.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.6/langchain_experimental/cpal/templates/univariate/narrative.py` & `langchain_experimental-0.0.7/langchain_experimental/cpal/templates/univariate/narrative.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.6/langchain_experimental/cpal/templates/univariate/query.py` & `langchain_experimental-0.0.7/langchain_experimental/cpal/templates/univariate/query.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.6/langchain_experimental/generative_agents/generative_agent.py` & `langchain_experimental-0.0.7/langchain_experimental/generative_agents/generative_agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,39 +7,35 @@
 from langchain.schema.language_model import BaseLanguageModel
 from pydantic import BaseModel, Field
 
 from langchain_experimental.generative_agents.memory import GenerativeAgentMemory
 
 
 class GenerativeAgent(BaseModel):
-    """A character with memory and innate characteristics."""
+    """An Agent as a character with memory and innate characteristics."""
 
     name: str
     """The character's name."""
-
     age: Optional[int] = None
     """The optional age of the character."""
     traits: str = "N/A"
     """Permanent traits to ascribe to the character."""
     status: str
     """The traits of the character you wish not to change."""
     memory: GenerativeAgentMemory
     """The memory object that combines relevance, recency, and 'importance'."""
     llm: BaseLanguageModel
     """The underlying language model."""
     verbose: bool = False
     summary: str = ""  #: :meta private:
     """Stateful self-summary generated via reflection on the character's memory."""
-
     summary_refresh_seconds: int = 3600  #: :meta private:
     """How frequently to re-generate the summary."""
-
     last_refreshed: datetime = Field(default_factory=datetime.now)  # : :meta private:
     """The last time the character's summary was regenerated."""
-
     daily_summaries: List[str] = Field(default_factory=list)  # : :meta private:
     """Summary of the events in the plan that the agent took."""
 
     class Config:
         """Configuration for this pydantic object."""
 
         arbitrary_types_allowed = True
```

### Comparing `langchain_experimental-0.0.6/langchain_experimental/generative_agents/memory.py` & `langchain_experimental-0.0.7/langchain_experimental/generative_agents/memory.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,32 +10,29 @@
 from langchain.schema.language_model import BaseLanguageModel
 from langchain.utils import mock_now
 
 logger = logging.getLogger(__name__)
 
 
 class GenerativeAgentMemory(BaseMemory):
+    """Memory for the generative agent."""
+
     llm: BaseLanguageModel
     """The core language model."""
-
     memory_retriever: TimeWeightedVectorStoreRetriever
     """The retriever to fetch related memories."""
     verbose: bool = False
-
     reflection_threshold: Optional[float] = None
     """When aggregate_importance exceeds reflection_threshold, stop to reflect."""
-
     current_plan: List[str] = []
     """The current plan of the agent."""
-
     # A weight of 0.15 makes this less important than it
     # would be otherwise, relative to salience and time
     importance_weight: float = 0.15
     """How much weight to assign the memory importance."""
-
     aggregate_importance: float = 0.0  # : :meta private:
     """Track the sum of the 'importance' of recent memories.
 
     Triggers reflection when it reaches reflection_threshold."""
 
     max_tokens_limit: int = 1200  # : :meta private:
     # input keys
```

### Comparing `langchain_experimental-0.0.6/langchain_experimental/llms/jsonformer_decoder.py` & `langchain_experimental-0.0.7/langchain_experimental/llms/jsonformer_decoder.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,22 +13,27 @@
 
 
 def import_jsonformer() -> jsonformer:
     """Lazily import jsonformer."""
     try:
         import jsonformer
     except ImportError:
-        raise ValueError(
+        raise ImportError(
             "Could not import jsonformer python package. "
             "Please install it with `pip install jsonformer`."
         )
     return jsonformer
 
 
 class JsonFormer(HuggingFacePipeline):
+    """Jsonformer wrapped LLM using HuggingFace Pipeline API.
+
+    This pipeline is experimental and not yet stable.
+    """
+
     json_schema: dict = Field(..., description="The JSON Schema to complete.")
     max_new_tokens: int = Field(
         default=200, description="Maximum number of new tokens to generate."
     )
     debug: bool = Field(default=False, description="Debug mode.")
 
     @root_validator
```

### Comparing `langchain_experimental-0.0.6/langchain_experimental/llms/llamaapi.py` & `langchain_experimental-0.0.7/langchain_experimental/llms/llamaapi.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.6/langchain_experimental/llms/rellm_decoder.py` & `langchain_experimental-0.0.7/langchain_experimental/llms/rellm_decoder.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,22 +19,24 @@
 
 
 def import_rellm() -> rellm:
     """Lazily import rellm."""
     try:
         import rellm
     except ImportError:
-        raise ValueError(
+        raise ImportError(
             "Could not import rellm python package. "
             "Please install it with `pip install rellm`."
         )
     return rellm
 
 
 class RELLM(HuggingFacePipeline):
+    """RELLM wrapped LLM using HuggingFace Pipeline API."""
+
     regex: RegexPattern = Field(..., description="The structured format to complete.")
     max_new_tokens: int = Field(
         default=200, description="Maximum number of new tokens to generate."
     )
 
     @root_validator
     def check_rellm_installation(cls, values: dict) -> dict:
```

### Comparing `langchain_experimental-0.0.6/langchain_experimental/pal_chain/base.py` & `langchain_experimental-0.0.7/langchain_experimental/pal_chain/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,24 +4,22 @@
 solutions. PAL is a technique described in the paper "Program-Aided Language Models"
 (https://arxiv.org/pdf/2211.10435.pdf).
 """
 
 from __future__ import annotations
 
 import ast
-import warnings
 from typing import Any, Dict, List, Optional
 
 from langchain.callbacks.manager import CallbackManagerForChainRun
 from langchain.chains.base import Chain
 from langchain.chains.llm import LLMChain
-from langchain.schema import BasePromptTemplate
 from langchain.schema.language_model import BaseLanguageModel
 from langchain.utilities import PythonREPL
-from pydantic import Extra, Field, root_validator
+from pydantic import Extra, Field
 
 from langchain_experimental.pal_chain.colored_object_prompt import COLORED_OBJECT_PROMPT
 from langchain_experimental.pal_chain.math_prompt import MATH_PROMPT
 
 COMMAND_EXECUTION_FUNCTIONS = ["system", "exec", "execfile", "eval"]
 
 
@@ -91,18 +89,14 @@
 
     This class implements the Program-Aided Language Models (PAL) for generating code
     solutions. PAL is a technique described in the paper "Program-Aided Language Models"
     (https://arxiv.org/pdf/2211.10435.pdf).
     """
 
     llm_chain: LLMChain
-    llm: Optional[BaseLanguageModel] = None
-    """[Deprecated]"""
-    prompt: BasePromptTemplate = MATH_PROMPT
-    """[Deprecated]"""
     stop: str = "\n\n"
     """Stop token to use when generating code."""
     get_answer_expr: str = "print(solution())"
     """Expression to use to get the answer from the generated code."""
     python_globals: Optional[Dict[str, Any]] = None
     """Python globals and locals to use when executing the generated code."""
     python_locals: Optional[Dict[str, Any]] = None
@@ -117,34 +111,21 @@
 
     class Config:
         """Configuration for this pydantic object."""
 
         extra = Extra.forbid
         arbitrary_types_allowed = True
 
-    @root_validator(pre=True)
-    def raise_deprecation(cls, values: Dict) -> Dict:
-        if "llm" in values:
-            warnings.warn(
-                "Directly instantiating a PALChain with an llm is deprecated. "
-                "Please instantiate with llm_chain argument or using one of "
-                "the class method constructors from_math_prompt, "
-                "from_colored_object_prompt."
-            )
-            if "llm_chain" not in values and values["llm"] is not None:
-                values["llm_chain"] = LLMChain(llm=values["llm"], prompt=MATH_PROMPT)
-        return values
-
     @property
     def input_keys(self) -> List[str]:
         """Return the singular input key.
 
         :meta private:
         """
-        return self.prompt.input_variables
+        return self.llm_chain.prompt.input_variables
 
     @property
     def output_keys(self) -> List[str]:
         """Return the singular output key.
 
         :meta private:
         """
```

### Comparing `langchain_experimental-0.0.6/langchain_experimental/pal_chain/colored_object_prompt.py` & `langchain_experimental-0.0.7/langchain_experimental/pal_chain/colored_object_prompt.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.6/langchain_experimental/pal_chain/math_prompt.py` & `langchain_experimental-0.0.7/langchain_experimental/pal_chain/math_prompt.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.6/langchain_experimental/plan_and_execute/agent_executor.py` & `langchain_experimental-0.0.7/langchain_experimental/plan_and_execute/agent_executor.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,17 +12,22 @@
 from langchain_experimental.plan_and_execute.schema import (
     BaseStepContainer,
     ListStepContainer,
 )
 
 
 class PlanAndExecute(Chain):
+    """Plan and execute a chain of steps."""
+
     planner: BasePlanner
+    """The planner to use."""
     executor: BaseExecutor
+    """The executor to use."""
     step_container: BaseStepContainer = Field(default_factory=ListStepContainer)
+    """The step container to use."""
     input_key: str = "input"
     output_key: str = "output"
 
     @property
     def input_keys(self) -> List[str]:
         return [self.input_key]
```

### Comparing `langchain_experimental-0.0.6/langchain_experimental/plan_and_execute/executors/agent_executor.py` & `langchain_experimental-0.0.7/langchain_experimental/plan_and_execute/executors/agent_executor.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.6/langchain_experimental/plan_and_execute/executors/base.py` & `langchain_experimental-0.0.7/langchain_experimental/plan_and_execute/executors/base.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,29 +5,34 @@
 from langchain.chains.base import Chain
 from pydantic import BaseModel
 
 from langchain_experimental.plan_and_execute.schema import StepResponse
 
 
 class BaseExecutor(BaseModel):
+    """Base executor."""
+
     @abstractmethod
     def step(
         self, inputs: dict, callbacks: Callbacks = None, **kwargs: Any
     ) -> StepResponse:
         """Take step."""
 
     @abstractmethod
     async def astep(
         self, inputs: dict, callbacks: Callbacks = None, **kwargs: Any
     ) -> StepResponse:
-        """Take step."""
+        """Take async step."""
 
 
 class ChainExecutor(BaseExecutor):
+    """Chain executor."""
+
     chain: Chain
+    """The chain to use."""
 
     def step(
         self, inputs: dict, callbacks: Callbacks = None, **kwargs: Any
     ) -> StepResponse:
         """Take step."""
         response = self.chain.run(**inputs, callbacks=callbacks)
         return StepResponse(response=response)
```

### Comparing `langchain_experimental-0.0.6/langchain_experimental/plan_and_execute/planners/base.py` & `langchain_experimental-0.0.7/langchain_experimental/plan_and_execute/planners/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,36 +5,43 @@
 from langchain.chains.llm import LLMChain
 from pydantic import BaseModel
 
 from langchain_experimental.plan_and_execute.schema import Plan, PlanOutputParser
 
 
 class BasePlanner(BaseModel):
+    """Base planner."""
+
     @abstractmethod
     def plan(self, inputs: dict, callbacks: Callbacks = None, **kwargs: Any) -> Plan:
         """Given input, decide what to do."""
 
     @abstractmethod
     async def aplan(
         self, inputs: dict, callbacks: Callbacks = None, **kwargs: Any
     ) -> Plan:
-        """Given input, decide what to do."""
+        """Given input, asynchronously decide what to do."""
 
 
 class LLMPlanner(BasePlanner):
+    """LLM planner."""
+
     llm_chain: LLMChain
+    """The LLM chain to use."""
     output_parser: PlanOutputParser
+    """The output parser to use."""
     stop: Optional[List] = None
+    """The stop list to use."""
 
     def plan(self, inputs: dict, callbacks: Callbacks = None, **kwargs: Any) -> Plan:
         """Given input, decide what to do."""
         llm_response = self.llm_chain.run(**inputs, stop=self.stop, callbacks=callbacks)
         return self.output_parser.parse(llm_response)
 
     async def aplan(
         self, inputs: dict, callbacks: Callbacks = None, **kwargs: Any
     ) -> Plan:
-        """Given input, decide what to do."""
+        """Given input, asynchronously decide what to do."""
         llm_response = await self.llm_chain.arun(
             **inputs, stop=self.stop, callbacks=callbacks
         )
         return self.output_parser.parse(llm_response)
```

### Comparing `langchain_experimental-0.0.6/langchain_experimental/plan_and_execute/planners/chat_planner.py` & `langchain_experimental-0.0.7/langchain_experimental/plan_and_execute/planners/chat_planner.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,24 +21,27 @@
     "the final step should almost always be 'Given the above steps taken, "
     "please respond to the users original question'. "
     "At the end of your plan, say '<END_OF_PLAN>'"
 )
 
 
 class PlanningOutputParser(PlanOutputParser):
+    """Planning output parser."""
+
     def parse(self, text: str) -> Plan:
         steps = [Step(value=v) for v in re.split("\n\s*\d+\. ", text)[1:]]
         return Plan(steps=steps)
 
 
 def load_chat_planner(
     llm: BaseLanguageModel, system_prompt: str = SYSTEM_PROMPT
 ) -> LLMPlanner:
     """
     Load a chat planner.
+
     Args:
         llm: Language model.
         system_prompt: System prompt.
 
     Returns:
         LLMPlanner
     """
```

### Comparing `langchain_experimental-0.0.6/langchain_experimental/plan_and_execute/schema.py` & `langchain_experimental-0.0.7/langchain_experimental/plan_and_execute/schema.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,45 +2,61 @@
 from typing import List, Tuple
 
 from langchain.schema import BaseOutputParser
 from pydantic import BaseModel, Field
 
 
 class Step(BaseModel):
+    """Step."""
+
     value: str
+    """The value."""
 
 
 class Plan(BaseModel):
+    """Plan."""
+
     steps: List[Step]
+    """The steps."""
 
 
 class StepResponse(BaseModel):
+    """Step response."""
+
     response: str
+    """The response."""
 
 
 class BaseStepContainer(BaseModel):
+    """Base step container."""
+
     @abstractmethod
     def add_step(self, step: Step, step_response: StepResponse) -> None:
         """Add step and step response to the container."""
 
     @abstractmethod
     def get_final_response(self) -> str:
         """Return the final response based on steps taken."""
 
 
 class ListStepContainer(BaseStepContainer):
+    """List step container."""
+
     steps: List[Tuple[Step, StepResponse]] = Field(default_factory=list)
+    """The steps."""
 
     def add_step(self, step: Step, step_response: StepResponse) -> None:
         self.steps.append((step, step_response))
 
     def get_steps(self) -> List[Tuple[Step, StepResponse]]:
         return self.steps
 
     def get_final_response(self) -> str:
         return self.steps[-1][1].response
 
 
 class PlanOutputParser(BaseOutputParser):
+    """Plan output parser."""
+
     @abstractmethod
     def parse(self, text: str) -> Plan:
         """Parse into a plan."""
```

### Comparing `langchain_experimental-0.0.6/langchain_experimental/prompts/load.py` & `langchain_experimental-0.0.7/langchain_experimental/prompts/load.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.6/langchain_experimental/sql/base.py` & `langchain_experimental-0.0.7/langchain_experimental/sql/base.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.6/langchain_experimental/tot/base.py` & `langchain_experimental-0.0.7/langchain_experimental/tot/base.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.6/langchain_experimental/tot/checker.py` & `langchain_experimental-0.0.7/langchain_experimental/tot/checker.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.6/langchain_experimental/tot/controller.py` & `langchain_experimental-0.0.7/langchain_experimental/tot/controller.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.6/langchain_experimental/tot/memory.py` & `langchain_experimental-0.0.7/langchain_experimental/tot/memory.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.6/langchain_experimental/tot/prompts.py` & `langchain_experimental-0.0.7/langchain_experimental/tot/prompts.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.6/langchain_experimental/tot/thought_generation.py` & `langchain_experimental-0.0.7/langchain_experimental/tot/thought_generation.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.6/pyproject.toml` & `langchain_experimental-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "langchain-experimental"
-version = "0.0.6"
+version = "0.0.7"
 description = "Building applications with LLMs through composability"
 authors = []
 license = "MIT"
 readme = "README.md"
 repository = "https://www.github.com/hwchase17/langchain"
```

### Comparing `langchain_experimental-0.0.6/PKG-INFO` & `langchain_experimental-0.0.7/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain-experimental
-Version: 0.0.6
+Version: 0.0.7
 Summary: Building applications with LLMs through composability
 Home-page: https://www.github.com/hwchase17/langchain
 License: MIT
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

