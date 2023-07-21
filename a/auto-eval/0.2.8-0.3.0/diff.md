# Comparing `tmp/auto-eval-0.2.8.tar.gz` & `tmp/auto-eval-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto-eval-0.2.8.tar", last modified: Thu Jun 29 07:44:40 2023, max compression
+gzip compressed data, was "auto-eval-0.3.0.tar", last modified: Fri Jul 21 10:57:34 2023, max compression
```

## Comparing `auto-eval-0.2.8.tar` & `auto-eval-0.3.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-06-29 07:44:40.326116 auto-eval-0.2.8/
--rw-r--r--   0 zhangchong   (501) staff       (20)     1071 2023-04-28 07:53:45.000000 auto-eval-0.2.8/LICENSE
--rw-r--r--   0 zhangchong   (501) staff       (20)    16509 2023-06-29 07:44:40.325723 auto-eval-0.2.8/PKG-INFO
--rw-r--r--   0 zhangchong   (501) staff       (20)    16083 2023-06-07 06:25:31.000000 auto-eval-0.2.8/README.md
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-06-29 07:44:40.322790 auto-eval-0.2.8/auto_eval.egg-info/
--rw-r--r--   0 zhangchong   (501) staff       (20)    16509 2023-06-29 07:44:40.000000 auto-eval-0.2.8/auto_eval.egg-info/PKG-INFO
--rw-r--r--   0 zhangchong   (501) staff       (20)      465 2023-06-29 07:44:40.000000 auto-eval-0.2.8/auto_eval.egg-info/SOURCES.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)        1 2023-06-29 07:44:40.000000 auto-eval-0.2.8/auto_eval.egg-info/dependency_links.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)       59 2023-06-29 07:44:40.000000 auto-eval-0.2.8/auto_eval.egg-info/entry_points.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)       49 2023-06-29 07:44:40.000000 auto-eval-0.2.8/auto_eval.egg-info/requires.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)        5 2023-06-29 07:44:40.000000 auto-eval-0.2.8/auto_eval.egg-info/top_level.txt
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-06-29 07:44:40.323333 auto-eval-0.2.8/eval/
--rw-r--r--   0 zhangchong   (501) staff       (20)      136 2023-05-08 07:54:51.000000 auto-eval-0.2.8/eval/__init__.py
--rw-r--r--   0 zhangchong   (501) staff       (20)    10360 2023-06-06 12:00:40.000000 auto-eval-0.2.8/eval/auto_llms_eval.py
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-06-29 07:44:40.324002 auto-eval-0.2.8/eval/commands/
--rw-r--r--   0 zhangchong   (501) staff       (20)        0 2023-04-28 08:32:15.000000 auto-eval-0.2.8/eval/commands/__init__.py
--rw-r--r--   0 zhangchong   (501) staff       (20)     6088 2023-06-06 11:35:46.000000 auto-eval-0.2.8/eval/commands/auto_eval.py
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-06-29 07:44:40.325067 auto-eval-0.2.8/eval/prompt_template/
--rw-r--r--   0 zhangchong   (501) staff       (20)      198 2023-05-19 08:23:31.000000 auto-eval-0.2.8/eval/prompt_template/__init__.py
--rw-r--r--   0 zhangchong   (501) staff       (20)     3094 2023-06-27 06:27:16.000000 auto-eval-0.2.8/eval/prompt_template/prompter.py
--rw-r--r--   0 zhangchong   (501) staff       (20)     2646 2023-06-28 02:43:09.000000 auto-eval-0.2.8/eval/prompt_template/prompts.py
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-06-29 07:44:40.325493 auto-eval-0.2.8/eval/utils/
--rw-r--r--   0 zhangchong   (501) staff       (20)       26 2023-04-28 09:40:19.000000 auto-eval-0.2.8/eval/utils/__init__.py
--rw-r--r--   0 zhangchong   (501) staff       (20)     4197 2023-06-29 07:42:59.000000 auto-eval-0.2.8/eval/utils/data_utils.py
--rw-r--r--   0 zhangchong   (501) staff       (20)       38 2023-06-29 07:44:40.326206 auto-eval-0.2.8/setup.cfg
--rw-r--r--   0 zhangchong   (501) staff       (20)      956 2023-06-29 07:44:30.000000 auto-eval-0.2.8/setup.py
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-07-21 10:57:34.295325 auto-eval-0.3.0/
+-rw-r--r--   0 zhangchong   (501) staff       (20)     1071 2023-04-28 07:53:45.000000 auto-eval-0.3.0/LICENSE
+-rw-r--r--   0 zhangchong   (501) staff       (20)    16509 2023-07-21 10:57:34.295078 auto-eval-0.3.0/PKG-INFO
+-rw-r--r--   0 zhangchong   (501) staff       (20)    16083 2023-06-07 06:25:31.000000 auto-eval-0.3.0/README.md
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-07-21 10:57:34.291531 auto-eval-0.3.0/auto_eval.egg-info/
+-rw-r--r--   0 zhangchong   (501) staff       (20)    16509 2023-07-21 10:57:34.000000 auto-eval-0.3.0/auto_eval.egg-info/PKG-INFO
+-rw-r--r--   0 zhangchong   (501) staff       (20)      465 2023-07-21 10:57:34.000000 auto-eval-0.3.0/auto_eval.egg-info/SOURCES.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)        1 2023-07-21 10:57:34.000000 auto-eval-0.3.0/auto_eval.egg-info/dependency_links.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)       59 2023-07-21 10:57:34.000000 auto-eval-0.3.0/auto_eval.egg-info/entry_points.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)       49 2023-07-21 10:57:34.000000 auto-eval-0.3.0/auto_eval.egg-info/requires.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)        5 2023-07-21 10:57:34.000000 auto-eval-0.3.0/auto_eval.egg-info/top_level.txt
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-07-21 10:57:34.291978 auto-eval-0.3.0/eval/
+-rw-r--r--   0 zhangchong   (501) staff       (20)      136 2023-05-08 07:54:51.000000 auto-eval-0.3.0/eval/__init__.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)    14793 2023-07-21 10:50:50.000000 auto-eval-0.3.0/eval/auto_llms_eval.py
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-07-21 10:57:34.292532 auto-eval-0.3.0/eval/commands/
+-rw-r--r--   0 zhangchong   (501) staff       (20)        0 2023-04-28 08:32:15.000000 auto-eval-0.3.0/eval/commands/__init__.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)     6144 2023-07-21 06:55:27.000000 auto-eval-0.3.0/eval/commands/auto_eval.py
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-07-21 10:57:34.293941 auto-eval-0.3.0/eval/prompt_template/
+-rw-r--r--   0 zhangchong   (501) staff       (20)      198 2023-05-19 08:23:31.000000 auto-eval-0.3.0/eval/prompt_template/__init__.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)     3094 2023-06-27 06:27:16.000000 auto-eval-0.3.0/eval/prompt_template/prompter.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)     2646 2023-06-28 02:43:09.000000 auto-eval-0.3.0/eval/prompt_template/prompts.py
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-07-21 10:57:34.294697 auto-eval-0.3.0/eval/utils/
+-rw-r--r--   0 zhangchong   (501) staff       (20)       26 2023-04-28 09:40:19.000000 auto-eval-0.3.0/eval/utils/__init__.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)     4197 2023-06-29 07:42:59.000000 auto-eval-0.3.0/eval/utils/data_utils.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)       38 2023-07-21 10:57:34.295400 auto-eval-0.3.0/setup.cfg
+-rw-r--r--   0 zhangchong   (501) staff       (20)      956 2023-07-21 10:51:03.000000 auto-eval-0.3.0/setup.py
```

### Comparing `auto-eval-0.2.8/LICENSE` & `auto-eval-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `auto-eval-0.2.8/PKG-INFO` & `auto-eval-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-eval
-Version: 0.2.8
+Version: 0.3.0
 Summary: Using only one line of commmands to evaluate multiple models
 Home-page: https://github.com/muximus3/Auto-Eval
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `auto-eval-0.2.8/README.md` & `auto-eval-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `auto-eval-0.2.8/auto_eval.egg-info/PKG-INFO` & `auto-eval-0.3.0/auto_eval.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-eval
-Version: 0.2.8
+Version: 0.3.0
 Summary: Using only one line of commmands to evaluate multiple models
 Home-page: https://github.com/muximus3/Auto-Eval
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `auto-eval-0.2.8/eval/auto_llms_eval.py` & `auto-eval-0.3.0/eval/auto_llms_eval.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,17 +2,21 @@
 import os
 import pandas as pd
 import traceback
 from typing import Union, List
 import random
 from tqdm import tqdm
 from typing import Optional, Tuple
