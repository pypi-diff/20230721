# Comparing `tmp/llmtuner-0.1.2.tar.gz` & `tmp/llmtuner-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llmtuner-0.1.2.tar", last modified: Thu Jul 20 14:33:27 2023, max compression
+gzip compressed data, was "llmtuner-0.1.3.tar", last modified: Fri Jul 21 08:46:23 2023, max compression
```

## Comparing `llmtuner-0.1.2.tar` & `llmtuner-0.1.3.tar`

### file list

```diff
@@ -1,89 +1,90 @@
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-20 14:33:27.086244 llmtuner-0.1.2/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)    11524 2023-07-20 14:33:04.000000 llmtuner-0.1.2/LICENSE
--rw-r--r--   0 zhengyw  (38105) domain users (10513)    15186 2023-07-20 14:33:27.086244 llmtuner-0.1.2/PKG-INFO
--rw-r--r--   0 zhengyw  (38105) domain users (10513)    14586 2023-07-20 14:33:09.000000 llmtuner-0.1.2/README.md
--rw-r--r--   0 zhengyw  (38105) domain users (10513)       87 2023-07-20 14:33:09.000000 llmtuner-0.1.2/pyproject.toml
--rw-r--r--   0 zhengyw  (38105) domain users (10513)       38 2023-07-20 14:33:27.086244 llmtuner-0.1.2/setup.cfg
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2033 2023-07-20 14:33:09.000000 llmtuner-0.1.2/setup.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-20 14:33:26.838234 llmtuner-0.1.2/src/
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-20 14:33:26.886236 llmtuner-0.1.2/src/llmtuner/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)       64 2023-07-20 14:33:08.000000 llmtuner-0.1.2/src/llmtuner/__init__.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-20 14:33:26.906237 llmtuner-0.1.2/src/llmtuner/api/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)        0 2023-07-20 14:33:05.000000 llmtuner-0.1.2/src/llmtuner/api/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     4620 2023-07-20 14:33:05.000000 llmtuner-0.1.2/src/llmtuner/api/app.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2146 2023-07-20 14:33:05.000000 llmtuner-0.1.2/src/llmtuner/api/protocol.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-20 14:33:26.926237 llmtuner-0.1.2/src/llmtuner/chat/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)       49 2023-07-20 14:33:05.000000 llmtuner-0.1.2/src/llmtuner/chat/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     3670 2023-07-20 14:33:05.000000 llmtuner-0.1.2/src/llmtuner/chat/stream_chat.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-20 14:33:26.934238 llmtuner-0.1.2/src/llmtuner/dsets/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      153 2023-07-20 14:33:05.000000 llmtuner-0.1.2/src/llmtuner/dsets/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     4294 2023-07-20 14:33:05.000000 llmtuner-0.1.2/src/llmtuner/dsets/loader.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     8202 2023-07-20 14:33:05.000000 llmtuner-0.1.2/src/llmtuner/dsets/preprocess.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      515 2023-07-20 14:33:05.000000 llmtuner-0.1.2/src/llmtuner/dsets/utils.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-20 14:33:26.950239 llmtuner-0.1.2/src/llmtuner/extras/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)        0 2023-07-20 14:33:06.000000 llmtuner-0.1.2/src/llmtuner/extras/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     3138 2023-07-20 14:33:05.000000 llmtuner-0.1.2/src/llmtuner/extras/callbacks.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     1735 2023-07-20 14:33:05.000000 llmtuner-0.1.2/src/llmtuner/extras/constants.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      751 2023-07-20 14:33:05.000000 llmtuner-0.1.2/src/llmtuner/extras/logging.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     3884 2023-07-20 14:33:05.000000 llmtuner-0.1.2/src/llmtuner/extras/misc.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     1788 2023-07-20 14:33:06.000000 llmtuner-0.1.2/src/llmtuner/extras/ploting.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2172 2023-07-20 14:33:06.000000 llmtuner-0.1.2/src/llmtuner/extras/save_and_load.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     6500 2023-07-20 14:33:06.000000 llmtuner-0.1.2/src/llmtuner/extras/template.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-20 14:33:26.966239 llmtuner-0.1.2/src/llmtuner/hparams/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      222 2023-07-20 14:33:06.000000 llmtuner-0.1.2/src/llmtuner/hparams/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     5013 2023-07-20 14:33:06.000000 llmtuner-0.1.2/src/llmtuner/hparams/data_args.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     3831 2023-07-20 14:33:06.000000 llmtuner-0.1.2/src/llmtuner/hparams/finetuning_args.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      388 2023-07-20 14:33:06.000000 llmtuner-0.1.2/src/llmtuner/hparams/general_args.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     1973 2023-07-20 14:33:06.000000 llmtuner-0.1.2/src/llmtuner/hparams/generating_args.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     3053 2023-07-20 14:33:06.000000 llmtuner-0.1.2/src/llmtuner/hparams/model_args.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-20 14:33:26.966239 llmtuner-0.1.2/src/llmtuner/tuner/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      241 2023-07-20 14:33:08.000000 llmtuner-0.1.2/src/llmtuner/tuner/__init__.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-20 14:33:26.986240 llmtuner-0.1.2/src/llmtuner/tuner/core/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      136 2023-07-20 14:33:06.000000 llmtuner-0.1.2/src/llmtuner/tuner/core/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     3839 2023-07-20 14:33:06.000000 llmtuner-0.1.2/src/llmtuner/tuner/core/adapter.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     7187 2023-07-20 14:33:06.000000 llmtuner-0.1.2/src/llmtuner/tuner/core/loader.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     6400 2023-07-20 14:33:06.000000 llmtuner-0.1.2/src/llmtuner/tuner/core/parser.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     4113 2023-07-20 14:33:06.000000 llmtuner-0.1.2/src/llmtuner/tuner/core/trainer.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-20 14:33:26.994240 llmtuner-0.1.2/src/llmtuner/tuner/ppo/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)       49 2023-07-20 14:33:07.000000 llmtuner-0.1.2/src/llmtuner/tuner/ppo/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     8221 2023-07-20 14:33:07.000000 llmtuner-0.1.2/src/llmtuner/tuner/ppo/trainer.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     1673 2023-07-20 14:33:07.000000 llmtuner-0.1.2/src/llmtuner/tuner/ppo/utils.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     3083 2023-07-20 14:33:07.000000 llmtuner-0.1.2/src/llmtuner/tuner/ppo/workflow.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-20 14:33:27.018241 llmtuner-0.1.2/src/llmtuner/tuner/pt/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)       47 2023-07-20 14:33:07.000000 llmtuner-0.1.2/src/llmtuner/tuner/pt/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2516 2023-07-20 14:33:07.000000 llmtuner-0.1.2/src/llmtuner/tuner/pt/workflow.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-20 14:33:27.030242 llmtuner-0.1.2/src/llmtuner/tuner/rm/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)       47 2023-07-20 14:33:07.000000 llmtuner-0.1.2/src/llmtuner/tuner/rm/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      722 2023-07-20 14:33:07.000000 llmtuner-0.1.2/src/llmtuner/tuner/rm/collator.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      273 2023-07-20 14:33:07.000000 llmtuner-0.1.2/src/llmtuner/tuner/rm/metric.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     1527 2023-07-20 14:33:07.000000 llmtuner-0.1.2/src/llmtuner/tuner/rm/trainer.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2486 2023-07-20 14:33:07.000000 llmtuner-0.1.2/src/llmtuner/tuner/rm/workflow.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-20 14:33:27.038242 llmtuner-0.1.2/src/llmtuner/tuner/sft/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)       49 2023-07-20 14:33:08.000000 llmtuner-0.1.2/src/llmtuner/tuner/sft/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2183 2023-07-20 14:33:08.000000 llmtuner-0.1.2/src/llmtuner/tuner/sft/metric.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     4553 2023-07-20 14:33:08.000000 llmtuner-0.1.2/src/llmtuner/tuner/sft/trainer.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     3896 2023-07-20 14:33:08.000000 llmtuner-0.1.2/src/llmtuner/tuner/sft/workflow.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-20 14:33:27.066243 llmtuner-0.1.2/src/llmtuner/webui/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)        0 2023-07-20 14:33:09.000000 llmtuner-0.1.2/src/llmtuner/webui/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2769 2023-07-20 14:33:08.000000 llmtuner-0.1.2/src/llmtuner/webui/chat.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2564 2023-07-20 14:33:08.000000 llmtuner-0.1.2/src/llmtuner/webui/common.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-20 14:33:27.082244 llmtuner-0.1.2/src/llmtuner/webui/components/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      234 2023-07-20 14:33:08.000000 llmtuner-0.1.2/src/llmtuner/webui/components/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     1837 2023-07-20 14:33:08.000000 llmtuner-0.1.2/src/llmtuner/webui/components/chatbot.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      625 2023-07-20 14:33:08.000000 llmtuner-0.1.2/src/llmtuner/webui/components/data.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2567 2023-07-20 14:33:08.000000 llmtuner-0.1.2/src/llmtuner/webui/components/eval.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     1424 2023-07-20 14:33:08.000000 llmtuner-0.1.2/src/llmtuner/webui/components/infer.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     5132 2023-07-20 14:33:08.000000 llmtuner-0.1.2/src/llmtuner/webui/components/sft.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2081 2023-07-20 14:33:08.000000 llmtuner-0.1.2/src/llmtuner/webui/components/top.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      387 2023-07-20 14:33:08.000000 llmtuner-0.1.2/src/llmtuner/webui/css.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     1456 2023-07-20 14:33:09.000000 llmtuner-0.1.2/src/llmtuner/webui/interface.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)    12736 2023-07-20 14:33:09.000000 llmtuner-0.1.2/src/llmtuner/webui/locales.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     1224 2023-07-20 14:33:09.000000 llmtuner-0.1.2/src/llmtuner/webui/manager.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     8072 2023-07-20 14:33:09.000000 llmtuner-0.1.2/src/llmtuner/webui/runner.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2896 2023-07-20 14:33:09.000000 llmtuner-0.1.2/src/llmtuner/webui/utils.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-20 14:33:26.902237 llmtuner-0.1.2/src/llmtuner.egg-info/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)    15186 2023-07-20 14:33:26.000000 llmtuner-0.1.2/src/llmtuner.egg-info/PKG-INFO
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2234 2023-07-20 14:33:26.000000 llmtuner-0.1.2/src/llmtuner.egg-info/SOURCES.txt
--rw-r--r--   0 zhengyw  (38105) domain users (10513)        1 2023-07-20 14:33:26.000000 llmtuner-0.1.2/src/llmtuner.egg-info/dependency_links.txt
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      215 2023-07-20 14:33:26.000000 llmtuner-0.1.2/src/llmtuner.egg-info/requires.txt
--rw-r--r--   0 zhengyw  (38105) domain users (10513)        9 2023-07-20 14:33:26.000000 llmtuner-0.1.2/src/llmtuner.egg-info/top_level.txt
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-21 08:46:23.642495 llmtuner-0.1.3/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)    11524 2023-07-21 08:45:52.000000 llmtuner-0.1.3/LICENSE
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)    15186 2023-07-21 08:46:23.642495 llmtuner-0.1.3/PKG-INFO
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)    14586 2023-07-21 08:45:58.000000 llmtuner-0.1.3/README.md
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)       87 2023-07-21 08:45:58.000000 llmtuner-0.1.3/pyproject.toml
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)       38 2023-07-21 08:46:23.642495 llmtuner-0.1.3/setup.cfg
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2033 2023-07-21 08:45:58.000000 llmtuner-0.1.3/setup.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-21 08:46:23.466489 llmtuner-0.1.3/src/
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-21 08:46:23.482490 llmtuner-0.1.3/src/llmtuner/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)       64 2023-07-21 08:45:56.000000 llmtuner-0.1.3/src/llmtuner/__init__.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-21 08:46:23.490490 llmtuner-0.1.3/src/llmtuner/api/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)        0 2023-07-21 08:45:53.000000 llmtuner-0.1.3/src/llmtuner/api/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     4620 2023-07-21 08:45:53.000000 llmtuner-0.1.3/src/llmtuner/api/app.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2146 2023-07-21 08:45:53.000000 llmtuner-0.1.3/src/llmtuner/api/protocol.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-21 08:46:23.494490 llmtuner-0.1.3/src/llmtuner/chat/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)       49 2023-07-21 08:45:53.000000 llmtuner-0.1.3/src/llmtuner/chat/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     3670 2023-07-21 08:45:53.000000 llmtuner-0.1.3/src/llmtuner/chat/stream_chat.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-21 08:46:23.502490 llmtuner-0.1.3/src/llmtuner/dsets/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      153 2023-07-21 08:45:54.000000 llmtuner-0.1.3/src/llmtuner/dsets/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     4294 2023-07-21 08:45:53.000000 llmtuner-0.1.3/src/llmtuner/dsets/loader.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     8250 2023-07-21 08:45:53.000000 llmtuner-0.1.3/src/llmtuner/dsets/preprocess.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      515 2023-07-21 08:45:53.000000 llmtuner-0.1.3/src/llmtuner/dsets/utils.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-21 08:46:23.514491 llmtuner-0.1.3/src/llmtuner/extras/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)        0 2023-07-21 08:45:54.000000 llmtuner-0.1.3/src/llmtuner/extras/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     3138 2023-07-21 08:45:54.000000 llmtuner-0.1.3/src/llmtuner/extras/callbacks.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     1735 2023-07-21 08:45:54.000000 llmtuner-0.1.3/src/llmtuner/extras/constants.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      751 2023-07-21 08:45:54.000000 llmtuner-0.1.3/src/llmtuner/extras/logging.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     3884 2023-07-21 08:45:54.000000 llmtuner-0.1.3/src/llmtuner/extras/misc.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     1788 2023-07-21 08:45:54.000000 llmtuner-0.1.3/src/llmtuner/extras/ploting.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2196 2023-07-21 08:45:54.000000 llmtuner-0.1.3/src/llmtuner/extras/save_and_load.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     6500 2023-07-21 08:45:54.000000 llmtuner-0.1.3/src/llmtuner/extras/template.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-21 08:46:23.530491 llmtuner-0.1.3/src/llmtuner/hparams/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      222 2023-07-21 08:45:54.000000 llmtuner-0.1.3/src/llmtuner/hparams/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     5013 2023-07-21 08:45:54.000000 llmtuner-0.1.3/src/llmtuner/hparams/data_args.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     3831 2023-07-21 08:45:54.000000 llmtuner-0.1.3/src/llmtuner/hparams/finetuning_args.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      388 2023-07-21 08:45:54.000000 llmtuner-0.1.3/src/llmtuner/hparams/general_args.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     1973 2023-07-21 08:45:54.000000 llmtuner-0.1.3/src/llmtuner/hparams/generating_args.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     3053 2023-07-21 08:45:54.000000 llmtuner-0.1.3/src/llmtuner/hparams/model_args.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-21 08:46:23.534491 llmtuner-0.1.3/src/llmtuner/tuner/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      241 2023-07-21 08:45:56.000000 llmtuner-0.1.3/src/llmtuner/tuner/__init__.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-21 08:46:23.554492 llmtuner-0.1.3/src/llmtuner/tuner/core/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      136 2023-07-21 08:45:55.000000 llmtuner-0.1.3/src/llmtuner/tuner/core/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     3839 2023-07-21 08:45:55.000000 llmtuner-0.1.3/src/llmtuner/tuner/core/adapter.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     6881 2023-07-21 08:45:55.000000 llmtuner-0.1.3/src/llmtuner/tuner/core/loader.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     6431 2023-07-21 08:45:55.000000 llmtuner-0.1.3/src/llmtuner/tuner/core/parser.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     4315 2023-07-21 08:45:55.000000 llmtuner-0.1.3/src/llmtuner/tuner/core/trainer.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-21 08:46:23.574493 llmtuner-0.1.3/src/llmtuner/tuner/ppo/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)       49 2023-07-21 08:45:55.000000 llmtuner-0.1.3/src/llmtuner/tuner/ppo/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     8221 2023-07-21 08:45:55.000000 llmtuner-0.1.3/src/llmtuner/tuner/ppo/trainer.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     1673 2023-07-21 08:45:55.000000 llmtuner-0.1.3/src/llmtuner/tuner/ppo/utils.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     3083 2023-07-21 08:45:55.000000 llmtuner-0.1.3/src/llmtuner/tuner/ppo/workflow.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-21 08:46:23.578493 llmtuner-0.1.3/src/llmtuner/tuner/pt/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)       47 2023-07-21 08:45:55.000000 llmtuner-0.1.3/src/llmtuner/tuner/pt/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2516 2023-07-21 08:45:55.000000 llmtuner-0.1.3/src/llmtuner/tuner/pt/workflow.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-21 08:46:23.590494 llmtuner-0.1.3/src/llmtuner/tuner/rm/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)       47 2023-07-21 08:45:56.000000 llmtuner-0.1.3/src/llmtuner/tuner/rm/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      722 2023-07-21 08:45:56.000000 llmtuner-0.1.3/src/llmtuner/tuner/rm/collator.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      273 2023-07-21 08:45:56.000000 llmtuner-0.1.3/src/llmtuner/tuner/rm/metric.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2555 2023-07-21 08:45:56.000000 llmtuner-0.1.3/src/llmtuner/tuner/rm/trainer.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2800 2023-07-21 08:45:56.000000 llmtuner-0.1.3/src/llmtuner/tuner/rm/workflow.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-21 08:46:23.598494 llmtuner-0.1.3/src/llmtuner/tuner/sft/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)       49 2023-07-21 08:45:56.000000 llmtuner-0.1.3/src/llmtuner/tuner/sft/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2183 2023-07-21 08:45:56.000000 llmtuner-0.1.3/src/llmtuner/tuner/sft/metric.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     4553 2023-07-21 08:45:56.000000 llmtuner-0.1.3/src/llmtuner/tuner/sft/trainer.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     3896 2023-07-21 08:45:56.000000 llmtuner-0.1.3/src/llmtuner/tuner/sft/workflow.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-21 08:46:23.618494 llmtuner-0.1.3/src/llmtuner/webui/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)        0 2023-07-21 08:45:57.000000 llmtuner-0.1.3/src/llmtuner/webui/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2997 2023-07-21 08:45:56.000000 llmtuner-0.1.3/src/llmtuner/webui/chat.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2564 2023-07-21 08:45:56.000000 llmtuner-0.1.3/src/llmtuner/webui/common.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-21 08:46:23.638495 llmtuner-0.1.3/src/llmtuner/webui/components/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      298 2023-07-21 08:45:57.000000 llmtuner-0.1.3/src/llmtuner/webui/components/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     1703 2023-07-21 08:45:57.000000 llmtuner-0.1.3/src/llmtuner/webui/components/chatbot.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      625 2023-07-21 08:45:57.000000 llmtuner-0.1.3/src/llmtuner/webui/components/data.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2567 2023-07-21 08:45:57.000000 llmtuner-0.1.3/src/llmtuner/webui/components/eval.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      895 2023-07-21 08:45:57.000000 llmtuner-0.1.3/src/llmtuner/webui/components/export.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     1424 2023-07-21 08:45:57.000000 llmtuner-0.1.3/src/llmtuner/webui/components/infer.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     5116 2023-07-21 08:45:57.000000 llmtuner-0.1.3/src/llmtuner/webui/components/sft.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2081 2023-07-21 08:45:57.000000 llmtuner-0.1.3/src/llmtuner/webui/components/top.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      387 2023-07-21 08:45:57.000000 llmtuner-0.1.3/src/llmtuner/webui/css.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     1585 2023-07-21 08:45:57.000000 llmtuner-0.1.3/src/llmtuner/webui/interface.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)    13920 2023-07-21 08:45:57.000000 llmtuner-0.1.3/src/llmtuner/webui/locales.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     1224 2023-07-21 08:45:57.000000 llmtuner-0.1.3/src/llmtuner/webui/manager.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     8176 2023-07-21 08:45:57.000000 llmtuner-0.1.3/src/llmtuner/webui/runner.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     4279 2023-07-21 08:45:57.000000 llmtuner-0.1.3/src/llmtuner/webui/utils.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-21 08:46:23.486490 llmtuner-0.1.3/src/llmtuner.egg-info/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)    15186 2023-07-21 08:46:22.000000 llmtuner-0.1.3/src/llmtuner.egg-info/PKG-INFO
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2274 2023-07-21 08:46:22.000000 llmtuner-0.1.3/src/llmtuner.egg-info/SOURCES.txt
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)        1 2023-07-21 08:46:22.000000 llmtuner-0.1.3/src/llmtuner.egg-info/dependency_links.txt
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      215 2023-07-21 08:46:22.000000 llmtuner-0.1.3/src/llmtuner.egg-info/requires.txt
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)        9 2023-07-21 08:46:22.000000 llmtuner-0.1.3/src/llmtuner.egg-info/top_level.txt
```

### Comparing `llmtuner-0.1.2/LICENSE` & `llmtuner-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `llmtuner-0.1.2/PKG-INFO` & `llmtuner-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llmtuner
-Version: 0.1.2
+Version: 0.1.3
 Summary: Easy-to-use fine-tuning framework using PEFT
 Home-page: https://github.com/hiyouga/LLaMA-Efficient-Tuning
 Author: hiyouga
 Author-email: hiyouga@buaa.edu.cn
 License: Apache 2.0 License
 Keywords: LLaMA,BLOOM,Falcon,LLM,ChatGPT,transformer,pytorch,deep learning
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `llmtuner-0.1.2/README.md` & `llmtuner-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `llmtuner-0.1.2/setup.py` & `llmtuner-0.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.1.2/src/llmtuner/api/app.py` & `llmtuner-0.1.3/src/llmtuner/api/app.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.1.2/src/llmtuner/api/protocol.py` & `llmtuner-0.1.3/src/llmtuner/api/protocol.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.1.2/src/llmtuner/chat/stream_chat.py` & `llmtuner-0.1.3/src/llmtuner/chat/stream_chat.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.1.2/src/llmtuner/dsets/loader.py` & `llmtuner-0.1.3/src/llmtuner/dsets/loader.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.1.2/src/llmtuner/dsets/preprocess.py` & `llmtuner-0.1.3/src/llmtuner/dsets/preprocess.py`

 * *Files 0% similar despite different names*

