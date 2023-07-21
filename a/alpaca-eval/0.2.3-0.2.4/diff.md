# Comparing `tmp/alpaca_eval-0.2.3.tar.gz` & `tmp/alpaca_eval-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alpaca_eval-0.2.3.tar", last modified: Sat Jul 15 16:24:00 2023, max compression
+gzip compressed data, was "alpaca_eval-0.2.4.tar", last modified: Fri Jul 21 15:23:03 2023, max compression
```

## Comparing `alpaca_eval-0.2.3.tar` & `alpaca_eval-0.2.4.tar`

### file list

```diff
@@ -1,212 +1,232 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:24:00.434027 alpaca_eval-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11409 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    66635 2023-07-15 16:24:00.434027 alpaca_eval-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    65813 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:24:00.410025 alpaca_eval-0.2.3/example/
--rw-r--r--   0 runner    (1001) docker     (123)   500735 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/example/outputs.json
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 16:24:00.434027 alpaca_eval-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:24:00.402025 alpaca_eval-0.2.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:24:00.414026 alpaca_eval-0.2.3/src/alpaca_eval/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-15 16:23:45.000000 alpaca_eval-0.2.3/src/alpaca_eval/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21377 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/analyze.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:24:00.414026 alpaca_eval-0.2.3/src/alpaca_eval/annotators/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/annotators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25039 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/annotators/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    16402 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/annotators/pairwise_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4834 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/completion_parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:24:00.418026 alpaca_eval-0.2.3/src/alpaca_eval/decoders/
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/decoders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4359 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/decoders/anthropic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/decoders/cohere.py
--rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/decoders/huggingface_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/decoders/huggingface_local.py
--rw-r--r--   0 runner    (1001) docker     (123)    12959 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/decoders/openai.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:24:00.418026 alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/
--rw-r--r--   0 runner    (1001) docker     (123)     9753 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:24:00.418026 alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4/
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4/alpaca_eval.txt
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:24:00.418026 alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4_fn/
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4_fn/alpaca_eval_fn.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4_fn/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:24:00.418026 alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/alpaca_farm/
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_chat_v0_without_inputs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5869 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_chat_without_inputs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_cot_json_without_inputs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_without_inputs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b4_cot_json_without_inputs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6849 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_diana_without_inputs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6797 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_joe_without_inputs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6700 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_without_inputs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6045 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/alpaca_farm/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b1_v0_without_inputs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3969 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b1_without_inputs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5932 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b4_reasoning_without_inputs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5370 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b5_without_inputs.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:24:00.418026 alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/alpaca_farm_greedy_gpt4/
--rw-r--r--   0 runner    (1001) docker     (123)     7373 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/alpaca_farm_greedy_gpt4/chatml_b5_without_inputs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/alpaca_farm_greedy_gpt4/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:24:00.422026 alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/aviary_gpt4/
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/aviary_gpt4/aviary_prompt.txt
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/aviary_gpt4/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:24:00.422026 alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/chatgpt/
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/chatgpt/basic_prompt.txt
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/chatgpt/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:24:00.422026 alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/chatgpt_fn/
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/chatgpt_fn/basic_function_prompt.txt
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/chatgpt_fn/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:24:00.422026 alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/claude/
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/claude/basic_prompt.txt
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/claude/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:24:00.422026 alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/claude_2/
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/claude_2/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:24:00.422026 alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/claude_ranking/
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/claude_ranking/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/claude_ranking/ranking_prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:24:00.422026 alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/cohere/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/cohere/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:24:00.422026 alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/gpt4/
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/gpt4/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:24:00.422026 alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/guanaco_33b/
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/guanaco_33b/basic_prompt.txt
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/guanaco_33b/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:24:00.422026 alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/improved_aviary_gpt4/
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/improved_aviary_gpt4/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:24:00.422026 alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/improved_lmsys_gpt4/
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/improved_lmsys_gpt4/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:24:00.422026 alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/lmsys_gpt4/
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/lmsys_gpt4/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/lmsys_gpt4/lmsys_prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:24:00.422026 alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/oasst_pythia_12b/
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/oasst_pythia_12b/basic_prompt.txt
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/oasst_pythia_12b/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:24:00.422026 alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/test/
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/test/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:24:00.426027 alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/text_davinci_003/
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/text_davinci_003/basic_prompt.txt
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/text_davinci_003/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:24:00.406025 alpaca_eval-0.2.3/src/alpaca_eval/leaderboards/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:24:00.426027 alpaca_eval-0.2.3/src/alpaca_eval/leaderboards/data_AlpacaEval/
--rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/leaderboards/data_AlpacaEval/alpaca_eval_gpt4_leaderboard.csv
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/leaderboards/data_AlpacaEval/chatgpt_fn_leaderboard.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/leaderboards/data_AlpacaEval/claude_leaderboard.csv
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/leaderboards/data_AlpacaEval/text_davinci_003_leaderboard.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:24:00.426027 alpaca_eval-0.2.3/src/alpaca_eval/leaderboards/evaluators/
--rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/leaderboards/evaluators/evaluators_leaderboard.csv
--rw-r--r--   0 runner    (1001) docker     (123)    21848 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:24:00.410025 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:24:00.426027 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/airoboros-33b/
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/airoboros-33b/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/airoboros-33b/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:24:00.426027 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/airoboros-65b/
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/airoboros-65b/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:24:00.426027 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/alpaca-7b/
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/alpaca-7b/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/alpaca-7b/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:24:00.426027 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/alpaca-farm-ppo-human/
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/alpaca-farm-ppo-human/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:24:00.426027 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/alpaca-farm-ppo-sim-gpt4-20k/
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/alpaca-farm-ppo-sim-gpt4-20k/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:24:00.426027 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/baize-v2-13b/
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/baize-v2-13b/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/baize-v2-13b/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:24:00.426027 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/baize-v2-7b/
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/baize-v2-7b/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:24:00.426027 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/chatgpt/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/chatgpt/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:24:00.426027 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/claude/
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/claude/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/claude/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:24:00.426027 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/claude-2/
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/claude-2/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:24:00.426027 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/cohere/
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/cohere/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/cohere/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:24:00.426027 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/cohere-chat/
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/cohere-chat/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:24:00.426027 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/falcon-40b-instruct/
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/falcon-40b-instruct/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:24:00.426027 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/falcon-7b-instruct/
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/falcon-7b-instruct/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:24:00.430027 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/gpt4/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/gpt4/chatml_prompt.txt
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/gpt4/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:24:00.430027 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/guanaco-13b/
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/guanaco-13b/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:24:00.430027 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/guanaco-33b/
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/guanaco-33b/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:24:00.430027 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/guanaco-65b/
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/guanaco-65b/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:24:00.430027 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/guanaco-7b/
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/guanaco-7b/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/guanaco-7b/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:24:00.430027 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/minotaur-13b/
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/minotaur-13b/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/minotaur-13b/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:24:00.430027 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/nous-hermes-13b/
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/nous-hermes-13b/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/nous-hermes-13b/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:24:00.430027 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/oasst-rlhf-llama-33b/
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/oasst-rlhf-llama-33b/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:24:00.430027 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/oasst-sft-llama-33b/
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/oasst-sft-llama-33b/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/oasst-sft-llama-33b/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:24:00.430027 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/oasst-sft-pythia-12b/
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/oasst-sft-pythia-12b/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/oasst-sft-pythia-12b/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:24:00.430027 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/openchat-13b/
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/openchat-13b/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/openchat-13b/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:24:00.430027 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/openchat-v2-13b/
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/openchat-v2-13b/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:24:00.430027 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/openchat-v2-w-13b/
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/openchat-v2-w-13b/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:24:00.430027 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/openchat8192-13b/
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/openchat8192-13b/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:24:00.430027 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/opencoderplus-15b/
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/opencoderplus-15b/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:24:00.430027 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/pythia-12b-mix-sft/
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/pythia-12b-mix-sft/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:24:00.430027 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/text_davinci_001/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/text_davinci_001/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:24:00.430027 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/text_davinci_003/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/text_davinci_003/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/text_davinci_003/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:24:00.434027 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/ultralm-13b/
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/ultralm-13b/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/ultralm-13b/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:24:00.434027 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/vicuna-13b/
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/vicuna-13b/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:24:00.434027 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/vicuna-13b-v1.3/
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/vicuna-13b-v1.3/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:24:00.434027 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/vicuna-33b-v1.3/
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/vicuna-33b-v1.3/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:24:00.434027 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/vicuna-7b/
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/vicuna-7b/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/vicuna-7b/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:24:00.434027 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/vicuna-7b-v1.3/
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/vicuna-7b-v1.3/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:24:00.434027 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/wizardlm-13b/
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/wizardlm-13b/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/wizardlm-13b/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:24:00.434027 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/wizardlm-13b-v1.1/
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/wizardlm-13b-v1.1/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    20680 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    16065 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:24:00.414026 alpaca_eval-0.2.3/src/alpaca_eval.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    66635 2023-07-15 16:24:00.000000 alpaca_eval-0.2.3/src/alpaca_eval.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7580 2023-07-15 16:24:00.000000 alpaca_eval-0.2.3/src/alpaca_eval.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 16:24:00.000000 alpaca_eval-0.2.3/src/alpaca_eval.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-15 16:24:00.000000 alpaca_eval-0.2.3/src/alpaca_eval.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-07-15 16:24:00.000000 alpaca_eval-0.2.3/src/alpaca_eval.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-15 16:24:00.000000 alpaca_eval-0.2.3/src/alpaca_eval.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:24:00.434027 alpaca_eval-0.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    17869 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/tests/test_analyze.py
--rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/tests/test_decoders_unit.py
--rw-r--r--   0 runner    (1001) docker     (123)     6381 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     5734 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/tests/test_pairwise_evaluator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.139952 alpaca_eval-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11409 2023-07-21 15:22:38.000000 alpaca_eval-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-21 15:22:38.000000 alpaca_eval-0.2.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    67440 2023-07-21 15:23:03.139952 alpaca_eval-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    66618 2023-07-21 15:22:38.000000 alpaca_eval-0.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.115952 alpaca_eval-0.2.4/example/
+-rw-r--r--   0 runner    (1001) docker     (123)   500735 2023-07-21 15:22:38.000000 alpaca_eval-0.2.4/example/outputs.json
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 15:23:03.139952 alpaca_eval-0.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.091951 alpaca_eval-0.2.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.119952 alpaca_eval-0.2.4/src/alpaca_eval/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-21 15:22:48.000000 alpaca_eval-0.2.4/src/alpaca_eval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21377 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/analyze.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.123952 alpaca_eval-0.2.4/src/alpaca_eval/annotators/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/annotators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26474 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/annotators/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16494 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/annotators/pairwise_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6389 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/completion_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4756 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.127952 alpaca_eval-0.2.4/src/alpaca_eval/decoders/
+-rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/decoders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4409 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/decoders/anthropic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/decoders/cohere.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/decoders/huggingface_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5090 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/decoders/huggingface_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12959 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/decoders/openai.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/decoders/replicate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.127952 alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/
+-rw-r--r--   0 runner    (1001) docker     (123)     9753 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.127952 alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4/alpaca_eval.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.127952 alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4_fn/
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4_fn/alpaca_eval_fn.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4_fn/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.127952 alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/alpaca_farm/
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_chat_v0_without_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5869 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_chat_without_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_cot_json_without_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_without_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b4_cot_json_without_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6849 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_diana_without_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6797 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_joe_without_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6700 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_without_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6045 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/alpaca_farm/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b1_v0_without_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3969 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b1_without_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5932 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b4_reasoning_without_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5370 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b5_without_inputs.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.127952 alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/alpaca_farm_greedy_gpt4/
+-rw-r--r--   0 runner    (1001) docker     (123)     7373 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/alpaca_farm_greedy_gpt4/chatml_b5_without_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/alpaca_farm_greedy_gpt4/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.127952 alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/aviary_gpt4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/aviary_gpt4/aviary_prompt.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/aviary_gpt4/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.127952 alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/chatgpt/
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/chatgpt/basic_prompt.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/chatgpt/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.127952 alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/chatgpt_fn/
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/chatgpt_fn/basic_function_prompt.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/chatgpt_fn/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.127952 alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/claude/
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/claude/basic_prompt.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/claude/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.127952 alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/claude_2/
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/claude_2/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.131952 alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/claude_ranking/
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/claude_ranking/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/claude_ranking/ranking_prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.131952 alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/cohere/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/cohere/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.131952 alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/gpt4/
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/gpt4/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.131952 alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/guanaco_33b/
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/guanaco_33b/basic_prompt.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/guanaco_33b/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.131952 alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/improved_aviary_gpt4/
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/improved_aviary_gpt4/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.131952 alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/improved_lmsys_gpt4/
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/improved_lmsys_gpt4/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.131952 alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/lmsys_gpt4/
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/lmsys_gpt4/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/lmsys_gpt4/lmsys_prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.131952 alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/oasst_pythia_12b/
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/oasst_pythia_12b/basic_prompt.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/oasst_pythia_12b/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.131952 alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/test/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.131952 alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/text_davinci_003/
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/text_davinci_003/basic_prompt.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/text_davinci_003/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.099952 alpaca_eval-0.2.4/src/alpaca_eval/leaderboards/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.131952 alpaca_eval-0.2.4/src/alpaca_eval/leaderboards/data_AlpacaEval/
+-rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/leaderboards/data_AlpacaEval/alpaca_eval_gpt4_leaderboard.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/leaderboards/data_AlpacaEval/chatgpt_fn_leaderboard.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/leaderboards/data_AlpacaEval/claude_leaderboard.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/leaderboards/data_AlpacaEval/text_davinci_003_leaderboard.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.131952 alpaca_eval-0.2.4/src/alpaca_eval/leaderboards/evaluators/
+-rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/leaderboards/evaluators/evaluators_leaderboard.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    21848 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.111952 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.131952 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/airoboros-33b/
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/airoboros-33b/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/airoboros-33b/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.131952 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/airoboros-65b/
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/airoboros-65b/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.131952 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/alpaca-7b/
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/alpaca-7b/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/alpaca-7b/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.131952 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/alpaca-farm-ppo-human/
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/alpaca-farm-ppo-human/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.131952 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/alpaca-farm-ppo-sim-gpt4-20k/
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/alpaca-farm-ppo-sim-gpt4-20k/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.131952 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/baichuan-13b-chat/
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/baichuan-13b-chat/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/baichuan-13b-chat/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.131952 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/baize-v2-13b/
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/baize-v2-13b/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/baize-v2-13b/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.131952 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/baize-v2-7b/
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/baize-v2-7b/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.131952 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/chatglm2-6b/
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/chatglm2-6b/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/chatglm2-6b/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.131952 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/chatgpt/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/chatgpt/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.135952 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/claude/
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/claude/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/claude/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.135952 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/claude-2/
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/claude-2/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.135952 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/cohere/
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/cohere/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/cohere/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.135952 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/cohere-chat/
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/cohere-chat/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.135952 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/falcon-40b-instruct/
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/falcon-40b-instruct/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.135952 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/falcon-7b-instruct/
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/falcon-7b-instruct/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.135952 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/gpt4/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/gpt4/chatml_prompt.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/gpt4/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.135952 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/guanaco-13b/
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/guanaco-13b/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.135952 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/guanaco-33b/
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/guanaco-33b/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.135952 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/guanaco-65b/
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/guanaco-65b/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.135952 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/guanaco-7b/
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/guanaco-7b/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/guanaco-7b/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.135952 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/llama-2-13b-chat-hf/
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/llama-2-13b-chat-hf/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.135952 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/llama-2-70b-chat-hf/
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/llama-2-70b-chat-hf/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.135952 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/llama-2-70b-chat-hf-replicate/
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/llama-2-70b-chat-hf-replicate/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/llama-2-70b-chat-hf-replicate/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.135952 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/llama-2-70b-chat-hf-replicate-noprompt/
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/llama-2-70b-chat-hf-replicate-noprompt/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/llama-2-70b-chat-hf-replicate-noprompt/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.135952 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/llama-2-7b-chat-hf/
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/llama-2-7b-chat-hf/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/llama-2-7b-chat-hf/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.135952 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/minotaur-13b/
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/minotaur-13b/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/minotaur-13b/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.135952 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/nous-hermes-13b/
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/nous-hermes-13b/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/nous-hermes-13b/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.135952 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/oasst-rlhf-llama-33b/
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/oasst-rlhf-llama-33b/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.135952 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/oasst-sft-llama-33b/
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/oasst-sft-llama-33b/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/oasst-sft-llama-33b/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.135952 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/oasst-sft-pythia-12b/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/oasst-sft-pythia-12b/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/oasst-sft-pythia-12b/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.139952 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/openchat-13b/
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/openchat-13b/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/openchat-13b/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.139952 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/openchat-v2-13b/
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/openchat-v2-13b/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.139952 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/openchat-v2-w-13b/
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/openchat-v2-w-13b/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.139952 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/openchat8192-13b/
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/openchat8192-13b/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.139952 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/opencoderplus-15b/
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/opencoderplus-15b/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.139952 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/pythia-12b-mix-sft/
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/pythia-12b-mix-sft/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.139952 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/text_davinci_001/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/text_davinci_001/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.139952 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/text_davinci_003/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/text_davinci_003/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/text_davinci_003/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.139952 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/ultralm-13b/
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/ultralm-13b/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/ultralm-13b/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.139952 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/vicuna-13b/
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/vicuna-13b/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.139952 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/vicuna-13b-v1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/vicuna-13b-v1.3/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.139952 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/vicuna-33b-v1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/vicuna-33b-v1.3/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.139952 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/vicuna-7b/
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/vicuna-7b/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/vicuna-7b/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.139952 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/vicuna-7b-v1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/vicuna-7b-v1.3/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.139952 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/wizardlm-13b/
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/wizardlm-13b/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/wizardlm-13b/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.139952 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/wizardlm-13b-v1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/models_configs/wizardlm-13b-v1.1/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    20680 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16065 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/src/alpaca_eval/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.123952 alpaca_eval-0.2.4/src/alpaca_eval.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    67440 2023-07-21 15:23:03.000000 alpaca_eval-0.2.4/src/alpaca_eval.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8412 2023-07-21 15:23:03.000000 alpaca_eval-0.2.4/src/alpaca_eval.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 15:23:03.000000 alpaca_eval-0.2.4/src/alpaca_eval.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-21 15:23:03.000000 alpaca_eval-0.2.4/src/alpaca_eval.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-07-21 15:23:03.000000 alpaca_eval-0.2.4/src/alpaca_eval.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-21 15:23:03.000000 alpaca_eval-0.2.4/src/alpaca_eval.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:03.139952 alpaca_eval-0.2.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    17869 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/tests/test_analyze.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/tests/test_decoders_unit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6381 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-07-21 15:22:39.000000 alpaca_eval-0.2.4/tests/test_pairwise_evaluator.py
```

### Comparing `alpaca_eval-0.2.3/LICENSE` & `alpaca_eval-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.3/PKG-INFO` & `alpaca_eval-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alpaca_eval
-Version: 0.2.3
+Version: 0.2.4
 Summary: AlpacaEval : An Automatic Evaluator of Instruction-following Models
 Author: The Alpaca Team
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -113,15 +113,15 @@
 
 ```bash
 export OPENAI_API_KEY=<your_api_key>
 export OPENAI_ORGANIZATION_IDS=<your_organization_id>  # Optional; if not set, this will be your default org id.
 alpaca_eval --model_outputs 'example/outputs.json' 
 ```
 