+import numpy as np
 import time
 import sys
 from dataclasses import dataclass
+import aiohttp
+import asyncio
+import openai
 from oneapi import OneAPITool
 sys.path.append(os.path.normpath(f'{os.path.dirname(os.path.abspath(__file__))}/..'))
 from eval.utils import df_saver, df_reader, binary_cross_entropy
 from eval.prompt_template import Prompter
 
 
 def eval_one_qa(
@@ -21,28 +25,59 @@
              question: str,
              candidate_answers: List[str],
              target: Union[str, None]='',
              engine: str='',
              temperature=0.1,
              max_new_tokens=2048) -> Tuple[Union[List[float], None], str]:
     raw_response = ''
+    shuffle_index = list(range(len(candidate_answers)))
+    np.random.shuffle(shuffle_index)
+    shuffle_answers = [candidate_answers[i] for i in shuffle_index]
     eval_prompt = eval_prompter.generate_prompt(question, target,
-                                                candidate_answers)
+                                                shuffle_answers)
     try:
         raw_response = api_tool.simple_chat(eval_prompt,
                                       model=engine,
                                       temperature=temperature,
-                                      max_new_tokens=max_new_tokens)
+                                      max_new_tokens=max_new_tokens, stream=False)
         scores = eval_prompter.extract_result_from_response(raw_response)