```diff
@@ -139,16 +139,18 @@
     def print_unsupervised_dataset_example(example):
         print("input_ids:\n{}".format(example["input_ids"]))
         print("inputs:\n{}".format(tokenizer.decode(example["input_ids"], skip_special_tokens=False)))
 
     if stage == "pt":
         preprocess_function = preprocess_pretrain_dataset
     elif stage == "sft":
-        preprocess_function = preprocess_unsupervised_dataset \
-            if training_args.predict_with_generate else preprocess_supervised_dataset
+        if not training_args.predict_with_generate:
+            preprocess_function = preprocess_supervised_dataset
+        else:
+            preprocess_function = preprocess_unsupervised_dataset
     elif stage == "rm":
         preprocess_function = preprocess_pairwise_dataset
     elif stage == "ppo":
         preprocess_function = preprocess_unsupervised_dataset
 
     with training_args.main_process_first(desc="dataset map pre-processing"):
         dataset = dataset.map(
```

### Comparing `llmtuner-0.1.2/src/llmtuner/dsets/utils.py` & `llmtuner-0.1.3/src/llmtuner/dsets/utils.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.1.2/src/llmtuner/extras/callbacks.py` & `llmtuner-0.1.3/src/llmtuner/extras/callbacks.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.1.2/src/llmtuner/extras/constants.py` & `llmtuner-0.1.3/src/llmtuner/extras/constants.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.1.2/src/llmtuner/extras/logging.py` & `llmtuner-0.1.3/src/llmtuner/extras/logging.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.1.2/src/llmtuner/extras/misc.py` & `llmtuner-0.1.3/src/llmtuner/extras/misc.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.1.2/src/llmtuner/extras/ploting.py` & `llmtuner-0.1.3/src/llmtuner/extras/ploting.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.1.2/src/llmtuner/extras/save_and_load.py` & `llmtuner-0.1.3/src/llmtuner/extras/save_and_load.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 import os
 import torch
