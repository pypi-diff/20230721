# Comparing `tmp/semantic_kernel-0.3.3.dev0.tar.gz` & `tmp/semantic_kernel-0.3.4.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "semantic_kernel-0.3.3.dev0.tar", max compression
+gzip compressed data, was "semantic_kernel-0.3.4.dev0.tar", max compression
```

## Comparing `semantic_kernel-0.3.3.dev0.tar` & `semantic_kernel-0.3.4.dev0.tar`

### file list

```diff
@@ -1,105 +1,107 @@
--rw-r--r--   0        0        0     1186 2023-05-08 23:38:10.000000 semantic_kernel-0.3.3.dev0/pip/README.md
--rw-r--r--   0        0        0     1322 2023-07-18 01:08:06.924816 semantic_kernel-0.3.3.dev0/pyproject.toml
--rw-r--r--   0        0        0     1375 2023-07-12 19:14:40.912511 semantic_kernel-0.3.3.dev0/semantic_kernel/__init__.py
--rw-r--r--   0        0        0      719 2023-05-25 17:48:21.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/connectors/ai/__init__.py
--rw-r--r--   0        0        0     1647 2023-04-30 18:57:02.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/connectors/ai/ai_exception.py
--rw-r--r--   0        0        0     1792 2023-06-12 17:06:53.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/connectors/ai/chat_completion_client_base.py
--rw-r--r--   0        0        0     1321 2023-07-14 16:57:26.312407 semantic_kernel-0.3.3.dev0/semantic_kernel/connectors/ai/chat_request_settings.py
--rw-r--r--   0        0        0     1484 2023-07-14 16:57:26.312942 semantic_kernel-0.3.3.dev0/semantic_kernel/connectors/ai/complete_request_settings.py
--rw-r--r--   0        0        0      282 2023-04-30 18:57:02.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/connectors/ai/embeddings/embedding_generator_base.py
--rw-r--r--   0        0        0      352 2023-04-30 18:57:02.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/connectors/ai/hugging_face/__init__.py
--rw-r--r--   0        0        0     6161 2023-06-12 17:06:53.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/connectors/ai/hugging_face/services/hf_text_completion.py
--rw-r--r--   0        0        0     2317 2023-05-08 23:38:10.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/connectors/ai/hugging_face/services/hf_text_embedding.py
--rw-r--r--   0        0        0      892 2023-04-30 18:57:02.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/connectors/ai/open_ai/__init__.py
--rw-r--r--   0        0        0     2615 2023-05-15 18:12:57.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_chat_completion.py
--rw-r--r--   0        0        0     2607 2023-05-15 18:12:57.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_text_completion.py
--rw-r--r--   0        0        0     2602 2023-05-15 18:12:57.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_text_embedding.py
--rw-r--r--   0        0        0     8903 2023-07-16 00:59:27.692753 semantic_kernel-0.3.3.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_chat_completion.py
--rw-r--r--   0        0        0     5788 2023-07-16 00:59:27.693316 semantic_kernel-0.3.3.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_completion.py
--rw-r--r--   0        0        0     2723 2023-05-15 18:12:57.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_embedding.py
--rw-r--r--   0        0        0     1616 2023-06-12 17:06:53.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/connectors/ai/text_completion_client_base.py
--rw-r--r--   0        0        0      204 2023-07-16 07:20:48.222581 semantic_kernel-0.3.3.dev0/semantic_kernel/connectors/memory/azure_search/__init__.py
--rw-r--r--   0        0        0    16254 2023-07-16 07:20:48.223592 semantic_kernel-0.3.3.dev0/semantic_kernel/connectors/memory/azure_search/azure_search_memory_store.py
--rw-r--r--   0        0        0     8040 2023-07-16 07:20:48.224597 semantic_kernel-0.3.3.dev0/semantic_kernel/connectors/memory/azure_search/utils.py
--rw-r--r--   0        0        0      182 2023-05-18 17:32:52.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/connectors/memory/chroma/__init__.py
--rw-r--r--   0        0        0    15273 2023-07-16 00:58:37.999718 semantic_kernel-0.3.3.dev0/semantic_kernel/connectors/memory/chroma/chroma_memory_store.py
--rw-r--r--   0        0        0     4426 2023-07-16 00:58:38.000353 semantic_kernel-0.3.3.dev0/semantic_kernel/connectors/memory/chroma/utils.py
--rw-r--r--   0        0        0      190 2023-07-06 22:13:35.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/connectors/memory/pinecone/__init__.py
--rw-r--r--   0        0        0    14928 2023-07-12 19:14:40.913001 semantic_kernel-0.3.3.dev0/semantic_kernel/connectors/memory/pinecone/pinecone_memory_store.py
--rw-r--r--   0        0        0     1154 2023-07-06 22:13:35.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/connectors/memory/pinecone/utils.py
--rw-r--r--   0        0        0      190 2023-07-12 19:14:40.913420 semantic_kernel-0.3.3.dev0/semantic_kernel/connectors/memory/postgres/__init__.py
--rw-r--r--   0        0        0    20480 2023-07-12 19:14:40.913726 semantic_kernel-0.3.3.dev0/semantic_kernel/connectors/memory/postgres/postgres_memory_store.py
--rw-r--r--   0        0        0    11295 2023-06-12 17:06:53.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/connectors/memory/weaviate/weaviate_memory_store.py
--rw-r--r--   0        0        0      111 2023-07-17 21:15:24.598216 semantic_kernel-0.3.3.dev0/semantic_kernel/connectors/search_engine/__init__.py
--rw-r--r--   0        0        0     2842 2023-07-17 21:15:24.598630 semantic_kernel-0.3.3.dev0/semantic_kernel/connectors/search_engine/bing_connector.py
--rw-r--r--   0        0        0      173 2023-07-17 21:15:24.599030 semantic_kernel-0.3.3.dev0/semantic_kernel/connectors/search_engine/connector.py
--rw-r--r--   0        0        0      804 2023-07-17 21:15:24.599960 semantic_kernel-0.3.3.dev0/semantic_kernel/core_skills/__init__.py
--rw-r--r--   0        0        0     2510 2023-05-15 18:12:57.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/core_skills/conversation_summary_skill.py
--rw-r--r--   0        0        0     2131 2023-07-16 00:59:27.693756 semantic_kernel-0.3.3.dev0/semantic_kernel/core_skills/file_io_skill.py
--rw-r--r--   0        0        0     3754 2023-04-22 04:06:40.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/core_skills/http_skill.py
--rw-r--r--   0        0        0     3171 2023-07-06 22:13:35.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/core_skills/math_skill.py
--rw-r--r--   0        0        0     4641 2023-04-14 00:51:57.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/core_skills/text_memory_skill.py
--rw-r--r--   0        0        0     2462 2023-07-16 00:59:27.694343 semantic_kernel-0.3.3.dev0/semantic_kernel/core_skills/text_skill.py
--rw-r--r--   0        0        0     7909 2023-07-16 00:59:27.694865 semantic_kernel-0.3.3.dev0/semantic_kernel/core_skills/time_skill.py
--rw-r--r--   0        0        0      678 2023-07-16 00:59:27.695359 semantic_kernel-0.3.3.dev0/semantic_kernel/core_skills/wait_skill.py
--rw-r--r--   0        0        0     1950 2023-07-17 21:15:24.600357 semantic_kernel-0.3.3.dev0/semantic_kernel/core_skills/web_search_engine_skill.py
--rw-r--r--   0        0        0    32289 2023-07-17 21:15:24.601483 semantic_kernel-0.3.3.dev0/semantic_kernel/kernel.py
--rw-r--r--   0        0        0     1726 2023-07-16 00:59:27.695868 semantic_kernel-0.3.3.dev0/semantic_kernel/kernel_exception.py
--rw-r--r--   0        0        0      160 2023-04-13 23:12:46.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/memory/__init__.py
--rw-r--r--   0        0        0     2544 2023-06-08 17:22:29.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/memory/memory_query_result.py
--rw-r--r--   0        0        0     3912 2023-07-12 19:14:40.914195 semantic_kernel-0.3.3.dev0/semantic_kernel/memory/memory_record.py
--rw-r--r--   0        0        0     2014 2023-05-19 23:02:13.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/memory/memory_store_base.py
--rw-r--r--   0        0        0     1272 2023-06-08 17:22:29.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/memory/null_memory.py
--rw-r--r--   0        0        0     6354 2023-07-16 00:42:59.250269 semantic_kernel-0.3.3.dev0/semantic_kernel/memory/semantic_text_memory.py
--rw-r--r--   0        0        0     1298 2023-06-08 17:22:29.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/memory/semantic_text_memory_base.py
--rw-r--r--   0        0        0    12032 2023-05-15 18:12:57.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/memory/volatile_memory_store.py
--rw-r--r--   0        0        0     2361 2023-04-22 04:06:40.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/orchestration/context_variables.py
--rw-r--r--   0        0        0     5079 2023-04-14 00:51:57.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/orchestration/delegate_handlers.py
--rw-r--r--   0        0        0     9005 2023-05-19 23:02:13.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/orchestration/delegate_inference.py
--rw-r--r--   0        0        0      638 2023-04-13 23:12:46.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/orchestration/delegate_types.py
--rw-r--r--   0        0        0     7514 2023-04-14 00:52:05.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/orchestration/sk_context.py
--rw-r--r--   0        0        0    16088 2023-07-06 22:13:35.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/orchestration/sk_function.py
--rw-r--r--   0        0        0     6158 2023-04-30 18:57:02.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/orchestration/sk_function_base.py
--rw-r--r--   0        0        0      158 2023-05-08 23:38:10.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/planning/__init__.py
--rw-r--r--   0        0        0     7538 2023-07-06 22:13:35.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/planning/basic_planner.py
--rw-r--r--   0        0        0    15624 2023-07-16 00:59:27.696327 semantic_kernel-0.3.3.dev0/semantic_kernel/planning/plan.py
--rw-r--r--   0        0        0      932 2023-05-19 23:02:13.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/reliability/pass_through_without_retry.py
--rw-r--r--   0        0        0      694 2023-06-05 21:39:19.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/reliability/retry_mechanism_base.py
--rw-r--r--   0        0        0     2101 2023-04-13 23:12:46.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/semantic_functions/chat_prompt_template.py
--rw-r--r--   0        0        0     2332 2023-04-14 00:51:57.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/semantic_functions/prompt_template.py
--rw-r--r--   0        0        0      506 2023-04-13 23:12:46.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/semantic_functions/prompt_template_base.py
--rw-r--r--   0        0        0     4525 2023-06-12 17:06:53.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/semantic_functions/prompt_template_config.py
--rw-r--r--   0        0        0      671 2023-04-14 00:51:57.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/semantic_functions/semantic_function_config.py
--rw-r--r--   0        0        0      322 2023-04-14 00:51:57.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/skill_definition/__init__.py
--rw-r--r--   0        0        0     2053 2023-04-14 00:51:57.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/skill_definition/function_view.py
--rw-r--r--   0        0        0     2199 2023-06-12 17:06:53.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/skill_definition/functions_view.py
--rw-r--r--   0        0        0     1026 2023-04-14 00:51:57.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/skill_definition/parameter_view.py
--rw-r--r--   0        0        0     2104 2023-04-14 00:51:57.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/skill_definition/read_only_skill_collection.py
--rw-r--r--   0        0        0     1345 2023-04-14 00:51:57.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/skill_definition/read_only_skill_collection_base.py
--rw-r--r--   0        0        0      858 2023-04-13 23:12:46.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/skill_definition/sk_function_context_parameter_decorator.py
--rw-r--r--   0        0        0      837 2023-04-14 00:51:57.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/skill_definition/sk_function_decorator.py
--rw-r--r--   0        0        0     6056 2023-04-14 00:51:57.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/skill_definition/skill_collection.py
--rw-r--r--   0        0        0      803 2023-04-13 23:12:46.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/skill_definition/skill_collection_base.py
--rw-r--r--   0        0        0     1115 2023-04-13 23:12:46.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/template_engine/README.md
--rw-r--r--   0        0        0      830 2023-04-14 00:51:57.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/template_engine/blocks/block.py
--rw-r--r--   0        0        0      228 2023-04-14 00:51:57.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/template_engine/blocks/block_types.py
--rw-r--r--   0        0        0     4577 2023-04-30 18:57:03.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/template_engine/blocks/code_block.py
--rw-r--r--   0        0        0     2653 2023-04-13 23:12:46.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/template_engine/blocks/function_id_block.py
--rw-r--r--   0        0        0      276 2023-04-13 23:12:46.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/template_engine/blocks/symbols.py
--rw-r--r--   0        0        0     1534 2023-04-14 00:51:57.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/template_engine/blocks/text_block.py
--rw-r--r--   0        0        0     2274 2023-04-13 23:12:46.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/template_engine/blocks/val_block.py
--rw-r--r--   0        0        0     2517 2023-04-14 00:51:57.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/template_engine/blocks/var_block.py
--rw-r--r--   0        0        0     6535 2023-04-13 23:12:46.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/template_engine/code_tokenizer.py
--rw-r--r--   0        0        0     6051 2023-04-14 00:51:57.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/template_engine/prompt_template_engine.py
--rw-r--r--   0        0        0      532 2023-04-13 23:12:46.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/template_engine/protocols/code_renderer.py
--rw-r--r--   0        0        0     3043 2023-04-13 23:12:46.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/template_engine/protocols/prompt_templating_engine.py
--rw-r--r--   0        0        0      596 2023-04-13 23:12:46.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/template_engine/protocols/text_renderer.py
--rw-r--r--   0        0        0     7637 2023-04-13 23:12:46.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/template_engine/template_tokenizer.py
--rw-r--r--   0        0        0      473 2023-04-30 18:57:03.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/text/__init__.py
--rw-r--r--   0        0        0      667 2023-04-30 18:57:03.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/text/function_extension.py
--rw-r--r--   0        0        0     8568 2023-07-16 00:58:38.006510 semantic_kernel-0.3.3.dev0/semantic_kernel/text/text_chunker.py
--rw-r--r--   0        0        0      403 2023-04-13 23:12:46.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/utils/null_logger.py
--rw-r--r--   0        0        0     2694 2023-07-12 19:14:40.915313 semantic_kernel-0.3.3.dev0/semantic_kernel/utils/settings.py
--rw-r--r--   0        0        0      221 2023-04-13 23:12:46.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/utils/static_property.py
--rw-r--r--   0        0        0     2198 2023-04-13 23:12:46.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/utils/validation.py
--rw-r--r--   0        0        0     1843 1970-01-01 00:00:00.000000 semantic_kernel-0.3.3.dev0/PKG-INFO
+-rw-r--r--   0        0        0     1186 2023-05-08 23:38:10.000000 semantic_kernel-0.3.4.dev0/pip/README.md
+-rw-r--r--   0        0        0     1412 2023-07-21 00:27:08.415513 semantic_kernel-0.3.4.dev0/pyproject.toml
+-rw-r--r--   0        0        0     1375 2023-07-12 19:14:40.912511 semantic_kernel-0.3.4.dev0/semantic_kernel/__init__.py
+-rw-r--r--   0        0        0      719 2023-05-25 17:48:21.000000 semantic_kernel-0.3.4.dev0/semantic_kernel/connectors/ai/__init__.py
+-rw-r--r--   0        0        0     1647 2023-04-30 18:57:02.000000 semantic_kernel-0.3.4.dev0/semantic_kernel/connectors/ai/ai_exception.py
+-rw-r--r--   0        0        0     1792 2023-06-12 17:06:53.000000 semantic_kernel-0.3.4.dev0/semantic_kernel/connectors/ai/chat_completion_client_base.py
+-rw-r--r--   0        0        0     1321 2023-07-14 16:57:26.312407 semantic_kernel-0.3.4.dev0/semantic_kernel/connectors/ai/chat_request_settings.py
+-rw-r--r--   0        0        0     1484 2023-07-14 16:57:26.312942 semantic_kernel-0.3.4.dev0/semantic_kernel/connectors/ai/complete_request_settings.py
+-rw-r--r--   0        0        0      282 2023-04-30 18:57:02.000000 semantic_kernel-0.3.4.dev0/semantic_kernel/connectors/ai/embeddings/embedding_generator_base.py
+-rw-r--r--   0        0        0      352 2023-04-30 18:57:02.000000 semantic_kernel-0.3.4.dev0/semantic_kernel/connectors/ai/hugging_face/__init__.py
+-rw-r--r--   0        0        0     6161 2023-06-12 17:06:53.000000 semantic_kernel-0.3.4.dev0/semantic_kernel/connectors/ai/hugging_face/services/hf_text_completion.py
+-rw-r--r--   0        0        0     2317 2023-05-08 23:38:10.000000 semantic_kernel-0.3.4.dev0/semantic_kernel/connectors/ai/hugging_face/services/hf_text_embedding.py
+-rw-r--r--   0        0        0      892 2023-04-30 18:57:02.000000 semantic_kernel-0.3.4.dev0/semantic_kernel/connectors/ai/open_ai/__init__.py
+-rw-r--r--   0        0        0     2615 2023-05-15 18:12:57.000000 semantic_kernel-0.3.4.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_chat_completion.py
+-rw-r--r--   0        0        0     2607 2023-05-15 18:12:57.000000 semantic_kernel-0.3.4.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_text_completion.py
+-rw-r--r--   0        0        0     2602 2023-05-15 18:12:57.000000 semantic_kernel-0.3.4.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_text_embedding.py
+-rw-r--r--   0        0        0     8903 2023-07-16 00:59:27.692753 semantic_kernel-0.3.4.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_chat_completion.py
+-rw-r--r--   0        0        0     5788 2023-07-16 00:59:27.693316 semantic_kernel-0.3.4.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_completion.py
+-rw-r--r--   0        0        0     2723 2023-05-15 18:12:57.000000 semantic_kernel-0.3.4.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_embedding.py
+-rw-r--r--   0        0        0     1616 2023-06-12 17:06:53.000000 semantic_kernel-0.3.4.dev0/semantic_kernel/connectors/ai/text_completion_client_base.py
+-rw-r--r--   0        0        0      242 2023-07-21 00:24:52.991872 semantic_kernel-0.3.4.dev0/semantic_kernel/connectors/memory/azure_cognitive_search/__init__.py
+-rw-r--r--   0        0        0    15609 2023-07-21 00:24:52.992413 semantic_kernel-0.3.4.dev0/semantic_kernel/connectors/memory/azure_cognitive_search/azure_cognitive_search_memory_store.py
+-rw-r--r--   0        0        0     8224 2023-07-21 00:24:52.992894 semantic_kernel-0.3.4.dev0/semantic_kernel/connectors/memory/azure_cognitive_search/utils.py
+-rw-r--r--   0        0        0      182 2023-05-18 17:32:52.000000 semantic_kernel-0.3.4.dev0/semantic_kernel/connectors/memory/chroma/__init__.py
+-rw-r--r--   0        0        0    15260 2023-07-21 00:24:52.994825 semantic_kernel-0.3.4.dev0/semantic_kernel/connectors/memory/chroma/chroma_memory_store.py
+-rw-r--r--   0        0        0     4426 2023-07-16 00:58:38.000353 semantic_kernel-0.3.4.dev0/semantic_kernel/connectors/memory/chroma/utils.py
+-rw-r--r--   0        0        0      133 2023-07-21 00:24:52.995551 semantic_kernel-0.3.4.dev0/semantic_kernel/connectors/memory/milvus/__init__.py
+-rw-r--r--   0        0        0    16859 2023-07-21 00:24:52.995917 semantic_kernel-0.3.4.dev0/semantic_kernel/connectors/memory/milvus/milvus_memory_store.py
+-rw-r--r--   0        0        0      190 2023-07-06 22:13:35.000000 semantic_kernel-0.3.4.dev0/semantic_kernel/connectors/memory/pinecone/__init__.py
+-rw-r--r--   0        0        0    14928 2023-07-12 19:14:40.913001 semantic_kernel-0.3.4.dev0/semantic_kernel/connectors/memory/pinecone/pinecone_memory_store.py
+-rw-r--r--   0        0        0     1154 2023-07-06 22:13:35.000000 semantic_kernel-0.3.4.dev0/semantic_kernel/connectors/memory/pinecone/utils.py
+-rw-r--r--   0        0        0      190 2023-07-12 19:14:40.913420 semantic_kernel-0.3.4.dev0/semantic_kernel/connectors/memory/postgres/__init__.py
+-rw-r--r--   0        0        0    20480 2023-07-12 19:14:40.913726 semantic_kernel-0.3.4.dev0/semantic_kernel/connectors/memory/postgres/postgres_memory_store.py
+-rw-r--r--   0        0        0    11295 2023-06-12 17:06:53.000000 semantic_kernel-0.3.4.dev0/semantic_kernel/connectors/memory/weaviate/weaviate_memory_store.py
+-rw-r--r--   0        0        0      111 2023-07-17 21:15:24.598216 semantic_kernel-0.3.4.dev0/semantic_kernel/connectors/search_engine/__init__.py
+-rw-r--r--   0        0        0     2842 2023-07-17 21:15:24.598630 semantic_kernel-0.3.4.dev0/semantic_kernel/connectors/search_engine/bing_connector.py
+-rw-r--r--   0        0        0      173 2023-07-17 21:15:24.599030 semantic_kernel-0.3.4.dev0/semantic_kernel/connectors/search_engine/connector.py
+-rw-r--r--   0        0        0      804 2023-07-17 21:15:24.599960 semantic_kernel-0.3.4.dev0/semantic_kernel/core_skills/__init__.py
+-rw-r--r--   0        0        0     2510 2023-05-15 18:12:57.000000 semantic_kernel-0.3.4.dev0/semantic_kernel/core_skills/conversation_summary_skill.py
+-rw-r--r--   0        0        0     2131 2023-07-16 00:59:27.693756 semantic_kernel-0.3.4.dev0/semantic_kernel/core_skills/file_io_skill.py
+-rw-r--r--   0        0        0     3754 2023-04-22 04:06:40.000000 semantic_kernel-0.3.4.dev0/semantic_kernel/core_skills/http_skill.py
+-rw-r--r--   0        0        0     3171 2023-07-06 22:13:35.000000 semantic_kernel-0.3.4.dev0/semantic_kernel/core_skills/math_skill.py
+-rw-r--r--   0        0        0     4641 2023-04-14 00:51:57.000000 semantic_kernel-0.3.4.dev0/semantic_kernel/core_skills/text_memory_skill.py
+-rw-r--r--   0        0        0     2462 2023-07-16 00:59:27.694343 semantic_kernel-0.3.4.dev0/semantic_kernel/core_skills/text_skill.py
+-rw-r--r--   0        0        0     7909 2023-07-16 00:59:27.694865 semantic_kernel-0.3.4.dev0/semantic_kernel/core_skills/time_skill.py
+-rw-r--r--   0        0        0      678 2023-07-16 00:59:27.695359 semantic_kernel-0.3.4.dev0/semantic_kernel/core_skills/wait_skill.py
+-rw-r--r--   0        0        0     1950 2023-07-17 21:15:24.600357 semantic_kernel-0.3.4.dev0/semantic_kernel/core_skills/web_search_engine_skill.py
+-rw-r--r--   0        0        0    32289 2023-07-17 21:15:24.601483 semantic_kernel-0.3.4.dev0/semantic_kernel/kernel.py
+-rw-r--r--   0        0        0     1726 2023-07-16 00:59:27.695868 semantic_kernel-0.3.4.dev0/semantic_kernel/kernel_exception.py
+-rw-r--r--   0        0        0      160 2023-04-13 23:12:46.000000 semantic_kernel-0.3.4.dev0/semantic_kernel/memory/__init__.py
+-rw-r--r--   0        0        0     2544 2023-06-08 17:22:29.000000 semantic_kernel-0.3.4.dev0/semantic_kernel/memory/memory_query_result.py
+-rw-r--r--   0        0        0     3912 2023-07-12 19:14:40.914195 semantic_kernel-0.3.4.dev0/semantic_kernel/memory/memory_record.py
+-rw-r--r--   0        0        0     2186 2023-07-21 00:24:52.996840 semantic_kernel-0.3.4.dev0/semantic_kernel/memory/memory_store_base.py
+-rw-r--r--   0        0        0     1272 2023-06-08 17:22:29.000000 semantic_kernel-0.3.4.dev0/semantic_kernel/memory/null_memory.py
+-rw-r--r--   0        0        0     6354 2023-07-16 00:42:59.250269 semantic_kernel-0.3.4.dev0/semantic_kernel/memory/semantic_text_memory.py
+-rw-r--r--   0        0        0     1298 2023-06-08 17:22:29.000000 semantic_kernel-0.3.4.dev0/semantic_kernel/memory/semantic_text_memory_base.py
+-rw-r--r--   0        0        0    12032 2023-05-15 18:12:57.000000 semantic_kernel-0.3.4.dev0/semantic_kernel/memory/volatile_memory_store.py
+-rw-r--r--   0        0        0     2361 2023-04-22 04:06:40.000000 semantic_kernel-0.3.4.dev0/semantic_kernel/orchestration/context_variables.py
+-rw-r--r--   0        0        0     5079 2023-04-14 00:51:57.000000 semantic_kernel-0.3.4.dev0/semantic_kernel/orchestration/delegate_handlers.py
+-rw-r--r--   0        0        0     9005 2023-05-19 23:02:13.000000 semantic_kernel-0.3.4.dev0/semantic_kernel/orchestration/delegate_inference.py
+-rw-r--r--   0        0        0      638 2023-04-13 23:12:46.000000 semantic_kernel-0.3.4.dev0/semantic_kernel/orchestration/delegate_types.py
+-rw-r--r--   0        0        0     7514 2023-04-14 00:52:05.000000 semantic_kernel-0.3.4.dev0/semantic_kernel/orchestration/sk_context.py
+-rw-r--r--   0        0        0    16088 2023-07-06 22:13:35.000000 semantic_kernel-0.3.4.dev0/semantic_kernel/orchestration/sk_function.py
+-rw-r--r--   0        0        0     6158 2023-04-30 18:57:02.000000 semantic_kernel-0.3.4.dev0/semantic_kernel/orchestration/sk_function_base.py
+-rw-r--r--   0        0        0      158 2023-05-08 23:38:10.000000 semantic_kernel-0.3.4.dev0/semantic_kernel/planning/__init__.py
+-rw-r--r--   0        0        0     7538 2023-07-06 22:13:35.000000 semantic_kernel-0.3.4.dev0/semantic_kernel/planning/basic_planner.py
+-rw-r--r--   0        0        0    15624 2023-07-16 00:59:27.696327 semantic_kernel-0.3.4.dev0/semantic_kernel/planning/plan.py
+-rw-r--r--   0        0        0      932 2023-05-19 23:02:13.000000 semantic_kernel-0.3.4.dev0/semantic_kernel/reliability/pass_through_without_retry.py
+-rw-r--r--   0        0        0      694 2023-06-05 21:39:19.000000 semantic_kernel-0.3.4.dev0/semantic_kernel/reliability/retry_mechanism_base.py
+-rw-r--r--   0        0        0     2101 2023-04-13 23:12:46.000000 semantic_kernel-0.3.4.dev0/semantic_kernel/semantic_functions/chat_prompt_template.py
+-rw-r--r--   0        0        0     2332 2023-04-14 00:51:57.000000 semantic_kernel-0.3.4.dev0/semantic_kernel/semantic_functions/prompt_template.py
+-rw-r--r--   0        0        0      506 2023-04-13 23:12:46.000000 semantic_kernel-0.3.4.dev0/semantic_kernel/semantic_functions/prompt_template_base.py
+-rw-r--r--   0        0        0     4525 2023-06-12 17:06:53.000000 semantic_kernel-0.3.4.dev0/semantic_kernel/semantic_functions/prompt_template_config.py
+-rw-r--r--   0        0        0      671 2023-04-14 00:51:57.000000 semantic_kernel-0.3.4.dev0/semantic_kernel/semantic_functions/semantic_function_config.py
+-rw-r--r--   0        0        0      322 2023-04-14 00:51:57.000000 semantic_kernel-0.3.4.dev0/semantic_kernel/skill_definition/__init__.py
+-rw-r--r--   0        0        0     2053 2023-04-14 00:51:57.000000 semantic_kernel-0.3.4.dev0/semantic_kernel/skill_definition/function_view.py
+-rw-r--r--   0        0        0     2199 2023-06-12 17:06:53.000000 semantic_kernel-0.3.4.dev0/semantic_kernel/skill_definition/functions_view.py
+-rw-r--r--   0        0        0     1026 2023-04-14 00:51:57.000000 semantic_kernel-0.3.4.dev0/semantic_kernel/skill_definition/parameter_view.py
+-rw-r--r--   0        0        0     2104 2023-04-14 00:51:57.000000 semantic_kernel-0.3.4.dev0/semantic_kernel/skill_definition/read_only_skill_collection.py
+-rw-r--r--   0        0        0     1345 2023-04-14 00:51:57.000000 semantic_kernel-0.3.4.dev0/semantic_kernel/skill_definition/read_only_skill_collection_base.py
+-rw-r--r--   0        0        0      858 2023-04-13 23:12:46.000000 semantic_kernel-0.3.4.dev0/semantic_kernel/skill_definition/sk_function_context_parameter_decorator.py
+-rw-r--r--   0        0        0      837 2023-04-14 00:51:57.000000 semantic_kernel-0.3.4.dev0/semantic_kernel/skill_definition/sk_function_decorator.py
+-rw-r--r--   0        0        0     6056 2023-04-14 00:51:57.000000 semantic_kernel-0.3.4.dev0/semantic_kernel/skill_definition/skill_collection.py
+-rw-r--r--   0        0        0      803 2023-04-13 23:12:46.000000 semantic_kernel-0.3.4.dev0/semantic_kernel/skill_definition/skill_collection_base.py
+-rw-r--r--   0        0        0     1115 2023-04-13 23:12:46.000000 semantic_kernel-0.3.4.dev0/semantic_kernel/template_engine/README.md
+-rw-r--r--   0        0        0      830 2023-04-14 00:51:57.000000 semantic_kernel-0.3.4.dev0/semantic_kernel/template_engine/blocks/block.py
+-rw-r--r--   0        0        0      228 2023-04-14 00:51:57.000000 semantic_kernel-0.3.4.dev0/semantic_kernel/template_engine/blocks/block_types.py
+-rw-r--r--   0        0        0     4577 2023-04-30 18:57:03.000000 semantic_kernel-0.3.4.dev0/semantic_kernel/template_engine/blocks/code_block.py
+-rw-r--r--   0        0        0     2653 2023-04-13 23:12:46.000000 semantic_kernel-0.3.4.dev0/semantic_kernel/template_engine/blocks/function_id_block.py
+-rw-r--r--   0        0        0      276 2023-04-13 23:12:46.000000 semantic_kernel-0.3.4.dev0/semantic_kernel/template_engine/blocks/symbols.py
+-rw-r--r--   0        0        0     1534 2023-04-14 00:51:57.000000 semantic_kernel-0.3.4.dev0/semantic_kernel/template_engine/blocks/text_block.py
+-rw-r--r--   0        0        0     2274 2023-04-13 23:12:46.000000 semantic_kernel-0.3.4.dev0/semantic_kernel/template_engine/blocks/val_block.py
+-rw-r--r--   0        0        0     2517 2023-04-14 00:51:57.000000 semantic_kernel-0.3.4.dev0/semantic_kernel/template_engine/blocks/var_block.py
+-rw-r--r--   0        0        0     6535 2023-04-13 23:12:46.000000 semantic_kernel-0.3.4.dev0/semantic_kernel/template_engine/code_tokenizer.py
+-rw-r--r--   0        0        0     6051 2023-04-14 00:51:57.000000 semantic_kernel-0.3.4.dev0/semantic_kernel/template_engine/prompt_template_engine.py
+-rw-r--r--   0        0        0      532 2023-04-13 23:12:46.000000 semantic_kernel-0.3.4.dev0/semantic_kernel/template_engine/protocols/code_renderer.py
+-rw-r--r--   0        0        0     3043 2023-04-13 23:12:46.000000 semantic_kernel-0.3.4.dev0/semantic_kernel/template_engine/protocols/prompt_templating_engine.py
+-rw-r--r--   0        0        0      596 2023-04-13 23:12:46.000000 semantic_kernel-0.3.4.dev0/semantic_kernel/template_engine/protocols/text_renderer.py
+-rw-r--r--   0        0        0     7637 2023-04-13 23:12:46.000000 semantic_kernel-0.3.4.dev0/semantic_kernel/template_engine/template_tokenizer.py
+-rw-r--r--   0        0        0      473 2023-04-30 18:57:03.000000 semantic_kernel-0.3.4.dev0/semantic_kernel/text/__init__.py
+-rw-r--r--   0        0        0      667 2023-04-30 18:57:03.000000 semantic_kernel-0.3.4.dev0/semantic_kernel/text/function_extension.py
+-rw-r--r--   0        0        0     8568 2023-07-16 00:58:38.006510 semantic_kernel-0.3.4.dev0/semantic_kernel/text/text_chunker.py
+-rw-r--r--   0        0        0      403 2023-04-13 23:12:46.000000 semantic_kernel-0.3.4.dev0/semantic_kernel/utils/null_logger.py
+-rw-r--r--   0        0        0     2694 2023-07-12 19:14:40.915313 semantic_kernel-0.3.4.dev0/semantic_kernel/utils/settings.py
+-rw-r--r--   0        0        0      221 2023-04-13 23:12:46.000000 semantic_kernel-0.3.4.dev0/semantic_kernel/utils/static_property.py
+-rw-r--r--   0        0        0     2198 2023-04-13 23:12:46.000000 semantic_kernel-0.3.4.dev0/semantic_kernel/utils/validation.py
+-rw-r--r--   0        0        0     1843 1970-01-01 00:00:00.000000 semantic_kernel-0.3.4.dev0/PKG-INFO
```

### Comparing `semantic_kernel-0.3.3.dev0/pip/README.md` & `semantic_kernel-0.3.4.dev0/pip/README.md`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.3.dev0/pyproject.toml` & `semantic_kernel-0.3.4.dev0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "semantic-kernel"
-version = "0.3.3.dev"
+version = "0.3.4.dev"
 description = ""
 authors = ["Microsoft <SK-Support@microsoft.com>"]
 readme = "pip/README.md"
 packages = [{include = "semantic_kernel"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
@@ -15,37 +15,41 @@
 regex = "^2023.6.3"
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "3.3.3"
 black = {version = "23.3.0", allow-prereleases = true}
 ipykernel = "^6.21.1"
 pytest = "7.4.0"
-ruff = "0.0.277"
+ruff = "0.0.278"
 pytest-asyncio = "0.21.0"
 
 [tool.poetry.group.hugging_face.dependencies]
 transformers = "^4.28.1"
 sentence-transformers = "^2.2.2"
 torch = "2.0.0"
 
 [tool.poetry.group.chromadb.dependencies]
-chromadb = "^0.3.29"
+chromadb = "^0.4.0"
+
+[tool.poetry.group.milvus.dependencies]
+pymilvus = "^2.2.11"
+milvus = "^2.2.11"
 
 [tool.poetry.group.weaviate.dependencies]
 weaviate-client = "^3.18.0"
 
 [tool.poetry.group.pinecone.dependencies]
 pinecone-client = "^2.2.2"
 
 [tool.poetry.group.postgres.dependencies]
 psycopg-pool = "^3.1.7"
 psycopg = "^3.1.9"
 psycopg-binary = "^3.1.9"
 
-[tool.poetry.group.azure_search.dependencies]
+[tool.poetry.group.azure_cognitive_search.dependencies]
 azure-search-documents = {version = "11.4.0b6", allow-prereleases = true}
 azure-core = "^1.28.0"
 azure-identity = "^1.13.0"
 
 [tool.isort]
 profile = "black"
```