+        scores = [scores[shuffle_index.index(i)] for i in range(len(scores))]
         return scores, raw_response
     except Exception as e:
         print(f'error, request result:{raw_response}, exception:{e}')
         traceback.print_exc()
         return None, raw_response
 
+async def aeval_one_qa(
+             api_tool: OneAPITool,
+             eval_prompter: Prompter,
+             question: str,
+             candidate_answers: List[str],
+             target: Union[str, None]='',
+             engine: str='',
+             temperature=0.1,
+             max_new_tokens=2048) -> Tuple[Union[List[float], None], str]:
+    raw_response = ''
+    shuffle_index = list(range(len(candidate_answers)))
+    np.random.shuffle(shuffle_index)
+    shuffle_answers = [candidate_answers[i] for i in shuffle_index]
+    eval_prompt = eval_prompter.generate_prompt(question, target,
+                                                shuffle_answers)
+    try:
+        raw_response = await api_tool.asimple_chat(eval_prompt,
+                                      model=engine,
+                                      temperature=temperature,
+                                      max_new_tokens=max_new_tokens)
+        scores = eval_prompter.extract_result_from_response(raw_response)
+        scores = [scores[shuffle_index.index(i)] for i in range(len(scores))]
+        return scores, raw_response
+    except Exception as e:
+        print(f'error, request result:{raw_response}, exception:{e}')
+        traceback.print_exc()
+        return None, raw_response
 
 def eval_one_group(
     api_tool: OneAPITool,
     eval_prompter: Prompter,
     data_group: pd.DataFrame,
     engine: str,
     temperature=0.1,
@@ -67,14 +102,46 @@
         group.at[0, 'raw_response'] = raw_response
         for i in range(len(scores)):
             group.at[i, 'score'] = scores[i]
         return group
     else:
         return None
 
+        
+async def aeval_one_group(
+    api_tool: OneAPITool,
+    eval_prompter: Prompter,
+    data_group: pd.DataFrame,
+    engine: str,
+    temperature=0.1,
+    max_new_tokens=2048,
+) -> Union[pd.DataFrame, None]:
+    group = data_group.reset_index(drop=True)
+    question = group['question'].unique()[0]
+    candidate_answers = group['output']
+    if 'target' in data_group.keys():
+        target = group['target'].unique()[0]
+    else:
+        target = ''
+    scores, raw_response = await aeval_one_qa(api_tool=api_tool,
+                      eval_prompter=eval_prompter,
+                      question=question,
+                      candidate_answers=candidate_answers,
+                      target=target,
+                      engine=engine,
+                      temperature=temperature,
+                      max_new_tokens=max_new_tokens)
+    if scores is not None and len(scores) == len(candidate_answers):
+        group.at[0, 'raw_response'] = raw_response
+        for i in range(len(scores)):
+            group.at[i, 'score'] = scores[i]
+        return group
+    else:
+        return None
+
 
 
 def prepare_eval_data(
     eval_data_path: List[str],
     eval_categories: Optional[List[str]] = None, 
     question_column_names: Optional[List[str]] = None,
     answer_column_names: Optional[List[str]] = None,
@@ -177,15 +244,15 @@
 def save_results(results_df: pd.DataFrame, output_path: str):
     print(f'Saving evaluation results: {output_path}')
     df_saver(results_df, output_path)
     print(f'Saved successfully.')
 
 @dataclass
 class EvalConfig:
-    api_config_file: str
+    api_config_files: str
     eval_prompter: Prompter
     eval_data_path: str
     question_column_names: Optional[List[str]] = None
     answer_column_names: Optional[List[str]] = None
     output_path: str = ''
     engine: str = ''
     eval_categories: Optional[List[str]] = None
@@ -199,39 +266,78 @@
 
 def eval_groups(
     eval_config: EvalConfig
 ):
     # Preparing data
     scored_groups, unscored_groups = prepare_eval_data(eval_config.eval_data_path, eval_config.eval_categories, eval_config.question_column_names, eval_config.answer_column_names, eval_config.sample_num, eval_config.eval_models)
 
+    process_num = len(eval_config.api_config_files)
     # Init api tool and prompter
-    tool = OneAPITool.from_config_file(config_file=eval_config.api_config_file)
-
-    failed_groups = []
-    for group in tqdm(unscored_groups):
-        result = eval_one_group(tool, eval_config.eval_prompter,  group,  eval_config.engine, eval_config.temperature, eval_config.max_new_tokens)
-        if result is not None:
-            scored_groups.append(result)
-        else:
-            failed_groups.append(group)
-        time.sleep(eval_config.request_interval)
-
-    # Retry failed requests
-    if len(failed_groups) > 0 and eval_config.retry:
-        for group in tqdm(failed_groups.copy(), desc='RETRY'):
+    if process_num == 1:
+        failed_groups = []
+        tool = OneAPITool.from_config_file(eval_config.api_config_files[0])
+        for group in tqdm(unscored_groups):
             result = eval_one_group(tool, eval_config.eval_prompter,  group,  eval_config.engine, eval_config.temperature, eval_config.max_new_tokens)
             if result is not None:
                 scored_groups.append(result)
-                failed_groups = [df for df in failed_groups if not df.equals(group)]
+            else:
+                failed_groups.append(group)
             time.sleep(eval_config.request_interval)
 
+        # Retry failed requests
+        if len(failed_groups) > 0 and eval_config.retry:
+            for group in tqdm(failed_groups.copy(), desc='RETRY'):
+                result = eval_one_group(tool, eval_config.eval_prompter,  group,  eval_config.engine, eval_config.temperature, eval_config.max_new_tokens)
+                if result is not None:
+                    scored_groups.append(result)
+                    failed_groups = [df for df in failed_groups if not df.equals(group)]
+                time.sleep(eval_config.request_interval)
+    else:
+        score_results = asyncio.run(aeval_groups(eval_config, unscored_groups))
+        failed_groups = []
+        for result in score_results:
+            if result is not None:
+                scored_groups.append(result)
+            else:
+                failed_groups.append(result)
+        # Retry failed requests
+        if len(failed_groups) > 0 and eval_config.retry:
+            score_results = asyncio.run(aeval_groups(eval_config, failed_groups))
+            for result in score_results:
+                if result is not None:
+                    scored_groups.append(result)
+                    failed_groups = [df for df in failed_groups if not df.equals(result)]
+
     scored_results_df = pd.concat(scored_groups)
     log_score_results(eval_results_df=scored_results_df, score_by=eval_config.score_by)
     log_eval_prompt_scores_loss(eval_results_df=scored_results_df)
     # Log score results
     print(f'Eval engine: {eval_config.engine}')
     print(f'Eval files: {eval_config.eval_data_path}')
     print(f'Failed requests: {len(failed_groups)}/{len(scored_groups) + len(failed_groups)}')
     results_df = pd.concat([scored_results_df, pd.concat(failed_groups)]) if len(failed_groups) > 0 else scored_results_df
     # Save results
     if eval_config.output_path:
         save_results(results_df=results_df, output_path=eval_config.output_path)
+
+
+
+async def bound_fetch(sem, pbar,*params, **kwargs):
+    async with sem:
+        result = await aeval_one_group(*params, **kwargs)
+        pbar.update(1)
+        return result
+
+async def aeval_groups(eval_config: EvalConfig, unscored_groups: List[pd.DataFrame]):
+    # Preparing data
+    process_num = len(eval_config.api_config_files)
+    pbar = tqdm(total=len(unscored_groups))
+    sem = asyncio.Semaphore(process_num)
+    async with aiohttp.ClientSession() as session:
+        openai.aiosession.set(session)
+        tools = [OneAPITool.from_config_file(config_file) for config_file in eval_config.api_config_files]
+        tasks = [asyncio.ensure_future(bound_fetch(sem, pbar, tools[i%process_num], eval_config.eval_prompter,  group,  eval_config.engine, eval_config.temperature, eval_config.max_new_tokens)) for i, group in enumerate(unscored_groups)]
+        results = await asyncio.gather(*tasks)
+    return results
+
+
+
```

### Comparing `auto-eval-0.2.8/eval/commands/auto_eval.py` & `auto-eval-0.3.0/eval/commands/auto_eval.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,19 @@
 from eval.prompt_template import prompter, prompts
 from eval.utils.data_utils import df_reader
 from eval.auto_llms_eval import eval_one_group, eval_one_qa, eval_groups, EvalConfig
 
 
 def add_shared_arguments(parser):
     parser.add_argument(
-        "-c", "--config_file", type=str, help="config file path", required=True
+        "-c", "--config_files",
+        default=None,
+        nargs="+", 
+        help="config file path", 
+        required=True
     )
     parser.add_argument(
         "-tp",
         "--template_path",
         type=str,
         default=None,
         help="eval prompt template path",
@@ -151,15 +155,15 @@
     else:
         if args.template_type in ['ec', 'e_commerce']:
             eval_prompter = prompter.EvalPrompter(prompts.EVAL_WITH_TARGET_TEMPLATE_ECOMMERCE, prompts.EVAL_WITHOUT_TARGET_TEMPLATE_ECOMMERCE, args.verbose)
         else:
             eval_prompter = prompter.EvalPrompter(prompts.EVAL_WITH_TARGET_TEMPLATE, prompts.EVAL_WITHOUT_TARGET_TEMPLATE, args.verbose)
 
     if args.command == "line":
-        tool = OneAPITool.from_config_file(args.config_file)
+        tool = OneAPITool.from_config_file(args.config_files[0])
         score, raw_response = eval_one_qa(
             api_tool=tool,
             eval_prompter=eval_prompter,
             question=args.prompt,
             candidate_answers=args.answers,
             target=args.target,
             engine=args.model,
@@ -167,15 +171,15 @@
             max_new_tokens=args.max_new_tokens,
         )
         print(f"\nSCORE:\n{score}")
 
     elif args.command == "file":
         eval_groups(
             EvalConfig(
-                api_config_file=args.config_file,
+                api_config_files=args.config_files,
                 eval_prompter=eval_prompter,
                 eval_data_path=args.eval_data_path,
                 question_column_names=args.question_column_names,
                 answer_column_names=args.answer_column_names,
                 output_path=args.output_path,
                 engine=args.model,
                 eval_categories=args.eval_categories,
```

### Comparing `auto-eval-0.2.8/eval/prompt_template/prompter.py` & `auto-eval-0.3.0/eval/prompt_template/prompter.py`

 * *Files identical despite different names*

### Comparing `auto-eval-0.2.8/eval/prompt_template/prompts.py` & `auto-eval-0.3.0/eval/prompt_template/prompts.py`

 * *Files identical despite different names*

### Comparing `auto-eval-0.2.8/eval/utils/data_utils.py` & `auto-eval-0.3.0/eval/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `auto-eval-0.2.8/setup.py` & `auto-eval-0.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="auto-eval",
-    version="0.2.8",
+    version="0.3.0",
     packages=find_packages(),
     # package_data={
     #   "eval":["prompt_template/eval_prompt_template.json"]  
     # },
     install_requires=[
         # Add your library's dependencies here
         "one-api-tool",
```