-Important parameters are the following:
+This will print the leaderboard to the console, and save both the leaderboard and the annotations to the same directory as the `model_outputs` file. Important parameters are the following:
 
 - **model_outputs** : A path to a json file for the outputs of the model to add to the leaderboard. Each dictionary
   should
   contain the keys `instruction` and `output`.
 - **annotators_config**: This is the annotator to use (e.g., `alpaca_eval_gpt4` or `claude`
   or `chatgpt_fn`). `alpaca_eval_gpt4` (
   default) has the
@@ -1057,14 +1057,29 @@
 ```
 
 After running this command, you should have generated an outputs json and a new entry in the corresponding [leaderboard
 file](https://github.com/tatsu-lab/alpaca_eval/tree/main/src/alpaca_eval/leaderboards/data_AlpacaEval). Please make a PR
 with the
 config, outputs file, and updated leaderboard.
 
+Concretely you should do something like:
+
+1. Fork the repository in github
+2. Clone the forked repository `git clone <URL>`
+3. Make a model config at `src/alpaca_eval/models_configs/<model_name>` and evaluate it `evaluate_from_model --model_configs '<model_name>'`
+4. Add the model configs, output, and leaderboard entry to the forked repository
+```sh
+git add src/alpaca_eval/models_configs/<model_name>
+git add src/alpaca_eval/leaderboards/data_AlpacaEval
+git add results/<model_name>/model_outputs.json
+git commit -m "Add <model_name> to AlpacaEval"
+git push
+``` 
+5. Create a [pull request on AlpacaEval](https://github.com/tatsu-lab/alpaca_eval/pulls)
+
 </details>
 
 <details>
   <summary><h2 tabindex="-1" dir="auto">Contributing an evaluator</h2></summary>
 
 Please first follow the directions in [Making a new evaluator](#making-a-new-evaluator).
 Once you're created the annotator config, we ask that you create a new leaderboard for the annotator by evaluating the
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: alpaca_eval Version: 0.2.3 Summary: AlpacaEval : An
+Metadata-Version: 2.1 Name: alpaca_eval Version: 0.2.4 Summary: AlpacaEval : An
 Automatic Evaluator of Instruction-following Models Author: The Alpaca Team
 Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
 Education Classifier: Intended Audience :: Science/Research Classifier: License
 :: OSI Approved :: Apache Software License Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
 Python :: 3.12 Classifier: Topic :: Scientific/Engineering :: Artificial
@@ -69,23 +69,25 @@
 Release](#data-release) - [Differences with AlpacaFarm](#differences-with-
 alpacafarm) - [Related work](#related-work) - [Major updates](#major-updates)
 # Quick Start To install the stable release, run ```bash pip install alpaca-
 eval ``` To install the nightly version, run ```bash pip install git+https://
 github.com/tatsu-lab/alpaca_eval ``` Then you can use it as follows: ```bash
 export OPENAI_API_KEY= export OPENAI_ORGANIZATION_IDS= # Optional; if not set,
 this will be your default org id. alpaca_eval --model_outputs 'example/
