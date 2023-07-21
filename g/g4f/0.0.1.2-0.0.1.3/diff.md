# Comparing `tmp/g4f-0.0.1.2.tar.gz` & `tmp/g4f-0.0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "g4f-0.0.1.2.tar", last modified: Mon Jul 17 23:14:52 2023, max compression
+gzip compressed data, was "g4f-0.0.1.3.tar", last modified: Fri Jul 21 20:44:02 2023, max compression
```

## Comparing `g4f-0.0.1.2.tar` & `g4f-0.0.1.3.tar`

### file list

```diff
@@ -1,20 +1,45 @@
-drwxr-xr-x   0 tek        (501) staff       (20)        0 2023-07-17 23:14:52.556352 g4f-0.0.1.2/
--rw-r--r--   0 tek        (501) staff       (20)    35149 2023-04-16 23:05:26.000000 g4f-0.0.1.2/LICENSE
--rw-r--r--   0 tek        (501) staff       (20)    19162 2023-07-17 23:14:52.556091 g4f-0.0.1.2/PKG-INFO
--rw-r--r--   0 tek        (501) staff       (20)    18414 2023-07-17 00:16:47.000000 g4f-0.0.1.2/README.md
-drwxr-xr-x   0 tek        (501) staff       (20)        0 2023-07-17 23:14:52.553658 g4f-0.0.1.2/g4f/
-drwxr-xr-x   0 tek        (501) staff       (20)        0 2023-07-17 23:14:52.555562 g4f-0.0.1.2/g4f/Provider/
--rw-r--r--   0 tek        (501) staff       (20)      501 2023-07-16 19:31:22.000000 g4f-0.0.1.2/g4f/Provider/Provider.py
--rw-r--r--   0 tek        (501) staff       (20)      353 2023-07-16 18:49:10.000000 g4f-0.0.1.2/g4f/Provider/__init__.py
--rw-r--r--   0 tek        (501) staff       (20)     1691 2023-07-16 19:31:26.000000 g4f-0.0.1.2/g4f/__init__.py
--rw-r--r--   0 tek        (501) staff       (20)     7561 2023-07-16 18:58:49.000000 g4f-0.0.1.2/g4f/models.py
--rw-r--r--   0 tek        (501) staff       (20)      110 2023-07-16 17:53:33.000000 g4f-0.0.1.2/g4f/typing.py
--rw-r--r--   0 tek        (501) staff       (20)     1700 2023-07-16 17:53:33.000000 g4f-0.0.1.2/g4f/utils.py
-drwxr-xr-x   0 tek        (501) staff       (20)        0 2023-07-17 23:14:52.554899 g4f-0.0.1.2/g4f.egg-info/
--rw-r--r--   0 tek        (501) staff       (20)    19162 2023-07-17 23:14:52.000000 g4f-0.0.1.2/g4f.egg-info/PKG-INFO
--rw-r--r--   0 tek        (501) staff       (20)      267 2023-07-17 23:14:52.000000 g4f-0.0.1.2/g4f.egg-info/SOURCES.txt
--rw-r--r--   0 tek        (501) staff       (20)        1 2023-07-17 23:14:52.000000 g4f-0.0.1.2/g4f.egg-info/dependency_links.txt
--rw-r--r--   0 tek        (501) staff       (20)       93 2023-07-17 23:14:52.000000 g4f-0.0.1.2/g4f.egg-info/requires.txt
--rw-r--r--   0 tek        (501) staff       (20)        4 2023-07-17 23:14:52.000000 g4f-0.0.1.2/g4f.egg-info/top_level.txt
--rw-r--r--   0 tek        (501) staff       (20)       38 2023-07-17 23:14:52.556500 g4f-0.0.1.2/setup.cfg
--rw-r--r--   0 tek        (501) staff       (20)     1318 2023-07-17 23:09:23.000000 g4f-0.0.1.2/setup.py
+drwxr-xr-x   0 tek        (501) staff       (20)        0 2023-07-21 20:44:02.692022 g4f-0.0.1.3/
+-rw-r--r--   0 tek        (501) staff       (20)    35149 2023-04-16 23:05:26.000000 g4f-0.0.1.3/LICENSE
+-rw-r--r--   0 tek        (501) staff       (20)    19188 2023-07-21 20:44:02.691728 g4f-0.0.1.3/PKG-INFO
+-rw-r--r--   0 tek        (501) staff       (20)    18440 2023-07-17 23:18:39.000000 g4f-0.0.1.3/README.md
+drwxr-xr-x   0 tek        (501) staff       (20)        0 2023-07-21 20:44:02.683951 g4f-0.0.1.3/g4f/
+drwxr-xr-x   0 tek        (501) staff       (20)        0 2023-07-21 20:44:02.685596 g4f-0.0.1.3/g4f/Provider/
+-rw-r--r--   0 tek        (501) staff       (20)      501 2023-07-16 19:31:22.000000 g4f-0.0.1.3/g4f/Provider/Provider.py
+drwxr-xr-x   0 tek        (501) staff       (20)        0 2023-07-21 20:44:02.691400 g4f-0.0.1.3/g4f/Provider/Providers/
+-rw-r--r--   0 tek        (501) staff       (20)     1411 2023-07-16 19:00:36.000000 g4f-0.0.1.3/g4f/Provider/Providers/AItianhu.py
+-rw-r--r--   0 tek        (501) staff       (20)     1362 2023-07-16 18:59:46.000000 g4f-0.0.1.3/g4f/Provider/Providers/Acytoo.py
+-rw-r--r--   0 tek        (501) staff       (20)     1243 2023-07-16 19:00:33.000000 g4f-0.0.1.3/g4f/Provider/Providers/AiService.py
+-rw-r--r--   0 tek        (501) staff       (20)     1578 2023-07-16 19:00:07.000000 g4f-0.0.1.3/g4f/Provider/Providers/Aichat.py
+-rw-r--r--   0 tek        (501) staff       (20)     3102 2023-07-16 19:00:12.000000 g4f-0.0.1.3/g4f/Provider/Providers/Ails.py
+-rw-r--r--   0 tek        (501) staff       (20)     2618 2023-07-16 19:01:02.000000 g4f-0.0.1.3/g4f/Provider/Providers/Bard.py
+-rw-r--r--   0 tek        (501) staff       (20)    13017 2023-07-16 19:01:09.000000 g4f-0.0.1.3/g4f/Provider/Providers/Bing.py
+-rw-r--r--   0 tek        (501) staff       (20)      952 2023-07-16 19:01:46.000000 g4f-0.0.1.3/g4f/Provider/Providers/BingHuan.py
+-rw-r--r--   0 tek        (501) staff       (20)     2033 2023-07-16 19:01:49.000000 g4f-0.0.1.3/g4f/Provider/Providers/ChatgptAi.py
+-rw-r--r--   0 tek        (501) staff       (20)     3763 2023-07-16 19:02:36.000000 g4f-0.0.1.3/g4f/Provider/Providers/ChatgptLogin.py
+-rw-r--r--   0 tek        (501) staff       (20)     1451 2023-07-16 19:02:54.000000 g4f-0.0.1.3/g4f/Provider/Providers/DeepAi.py
+-rw-r--r--   0 tek        (501) staff       (20)     2229 2023-07-21 20:42:14.000000 g4f-0.0.1.3/g4f/Provider/Providers/DfeHub.py
+-rw-r--r--   0 tek        (501) staff       (20)     1977 2023-07-16 19:03:36.000000 g4f-0.0.1.3/g4f/Provider/Providers/EasyChat.py
+-rw-r--r--   0 tek        (501) staff       (20)     1209 2023-07-16 19:03:41.000000 g4f-0.0.1.3/g4f/Provider/Providers/Forefront.py
+-rw-r--r--   0 tek        (501) staff       (20)     2178 2023-07-16 19:03:43.000000 g4f-0.0.1.3/g4f/Provider/Providers/GetGpt.py
+-rw-r--r--   0 tek        (501) staff       (20)     3761 2023-07-16 19:07:34.000000 g4f-0.0.1.3/g4f/Provider/Providers/H2o.py
+-rw-r--r--   0 tek        (501) staff       (20)     1728 2023-07-16 19:08:58.000000 g4f-0.0.1.3/g4f/Provider/Providers/Liaobots.py
+-rw-r--r--   0 tek        (501) staff       (20)     1396 2023-07-16 19:09:35.000000 g4f-0.0.1.3/g4f/Provider/Providers/Lockchat.py
+-rw-r--r--   0 tek        (501) staff       (20)      945 2023-07-17 00:24:27.000000 g4f-0.0.1.3/g4f/Provider/Providers/Theb.py
+-rw-r--r--   0 tek        (501) staff       (20)    17642 2023-07-16 19:30:13.000000 g4f-0.0.1.3/g4f/Provider/Providers/Vercel.py
+-rw-r--r--   0 tek        (501) staff       (20)     2640 2023-07-16 19:30:16.000000 g4f-0.0.1.3/g4f/Provider/Providers/Wewordle.py
+-rw-r--r--   0 tek        (501) staff       (20)      654 2023-07-16 19:30:07.000000 g4f-0.0.1.3/g4f/Provider/Providers/You.py
+-rw-r--r--   0 tek        (501) staff       (20)     1394 2023-07-16 19:30:48.000000 g4f-0.0.1.3/g4f/Provider/Providers/Yqcloud.py
+-rw-r--r--   0 tek        (501) staff       (20)        0 2023-07-21 20:42:14.000000 g4f-0.0.1.3/g4f/Provider/Providers/__init__.py
+-rw-r--r--   0 tek        (501) staff       (20)      353 2023-07-16 18:49:10.000000 g4f-0.0.1.3/g4f/Provider/__init__.py
+-rw-r--r--   0 tek        (501) staff       (20)     1691 2023-07-16 19:31:26.000000 g4f-0.0.1.3/g4f/__init__.py
+-rw-r--r--   0 tek        (501) staff       (20)     7561 2023-07-16 18:58:49.000000 g4f-0.0.1.3/g4f/models.py
+-rw-r--r--   0 tek        (501) staff       (20)      110 2023-07-16 17:53:33.000000 g4f-0.0.1.3/g4f/typing.py
+-rw-r--r--   0 tek        (501) staff       (20)     1700 2023-07-16 17:53:33.000000 g4f-0.0.1.3/g4f/utils.py
+drwxr-xr-x   0 tek        (501) staff       (20)        0 2023-07-21 20:44:02.685097 g4f-0.0.1.3/g4f.egg-info/
+-rw-r--r--   0 tek        (501) staff       (20)    19188 2023-07-21 20:44:02.000000 g4f-0.0.1.3/g4f.egg-info/PKG-INFO
+-rw-r--r--   0 tek        (501) staff       (20)     1075 2023-07-21 20:44:02.000000 g4f-0.0.1.3/g4f.egg-info/SOURCES.txt
+-rw-r--r--   0 tek        (501) staff       (20)        1 2023-07-21 20:44:02.000000 g4f-0.0.1.3/g4f.egg-info/dependency_links.txt
+-rw-r--r--   0 tek        (501) staff       (20)       84 2023-07-21 20:44:02.000000 g4f-0.0.1.3/g4f.egg-info/requires.txt
+-rw-r--r--   0 tek        (501) staff       (20)        4 2023-07-21 20:44:02.000000 g4f-0.0.1.3/g4f.egg-info/top_level.txt
+-rw-r--r--   0 tek        (501) staff       (20)       38 2023-07-21 20:44:02.692107 g4f-0.0.1.3/setup.cfg
+-rw-r--r--   0 tek        (501) staff       (20)     1318 2023-07-21 20:43:58.000000 g4f-0.0.1.3/setup.py
```

### Comparing `g4f-0.0.1.2/LICENSE` & `g4f-0.0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `g4f-0.0.1.2/PKG-INFO` & `g4f-0.0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: g4f
-Version: 0.0.1.2
+Version: 0.0.1.3
 Summary: The official gpt4free repository | various collection of powerful language models
 Author: Tekky
 Author-email: <support@g4f.ai>
 Keywords: python,chatbot,reverse-engineering,openai,chatbots,gpt,language-model,gpt-3,gpt3,openai-api,gpt-4,gpt4,chatgpt,chatgpt-api,openai-chatgpt,chatgpt-free,chatgpt-4,chatgpt4,chatgpt4-api,free,free-gpt,gpt4free,g4f
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -21,15 +21,15 @@
 
 This (quite censored) New Version of gpt4free, was just released, it may contain bugs, open an issue or contribute a PR when encountering one, some features were disabled.
 Docker is for now not available but I would be happy if someone contributes a PR. The g4f GUI will be uploaded soon enough.
 
 ### New
 - pypi package:
 ```