### Comparing `semantic_kernel-0.3.3.dev0/semantic_kernel/__init__.py` & `semantic_kernel-0.3.4.dev0/semantic_kernel/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.3.dev0/semantic_kernel/connectors/ai/__init__.py` & `semantic_kernel-0.3.4.dev0/semantic_kernel/connectors/ai/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.3.dev0/semantic_kernel/connectors/ai/ai_exception.py` & `semantic_kernel-0.3.4.dev0/semantic_kernel/connectors/ai/ai_exception.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.3.dev0/semantic_kernel/connectors/ai/chat_completion_client_base.py` & `semantic_kernel-0.3.4.dev0/semantic_kernel/connectors/ai/chat_completion_client_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.3.dev0/semantic_kernel/connectors/ai/chat_request_settings.py` & `semantic_kernel-0.3.4.dev0/semantic_kernel/connectors/ai/chat_request_settings.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.3.dev0/semantic_kernel/connectors/ai/complete_request_settings.py` & `semantic_kernel-0.3.4.dev0/semantic_kernel/connectors/ai/complete_request_settings.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.3.dev0/semantic_kernel/connectors/ai/hugging_face/services/hf_text_completion.py` & `semantic_kernel-0.3.4.dev0/semantic_kernel/connectors/ai/hugging_face/services/hf_text_completion.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.3.dev0/semantic_kernel/connectors/ai/hugging_face/services/hf_text_embedding.py` & `semantic_kernel-0.3.4.dev0/semantic_kernel/connectors/ai/hugging_face/services/hf_text_embedding.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.3.dev0/semantic_kernel/connectors/ai/open_ai/__init__.py` & `semantic_kernel-0.3.4.dev0/semantic_kernel/connectors/ai/open_ai/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.3.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_chat_completion.py` & `semantic_kernel-0.3.4.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_chat_completion.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.3.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_text_completion.py` & `semantic_kernel-0.3.4.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_text_completion.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.3.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_text_embedding.py` & `semantic_kernel-0.3.4.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_text_embedding.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.3.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_chat_completion.py` & `semantic_kernel-0.3.4.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_chat_completion.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.3.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_completion.py` & `semantic_kernel-0.3.4.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_completion.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.3.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_embedding.py` & `semantic_kernel-0.3.4.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_embedding.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.3.dev0/semantic_kernel/connectors/ai/text_completion_client_base.py` & `semantic_kernel-0.3.4.dev0/semantic_kernel/connectors/ai/text_completion_client_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.3.dev0/semantic_kernel/connectors/memory/azure_search/azure_search_memory_store.py` & `semantic_kernel-0.3.4.dev0/semantic_kernel/connectors/memory/azure_cognitive_search/azure_cognitive_search_memory_store.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,89 +1,85 @@
 # Copyright (c) Microsoft. All rights reserved.
 