-outputs.json' ``` Important parameters are the following: - **model_outputs** :
-A path to a json file for the outputs of the model to add to the leaderboard.
-Each dictionary should contain the keys `instruction` and `output`. -
-**annotators_config**: This is the annotator to use (e.g., `alpaca_eval_gpt4`
-or `claude` or `chatgpt_fn`). `alpaca_eval_gpt4` ( default) has the highest
-agreement rate with our human annotation data. `claude` has a decent agreement
-and is free for academics. `chatgpt_fn` is the worst of the three, but is
-available to everyone, cheap, and has 2x larger context window (16K tokens).
-For a comparison of annotators see [here](#evaluators). -
+outputs.json' ``` This will print the leaderboard to the console, and save both
+the leaderboard and the annotations to the same directory as the
+`model_outputs` file. Important parameters are the following: -
+**model_outputs** : A path to a json file for the outputs of the model to add
+to the leaderboard. Each dictionary should contain the keys `instruction` and
+`output`. - **annotators_config**: This is the annotator to use (e.g.,
+`alpaca_eval_gpt4` or `claude` or `chatgpt_fn`). `alpaca_eval_gpt4` ( default)
+has the highest agreement rate with our human annotation data. `claude` has a
+decent agreement and is free for academics. `chatgpt_fn` is the worst of the
+three, but is available to everyone, cheap, and has 2x larger context window
+(16K tokens). For a comparison of annotators see [here](#evaluators). -
 **reference_outputs**: The outputs of the reference model. Same format as
 `model_outputs`. By default, this is `text-davinci003` outputs on AlpacaEval
 dataset. - **output_path**: Path for saving annotations and leaderboard. If you
 don't have the model outputs, you can use [`evaluate_from_model`](https://
 github.com/tatsu-lab/alpaca_eval/tree/main#evaluating-a-model) and pass a local
 path or a name of a HuggingFace model, or a model from a standard API (OpenAI,
 Anthropic, Cohere). Other commands:  >>> alpaca_eval -- --help ``` SYNOPSIS
@@ -619,15 +621,23 @@
 model) to run inference on the model to produce outputs on the eval set and
 score the model according to one of the evaluators. An example command may look
 like: ```sh alpaca_eval evaluate_from_model \ --model_configs 'falcon-7b-
 instruct' \ --annotators_config 'alpaca_eval_gpt4' ``` After running this
 command, you should have generated an outputs json and a new entry in the
 corresponding [leaderboard file](https://github.com/tatsu-lab/alpaca_eval/tree/
 main/src/alpaca_eval/leaderboards/data_AlpacaEval). Please make a PR with the
-config, outputs file, and updated leaderboard.
+config, outputs file, and updated leaderboard. Concretely you should do
+something like: 1. Fork the repository in github 2. Clone the forked repository
+`git clone ` 3. Make a model config at `src/alpaca_eval/models_configs/` and
+evaluate it `evaluate_from_model --model_configs ''` 4. Add the model configs,
+output, and leaderboard entry to the forked repository ```sh git add src/
+alpaca_eval/models_configs/ git add src/alpaca_eval/leaderboards/
+data_AlpacaEval git add results//model_outputs.json git commit -m "Add  to
+AlpacaEval" git push ``` 5. Create a [pull request on AlpacaEval](https://
+github.com/tatsu-lab/alpaca_eval/pulls)
 ***** Contributing an evaluator *****
 Please first follow the directions in [Making a new evaluator](#making-a-new-
 evaluator). Once you're created the annotator config, we ask that you create a
 new leaderboard for the annotator by evaluating the minimal set of models. The
 outputs for these models can be found by downloading
 [alpaca_eval_all_outputs.json](https://huggingface.co/datasets/tatsu-lab/
 alpaca_eval/blob/main/alpaca_eval_all_outputs.json). ```bash alpaca_eval
```

### Comparing `alpaca_eval-0.2.3/README.md` & `alpaca_eval-0.2.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -90,15 +90,15 @@
 
 ```bash
 export OPENAI_API_KEY=<your_api_key>
 export OPENAI_ORGANIZATION_IDS=<your_organization_id>  # Optional; if not set, this will be your default org id.
 alpaca_eval --model_outputs 'example/outputs.json' 
 ```
 
-Important parameters are the following:
+This will print the leaderboard to the console, and save both the leaderboard and the annotations to the same directory as the `model_outputs` file. Important parameters are the following:
 
 - **model_outputs** : A path to a json file for the outputs of the model to add to the leaderboard. Each dictionary
   should
   contain the keys `instruction` and `output`.
 - **annotators_config**: This is the annotator to use (e.g., `alpaca_eval_gpt4` or `claude`
   or `chatgpt_fn`). `alpaca_eval_gpt4` (
   default) has the
@@ -1034,14 +1034,29 @@
 ```
 
 After running this command, you should have generated an outputs json and a new entry in the corresponding [leaderboard
 file](https://github.com/tatsu-lab/alpaca_eval/tree/main/src/alpaca_eval/leaderboards/data_AlpacaEval). Please make a PR
 with the
 config, outputs file, and updated leaderboard.
 
+Concretely you should do something like:
+
+1. Fork the repository in github
+2. Clone the forked repository `git clone <URL>`
+3. Make a model config at `src/alpaca_eval/models_configs/<model_name>` and evaluate it `evaluate_from_model --model_configs '<model_name>'`
+4. Add the model configs, output, and leaderboard entry to the forked repository
+```sh
+git add src/alpaca_eval/models_configs/<model_name>
+git add src/alpaca_eval/leaderboards/data_AlpacaEval
+git add results/<model_name>/model_outputs.json
+git commit -m "Add <model_name> to AlpacaEval"
+git push
+``` 
+5. Create a [pull request on AlpacaEval](https://github.com/tatsu-lab/alpaca_eval/pulls)
+
 </details>
 
 <details>
   <summary><h2 tabindex="-1" dir="auto">Contributing an evaluator</h2></summary>
 
 Please first follow the directions in [Making a new evaluator](#making-a-new-evaluator).
 Once you're created the annotator config, we ask that you create a new leaderboard for the annotator by evaluating the
```

#### html2text {}

```diff
@@ -58,23 +58,25 @@
 Release](#data-release) - [Differences with AlpacaFarm](#differences-with-
 alpacafarm) - [Related work](#related-work) - [Major updates](#major-updates)
 # Quick Start To install the stable release, run ```bash pip install alpaca-
 eval ``` To install the nightly version, run ```bash pip install git+https://
 github.com/tatsu-lab/alpaca_eval ``` Then you can use it as follows: ```bash
 export OPENAI_API_KEY= export OPENAI_ORGANIZATION_IDS= # Optional; if not set,
 this will be your default org id. alpaca_eval --model_outputs 'example/
-outputs.json' ``` Important parameters are the following: - **model_outputs** :
-A path to a json file for the outputs of the model to add to the leaderboard.
-Each dictionary should contain the keys `instruction` and `output`. -
-**annotators_config**: This is the annotator to use (e.g., `alpaca_eval_gpt4`
-or `claude` or `chatgpt_fn`). `alpaca_eval_gpt4` ( default) has the highest
-agreement rate with our human annotation data. `claude` has a decent agreement
-and is free for academics. `chatgpt_fn` is the worst of the three, but is
-available to everyone, cheap, and has 2x larger context window (16K tokens).
-For a comparison of annotators see [here](#evaluators). -
+outputs.json' ``` This will print the leaderboard to the console, and save both
+the leaderboard and the annotations to the same directory as the
+`model_outputs` file. Important parameters are the following: -
+**model_outputs** : A path to a json file for the outputs of the model to add
+to the leaderboard. Each dictionary should contain the keys `instruction` and
+`output`. - **annotators_config**: This is the annotator to use (e.g.,
+`alpaca_eval_gpt4` or `claude` or `chatgpt_fn`). `alpaca_eval_gpt4` ( default)
+has the highest agreement rate with our human annotation data. `claude` has a
+decent agreement and is free for academics. `chatgpt_fn` is the worst of the
+three, but is available to everyone, cheap, and has 2x larger context window
+(16K tokens). For a comparison of annotators see [here](#evaluators). -
 **reference_outputs**: The outputs of the reference model. Same format as
 `model_outputs`. By default, this is `text-davinci003` outputs on AlpacaEval
 dataset. - **output_path**: Path for saving annotations and leaderboard. If you
 don't have the model outputs, you can use [`evaluate_from_model`](https://
 github.com/tatsu-lab/alpaca_eval/tree/main#evaluating-a-model) and pass a local
 path or a name of a HuggingFace model, or a model from a standard API (OpenAI,
 Anthropic, Cohere). Other commands:  >>> alpaca_eval -- --help ``` SYNOPSIS
@@ -608,15 +610,23 @@
 model) to run inference on the model to produce outputs on the eval set and
 score the model according to one of the evaluators. An example command may look
 like: ```sh alpaca_eval evaluate_from_model \ --model_configs 'falcon-7b-
 instruct' \ --annotators_config 'alpaca_eval_gpt4' ``` After running this
 command, you should have generated an outputs json and a new entry in the
 corresponding [leaderboard file](https://github.com/tatsu-lab/alpaca_eval/tree/
 main/src/alpaca_eval/leaderboards/data_AlpacaEval). Please make a PR with the
-config, outputs file, and updated leaderboard.
+config, outputs file, and updated leaderboard. Concretely you should do
+something like: 1. Fork the repository in github 2. Clone the forked repository
+`git clone ` 3. Make a model config at `src/alpaca_eval/models_configs/` and
+evaluate it `evaluate_from_model --model_configs ''` 4. Add the model configs,
+output, and leaderboard entry to the forked repository ```sh git add src/
+alpaca_eval/models_configs/ git add src/alpaca_eval/leaderboards/
+data_AlpacaEval git add results//model_outputs.json git commit -m "Add  to
+AlpacaEval" git push ``` 5. Create a [pull request on AlpacaEval](https://
+github.com/tatsu-lab/alpaca_eval/pulls)
 ***** Contributing an evaluator *****
 Please first follow the directions in [Making a new evaluator](#making-a-new-
 evaluator). Once you're created the annotator config, we ask that you create a
 new leaderboard for the annotator by evaluating the minimal set of models. The
 outputs for these models can be found by downloading
 [alpaca_eval_all_outputs.json](https://huggingface.co/datasets/tatsu-lab/
 alpaca_eval/blob/main/alpaca_eval_all_outputs.json). ```bash alpaca_eval
```

### Comparing `alpaca_eval-0.2.3/example/outputs.json` & `alpaca_eval-0.2.4/example/outputs.json`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.3/setup.py` & `alpaca_eval-0.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     "pytest",
     "pytest-mock",
     "pytest-skip-slow",
     "python-dotenv",
 ]
 PACKAGES_ANALYSIS = ["seaborn", "matplotlib", "jupyterlab"]
 PACKAGES_LOCAL = ["accelerate", "transformers", "bitsandbytes", "xformers", "peft", "optimum", "scipy", "einops"]
-PACKAGES_ALL_API = ["anthropic>=0.3.3", "huggingface_hub", "cohere"]
+PACKAGES_ALL_API = ["anthropic>=0.3.3", "huggingface_hub", "cohere", "replicate"]
 PACKAGES_ALL = PACKAGES_LOCAL + PACKAGES_ALL_API + PACKAGES_ANALYSIS + PACKAGES_DEV
 
 setuptools.setup(
     name="alpaca_eval",
     version=version,
     description="AlpacaEval : An Automatic Evaluator of Instruction-following Models",
     package_dir={"": "src"},
```

### Comparing `alpaca_eval-0.2.3/src/alpaca_eval/analyze.py` & `alpaca_eval-0.2.4/src/alpaca_eval/analyze.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.3/src/alpaca_eval/annotators/base.py` & `alpaca_eval-0.2.4/src/alpaca_eval/annotators/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -75,15 +75,19 @@
 
     def __init__(
         self,
         primary_keys: Sequence[str],
         annotators_config: Union[utils.AnyPath, list[dict[str, Any]]] = "claude",
         seed: Optional[int] = 0,
         is_avoid_reannotations: bool = True,
-        other_keys_to_keep: Sequence[str] = ("price_per_example", "time_per_example"),
+        other_keys_to_keep: Sequence[str] = (
+            "price_per_example",
+            "time_per_example",
+            "raw_completion",
+        ),
         is_store_missing_annotations: bool = True,
         base_dir: Optional[utils.AnyPath] = None,
         is_raise_if_missing_primary_keys: bool = True,
         annotation_type: Optional[Type] = None,
     ):
         logging.info(f"Creating the annotator from `{annotators_config}`.")
         self.base_dir = Path(base_dir or self.DEFAULT_BASE_DIR)
@@ -106,14 +110,19 @@
     @abc.abstractmethod
     def SingleAnnotator(self) -> Type["SingleAnnotator"]:
         """Class to use for each single annotator."""
         pass
 
     #######################
     @property
+    def available_fields_to_format(self):
+        """Fields that can be formatted in the prompt template."""
+        return self.all_keys
+
+    @property
     def annotation_key(self) -> str:
         """How to refer to the annotations, this will be the key for annotations in the output."""
         return "annotation"
 
     @property
     def random_seed_key(self) -> list[str]:
         """What key / column to seed on for the random generator."""
@@ -171,15 +180,18 @@
             # in case a path is given we make it relative to that path
             base_dir = self.annotators_config.parents[1]
         except:
             base_dir = self.base_dir
 
         return {
             name: self.SingleAnnotator(
-                seed=self.seed, base_dir=base_dir, annotation_column=self.annotation_key, **annotator_config
+                seed=self.seed,
+                base_dir=base_dir,
+                annotation_column=self.annotation_key,
+                **annotator_config,
             )
             for name, annotator_config in annotators_config.items()
         }
 
     def _add_missing_primary_keys_(self, df: pd.DataFrame):
         missing_primary_keys = [c for c in self.primary_keys if c not in df.columns]
         if self.is_raise_if_missing_primary_keys:
@@ -227,15 +239,18 @@
             curr_idcs = df_annotated[self.ANNOTATOR_COLUMN] == annotator
             if self.annotation_key in df_annotated.columns:
                 curr_idcs &= df_annotated[self.annotation_key].isna()
 
             logging.info(f"Annotating {curr_idcs.sum()} examples with {annotator}")
 
             # actual annotation
-            curr_annotated = self.annotators[annotator](df_annotated.loc[curr_idcs, self.all_keys], **decoding_kwargs)
+            curr_annotated = self.annotators[annotator](
+                df_annotated.loc[curr_idcs, self.available_fields_to_format],
+                **decoding_kwargs,
+            )
 
             df_annotated = self._merge_annotations(df_annotated, curr_annotated)
 
         return df_annotated
 
     def _postprocess_and_store_(
         self,
@@ -267,30 +282,33 @@
             # put back None
             df_annotated[self.annotation_key] = df_annotated[self.annotation_key].replace(
                 self.TMP_MISSING_ANNOTATION, None
             )
 
         # need to merge with df_to_annotate in case you dropped duplicates
         on = list(self.primary_keys)
-        df_annotated = df_annotated[self._get_all_keys_to_keep(df_to_annotate)]
+        # keeps columns from both df_to_annotate and df_annotated that are useful
+        df_annotated = df_annotated[
+            self._get_all_keys_to_keep(list(df_to_annotate.columns) + list(df_annotated.columns))
+        ]
         df_to_annotate = df_to_annotate[[c for c in df_to_annotate.columns if c not in df_annotated.columns or c in on]]
         # need to remove all other columns before merging if not you will
         df_annotated = df_to_annotate.merge(df_annotated, on=on, how="outer")
 
         annotated = df_annotated.to_dict(orient="records")
 
         return annotated
 
     def _filter_annotations_before_storing(self, df_annotated: pd.DataFrame) -> pd.DataFrame:
         """Filter annotations before storing them."""
-        df_annotated = df_annotated[self._get_all_keys_to_keep(df_annotated)]
+        df_annotated = df_annotated[self._get_all_keys_to_keep(df_annotated.columns)]
         return df_annotated
 
-    def _get_all_keys_to_keep(self, df: pd.DataFrame) -> list[str]:
-        other_keys_to_keep = [c for c in self.other_keys_to_keep if c in df.columns]
+    def _get_all_keys_to_keep(self, current_columns: Sequence) -> list[str]:
+        other_keys_to_keep = [c for c in self.other_keys_to_keep if c in current_columns]
         all_keys_to_keep = self.all_keys + [self.annotation_key] + other_keys_to_keep
         return all_keys_to_keep
 
     def _apply_cached_annotations(self, df_to_annotate: pd.DataFrame) -> pd.DataFrame:
         """annotate examples with cached annotations"""
         df_to_annotate = self._merge_annotations(df_to_annotate, self.df_annotations)
         return df_to_annotate
@@ -316,21 +334,23 @@
         kwargs = dict(
             on=self.all_keys,
             how="left",
             suffixes=("_old", "_new"),
         )
         try:
             df_to_annotate = df_to_annotate.merge(
-                df_partially_annotated[self.all_keys + [self.annotation_key] + other_keys_to_keep], **kwargs
+                df_partially_annotated[self.all_keys + [self.annotation_key] + other_keys_to_keep],
+                **kwargs,
             )
         except ValueError:
             # can have merging issues if columns have different dtypes
             df_partially_annotated = df_partially_annotated.astype({k: str for k in self.all_keys})
             df_to_annotate = df_to_annotate.astype({k: str for k in self.all_keys}).merge(
-                df_partially_annotated[self.all_keys + [self.annotation_key] + other_keys_to_keep], **kwargs
+                df_partially_annotated[self.all_keys + [self.annotation_key] + other_keys_to_keep],
+                **kwargs,
             )
 
         # if columns were in both dataframes, try to merge them
         for c in other_keys_to_keep + [self.annotation_key]:
             if f"{c}_old" in df_to_annotate.columns and f"{c}_new" in df_to_annotate.columns:
                 df_to_annotate[c] = df_to_annotate[c + "_old"].fillna(df_to_annotate[c + "_new"])
                 df_to_annotate = df_to_annotate.drop(columns=[c + "_old", c + "_new"])
@@ -339,15 +359,16 @@
 
     #######################
 
 
 class BaseAnnotatorJSON(BaseAnnotator):
     __doc__ = (
         BaseAnnotator.__doc__.replace(
-            "Base class for a pool of annotators.", "Base class for a pool of annotators with caching to JSON file."
+            "Base class for a pool of annotators.",
+            "Base class for a pool of annotators with caching to JSON file.",
         )
         + """
     caching_path : Path, optional
         Path to cache the annotations to. If None, will not save the annotations. If the path already exists it will
         load annotations from there.
     """
     )
@@ -439,28 +460,32 @@
 
     base_dir : Path, optional
         Path to the directory containing the annotators configs. I.e. annotators_config will be relative
         to this directory.
 
     annotation_column : str, optional
         Name of the annotation column in the output dataframe.
+
+    is_store_raw_completions : bool, optional
+        Whether to store raw completions at `"raw_completion"` column in the output dataframe.
     """
 
     def __init__(
         self,
         prompt_template: utils.AnyPath,
         fn_completion_parser: Optional[Union[Callable, str]] = "regex_parser",
         completion_parser_kwargs: Optional[dict[str, Any]] = None,
         fn_completions: Union[Callable, str] = "openai_completions",
         completions_kwargs: Optional[dict[str, Any]] = None,
         is_shuffle: bool = True,
         seed: Optional[int] = 123,
         batch_size: int = 1,
         base_dir: utils.AnyPath = constants.EVALUATORS_CONFIG_DIR,
         annotation_column: str = "annotation",
+        is_store_raw_completions: bool = False,
     ):
         self.base_dir = Path(base_dir)
         self.prompt_template = self._get_prompt_template(prompt_template)
 
         if fn_completion_parser is None:
             fn_completion_parser = lambda x: [x]
         elif isinstance(fn_completion_parser, str):
@@ -470,14 +495,15 @@
 
         self.fn_completions = get_fn_completions(fn_completions)
         self.completions_kwargs = completions_kwargs or {}
         self.seed = seed
         self.is_shuffle = is_shuffle
         self.batch_size = batch_size
         self.annotation_column = annotation_column
+        self.completion_column = "raw_completion" if is_store_raw_completions else None
 
     ### Public methods ###
     def __call__(self, df_to_annotate: pd.DataFrame, **decoding_kwargs) -> pd.DataFrame:
         """Annotates the given examples.
 
         Parameters
         ----------
@@ -496,15 +522,19 @@
         df_to_annotate = self._preprocess(df_to_annotate)
 
         # prompts and completions here will not be the same length as the dataframe due to batching
         prompts, df_to_annotate = self._make_prompts(df_to_annotate)
 
         completions = self.fn_completions(prompts=prompts, **self.completions_kwargs, **decoding_kwargs)
 
-        df_to_annotate[self.annotation_column] = self._parse_completions(completions=completions["completions"])
+        annotations_to_save, completions_to_save = self._parse_completions(completions=completions["completions"])
+        df_to_annotate[self.annotation_column] = annotations_to_save
+        if self.completion_column is not None:
+            df_to_annotate[self.completion_column] = completions_to_save
+
         for k, v in completions.items():
             if k != "completions":
                 if len(df_to_annotate[self.annotation_column]) == len(v) * self.batch_size:
                     v = [el for el in v for _ in range(self.batch_size)]
                 df_to_annotate[k] = v
                 if "per_example" in k:
                     df_to_annotate[k] = df_to_annotate[k] / self.batch_size
@@ -552,27 +582,37 @@
         """Preprocess the examples before annotating. In particular, takes care of all the randomization."""
 
         if self.is_shuffle:
             df_to_annotate = df_to_annotate.sample(frac=1, random_state=self.seed)
 
         return df_to_annotate
 
-    def _parse_completions(self, completions: list[str]) -> list[Any]:
+    def _parse_completions(self, completions: list[str]) -> tuple[list[Any], list[Any]]:
         """Converts the completions into annotations."""
         all_annotations = []
+        all_completions = []
         for completion in completions:
-            batch_annotations = list(self.fn_completion_parser(completion))
-            if len(batch_annotations) != self.batch_size:
-                logging.warning(
-                    f"Found {len(batch_annotations)} annotations in:'''\n{completion}\n''' but expected"
-                    f" {self.batch_size}. We are setting all annotations to None."
-                )
+            try:
+                batch_annotations = self.fn_completion_parser(completion)
+                batch_annotations = list(batch_annotations)
+
+                if len(batch_annotations) != self.batch_size:
+                    logging.warning(
+                        f"Found {len(batch_annotations)} annotations in:'''\n{completion}\n''' but expected"
+                        f" {self.batch_size}. We are setting all annotations to None."
+                    )
+                    batch_annotations = [None] * self.batch_size
+
+            except Exception as e:
+                logging.exception(f"Error while parsing completion: '''\n{completion}\n'''")
                 batch_annotations = [None] * self.batch_size
+
             all_annotations += batch_annotations
-        return all_annotations
+            all_completions += [completion] * self.batch_size
+        return all_annotations, all_completions
 
     def _postprocess(self, df_annotated: pd.DataFrame) -> pd.DataFrame:
         """Postprocess the annotated examples."""
 
         # remove padding examples when using batch_size > 1
         df_annotated = df_annotated.query("is_padding == False").drop(columns=["is_padding"])
```

### Comparing `alpaca_eval-0.2.3/src/alpaca_eval/annotators/pairwise_evaluator.py` & `alpaca_eval-0.2.4/src/alpaca_eval/annotators/pairwise_evaluator.py`

 * *Files 0% similar despite different names*

```diff
@@ -365,15 +365,17 @@
         df_to_annotate = super()._preprocess(df_to_annotate)
 
         return df_to_annotate
 
     def _postprocess(self, df_annotated: pd.DataFrame) -> pd.DataFrame:
         df_annotated = super()._postprocess(df_annotated)
 
-        assert set(df_annotated[self.annotation_column].unique().tolist()) <= {0, 1, 2}
+        all_values = df_annotated[self.annotation_column]
+        all_values = all_values[~all_values.isna()]
+        assert set(all_values.unique().tolist()) <= {0, 1, 2, np.nan}
 
         if self.is_randomize_output_order:
             # unshuffles output 1 and output 2. For binary preference, unshuffling is equivalent to reshuffling
             df_annotated = utils.shuffle_pairwise_preferences(df_annotated, df_annotated["is_switched_outputs"])
             df_annotated = df_annotated.drop(columns=["is_switched_outputs"])
 
         return df_annotated
```

### Comparing `alpaca_eval-0.2.3/src/alpaca_eval/completion_parsers.py` & `alpaca_eval-0.2.4/src/alpaca_eval/completion_parsers.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import ast
 import copy
+import json
 import logging
 import re
 from typing import Any
 
 import numpy as np
 
 from . import utils
@@ -115,7 +116,50 @@
         rank = [c for c in ordered_completions if c["model"] == "model_1"][0]["rank"]
         assert rank in [1, 2]
 
         return [rank]
     except Exception as e:
         logging.error(f"{e}\nContent: {completion}\n" "You must manually fix the score pair.")
         return [np.nan]
+
+
+def json_parser(completion: str, annotation_key: str) -> list[Any]:
+    """Parse the completion by reading it as a JSON and selecting "annotation_key".
+
+    Examples
+    --------
+    >>> completion = '{"short_explanation": "that is why", "is_incorporated": true}'
+    >>> json_parser(completion, "is_incorporated")
+    [True]
+    >>> completion = '[{"short_explanation": "that is why", "is_incorporated": true}, {"is_incorporated": false}]'
+    >>> json_parser(completion, "is_incorporated")
+    [True, False]
+    >>> completion = 'blah ```json\n{"short_explanation": "that is why", "integer": 1}```'
+    >>> json_parser(completion, "integer")
+    [1]
+    """
+    # search for a pattern "```json{...}```" and take what is inside the curly brackets
+    if "```json" in completion:
+        completion = re.search(r"```json(.*?)```", completion, re.DOTALL).group(1)
+
+    json_loaded = json.loads(completion)
+    if isinstance(json_loaded, dict):
+        return [json_loaded[annotation_key]]
+    return [d[annotation_key] for d in json.loads(completion)]
+
+
+def eval_parser(completion: str) -> list[Any]:
+    """Parse the completion by evaluating it.
+
+    Examples
+    --------
+    >>> eval_parser("True")
+    [True]
+    >>> eval_parser("(True,1,'False')")
+    [(True, 1, 'False')]
+    >>> eval_parser("[True,1,'False']")
+    [True, 1, 'False']
+    """
+    evaluated_completion = ast.literal_eval(completion)
+    if not isinstance(evaluated_completion, list):
+        evaluated_completion = [evaluated_completion]
+    return evaluated_completion
```

### Comparing `alpaca_eval-0.2.3/src/alpaca_eval/constants.py` & `alpaca_eval-0.2.4/src/alpaca_eval/constants.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,48 +23,14 @@
 ########################
 
 DEFAULT_CACHE_DIR = None
 CURRENT_DIR = Path(__file__).parent
 EVALUATORS_CONFIG_DIR = CURRENT_DIR / "evaluators_configs"
 MODELS_CONFIG_DIR = CURRENT_DIR / "models_configs"
 BASE_DIR = Path(__file__).parents[2]
-RESULTS_DIR = BASE_DIR / "results"
-
-MINIMAL_MODELS = (
-    "gpt4",
-    "claude",
-    "claude-2",
-    "chatgpt",
-    "wizardlm-13b",
-    "vicuna-13b",
-    "guanaco-65b",
-    "oasst-rlhf-llama-33b",
-    "text_davinci_003",
-    "alpaca-farm-ppo-human",
-    "falcon-40b-instruct",
-    "alpaca-7b",
-    "text_davinci_001",
-)
-VERIFIED_MODELS = MINIMAL_MODELS + (
-    "alpaca-farm-ppo-sim-gpt4-20k",
-    # "cohere", we only ran eval not generations
-    "falcon-7b-instruct",
-    "guanaco-7b",
-    "guanaco-13b",
-    "guanaco-33b",
-    "nous-hermes-13b",
-    "oasst-sft-llama-33b",
-    "oasst-sft-pythia-12b",
-    "pythia-12b-mix-sft",
-    "vicuna-7b",
-    "wizardlm-13b",
-    "vicuna-7b-v1.3",
-    "vicuna-13b-v1.3",
-    "vicuna-33b-v1.3",
-)
 
 MINIMAL_EVALUATORS = (
     "alpaca_eval_gpt4",
     "aviary_gpt4",
     "gpt4",
     "claude",
     "text_davinci_003",
```

### Comparing `alpaca_eval-0.2.3/src/alpaca_eval/decoders/__init__.py` & `alpaca_eval-0.2.4/src/alpaca_eval/decoders/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -53,9 +53,19 @@
         except ImportError as e:
             packages = ["cohere"]
             logging.exception(f"You need {packages} to use cohere_completions. Error:")
             raise e
 
         return cohere_completions
 
+    elif name == "replicate_completions":
+        try:
+            from .replicate import replicate_completions
+        except ImportError as e:
+            packages = ["replicate"]
+            logging.exception(f"You need {packages} to use replicate_completions. Error:")
+            raise e
+
+        return replicate_completions
+
     else:
         raise ValueError(f"Unknown decoder: {name}")
```

### Comparing `alpaca_eval-0.2.3/src/alpaca_eval/decoders/anthropic.py` & `alpaca_eval-0.2.4/src/alpaca_eval/decoders/anthropic.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,16 @@
     """
 
     n_examples = len(prompts)
     if n_examples == 0:
         logging.info("No samples to annotate.")
         return []
     else:
-        logging.info(f"Using `anthropic_completions` on {n_examples} prompts using {model_name}.")
+        to_log = f"Using `anthropic_completions` on {n_examples} prompts using {model_name} and num_procs={num_procs}."
+        logging.info(to_log)
 
     kwargs = dict(model=model_name, **decoding_kwargs)
     logging.info(f"Kwargs to completion: {kwargs}")
     with utils.Timer() as t:
         if num_procs == 1:
             completions = [
                 _anthropic_completion_helper(prompt, **kwargs) for prompt in tqdm.tqdm(prompts, desc="prompts")
```

### Comparing `alpaca_eval-0.2.3/src/alpaca_eval/decoders/cohere.py` & `alpaca_eval-0.2.4/src/alpaca_eval/decoders/cohere.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.3/src/alpaca_eval/decoders/huggingface_api.py` & `alpaca_eval-0.2.4/src/alpaca_eval/decoders/huggingface_api.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.3/src/alpaca_eval/decoders/huggingface_local.py` & `alpaca_eval-0.2.4/src/alpaca_eval/decoders/huggingface_local.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 import logging
 from typing import Optional, Sequence
 
 import numpy as np
 import torch
 import transformers
-from datasets import Dataset
 from peft import PeftModel
 from torch.utils.data import Dataset
-from tqdm import tqdm, trange
+from tqdm import tqdm
 from transformers import AutoModelForCausalLM, AutoTokenizer
 
 from .. import constants, utils
 
 __all__ = ["huggingface_local_completions"]
```

### Comparing `alpaca_eval-0.2.3/src/alpaca_eval/decoders/openai.py` & `alpaca_eval-0.2.4/src/alpaca_eval/decoders/openai.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/README.md` & `alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/README.md`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4/alpaca_eval.txt` & `alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4/alpaca_eval.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4_fn/alpaca_eval_fn.txt` & `alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4_fn/alpaca_eval_fn.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4_fn/configs.yaml` & `alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4_fn/configs.yaml`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_chat_v0_without_inputs.txt` & `alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_chat_v0_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_chat_without_inputs.txt` & `alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_chat_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_cot_json_without_inputs.txt` & `alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_cot_json_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_without_inputs.txt` & `alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b4_cot_json_without_inputs.txt` & `alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b4_cot_json_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_diana_without_inputs.txt` & `alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_diana_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_joe_without_inputs.txt` & `alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_joe_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_without_inputs.txt` & `alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/alpaca_farm/configs.yaml` & `alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/alpaca_farm/configs.yaml`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b1_v0_without_inputs.txt` & `alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b1_v0_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b1_without_inputs.txt` & `alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b1_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b4_reasoning_without_inputs.txt` & `alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b4_reasoning_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b5_without_inputs.txt` & `alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b5_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/alpaca_farm_greedy_gpt4/chatml_b5_without_inputs.txt` & `alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/alpaca_farm_greedy_gpt4/chatml_b5_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/aviary_gpt4/aviary_prompt.txt` & `alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/aviary_gpt4/aviary_prompt.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/chatgpt/basic_prompt.txt` & `alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/chatgpt/basic_prompt.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/chatgpt_fn/basic_function_prompt.txt` & `alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/chatgpt_fn/basic_function_prompt.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/chatgpt_fn/configs.yaml` & `alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/chatgpt_fn/configs.yaml`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/claude/basic_prompt.txt` & `alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/claude/basic_prompt.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/claude_ranking/ranking_prompt.txt` & `alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/claude_ranking/ranking_prompt.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/guanaco_33b/basic_prompt.txt` & `alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/guanaco_33b/basic_prompt.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/lmsys_gpt4/lmsys_prompt.txt` & `alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/lmsys_gpt4/lmsys_prompt.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/oasst_pythia_12b/basic_prompt.txt` & `alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/oasst_pythia_12b/basic_prompt.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/text_davinci_003/basic_prompt.txt` & `alpaca_eval-0.2.4/src/alpaca_eval/evaluators_configs/text_davinci_003/basic_prompt.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.3/src/alpaca_eval/leaderboards/data_AlpacaEval/alpaca_eval_gpt4_leaderboard.csv` & `alpaca_eval-0.2.4/src/alpaca_eval/leaderboards/data_AlpacaEval/alpaca_eval_gpt4_leaderboard.csv`

 * *Files 9% similar despite different names*

```diff
@@ -2,40 +2,45 @@
 gpt4,95.27950310559004,0.716281440286153,minimal,12,805,761,32,1365
 claude-2,91.35572139303484,0.9897323784630048,minimal,1,804,734,69,1069
 vicuna-33b-v1.3,88.99253731343283,1.095692216068168,verified,5,804,713,86,1479
 claude,88.38509316770187,1.1144875403283188,minimal,9,805,707,89,1082
 openchat-v2-w-13b,87.1268656716418,1.1769197439396015,community,3,804,699,102,1566
 wizardlm-13b-v1.1,86.31840796019901,1.2063217831272972,community,4,804,692,108,1525
 chatgpt,86.08695652173914,1.2110077772660273,minimal,6,805,690,109,811
+llama-2-70b-chat-hf,85.136815920398,1.253783670416838,minimal,1,804,684,119,1451
 openchat-v2-13b,84.96894409937889,1.2572979835605944,community,2,805,683,120,1564
 vicuna-13b-v1.3,82.11180124223603,1.348769957803504,verified,2,805,660,143,1132
+llama-2-13b-chat-hf,81.09452736318407,1.3817573087734825,minimal,0,804,652,152,1513
 openchat-13b,80.8695652173913,1.3843738653129234,community,2,805,650,153,1632
 ultralm-13b,80.63511830635119,1.3939556917204066,community,1,803,647,155,1087
 openchat8192-13b,79.53980099502488,1.4222439886269744,community,1,804,639,164,1664
 opencoderplus-15b,78.69565217391305,1.440029529188432,community,3,805,632,170,1628
 vicuna-7b-v1.3,76.8414481897628,1.487520320531845,verified,3,801,614,184,1110
 wizardlm-13b,75.31094527363184,1.5101858292160824,minimal,9,804,601,194,985
-airoboros-65b,73.91304347826086,1.5285333061227804,verified,16,805,587,202,1512
-airoboros-33b,73.29192546583852,1.55290318216736,verified,6,805,587,212,1514
+airoboros-65b,73.91304347826086,1.5285333061227804,community,16,805,587,202,1512
+airoboros-33b,73.29192546583852,1.55290318216736,community,6,805,587,212,1514
 guanaco-65b,71.80124223602485,1.586912361158523,minimal,0,805,578,227,1249
+llama-2-7b-chat-hf,71.36645962732919,1.593038654706019,minimal,1,805,574,230,1479
 vicuna-13b,70.43478260869566,1.6069688407799696,minimal,2,805,566,237,1037
 baize-v2-13b,66.95652173913044,1.6565358231309506,community,2,805,538,265,930
 oasst-rlhf-llama-33b,66.52173913043478,1.6608288428292477,minimal,3,805,534,268,1079
 minotaur-13b,66.02484472049689,1.6645545328264226,community,5,805,529,271,881
 guanaco-33b,65.96273291925466,1.67108537053247,verified,0,805,531,274,1311
 nous-hermes-13b,65.46583850931677,1.669962276077284,verified,6,805,524,275,844
 vicuna-7b,64.40993788819875,1.6851107260487883,verified,3,805,517,285,1044
 baize-v2-7b,63.85093167701863,1.6945981855442178,community,0,805,514,291,1127
 oasst-sft-llama-33b,54.96894409937888,1.7402667933686875,verified,13,805,436,356,748
 guanaco-13b,52.60869565217391,1.7576690299699242,verified,3,805,422,380,1774
 text_davinci_003,50.0,0.0,minimal,805,805,0,0,307
+chatglm2-6b,47.12858926342072,1.7593143221324448,community,5,801,375,421,1027
 guanaco-7b,46.58385093167702,1.7570464905413992,verified,2,805,374,429,1364
 falcon-40b-instruct,45.71428571428572,1.7524717060805597,minimal,4,805,366,435,662
 alpaca-farm-ppo-sim-gpt4-20k,44.099378881987576,1.7399772578861137,verified,10,805,350,445,511
 pythia-12b-mix-sft,41.86335403726708,1.737637146007538,verified,2,805,336,467,913
 alpaca-farm-ppo-human,41.24223602484472,1.7271813123250834,minimal,8,805,328,469,803
 cohere-chat,29.565217391304348,1.5949050483247118,community,12,805,232,561,779
 cohere,28.385093167701864,1.5717547121761728,community,15,805,221,569,682
 alpaca-7b,26.459627329192543,1.535711469748,minimal,16,805,205,584,396
 oasst-sft-pythia-12b,25.962732919254663,1.5261079289535309,verified,16,805,201,588,726
 falcon-7b-instruct,23.60248447204969,1.4898235369056625,verified,6,805,187,612,478
+baichuan-13b-chat,21.801242236024844,1.4495247592518703,community,5,805,173,627,1727
 text_davinci_001,15.17412935323383,1.235107892276849,minimal,20,804,112,672,296
```

### Comparing `alpaca_eval-0.2.3/src/alpaca_eval/leaderboards/data_AlpacaEval/chatgpt_fn_leaderboard.csv` & `alpaca_eval-0.2.4/src/alpaca_eval/leaderboards/data_AlpacaEval/chatgpt_fn_leaderboard.csv`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.3/src/alpaca_eval/leaderboards/data_AlpacaEval/claude_leaderboard.csv` & `alpaca_eval-0.2.4/src/alpaca_eval/leaderboards/data_AlpacaEval/claude_leaderboard.csv`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 ,win_rate,standard_error,mode,n_draws,n_total,n_wins,n_wins_base,output_length,avg_length
 gpt4,77.01863354037268,1.46803688292698,minimal,12,805,614,179,,1365
 claude,75.83850931677019,1.4981004247868313,minimal,9,805,606,190,,1082
 vicuna-33b-v1.3,72.36024844720497,1.5710737760483915,verified,5,805,580,220,,1479
 claude-2,71.98757763975155,1.5824915958976835,minimal,1,805,579,225,1069.0,1069
 chatgpt,67.70186335403726,1.642111587090117,minimal,6,805,542,257,,811
 vicuna-13b-v1.3,66.2111801242236,1.6657907370589309,verified,2,805,532,271,,1132
+llama-2-70b-chat-hf,66.14906832298136,1.6676994320973642,minimal,1,805,532,272,,1451
 wizardlm-13b,66.14906832298136,1.6584088766540706,minimal,9,805,528,268,,985
 vicuna-13b,63.22981366459627,1.698243477332765,minimal,2,805,508,295,,1037
 guanaco-65b,62.60869565217392,1.7063755171155923,minimal,0,805,504,301,,1249
 vicuna-7b-v1.3,62.54658385093168,1.7035470981976453,verified,3,805,502,300,,1110
 nous-hermes-13b,60.86956521739131,1.7144465955143962,verified,6,805,487,312,,844
 guanaco-33b,57.88819875776397,1.7412811662531051,verified,0,805,466,339,,1311
 vicuna-7b,57.329192546583855,1.7409917994657298,verified,3,805,460,342,,1044
 oasst-rlhf-llama-33b,57.329192546583855,1.7409917994657302,minimal,3,805,460,342,,1079
+llama-2-13b-chat-hf,56.149068322981364,1.7499783078823692,minimal,0,805,452,353,,1513
 guanaco-13b,53.36239103362392,1.7582560332920765,verified,3,803,427,373,,1774
+llama-2-7b-chat-hf,51.98757763975155,1.7608738025727095,minimal,1,805,418,386,,1479
 oasst-sft-llama-33b,51.24223602484472,1.748518981999294,verified,13,805,406,386,,748
 text_davinci_003,50.0,0.0,minimal,805,805,0,0,,307
 alpaca-farm-ppo-sim-gpt4-20k,48.19875776397515,1.7512254507446705,verified,10,805,383,412,,511
 guanaco-7b,47.5776397515528,1.7590989434689512,verified,2,805,382,421,,1364
 falcon-40b-instruct,46.70807453416149,1.7551420072945083,minimal,4,805,374,427,,662
 alpaca-farm-ppo-human,46.45962732919255,1.750131850347461,minimal,8,805,370,427,,803
 pythia-12b-mix-sft,43.22981366459627,1.7449120766669366,verified,2,805,347,456,,913
```

### Comparing `alpaca_eval-0.2.3/src/alpaca_eval/leaderboards/evaluators/evaluators_leaderboard.csv` & `alpaca_eval-0.2.4/src/alpaca_eval/leaderboards/evaluators/evaluators_leaderboard.csv`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.3/src/alpaca_eval/main.py` & `alpaca_eval-0.2.4/src/alpaca_eval/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
         The path the (or list of dict of) the annotator's config file. For details see the docstring of
         `PairwiseAnnotator`.
 
     name : str, optional
         The name of the model to add to the leaderboard. If None we check if `generator is in model_outputs` if not
         we use "Current model".
 
-    output_path : bool, optional
+    output_path : path, optional
         Path to the directory where the new leaderboard and the annotations should be stored. If None we don't save.
         If `auto` we use `model_outputs` if it is a path, and otherwise use the directory from which we call the script.
 
     precomputed_leaderboard : path or data, optional
         The precomputed leaderboard or a path to it (json, csv, or tsv). The leaderboard should contain at least the
         column `win_rate`. If `auto` we will try to use the corresponding leaderboard for the reference outputs (only if
         in CORRESPONDING_OUTPUTS_LEADERBOARDS). If `None` we won't add other models from the leaderboard.
```

### Comparing `alpaca_eval-0.2.3/src/alpaca_eval/metrics.py` & `alpaca_eval-0.2.4/src/alpaca_eval/metrics.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.3/src/alpaca_eval/plotting.py` & `alpaca_eval-0.2.4/src/alpaca_eval/plotting.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.3/src/alpaca_eval/utils.py` & `alpaca_eval-0.2.4/src/alpaca_eval/utils.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.3/src/alpaca_eval.egg-info/PKG-INFO` & `alpaca_eval-0.2.4/src/alpaca_eval.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alpaca-eval
-Version: 0.2.3
+Version: 0.2.4
 Summary: AlpacaEval : An Automatic Evaluator of Instruction-following Models
 Author: The Alpaca Team
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -113,15 +113,15 @@
 
 ```bash
 export OPENAI_API_KEY=<your_api_key>
 export OPENAI_ORGANIZATION_IDS=<your_organization_id>  # Optional; if not set, this will be your default org id.
 alpaca_eval --model_outputs 'example/outputs.json' 
 ```
 
-Important parameters are the following:
+This will print the leaderboard to the console, and save both the leaderboard and the annotations to the same directory as the `model_outputs` file. Important parameters are the following:
 
 - **model_outputs** : A path to a json file for the outputs of the model to add to the leaderboard. Each dictionary
   should
   contain the keys `instruction` and `output`.
 - **annotators_config**: This is the annotator to use (e.g., `alpaca_eval_gpt4` or `claude`
   or `chatgpt_fn`). `alpaca_eval_gpt4` (
   default) has the
@@ -1057,14 +1057,29 @@
 ```
 
 After running this command, you should have generated an outputs json and a new entry in the corresponding [leaderboard
 file](https://github.com/tatsu-lab/alpaca_eval/tree/main/src/alpaca_eval/leaderboards/data_AlpacaEval). Please make a PR
 with the
 config, outputs file, and updated leaderboard.
 
+Concretely you should do something like:
+
+1. Fork the repository in github
+2. Clone the forked repository `git clone <URL>`
+3. Make a model config at `src/alpaca_eval/models_configs/<model_name>` and evaluate it `evaluate_from_model --model_configs '<model_name>'`
+4. Add the model configs, output, and leaderboard entry to the forked repository
+```sh
+git add src/alpaca_eval/models_configs/<model_name>
+git add src/alpaca_eval/leaderboards/data_AlpacaEval
+git add results/<model_name>/model_outputs.json
+git commit -m "Add <model_name> to AlpacaEval"
+git push
+``` 
+5. Create a [pull request on AlpacaEval](https://github.com/tatsu-lab/alpaca_eval/pulls)
+
 </details>
 
 <details>
   <summary><h2 tabindex="-1" dir="auto">Contributing an evaluator</h2></summary>
 
 Please first follow the directions in [Making a new evaluator](#making-a-new-evaluator).
 Once you're created the annotator config, we ask that you create a new leaderboard for the annotator by evaluating the
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: alpaca-eval Version: 0.2.3 Summary: AlpacaEval : An
+Metadata-Version: 2.1 Name: alpaca-eval Version: 0.2.4 Summary: AlpacaEval : An
 Automatic Evaluator of Instruction-following Models Author: The Alpaca Team
 Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
 Education Classifier: Intended Audience :: Science/Research Classifier: License
 :: OSI Approved :: Apache Software License Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
 Python :: 3.12 Classifier: Topic :: Scientific/Engineering :: Artificial
@@ -69,23 +69,25 @@
 Release](#data-release) - [Differences with AlpacaFarm](#differences-with-
 alpacafarm) - [Related work](#related-work) - [Major updates](#major-updates)
 # Quick Start To install the stable release, run ```bash pip install alpaca-
 eval ``` To install the nightly version, run ```bash pip install git+https://
 github.com/tatsu-lab/alpaca_eval ``` Then you can use it as follows: ```bash
 export OPENAI_API_KEY= export OPENAI_ORGANIZATION_IDS= # Optional; if not set,
 this will be your default org id. alpaca_eval --model_outputs 'example/
-outputs.json' ``` Important parameters are the following: - **model_outputs** :
-A path to a json file for the outputs of the model to add to the leaderboard.
-Each dictionary should contain the keys `instruction` and `output`. -
-**annotators_config**: This is the annotator to use (e.g., `alpaca_eval_gpt4`
-or `claude` or `chatgpt_fn`). `alpaca_eval_gpt4` ( default) has the highest
-agreement rate with our human annotation data. `claude` has a decent agreement
-and is free for academics. `chatgpt_fn` is the worst of the three, but is
-available to everyone, cheap, and has 2x larger context window (16K tokens).
-For a comparison of annotators see [here](#evaluators). -
+outputs.json' ``` This will print the leaderboard to the console, and save both
+the leaderboard and the annotations to the same directory as the
+`model_outputs` file. Important parameters are the following: -
+**model_outputs** : A path to a json file for the outputs of the model to add
+to the leaderboard. Each dictionary should contain the keys `instruction` and
+`output`. - **annotators_config**: This is the annotator to use (e.g.,
+`alpaca_eval_gpt4` or `claude` or `chatgpt_fn`). `alpaca_eval_gpt4` ( default)
+has the highest agreement rate with our human annotation data. `claude` has a
+decent agreement and is free for academics. `chatgpt_fn` is the worst of the
+three, but is available to everyone, cheap, and has 2x larger context window
+(16K tokens). For a comparison of annotators see [here](#evaluators). -
 **reference_outputs**: The outputs of the reference model. Same format as
 `model_outputs`. By default, this is `text-davinci003` outputs on AlpacaEval
 dataset. - **output_path**: Path for saving annotations and leaderboard. If you
 don't have the model outputs, you can use [`evaluate_from_model`](https://
 github.com/tatsu-lab/alpaca_eval/tree/main#evaluating-a-model) and pass a local
 path or a name of a HuggingFace model, or a model from a standard API (OpenAI,
 Anthropic, Cohere). Other commands:  >>> alpaca_eval -- --help ``` SYNOPSIS
@@ -619,15 +621,23 @@
 model) to run inference on the model to produce outputs on the eval set and
 score the model according to one of the evaluators. An example command may look
 like: ```sh alpaca_eval evaluate_from_model \ --model_configs 'falcon-7b-
 instruct' \ --annotators_config 'alpaca_eval_gpt4' ``` After running this
 command, you should have generated an outputs json and a new entry in the
 corresponding [leaderboard file](https://github.com/tatsu-lab/alpaca_eval/tree/
 main/src/alpaca_eval/leaderboards/data_AlpacaEval). Please make a PR with the
-config, outputs file, and updated leaderboard.
+config, outputs file, and updated leaderboard. Concretely you should do
+something like: 1. Fork the repository in github 2. Clone the forked repository
+`git clone ` 3. Make a model config at `src/alpaca_eval/models_configs/` and
+evaluate it `evaluate_from_model --model_configs ''` 4. Add the model configs,
+output, and leaderboard entry to the forked repository ```sh git add src/
+alpaca_eval/models_configs/ git add src/alpaca_eval/leaderboards/
+data_AlpacaEval git add results//model_outputs.json git commit -m "Add  to
+AlpacaEval" git push ``` 5. Create a [pull request on AlpacaEval](https://
+github.com/tatsu-lab/alpaca_eval/pulls)
 ***** Contributing an evaluator *****
 Please first follow the directions in [Making a new evaluator](#making-a-new-
 evaluator). Once you're created the annotator config, we ask that you create a
 new leaderboard for the annotator by evaluating the minimal set of models. The
 outputs for these models can be found by downloading
 [alpaca_eval_all_outputs.json](https://huggingface.co/datasets/tatsu-lab/
 alpaca_eval/blob/main/alpaca_eval_all_outputs.json). ```bash alpaca_eval
```

### Comparing `alpaca_eval-0.2.3/src/alpaca_eval.egg-info/SOURCES.txt` & `alpaca_eval-0.2.4/src/alpaca_eval.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 src/alpaca_eval/annotators/pairwise_evaluator.py
 src/alpaca_eval/decoders/__init__.py
 src/alpaca_eval/decoders/anthropic.py
 src/alpaca_eval/decoders/cohere.py
 src/alpaca_eval/decoders/huggingface_api.py
 src/alpaca_eval/decoders/huggingface_local.py
 src/alpaca_eval/decoders/openai.py
+src/alpaca_eval/decoders/replicate.py
 src/alpaca_eval/evaluators_configs/README.md
 src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4/alpaca_eval.txt
 src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4/configs.yaml
 src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4_fn/alpaca_eval_fn.txt
 src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4_fn/configs.yaml
 src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_chat_v0_without_inputs.txt
 src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_chat_without_inputs.txt
@@ -79,17 +80,21 @@
 src/alpaca_eval/models_configs/airoboros-33b/configs.yaml
 src/alpaca_eval/models_configs/airoboros-33b/prompt.txt
 src/alpaca_eval/models_configs/airoboros-65b/configs.yaml
 src/alpaca_eval/models_configs/alpaca-7b/configs.yaml
 src/alpaca_eval/models_configs/alpaca-7b/prompt.txt
 src/alpaca_eval/models_configs/alpaca-farm-ppo-human/configs.yaml
 src/alpaca_eval/models_configs/alpaca-farm-ppo-sim-gpt4-20k/configs.yaml
+src/alpaca_eval/models_configs/baichuan-13b-chat/configs.yaml
+src/alpaca_eval/models_configs/baichuan-13b-chat/prompt.txt
 src/alpaca_eval/models_configs/baize-v2-13b/configs.yaml
 src/alpaca_eval/models_configs/baize-v2-13b/prompt.txt
 src/alpaca_eval/models_configs/baize-v2-7b/configs.yaml
+src/alpaca_eval/models_configs/chatglm2-6b/configs.yaml
+src/alpaca_eval/models_configs/chatglm2-6b/prompt.txt
 src/alpaca_eval/models_configs/chatgpt/configs.yaml
 src/alpaca_eval/models_configs/claude/configs.yaml
 src/alpaca_eval/models_configs/claude/prompt.txt
 src/alpaca_eval/models_configs/claude-2/configs.yaml
 src/alpaca_eval/models_configs/cohere/configs.yaml
 src/alpaca_eval/models_configs/cohere/prompt.txt
 src/alpaca_eval/models_configs/cohere-chat/configs.yaml
@@ -98,14 +103,22 @@
 src/alpaca_eval/models_configs/gpt4/chatml_prompt.txt
 src/alpaca_eval/models_configs/gpt4/configs.yaml
 src/alpaca_eval/models_configs/guanaco-13b/configs.yaml
 src/alpaca_eval/models_configs/guanaco-33b/configs.yaml
 src/alpaca_eval/models_configs/guanaco-65b/configs.yaml
 src/alpaca_eval/models_configs/guanaco-7b/configs.yaml
 src/alpaca_eval/models_configs/guanaco-7b/prompt.txt
+src/alpaca_eval/models_configs/llama-2-13b-chat-hf/configs.yaml
+src/alpaca_eval/models_configs/llama-2-70b-chat-hf/configs.yaml
+src/alpaca_eval/models_configs/llama-2-70b-chat-hf-replicate/configs.yaml
+src/alpaca_eval/models_configs/llama-2-70b-chat-hf-replicate/prompt.txt
+src/alpaca_eval/models_configs/llama-2-70b-chat-hf-replicate-noprompt/configs.yaml
+src/alpaca_eval/models_configs/llama-2-70b-chat-hf-replicate-noprompt/prompt.txt
+src/alpaca_eval/models_configs/llama-2-7b-chat-hf/configs.yaml
+src/alpaca_eval/models_configs/llama-2-7b-chat-hf/prompt.txt
 src/alpaca_eval/models_configs/minotaur-13b/configs.yaml
 src/alpaca_eval/models_configs/minotaur-13b/prompt.txt
 src/alpaca_eval/models_configs/nous-hermes-13b/configs.yaml
 src/alpaca_eval/models_configs/nous-hermes-13b/prompt.txt
 src/alpaca_eval/models_configs/oasst-rlhf-llama-33b/configs.yaml
 src/alpaca_eval/models_configs/oasst-sft-llama-33b/configs.yaml
 src/alpaca_eval/models_configs/oasst-sft-llama-33b/prompt.txt
```

### Comparing `alpaca_eval-0.2.3/src/alpaca_eval.egg-info/requires.txt` & `alpaca_eval-0.2.4/src/alpaca_eval.egg-info/requires.txt`

 * *Files 21% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 peft
 optimum
 scipy
 einops
 anthropic>=0.3.3
 huggingface_hub
 cohere
+replicate
 seaborn
 matplotlib
 jupyterlab
 pre-commit>=3.2.0
 black>=23.1.0
 isort
 pytest
@@ -33,14 +34,15 @@
 matplotlib
 jupyterlab
 
 [api]
 anthropic>=0.3.3
 huggingface_hub
 cohere
+replicate
 
 [dev]
 pre-commit>=3.2.0
 black>=23.1.0
 isort
 pytest
 pytest-mock
```

### Comparing `alpaca_eval-0.2.3/tests/test_analyze.py` & `alpaca_eval-0.2.4/tests/test_analyze.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.3/tests/test_decoders_unit.py` & `alpaca_eval-0.2.4/tests/test_decoders_unit.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.3/tests/test_main.py` & `alpaca_eval-0.2.4/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.3/tests/test_pairwise_evaluator.py` & `alpaca_eval-0.2.4/tests/test_pairwise_evaluator.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,30 +52,30 @@
         is_randomize_output_order=False,
         is_shuffle=False,
     )
 
 
 def test_single_annotator(single_annotator, df_to_annotate):
     # Create a sample DataFrame for testing
-
-    single_annotator.fn_completions = MagicMock(
-        return_value={"completions": ["Output (a)", "Output (b)", "not parsable"]}
-    )
+    parsable_completions = ["Output (a)", "Output (b)"]
+    completions = parsable_completions + ["not parsable"]  # add an example that can't be parsed
+    single_annotator.fn_completions = MagicMock(return_value={"completions": completions})
+    # set a completion_column => store it
+    single_annotator.completion_column = "completions"
 
     # Call the preprocess method
     df_annotated = single_annotator(df_to_annotate)
 
     assert df_annotated["preference"].tolist() == [1, 2]
     assert df_annotated["instruction"].tolist() == ["2+2", "1+1"]
-    assert df_annotated.columns.tolist() == [
-        "instruction",
-        "output_1",
-        "output_2",
-        "preference",
-    ]
+    assert set(df_annotated.columns.tolist()) == set(
+        ["instruction", "output_1", "output_2", "preference", "completions"]
+    )
+    # check that you also save the completions.
+    assert df_annotated["completions"].tolist() == parsable_completions
 
 
 @pytest.fixture
 def pairwise_annotator(tmp_path):
     return PairwiseAnnotator(
         annotators_config="text_davinci_003",
         caching_path=tmp_path / "cache_{seed}.json",
```