-pip install g4f
+pip install -U g4f
 ```
 
 ## Table of Contents:
 
 - [Getting Started](#getting-started)
     + [Prerequisites](#prerequisites)
     + [Setting up the project](#setting-up-the-project)
@@ -50,15 +50,15 @@
 
 #### Prerequisites:
 1. [Download and install Python](https://www.python.org/downloads/) (Version 3.x is recommended).
 
 #### Setting up the project:
 ##### Install using pypi
 ```
-pip install g4f
+pip install -U g4f
 ```
 
 ##### or
 
 1. Clone the GitHub repository: 
 ```
 git clone https://github.com/xtekky/gpt4free.git
@@ -174,39 +174,39 @@
         print(content)
 ```
 
 ## Models
 
 ### gpt-3.5 / gpt-4
 
-| Website| Provider| gpt-3.5 | gpt-4 | Streaming | Status | Auth |
+| Website| Provider| gpt-3.5 | gpt-4 | Stream | Status | Auth |
 | --- | --- | --- | --- | --- | --- | --- |
-| [ai.ls](https://ai.ls) | `g4f.ProviderAils` | ✔️ | ❌ | ✔️ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
-| [you.com](https://you.com) | `g4f.ProviderYou` | ✔️ | ❌ | ✔️ | ![Inactive](https://img.shields.io/badge/Inactive-red) | ❌ |
-| [bing.com](https://bing.com/chat) | `g4f.ProviderBing` | ❌ | ✔️ | ✔️ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
-| [chat9.yqcloud.top](https://chat9.yqcloud.top/) | `g4f.ProviderYqcloud` | ✔️ | ❌ | ✔️ | ![Inactive](https://img.shields.io/badge/Inactive-red) | ❌ |
-| [theb.ai](https://theb.ai) | `g4f.ProviderTheb` | ✔️ | ❌ | ✔️ | ![Inactive](https://img.shields.io/badge/Inactive-red) | ❌ |
-| [chat-gpt.org](https://chat-gpt.org/chat) | `g4f.ProviderAichat` | ✔️ | ❌ | ❌ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
-| [bard.google.com](https://bard.google.com) | `g4f.ProviderBard` | ❌ | ❌ | ❌ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ✔️ |
-| [play.vercel.ai](https://play.vercel.ai) | `g4f.ProviderVercel` | ✔️ | ❌ | ✔️ | ![Inactive](https://img.shields.io/badge/Inactive-red) | ❌ |
-| [forefront.com](https://forefront.com) | `g4f.ProviderForefront` | ✔️ | ❌ | ✔️ | ![Inactive](https://img.shields.io/badge/Inactive-red) | ❌ |
-| [supertest.lockchat.app](http://supertest.lockchat.app) | `g4f.ProviderLockchat` | ✔️ | ✔️ | ✔️ | ![Inactive](https://img.shields.io/badge/Inactive-red) | ❌ |
-| [liaobots.com](https://liaobots.com) | `g4f.ProviderLiaobots` | ✔️ | ✔️ | ✔️ | ![Inactive](https://img.shields.io/badge/Inactive-red) | ✔️ |
-| [gpt-gm.h2o.ai](https://gpt-gm.h2o.ai) | `g4f.ProviderH2o` | ❌ | ❌ | ✔️ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
-| [chatgptlogin.ac](https://chatgptlogin.ac) | `g4f.ProviderChatgptLogin` | ✔️ | ❌ | ❌ | ![Inactive](https://img.shields.io/badge/Inactive-red) | ❌ |
-| [deepai.org](https://deepai.org) | `g4f.ProviderDeepAi` | ✔️ | ❌ | ✔️ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
-| [chat.getgpt.world](https://chat.getgpt.world/) | `g4f.ProviderGetGpt` | ✔️ | ❌ | ✔️ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
-| [www.aitianhu.com](https://www.aitianhu.com/api/chat-process) | `g4f.ProviderAItianhu` | ✔️ | ❌ | ❌ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
-| [free.easychat.work](https://free.easychat.work) | `g4f.ProviderEasyChat` | ✔️ | ❌ | ✔️ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
-| [chat.acytoo.com](https://chat.acytoo.com/api/completions) | `g4f.ProviderAcytoo` | ✔️ | ❌ | ❌ | ![Inactive](https://img.shields.io/badge/Inactive-red) | ❌ |
-| [chat.dfehub.com](https://chat.dfehub.com/api/chat) | `g4f.ProviderDfeHub` | ✔️ | ❌ | ✔️ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
-| [aiservice.vercel.app](https://aiservice.vercel.app/api/chat/answer) | `g4f.ProviderAiService` | ✔️ | ❌ | ❌ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
-| [b.ai-huan.xyz](https://b.ai-huan.xyz) | `g4f.ProviderBingHuan` | ✔️ | ✔️ | ✔️ | ![Inactive](https://img.shields.io/badge/Inactive-red) | ❌ |
-| [wewordle.org](https://wewordle.org/gptapi/v1/android/turbo) | `g4f.ProviderWewordle` | ✔️ | ❌ | ❌ | ![Inactive](https://img.shields.io/badge/Inactive-red) | ❌ |
-| [chatgpt.ai](https://chatgpt.ai/gpt-4/) | `g4f.ProviderChatgptAi` | ❌ | ✔️ | ❌ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
+| [ai.ls](https://ai.ls) | `g4f.Provider.Ails` | ✔️ | ❌ | ✔️ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
+| [you.com](https://you.com) | `g4f.Provider.You` | ✔️ | ❌ | ✔️ | ![Inactive](https://img.shields.io/badge/Inactive-red) | ❌ |
+| [bing.com](https://bing.com/chat) | `g4f.Provider.Bing` | ❌ | ✔️ | ✔️ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
+| [chat9.yqcloud.top](https://chat9.yqcloud.top/) | `g4f.Provider.Yqcloud` | ✔️ | ❌ | ✔️ | ![Inactive](https://img.shields.io/badge/Inactive-red) | ❌ |
+| [theb.ai](https://theb.ai) | `g4f.Provider.Theb` | ✔️ | ❌ | ✔️ | ![Inactive](https://img.shields.io/badge/Inactive-red) | ❌ |
+| [chat-gpt.org](https://chat-gpt.org/chat) | `g4f.Provider.Aichat` | ✔️ | ❌ | ❌ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
+| [bard.google.com](https://bard.google.com) | `g4f.Provider.Bard` | ❌ | ❌ | ❌ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ✔️ |
+| [play.vercel.ai](https://play.vercel.ai) | `g4f.Provider.Vercel` | ✔️ | ❌ | ✔️ | ![Inactive](https://img.shields.io/badge/Inactive-red) | ❌ |
+| [forefront.com](https://forefront.com) | `g4f.Provider.Forefront` | ✔️ | ❌ | ✔️ | ![Inactive](https://img.shields.io/badge/Inactive-red) | ❌ |
+| [supertest.lockchat.app](http://supertest.lockchat.app) | `g4f.Provider.Lockchat` | ✔️ | ✔️ | ✔️ | ![Inactive](https://img.shields.io/badge/Inactive-red) | ❌ |
+| [liaobots.com](https://liaobots.com) | `g4f.Provider.Liaobots` | ✔️ | ✔️ | ✔️ | ![Inactive](https://img.shields.io/badge/Inactive-red) | ✔️ |
+| [gpt-gm.h2o.ai](https://gpt-gm.h2o.ai) | `g4f.Provider.H2o` | ❌ | ❌ | ✔️ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
+| [chatgptlogin.ac](https://chatgptlogin.ac) | `g4f.Provider.ChatgptLogin` | ✔️ | ❌ | ❌ | ![Inactive](https://img.shields.io/badge/Inactive-red) | ❌ |
+| [deepai.org](https://deepai.org) | `g4f.Provider.DeepAi` | ✔️ | ❌ | ✔️ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
+| [chat.getgpt.world](https://chat.getgpt.world/) | `g4f.Provider.GetGpt` | ✔️ | ❌ | ✔️ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
+| [www.aitianhu.com](https://www.aitianhu.com/api/chat-process) | `g4f.Provider.AItianhu` | ✔️ | ❌ | ❌ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
+| [free.easychat.work](https://free.easychat.work) | `g4f.Provider.EasyChat` | ✔️ | ❌ | ✔️ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
+| [chat.acytoo.com](https://chat.acytoo.com/api/completions) | `g4f.Provider.Acytoo` | ✔️ | ❌ | ❌ | ![Inactive](https://img.shields.io/badge/Inactive-red) | ❌ |
+| [chat.dfehub.com](https://chat.dfehub.com/api/chat) | `g4f.Provider.DfeHub` | ✔️ | ❌ | ✔️ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
+| [aiservice.vercel.app](https://aiservice.vercel.app/api/chat/answer) | `g4f.Provider.AiService` | ✔️ | ❌ | ❌ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
+| [b.ai-huan.xyz](https://b.ai-huan.xyz) | `g4f.Provider.BingHuan` | ✔️ | ✔️ | ✔️ | ![Inactive](https://img.shields.io/badge/Inactive-red) | ❌ |
+| [wewordle.org](https://wewordle.org/gptapi/v1/android/turbo) | `g4f.Provider.Wewordle` | ✔️ | ❌ | ❌ | ![Inactive](https://img.shields.io/badge/Inactive-red) | ❌ |
+| [chatgpt.ai](https://chatgpt.ai/gpt-4/) | `g4f.Provider.ChatgptAi` | ❌ | ✔️ | ❌ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
 
 
 ### Other Models
 
 | Model| Base Provider | Provider | Website |
 | ------- | ----------- | ---- |---- |
 | palm2 | Google | `g4f.Provider.Bard` | [bard.google.com](https://bard.google.com/) |
```

