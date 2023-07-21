# Comparing `tmp/langkit-0.0.7.tar.gz` & `tmp/langkit-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langkit-0.0.7.tar", max compression
+gzip compressed data, was "langkit-0.0.8.tar", max compression
```

## Comparing `langkit-0.0.7.tar` & `langkit-0.0.8.tar`

### file list

```diff
@@ -1,53 +1,57 @@
--rw-r--r--   0        0        0     3205 2023-07-04 20:10:20.545540 langkit-0.0.7/DESCRIPTION.md
--rw-r--r--   0        0        0    11357 2023-04-27 19:37:47.238351 langkit-0.0.7/LICENSE
--rw-r--r--   0        0        0      998 2023-07-12 19:53:12.139567 langkit-0.0.7/langkit/__init__.py
--rw-r--r--   0        0        0      596 2023-07-06 08:00:05.378422 langkit-0.0.7/langkit/all_metrics.py
--rw-r--r--   0        0        0     7915 2023-07-12 20:36:17.619567 langkit-0.0.7/langkit/callback_handler.py
--rw-r--r--   0        0        0      140 2023-07-04 20:11:04.055540 langkit-0.0.7/langkit/config/__init__.py
--rw-r--r--   0        0        0     1757 2023-07-04 20:11:04.055540 langkit-0.0.7/langkit/config/environment.py
--rw-r--r--   0        0        0     1260 2023-07-04 20:11:04.055540 langkit-0.0.7/langkit/docs/features/quality.md
--rw-r--r--   0        0        0     1801 2023-07-04 20:11:04.055540 langkit-0.0.7/langkit/docs/features/relevance.md
--rw-r--r--   0        0        0     1886 2023-07-04 20:11:04.055540 langkit-0.0.7/langkit/docs/features/security.md
--rw-r--r--   0        0        0     1364 2023-07-04 20:11:04.055540 langkit-0.0.7/langkit/docs/features/sentiment.md
--rw-r--r--   0        0        0    11682 2023-07-04 20:11:04.055540 langkit-0.0.7/langkit/docs/modules.md
--rw-r--r--   0        0        0    11230 2023-07-04 20:11:04.055540 langkit-0.0.7/langkit/examples/Batch_to_Whylabs.ipynb
--rw-r--r--   0        0        0     9709 2023-07-12 20:36:17.619567 langkit-0.0.7/langkit/examples/Intro_to_Langkit.ipynb
--rw-r--r--   0        0        0   262944 2023-07-04 20:11:04.065540 langkit-0.0.7/langkit/examples/LLM_to_WhyLabs.ipynb
--rw-r--r--   0        0        0    11770 2023-07-04 20:11:04.065540 langkit-0.0.7/langkit/examples/Langchain_OpenAI_LLM_Monitoring_with_WhyLabs.ipynb
--rw-r--r--   0        0        0    21888 2023-07-04 20:11:04.065540 langkit-0.0.7/langkit/examples/Logging_Text.ipynb
--rw-r--r--   0        0        0     7126 2023-07-04 20:11:04.065540 langkit-0.0.7/langkit/examples/Sentiment_and_Toxicity.ipynb
--rw-r--r--   0        0        0    17842 2023-07-07 22:52:41.688422 langkit-0.0.7/langkit/examples/tutorials/Safeguarding_and_Monitoring_LLMs.ipynb
--rw-r--r--   0        0        0   109092 2023-07-07 22:52:41.698422 langkit-0.0.7/langkit/examples/tutorials/images/dashboard.png
--rw-r--r--   0        0        0   336393 2023-07-07 22:52:41.698422 langkit-0.0.7/langkit/examples/tutorials/images/safeguards_pipeline.png
--rw-r--r--   0        0        0     1362 2023-07-04 20:11:04.065540 langkit-0.0.7/langkit/injections.py
--rw-r--r--   0        0        0     2210 2023-07-04 20:11:04.065540 langkit-0.0.7/langkit/input_output.py
--rw-r--r--   0        0        0      297 2023-07-04 20:11:04.065540 langkit-0.0.7/langkit/light_metrics.py
--rw-r--r--   0        0        0      730 2023-07-14 23:21:22.918508 langkit-0.0.7/langkit/llm_metrics.py
--rw-r--r--   0        0        0       75 2023-07-04 20:11:04.065540 langkit-0.0.7/langkit/openai/__init__.py
--rw-r--r--   0        0        0     1167 2023-07-04 20:11:04.065540 langkit-0.0.7/langkit/openai/openai.py
--rw-r--r--   0        0        0     1741 2023-07-04 20:11:04.065540 langkit-0.0.7/langkit/openai_wrapper.py
--rw-r--r--   0        0        0      793 2023-07-18 16:31:35.458508 langkit-0.0.7/langkit/pattern_groups.json
--rw-r--r--   0        0        0     2938 2023-07-18 16:31:35.458508 langkit-0.0.7/langkit/regexes.py
--rw-r--r--   0        0        0      943 2023-07-04 20:11:04.065540 langkit-0.0.7/langkit/sentiment.py
--rw-r--r--   0        0        0      998 2023-07-12 20:36:17.619567 langkit-0.0.7/langkit/tests/__init__.py
--rw-r--r--   0        0        0     3970 2023-07-04 20:11:04.065540 langkit-0.0.7/langkit/tests/conftest.py
--rw-r--r--   0        0        0     4407 2023-07-12 20:36:17.619567 langkit-0.0.7/langkit/tests/test_callback_handler.py
--rw-r--r--   0        0        0     1078 2023-07-04 20:11:04.065540 langkit-0.0.7/langkit/tests/test_injections.py
--rw-r--r--   0        0        0     2308 2023-07-04 20:11:04.065540 langkit-0.0.7/langkit/tests/test_input_output.py
--rw-r--r--   0        0        0     2150 2023-07-18 16:31:35.458508 langkit-0.0.7/langkit/tests/test_patterns.py
--rw-r--r--   0        0        0     3658 2023-07-11 19:04:26.469567 langkit-0.0.7/langkit/tests/test_themes.py
--rw-r--r--   0        0        0      798 2023-07-04 20:11:04.065540 langkit-0.0.7/langkit/tests/test_toxicity.py
--rw-r--r--   0        0        0     3742 2023-07-04 20:11:04.065540 langkit-0.0.7/langkit/textstat.py
--rw-r--r--   0        0        0     8939 2023-07-04 20:11:04.065540 langkit-0.0.7/langkit/themes.json
--rw-r--r--   0        0        0      261 2023-07-04 20:11:04.065540 langkit-0.0.7/langkit/themes.json.txt
--rw-r--r--   0        0        0     4220 2023-07-14 23:09:08.118508 langkit-0.0.7/langkit/themes.py
--rw-r--r--   0        0        0      679 2023-07-04 20:11:04.065540 langkit-0.0.7/langkit/topics.py
--rw-r--r--   0        0        0     1305 2023-07-04 20:11:04.065540 langkit-0.0.7/langkit/toxicity.py
--rw-r--r--   0        0        0      144 2023-07-04 20:11:04.065540 langkit-0.0.7/langkit/transformer.py
--rw-r--r--   0        0        0     1159 2023-07-12 20:36:17.619567 langkit-0.0.7/langkit/whylogs/example_utils/guardrails_example_utils.py
--rw-r--r--   0        0        0     6609 2023-07-07 22:52:41.698422 langkit-0.0.7/langkit/whylogs/example_utils/guardrails_llm_schema.py
--rw-r--r--   0        0        0    30472 2023-07-04 20:11:04.075540 langkit-0.0.7/langkit/whylogs/reference_chats.json
--rw-r--r--   0        0        0      474 2023-07-04 20:11:04.075540 langkit-0.0.7/langkit/whylogs/rolling_logger.py
--rw-r--r--   0        0        0      993 2023-07-04 20:11:04.075540 langkit-0.0.7/langkit/whylogs/samples.py
--rw-r--r--   0        0        0      888 2023-07-17 21:19:54.878508 langkit-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     4204 1970-01-01 00:00:00.000000 langkit-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     3205 2023-07-04 20:10:20.545540 langkit-0.0.8/DESCRIPTION.md
+-rw-r--r--   0        0        0    11357 2023-04-27 19:37:47.238351 langkit-0.0.8/LICENSE
+-rw-r--r--   0        0        0     1172 2023-07-21 20:23:56.497422 langkit-0.0.8/langkit/__init__.py
+-rw-r--r--   0        0        0      596 2023-07-06 08:00:05.378422 langkit-0.0.8/langkit/all_metrics.py
+-rw-r--r--   0        0        0     7915 2023-07-21 20:23:39.317422 langkit-0.0.8/langkit/callback_handler.py
+-rw-r--r--   0        0        0      140 2023-07-04 20:11:04.055540 langkit-0.0.8/langkit/config/__init__.py
+-rw-r--r--   0        0        0     1757 2023-07-04 20:11:04.055540 langkit-0.0.8/langkit/config/environment.py
+-rw-r--r--   0        0        0     1260 2023-07-04 20:11:04.055540 langkit-0.0.8/langkit/docs/features/quality.md
+-rw-r--r--   0        0        0     1801 2023-07-04 20:11:04.055540 langkit-0.0.8/langkit/docs/features/relevance.md
+-rw-r--r--   0        0        0     1886 2023-07-04 20:11:04.055540 langkit-0.0.8/langkit/docs/features/security.md
+-rw-r--r--   0        0        0     1364 2023-07-04 20:11:04.055540 langkit-0.0.8/langkit/docs/features/sentiment.md
+-rw-r--r--   0        0        0    13344 2023-07-21 20:23:56.497422 langkit-0.0.8/langkit/docs/modules.md
+-rw-r--r--   0        0        0    11230 2023-07-04 20:11:04.055540 langkit-0.0.8/langkit/examples/Batch_to_Whylabs.ipynb
+-rw-r--r--   0        0        0   247730 2023-07-21 20:23:56.497422 langkit-0.0.8/langkit/examples/ChatGPT_Behavioral_Monitoring.ipynb
+-rw-r--r--   0        0        0     9709 2023-07-18 18:24:21.578508 langkit-0.0.8/langkit/examples/Intro_to_Langkit.ipynb
+-rw-r--r--   0        0        0   262944 2023-07-04 20:11:04.065540 langkit-0.0.8/langkit/examples/LLM_to_WhyLabs.ipynb
+-rw-r--r--   0        0        0    11770 2023-07-04 20:11:04.065540 langkit-0.0.8/langkit/examples/Langchain_OpenAI_LLM_Monitoring_with_WhyLabs.ipynb
+-rw-r--r--   0        0        0    21888 2023-07-04 20:11:04.065540 langkit-0.0.8/langkit/examples/Logging_Text.ipynb
+-rw-r--r--   0        0        0     7126 2023-07-04 20:11:04.065540 langkit-0.0.8/langkit/examples/Sentiment_and_Toxicity.ipynb
+-rw-r--r--   0        0        0    32760 2023-07-21 03:21:01.012440 langkit-0.0.8/langkit/examples/huggingface_langkit_whylabs.ipynb
+-rw-r--r--   0        0        0    17916 2023-07-18 18:26:20.608508 langkit-0.0.8/langkit/examples/tutorials/Safeguarding_and_Monitoring_LLMs.ipynb
+-rw-r--r--   0        0        0   109092 2023-07-07 22:52:41.698422 langkit-0.0.8/langkit/examples/tutorials/images/dashboard.png
+-rw-r--r--   0        0        0   336393 2023-07-07 22:52:41.698422 langkit-0.0.8/langkit/examples/tutorials/images/safeguards_pipeline.png
+-rw-r--r--   0        0        0     1362 2023-07-04 20:11:04.065540 langkit-0.0.8/langkit/injections.py
+-rw-r--r--   0        0        0     2210 2023-07-04 20:11:04.065540 langkit-0.0.8/langkit/input_output.py
+-rw-r--r--   0        0        0      297 2023-07-04 20:11:04.065540 langkit-0.0.8/langkit/light_metrics.py
+-rw-r--r--   0        0        0      730 2023-07-14 23:21:22.918508 langkit-0.0.8/langkit/llm_metrics.py
+-rw-r--r--   0        0        0     1934 2023-07-21 20:23:56.497422 langkit-0.0.8/langkit/nlp_scores.py
+-rw-r--r--   0        0        0       75 2023-07-04 20:11:04.065540 langkit-0.0.8/langkit/openai/__init__.py
+-rw-r--r--   0        0        0     1167 2023-07-04 20:11:04.065540 langkit-0.0.8/langkit/openai/openai.py
+-rw-r--r--   0        0        0     1741 2023-07-04 20:11:04.065540 langkit-0.0.8/langkit/openai_wrapper.py
+-rw-r--r--   0        0        0      807 2023-07-21 03:21:01.012440 langkit-0.0.8/langkit/pattern_groups.json
+-rw-r--r--   0        0        0     3038 2023-07-21 03:21:01.012440 langkit-0.0.8/langkit/regexes.py
+-rw-r--r--   0        0        0      943 2023-07-04 20:11:04.065540 langkit-0.0.8/langkit/sentiment.py
+-rw-r--r--   0        0        0     1172 2023-07-21 20:23:56.497422 langkit-0.0.8/langkit/tests/__init__.py
+-rw-r--r--   0        0        0     3970 2023-07-04 20:11:04.065540 langkit-0.0.8/langkit/tests/conftest.py
+-rw-r--r--   0        0        0     4407 2023-07-18 18:24:21.578508 langkit-0.0.8/langkit/tests/test_callback_handler.py
+-rw-r--r--   0        0        0     1078 2023-07-04 20:11:04.065540 langkit-0.0.8/langkit/tests/test_injections.py
+-rw-r--r--   0        0        0     2308 2023-07-04 20:11:04.065540 langkit-0.0.8/langkit/tests/test_input_output.py
+-rw-r--r--   0        0        0      653 2023-07-21 20:23:56.497422 langkit-0.0.8/langkit/tests/test_nlp_scores.py
+-rw-r--r--   0        0        0     4700 2023-07-21 03:21:01.012440 langkit-0.0.8/langkit/tests/test_patterns.py
+-rw-r--r--   0        0        0     3718 2023-07-18 23:33:02.638508 langkit-0.0.8/langkit/tests/test_themes.py
+-rw-r--r--   0        0        0      798 2023-07-04 20:11:04.065540 langkit-0.0.8/langkit/tests/test_toxicity.py
+-rw-r--r--   0        0        0     3742 2023-07-04 20:11:04.065540 langkit-0.0.8/langkit/textstat.py
+-rw-r--r--   0        0        0     8939 2023-07-04 20:11:04.065540 langkit-0.0.8/langkit/themes.json
+-rw-r--r--   0        0        0      261 2023-07-04 20:11:04.065540 langkit-0.0.8/langkit/themes.json.txt
+-rw-r--r--   0        0        0     4220 2023-07-18 18:24:21.578508 langkit-0.0.8/langkit/themes.py
+-rw-r--r--   0        0        0      679 2023-07-04 20:11:04.065540 langkit-0.0.8/langkit/topics.py
+-rw-r--r--   0        0        0     1305 2023-07-04 20:11:04.065540 langkit-0.0.8/langkit/toxicity.py
+-rw-r--r--   0        0        0      144 2023-07-04 20:11:04.065540 langkit-0.0.8/langkit/transformer.py
+-rw-r--r--   0        0        0     1159 2023-07-18 18:24:21.578508 langkit-0.0.8/langkit/whylogs/example_utils/guardrails_example_utils.py
+-rw-r--r--   0        0        0     6609 2023-07-07 22:52:41.698422 langkit-0.0.8/langkit/whylogs/example_utils/guardrails_llm_schema.py
+-rw-r--r--   0        0        0    30472 2023-07-04 20:11:04.075540 langkit-0.0.8/langkit/whylogs/reference_chats.json
+-rw-r--r--   0        0        0      474 2023-07-04 20:11:04.075540 langkit-0.0.8/langkit/whylogs/rolling_logger.py
+-rw-r--r--   0        0        0      993 2023-07-04 20:11:04.075540 langkit-0.0.8/langkit/whylogs/samples.py
+-rw-r--r--   0        0        0     1118 2023-07-21 20:28:08.227422 langkit-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     4255 1970-01-01 00:00:00.000000 langkit-0.0.8/PKG-INFO
```

### Comparing `langkit-0.0.7/DESCRIPTION.md` & `langkit-0.0.8/DESCRIPTION.md`

 * *Files identical despite different names*

### Comparing `langkit-0.0.7/LICENSE` & `langkit-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `langkit-0.0.7/langkit/__init__.py` & `langkit-0.0.8/langkit/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -18,14 +18,22 @@
             "finance",
             "medical",
             "education",
             "politics",
             "support",
         ]
     )
+    nlp_scores: list = field(
+        default_factory=lambda: [
+            "bleu",
+            "rouge",
+            "meteor",
+        ]
+    )
+    reference_corpus: str = ""
 
 
 def package_version(package: str = __package__) -> str:
     """Calculate version number based on pyproject.toml"""
     try:
         from importlib import metadata
```

