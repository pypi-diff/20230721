# Comparing `tmp/langchain_experimental-0.0.1rc1.tar.gz` & `tmp/langchain_experimental-0.0.1rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_experimental-0.0.1rc1.tar", max compression
+gzip compressed data, was "langchain_experimental-0.0.1rc2.tar", max compression
```

## Comparing `langchain_experimental-0.0.1rc1.tar` & `langchain_experimental-0.0.1rc2.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0       93 2023-07-21 21:44:15.906230 langchain_experimental-0.0.1rc1/README.md
--rw-r--r--   0        0        0      617 2023-07-21 21:44:15.906230 langchain_experimental-0.0.1rc1/langchain/__init__.py
--rw-r--r--   0        0        0        0 2023-07-21 21:44:15.906230 langchain_experimental-0.0.1rc1/langchain/experimental/__init__.py
--rw-r--r--   0        0        0      188 2023-07-21 21:44:15.906230 langchain_experimental-0.0.1rc1/langchain/experimental/autonomous_agents/__init__.py
--rw-r--r--   0        0        0        0 2023-07-21 21:44:15.906230 langchain_experimental-0.0.1rc1/langchain/experimental/autonomous_agents/autogpt/__init__.py
--rw-r--r--   0        0        0     5244 2023-07-21 21:44:15.906230 langchain_experimental-0.0.1rc1/langchain/experimental/autonomous_agents/autogpt/agent.py
--rw-r--r--   0        0        0     1073 2023-07-21 21:44:15.906230 langchain_experimental-0.0.1rc1/langchain/experimental/autonomous_agents/autogpt/memory.py
--rw-r--r--   0        0        0     1750 2023-07-21 21:44:15.906230 langchain_experimental-0.0.1rc1/langchain/experimental/autonomous_agents/autogpt/output_parser.py
--rw-r--r--   0        0        0     3274 2023-07-21 21:44:15.906230 langchain_experimental-0.0.1rc1/langchain/experimental/autonomous_agents/autogpt/prompt.py
--rw-r--r--   0        0        0     6587 2023-07-21 21:44:15.906230 langchain_experimental-0.0.1rc1/langchain/experimental/autonomous_agents/autogpt/prompt_generator.py
--rw-r--r--   0        0        0      514 2023-07-21 21:44:15.906230 langchain_experimental-0.0.1rc1/langchain/experimental/autonomous_agents/baby_agi/__init__.py
--rw-r--r--   0        0        0     7469 2023-07-21 21:44:15.906230 langchain_experimental-0.0.1rc1/langchain/experimental/autonomous_agents/baby_agi/baby_agi.py
--rw-r--r--   0        0        0     1284 2023-07-21 21:44:15.906230 langchain_experimental-0.0.1rc1/langchain/experimental/autonomous_agents/baby_agi/task_creation.py
--rw-r--r--   0        0        0      835 2023-07-21 21:44:15.906230 langchain_experimental-0.0.1rc1/langchain/experimental/autonomous_agents/baby_agi/task_execution.py
--rw-r--r--   0        0        0     1076 2023-07-21 21:44:15.906230 langchain_experimental-0.0.1rc1/langchain/experimental/autonomous_agents/baby_agi/task_prioritization.py
--rw-r--r--   0        0        0      100 2023-07-21 21:44:15.906230 langchain_experimental-0.0.1rc1/langchain/experimental/cpal/README.md
--rw-r--r--   0        0        0        0 2023-07-21 21:44:15.906230 langchain_experimental-0.0.1rc1/langchain/experimental/cpal/__init__.py
--rw-r--r--   0        0        0     9041 2023-07-21 21:44:15.906230 langchain_experimental-0.0.1rc1/langchain/experimental/cpal/base.py
--rw-r--r--   0        0        0      198 2023-07-21 21:44:15.906230 langchain_experimental-0.0.1rc1/langchain/experimental/cpal/constants.py
--rw-r--r--   0        0        0     8322 2023-07-21 21:44:15.906230 langchain_experimental-0.0.1rc1/langchain/experimental/cpal/models.py
--rw-r--r--   0        0        0        0 2023-07-21 21:44:15.906230 langchain_experimental-0.0.1rc1/langchain/experimental/cpal/templates/__init__.py
--rw-r--r--   0        0        0        0 2023-07-21 21:44:15.906230 langchain_experimental-0.0.1rc1/langchain/experimental/cpal/templates/univariate/__init__.py
--rw-r--r--   0        0        0     2175 2023-07-21 21:44:15.906230 langchain_experimental-0.0.1rc1/langchain/experimental/cpal/templates/univariate/causal.py
--rw-r--r--   0        0        0      706 2023-07-21 21:44:15.906230 langchain_experimental-0.0.1rc1/langchain/experimental/cpal/templates/univariate/intervention.py
--rw-r--r--   0        0        0     1750 2023-07-21 21:44:15.906230 langchain_experimental-0.0.1rc1/langchain/experimental/cpal/templates/univariate/narrative.py
--rw-r--r--   0        0        0     4503 2023-07-21 21:44:15.906230 langchain_experimental-0.0.1rc1/langchain/experimental/cpal/templates/univariate/query.py
--rw-r--r--   0        0        0      260 2023-07-21 21:44:15.906230 langchain_experimental-0.0.1rc1/langchain/experimental/generative_agents/__init__.py
--rw-r--r--   0        0        0    10150 2023-07-21 21:44:15.906230 langchain_experimental-0.0.1rc1/langchain/experimental/generative_agents/generative_agent.py
--rw-r--r--   0        0        0    12461 2023-07-21 21:44:15.906230 langchain_experimental-0.0.1rc1/langchain/experimental/generative_agents/memory.py
--rw-r--r--   0        0        0      199 2023-07-21 21:44:15.906230 langchain_experimental-0.0.1rc1/langchain/experimental/llms/__init__.py
--rw-r--r--   0        0        0     1839 2023-07-21 21:44:15.906230 langchain_experimental-0.0.1rc1/langchain/experimental/llms/jsonformer_decoder.py
--rw-r--r--   0        0        0     2028 2023-07-21 21:44:15.906230 langchain_experimental-0.0.1rc1/langchain/experimental/llms/rellm_decoder.py
--rw-r--r--   0        0        0      277 2023-07-21 21:44:15.906230 langchain_experimental-0.0.1rc1/langchain/experimental/pal_chain/__init__.py
--rw-r--r--   0        0        0    12458 2023-07-21 21:44:15.906230 langchain_experimental-0.0.1rc1/langchain/experimental/pal_chain/base.py
--rw-r--r--   0        0        0     2645 2023-07-21 21:44:15.906230 langchain_experimental-0.0.1rc1/langchain/experimental/pal_chain/colored_object_prompt.py
--rw-r--r--   0        0        0     4301 2023-07-21 21:44:15.906230 langchain_experimental-0.0.1rc1/langchain/experimental/pal_chain/math_prompt.py
--rw-r--r--   0        0        0      363 2023-07-21 21:44:15.906230 langchain_experimental-0.0.1rc1/langchain/experimental/plan_and_execute/__init__.py
--rw-r--r--   0        0        0     2078 2023-07-21 21:44:15.906230 langchain_experimental-0.0.1rc1/langchain/experimental/plan_and_execute/agent_executor.py
--rw-r--r--   0        0        0        0 2023-07-21 21:44:15.906230 langchain_experimental-0.0.1rc1/langchain/experimental/plan_and_execute/executors/__init__.py
--rw-r--r--   0        0        0     1463 2023-07-21 21:44:15.906230 langchain_experimental-0.0.1rc1/langchain/experimental/plan_and_execute/executors/agent_executor.py
--rw-r--r--   0        0        0     1156 2023-07-21 21:44:15.906230 langchain_experimental-0.0.1rc1/langchain/experimental/plan_and_execute/executors/base.py
--rw-r--r--   0        0        0        0 2023-07-21 21:44:15.906230 langchain_experimental-0.0.1rc1/langchain/experimental/plan_and_execute/planners/__init__.py
--rw-r--r--   0        0        0     1362 2023-07-21 21:44:15.906230 langchain_experimental-0.0.1rc1/langchain/experimental/plan_and_execute/planners/base.py
--rw-r--r--   0        0        0     1799 2023-07-21 21:44:15.906230 langchain_experimental-0.0.1rc1/langchain/experimental/plan_and_execute/planners/chat_planner.py
--rw-r--r--   0        0        0     1150 2023-07-21 21:44:15.906230 langchain_experimental-0.0.1rc1/langchain/experimental/plan_and_execute/schema.py
--rw-r--r--   0        0        0       87 2023-07-21 21:44:15.906230 langchain_experimental-0.0.1rc1/langchain/experimental/prompts/__init__.py
--rw-r--r--   0        0        0     1874 2023-07-21 21:44:15.906230 langchain_experimental-0.0.1rc1/langchain/experimental/prompts/load.py
--rw-r--r--   0        0        0      140 2023-07-21 21:44:15.906230 langchain_experimental-0.0.1rc1/langchain/experimental/sql/__init__.py
--rw-r--r--   0        0        0    11414 2023-07-21 21:44:15.906230 langchain_experimental-0.0.1rc1/langchain/experimental/sql/base.py
--rw-r--r--   0        0        0    14202 2023-07-21 21:44:15.906230 langchain_experimental-0.0.1rc1/langchain/experimental/sql/prompt.py
--rw-r--r--   0        0        0     1950 2023-07-21 21:44:15.910230 langchain_experimental-0.0.1rc1/pyproject.toml
--rw-r--r--   0        0        0      720 1970-01-01 00:00:00.000000 langchain_experimental-0.0.1rc1/PKG-INFO
+-rw-r--r--   0        0        0       93 2023-07-21 21:52:48.319310 langchain_experimental-0.0.1rc2/README.md
+-rw-r--r--   0        0        0        1 2023-07-21 21:52:48.319310 langchain_experimental-0.0.1rc2/langchain/__init__.py
+-rw-r--r--   0        0        0      617 2023-07-21 21:52:48.319310 langchain_experimental-0.0.1rc2/langchain/experimental/__init__.py
+-rw-r--r--   0        0        0      188 2023-07-21 21:52:48.319310 langchain_experimental-0.0.1rc2/langchain/experimental/autonomous_agents/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-21 21:52:48.319310 langchain_experimental-0.0.1rc2/langchain/experimental/autonomous_agents/autogpt/__init__.py
+-rw-r--r--   0        0        0     5244 2023-07-21 21:52:48.319310 langchain_experimental-0.0.1rc2/langchain/experimental/autonomous_agents/autogpt/agent.py
+-rw-r--r--   0        0        0     1073 2023-07-21 21:52:48.319310 langchain_experimental-0.0.1rc2/langchain/experimental/autonomous_agents/autogpt/memory.py
+-rw-r--r--   0        0        0     1750 2023-07-21 21:52:48.319310 langchain_experimental-0.0.1rc2/langchain/experimental/autonomous_agents/autogpt/output_parser.py
+-rw-r--r--   0        0        0     3274 2023-07-21 21:52:48.319310 langchain_experimental-0.0.1rc2/langchain/experimental/autonomous_agents/autogpt/prompt.py
+-rw-r--r--   0        0        0     6587 2023-07-21 21:52:48.319310 langchain_experimental-0.0.1rc2/langchain/experimental/autonomous_agents/autogpt/prompt_generator.py
+-rw-r--r--   0        0        0      514 2023-07-21 21:52:48.319310 langchain_experimental-0.0.1rc2/langchain/experimental/autonomous_agents/baby_agi/__init__.py
+-rw-r--r--   0        0        0     7469 2023-07-21 21:52:48.319310 langchain_experimental-0.0.1rc2/langchain/experimental/autonomous_agents/baby_agi/baby_agi.py
+-rw-r--r--   0        0        0     1284 2023-07-21 21:52:48.319310 langchain_experimental-0.0.1rc2/langchain/experimental/autonomous_agents/baby_agi/task_creation.py
+-rw-r--r--   0        0        0      835 2023-07-21 21:52:48.319310 langchain_experimental-0.0.1rc2/langchain/experimental/autonomous_agents/baby_agi/task_execution.py
+-rw-r--r--   0        0        0     1076 2023-07-21 21:52:48.319310 langchain_experimental-0.0.1rc2/langchain/experimental/autonomous_agents/baby_agi/task_prioritization.py
+-rw-r--r--   0        0        0      100 2023-07-21 21:52:48.319310 langchain_experimental-0.0.1rc2/langchain/experimental/cpal/README.md
+-rw-r--r--   0        0        0        0 2023-07-21 21:52:48.319310 langchain_experimental-0.0.1rc2/langchain/experimental/cpal/__init__.py
+-rw-r--r--   0        0        0     9041 2023-07-21 21:52:48.319310 langchain_experimental-0.0.1rc2/langchain/experimental/cpal/base.py
+-rw-r--r--   0        0        0      198 2023-07-21 21:52:48.319310 langchain_experimental-0.0.1rc2/langchain/experimental/cpal/constants.py
+-rw-r--r--   0        0        0     8322 2023-07-21 21:52:48.319310 langchain_experimental-0.0.1rc2/langchain/experimental/cpal/models.py
+-rw-r--r--   0        0        0        0 2023-07-21 21:52:48.319310 langchain_experimental-0.0.1rc2/langchain/experimental/cpal/templates/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-21 21:52:48.319310 langchain_experimental-0.0.1rc2/langchain/experimental/cpal/templates/univariate/__init__.py
+-rw-r--r--   0        0        0     2175 2023-07-21 21:52:48.319310 langchain_experimental-0.0.1rc2/langchain/experimental/cpal/templates/univariate/causal.py
+-rw-r--r--   0        0        0      706 2023-07-21 21:52:48.319310 langchain_experimental-0.0.1rc2/langchain/experimental/cpal/templates/univariate/intervention.py
+-rw-r--r--   0        0        0     1750 2023-07-21 21:52:48.319310 langchain_experimental-0.0.1rc2/langchain/experimental/cpal/templates/univariate/narrative.py
+-rw-r--r--   0        0        0     4503 2023-07-21 21:52:48.319310 langchain_experimental-0.0.1rc2/langchain/experimental/cpal/templates/univariate/query.py
+-rw-r--r--   0        0        0      260 2023-07-21 21:52:48.323310 langchain_experimental-0.0.1rc2/langchain/experimental/generative_agents/__init__.py
+-rw-r--r--   0        0        0    10150 2023-07-21 21:52:48.323310 langchain_experimental-0.0.1rc2/langchain/experimental/generative_agents/generative_agent.py
+-rw-r--r--   0        0        0    12461 2023-07-21 21:52:48.323310 langchain_experimental-0.0.1rc2/langchain/experimental/generative_agents/memory.py
+-rw-r--r--   0        0        0      199 2023-07-21 21:52:48.323310 langchain_experimental-0.0.1rc2/langchain/experimental/llms/__init__.py
+-rw-r--r--   0        0        0     1839 2023-07-21 21:52:48.323310 langchain_experimental-0.0.1rc2/langchain/experimental/llms/jsonformer_decoder.py
+-rw-r--r--   0        0        0     2028 2023-07-21 21:52:48.323310 langchain_experimental-0.0.1rc2/langchain/experimental/llms/rellm_decoder.py
+-rw-r--r--   0        0        0      277 2023-07-21 21:52:48.323310 langchain_experimental-0.0.1rc2/langchain/experimental/pal_chain/__init__.py
+-rw-r--r--   0        0        0    12458 2023-07-21 21:52:48.323310 langchain_experimental-0.0.1rc2/langchain/experimental/pal_chain/base.py
+-rw-r--r--   0        0        0     2645 2023-07-21 21:52:48.323310 langchain_experimental-0.0.1rc2/langchain/experimental/pal_chain/colored_object_prompt.py
+-rw-r--r--   0        0        0     4301 2023-07-21 21:52:48.323310 langchain_experimental-0.0.1rc2/langchain/experimental/pal_chain/math_prompt.py
+-rw-r--r--   0        0        0      363 2023-07-21 21:52:48.323310 langchain_experimental-0.0.1rc2/langchain/experimental/plan_and_execute/__init__.py
+-rw-r--r--   0        0        0     2078 2023-07-21 21:52:48.323310 langchain_experimental-0.0.1rc2/langchain/experimental/plan_and_execute/agent_executor.py
+-rw-r--r--   0        0        0        0 2023-07-21 21:52:48.323310 langchain_experimental-0.0.1rc2/langchain/experimental/plan_and_execute/executors/__init__.py
+-rw-r--r--   0        0        0     1463 2023-07-21 21:52:48.323310 langchain_experimental-0.0.1rc2/langchain/experimental/plan_and_execute/executors/agent_executor.py
+-rw-r--r--   0        0        0     1156 2023-07-21 21:52:48.323310 langchain_experimental-0.0.1rc2/langchain/experimental/plan_and_execute/executors/base.py
+-rw-r--r--   0        0        0        0 2023-07-21 21:52:48.323310 langchain_experimental-0.0.1rc2/langchain/experimental/plan_and_execute/planners/__init__.py
+-rw-r--r--   0        0        0     1362 2023-07-21 21:52:48.323310 langchain_experimental-0.0.1rc2/langchain/experimental/plan_and_execute/planners/base.py
+-rw-r--r--   0        0        0     1799 2023-07-21 21:52:48.323310 langchain_experimental-0.0.1rc2/langchain/experimental/plan_and_execute/planners/chat_planner.py
+-rw-r--r--   0        0        0     1150 2023-07-21 21:52:48.323310 langchain_experimental-0.0.1rc2/langchain/experimental/plan_and_execute/schema.py
+-rw-r--r--   0        0        0       87 2023-07-21 21:52:48.323310 langchain_experimental-0.0.1rc2/langchain/experimental/prompts/__init__.py
+-rw-r--r--   0        0        0     1874 2023-07-21 21:52:48.323310 langchain_experimental-0.0.1rc2/langchain/experimental/prompts/load.py
+-rw-r--r--   0        0        0      140 2023-07-21 21:52:48.323310 langchain_experimental-0.0.1rc2/langchain/experimental/sql/__init__.py
+-rw-r--r--   0        0        0    11414 2023-07-21 21:52:48.323310 langchain_experimental-0.0.1rc2/langchain/experimental/sql/base.py
+-rw-r--r--   0        0        0    14202 2023-07-21 21:52:48.323310 langchain_experimental-0.0.1rc2/langchain/experimental/sql/prompt.py
+-rw-r--r--   0        0        0     1950 2023-07-21 21:52:48.327310 langchain_experimental-0.0.1rc2/pyproject.toml
+-rw-r--r--   0        0        0      720 1970-01-01 00:00:00.000000 langchain_experimental-0.0.1rc2/PKG-INFO
```

### Comparing `langchain_experimental-0.0.1rc1/langchain/__init__.py` & `langchain_experimental-0.0.1rc2/langchain/experimental/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.1rc1/langchain/experimental/autonomous_agents/autogpt/agent.py` & `langchain_experimental-0.0.1rc2/langchain/experimental/autonomous_agents/autogpt/agent.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.1rc1/langchain/experimental/autonomous_agents/autogpt/memory.py` & `langchain_experimental-0.0.1rc2/langchain/experimental/autonomous_agents/autogpt/memory.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.1rc1/langchain/experimental/autonomous_agents/autogpt/output_parser.py` & `langchain_experimental-0.0.1rc2/langchain/experimental/autonomous_agents/autogpt/output_parser.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.1rc1/langchain/experimental/autonomous_agents/autogpt/prompt.py` & `langchain_experimental-0.0.1rc2/langchain/experimental/autonomous_agents/autogpt/prompt.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.1rc1/langchain/experimental/autonomous_agents/autogpt/prompt_generator.py` & `langchain_experimental-0.0.1rc2/langchain/experimental/autonomous_agents/autogpt/prompt_generator.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.1rc1/langchain/experimental/autonomous_agents/baby_agi/__init__.py` & `langchain_experimental-0.0.1rc2/langchain/experimental/autonomous_agents/baby_agi/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.1rc1/langchain/experimental/autonomous_agents/baby_agi/baby_agi.py` & `langchain_experimental-0.0.1rc2/langchain/experimental/autonomous_agents/baby_agi/baby_agi.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.1rc1/langchain/experimental/autonomous_agents/baby_agi/task_creation.py` & `langchain_experimental-0.0.1rc2/langchain/experimental/autonomous_agents/baby_agi/task_creation.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.1rc1/langchain/experimental/autonomous_agents/baby_agi/task_execution.py` & `langchain_experimental-0.0.1rc2/langchain/experimental/autonomous_agents/baby_agi/task_execution.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.1rc1/langchain/experimental/autonomous_agents/baby_agi/task_prioritization.py` & `langchain_experimental-0.0.1rc2/langchain/experimental/autonomous_agents/baby_agi/task_prioritization.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.1rc1/langchain/experimental/cpal/base.py` & `langchain_experimental-0.0.1rc2/langchain/experimental/cpal/base.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.1rc1/langchain/experimental/cpal/models.py` & `langchain_experimental-0.0.1rc2/langchain/experimental/cpal/models.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.1rc1/langchain/experimental/cpal/templates/univariate/causal.py` & `langchain_experimental-0.0.1rc2/langchain/experimental/cpal/templates/univariate/causal.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.1rc1/langchain/experimental/cpal/templates/univariate/intervention.py` & `langchain_experimental-0.0.1rc2/langchain/experimental/cpal/templates/univariate/intervention.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.1rc1/langchain/experimental/cpal/templates/univariate/narrative.py` & `langchain_experimental-0.0.1rc2/langchain/experimental/cpal/templates/univariate/narrative.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.1rc1/langchain/experimental/cpal/templates/univariate/query.py` & `langchain_experimental-0.0.1rc2/langchain/experimental/cpal/templates/univariate/query.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.1rc1/langchain/experimental/generative_agents/generative_agent.py` & `langchain_experimental-0.0.1rc2/langchain/experimental/generative_agents/generative_agent.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.1rc1/langchain/experimental/generative_agents/memory.py` & `langchain_experimental-0.0.1rc2/langchain/experimental/generative_agents/memory.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.1rc1/langchain/experimental/llms/jsonformer_decoder.py` & `langchain_experimental-0.0.1rc2/langchain/experimental/llms/jsonformer_decoder.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.1rc1/langchain/experimental/llms/rellm_decoder.py` & `langchain_experimental-0.0.1rc2/langchain/experimental/llms/rellm_decoder.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.1rc1/langchain/experimental/pal_chain/base.py` & `langchain_experimental-0.0.1rc2/langchain/experimental/pal_chain/base.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.1rc1/langchain/experimental/pal_chain/colored_object_prompt.py` & `langchain_experimental-0.0.1rc2/langchain/experimental/pal_chain/colored_object_prompt.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.1rc1/langchain/experimental/pal_chain/math_prompt.py` & `langchain_experimental-0.0.1rc2/langchain/experimental/pal_chain/math_prompt.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.1rc1/langchain/experimental/plan_and_execute/agent_executor.py` & `langchain_experimental-0.0.1rc2/langchain/experimental/plan_and_execute/agent_executor.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.1rc1/langchain/experimental/plan_and_execute/executors/agent_executor.py` & `langchain_experimental-0.0.1rc2/langchain/experimental/plan_and_execute/executors/agent_executor.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.1rc1/langchain/experimental/plan_and_execute/executors/base.py` & `langchain_experimental-0.0.1rc2/langchain/experimental/plan_and_execute/executors/base.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.1rc1/langchain/experimental/plan_and_execute/planners/base.py` & `langchain_experimental-0.0.1rc2/langchain/experimental/plan_and_execute/planners/base.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.1rc1/langchain/experimental/plan_and_execute/planners/chat_planner.py` & `langchain_experimental-0.0.1rc2/langchain/experimental/plan_and_execute/planners/chat_planner.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.1rc1/langchain/experimental/plan_and_execute/schema.py` & `langchain_experimental-0.0.1rc2/langchain/experimental/plan_and_execute/schema.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.1rc1/langchain/experimental/prompts/load.py` & `langchain_experimental-0.0.1rc2/langchain/experimental/prompts/load.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.1rc1/langchain/experimental/sql/base.py` & `langchain_experimental-0.0.1rc2/langchain/experimental/sql/base.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.1rc1/langchain/experimental/sql/prompt.py` & `langchain_experimental-0.0.1rc2/langchain/experimental/sql/prompt.py`

 * *Files identical despite different names*

### Comparing `langchain_experimental-0.0.1rc1/pyproject.toml` & `langchain_experimental-0.0.1rc2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "langchain-experimental"
-version = "0.0.1rc1"
+version = "0.0.1rc2"
 description = "Building applications with LLMs through composability"
 authors = []
 license = "MIT"
 readme = "README.md"
 repository = "https://www.github.com/hwchase17/langchain"
 packages = [
     {include = "langchain"}
```

### Comparing `langchain_experimental-0.0.1rc1/PKG-INFO` & `langchain_experimental-0.0.1rc2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain-experimental
-Version: 0.0.1rc1
+Version: 0.0.1rc2
 Summary: Building applications with LLMs through composability
 Home-page: https://www.github.com/hwchase17/langchain
 License: MIT
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