-import asyncio
 import uuid
 from logging import Logger
 from typing import List, Optional, Tuple
 
 from azure.core.credentials import AzureKeyCredential, TokenCredential
 from azure.core.exceptions import ResourceNotFoundError
 from azure.search.documents.indexes.aio import SearchIndexClient
 from azure.search.documents.indexes.models import (
     SearchIndex,
     VectorSearch,
     VectorSearchAlgorithmConfiguration,
 )
 from numpy import ndarray
 
-from semantic_kernel.connectors.memory.azure_search.utils import (
+from semantic_kernel.connectors.memory.azure_cognitive_search.utils import (
     SEARCH_FIELD_EMBEDDING,
     SEARCH_FIELD_ID,
     dict_to_memory_record,
     encode_id,
     get_field_selection,
     get_index_schema,
     get_search_index_async_client,
     memory_record_to_search_record,
 )
 from semantic_kernel.memory.memory_record import MemoryRecord
 from semantic_kernel.memory.memory_store_base import MemoryStoreBase
 from semantic_kernel.utils.null_logger import NullLogger
 
 
-class AzureSearchMemoryStore(MemoryStoreBase):
+class AzureCognitiveSearchMemoryStore(MemoryStoreBase):
     _search_index_client: SearchIndexClient = None
     _vector_size: int = None
     _logger: Logger = None
 
     def __init__(
         self,
         vector_size: int,
         search_endpoint: Optional[str] = None,
         admin_key: Optional[str] = None,
         azure_credentials: Optional[AzureKeyCredential] = None,
         token_credentials: Optional[TokenCredential] = None,
         logger: Optional[Logger] = None,
     ) -> None:
-        """Initializes a new instance of the AzureSearchMemoryStore class.
+        """Initializes a new instance of the AzureCognitiveSearchMemoryStore class.
 
         Arguments:
             vector_size {int}                                -- Embedding vector size.
-            search_endpoint {Optional[str]}                  -- The endpoint of the Azure Search service
+            search_endpoint {Optional[str]}                  -- The endpoint of the Azure Cognitive Search service
                                                                 (default: {None}).
-            admin_key {Optional[str]}                        -- Azure Search API key (default: {None}).
-            azure_credentials {Optional[AzureKeyCredential]} -- Azure Search credentials (default: {None}).
-            token_credentials {Optional[TokenCredential]}    -- Azure Search token credentials
+            admin_key {Optional[str]}                        -- Azure Cognitive Search API key (default: {None}).
+            azure_credentials {Optional[AzureKeyCredential]} -- Azure Cognitive Search credentials (default: {None}).
+            token_credentials {Optional[TokenCredential]}    -- Azure Cognitive Search token credentials
                                                                 (default: {None}).
             logger {Optional[Logger]}                        -- The logger to use (default: {None}).
+
+        Instantiate using Async Context Manager:
+            async with AzureCognitiveSearchMemoryStore(<...>) as memory:
+                await memory.<...>
+
         """
         try:
             pass
         except ImportError:
             raise ValueError(
-                "Error: Unable to import Azure Search client python package. Please install Azure Search client"
+                "Error: Unable to import Azure Cognitive Search client python package."
+                "Please install Azure Cognitive Search client"
             )
 
         self._logger = logger or NullLogger()
         self._vector_size = vector_size
         self._search_index_client = get_search_index_async_client(
             search_endpoint, admin_key, azure_credentials, token_credentials
         )
 
-    def __del__(self):
-        try:
-            loop = asyncio.get_event_loop()
-            if loop.is_running():
-                loop.create_task(self.close())
-            else:
-                loop.run_until_complete(self.close())
-        except Exception:
-            pass
-
-    async def close(self):
+    async def close_async(self):
+        """Async close connection, invoked by MemoryStoreBase.__aexit__()"""
         if self._search_index_client is not None:
             await self._search_index_client.close()
 
     async def create_collection_async(
         self,
         collection_name: str,
         vector_config: Optional[VectorSearchAlgorithmConfiguration] = None,
@@ -149,38 +145,26 @@
     async def get_collections_async(self) -> List[str]:
         """Gets the list of collections.
 
         Returns:
             List[str] -- The list of collections.
         """
 
-        results_list = list(str)
-        items = self._search_index_client.list_index_names()
+        results_list = []
+        try:
+            items = await self._search_index_client.list_index_names()
+        except TypeError:
+            # Note: used on Windows
+            items = self._search_index_client.list_index_names()
 
-        for result in items:
+        async for result in items:
             results_list.append(result)
 
         return results_list
 
-    async def get_collection_async(self, collection_name: str) -> SearchIndex:
-        """Gets the a collections based upon collection name.
-
-        Arguments:
-            collection_name {str} -- Name of the collection.
-
-        Returns:
-            SearchIndex -- Collection Information.
-        """
-
-        collection_result = await self._search_index_client.get_index(
-            name=collection_name.lower()
-        )
-
-        return collection_result
-
     async def delete_collection_async(self, collection_name: str) -> None:
         """Deletes a collection.
 
         Arguments:
             collection_name {str} -- The name of the collection to delete.
 
         Returns:
@@ -217,35 +201,18 @@
             collection_name {str} -- The name of the collection to upsert the record into.
             record {MemoryRecord} -- The record to upsert.
 
         Returns:
             str -- The unique record id of the record.
         """
 
-        # Look up Search client class to see if exists or create
-        azure_search_client = self._search_index_client.get_search_client(
-            collection_name.lower()
-        )
-
-        # Note:
-        # * Document id     = user provided value
-        # * MemoryRecord.id = base64(Document id)
-        if not record._id:
-            record._id = str(uuid.uuid4())
-
-        search_record = memory_record_to_search_record(record)
-
-        result = await azure_search_client.upload_documents(documents=[search_record])
-
-        # Throw exception if problem
-        # Clean this up not needed if throwing
-        if result[0].succeeded:
-            return record._id
-        else:
-            raise ValueError("Error: Unable to upsert record.")
+        result = await self.upsert_batch_async(collection_name, [record])
+        if result:
+            return result[0]
+        return None
 
     async def upsert_batch_async(
         self, collection_name: str, records: List[MemoryRecord]
     ) -> List[str]:
         """Upsert a batch of records.
 
         Arguments:
@@ -254,15 +221,15 @@
 
         Returns:
             List[str] -- The unique database keys of the records.
         """
 
         # Initialize search client here
         # Look up Search client class to see if exists or create
-        azure_search_client = self._search_index_client.get_search_client(
+        search_client = self._search_index_client.get_search_client(
             collection_name.lower()
         )
 
         search_records = []
         search_ids = []
 
         for record in records:
@@ -272,15 +239,16 @@
             if not record._id:
                 record._id = str(uuid.uuid4())
 
             search_record = memory_record_to_search_record(record)
             search_records.append(search_record)
             search_ids.append(record._id)
 
-        result = azure_search_client.upload_documents(documents=search_records)
+        result = await search_client.upload_documents(documents=search_records)
+        await search_client.close()
 
         if result[0].succeeded:
             return search_ids
         else:
             return None
 
     async def get_async(
@@ -303,16 +271,19 @@
         )
 
         try:
             search_result = await search_client.get_document(
                 key=encode_id(key), selected_fields=get_field_selection(with_embedding)
             )
         except ResourceNotFoundError:
+            await search_client.close()
             raise KeyError("Memory record not found")
 
+        await search_client.close()
+
         # Create Memory record from document
         return dict_to_memory_record(search_result, with_embedding)
 
     async def get_batch_async(
         self, collection_name: str, keys: List[str], with_embeddings: bool = False
     ) -> List[MemoryRecord]:
         """Gets a batch of records.
@@ -368,14 +339,15 @@
         # Look up Search client class to see if exists or create
         search_client = self._search_index_client.get_search_client(
             collection_name.lower()
         )
         docs_to_delete = {SEARCH_FIELD_ID: encode_id(key)}
 
         await search_client.delete_documents(documents=[docs_to_delete])
+        await search_client.close()
 
     async def get_nearest_match_async(
         self,
         collection_name: str,
         embedding: ndarray,
         min_relevance_score: float = 0.0,
         with_embedding: bool = False,
@@ -436,19 +408,21 @@
             vector_fields=SEARCH_FIELD_EMBEDDING,
             vector=embedding.tolist(),
             select=get_field_selection(with_embeddings),
             top_k=limit,
         )
 
         if not search_results or search_results is None:
+            await search_client.close()
             return []
 
         # Convert the results to MemoryRecords
         nearest_results = []
         async for search_record in search_results:
             if search_record["@search.score"] < min_relevance_score:
                 continue
 
             memory_record = dict_to_memory_record(search_record, with_embeddings)
             nearest_results.append((memory_record, search_record["@search.score"]))
 
+        await search_client.close()
         return nearest_results
```

### Comparing `semantic_kernel-0.3.3.dev0/semantic_kernel/connectors/memory/azure_search/utils.py` & `semantic_kernel-0.3.4.dev0/semantic_kernel/connectors/memory/azure_cognitive_search/utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -26,92 +26,93 @@
 
 def get_search_index_async_client(
     search_endpoint: Optional[str] = None,
     admin_key: Optional[str] = None,
     azure_credential: Optional[AzureKeyCredential] = None,
     token_credential: Optional[TokenCredential] = None,
 ):
-    """Return a client for Azure Search.
+    """Return a client for Azure Cognitive Search.
 
     Arguments:
         search_endpoint {str}                 -- Optional endpoint (default: {None}).
         admin_key {str}                       -- Optional API key (default: {None}).
         azure_credential {AzureKeyCredential} -- Optional Azure credentials (default: {None}).
         token_credential {TokenCredential}    -- Optional Token credential (default: {None}).
     """
 
-    ENV_VAR_ENDPOINT = "AZURE_SEARCH_ENDPOINT"
-    ENV_VAR_API_KEY = "AZURE_SEARCH_ADMIN_KEY"
+    ENV_VAR_ENDPOINT = "AZURE_COGNITIVE_SEARCH_ENDPOINT"
+    ENV_VAR_API_KEY = "AZURE_COGNITIVE_SEARCH_ADMIN_KEY"
 
     try:
         # Note: there are two client classes available:
         # 1. Async: azure.search.documents.indexes.aio.SearchIndexClient
         # 2. Sync: azure.search.documents.indexes.SearchIndexClient
         from azure.search.documents.indexes.aio import SearchIndexClient
     except ImportError:
         raise ValueError(
-            "Error: Unable to import Azure Search client python package. Please install Azure Search client"
+            "Error: Unable to import Azure Cognitive Search client python package."
+            "Please install Azure Cognitive Search client"
         )
 
     azure_credential: AzureKeyCredential = None
     token_credential: TokenCredential = None
 
     # Load environment variables
     load_dotenv()
 
     # Service endpoint
     if search_endpoint:
         service_endpoint = search_endpoint
     elif os.getenv(ENV_VAR_ENDPOINT):
         service_endpoint = os.getenv(ENV_VAR_ENDPOINT)
     else:
-        raise ValueError("Error: missing Azure Search client endpoint.")
+        raise ValueError("Error: missing Azure Cognitive Search client endpoint.")
 
     if service_endpoint is None:
         print(service_endpoint)
-        raise ValueError("Error: Azure Search client not set.")
+        raise ValueError("Error: Azure Cognitive Search client not set.")
 
     # Credentials
     if admin_key:
         azure_credential = AzureKeyCredential(admin_key)
     elif azure_credential:
         azure_credential = azure_credential
     elif token_credential:
         token_credential = token_credential
     elif os.getenv(ENV_VAR_API_KEY):
         azure_credential = AzureKeyCredential(os.getenv(ENV_VAR_API_KEY))
     else:
-        raise ValueError("Error: missing Azure Search client credentials.")
+        raise ValueError("Error: missing Azure Cognitive Search client credentials.")
 
     if azure_credential is None and token_credential is None:
-        raise ValueError("Error: Azure Search credentials not set.")
+        raise ValueError("Error: Azure Cognitive Search credentials not set.")
 
     sk_headers = {"User-Agent": "Semantic-Kernel"}
 
     if azure_credential:
         return SearchIndexClient(
             endpoint=service_endpoint, credential=azure_credential, headers=sk_headers
         )
 
     if token_credential:
         return SearchIndexClient(
             endpoint=service_endpoint, credential=token_credential, headers=sk_headers
         )
 
-    raise ValueError("Error: unable to create Azure Search client.")
+    raise ValueError("Error: unable to create Azure Cognitive Search client.")
 
 
 def get_index_schema(vector_size: int) -> list:
     """Return the schema of search indexes.
 
     Arguments:
         vector_size {int} -- The size of the vectors being stored in collection/index.
 
     Returns:
-        list -- The Azure Search schema as list type.
+        list -- The Azure Cognitive Search schema as list type.
     """
 
     search_fields = [
         SimpleField(
             name=SEARCH_FIELD_ID,
             type=SearchFieldDataType.String,
             searchable=True,
@@ -191,18 +192,18 @@
     return field_selection
 
 
 def dict_to_memory_record(data: dict, with_embeddings: bool) -> MemoryRecord:
     """Converts a search result to a MemoryRecord.
 
     Arguments:
-        data {dict} -- Azure Search result data.
+        data {dict} -- Azure Cognitive Search result data.
 
     Returns:
-        MemoryRecord -- The MemoryRecord from Azure Search Data Result.
+        MemoryRecord -- The MemoryRecord from Azure Cognitive Search Data Result.
     """
 
     sk_result = MemoryRecord(
         id=decode_id(data[SEARCH_FIELD_ID]),
         key=data[SEARCH_FIELD_ID],
         text=data[SEARCH_FIELD_TEXT],
         external_source_name=data[SEARCH_FIELD_SRC],
@@ -215,15 +216,15 @@
     return sk_result
 
 
 def memory_record_to_search_record(record: MemoryRecord) -> dict:
     """Convert a MemoryRecord to a dictionary
 
     Arguments:
-        record {MemoryRecord} -- The MemoryRecord from Azure Search Data Result.
+        record {MemoryRecord} -- The MemoryRecord from Azure Cognitive Search Data Result.
 
     Returns:
         data {dict} -- Dictionary data.
     """
 
     return {
         SEARCH_FIELD_ID: encode_id(record._id),
@@ -233,28 +234,28 @@
         SEARCH_FIELD_METADATA: record._additional_metadata or "",
         SEARCH_FIELD_IS_REF: str(record._is_reference),
         SEARCH_FIELD_EMBEDDING: record._embedding.tolist(),
     }
 
 
 def encode_id(id: str) -> str:
-    """Encode a record id to ensure compatibility with Azure search.
+    """Encode a record id to ensure compatibility with Azure Cognitive Search.
 
-    Azure Search keys can contain only letters, digits, underscore, dash, equal sign,
-    recommending to encode values with a URL-safe algorithm.
+    Azure Cognitive Search keys can contain only letters, digits, underscore, dash,
+    equal sign, recommending to encode values with a URL-safe algorithm.
     """
 
     id_bytes = id.encode("ascii")
     base64_bytes = base64.b64encode(id_bytes)
     return base64_bytes.decode("ascii")
 
 
 def decode_id(base64_id: str) -> str:
     """Decode a record id to the original value.
 
-    Azure Search keys can contain only letters, digits, underscore, dash, equal sign,
-    recommending to encode values with a URL-safe algorithm.
+    Azure Cognitive Search keys can contain only letters, digits, underscore, dash,
+    equal sign, recommending to encode values with a URL-safe algorithm.
     """
 
     base64_bytes = base64_id.encode("ascii")
     message_bytes = base64.b64decode(base64_bytes)
     return message_bytes.decode("ascii")
```

### Comparing `semantic_kernel-0.3.3.dev0/semantic_kernel/connectors/memory/chroma/chroma_memory_store.py` & `semantic_kernel-0.3.4.dev0/semantic_kernel/connectors/memory/chroma/chroma_memory_store.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 
         if client_settings:
             self._client_settings = client_settings
         else:
             self._client_settings = chromadb.config.Settings()
             if persist_directory is not None:
                 self._client_settings = chromadb.config.Settings(
-                    chroma_db_impl="duckdb+parquet", persist_directory=persist_directory
+                    is_persistent=True, persist_directory=persist_directory
                 )
         self._client = chromadb.Client(self._client_settings)
         self._persist_directory = persist_directory
         self._default_query_includes = ["embeddings", "metadatas", "documents"]
 
         self._logger = logger or NullLogger()
         self._default_embedding_function = "DisableChromaEmbeddingFunction"
```

### Comparing `semantic_kernel-0.3.3.dev0/semantic_kernel/connectors/memory/chroma/utils.py` & `semantic_kernel-0.3.4.dev0/semantic_kernel/connectors/memory/chroma/utils.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.3.dev0/semantic_kernel/connectors/memory/pinecone/pinecone_memory_store.py` & `semantic_kernel-0.3.4.dev0/semantic_kernel/connectors/memory/pinecone/pinecone_memory_store.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.3.dev0/semantic_kernel/connectors/memory/pinecone/utils.py` & `semantic_kernel-0.3.4.dev0/semantic_kernel/connectors/memory/pinecone/utils.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.3.dev0/semantic_kernel/connectors/memory/postgres/postgres_memory_store.py` & `semantic_kernel-0.3.4.dev0/semantic_kernel/connectors/memory/postgres/postgres_memory_store.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.3.dev0/semantic_kernel/connectors/memory/weaviate/weaviate_memory_store.py` & `semantic_kernel-0.3.4.dev0/semantic_kernel/connectors/memory/weaviate/weaviate_memory_store.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.3.dev0/semantic_kernel/connectors/search_engine/bing_connector.py` & `semantic_kernel-0.3.4.dev0/semantic_kernel/connectors/search_engine/bing_connector.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.3.dev0/semantic_kernel/core_skills/__init__.py` & `semantic_kernel-0.3.4.dev0/semantic_kernel/core_skills/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.3.dev0/semantic_kernel/core_skills/conversation_summary_skill.py` & `semantic_kernel-0.3.4.dev0/semantic_kernel/core_skills/conversation_summary_skill.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.3.dev0/semantic_kernel/core_skills/file_io_skill.py` & `semantic_kernel-0.3.4.dev0/semantic_kernel/core_skills/file_io_skill.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.3.dev0/semantic_kernel/core_skills/http_skill.py` & `semantic_kernel-0.3.4.dev0/semantic_kernel/core_skills/http_skill.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.3.dev0/semantic_kernel/core_skills/math_skill.py` & `semantic_kernel-0.3.4.dev0/semantic_kernel/core_skills/math_skill.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.3.dev0/semantic_kernel/core_skills/text_memory_skill.py` & `semantic_kernel-0.3.4.dev0/semantic_kernel/core_skills/text_memory_skill.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.3.dev0/semantic_kernel/core_skills/text_skill.py` & `semantic_kernel-0.3.4.dev0/semantic_kernel/core_skills/text_skill.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.3.dev0/semantic_kernel/core_skills/time_skill.py` & `semantic_kernel-0.3.4.dev0/semantic_kernel/core_skills/time_skill.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.3.dev0/semantic_kernel/core_skills/wait_skill.py` & `semantic_kernel-0.3.4.dev0/semantic_kernel/core_skills/wait_skill.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.3.dev0/semantic_kernel/core_skills/web_search_engine_skill.py` & `semantic_kernel-0.3.4.dev0/semantic_kernel/core_skills/web_search_engine_skill.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.3.dev0/semantic_kernel/kernel.py` & `semantic_kernel-0.3.4.dev0/semantic_kernel/kernel.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.3.dev0/semantic_kernel/kernel_exception.py` & `semantic_kernel-0.3.4.dev0/semantic_kernel/kernel_exception.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.3.dev0/semantic_kernel/memory/memory_query_result.py` & `semantic_kernel-0.3.4.dev0/semantic_kernel/memory/memory_query_result.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.3.dev0/semantic_kernel/memory/memory_record.py` & `semantic_kernel-0.3.4.dev0/semantic_kernel/memory/memory_record.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.3.dev0/semantic_kernel/memory/memory_store_base.py` & `semantic_kernel-0.3.4.dev0/semantic_kernel/memory/memory_store_base.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,23 @@
 
 from numpy import ndarray
 
 from semantic_kernel.memory.memory_record import MemoryRecord
 
 
 class MemoryStoreBase(ABC):
+    async def __aenter__(self):
+        return self
+
+    async def __aexit__(self, *args):
+        await self.close_async()
+
+    async def close_async(self):
+        pass
+
     @abstractmethod
     async def create_collection_async(self, collection_name: str) -> None:
         pass
 
     @abstractmethod
     async def get_collections_async(
         self,
```

### Comparing `semantic_kernel-0.3.3.dev0/semantic_kernel/memory/null_memory.py` & `semantic_kernel-0.3.4.dev0/semantic_kernel/memory/null_memory.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.3.dev0/semantic_kernel/memory/semantic_text_memory.py` & `semantic_kernel-0.3.4.dev0/semantic_kernel/memory/semantic_text_memory.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.3.dev0/semantic_kernel/memory/semantic_text_memory_base.py` & `semantic_kernel-0.3.4.dev0/semantic_kernel/memory/semantic_text_memory_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.3.dev0/semantic_kernel/memory/volatile_memory_store.py` & `semantic_kernel-0.3.4.dev0/semantic_kernel/memory/volatile_memory_store.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.3.dev0/semantic_kernel/orchestration/context_variables.py` & `semantic_kernel-0.3.4.dev0/semantic_kernel/orchestration/context_variables.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.3.dev0/semantic_kernel/orchestration/delegate_handlers.py` & `semantic_kernel-0.3.4.dev0/semantic_kernel/orchestration/delegate_handlers.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.3.dev0/semantic_kernel/orchestration/delegate_inference.py` & `semantic_kernel-0.3.4.dev0/semantic_kernel/orchestration/delegate_inference.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.3.dev0/semantic_kernel/orchestration/delegate_types.py` & `semantic_kernel-0.3.4.dev0/semantic_kernel/orchestration/delegate_types.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.3.dev0/semantic_kernel/orchestration/sk_context.py` & `semantic_kernel-0.3.4.dev0/semantic_kernel/orchestration/sk_context.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.3.dev0/semantic_kernel/orchestration/sk_function.py` & `semantic_kernel-0.3.4.dev0/semantic_kernel/orchestration/sk_function.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.3.dev0/semantic_kernel/orchestration/sk_function_base.py` & `semantic_kernel-0.3.4.dev0/semantic_kernel/orchestration/sk_function_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.3.dev0/semantic_kernel/planning/basic_planner.py` & `semantic_kernel-0.3.4.dev0/semantic_kernel/planning/basic_planner.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.3.dev0/semantic_kernel/planning/plan.py` & `semantic_kernel-0.3.4.dev0/semantic_kernel/planning/plan.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.3.dev0/semantic_kernel/reliability/pass_through_without_retry.py` & `semantic_kernel-0.3.4.dev0/semantic_kernel/reliability/pass_through_without_retry.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.3.dev0/semantic_kernel/reliability/retry_mechanism_base.py` & `semantic_kernel-0.3.4.dev0/semantic_kernel/reliability/retry_mechanism_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.3.dev0/semantic_kernel/semantic_functions/chat_prompt_template.py` & `semantic_kernel-0.3.4.dev0/semantic_kernel/semantic_functions/chat_prompt_template.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.3.dev0/semantic_kernel/semantic_functions/prompt_template.py` & `semantic_kernel-0.3.4.dev0/semantic_kernel/semantic_functions/prompt_template.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.3.dev0/semantic_kernel/semantic_functions/prompt_template_config.py` & `semantic_kernel-0.3.4.dev0/semantic_kernel/semantic_functions/prompt_template_config.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.3.dev0/semantic_kernel/semantic_functions/semantic_function_config.py` & `semantic_kernel-0.3.4.dev0/semantic_kernel/semantic_functions/semantic_function_config.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.3.dev0/semantic_kernel/skill_definition/function_view.py` & `semantic_kernel-0.3.4.dev0/semantic_kernel/skill_definition/function_view.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.3.dev0/semantic_kernel/skill_definition/functions_view.py` & `semantic_kernel-0.3.4.dev0/semantic_kernel/skill_definition/functions_view.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.3.dev0/semantic_kernel/skill_definition/parameter_view.py` & `semantic_kernel-0.3.4.dev0/semantic_kernel/skill_definition/parameter_view.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.3.dev0/semantic_kernel/skill_definition/read_only_skill_collection.py` & `semantic_kernel-0.3.4.dev0/semantic_kernel/skill_definition/read_only_skill_collection.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.3.dev0/semantic_kernel/skill_definition/read_only_skill_collection_base.py` & `semantic_kernel-0.3.4.dev0/semantic_kernel/skill_definition/read_only_skill_collection_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.3.dev0/semantic_kernel/skill_definition/sk_function_context_parameter_decorator.py` & `semantic_kernel-0.3.4.dev0/semantic_kernel/skill_definition/sk_function_context_parameter_decorator.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.3.dev0/semantic_kernel/skill_definition/sk_function_decorator.py` & `semantic_kernel-0.3.4.dev0/semantic_kernel/skill_definition/sk_function_decorator.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.3.dev0/semantic_kernel/skill_definition/skill_collection.py` & `semantic_kernel-0.3.4.dev0/semantic_kernel/skill_definition/skill_collection.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.3.dev0/semantic_kernel/skill_definition/skill_collection_base.py` & `semantic_kernel-0.3.4.dev0/semantic_kernel/skill_definition/skill_collection_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.3.dev0/semantic_kernel/template_engine/README.md` & `semantic_kernel-0.3.4.dev0/semantic_kernel/template_engine/README.md`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.3.dev0/semantic_kernel/template_engine/blocks/block.py` & `semantic_kernel-0.3.4.dev0/semantic_kernel/template_engine/blocks/block.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.3.dev0/semantic_kernel/template_engine/blocks/code_block.py` & `semantic_kernel-0.3.4.dev0/semantic_kernel/template_engine/blocks/code_block.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.3.dev0/semantic_kernel/template_engine/blocks/function_id_block.py` & `semantic_kernel-0.3.4.dev0/semantic_kernel/template_engine/blocks/function_id_block.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.3.dev0/semantic_kernel/template_engine/blocks/text_block.py` & `semantic_kernel-0.3.4.dev0/semantic_kernel/template_engine/blocks/text_block.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.3.dev0/semantic_kernel/template_engine/blocks/val_block.py` & `semantic_kernel-0.3.4.dev0/semantic_kernel/template_engine/blocks/val_block.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.3.dev0/semantic_kernel/template_engine/blocks/var_block.py` & `semantic_kernel-0.3.4.dev0/semantic_kernel/template_engine/blocks/var_block.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.3.dev0/semantic_kernel/template_engine/code_tokenizer.py` & `semantic_kernel-0.3.4.dev0/semantic_kernel/template_engine/code_tokenizer.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.3.dev0/semantic_kernel/template_engine/prompt_template_engine.py` & `semantic_kernel-0.3.4.dev0/semantic_kernel/template_engine/prompt_template_engine.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.3.dev0/semantic_kernel/template_engine/protocols/code_renderer.py` & `semantic_kernel-0.3.4.dev0/semantic_kernel/template_engine/protocols/code_renderer.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.3.dev0/semantic_kernel/template_engine/protocols/prompt_templating_engine.py` & `semantic_kernel-0.3.4.dev0/semantic_kernel/template_engine/protocols/prompt_templating_engine.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.3.dev0/semantic_kernel/template_engine/protocols/text_renderer.py` & `semantic_kernel-0.3.4.dev0/semantic_kernel/template_engine/protocols/text_renderer.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.3.dev0/semantic_kernel/template_engine/template_tokenizer.py` & `semantic_kernel-0.3.4.dev0/semantic_kernel/template_engine/template_tokenizer.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.3.dev0/semantic_kernel/text/function_extension.py` & `semantic_kernel-0.3.4.dev0/semantic_kernel/text/function_extension.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.3.dev0/semantic_kernel/text/text_chunker.py` & `semantic_kernel-0.3.4.dev0/semantic_kernel/text/text_chunker.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.3.dev0/semantic_kernel/utils/settings.py` & `semantic_kernel-0.3.4.dev0/semantic_kernel/utils/settings.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.3.dev0/semantic_kernel/utils/validation.py` & `semantic_kernel-0.3.4.dev0/semantic_kernel/utils/validation.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.3.dev0/PKG-INFO` & `semantic_kernel-0.3.4.dev0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: semantic-kernel
-Version: 0.3.3.dev0
+Version: 0.3.4.dev0
 Summary: 
 Author: Microsoft
 Author-email: SK-Support@microsoft.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