### Comparing `langkit-0.0.7/langkit/all_metrics.py` & `langkit-0.0.8/langkit/all_metrics.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.7/langkit/callback_handler.py` & `langkit-0.0.8/langkit/callback_handler.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.7/langkit/config/environment.py` & `langkit-0.0.8/langkit/config/environment.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.7/langkit/docs/features/quality.md` & `langkit-0.0.8/langkit/docs/features/quality.md`

 * *Files identical despite different names*

### Comparing `langkit-0.0.7/langkit/docs/features/relevance.md` & `langkit-0.0.8/langkit/docs/features/relevance.md`

 * *Files identical despite different names*

### Comparing `langkit-0.0.7/langkit/docs/features/security.md` & `langkit-0.0.8/langkit/docs/features/security.md`

 * *Files identical despite different names*

### Comparing `langkit-0.0.7/langkit/docs/features/sentiment.md` & `langkit-0.0.8/langkit/docs/features/sentiment.md`

 * *Files identical despite different names*

### Comparing `langkit-0.0.7/langkit/docs/modules.md` & `langkit-0.0.8/langkit/docs/modules.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 # Modules List
 
-- [Injections](#injections)
-- [Input/Output](#inputoutput)
-- [Regexes](#regexes)
-- [Sentiment](#sentiment)
-- [Text Statistics](#text-statistics)
-- [Themes](#themes)
-- [Topics](#topics)
-- [Toxicity](#toxicity)
+|             **Module**              |                               **Description**                               | **Target**          |            **Notes**             |
+| :---------------------------------: | :-------------------------------------------------------------------------: | ------------------- | :------------------------------: |
+|      [Injections](#injections)      |                   Prompt injection classification scores                    | Prompt              |                                  |
+|    [Input/Output](#inputoutput)     |               Semantic similarity between prompt and response               | Prompt and Response |        Default llm metric        |
+|         [Regexes](#regexes)         |              Regex pattern matching for sensitive information               | Any string column   | Default llm metric, light-weight |
+|       [Sentiment](#sentiment)       |                             Sentiment Analysis                              | Any string column   |        Default llm metric        |
+| [Text Statistics](#text-statistics) |           Text quality, readability, complexity, and grade level.           | Any string column   | Default llm metric, light-weight |
+|          [Themes](#themes)          | Semantic similarity between set of known jailbreak and LLM refusal examples | Any string column   |        Default llm metric        |
+|          [Topics](#topics)          |  Text classification into predefined topics - law, finance, medical, etc.   | Any string column   |                                  |
+|        [Toxicity](#toxicity)        |                   Toxicity, harmfulness and offensiveness                   | Any string column   |        Default llm metric        |
 
 ## Injections
 
 The `injections` module gather metrics on possible prompt injection attacks. It will be applied to column named `prompt`, and it will create a new column named `prompt.injection`.
 
 ### Usage
 
@@ -26,14 +28,16 @@
 
 ### `prompt.injection`
 
 The `prompt.injection` computed column will contain classification scores from a prompt injection classifier to attempt to predict whether a prompt contains an injection attack. The higher the score, the more likely it is to be a prompt injection attack.
 
 It currently uses the HuggingFace's model [`JasperLS/gelectra-base-injection`](https://huggingface.co/JasperLS/gelectra-base-injection) to make predictions.
 
+> Note: The current model has been known to yield high false positive rates and might not be suited for production use.
+
 ## Input/Output
 
 The `input_output` module will compute similarity scores between two columns called `prompt` and `response`. It will create a new column named `response.relevance_to_prompt`
 
 ### Usage
 
 ```python
```

### Comparing `langkit-0.0.7/langkit/examples/Batch_to_Whylabs.ipynb` & `langkit-0.0.8/langkit/examples/Batch_to_Whylabs.ipynb`

 * *Files identical despite different names*

### Comparing `langkit-0.0.7/langkit/examples/Intro_to_Langkit.ipynb` & `langkit-0.0.8/langkit/examples/Intro_to_Langkit.ipynb`

 * *Files identical despite different names*

### Comparing `langkit-0.0.7/langkit/examples/LLM_to_WhyLabs.ipynb` & `langkit-0.0.8/langkit/examples/LLM_to_WhyLabs.ipynb`

 * *Files identical despite different names*

### Comparing `langkit-0.0.7/langkit/examples/Langchain_OpenAI_LLM_Monitoring_with_WhyLabs.ipynb` & `langkit-0.0.8/langkit/examples/Langchain_OpenAI_LLM_Monitoring_with_WhyLabs.ipynb`

 * *Files identical despite different names*

### Comparing `langkit-0.0.7/langkit/examples/Logging_Text.ipynb` & `langkit-0.0.8/langkit/examples/Logging_Text.ipynb`

 * *Files identical despite different names*

### Comparing `langkit-0.0.7/langkit/examples/Sentiment_and_Toxicity.ipynb` & `langkit-0.0.8/langkit/examples/Sentiment_and_Toxicity.ipynb`

 * *Files identical despite different names*

### Comparing `langkit-0.0.7/langkit/examples/tutorials/Safeguarding_and_Monitoring_LLMs.ipynb` & `langkit-0.0.8/langkit/examples/tutorials/Safeguarding_and_Monitoring_LLMs.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998611111111111%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(7, '> This notebook is a complement to the blog post "*

 * *            '[Monitoring and Safeguarding Large Language Model '*

 * *            'Applications](https://whylabs.ai/blog/posts/safeguard-monitor-large-language-model-llm-applications). '*

 * *            "Please refer to the blog post for additional context.\\n')], delete: [7]}}}"}*

```diff
@@ -8,15 +8,15 @@
                 ">### \ud83d\udea9 *Create a free WhyLabs account to get more value out of whylogs!*<br> \n",
                 ">*Did you know you can store, visualize, and monitor language model profiles with the [WhyLabs Observability Platform](https://whylabs.ai/whylogs-free-signup?utm_source=github&utm_medium=referral&utm_campaign=langkit_safeguard_example)? Sign up for a [free WhyLabs account](https://whylabs.ai/whylogs-free-signup?utm_source=github&utm_medium=referral&utm_campaign=langkit_safeguard_example) to leverage the power of LangKit and WhyLabs together!*\n",
                 "\n",
                 "# Monitoring and Safeguarding Large Language Model Applications\n",
                 "\n",
                 "[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/whylabs/langkit/blob/main/langkit/examples/tutorials/Safeguarding_and_Monitoring_LLMS.ipynb)\n",
                 "\n",
-                "> This notebook is a complement to the blog post [Monitoring and Safeguarding Large Language Model Applications](placeholder). Please refer to the blog post for additional context.\n",
+                "> This notebook is a complement to the blog post [Monitoring and Safeguarding Large Language Model Applications](https://whylabs.ai/blog/posts/safeguard-monitor-large-language-model-llm-applications). Please refer to the blog post for additional context.\n",
                 "\n",
                 "Large Language models (LLMs) have become increasingly powerful tools for generating text, but with great power comes the need for responsible usage. As LLMs are deployed in various applications, it becomes crucial to monitor their behavior and implement safeguards to prevent potential issues such as toxic prompts and responses or the presence of sensitive content. In this blog post, we will explore the concept of observability and validation in the context of language models, and demonstrate how to effectively safeguard LLMs using guardrails.\n",
                 "\n",
                 "In this article, we will build a simple pipeline that will validate and moderate user prompts and LLM responses for toxicity and the presence of sensitive content. We will do so by using LangKit's `toxicity` and `regexes` module in conjunction with whylogs' `Condition Validators`. We will also calculate text-based metrics with LangKit, generate statistical profiles with whylogs and send them to the WhyLabs observability platform for visualization and monitoring.\n",
                 "\n",
                 "> Note: the current example was built for didactic purposes and it\u2019s not meant to be used in production.\n"
             ]
```

### Comparing `langkit-0.0.7/langkit/examples/tutorials/images/dashboard.png` & `langkit-0.0.8/langkit/examples/tutorials/images/dashboard.png`

 * *Files identical despite different names*

### Comparing `langkit-0.0.7/langkit/examples/tutorials/images/safeguards_pipeline.png` & `langkit-0.0.8/langkit/examples/tutorials/images/safeguards_pipeline.png`

 * *Files identical despite different names*

### Comparing `langkit-0.0.7/langkit/injections.py` & `langkit-0.0.8/langkit/injections.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.7/langkit/input_output.py` & `langkit-0.0.8/langkit/input_output.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.7/langkit/llm_metrics.py` & `langkit-0.0.8/langkit/llm_metrics.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.7/langkit/openai/openai.py` & `langkit-0.0.8/langkit/openai/openai.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.7/langkit/openai_wrapper.py` & `langkit-0.0.8/langkit/openai_wrapper.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.7/langkit/pattern_groups.json` & `langkit-0.0.8/langkit/pattern_groups.json`

 * *Files 17% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8%*

 * *Differences: {'0': "{'expressions': ['(?!(\\\\d){3}(-| "*

 * *      '|)\\\\1{2}\\\\2\\\\1{4})(?!666|000|9\\\\d{2})(\\\\b\\\\d{3}(-| '*

 * *      "|)(?!00)\\\\d{2}\\\\4(?!0{4})\\\\d{4}\\\\b)'], 'name': 'SSN'}",*

 * * '1': "{'expressions': ['\\\\b\\\\d{4}[- ]?(\\\\d{4}[- "*

 * *      "]?){2,3}\\\\d{4}\\\\b|\\\\b\\\\d{15}\\\\b'], 'name': 'credit card number'}"}*

```diff
@@ -1,19 +1,19 @@
 [
     {
         "expressions": [
-            "\\b\\d{4}[- ]?(\\d{4}[- ]?){2,3}\\d{4}\\b"
+            "(?!(\\d){3}(-| |)\\1{2}\\2\\1{4})(?!666|000|9\\d{2})(\\b\\d{3}(-| |)(?!00)\\d{2}\\4(?!0{4})\\d{4}\\b)"
         ],
-        "name": "credit card number"
+        "name": "SSN"
     },
     {
         "expressions": [
-            "(?!(\\d){3}(-| |)\\1{2}\\2\\1{4})(?!666|000|9\\d{2})(\\b\\d{3}(-| |)(?!00)\\d{2}\\4(?!0{4})\\d{4}\\b)"
+            "\\b\\d{4}[- ]?(\\d{4}[- ]?){2,3}\\d{4}\\b|\\b\\d{15}\\b"
         ],
-        "name": "SSN"
+        "name": "credit card number"
     },
     {
         "expressions": [
             "((\\+\\d{1,2}\\s)?\\(?\\d{3}\\)?[\\s.-]\\d{3}[\\s.-]\\d{4}|[0-9]{10}|\\+{1}[0-9 ]{11,15}|[0-9]{4} [0-9]{6})"
         ],
         "name": "phone number"
     },
```

### Comparing `langkit-0.0.7/langkit/regexes.py` & `langkit-0.0.8/langkit/regexes.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,16 +5,14 @@
 from whylogs.experimental.core.metrics.udf_metric import register_metric_udf
 from . import LangKitConfig
 from whylogs.core.datatypes import TypeMapper, DataType, String
 from typing import Any, List, Optional, Type
 
 diagnostic_logger = getLogger(__name__)
 
-lang_config = LangKitConfig()
-
 
 class AllString(TypeMapper):
     """Map a dtype (Pandas) or a Python type to a data type."""
 
     def __init__(self, custom_types: Optional[List[Type[DataType]]] = None):
         """
 
@@ -69,26 +67,31 @@
 
 
 pattern_loader = PatternLoader()
 
 
 def has_patterns(text: str) -> Optional[str]:
     regex_groups = pattern_loader.get_regex_groups()
-    patterns_info = None
     if regex_groups:
         for group in regex_groups:
             for expression in group["expressions"]:
                 if expression.search(text):
-                    patterns_info = group["name"]
                     return group["name"]
-    return patterns_info
+    return None
 
 
 if pattern_loader.get_regex_groups() is not None:
     register_metric_udf(col_type=String, type_mapper=AllString())(has_patterns)
 
 
-def init(pattern_file_path: Optional[str] = None):
+def init(
+    pattern_file_path: Optional[str] = None, lang_config: Optional[LangKitConfig] = None
+):
+    if lang_config is None:
+        lang_config = LangKitConfig()
     if pattern_file_path:
         lang_config.pattern_file_path = pattern_file_path
         pattern_loader.set_config(lang_config)
         pattern_loader.update_patterns()
+    else:
+        pattern_loader.set_config(lang_config)
+        pattern_loader.update_patterns()
```

### Comparing `langkit-0.0.7/langkit/sentiment.py` & `langkit-0.0.8/langkit/sentiment.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.7/langkit/tests/__init__.py` & `langkit-0.0.8/langkit/tests/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -18,14 +18,22 @@
             "finance",
             "medical",
             "education",
             "politics",
             "support",
         ]
     )
+    nlp_scores: list = field(
+        default_factory=lambda: [
+            "bleu",
+            "rouge",
+            "meteor",
+        ]
+    )
+    reference_corpus: str = ""
 
 
 def package_version(package: str = __package__) -> str:
     """Calculate version number based on pyproject.toml"""
     try:
         from importlib import metadata
```

### Comparing `langkit-0.0.7/langkit/tests/conftest.py` & `langkit-0.0.8/langkit/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.7/langkit/tests/test_callback_handler.py` & `langkit-0.0.8/langkit/tests/test_callback_handler.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.7/langkit/tests/test_injections.py` & `langkit-0.0.8/langkit/tests/test_injections.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.7/langkit/tests/test_input_output.py` & `langkit-0.0.8/langkit/tests/test_input_output.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.7/langkit/tests/test_themes.py` & `langkit-0.0.8/langkit/tests/test_themes.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,18 +67,22 @@
     from whylogs.experimental.core.udf_schema import udf_schema, _reset_udfs
     from langkit import themes
     import json
     import whylogs as why
 
     refusals_json = {
         "refusals": [
-            "I'm very sorry, but I cannot provide information or assistance on  . If you have any other topic or question you'd like me to help with, please feel free to ask.",
+            "I'm very sorry, but I cannot provide information or assistance on  ."
+            " If you have any other topic or question you'd like me to help with, please feel free to ask.",
             "Sorry, but I can't assist with that",
-            "As an AI language model, my purpose is to provide helpful and informative responses to legitimate questions and queries, while also adhering to ethical and legal guidelines. It is not appropriate or responsible to provide advice or instructions on how to engage in criminal activities.",
-            "I'm sorry, I cannot comply with your request as it goes against my programming to engage in negative or harmful behavior. My purpose is to assist and provide helpful responses.",
+            "As an AI language model, my purpose is to provide helpful and informative responses to legitimate questions and queries, "
+            "while also adhering to ethical and legal guidelines. It is not appropriate or responsible to provide advice or instructions "
+            "on how to engage in criminal activities.",
+            "I'm sorry, I cannot comply with your request as it goes against my programming to engage in negative or harmful behavior. "
+            "My purpose is to assist and provide helpful responses.",
         ]
     }
     # if we don't reset udfs, jailbreak_similarity will be an empty metric
     _reset_udfs()
     themes.init(theme_json=json.dumps(refusals_json))
     schema = udf_schema()
```

### Comparing `langkit-0.0.7/langkit/tests/test_toxicity.py` & `langkit-0.0.8/langkit/tests/test_toxicity.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.7/langkit/textstat.py` & `langkit-0.0.8/langkit/textstat.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.7/langkit/themes.json` & `langkit-0.0.8/langkit/themes.json`

 * *Files identical despite different names*

### Comparing `langkit-0.0.7/langkit/themes.py` & `langkit-0.0.8/langkit/themes.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.7/langkit/topics.py` & `langkit-0.0.8/langkit/topics.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.7/langkit/toxicity.py` & `langkit-0.0.8/langkit/toxicity.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.7/langkit/whylogs/example_utils/guardrails_example_utils.py` & `langkit-0.0.8/langkit/whylogs/example_utils/guardrails_example_utils.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.7/langkit/whylogs/example_utils/guardrails_llm_schema.py` & `langkit-0.0.8/langkit/whylogs/example_utils/guardrails_llm_schema.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.7/langkit/whylogs/reference_chats.json` & `langkit-0.0.8/langkit/whylogs/reference_chats.json`

 * *Files identical despite different names*

### Comparing `langkit-0.0.7/langkit/whylogs/samples.py` & `langkit-0.0.8/langkit/whylogs/samples.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.7/pyproject.toml` & `langkit-0.0.8/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,42 +1,50 @@
 [tool.poetry]
 name = "langkit"
-version = "0.0.7"
+version = "0.0.8"
 description = "A collection of text metric udfs for whylogs profiling and monitoring in WhyLabs"
 authors = ["WhyLabs.ai <langkit@whylabs.ai>"]
 license = "Apache-2.0"
 readme = "DESCRIPTION.md"
 
 
 [tool.poetry.dependencies]
 python = "^3.8"
 textstat = "^0.7.3"
 pandas = "*"
-whylogs = "^1.2.4"
+whylogs = "1.2.4"
 
 
 # optional dependencies
 torch = {version = "*", optional = true}
 datasets = {version ="^2.12.0", optional = true}
 openai = {version ="^0.27.6", optional = true}
 nltk = {version ="^3.8.1", optional = true}
 sentence-transformers = {version ="^2.2.2", optional = true}
+evaluate = {version = "^0.4.0", optional = true}
 
 
 [tool.poetry.group.dev.dependencies]
 ipykernel = "^6.23.0"
 pytest = "^7.3.1"
+mypy = "^1.4.1"
+pre-commit = "^2.8"
+black = "^23.7.0"
+flake8 = { version = "^6.0.0", python = ">=3.8.1,<4.0" }
+types-setuptools = "^68.0.0.2"
+bump2version = "^1.0.1"
 
 
 [tool.poetry.extras]
 all = [
     "torch",
     "datasets",
     "openai",
     "nltk",
     "sentence-transformers",
+    "evaluate",
 ]
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `langkit-0.0.7/PKG-INFO` & `langkit-0.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 Metadata-Version: 2.1
 Name: langkit
-Version: 0.0.7
+Version: 0.0.8
 Summary: A collection of text metric udfs for whylogs profiling and monitoring in WhyLabs
 License: Apache-2.0
 Author: WhyLabs.ai
 Author-email: langkit@whylabs.ai
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: all
 Requires-Dist: datasets (>=2.12.0,<3.0.0) ; extra == "all"
+Requires-Dist: evaluate (>=0.4.0,<0.5.0) ; extra == "all"
 Requires-Dist: nltk (>=3.8.1,<4.0.0) ; extra == "all"
 Requires-Dist: openai (>=0.27.6,<0.28.0) ; extra == "all"
 Requires-Dist: pandas
 Requires-Dist: sentence-transformers (>=2.2.2,<3.0.0) ; extra == "all"
 Requires-Dist: textstat (>=0.7.3,<0.8.0)
 Requires-Dist: torch ; extra == "all"
-Requires-Dist: whylogs (>=1.2.4,<2.0.0)
+Requires-Dist: whylogs (==1.2.4)
 Description-Content-Type: text/markdown
 
 LangKit is an open-source text metrics toolkit for monitoring language models. It offers an array of methods for extracting relevant signals from the input and/or output text, which are compatible with the open-source data logging library [whylogs](https://whylogs.readthedocs.io/en/latest).
 
 > 💡 Want to experience LangKit? Go to this [notebook](https://github.com/whylabs/langkit/blob/main/langkit/examples/Intro_to_Langkit.ipynb)!
 
 ## Table of Contents 📖
```