-from typing import Dict
+from typing import Dict, Optional
 
 from transformers.trainer import WEIGHTS_NAME, WEIGHTS_INDEX_NAME
 from transformers.modeling_utils import load_sharded_checkpoint
 
 from llmtuner.extras.constants import VALUE_HEAD_FILE_NAME
 from llmtuner.extras.logging import get_logger
 
 
 logger = get_logger(__name__)
 
 
-def get_state_dict(model: torch.nn.Module) -> Dict[str, torch.Tensor]: # get state dict containing trainable parameters
+def get_state_dict(model: torch.nn.Module, trainable_only: Optional[bool] = True) -> Dict[str, torch.Tensor]:
     state_dict = model.state_dict()
     filtered_state_dict = {}
 
     for k, v in model.named_parameters():
-        if v.requires_grad:
+        if (not trainable_only) or v.requires_grad:
             filtered_state_dict[k] = state_dict[k].cpu().clone().detach()
 
     return filtered_state_dict
 
 
 def load_trainable_params(model: torch.nn.Module, checkpoint_dir: os.PathLike) -> bool:
     weights_file = os.path.join(checkpoint_dir, WEIGHTS_NAME)
```

### Comparing `llmtuner-0.1.2/src/llmtuner/extras/template.py` & `llmtuner-0.1.3/src/llmtuner/extras/template.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.1.2/src/llmtuner/hparams/data_args.py` & `llmtuner-0.1.3/src/llmtuner/hparams/data_args.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.1.2/src/llmtuner/hparams/finetuning_args.py` & `llmtuner-0.1.3/src/llmtuner/hparams/finetuning_args.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.1.2/src/llmtuner/hparams/generating_args.py` & `llmtuner-0.1.3/src/llmtuner/hparams/generating_args.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.1.2/src/llmtuner/hparams/model_args.py` & `llmtuner-0.1.3/src/llmtuner/hparams/model_args.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.1.2/src/llmtuner/tuner/core/adapter.py` & `llmtuner-0.1.3/src/llmtuner/tuner/core/adapter.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.1.2/src/llmtuner/tuner/core/loader.py` & `llmtuner-0.1.3/src/llmtuner/tuner/core/loader.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,16 +23,16 @@
 
 
 logger = get_logger(__name__)
 
 
 check_min_version("4.29.1")
 require_version("datasets>=2.12.0", "To fix: pip install datasets>=2.12.0")