### Comparing `g4f-0.0.1.2/README.md` & `g4f-0.0.1.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 This (quite censored) New Version of gpt4free, was just released, it may contain bugs, open an issue or contribute a PR when encountering one, some features were disabled.
 Docker is for now not available but I would be happy if someone contributes a PR. The g4f GUI will be uploaded soon enough.
 
 ### New
 - pypi package:
 ```
-pip install g4f
+pip install -U g4f
 ```
 
 ## Table of Contents:
 
 - [Getting Started](#getting-started)
     + [Prerequisites](#prerequisites)
     + [Setting up the project](#setting-up-the-project)
@@ -33,15 +33,15 @@
 
 #### Prerequisites:
 1. [Download and install Python](https://www.python.org/downloads/) (Version 3.x is recommended).
 
 #### Setting up the project:
 ##### Install using pypi
 ```
-pip install g4f
+pip install -U g4f
 ```
 
 ##### or
 
 1. Clone the GitHub repository: 
 ```
 git clone https://github.com/xtekky/gpt4free.git
@@ -157,39 +157,39 @@
         print(content)
 ```
 
 ## Models
 
 ### gpt-3.5 / gpt-4
 
-| Website| Provider| gpt-3.5 | gpt-4 | Streaming | Status | Auth |
+| Website| Provider| gpt-3.5 | gpt-4 | Stream | Status | Auth |
 | --- | --- | --- | --- | --- | --- | --- |
-| [ai.ls](https://ai.ls) | `g4f.ProviderAils` | ✔️ | ❌ | ✔️ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
-| [you.com](https://you.com) | `g4f.ProviderYou` | ✔️ | ❌ | ✔️ | ![Inactive](https://img.shields.io/badge/Inactive-red) | ❌ |
-| [bing.com](https://bing.com/chat) | `g4f.ProviderBing` | ❌ | ✔️ | ✔️ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
-| [chat9.yqcloud.top](https://chat9.yqcloud.top/) | `g4f.ProviderYqcloud` | ✔️ | ❌ | ✔️ | ![Inactive](https://img.shields.io/badge/Inactive-red) | ❌ |
-| [theb.ai](https://theb.ai) | `g4f.ProviderTheb` | ✔️ | ❌ | ✔️ | ![Inactive](https://img.shields.io/badge/Inactive-red) | ❌ |
-| [chat-gpt.org](https://chat-gpt.org/chat) | `g4f.ProviderAichat` | ✔️ | ❌ | ❌ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
-| [bard.google.com](https://bard.google.com) | `g4f.ProviderBard` | ❌ | ❌ | ❌ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ✔️ |
-| [play.vercel.ai](https://play.vercel.ai) | `g4f.ProviderVercel` | ✔️ | ❌ | ✔️ | ![Inactive](https://img.shields.io/badge/Inactive-red) | ❌ |
-| [forefront.com](https://forefront.com) | `g4f.ProviderForefront` | ✔️ | ❌ | ✔️ | ![Inactive](https://img.shields.io/badge/Inactive-red) | ❌ |
-| [supertest.lockchat.app](http://supertest.lockchat.app) | `g4f.ProviderLockchat` | ✔️ | ✔️ | ✔️ | ![Inactive](https://img.shields.io/badge/Inactive-red) | ❌ |
-| [liaobots.com](https://liaobots.com) | `g4f.ProviderLiaobots` | ✔️ | ✔️ | ✔️ | ![Inactive](https://img.shields.io/badge/Inactive-red) | ✔️ |
-| [gpt-gm.h2o.ai](https://gpt-gm.h2o.ai) | `g4f.ProviderH2o` | ❌ | ❌ | ✔️ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
-| [chatgptlogin.ac](https://chatgptlogin.ac) | `g4f.ProviderChatgptLogin` | ✔️ | ❌ | ❌ | ![Inactive](https://img.shields.io/badge/Inactive-red) | ❌ |
-| [deepai.org](https://deepai.org) | `g4f.ProviderDeepAi` | ✔️ | ❌ | ✔️ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
-| [chat.getgpt.world](https://chat.getgpt.world/) | `g4f.ProviderGetGpt` | ✔️ | ❌ | ✔️ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
-| [www.aitianhu.com](https://www.aitianhu.com/api/chat-process) | `g4f.ProviderAItianhu` | ✔️ | ❌ | ❌ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
-| [free.easychat.work](https://free.easychat.work) | `g4f.ProviderEasyChat` | ✔️ | ❌ | ✔️ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
-| [chat.acytoo.com](https://chat.acytoo.com/api/completions) | `g4f.ProviderAcytoo` | ✔️ | ❌ | ❌ | ![Inactive](https://img.shields.io/badge/Inactive-red) | ❌ |
-| [chat.dfehub.com](https://chat.dfehub.com/api/chat) | `g4f.ProviderDfeHub` | ✔️ | ❌ | ✔️ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
-| [aiservice.vercel.app](https://aiservice.vercel.app/api/chat/answer) | `g4f.ProviderAiService` | ✔️ | ❌ | ❌ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
-| [b.ai-huan.xyz](https://b.ai-huan.xyz) | `g4f.ProviderBingHuan` | ✔️ | ✔️ | ✔️ | ![Inactive](https://img.shields.io/badge/Inactive-red) | ❌ |
-| [wewordle.org](https://wewordle.org/gptapi/v1/android/turbo) | `g4f.ProviderWewordle` | ✔️ | ❌ | ❌ | ![Inactive](https://img.shields.io/badge/Inactive-red) | ❌ |
-| [chatgpt.ai](https://chatgpt.ai/gpt-4/) | `g4f.ProviderChatgptAi` | ❌ | ✔️ | ❌ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
+| [ai.ls](https://ai.ls) | `g4f.Provider.Ails` | ✔️ | ❌ | ✔️ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
+| [you.com](https://you.com) | `g4f.Provider.You` | ✔️ | ❌ | ✔️ | ![Inactive](https://img.shields.io/badge/Inactive-red) | ❌ |
+| [bing.com](https://bing.com/chat) | `g4f.Provider.Bing` | ❌ | ✔️ | ✔️ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
+| [chat9.yqcloud.top](https://chat9.yqcloud.top/) | `g4f.Provider.Yqcloud` | ✔️ | ❌ | ✔️ | ![Inactive](https://img.shields.io/badge/Inactive-red) | ❌ |
+| [theb.ai](https://theb.ai) | `g4f.Provider.Theb` | ✔️ | ❌ | ✔️ | ![Inactive](https://img.shields.io/badge/Inactive-red) | ❌ |
+| [chat-gpt.org](https://chat-gpt.org/chat) | `g4f.Provider.Aichat` | ✔️ | ❌ | ❌ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
+| [bard.google.com](https://bard.google.com) | `g4f.Provider.Bard` | ❌ | ❌ | ❌ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ✔️ |
+| [play.vercel.ai](https://play.vercel.ai) | `g4f.Provider.Vercel` | ✔️ | ❌ | ✔️ | ![Inactive](https://img.shields.io/badge/Inactive-red) | ❌ |
+| [forefront.com](https://forefront.com) | `g4f.Provider.Forefront` | ✔️ | ❌ | ✔️ | ![Inactive](https://img.shields.io/badge/Inactive-red) | ❌ |
+| [supertest.lockchat.app](http://supertest.lockchat.app) | `g4f.Provider.Lockchat` | ✔️ | ✔️ | ✔️ | ![Inactive](https://img.shields.io/badge/Inactive-red) | ❌ |
+| [liaobots.com](https://liaobots.com) | `g4f.Provider.Liaobots` | ✔️ | ✔️ | ✔️ | ![Inactive](https://img.shields.io/badge/Inactive-red) | ✔️ |
+| [gpt-gm.h2o.ai](https://gpt-gm.h2o.ai) | `g4f.Provider.H2o` | ❌ | ❌ | ✔️ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
+| [chatgptlogin.ac](https://chatgptlogin.ac) | `g4f.Provider.ChatgptLogin` | ✔️ | ❌ | ❌ | ![Inactive](https://img.shields.io/badge/Inactive-red) | ❌ |
+| [deepai.org](https://deepai.org) | `g4f.Provider.DeepAi` | ✔️ | ❌ | ✔️ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
+| [chat.getgpt.world](https://chat.getgpt.world/) | `g4f.Provider.GetGpt` | ✔️ | ❌ | ✔️ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
+| [www.aitianhu.com](https://www.aitianhu.com/api/chat-process) | `g4f.Provider.AItianhu` | ✔️ | ❌ | ❌ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
+| [free.easychat.work](https://free.easychat.work) | `g4f.Provider.EasyChat` | ✔️ | ❌ | ✔️ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
+| [chat.acytoo.com](https://chat.acytoo.com/api/completions) | `g4f.Provider.Acytoo` | ✔️ | ❌ | ❌ | ![Inactive](https://img.shields.io/badge/Inactive-red) | ❌ |
+| [chat.dfehub.com](https://chat.dfehub.com/api/chat) | `g4f.Provider.DfeHub` | ✔️ | ❌ | ✔️ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
+| [aiservice.vercel.app](https://aiservice.vercel.app/api/chat/answer) | `g4f.Provider.AiService` | ✔️ | ❌ | ❌ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
+| [b.ai-huan.xyz](https://b.ai-huan.xyz) | `g4f.Provider.BingHuan` | ✔️ | ✔️ | ✔️ | ![Inactive](https://img.shields.io/badge/Inactive-red) | ❌ |
+| [wewordle.org](https://wewordle.org/gptapi/v1/android/turbo) | `g4f.Provider.Wewordle` | ✔️ | ❌ | ❌ | ![Inactive](https://img.shields.io/badge/Inactive-red) | ❌ |
+| [chatgpt.ai](https://chatgpt.ai/gpt-4/) | `g4f.Provider.ChatgptAi` | ❌ | ✔️ | ❌ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
 
 
 ### Other Models
 
 | Model| Base Provider | Provider | Website |
 | ------- | ----------- | ---- |---- |
 | palm2 | Google | `g4f.Provider.Bard` | [bard.google.com](https://bard.google.com/) |
```

### Comparing `g4f-0.0.1.2/g4f/__init__.py` & `g4f-0.0.1.3/g4f/__init__.py`

 * *Files identical despite different names*

### Comparing `g4f-0.0.1.2/g4f/models.py` & `g4f-0.0.1.3/g4f/models.py`

 * *Files identical despite different names*

### Comparing `g4f-0.0.1.2/g4f/utils.py` & `g4f-0.0.1.3/g4f/utils.py`

 * *Files identical despite different names*

### Comparing `g4f-0.0.1.2/g4f.egg-info/PKG-INFO` & `g4f-0.0.1.3/g4f.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: g4f
-Version: 0.0.1.2
+Version: 0.0.1.3
 Summary: The official gpt4free repository | various collection of powerful language models
 Author: Tekky
 Author-email: <support@g4f.ai>
 Keywords: python,chatbot,reverse-engineering,openai,chatbots,gpt,language-model,gpt-3,gpt3,openai-api,gpt-4,gpt4,chatgpt,chatgpt-api,openai-chatgpt,chatgpt-free,chatgpt-4,chatgpt4,chatgpt4-api,free,free-gpt,gpt4free,g4f
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -21,15 +21,15 @@
 
 This (quite censored) New Version of gpt4free, was just released, it may contain bugs, open an issue or contribute a PR when encountering one, some features were disabled.
 Docker is for now not available but I would be happy if someone contributes a PR. The g4f GUI will be uploaded soon enough.
 
 ### New
 - pypi package:
 ```
-pip install g4f
+pip install -U g4f
 ```
 
 ## Table of Contents:
 
 - [Getting Started](#getting-started)
     + [Prerequisites](#prerequisites)
     + [Setting up the project](#setting-up-the-project)
@@ -50,15 +50,15 @@
 
 #### Prerequisites:
 1. [Download and install Python](https://www.python.org/downloads/) (Version 3.x is recommended).
 
 #### Setting up the project:
 ##### Install using pypi
 ```
-pip install g4f
+pip install -U g4f
 ```
 
 ##### or
 
 1. Clone the GitHub repository: 
 ```
 git clone https://github.com/xtekky/gpt4free.git
@@ -174,39 +174,39 @@
         print(content)
 ```
 
 ## Models
 
 ### gpt-3.5 / gpt-4
 
-| Website| Provider| gpt-3.5 | gpt-4 | Streaming | Status | Auth |
+| Website| Provider| gpt-3.5 | gpt-4 | Stream | Status | Auth |
 | --- | --- | --- | --- | --- | --- | --- |
-| [ai.ls](https://ai.ls) | `g4f.ProviderAils` | ✔️ | ❌ | ✔️ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
-| [you.com](https://you.com) | `g4f.ProviderYou` | ✔️ | ❌ | ✔️ | ![Inactive](https://img.shields.io/badge/Inactive-red) | ❌ |
-| [bing.com](https://bing.com/chat) | `g4f.ProviderBing` | ❌ | ✔️ | ✔️ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
-| [chat9.yqcloud.top](https://chat9.yqcloud.top/) | `g4f.ProviderYqcloud` | ✔️ | ❌ | ✔️ | ![Inactive](https://img.shields.io/badge/Inactive-red) | ❌ |
-| [theb.ai](https://theb.ai) | `g4f.ProviderTheb` | ✔️ | ❌ | ✔️ | ![Inactive](https://img.shields.io/badge/Inactive-red) | ❌ |
-| [chat-gpt.org](https://chat-gpt.org/chat) | `g4f.ProviderAichat` | ✔️ | ❌ | ❌ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
-| [bard.google.com](https://bard.google.com) | `g4f.ProviderBard` | ❌ | ❌ | ❌ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ✔️ |
-| [play.vercel.ai](https://play.vercel.ai) | `g4f.ProviderVercel` | ✔️ | ❌ | ✔️ | ![Inactive](https://img.shields.io/badge/Inactive-red) | ❌ |
-| [forefront.com](https://forefront.com) | `g4f.ProviderForefront` | ✔️ | ❌ | ✔️ | ![Inactive](https://img.shields.io/badge/Inactive-red) | ❌ |
-| [supertest.lockchat.app](http://supertest.lockchat.app) | `g4f.ProviderLockchat` | ✔️ | ✔️ | ✔️ | ![Inactive](https://img.shields.io/badge/Inactive-red) | ❌ |
-| [liaobots.com](https://liaobots.com) | `g4f.ProviderLiaobots` | ✔️ | ✔️ | ✔️ | ![Inactive](https://img.shields.io/badge/Inactive-red) | ✔️ |
-| [gpt-gm.h2o.ai](https://gpt-gm.h2o.ai) | `g4f.ProviderH2o` | ❌ | ❌ | ✔️ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
-| [chatgptlogin.ac](https://chatgptlogin.ac) | `g4f.ProviderChatgptLogin` | ✔️ | ❌ | ❌ | ![Inactive](https://img.shields.io/badge/Inactive-red) | ❌ |
-| [deepai.org](https://deepai.org) | `g4f.ProviderDeepAi` | ✔️ | ❌ | ✔️ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
-| [chat.getgpt.world](https://chat.getgpt.world/) | `g4f.ProviderGetGpt` | ✔️ | ❌ | ✔️ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
-| [www.aitianhu.com](https://www.aitianhu.com/api/chat-process) | `g4f.ProviderAItianhu` | ✔️ | ❌ | ❌ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
-| [free.easychat.work](https://free.easychat.work) | `g4f.ProviderEasyChat` | ✔️ | ❌ | ✔️ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
-| [chat.acytoo.com](https://chat.acytoo.com/api/completions) | `g4f.ProviderAcytoo` | ✔️ | ❌ | ❌ | ![Inactive](https://img.shields.io/badge/Inactive-red) | ❌ |
-| [chat.dfehub.com](https://chat.dfehub.com/api/chat) | `g4f.ProviderDfeHub` | ✔️ | ❌ | ✔️ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
-| [aiservice.vercel.app](https://aiservice.vercel.app/api/chat/answer) | `g4f.ProviderAiService` | ✔️ | ❌ | ❌ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
-| [b.ai-huan.xyz](https://b.ai-huan.xyz) | `g4f.ProviderBingHuan` | ✔️ | ✔️ | ✔️ | ![Inactive](https://img.shields.io/badge/Inactive-red) | ❌ |
-| [wewordle.org](https://wewordle.org/gptapi/v1/android/turbo) | `g4f.ProviderWewordle` | ✔️ | ❌ | ❌ | ![Inactive](https://img.shields.io/badge/Inactive-red) | ❌ |
-| [chatgpt.ai](https://chatgpt.ai/gpt-4/) | `g4f.ProviderChatgptAi` | ❌ | ✔️ | ❌ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
+| [ai.ls](https://ai.ls) | `g4f.Provider.Ails` | ✔️ | ❌ | ✔️ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
+| [you.com](https://you.com) | `g4f.Provider.You` | ✔️ | ❌ | ✔️ | ![Inactive](https://img.shields.io/badge/Inactive-red) | ❌ |
+| [bing.com](https://bing.com/chat) | `g4f.Provider.Bing` | ❌ | ✔️ | ✔️ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
+| [chat9.yqcloud.top](https://chat9.yqcloud.top/) | `g4f.Provider.Yqcloud` | ✔️ | ❌ | ✔️ | ![Inactive](https://img.shields.io/badge/Inactive-red) | ❌ |
+| [theb.ai](https://theb.ai) | `g4f.Provider.Theb` | ✔️ | ❌ | ✔️ | ![Inactive](https://img.shields.io/badge/Inactive-red) | ❌ |
+| [chat-gpt.org](https://chat-gpt.org/chat) | `g4f.Provider.Aichat` | ✔️ | ❌ | ❌ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
+| [bard.google.com](https://bard.google.com) | `g4f.Provider.Bard` | ❌ | ❌ | ❌ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ✔️ |
+| [play.vercel.ai](https://play.vercel.ai) | `g4f.Provider.Vercel` | ✔️ | ❌ | ✔️ | ![Inactive](https://img.shields.io/badge/Inactive-red) | ❌ |
+| [forefront.com](https://forefront.com) | `g4f.Provider.Forefront` | ✔️ | ❌ | ✔️ | ![Inactive](https://img.shields.io/badge/Inactive-red) | ❌ |
+| [supertest.lockchat.app](http://supertest.lockchat.app) | `g4f.Provider.Lockchat` | ✔️ | ✔️ | ✔️ | ![Inactive](https://img.shields.io/badge/Inactive-red) | ❌ |
+| [liaobots.com](https://liaobots.com) | `g4f.Provider.Liaobots` | ✔️ | ✔️ | ✔️ | ![Inactive](https://img.shields.io/badge/Inactive-red) | ✔️ |
+| [gpt-gm.h2o.ai](https://gpt-gm.h2o.ai) | `g4f.Provider.H2o` | ❌ | ❌ | ✔️ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
+| [chatgptlogin.ac](https://chatgptlogin.ac) | `g4f.Provider.ChatgptLogin` | ✔️ | ❌ | ❌ | ![Inactive](https://img.shields.io/badge/Inactive-red) | ❌ |
+| [deepai.org](https://deepai.org) | `g4f.Provider.DeepAi` | ✔️ | ❌ | ✔️ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
+| [chat.getgpt.world](https://chat.getgpt.world/) | `g4f.Provider.GetGpt` | ✔️ | ❌ | ✔️ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
+| [www.aitianhu.com](https://www.aitianhu.com/api/chat-process) | `g4f.Provider.AItianhu` | ✔️ | ❌ | ❌ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
+| [free.easychat.work](https://free.easychat.work) | `g4f.Provider.EasyChat` | ✔️ | ❌ | ✔️ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
+| [chat.acytoo.com](https://chat.acytoo.com/api/completions) | `g4f.Provider.Acytoo` | ✔️ | ❌ | ❌ | ![Inactive](https://img.shields.io/badge/Inactive-red) | ❌ |
+| [chat.dfehub.com](https://chat.dfehub.com/api/chat) | `g4f.Provider.DfeHub` | ✔️ | ❌ | ✔️ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
+| [aiservice.vercel.app](https://aiservice.vercel.app/api/chat/answer) | `g4f.Provider.AiService` | ✔️ | ❌ | ❌ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
+| [b.ai-huan.xyz](https://b.ai-huan.xyz) | `g4f.Provider.BingHuan` | ✔️ | ✔️ | ✔️ | ![Inactive](https://img.shields.io/badge/Inactive-red) | ❌ |
+| [wewordle.org](https://wewordle.org/gptapi/v1/android/turbo) | `g4f.Provider.Wewordle` | ✔️ | ❌ | ❌ | ![Inactive](https://img.shields.io/badge/Inactive-red) | ❌ |
+| [chatgpt.ai](https://chatgpt.ai/gpt-4/) | `g4f.Provider.ChatgptAi` | ❌ | ✔️ | ❌ | ![Active](https://img.shields.io/badge/Active-brightgreen) | ❌ |
 
 
 ### Other Models
 
 | Model| Base Provider | Provider | Website |
 | ------- | ----------- | ---- |---- |
 | palm2 | Google | `g4f.Provider.Bard` | [bard.google.com](https://bard.google.com/) |
```

### Comparing `g4f-0.0.1.2/setup.py` & `g4f-0.0.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
     
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
-VERSION = '0.0.1.2'
+VERSION = '0.0.1.3'
 DESCRIPTION = 'The official gpt4free repository | various collection of powerful language models'
 
 # Setting up
 setup(
     name="g4f",
     version=VERSION,
     author="Tekky",
```