-require_version("accelerate>=0.19.0", "To fix: pip install accelerate>=0.19.0")
-require_version("peft>=0.3.0", "To fix: pip install peft>=0.3.0")
+require_version("accelerate>=0.21.0", "To fix: pip install accelerate>=0.21.0")
+require_version("peft>=0.4.0", "To fix: pip install peft>=0.4.0")
 require_version("trl>=0.4.7", "To fix: pip install trl>=0.4.7")
 
 
 def load_model_and_tokenizer(
     model_args: ModelArguments,
     finetuning_args: FinetuningArguments,
     is_trainable: Optional[bool] = False,
@@ -77,17 +77,14 @@
             config_kwargs["quantization_config"] = BitsAndBytesConfig(
                 load_in_8bit=True,
                 llm_int8_threshold=6.0
             )
 
         elif model_args.quantization_bit == 4:
             require_version("bitsandbytes>=0.39.0", "To fix: pip install bitsandbytes>=0.39.0")
-            require_version("transformers>=4.30.1", "To fix: pip install transformers>=4.30.1")
-            require_version("accelerate>=0.20.3", "To fix: pip install accelerate>=0.20.3")
-            require_version("peft>=0.4.0.dev0", "To fix: pip install git+https://github.com/huggingface/peft.git")
             config_kwargs["load_in_4bit"] = True
             config_kwargs["quantization_config"] = BitsAndBytesConfig(
                 load_in_4bit=True,
                 bnb_4bit_compute_dtype=model_args.compute_dtype,
                 bnb_4bit_use_double_quant=model_args.double_quantization,
                 bnb_4bit_quant_type=model_args.quantization_type
             )
```

### Comparing `llmtuner-0.1.2/src/llmtuner/tuner/core/parser.py` & `llmtuner-0.1.3/src/llmtuner/tuner/core/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 
     assert general_args.stage == "sft" or (not training_args.predict_with_generate), \
         "`predict_with_generate` cannot be set as True at PT, RM and PPO stages."
 
     assert not (training_args.do_train and training_args.predict_with_generate), \
         "`predict_with_generate` cannot be set as True while training."
 
-    assert (not training_args.do_predict) or training_args.predict_with_generate, \
+    assert general_args.stage != "sft" or (not training_args.do_predict) or training_args.predict_with_generate, \
         "Please enable `predict_with_generate` to save model predictions."
 
     assert model_args.quantization_bit is None or finetuning_args.finetuning_type == "lora", \
         "Quantization is only compatible with the LoRA method."
 
     if model_args.checkpoint_dir is not None:
         if finetuning_args.finetuning_type != "lora":
```

### Comparing `llmtuner-0.1.2/src/llmtuner/tuner/core/trainer.py` & `llmtuner-0.1.3/src/llmtuner/tuner/core/trainer.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import os
 import torch
 from typing import Dict, Optional
 
 from transformers import Seq2SeqTrainer
 from transformers.trainer import TRAINING_ARGS_NAME
-from transformers.modeling_utils import unwrap_model
+from transformers.modeling_utils import PreTrainedModel, unwrap_model
+from peft import PeftModel
 
 from llmtuner.extras.constants import FINETUNING_ARGS_NAME, VALUE_HEAD_FILE_NAME
 from llmtuner.extras.logging import get_logger
 from llmtuner.extras.save_and_load import get_state_dict, load_trainable_params, load_valuehead_params
 from llmtuner.hparams import FinetuningArguments
 
 
@@ -45,26 +46,28 @@
 
         if hasattr(model, "pretrained_model"): # for models with valuehead (currently using LoRA only)
             backbone_model = getattr(model, "pretrained_model")
             torch.save(get_state_dict(getattr(model, "v_head")), os.path.join(output_dir, VALUE_HEAD_FILE_NAME))
         else:
             backbone_model = model
 
-        if self.finetuning_args.finetuning_type == "lora":
+        if isinstance(backbone_model, PeftModel): # LoRA tuning
             backbone_model.save_pretrained(output_dir, state_dict=get_state_dict(backbone_model))
-        else: # freeze/full tuning
+        elif isinstance(backbone_model, PreTrainedModel): # freeze/full tuning
             backbone_model.config.use_cache = True
             backbone_model.save_pretrained(
                 output_dir,
-                state_dict=get_state_dict(backbone_model),
+                state_dict=get_state_dict(backbone_model, trainable_only=(self.finetuning_args.finetuning_type != "full")),
                 safe_serialization=self.args.save_safetensors
             )
             backbone_model.config.use_cache = False
             if self.tokenizer is not None:
                 self.tokenizer.save_pretrained(output_dir)
+        else:
+            logger.warning("No model to save.")
 
         with open(os.path.join(output_dir, TRAINING_ARGS_NAME), "w", encoding="utf-8") as f:
             f.write(self.args.to_json_string() + "\n")
         self.finetuning_args.save_to_json(os.path.join(output_dir, FINETUNING_ARGS_NAME))
 
     def _load_best_model(self):
         r"""
@@ -73,16 +76,16 @@
         Subclass and override to inject custom behavior. It should not be directly used by external scripts.
         """
         logger.info(f"Loading best model from {self.state.best_model_checkpoint} (score: {self.state.best_metric}).")
 
         model = unwrap_model(self.model)
         backbone_model = getattr(model, "pretrained_model") if hasattr(model, "pretrained_model") else model
 
-        if self.finetuning_args.finetuning_type == "lora":
-            backbone_model.load_adapter(self.state.best_model_checkpoint, getattr(backbone_model, "active_adapter"))
+        if isinstance(backbone_model, PeftModel):
+            backbone_model.load_adapter(self.state.best_model_checkpoint, backbone_model.active_adapter)
             if hasattr(model, "v_head") and load_valuehead_params(model, self.state.best_model_checkpoint):
                 model.v_head.load_state_dict({
                     "summary.weight": getattr(model, "reward_head_weight"),
                     "summary.bias": getattr(model, "reward_head_bias")
                 })
         else: # freeze/full-tuning
             load_trainable_params(backbone_model, self.state.best_model_checkpoint)
```

### Comparing `llmtuner-0.1.2/src/llmtuner/tuner/ppo/trainer.py` & `llmtuner-0.1.3/src/llmtuner/tuner/ppo/trainer.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.1.2/src/llmtuner/tuner/ppo/utils.py` & `llmtuner-0.1.3/src/llmtuner/tuner/ppo/utils.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.1.2/src/llmtuner/tuner/ppo/workflow.py` & `llmtuner-0.1.3/src/llmtuner/tuner/ppo/workflow.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.1.2/src/llmtuner/tuner/pt/workflow.py` & `llmtuner-0.1.3/src/llmtuner/tuner/pt/workflow.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.1.2/src/llmtuner/tuner/rm/collator.py` & `llmtuner-0.1.3/src/llmtuner/tuner/rm/collator.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.1.2/src/llmtuner/tuner/rm/workflow.py` & `llmtuner-0.1.3/src/llmtuner/tuner/rm/workflow.py`

 * *Files 16% similar despite different names*

```diff
@@ -52,7 +52,14 @@
             plot_loss(training_args.output_dir, keys=["loss", "eval_loss"])
 
     # Evaluation
     if training_args.do_eval:
         metrics = trainer.evaluate(metric_key_prefix="eval")
         trainer.log_metrics("eval", metrics)
         trainer.save_metrics("eval", metrics)
+
+    # Predict
+    if training_args.do_predict:
+        predict_results = trainer.predict(dataset, metric_key_prefix="predict")
+        trainer.log_metrics("predict", predict_results.metrics)
+        trainer.save_metrics("predict", predict_results.metrics)
+        trainer.save_predictions(predict_results)
```

### Comparing `llmtuner-0.1.2/src/llmtuner/tuner/sft/metric.py` & `llmtuner-0.1.3/src/llmtuner/tuner/sft/metric.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.1.2/src/llmtuner/tuner/sft/trainer.py` & `llmtuner-0.1.3/src/llmtuner/tuner/sft/trainer.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.1.2/src/llmtuner/tuner/sft/workflow.py` & `llmtuner-0.1.3/src/llmtuner/tuner/sft/workflow.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.1.2/src/llmtuner/webui/chat.py` & `llmtuner-0.1.3/src/llmtuner/webui/chat.py`

 * *Files 10% similar despite different names*

```diff
@@ -80,10 +80,16 @@
     ):
         chatbot.append([query, ""])
         response = ""
         for new_text in self.stream_chat(
             query, history, prefix, max_new_tokens=max_new_tokens, top_p=top_p, temperature=temperature
         ):
             response += new_text
+            response = self.postprocess(response)
             new_history = history + [(query, response)]
             chatbot[-1] = [query, response]
             yield chatbot, new_history
+
+    def postprocess(self, response: str) -> str:
+        response = response.replace("<", "&lt;")
+        response = response.replace(">", "&gt;")
+        return response
```

### Comparing `llmtuner-0.1.2/src/llmtuner/webui/common.py` & `llmtuner-0.1.3/src/llmtuner/webui/common.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.1.2/src/llmtuner/webui/components/chatbot.py` & `llmtuner-0.1.3/src/llmtuner/webui/components/chatbot.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,21 +18,17 @@
             with gr.Column(scale=4):
                 prefix = gr.Textbox(show_label=False)
                 query = gr.Textbox(show_label=False, lines=8)
                 submit_btn = gr.Button(variant="primary")
 
             with gr.Column(scale=1):
                 clear_btn = gr.Button()
-                max_new_tokens = gr.Slider(
-                    10, 2048, value=chat_model.generating_args.max_new_tokens, step=1, interactive=True
-                )
-                top_p = gr.Slider(0.01, 1, value=chat_model.generating_args.top_p, step=0.01, interactive=True)
-                temperature = gr.Slider(
-                    0.01, 1.5, value=chat_model.generating_args.temperature, step=0.01, interactive=True
-                )
+                max_new_tokens = gr.Slider(10, 2048, value=chat_model.generating_args.max_new_tokens, step=1)
+                top_p = gr.Slider(0.01, 1, value=chat_model.generating_args.top_p, step=0.01)
+                temperature = gr.Slider(0.01, 1.5, value=chat_model.generating_args.temperature, step=0.01)
 
     history = gr.State([])
 
     submit_btn.click(
         chat_model.predict,
         [chatbot, query, history, prefix, max_new_tokens, top_p, temperature],
         [chatbot, history],
```

### Comparing `llmtuner-0.1.2/src/llmtuner/webui/components/data.py` & `llmtuner-0.1.3/src/llmtuner/webui/components/data.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.1.2/src/llmtuner/webui/components/eval.py` & `llmtuner-0.1.3/src/llmtuner/webui/components/eval.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.1.2/src/llmtuner/webui/components/infer.py` & `llmtuner-0.1.3/src/llmtuner/webui/components/infer.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.1.2/src/llmtuner/webui/components/sft.py` & `llmtuner-0.1.3/src/llmtuner/webui/components/sft.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 
     with gr.Row():
         start_btn = gr.Button()
         stop_btn = gr.Button()
 
     with gr.Row():
         with gr.Column(scale=4):
-            output_dir = gr.Textbox(interactive=True)
+            output_dir = gr.Textbox()
 
             with gr.Box():
                 output_box = gr.Markdown()
 
         with gr.Column(scale=1):
             loss_viewer = gr.Plot()
```

### Comparing `llmtuner-0.1.2/src/llmtuner/webui/components/top.py` & `llmtuner-0.1.3/src/llmtuner/webui/components/top.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.1.2/src/llmtuner/webui/interface.py` & `llmtuner-0.1.3/src/llmtuner/webui/interface.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import gradio as gr
 from transformers.utils.versions import require_version
 
 from llmtuner.webui.components import (
     create_top,
     create_sft_tab,
     create_eval_tab,
-    create_infer_tab
+    create_infer_tab,
+    create_export_tab
 )
 from llmtuner.webui.css import CSS
 from llmtuner.webui.manager import Manager
 from llmtuner.webui.runner import Runner
 
 
 require_version("gradio>=3.36.0", "To fix: pip install gradio>=3.36.0")
@@ -26,15 +27,18 @@
 
         with gr.Tab("Evaluate"):
             eval_elems = create_eval_tab(top_elems, runner)
 
         with gr.Tab("Chat"):
             infer_elems = create_infer_tab(top_elems)
 
-        elem_list = [top_elems, sft_elems, eval_elems, infer_elems]
+        with gr.Tab("Export"):
+            export_elems = create_export_tab(top_elems)
+
+        elem_list = [top_elems, sft_elems, eval_elems, infer_elems, export_elems]
         manager = Manager(elem_list)
 
         demo.load(
             manager.gen_label,
             [top_elems["lang"]],
             [elem for elems in elem_list for elem in elems.values()],
         )
```

### Comparing `llmtuner-0.1.2/src/llmtuner/webui/locales.py` & `llmtuner-0.1.3/src/llmtuner/webui/locales.py`

 * *Files 2% similar despite different names*

```diff
@@ -448,14 +448,42 @@
     "temperature": {
         "en": {
             "label": "Temperature"
         },
         "zh": {
             "label": "温度系数"
         }
+    },
+    "save_dir": {
+        "en": {
+            "label": "Export dir",
+            "info": "Directory to save exported model."
+        },
+        "zh": {
+            "label": "导出目录",
+            "info": "保存导出模型的文件夹路径。"
+        }
+    },
+    "max_shard_size": {
+        "en": {
+            "label": "Max shard size (GB)",
+            "info": "The maximum size for a model file."
+        },
+        "zh": {
+            "label": "最大分块大小（GB）",
+            "info": "模型文件的最大大小。"
+        }
+    },
+    "export_btn": {
+        "en": {
+            "value": "Export"
+        },
+        "zh": {
+            "value": "开始导出"
+        }
     }
 }
 
 
 ALERTS = {
     "err_conflict": {
         "en": "A process is in running, please abort it firstly.",
@@ -473,14 +501,22 @@
         "en": "Model not found.",
         "zh": "模型未找到。"
     },
     "err_no_dataset": {
         "en": "Please choose a dataset.",
         "zh": "请选择数据集。"
     },
+    "err_no_checkpoint": {
+        "en": "Please select a checkpoint.",
+        "zh": "请选择断点。"
+    },
+    "err_no_save_dir": {
+        "en": "Please provide export dir.",
+        "zh": "请填写导出目录"
+    },
     "info_aborting": {
         "en": "Aborted, wait for terminating...",
         "zh": "训练中断，正在等待线程结束……"
     },
     "info_aborted": {
         "en": "Ready.",
         "zh": "准备就绪。"
@@ -500,9 +536,17 @@
     "info_loaded": {
         "en": "Model loaded, now you can chat with your model!",
         "zh": "模型已加载，可以开始聊天了！"
     },
     "info_unloaded": {
         "en": "Model unloaded.",
         "zh": "模型已卸载。"
+    },
+    "info_exporting": {
+        "en": "Exporting model...",
+        "zh": "正在导出模型……"
+    },
+    "info_exported": {
+        "en": "Model exported.",
+        "zh": "模型导出完成。"
     }
 }
```

### Comparing `llmtuner-0.1.2/src/llmtuner/webui/manager.py` & `llmtuner-0.1.3/src/llmtuner/webui/manager.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.1.2/src/llmtuner/webui/runner.py` & `llmtuner-0.1.3/src/llmtuner/webui/runner.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
 import os
 import threading
 import time
 import transformers
-from typing import List, Optional, Tuple
+from typing import Generator, List, Optional, Tuple
 
 from llmtuner.extras.callbacks import LogCallback
 from llmtuner.extras.constants import DEFAULT_MODULE
 from llmtuner.extras.logging import LoggerHandler
 from llmtuner.extras.misc import torch_gc
 from llmtuner.tuner import get_train_args, run_sft
 from llmtuner.webui.common import get_model_path, get_save_dir
@@ -21,15 +21,17 @@
         self.aborted = False
         self.running = False
 
     def set_abort(self):
         self.aborted = True
         self.running = False
 
-    def initialize(self, lang: str, model_name: str, dataset: list) -> Tuple[str, str, LoggerHandler, LogCallback]:
+    def initialize(
+        self, lang: str, model_name: str, dataset: List[str]
+    ) -> Tuple[str, str, LoggerHandler, LogCallback]:
         if self.running:
             return None, ALERTS["err_conflict"][lang], None, None
 
         if not model_name:
             return None, ALERTS["err_no_model"][lang], None, None
 
         model_name_or_path = get_model_path(model_name)
@@ -46,15 +48,17 @@
         logger_handler.setLevel(logging.INFO)
         logging.root.addHandler(logger_handler)
         transformers.logging.add_handler(logger_handler)
         trainer_callback = LogCallback(self)
 
         return model_name_or_path, "", logger_handler, trainer_callback
 
-    def finalize(self, lang: str, finish_info: Optional[str] = None) -> str:
+    def finalize(
+        self, lang: str, finish_info: Optional[str] = None
+    ) -> str:
         self.running = False
         torch_gc()
         if self.aborted:
             return ALERTS["info_aborted"][lang]
         else:
             return finish_info if finish_info is not None else ALERTS["info_finished"][lang]
 
@@ -83,15 +87,15 @@
         save_steps: int,
         warmup_steps: int,
         compute_type: str,
         lora_rank: int,
         lora_dropout: float,
         lora_target: str,
         output_dir: str
-    ):
+    ) -> Generator[str, None, None]:
         model_name_or_path, error, logger_handler, trainer_callback = self.initialize(lang, model_name, dataset)
         if error:
             yield error
             return
 
         if checkpoints:
             checkpoint_dir = ",".join(
@@ -170,15 +174,15 @@
         dataset_dir: str,
         dataset: List[str],
         max_source_length: int,
         max_target_length: int,
         max_samples: str,
         batch_size: int,
         predict: bool
-    ):
+    ) -> Generator[str, None, None]:
         model_name_or_path, error, logger_handler, trainer_callback = self.initialize(lang, model_name, dataset)
         if error:
             yield error
             return
 
         if checkpoints:
             checkpoint_dir = ",".join(
```

### Comparing `llmtuner-0.1.2/src/llmtuner.egg-info/PKG-INFO` & `llmtuner-0.1.3/src/llmtuner.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llmtuner
-Version: 0.1.2
+Version: 0.1.3
 Summary: Easy-to-use fine-tuning framework using PEFT
 Home-page: https://github.com/hiyouga/LLaMA-Efficient-Tuning
 Author: hiyouga
 Author-email: hiyouga@buaa.edu.cn
 License: Apache 2.0 License
 Keywords: LLaMA,BLOOM,Falcon,LLM,ChatGPT,transformer,pytorch,deep learning
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `llmtuner-0.1.2/src/llmtuner.egg-info/SOURCES.txt` & `llmtuner-0.1.3/src/llmtuner.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -61,10 +61,11 @@
 src/llmtuner/webui/manager.py
 src/llmtuner/webui/runner.py
 src/llmtuner/webui/utils.py
 src/llmtuner/webui/components/__init__.py
 src/llmtuner/webui/components/chatbot.py
 src/llmtuner/webui/components/data.py
 src/llmtuner/webui/components/eval.py
+src/llmtuner/webui/components/export.py
 src/llmtuner/webui/components/infer.py
 src/llmtuner/webui/components/sft.py
 src/llmtuner/webui/components/top.py
```

