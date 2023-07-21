# Comparing `tmp/pxgpt-0.0.0rc0.tar.gz` & `tmp/pxgpt-0.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pxgpt-0.0.0rc0.tar", max compression
+gzip compressed data, was "pxgpt-0.0.0rc1.tar", max compression
```

## Comparing `pxgpt-0.0.0rc0.tar` & `pxgpt-0.0.0rc1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0      546 2023-07-19 17:37:26.250723 pxgpt-0.0.0rc0/LICENSE
--rw-r--r--   0        0        0     6898 2023-07-19 17:37:26.250723 pxgpt-0.0.0rc0/README.md
--rw-r--r--   0        0        0       53 2023-07-19 17:37:26.254722 pxgpt-0.0.0rc0/pxgpt/__init__.py
--rw-r--r--   0        0        0       61 2023-07-19 17:37:26.254722 pxgpt-0.0.0rc0/pxgpt/__main__.py
--rw-r--r--   0        0        0    14744 2023-07-19 17:37:26.254722 pxgpt-0.0.0rc0/pxgpt/chat.py
--rw-r--r--   0        0        0     2881 2023-07-19 17:37:26.254722 pxgpt-0.0.0rc0/pxgpt/cli.py
--rw-r--r--   0        0        0     4437 2023-07-19 17:37:26.254722 pxgpt-0.0.0rc0/pxgpt/config.py
--rw-r--r--   0        0        0      651 2023-07-19 17:37:26.254722 pxgpt-0.0.0rc0/pxgpt/docs.py
--rw-r--r--   0        0        0    28133 2023-07-19 17:37:26.254722 pxgpt-0.0.0rc0/pxgpt/frontend/build/assets/favicon.png
--rw-r--r--   0        0        0   614810 2023-07-19 17:37:26.258723 pxgpt-0.0.0rc0/pxgpt/frontend/build/assets/index.css
--rw-r--r--   0        0        0   221931 2023-07-19 17:37:26.258723 pxgpt-0.0.0rc0/pxgpt/frontend/build/assets/index.js
--rw-r--r--   0        0        0      427 2023-07-19 17:37:26.258723 pxgpt-0.0.0rc0/pxgpt/frontend/build/index.html
--rw-r--r--   0        0        0      416 2023-07-19 17:37:26.262723 pxgpt-0.0.0rc0/pxgpt/ingest.py
--rw-r--r--   0        0        0      575 2023-07-19 17:37:26.262723 pxgpt-0.0.0rc0/pxgpt/logger.py
--rw-r--r--   0        0        0     8917 2023-07-19 17:37:26.262723 pxgpt-0.0.0rc0/pxgpt/manager.py
--rw-r--r--   0        0        0       55 2023-07-19 17:37:26.262723 pxgpt-0.0.0rc0/pxgpt/rings/__init__.py
--rw-r--r--   0        0        0     6971 2023-07-19 17:37:26.262723 pxgpt-0.0.0rc0/pxgpt/rings/_callbacks.py
--rw-r--r--   0        0        0      755 2023-07-19 17:37:26.262723 pxgpt-0.0.0rc0/pxgpt/rings/_llms.py
--rw-r--r--   0        0        0    13328 2023-07-19 17:37:26.262723 pxgpt-0.0.0rc0/pxgpt/rings/_mixins.py
--rw-r--r--   0        0        0    17176 2023-07-19 17:37:26.262723 pxgpt-0.0.0rc0/pxgpt/rings/base.py
--rw-r--r--   0        0        0      202 2023-07-19 17:37:26.262723 pxgpt-0.0.0rc0/pxgpt/rings/chatopenai.py
--rw-r--r--   0        0        0      482 2023-07-19 17:37:26.262723 pxgpt-0.0.0rc0/pxgpt/rings/gpt4all.py
--rw-r--r--   0        0        0      728 2023-07-19 17:37:26.262723 pxgpt-0.0.0rc0/pxgpt/rings/llamacpp.py
--rw-r--r--   0        0        0     2040 2023-07-19 17:37:26.262723 pxgpt-0.0.0rc0/pxgpt/rings/openai.py
--rw-r--r--   0        0        0     3163 2023-07-19 17:37:26.262723 pxgpt-0.0.0rc0/pxgpt/serve.py
--rw-r--r--   0        0        0       25 2023-07-19 17:37:26.262723 pxgpt-0.0.0rc0/pxgpt/version.py
--rw-r--r--   0        0        0    11669 2023-07-19 17:37:26.262723 pxgpt-0.0.0rc0/pxgpt/ws.py
--rw-r--r--   0        0        0     2506 2023-07-19 17:37:26.262723 pxgpt-0.0.0rc0/pxgpt/zzz.py
--rw-r--r--   0        0        0     1140 2023-07-19 17:37:26.262723 pxgpt-0.0.0rc0/pyproject.toml
--rw-r--r--   0        0        0     8346 1970-01-01 00:00:00.000000 pxgpt-0.0.0rc0/setup.py
--rw-r--r--   0        0        0     8011 1970-01-01 00:00:00.000000 pxgpt-0.0.0rc0/PKG-INFO
+-rw-r--r--   0        0        0      546 2023-07-21 01:51:29.637142 pxgpt-0.0.0rc1/LICENSE
+-rw-r--r--   0        0        0     8573 2023-07-21 01:51:29.637142 pxgpt-0.0.0rc1/README.md
+-rw-r--r--   0        0        0       86 2023-07-21 01:51:29.641142 pxgpt-0.0.0rc1/pxgpt/__init__.py
+-rw-r--r--   0        0        0       61 2023-07-21 01:51:29.641142 pxgpt-0.0.0rc1/pxgpt/__main__.py
+-rw-r--r--   0        0        0    14770 2023-07-21 01:51:29.641142 pxgpt-0.0.0rc1/pxgpt/chat.py
+-rw-r--r--   0        0        0     3134 2023-07-21 01:51:29.641142 pxgpt-0.0.0rc1/pxgpt/cli.py
+-rw-r--r--   0        0        0     4444 2023-07-21 01:51:29.641142 pxgpt-0.0.0rc1/pxgpt/config.py
+-rw-r--r--   0        0        0      651 2023-07-21 01:51:29.641142 pxgpt-0.0.0rc1/pxgpt/docs.py
+-rw-r--r--   0        0        0    29785 2023-07-21 01:51:29.641142 pxgpt-0.0.0rc1/pxgpt/frontend/build/assets/favicon.png
+-rw-r--r--   0        0        0   614810 2023-07-21 01:51:29.645143 pxgpt-0.0.0rc1/pxgpt/frontend/build/assets/index.css
+-rw-r--r--   0        0        0   221977 2023-07-21 01:51:29.645143 pxgpt-0.0.0rc1/pxgpt/frontend/build/assets/index.js
+-rw-r--r--   0        0        0      431 2023-07-21 01:51:29.645143 pxgpt-0.0.0rc1/pxgpt/frontend/build/index.html
+-rw-r--r--   0        0        0      416 2023-07-21 01:51:29.649143 pxgpt-0.0.0rc1/pxgpt/ingest.py
+-rw-r--r--   0        0        0      575 2023-07-21 01:51:29.649143 pxgpt-0.0.0rc1/pxgpt/logger.py
+-rw-r--r--   0        0        0     9146 2023-07-21 01:51:29.649143 pxgpt-0.0.0rc1/pxgpt/manager.py
+-rw-r--r--   0        0        0       55 2023-07-21 01:51:29.649143 pxgpt-0.0.0rc1/pxgpt/rings/__init__.py
+-rw-r--r--   0        0        0     6971 2023-07-21 01:51:29.649143 pxgpt-0.0.0rc1/pxgpt/rings/_callbacks.py
+-rw-r--r--   0        0        0      755 2023-07-21 01:51:29.649143 pxgpt-0.0.0rc1/pxgpt/rings/_llms.py
+-rw-r--r--   0        0        0    13337 2023-07-21 01:51:29.649143 pxgpt-0.0.0rc1/pxgpt/rings/_mixins.py
+-rw-r--r--   0        0        0    17814 2023-07-21 01:51:29.649143 pxgpt-0.0.0rc1/pxgpt/rings/base.py
+-rw-r--r--   0        0        0      202 2023-07-21 01:51:29.649143 pxgpt-0.0.0rc1/pxgpt/rings/chatopenai.py
+-rw-r--r--   0        0        0     1015 2023-07-21 01:51:29.649143 pxgpt-0.0.0rc1/pxgpt/rings/gpt4all.py
+-rw-r--r--   0        0        0     1572 2023-07-21 01:51:29.649143 pxgpt-0.0.0rc1/pxgpt/rings/llamacpp.py
+-rw-r--r--   0        0        0     2225 2023-07-21 01:51:29.649143 pxgpt-0.0.0rc1/pxgpt/rings/openai.py
+-rw-r--r--   0        0        0     3163 2023-07-21 01:51:29.649143 pxgpt-0.0.0rc1/pxgpt/serve.py
+-rw-r--r--   0        0        0       25 2023-07-21 01:51:29.649143 pxgpt-0.0.0rc1/pxgpt/version.py
+-rw-r--r--   0        0        0    11669 2023-07-21 01:51:29.649143 pxgpt-0.0.0rc1/pxgpt/ws.py
+-rw-r--r--   0        0        0     2506 2023-07-21 01:51:29.649143 pxgpt-0.0.0rc1/pxgpt/zzz.py
+-rw-r--r--   0        0        0     1125 2023-07-21 01:51:29.649143 pxgpt-0.0.0rc1/pyproject.toml
+-rw-r--r--   0        0        0    10198 1970-01-01 00:00:00.000000 pxgpt-0.0.0rc1/setup.py
+-rw-r--r--   0        0        0     9950 1970-01-01 00:00:00.000000 pxgpt-0.0.0rc1/PKG-INFO
```

### Comparing `pxgpt-0.0.0rc0/LICENSE` & `pxgpt-0.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `pxgpt-0.0.0rc0/README.md` & `pxgpt-0.0.0rc1/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,17 +1,25 @@
-# <img src="pxgpt/frontend/public/assets/favicon.png" alt="p" width=28 />GPT: Your personal, powerful and private GPT
+<div style="display: flex; align-items: center; justify-content: center; gap: .2rem">
+  <img src="pxgpt/frontend/public/assets/favicon.png" alt="px" style="width: 32px; height: 32px;" />
+  <div style="font-size: 24px; font-weight: bold">GPT</div>
+</div>
+<hr />
+<p style="text-align: center">Your personal, powerful and private GPT</p>
+
+
 
 ## Features
 
 - Ingest of your own documents and talk to them.
 - Store your data locally on your device.
 - Choose from a variety of models, including OpenAI.
 - Support conversation history and memory.
 - Switch between profiles with different settings.
 - Support both web interface and command line interface.
+- Support Llama v2!
 
 ## Installation
 
 ```shell
 # With all supported models
 $ pip install -U pxgpt[all]
 
@@ -21,44 +29,53 @@
 # With support for llama-cpp only
 $ pip install -U pxgpt[llama-cpp]
 
 # With support for openai only
 $ pip install -U pxgpt[openai]
 ```
 
+Then copy the configuration from `.pxgpt.config-example.yml` to `.pxgpt.config.yml` and modify it to your needs.
+
 ## Usage
 
 ### Chat from CLI
 
 ```shell
 $ 23:45:06 ❯ pxgpt chat
 
-Welcome to chat via the pxgpt CLI v0.0.0!
+Welcome to chat via the pxGPT CLI v0.0.0rc0!
 Hit 'Ctrl+c' or 'Ctrl+d' to exit.
-[2023-07-18 23:45:09,969] INFO Creating LLM (GPT4All)
-Found model file at  models/gpt4all/ggml-gpt4all-j-v1.3-groovy.bin
-gptj_model_load: loading model from 'models/gpt4all/ggml-gpt4all-j-v1.3-groovy.bin' - please wait ...
-gptj_model_load: n_vocab = 50400
-gptj_model_load: n_ctx   = 2048
-gptj_model_load: n_embd  = 4096
-gptj_model_load: n_head  = 16
-gptj_model_load: n_layer = 28
-gptj_model_load: n_rot   = 64
-gptj_model_load: f16     = 2
-gptj_model_load: ggml ctx size = 5401.45 MB
-gptj_model_load: kv self size  =  896.00 MB
-gptj_model_load: ................................... done
-gptj_model_load: model size =  3609.38 MB / num tensors = 285
-[2023-07-18 23:45:11,741] INFO Entering chat mode
-Loaded conversation:  2023-07-16_23-11-27
+[2023-07-20 20:03:22,716] INFO Switched profile to llamacpp-chat
+[2023-07-20 20:03:22,719] INFO Creating LLM (LlamaCpp)
+llama.cpp: loading model from models/llamacpp/llama-2-7b.ggmlv3.q4_0.bin
+llama_model_load_internal: format     = ggjt v3 (latest)
+llama_model_load_internal: n_vocab    = 32000
+llama_model_load_internal: n_ctx      = 512
+llama_model_load_internal: n_embd     = 4096
+llama_model_load_internal: n_mult     = 256
+llama_model_load_internal: n_head     = 32
+llama_model_load_internal: n_layer    = 32
+llama_model_load_internal: n_rot      = 128
+llama_model_load_internal: freq_base  = 10000.0
+llama_model_load_internal: freq_scale = 1
+llama_model_load_internal: ftype      = 2 (mostly Q4_0)
+llama_model_load_internal: n_ff       = 11008
+llama_model_load_internal: model size = 7B
+llama_model_load_internal: ggml ctx size =    0.08 MB
+llama_model_load_internal: mem required  = 5185.72 MB (+ 1026.00 MB per state)
+llama_new_context_with_model: kv self size  =  256.00 MB
+[2023-07-20 20:03:24,552] INFO Entering chat mode
+Loaded conversation:  2023-07-20_20-03-17
 Use the up/down arrow keys to navigate history.
 Use /help to see the list of commands.
 
->>> Hello?
-  Hi there! How may I help you today?
+>>> Hello Llama 2, if you could choose a superpower, what would it be and why?
+ I will answer this question in two parts. The first part is the super power that I will choose. The second part is why I chose this super power.
+In the first part, the super power that I will choose is the ability to fly. This is because flying has many benefits. It allows me to travel quickly and easily, without having to deal with traffic or waiting at airports. Additionally, it saves time since I don't have to wait for a bus or train ride. Finally, flying gives me an opportunity to see new places and explore new cultures.
+In the second part of my answer, I will explain why I chose this super power. The reason is because flying allows me to travel quickly and easily, without having to deal with traffic or waiting at airports. Additionally, it saves time since I don't have to wait for a bus or train ride. Finally, flying gives me an opportunity to see new places and explore new cultures.
 
 >>> /help
 Commands:
   - /help: List the commands
   - /new: Start a new conversation
   - /switch: Switch to a conversation
   - /list: List all conversations
@@ -78,15 +95,15 @@
 $ pxgpt serve
 # Open http://localhost:7758 in your browser
 ```
 
 ![Web-interface](web-interface.png)
 
 ### Configuration
-
+px
 The configuration files are loaded from the following paths:
 
 - `~/.config/pxgpt/config.yml`
 - `~/.pxgpt.config.yml`
 - `./.pxgpt.config.yml`
 
 #### Profiles
@@ -168,22 +185,23 @@
 
 `pxgpt` is Inspired by [privateGPT][8], with the addition of openai API support, history and memory support, and a web interface.
 
 ## TODO
 
 - [ ] Support ingestion management (upload/download/delete/ingest documents) from the web interface
 - [ ] Support profile management (add/remove/modify) from the web interface
+- [ ] Use markdown to format the response on the web interface
 - [ ] Build a docker image
 - [ ] Support more models
 
 ## Q & A
 
 [QA.md](QA.md)
 
 [1]: https://api.python.langchain.com/en/latest/llms/langchain.llms.gpt4all.GPT4All.html#langchain.llms.gpt4all.GPT4All
 [2]: https://api.python.langchain.com/en/latest/llms/langchain.llms.llamacpp.LlamaCpp.html#langchain.llms.llamacpp.LlamaCpp
 [3]: https://api.python.langchain.com/en/latest/chat_models/langchain.chat_models.openai.ChatOpenAI.html#langchain.chat_models.openai.ChatOpenAI
 [4]: https://api.python.langchain.com/en/latest/llms/langchain.llms.openai.OpenAI.html#langchain.llms.openai.OpenAI
-[5]: https://api.python.langchain.com/en/latest/embeddings/langchain.embeddings.huggingface.HuggingFaceEmbeddings.html#langchain.embeddings.huggingface.HuggingFaceEmbeddings
+[5]: https://api.python.langchain.com/en/latest/embeddings/langchain.embeddings.gpt4all.GPT4AllEmbeddings.html#langchain.embeddings.gpt4all.GPT4AllEmbeddings
 [6]: https://api.python.langchain.com/en/latest/embeddings/langchain.embeddings.llamacpp.LlamaCppEmbeddings.html#langchain.embeddings.llamacpp.LlamaCppEmbeddings
 [7]: https://api.python.langchain.com/en/latest/embeddings/langchain.embeddings.openai.OpenAIEmbeddings.html#langchain.embeddings.openai.OpenAIEmbeddings
 [8]: https://github.com/imartinez/privateGPT
```

### Comparing `pxgpt-0.0.0rc0/pxgpt/chat.py` & `pxgpt-0.0.0rc1/pxgpt/chat.py`

 * *Files 0% similar despite different names*

```diff
@@ -450,21 +450,21 @@
 
     if asyn:
         asyncio.run(_a_chat(manager, session, history_name, history_list))
     else:
         _chat(manager, session, history_name, history_list)
 
 
-def chat_cli(profile: str, asyn: bool) -> None:
+def chat_cli(profile: str, asyn: bool, debug: bool) -> None:
     """Chat with the model in the terminal"""
     print()
     print(f"Welcome to chat via the pxGPT CLI v{__version__}!")
     print("Hit 'Ctrl+c' or 'Ctrl+d' to exit.")
 
-    manager = Manager(profile)
+    manager = Manager(profile, debug=debug)
     history = None
     history_list = manager.get_histories()
 
     if not history_list:
         history_list = [manager.new_history()]
         msg = "Created a new conversation: "
     else:
```

### Comparing `pxgpt-0.0.0rc0/pxgpt/cli.py` & `pxgpt-0.0.0rc1/pxgpt/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,14 +38,23 @@
         action="store_true",
         help=(
             "Use async calls to the model? "
             "Don't use it if you don't know what it is."
         ),
         default=False,
     )
+    parser_chat.add_argument(
+        "--debug",
+        action="store_true",
+        default=False,
+        help=(
+            "Debug mode. Set the verbose to True for the chains "
+            "to print the final prompts."
+        ),
+    )
     parser_chat.add_argument(*profile_names, **profile_args)
     # docs
     parser_docs = parser.add_command(
         "docs", help="Show ingested and pending documents under a profile"
     )
     parser_docs.add_argument(*profile_names, **profile_args)
     # serve
@@ -77,15 +86,15 @@
 
     if args.COMMAND == 'ingest':
         from .ingest import ingest_cli
         ingest_cli(args.profile, args.force)
 
     elif args.COMMAND == 'chat':
         from .chat import chat_cli
-        chat_cli(args.profile, args.asyn)
+        chat_cli(args.profile, args.asyn, args.debug)
 
     elif args.COMMAND == 'serve':
         from .serve import serve
         serve(args.port)
 
     elif args.COMMAND == 'profiles':
         from .config import config
```

### Comparing `pxgpt-0.0.0rc0/pxgpt/config.py` & `pxgpt-0.0.0rc1/pxgpt/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,16 +8,16 @@
     history_directory="~/.config/pxgpt/history",
     history_into_memory=True,
     credentials=Diot(
         openai_api_key=None,
     ),
     embeddings=Diot(),
     model=Diot(
-        type="GPT4All",
-        model="models/gpt4all/ggml-gpt4all-j-v1.3-groovy.bin",
+        # type="LlamaCpp",
+        # model_path="models/llamacpp/llama-2-7b.ggmlv3.q4_0.bin",
     ),
     ingest=Diot(
         chunk_size=500,
         chunk_overlap=50,
         source_directory=None,
         n_workers=0,
         persist_directory=None,
```

### Comparing `pxgpt-0.0.0rc0/pxgpt/docs.py` & `pxgpt-0.0.0rc1/pxgpt/docs.py`

 * *Files identical despite different names*

### Comparing `pxgpt-0.0.0rc0/pxgpt/frontend/build/assets/index.css` & `pxgpt-0.0.0rc1/pxgpt/frontend/build/assets/index.css`

 * *Files identical despite different names*

### Comparing `pxgpt-0.0.0rc0/pxgpt/frontend/build/assets/index.js` & `pxgpt-0.0.0rc1/pxgpt/frontend/build/assets/index.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -205,15 +205,15 @@
         return b(p)
     }, o.allocUnsafeSlow = function(p) {
         return b(p)
     };
 
     function d(p, c) {
         if ((typeof c != "string" || c === "") && (c = "utf8"), !o.isEncoding(c)) throw new TypeError("Unknown encoding: " + c);
-        var m = D(p, c) | 0,
+        var m = P(p, c) | 0,
             y = r(m),
             H = y.write(p, c);
         return H !== m && (y = y.slice(0, H)), y
     }
 
     function g(p) {
         for (var c = p.length < 0 ? 0 : B(p.length) | 0, m = r(c), y = 0; y < c; y += 1) m[y] = p[y] & 255;
@@ -294,15 +294,15 @@
             else if (o.isBuffer(S)) S.copy(H, Q);
             else throw new TypeError('"list" argument must be an Array of Buffers');
             Q += S.length
         }
         return H
     };
 
-    function D(p, c) {
+    function P(p, c) {
         if (o.isBuffer(p)) return p.length;
         if (ArrayBuffer.isView(p) || Ze(p, ArrayBuffer)) return p.byteLength;
         if (typeof p != "string") throw new TypeError('The "string" argument must be one of type string, Buffer, or ArrayBuffer. Received type ' + typeof p);
         var m = p.length,
             y = arguments.length > 2 && arguments[2] === !0;
         if (!y && m === 0) return 0;
         for (var H = !1;;) switch (c) {
@@ -323,15 +323,15 @@
             case "base64":
                 return ue(p).length;
             default:
                 if (H) return y ? -1 : Ye(p).length;
                 c = ("" + c).toLowerCase(), H = !0
         }
     }
-    o.byteLength = D;
+    o.byteLength = P;
 
     function O(p, c, m) {
         var y = !1;
         if ((c === void 0 || c < 0) && (c = 0), c > this.length || ((m === void 0 || m > this.length) && (m = this.length), m <= 0) || (m >>>= 0, c >>>= 0, m <= c)) return "";
         for (p || (p = "utf8");;) switch (p) {
             case "hex":
                 return Ce(this, c, m);
@@ -636,77 +636,77 @@
         return c = c >>> 0, m || Te(c, 4, this.length), t.read(this, c, !1, 23, 4)
     }, o.prototype.readDoubleLE = function(c, m) {
         return c = c >>> 0, m || Te(c, 8, this.length), t.read(this, c, !0, 52, 8)
     }, o.prototype.readDoubleBE = function(c, m) {
         return c = c >>> 0, m || Te(c, 8, this.length), t.read(this, c, !1, 52, 8)
     };
 
-    function P(p, c, m, y, H, Q) {
+    function D(p, c, m, y, H, Q) {
         if (!o.isBuffer(p)) throw new TypeError('"buffer" argument must be a Buffer instance');
         if (c > H || c < Q) throw new RangeError('"value" argument is out of bounds');
         if (m + y > p.length) throw new RangeError("Index out of range")
     }
     o.prototype.writeUintLE = o.prototype.writeUIntLE = function(c, m, y, H) {
         if (c = +c, m = m >>> 0, y = y >>> 0, !H) {
             var Q = Math.pow(2, 8 * y) - 1;
-            P(this, c, m, y, Q, 0)
+            D(this, c, m, y, Q, 0)
         }
         var S = 1,
             Ae = 0;
         for (this[m] = c & 255; ++Ae < y && (S *= 256);) this[m + Ae] = c / S & 255;
         return m + y
     }, o.prototype.writeUintBE = o.prototype.writeUIntBE = function(c, m, y, H) {
         if (c = +c, m = m >>> 0, y = y >>> 0, !H) {
             var Q = Math.pow(2, 8 * y) - 1;
-            P(this, c, m, y, Q, 0)
+            D(this, c, m, y, Q, 0)
         }
         var S = y - 1,
             Ae = 1;
         for (this[m + S] = c & 255; --S >= 0 && (Ae *= 256);) this[m + S] = c / Ae & 255;
         return m + y
     }, o.prototype.writeUint8 = o.prototype.writeUInt8 = function(c, m, y) {
-        return c = +c, m = m >>> 0, y || P(this, c, m, 1, 255, 0), this[m] = c & 255, m + 1
+        return c = +c, m = m >>> 0, y || D(this, c, m, 1, 255, 0), this[m] = c & 255, m + 1
     }, o.prototype.writeUint16LE = o.prototype.writeUInt16LE = function(c, m, y) {
-        return c = +c, m = m >>> 0, y || P(this, c, m, 2, 65535, 0), this[m] = c & 255, this[m + 1] = c >>> 8, m + 2
+        return c = +c, m = m >>> 0, y || D(this, c, m, 2, 65535, 0), this[m] = c & 255, this[m + 1] = c >>> 8, m + 2
     }, o.prototype.writeUint16BE = o.prototype.writeUInt16BE = function(c, m, y) {
-        return c = +c, m = m >>> 0, y || P(this, c, m, 2, 65535, 0), this[m] = c >>> 8, this[m + 1] = c & 255, m + 2
+        return c = +c, m = m >>> 0, y || D(this, c, m, 2, 65535, 0), this[m] = c >>> 8, this[m + 1] = c & 255, m + 2
     }, o.prototype.writeUint32LE = o.prototype.writeUInt32LE = function(c, m, y) {
-        return c = +c, m = m >>> 0, y || P(this, c, m, 4, 4294967295, 0), this[m + 3] = c >>> 24, this[m + 2] = c >>> 16, this[m + 1] = c >>> 8, this[m] = c & 255, m + 4
+        return c = +c, m = m >>> 0, y || D(this, c, m, 4, 4294967295, 0), this[m + 3] = c >>> 24, this[m + 2] = c >>> 16, this[m + 1] = c >>> 8, this[m] = c & 255, m + 4
     }, o.prototype.writeUint32BE = o.prototype.writeUInt32BE = function(c, m, y) {
-        return c = +c, m = m >>> 0, y || P(this, c, m, 4, 4294967295, 0), this[m] = c >>> 24, this[m + 1] = c >>> 16, this[m + 2] = c >>> 8, this[m + 3] = c & 255, m + 4
+        return c = +c, m = m >>> 0, y || D(this, c, m, 4, 4294967295, 0), this[m] = c >>> 24, this[m + 1] = c >>> 16, this[m + 2] = c >>> 8, this[m + 3] = c & 255, m + 4
     }, o.prototype.writeIntLE = function(c, m, y, H) {
         if (c = +c, m = m >>> 0, !H) {
             var Q = Math.pow(2, 8 * y - 1);
-            P(this, c, m, y, Q - 1, -Q)
+            D(this, c, m, y, Q - 1, -Q)
         }
         var S = 0,
             Ae = 1,
             Be = 0;
         for (this[m] = c & 255; ++S < y && (Ae *= 256);) c < 0 && Be === 0 && this[m + S - 1] !== 0 && (Be = 1), this[m + S] = (c / Ae >> 0) - Be & 255;
         return m + y
     }, o.prototype.writeIntBE = function(c, m, y, H) {
         if (c = +c, m = m >>> 0, !H) {
             var Q = Math.pow(2, 8 * y - 1);
-            P(this, c, m, y, Q - 1, -Q)
+            D(this, c, m, y, Q - 1, -Q)
         }
         var S = y - 1,
             Ae = 1,
             Be = 0;
         for (this[m + S] = c & 255; --S >= 0 && (Ae *= 256);) c < 0 && Be === 0 && this[m + S + 1] !== 0 && (Be = 1), this[m + S] = (c / Ae >> 0) - Be & 255;
         return m + y
     }, o.prototype.writeInt8 = function(c, m, y) {
-        return c = +c, m = m >>> 0, y || P(this, c, m, 1, 127, -128), c < 0 && (c = 255 + c + 1), this[m] = c & 255, m + 1
+        return c = +c, m = m >>> 0, y || D(this, c, m, 1, 127, -128), c < 0 && (c = 255 + c + 1), this[m] = c & 255, m + 1
     }, o.prototype.writeInt16LE = function(c, m, y) {
-        return c = +c, m = m >>> 0, y || P(this, c, m, 2, 32767, -32768), this[m] = c & 255, this[m + 1] = c >>> 8, m + 2
+        return c = +c, m = m >>> 0, y || D(this, c, m, 2, 32767, -32768), this[m] = c & 255, this[m + 1] = c >>> 8, m + 2
     }, o.prototype.writeInt16BE = function(c, m, y) {
-        return c = +c, m = m >>> 0, y || P(this, c, m, 2, 32767, -32768), this[m] = c >>> 8, this[m + 1] = c & 255, m + 2
+        return c = +c, m = m >>> 0, y || D(this, c, m, 2, 32767, -32768), this[m] = c >>> 8, this[m + 1] = c & 255, m + 2
     }, o.prototype.writeInt32LE = function(c, m, y) {
-        return c = +c, m = m >>> 0, y || P(this, c, m, 4, 2147483647, -2147483648), this[m] = c & 255, this[m + 1] = c >>> 8, this[m + 2] = c >>> 16, this[m + 3] = c >>> 24, m + 4
+        return c = +c, m = m >>> 0, y || D(this, c, m, 4, 2147483647, -2147483648), this[m] = c & 255, this[m + 1] = c >>> 8, this[m + 2] = c >>> 16, this[m + 3] = c >>> 24, m + 4
     }, o.prototype.writeInt32BE = function(c, m, y) {
-        return c = +c, m = m >>> 0, y || P(this, c, m, 4, 2147483647, -2147483648), c < 0 && (c = 4294967295 + c + 1), this[m] = c >>> 24, this[m + 1] = c >>> 16, this[m + 2] = c >>> 8, this[m + 3] = c & 255, m + 4
+        return c = +c, m = m >>> 0, y || D(this, c, m, 4, 2147483647, -2147483648), c < 0 && (c = 4294967295 + c + 1), this[m] = c >>> 24, this[m + 1] = c >>> 16, this[m + 2] = c >>> 8, this[m + 3] = c & 255, m + 4
     };
 
     function we(p, c, m, y, H, Q) {
         if (m + y > p.length) throw new RangeError("Index out of range");
         if (m < 0) throw new RangeError("Index out of range")
     }
 
@@ -1335,20 +1335,20 @@
         g = f.length,
         _ = d;
     const k = {};
     for (; _--;) k[i[_].key] = _;
     const w = [],
         B = new Map,
         T = new Map,
-        D = [];
+        P = [];
     for (_ = g; _--;) {
         const q = b(l, f, _),
             L = t(q);
         let C = r.get(L);
-        C ? n && D.push(() => C.p(q, e)) : (C = u(L, q), C.c()), B.set(L, w[_] = C), L in k && T.set(L, Math.abs(_ - k[L]))
+        C ? n && P.push(() => C.p(q, e)) : (C = u(L, q), C.c()), B.set(L, w[_] = C), L in k && T.set(L, Math.abs(_ - k[L]))
     }
     const O = new Set,
         R = new Set;
 
     function U(q) {
         v(q, 1), q.m(o, a), r.set(q.key, q), a = q.first, g--
     }
@@ -1360,15 +1360,15 @@
         q === L ? (a = q.first, d--, g--) : B.has(ne) ? !r.has(C) || O.has(C) ? U(q) : R.has(ne) ? d-- : T.get(C) > T.get(ne) ? (R.add(C), U(q)) : (O.add(ne), d--) : (s(L, r), d--)
     }
     for (; d--;) {
         const q = i[d];
         B.has(q.key) || s(q, r)
     }
     for (; g;) U(w[g - 1]);
-    return Le(D), w
+    return Le(P), w
 }
 
 function pe(i, e) {
     const t = {},
         n = {},
         l = {
             $$scope: 1
@@ -2130,15 +2130,15 @@
     } = e, {
         tooltipAlignment: w = "center"
     } = e, {
         tooltipPosition: B = "bottom"
     } = e, {
         as: T = !1
     } = e, {
-        skeleton: D = !1
+        skeleton: P = !1
     } = e, {
         disabled: O = !1
     } = e, {
         href: R = void 0
     } = e, {
         tabindex: U = "0"
     } = e, {
@@ -2192,38 +2192,38 @@
         J.call(this, i, fe)
     }
 
     function Te(fe) {
         J.call(this, i, fe)
     }
 
-    function P(fe) {
+    function D(fe) {
         ze[fe ? "unshift" : "push"](() => {
             L = fe, t(0, L)
         })
     }
 
     function we(fe) {
         ze[fe ? "unshift" : "push"](() => {
             L = fe, t(0, L)
         })
     }
     return i.$$set = fe => {
-        e = Z(Z({}, e), ce(fe)), t(10, r = ie(e, f)), "kind" in fe && t(11, a = fe.kind), "size" in fe && t(1, b = fe.size), "expressive" in fe && t(12, d = fe.expressive), "isSelected" in fe && t(13, g = fe.isSelected), "icon" in fe && t(2, _ = fe.icon), "iconDescription" in fe && t(3, k = fe.iconDescription), "tooltipAlignment" in fe && t(14, w = fe.tooltipAlignment), "tooltipPosition" in fe && t(15, B = fe.tooltipPosition), "as" in fe && t(4, T = fe.as), "skeleton" in fe && t(5, D = fe.skeleton), "disabled" in fe && t(6, O = fe.disabled), "href" in fe && t(7, R = fe.href), "tabindex" in fe && t(16, U = fe.tabindex), "type" in fe && t(17, q = fe.type), "ref" in fe && t(0, L = fe.ref), "$$scope" in fe && t(18, s = fe.$$scope)
+        e = Z(Z({}, e), ce(fe)), t(10, r = ie(e, f)), "kind" in fe && t(11, a = fe.kind), "size" in fe && t(1, b = fe.size), "expressive" in fe && t(12, d = fe.expressive), "isSelected" in fe && t(13, g = fe.isSelected), "icon" in fe && t(2, _ = fe.icon), "iconDescription" in fe && t(3, k = fe.iconDescription), "tooltipAlignment" in fe && t(14, w = fe.tooltipAlignment), "tooltipPosition" in fe && t(15, B = fe.tooltipPosition), "as" in fe && t(4, T = fe.as), "skeleton" in fe && t(5, P = fe.skeleton), "disabled" in fe && t(6, O = fe.disabled), "href" in fe && t(7, R = fe.href), "tabindex" in fe && t(16, U = fe.tabindex), "type" in fe && t(17, q = fe.type), "ref" in fe && t(0, L = fe.ref), "$$scope" in fe && t(18, s = fe.$$scope)
     }, i.$$.update = () => {
         i.$$.dirty[0] & 1 && C && L && C.declareRef(L), i.$$.dirty[0] & 4 && t(8, n = _ && !u.default), t(9, l = {
             type: R && !O ? void 0 : q,
             tabindex: U,
             disabled: O === !0 ? !0 : void 0,
             href: R,
             "aria-pressed": n && a === "ghost" && !R ? g : void 0,
             ...r,
             class: ["bx--btn", d && "bx--btn--expressive", (b === "small" && !d || b === "sm" && !d || b === "small" && !d) && "bx--btn--sm", b === "field" && !d || b === "md" && !d && "bx--btn--md", b === "field" && "bx--btn--field", b === "small" && "bx--btn--sm", b === "lg" && "bx--btn--lg", b === "xl" && "bx--btn--xl", a && `bx--btn--${a}`, O && "bx--btn--disabled", n && "bx--btn--icon-only", n && "bx--tooltip__trigger", n && "bx--tooltip--a11y", n && B && `bx--btn--icon-only--${B}`, n && w && `bx--tooltip--align-${w}`, n && g && a === "ghost" && "bx--btn--selected", r.class].filter(Boolean).join(" ")
         })
-    }, [L, b, _, k, T, D, O, R, n, l, r, a, d, g, w, B, U, q, s, o, ne, j, N, Y, se, ke, he, F, x, Ce, Ee, Te, P, we]
+    }, [L, b, _, k, T, P, O, R, n, l, r, a, d, g, w, B, U, q, s, o, ne, j, N, Y, se, ke, he, F, x, Ce, Ee, Te, D, we]
 }
 class yr extends ge {
     constructor(e) {
         super(), be(this, e, Tr, wr, _e, {
             kind: 11,
             size: 1,
             expressive: 12,
@@ -2665,15 +2665,15 @@
         d(t) {
             t && E(e)
         }
     }
 }
 
 function Pr(i) {
-    let e, t, n, l, f, r, o, s, u, a, b, d, g, _, k, w, B, T, D, O, R = i[5] && si(i),
+    let e, t, n, l, f, r, o, s, u, a, b, d, g, _, k, w, B, T, P, O, R = i[5] && si(i),
         U = i[7] && ui(i);
     const q = i[31].heading,
         L = Fe(q, i, i[50], oi),
         C = L || Cr(i);
     let ne = !i[5] && ai(i);
     const j = i[31].default,
         N = Fe(j, i, i[50], null);
@@ -2687,15 +2687,15 @@
         he = {};
     for (let F = 0; F < ke.length; F += 1) he = Z(he, ke[F]);
     return {
         c() {
             e = V("div"), t = V("div"), n = V("div"), R && R.c(), l = $(), U && U.c(), f = $(), r = V("h3"), C && C.c(), o = $(), ne && ne.c(), s = $(), u = V("div"), N && N.c(), _ = $(), Y && Y.c(), k = $(), se && se.c(), z(r, "id", i[24]), h(r, "bx--modal-header__heading", !0), h(n, "bx--modal-header", !0), z(u, "id", i[23]), z(u, "tabindex", a = i[10] ? "0" : void 0), z(u, "role", b = i[10] ? "region" : void 0), z(u, "aria-label", d = i[10] ? i[22] : void 0), z(u, "aria-labelledby", g = i[7] ? i[25] : i[24]), h(u, "bx--modal-content", !0), h(u, "bx--modal-content--with-form", i[9]), h(u, "bx--modal-scroll-content", i[10]), z(t, "tabindex", "-1"), z(t, "role", w = i[4] ? i[5] ? "alert" : "alertdialog" : "dialog"), z(t, "aria-describedby", B = i[4] && !i[5] ? i[23] : void 0), z(t, "aria-modal", "true"), z(t, "aria-label", i[22]), h(t, "bx--modal-container", !0), h(t, "bx--modal-container--xs", i[2] === "xs"), h(t, "bx--modal-container--sm", i[2] === "sm"), h(t, "bx--modal-container--lg", i[2] === "lg"), ve(e, he), h(e, "bx--modal", !0), h(e, "bx--modal-tall", !i[5]), h(e, "is-visible", i[0]), h(e, "bx--modal--danger", i[3])
         },
         m(F, x) {
-            I(F, e, x), M(e, t), M(t, n), R && R.m(n, null), M(n, l), U && U.m(n, null), M(n, f), M(n, r), C && C.m(r, null), M(n, o), ne && ne.m(n, null), M(t, s), M(t, u), N && N.m(u, null), M(t, _), Y && Y.m(t, null), M(t, k), se && se.m(t, null), i[44](t), i[46](e), T = !0, D || (O = [W(t, "click", i[45]), W(e, "keydown", i[32]), W(e, "keydown", i[47]), W(e, "click", i[33]), W(e, "click", i[48]), W(e, "mouseover", i[34]), W(e, "mouseenter", i[35]), W(e, "mouseleave", i[36]), W(e, "transitionend", i[49])], D = !0)
+            I(F, e, x), M(e, t), M(t, n), R && R.m(n, null), M(n, l), U && U.m(n, null), M(n, f), M(n, r), C && C.m(r, null), M(n, o), ne && ne.m(n, null), M(t, s), M(t, u), N && N.m(u, null), M(t, _), Y && Y.m(t, null), M(t, k), se && se.m(t, null), i[44](t), i[46](e), T = !0, P || (O = [W(t, "click", i[45]), W(e, "keydown", i[32]), W(e, "keydown", i[47]), W(e, "click", i[33]), W(e, "click", i[48]), W(e, "mouseover", i[34]), W(e, "mouseenter", i[35]), W(e, "mouseleave", i[36]), W(e, "transitionend", i[49])], P = !0)
         },
         p(F, x) {
             F[5] ? R ? (R.p(F, x), x[0] & 32 && v(R, 1)) : (R = si(F), R.c(), v(R, 1), R.m(n, l)) : R && (de(), A(R, 1, 1, () => {
                 R = null
             }), me()), F[7] ? U ? (U.p(F, x), x[0] & 128 && v(U, 1)) : (U = ui(F), U.c(), v(U, 1), U.m(n, f)) : U && (de(), A(U, 1, 1, () => {
                 U = null
             }), me()), L ? L.p && (!T || x[1] & 524288) && Pe(L, q, F, F[50], T ? Se(q, F[50], x, Mr) : De(F[50]), oi) : C && C.p && (!T || x[0] & 64) && C.p(F, T ? x : [-1, -1]), (!T || x[0] & 16777216) && z(r, "id", F[24]), F[5] ? ne && (de(), A(ne, 1, 1, () => {
@@ -2711,15 +2711,15 @@
         i(F) {
             T || (v(R), v(U), v(C, F), v(ne), v(N, F), v(se), T = !0)
         },
         o(F) {
             A(R), A(U), A(C, F), A(ne), A(N, F), A(se), T = !1
         },
         d(F) {
-            F && E(e), R && R.d(), U && U.d(), C && C.d(F), ne && ne.d(), N && N.d(F), Y && Y.d(), se && se.d(), i[44](null), i[46](null), D = !1, Le(O)
+            F && E(e), R && R.d(), U && U.d(), C && C.d(F), ne && ne.d(), N && N.d(F), Y && Y.d(), se && se.d(), i[44](null), i[46](null), P = !1, Le(O)
         }
     }
 }
 
 function Dr(i, e, t) {
     let n, l, f, r;
     const o = ["size", "open", "danger", "alert", "passiveModal", "modalHeading", "modalLabel", "modalAriaLabel", "iconDescription", "hasForm", "hasScrollingContent", "primaryButtonText", "primaryButtonDisabled", "primaryButtonIcon", "shouldSubmitOnEnter", "secondaryButtonText", "secondaryButtons", "selectorPrimaryFocus", "preventCloseOnClickOutside", "id", "ref"];
@@ -2746,15 +2746,15 @@
         {
             modalHeading: B = void 0
         } = e,
         {
             modalLabel: T = void 0
         } = e,
         {
-            modalAriaLabel: D = void 0
+            modalAriaLabel: P = void 0
         } = e,
         {
             iconDescription: O = "Close the modal"
         } = e,
         {
             hasForm: R = !1
         } = e,
@@ -2793,20 +2793,20 @@
         } = e;
     const F = je();
     let x = null,
         Ce = null,
         Ee = !1,
         Te = !1;
 
-    function P(S) {
+    function D(S) {
         ((S || Ce).querySelector(Y) || x).focus()
     }
     const we = At(g);
     lt(i, we, S => t(52, u = S)), Ar(we), vl(() => {
-        Ee ? g || (Ee = !1, F("close")) : g && (Ee = !0, P(), F("open"))
+        Ee ? g || (Ee = !1, F("close")) : g && (Ee = !0, D(), F("open"))
     });
 
     function fe(S) {
         J.call(this, i, S)
     }
 
     function Ge(S) {
@@ -2890,18 +2890,18 @@
         },
         Q = S => {
             S.propertyName === "transform" && F("transitionend", {
                 open: g
             })
         };
     return i.$$set = S => {
-        t(54, e = Z(Z({}, e), ce(S))), t(28, s = ie(e, o)), "size" in S && t(2, d = S.size), "open" in S && t(0, g = S.open), "danger" in S && t(3, _ = S.danger), "alert" in S && t(4, k = S.alert), "passiveModal" in S && t(5, w = S.passiveModal), "modalHeading" in S && t(6, B = S.modalHeading), "modalLabel" in S && t(7, T = S.modalLabel), "modalAriaLabel" in S && t(29, D = S.modalAriaLabel), "iconDescription" in S && t(8, O = S.iconDescription), "hasForm" in S && t(9, R = S.hasForm), "hasScrollingContent" in S && t(10, U = S.hasScrollingContent), "primaryButtonText" in S && t(11, q = S.primaryButtonText), "primaryButtonDisabled" in S && t(12, L = S.primaryButtonDisabled), "primaryButtonIcon" in S && t(13, C = S.primaryButtonIcon), "shouldSubmitOnEnter" in S && t(14, ne = S.shouldSubmitOnEnter), "secondaryButtonText" in S && t(15, j = S.secondaryButtonText), "secondaryButtons" in S && t(16, N = S.secondaryButtons), "selectorPrimaryFocus" in S && t(30, Y = S.selectorPrimaryFocus), "preventCloseOnClickOutside" in S && t(17, se = S.preventCloseOnClickOutside), "id" in S && t(18, ke = S.id), "ref" in S && t(1, he = S.ref), "$$scope" in S && t(50, b = S.$$scope)
+        t(54, e = Z(Z({}, e), ce(S))), t(28, s = ie(e, o)), "size" in S && t(2, d = S.size), "open" in S && t(0, g = S.open), "danger" in S && t(3, _ = S.danger), "alert" in S && t(4, k = S.alert), "passiveModal" in S && t(5, w = S.passiveModal), "modalHeading" in S && t(6, B = S.modalHeading), "modalLabel" in S && t(7, T = S.modalLabel), "modalAriaLabel" in S && t(29, P = S.modalAriaLabel), "iconDescription" in S && t(8, O = S.iconDescription), "hasForm" in S && t(9, R = S.hasForm), "hasScrollingContent" in S && t(10, U = S.hasScrollingContent), "primaryButtonText" in S && t(11, q = S.primaryButtonText), "primaryButtonDisabled" in S && t(12, L = S.primaryButtonDisabled), "primaryButtonIcon" in S && t(13, C = S.primaryButtonIcon), "shouldSubmitOnEnter" in S && t(14, ne = S.shouldSubmitOnEnter), "secondaryButtonText" in S && t(15, j = S.secondaryButtonText), "secondaryButtons" in S && t(16, N = S.secondaryButtons), "selectorPrimaryFocus" in S && t(30, Y = S.selectorPrimaryFocus), "preventCloseOnClickOutside" in S && t(17, se = S.preventCloseOnClickOutside), "id" in S && t(18, ke = S.id), "ref" in S && t(1, he = S.ref), "$$scope" in S && t(50, b = S.$$scope)
     }, i.$$.update = () => {
-        i.$$.dirty[0] & 1 && Wl(we, u = g, u), i.$$.dirty[0] & 262144 && t(25, n = `bx--modal-header__label--modal-${ke}`), i.$$.dirty[0] & 262144 && t(24, l = `bx--modal-header__heading--modal-${ke}`), i.$$.dirty[0] & 262144 && t(23, f = `bx--modal-body--${ke}`), t(22, r = T || e["aria-label"] || D || B)
-    }, e = ce(e), [g, he, d, _, k, w, B, T, O, R, U, q, L, C, ne, j, N, se, ke, x, Ce, Te, r, f, l, n, F, we, s, D, Y, a, fe, Ge, le, Me, Ye, ot, ft, ue, re, Ze, kt, Pt, p, c, m, y, H, Q, b]
+        i.$$.dirty[0] & 1 && Wl(we, u = g, u), i.$$.dirty[0] & 262144 && t(25, n = `bx--modal-header__label--modal-${ke}`), i.$$.dirty[0] & 262144 && t(24, l = `bx--modal-header__heading--modal-${ke}`), i.$$.dirty[0] & 262144 && t(23, f = `bx--modal-body--${ke}`), t(22, r = T || e["aria-label"] || P || B)
+    }, e = ce(e), [g, he, d, _, k, w, B, T, O, R, U, q, L, C, ne, j, N, se, ke, x, Ce, Te, r, f, l, n, F, we, s, P, Y, a, fe, Ge, le, Me, Ye, ot, ft, ue, re, Ze, kt, Pt, p, c, m, y, H, Q, b]
 }
 class Nr extends ge {
     constructor(e) {
         super(), be(this, e, Dr, Pr, _e, {
             size: 2,
             open: 0,
             danger: 3,
@@ -3203,15 +3203,15 @@
         J.call(this, i, C)
     }
 
     function T(C) {
         J.call(this, i, C)
     }
 
-    function D(C) {
+    function P(C) {
         J.call(this, i, C)
     }
 
     function O(C) {
         J.call(this, i, C)
     }
 
@@ -3232,15 +3232,15 @@
     function L(C) {
         ze[C ? "unshift" : "push"](() => {
             _ = C, t(0, _)
         })
     }
     return i.$$set = C => {
         e = Z(Z({}, e), ce(C)), t(7, l = ie(e, n)), "size" in C && t(1, s = C.size), "href" in C && t(2, u = C.href), "inline" in C && t(3, a = C.inline), "icon" in C && t(4, b = C.icon), "disabled" in C && t(5, d = C.disabled), "visited" in C && t(6, g = C.visited), "ref" in C && t(0, _ = C.ref), "$$scope" in C && t(9, r = C.$$scope)
-    }, [_, s, u, a, b, d, g, l, o, r, f, k, w, B, T, D, O, R, U, q, L]
+    }, [_, s, u, a, b, d, g, l, o, r, f, k, w, B, T, P, O, R, U, q, L]
 }
 class Wr extends ge {
     constructor(e) {
         super(), be(this, e, Zr, Yr, _e, {
             size: 1,
             href: 2,
             inline: 3,
@@ -3590,15 +3590,15 @@
         J.call(this, i, R)
     }
 
     function T(R) {
         J.call(this, i, R)
     }
 
-    function D(R) {
+    function P(R) {
         J.call(this, i, R)
     }
 
     function O(R) {
         J.call(this, i, R)
     }
     return i.$$set = R => {
@@ -3609,15 +3609,15 @@
                 const U = f ? l - 75 : 0,
                     q = f ? l : 75,
                     L = Math.floor(d[R % 3] * (q - U + 1)) + U + "px";
                 t(3, n = [...n, {
                     width: f ? L : `calc(${b} - ${L})`
                 }])
             }
-    }, t(3, n = []), [u, a, b, n, o, s, f, l, g, _, k, w, B, T, D, O]
+    }, t(3, n = []), [u, a, b, n, o, s, f, l, g, _, k, w, B, T, P, O]
 }
 class no extends ge {
     constructor(e) {
         super(), be(this, e, io, to, _e, {
             lines: 5,
             heading: 0,
             paragraph: 1,
@@ -3955,22 +3955,22 @@
         J.call(this, i, O)
     }
 
     function T(O) {
         J.call(this, i, O)
     }
 
-    function D(O) {
+    function P(O) {
         J.call(this, i, O)
     }
     return i.$$set = O => {
         e = Z(Z({}, e), ce(O)), t(3, l = ie(e, n)), "align" in O && t(0, o = O.align), "size" in O && t(1, s = O.size), "disabled" in O && t(4, u = O.disabled), "skeleton" in O && t(2, a = O.skeleton), "$$scope" in O && t(5, r = O.$$scope)
     }, i.$$.update = () => {
         i.$$.dirty & 16 && b.set(u)
-    }, [o, s, a, l, u, r, f, d, g, _, k, w, B, T, D]
+    }, [o, s, a, l, u, r, f, d, g, _, k, w, B, T, P]
 }
 class mo extends ge {
     constructor(e) {
         super(), be(this, e, co, ao, _e, {
             align: 0,
             size: 1,
             disabled: 4,
@@ -4016,20 +4016,20 @@
     let w = [i[5]],
         B = {};
     for (let T = 0; T < w.length; T += 1) B = Z(B, w[T]);
     return {
         c() {
             e = V("li"), t = V("button"), X(n.$$.fragment), l = $(), f = V("div"), g && g.c(), r = $(), o = V("div"), k && k.c(), h(f, "bx--accordion__title", !0), z(t, "type", "button"), z(t, "title", i[3]), z(t, "aria-expanded", i[0]), t.disabled = i[1], h(t, "bx--accordion__heading", !0), h(o, "bx--accordion__content", !0), ve(e, B), h(e, "bx--accordion__item", !0), h(e, "bx--accordion__item--active", i[0]), h(e, "bx--accordion__item--disabled", i[1]), h(e, "bx--accordion__item--expanding", i[4] === "expanding"), h(e, "bx--accordion__item--collapsing", i[4] === "collapsing")
         },
-        m(T, D) {
-            I(T, e, D), M(e, t), G(n, t, null), M(t, l), M(t, f), g && g.m(f, null), M(e, r), M(e, o), k && k.m(o, null), s = !0, u || (a = [W(t, "click", i[9]), W(t, "click", i[14]), W(t, "mouseover", i[10]), W(t, "mouseenter", i[11]), W(t, "mouseleave", i[12]), W(t, "keydown", i[13]), W(t, "keydown", i[15]), W(e, "animationend", i[8]), W(e, "animationend", i[16])], u = !0)
+        m(T, P) {
+            I(T, e, P), M(e, t), G(n, t, null), M(t, l), M(t, f), g && g.m(f, null), M(e, r), M(e, o), k && k.m(o, null), s = !0, u || (a = [W(t, "click", i[9]), W(t, "click", i[14]), W(t, "mouseover", i[10]), W(t, "mouseenter", i[11]), W(t, "mouseleave", i[12]), W(t, "keydown", i[13]), W(t, "keydown", i[15]), W(e, "animationend", i[8]), W(e, "animationend", i[16])], u = !0)
         },
-        p(T, [D]) {
+        p(T, [P]) {
             const O = {};
-            D & 8 && (O["aria-label"] = T[3]), n.$set(O), d ? d.p && (!s || D & 64) && Pe(d, b, T, T[6], s ? Se(b, T[6], D, _o) : De(T[6]), zi) : g && g.p && (!s || D & 4) && g.p(T, s ? D : -1), (!s || D & 8) && z(t, "title", T[3]), (!s || D & 1) && z(t, "aria-expanded", T[0]), (!s || D & 2) && (t.disabled = T[1]), k && k.p && (!s || D & 64) && Pe(k, _, T, T[6], s ? Se(_, T[6], D, null) : De(T[6]), null), ve(e, B = pe(w, [D & 32 && T[5]])), h(e, "bx--accordion__item", !0), h(e, "bx--accordion__item--active", T[0]), h(e, "bx--accordion__item--disabled", T[1]), h(e, "bx--accordion__item--expanding", T[4] === "expanding"), h(e, "bx--accordion__item--collapsing", T[4] === "collapsing")
+            P & 8 && (O["aria-label"] = T[3]), n.$set(O), d ? d.p && (!s || P & 64) && Pe(d, b, T, T[6], s ? Se(b, T[6], P, _o) : De(T[6]), zi) : g && g.p && (!s || P & 4) && g.p(T, s ? P : -1), (!s || P & 8) && z(t, "title", T[3]), (!s || P & 1) && z(t, "aria-expanded", T[0]), (!s || P & 2) && (t.disabled = T[1]), k && k.p && (!s || P & 64) && Pe(k, _, T, T[6], s ? Se(_, T[6], P, null) : De(T[6]), null), ve(e, B = pe(w, [P & 32 && T[5]])), h(e, "bx--accordion__item", !0), h(e, "bx--accordion__item--active", T[0]), h(e, "bx--accordion__item--disabled", T[1]), h(e, "bx--accordion__item--expanding", T[4] === "expanding"), h(e, "bx--accordion__item--collapsing", T[4] === "collapsing")
         },
         i(T) {
             s || (v(n.$$.fragment, T), v(g, T), v(k, T), s = !0)
         },
         o(T) {
             A(n.$$.fragment, T), A(g, T), A(k, T), s = !1
         },
@@ -4079,15 +4079,15 @@
         J.call(this, i, L)
     }
 
     function T(L) {
         J.call(this, i, L)
     }
 
-    function D(L) {
+    function P(L) {
         J.call(this, i, L)
     }
 
     function O(L) {
         J.call(this, i, L)
     }
     const R = () => {
@@ -4099,15 +4099,15 @@
             s && L === "Escape" && t(0, s = !1)
         },
         q = () => {
             t(4, _ = void 0)
         };
     return i.$$set = L => {
         e = Z(Z({}, e), ce(L)), t(5, l = ie(e, n)), "title" in L && t(2, o = L.title), "open" in L && t(0, s = L.open), "disabled" in L && t(1, u = L.disabled), "iconDescription" in L && t(3, a = L.iconDescription), "$$scope" in L && t(6, r = L.$$scope)
-    }, [s, u, o, a, _, l, r, f, k, w, B, T, D, O, R, U, q]
+    }, [s, u, o, a, _, l, r, f, k, w, B, T, P, O, R, U, q]
 }
 class vo extends ge {
     constructor(e) {
         super(), be(this, e, ko, go, _e, {
             title: 2,
             open: 0,
             disabled: 1,
@@ -4843,21 +4843,21 @@
         d(n) {
             n && E(e)
         }
     }
 }
 
 function Uo(i) {
-    let e, t, n, l, f, r, o, s, u, a, b, d, g, _, k, w, B, T, D, O, R, U, q, L, C = i[16] && Pi(i),
+    let e, t, n, l, f, r, o, s, u, a, b, d, g, _, k, w, B, T, P, O, R, U, q, L, C = i[16] && Pi(i),
         ne = !i[16] && (i[9] || i[26].labelText) && Hi(i);
     const j = [Ro, Ho],
         N = [];
 
-    function Y(P, we) {
-        return P[17] ? 0 : 1
+    function Y(D, we) {
+        return D[17] ? 0 : 1
     }
     r = Y(i), o = N[r] = j[r](i);
     let se = [{
             "data-invalid": a = i[21] || void 0
         }, {
             "aria-invalid": b = i[21] || void 0
         }, {
@@ -4874,67 +4874,67 @@
             placeholder: i[3]
         }, {
             required: i[15]
         }, {
             readOnly: i[17]
         }, i[25]],
         ke = {};
-    for (let P = 0; P < se.length; P += 1) ke = Z(ke, se[P]);
+    for (let D = 0; D < se.length; D += 1) ke = Z(ke, se[D]);
     let he = i[22] && qi(),
         F = i[22] && !i[16] && i[11] && Oi(i),
         x = i[22] && !i[16] && i[13] && Vi(i),
         Ce = !i[11] && !i[13] && !i[22] && !i[16] && i[6] && Yi(i),
         Ee = !i[22] && i[11] && Zi(i),
         Te = !i[22] && !i[11] && i[13] && Wi(i);
     return {
         c() {
-            e = V("div"), C && C.c(), t = $(), ne && ne.c(), n = $(), l = V("div"), f = V("div"), o.c(), s = $(), u = V("input"), _ = $(), he && he.c(), k = $(), F && F.c(), w = $(), x && x.c(), D = $(), Ce && Ce.c(), O = $(), Ee && Ee.c(), R = $(), Te && Te.c(), ve(u, ke), h(u, "bx--text-input", !0), h(u, "bx--text-input--light", i[4]), h(u, "bx--text-input--invalid", i[21]), h(u, "bx--text-input--warning", i[13]), h(u, "bx--text-input--sm", i[2] === "sm"), h(u, "bx--text-input--xl", i[2] === "xl"), z(f, "data-invalid", B = i[21] || void 0), z(f, "data-warn", T = i[13] || void 0), h(f, "bx--text-input__field-wrapper", !0), h(f, "bx--text-input__field-wrapper--warning", !i[11] && i[13]), h(l, "bx--text-input__field-outer-wrapper", !0), h(l, "bx--text-input__field-outer-wrapper--inline", i[16]), h(e, "bx--form-item", !0), h(e, "bx--text-input-wrapper", !0), h(e, "bx--text-input-wrapper--inline", i[16]), h(e, "bx--text-input-wrapper--light", i[4]), h(e, "bx--text-input-wrapper--readonly", i[17])
+            e = V("div"), C && C.c(), t = $(), ne && ne.c(), n = $(), l = V("div"), f = V("div"), o.c(), s = $(), u = V("input"), _ = $(), he && he.c(), k = $(), F && F.c(), w = $(), x && x.c(), P = $(), Ce && Ce.c(), O = $(), Ee && Ee.c(), R = $(), Te && Te.c(), ve(u, ke), h(u, "bx--text-input", !0), h(u, "bx--text-input--light", i[4]), h(u, "bx--text-input--invalid", i[21]), h(u, "bx--text-input--warning", i[13]), h(u, "bx--text-input--sm", i[2] === "sm"), h(u, "bx--text-input--xl", i[2] === "xl"), z(f, "data-invalid", B = i[21] || void 0), z(f, "data-warn", T = i[13] || void 0), h(f, "bx--text-input__field-wrapper", !0), h(f, "bx--text-input__field-wrapper--warning", !i[11] && i[13]), h(l, "bx--text-input__field-outer-wrapper", !0), h(l, "bx--text-input__field-outer-wrapper--inline", i[16]), h(e, "bx--form-item", !0), h(e, "bx--text-input-wrapper", !0), h(e, "bx--text-input-wrapper--inline", i[16]), h(e, "bx--text-input-wrapper--light", i[4]), h(e, "bx--text-input-wrapper--readonly", i[17])
         },
-        m(P, we) {
-            I(P, e, we), C && C.m(e, null), M(e, t), ne && ne.m(e, null), M(e, n), M(e, l), M(l, f), N[r].m(f, null), M(f, s), M(f, u), u.autofocus && u.focus(), i[38](u), Et(u, i[0]), M(f, _), he && he.m(f, null), M(f, k), F && F.m(f, null), M(f, w), x && x.m(f, null), M(l, D), Ce && Ce.m(l, null), M(l, O), Ee && Ee.m(l, null), M(l, R), Te && Te.m(l, null), U = !0, q || (L = [W(u, "input", i[39]), W(u, "change", i[24]), W(u, "input", i[23]), W(u, "keydown", i[33]), W(u, "keyup", i[34]), W(u, "focus", i[35]), W(u, "blur", i[36]), W(u, "paste", i[37]), W(e, "click", i[29]), W(e, "mouseover", i[30]), W(e, "mouseenter", i[31]), W(e, "mouseleave", i[32])], q = !0)
+        m(D, we) {
+            I(D, e, we), C && C.m(e, null), M(e, t), ne && ne.m(e, null), M(e, n), M(e, l), M(l, f), N[r].m(f, null), M(f, s), M(f, u), u.autofocus && u.focus(), i[38](u), Et(u, i[0]), M(f, _), he && he.m(f, null), M(f, k), F && F.m(f, null), M(f, w), x && x.m(f, null), M(l, P), Ce && Ce.m(l, null), M(l, O), Ee && Ee.m(l, null), M(l, R), Te && Te.m(l, null), U = !0, q || (L = [W(u, "input", i[39]), W(u, "change", i[24]), W(u, "input", i[23]), W(u, "keydown", i[33]), W(u, "keyup", i[34]), W(u, "focus", i[35]), W(u, "blur", i[36]), W(u, "paste", i[37]), W(e, "click", i[29]), W(e, "mouseover", i[30]), W(e, "mouseenter", i[31]), W(e, "mouseleave", i[32])], q = !0)
         },
-        p(P, we) {
-            P[16] ? C ? (C.p(P, we), we[0] & 65536 && v(C, 1)) : (C = Pi(P), C.c(), v(C, 1), C.m(e, t)) : C && (de(), A(C, 1, 1, () => {
+        p(D, we) {
+            D[16] ? C ? (C.p(D, we), we[0] & 65536 && v(C, 1)) : (C = Pi(D), C.c(), v(C, 1), C.m(e, t)) : C && (de(), A(C, 1, 1, () => {
                 C = null
-            }), me()), !P[16] && (P[9] || P[26].labelText) ? ne ? (ne.p(P, we), we[0] & 67174912 && v(ne, 1)) : (ne = Hi(P), ne.c(), v(ne, 1), ne.m(e, n)) : ne && (de(), A(ne, 1, 1, () => {
+            }), me()), !D[16] && (D[9] || D[26].labelText) ? ne ? (ne.p(D, we), we[0] & 67174912 && v(ne, 1)) : (ne = Hi(D), ne.c(), v(ne, 1), ne.m(e, n)) : ne && (de(), A(ne, 1, 1, () => {
                 ne = null
             }), me());
             let fe = r;
-            r = Y(P), r === fe ? N[r].p(P, we) : (de(), A(N[fe], 1, 1, () => {
+            r = Y(D), r === fe ? N[r].p(D, we) : (de(), A(N[fe], 1, 1, () => {
                 N[fe] = null
-            }), me(), o = N[r], o ? o.p(P, we) : (o = N[r] = j[r](P), o.c()), v(o, 1), o.m(f, s)), ve(u, ke = pe(se, [(!U || we[0] & 2097152 && a !== (a = P[21] || void 0)) && {
+            }), me(), o = N[r], o ? o.p(D, we) : (o = N[r] = j[r](D), o.c()), v(o, 1), o.m(f, s)), ve(u, ke = pe(se, [(!U || we[0] & 2097152 && a !== (a = D[21] || void 0)) && {
                 "data-invalid": a
-            }, (!U || we[0] & 2097152 && b !== (b = P[21] || void 0)) && {
+            }, (!U || we[0] & 2097152 && b !== (b = D[21] || void 0)) && {
                 "aria-invalid": b
-            }, (!U || we[0] & 8192 && d !== (d = P[13] || void 0)) && {
+            }, (!U || we[0] & 8192 && d !== (d = D[13] || void 0)) && {
                 "data-warn": d
-            }, (!U || we[0] & 3940416 && g !== (g = P[21] ? P[19] : P[13] ? P[18] : P[6] ? P[20] : void 0)) && {
+            }, (!U || we[0] & 3940416 && g !== (g = D[21] ? D[19] : D[13] ? D[18] : D[6] ? D[20] : void 0)) && {
                 "aria-describedby": g
             }, (!U || we[0] & 32) && {
-                disabled: P[5]
+                disabled: D[5]
             }, (!U || we[0] & 128) && {
-                id: P[7]
+                id: D[7]
             }, (!U || we[0] & 256) && {
-                name: P[8]
+                name: D[8]
             }, (!U || we[0] & 8) && {
-                placeholder: P[3]
+                placeholder: D[3]
             }, (!U || we[0] & 32768) && {
-                required: P[15]
+                required: D[15]
             }, (!U || we[0] & 131072) && {
-                readOnly: P[17]
-            }, we[0] & 33554432 && P[25]])), we[0] & 1 && u.value !== P[0] && Et(u, P[0]), h(u, "bx--text-input", !0), h(u, "bx--text-input--light", P[4]), h(u, "bx--text-input--invalid", P[21]), h(u, "bx--text-input--warning", P[13]), h(u, "bx--text-input--sm", P[2] === "sm"), h(u, "bx--text-input--xl", P[2] === "xl"), P[22] ? he || (he = qi(), he.c(), he.m(f, k)) : he && (he.d(1), he = null), P[22] && !P[16] && P[11] ? F ? F.p(P, we) : (F = Oi(P), F.c(), F.m(f, w)) : F && (F.d(1), F = null), P[22] && !P[16] && P[13] ? x ? x.p(P, we) : (x = Vi(P), x.c(), x.m(f, null)) : x && (x.d(1), x = null), (!U || we[0] & 2097152 && B !== (B = P[21] || void 0)) && z(f, "data-invalid", B), (!U || we[0] & 8192 && T !== (T = P[13] || void 0)) && z(f, "data-warn", T), (!U || we[0] & 10240) && h(f, "bx--text-input__field-wrapper--warning", !P[11] && P[13]), !P[11] && !P[13] && !P[22] && !P[16] && P[6] ? Ce ? Ce.p(P, we) : (Ce = Yi(P), Ce.c(), Ce.m(l, O)) : Ce && (Ce.d(1), Ce = null), !P[22] && P[11] ? Ee ? Ee.p(P, we) : (Ee = Zi(P), Ee.c(), Ee.m(l, R)) : Ee && (Ee.d(1), Ee = null), !P[22] && !P[11] && P[13] ? Te ? Te.p(P, we) : (Te = Wi(P), Te.c(), Te.m(l, null)) : Te && (Te.d(1), Te = null), (!U || we[0] & 65536) && h(l, "bx--text-input__field-outer-wrapper--inline", P[16]), (!U || we[0] & 65536) && h(e, "bx--text-input-wrapper--inline", P[16]), (!U || we[0] & 16) && h(e, "bx--text-input-wrapper--light", P[4]), (!U || we[0] & 131072) && h(e, "bx--text-input-wrapper--readonly", P[17])
+                readOnly: D[17]
+            }, we[0] & 33554432 && D[25]])), we[0] & 1 && u.value !== D[0] && Et(u, D[0]), h(u, "bx--text-input", !0), h(u, "bx--text-input--light", D[4]), h(u, "bx--text-input--invalid", D[21]), h(u, "bx--text-input--warning", D[13]), h(u, "bx--text-input--sm", D[2] === "sm"), h(u, "bx--text-input--xl", D[2] === "xl"), D[22] ? he || (he = qi(), he.c(), he.m(f, k)) : he && (he.d(1), he = null), D[22] && !D[16] && D[11] ? F ? F.p(D, we) : (F = Oi(D), F.c(), F.m(f, w)) : F && (F.d(1), F = null), D[22] && !D[16] && D[13] ? x ? x.p(D, we) : (x = Vi(D), x.c(), x.m(f, null)) : x && (x.d(1), x = null), (!U || we[0] & 2097152 && B !== (B = D[21] || void 0)) && z(f, "data-invalid", B), (!U || we[0] & 8192 && T !== (T = D[13] || void 0)) && z(f, "data-warn", T), (!U || we[0] & 10240) && h(f, "bx--text-input__field-wrapper--warning", !D[11] && D[13]), !D[11] && !D[13] && !D[22] && !D[16] && D[6] ? Ce ? Ce.p(D, we) : (Ce = Yi(D), Ce.c(), Ce.m(l, O)) : Ce && (Ce.d(1), Ce = null), !D[22] && D[11] ? Ee ? Ee.p(D, we) : (Ee = Zi(D), Ee.c(), Ee.m(l, R)) : Ee && (Ee.d(1), Ee = null), !D[22] && !D[11] && D[13] ? Te ? Te.p(D, we) : (Te = Wi(D), Te.c(), Te.m(l, null)) : Te && (Te.d(1), Te = null), (!U || we[0] & 65536) && h(l, "bx--text-input__field-outer-wrapper--inline", D[16]), (!U || we[0] & 65536) && h(e, "bx--text-input-wrapper--inline", D[16]), (!U || we[0] & 16) && h(e, "bx--text-input-wrapper--light", D[4]), (!U || we[0] & 131072) && h(e, "bx--text-input-wrapper--readonly", D[17])
         },
-        i(P) {
+        i(D) {
             U || (v(C), v(ne), v(o), U = !0)
         },
-        o(P) {
+        o(D) {
             A(C), A(ne), A(o), U = !1
         },
-        d(P) {
-            P && E(e), C && C.d(), ne && ne.d(), N[r].d(), i[38](null), he && he.d(), F && F.d(), x && x.d(), Ce && Ce.d(), Ee && Ee.d(), Te && Te.d(), q = !1, Le(L)
+        d(D) {
+            D && E(e), C && C.d(), ne && ne.d(), N[r].d(), i[38](null), he && he.d(), F && F.d(), x && x.d(), Ce && Ce.d(), Ee && Ee.d(), Te && Te.d(), q = !1, Le(L)
         }
     }
 }
 
 function qo(i, e, t) {
     let n, l, f, r, o;
     const s = ["size", "value", "placeholder", "light", "disabled", "helperText", "id", "name", "labelText", "hideLabel", "invalid", "invalidText", "warn", "warnText", "ref", "required", "inline", "readonly"];
@@ -4953,15 +4953,15 @@
     } = e, {
         light: w = !1
     } = e, {
         disabled: B = !1
     } = e, {
         helperText: T = ""
     } = e, {
-        id: D = "ccs-" + Math.random().toString(36)
+        id: P = "ccs-" + Math.random().toString(36)
     } = e, {
         name: O = void 0
     } = e, {
         labelText: R = ""
     } = e, {
         hideLabel: U = !1
     } = e, {
@@ -4998,15 +4998,15 @@
         J.call(this, i, ue)
     }
 
     function Te(ue) {
         J.call(this, i, ue)
     }
 
-    function P(ue) {
+    function D(ue) {
         J.call(this, i, ue)
     }
 
     function we(ue) {
         J.call(this, i, ue)
     }
 
@@ -5036,18 +5036,18 @@
         })
     }
 
     function ft() {
         _ = this.value, t(0, _)
     }
     return i.$$set = ue => {
-        e = Z(Z({}, e), ce(ue)), t(25, u = ie(e, s)), "size" in ue && t(2, g = ue.size), "value" in ue && t(0, _ = ue.value), "placeholder" in ue && t(3, k = ue.placeholder), "light" in ue && t(4, w = ue.light), "disabled" in ue && t(5, B = ue.disabled), "helperText" in ue && t(6, T = ue.helperText), "id" in ue && t(7, D = ue.id), "name" in ue && t(8, O = ue.name), "labelText" in ue && t(9, R = ue.labelText), "hideLabel" in ue && t(10, U = ue.hideLabel), "invalid" in ue && t(11, q = ue.invalid), "invalidText" in ue && t(12, L = ue.invalidText), "warn" in ue && t(13, C = ue.warn), "warnText" in ue && t(14, ne = ue.warnText), "ref" in ue && t(1, j = ue.ref), "required" in ue && t(15, N = ue.required), "inline" in ue && t(16, Y = ue.inline), "readonly" in ue && t(17, se = ue.readonly), "$$scope" in ue && t(27, b = ue.$$scope)
+        e = Z(Z({}, e), ce(ue)), t(25, u = ie(e, s)), "size" in ue && t(2, g = ue.size), "value" in ue && t(0, _ = ue.value), "placeholder" in ue && t(3, k = ue.placeholder), "light" in ue && t(4, w = ue.light), "disabled" in ue && t(5, B = ue.disabled), "helperText" in ue && t(6, T = ue.helperText), "id" in ue && t(7, P = ue.id), "name" in ue && t(8, O = ue.name), "labelText" in ue && t(9, R = ue.labelText), "hideLabel" in ue && t(10, U = ue.hideLabel), "invalid" in ue && t(11, q = ue.invalid), "invalidText" in ue && t(12, L = ue.invalidText), "warn" in ue && t(13, C = ue.warn), "warnText" in ue && t(14, ne = ue.warnText), "ref" in ue && t(1, j = ue.ref), "required" in ue && t(15, N = ue.required), "inline" in ue && t(16, Y = ue.inline), "readonly" in ue && t(17, se = ue.readonly), "$$scope" in ue && t(27, b = ue.$$scope)
     }, i.$$.update = () => {
-        i.$$.dirty[0] & 133120 && t(21, l = q && !se), i.$$.dirty[0] & 128 && t(20, f = `helper-${D}`), i.$$.dirty[0] & 128 && t(19, r = `error-${D}`), i.$$.dirty[0] & 128 && t(18, o = `warn-${D}`)
-    }, t(22, n = !!ke && ke.isFluid), [_, j, g, k, w, B, T, D, O, R, U, q, L, C, ne, N, Y, se, o, r, f, l, n, x, Ce, u, d, b, a, Ee, Te, P, we, fe, Ge, le, Me, Ye, ot, ft]
+        i.$$.dirty[0] & 133120 && t(21, l = q && !se), i.$$.dirty[0] & 128 && t(20, f = `helper-${P}`), i.$$.dirty[0] & 128 && t(19, r = `error-${P}`), i.$$.dirty[0] & 128 && t(18, o = `warn-${P}`)
+    }, t(22, n = !!ke && ke.isFluid), [_, j, g, k, w, B, T, P, O, R, U, q, L, C, ne, N, Y, se, o, r, f, l, n, x, Ce, u, d, b, a, Ee, Te, D, we, fe, Ge, le, Me, Ye, ot, ft]
 }
 class Oo extends ge {
     constructor(e) {
         super(), be(this, e, qo, Uo, _e, {
             size: 2,
             value: 0,
             placeholder: 3,
@@ -5465,38 +5465,38 @@
     };
     i[0].title !== void 0 && (_.value = i[0].title), n = new $e({
         props: _
     }), ze.push(() => Ve(n, "value", g)), n.$on("blur", i[10]), n.$on("click", i[11]);
     const k = [$o, xo],
         w = [];
 
-    function B(T, D) {
+    function B(T, P) {
         return T[2] ? 1 : 0
     }
     return o = B(i), s = w[o] = k[o](i), a = new xe({
         props: {
             size: "small",
             kind: "ghost",
             icon: Xo,
             iconDescription: "Delete the Chat"
         }
     }), a.$on("click", i[4]), {
         c() {
             e = V("div"), t = V("div"), X(n.$$.fragment), f = $(), r = V("div"), s.c(), u = $(), X(a.$$.fragment), z(t, "class", "input svelte-1hg40nj"), z(r, "class", "actions svelte-1hg40nj"), z(e, "class", b = "chat-history-item " + (i[1] ? "current" : "") + " svelte-1hg40nj")
         },
-        m(T, D) {
-            I(T, e, D), M(e, t), G(n, t, null), M(e, f), M(e, r), w[o].m(r, null), M(r, u), G(a, r, null), d = !0
+        m(T, P) {
+            I(T, e, P), M(e, t), G(n, t, null), M(e, f), M(e, r), w[o].m(r, null), M(r, u), G(a, r, null), d = !0
         },
-        p(T, [D]) {
+        p(T, [P]) {
             const O = {};
-            D & 1 && (O.id = T[0].name + "-title"), D & 4 && (O.readonly = !T[2]), !l && D & 1 && (l = !0, O.value = T[0].title, Oe(() => l = !1)), n.$set(O);
+            P & 1 && (O.id = T[0].name + "-title"), P & 4 && (O.readonly = !T[2]), !l && P & 1 && (l = !0, O.value = T[0].title, Oe(() => l = !1)), n.$set(O);
             let R = o;
-            o = B(T), o === R ? w[o].p(T, D) : (de(), A(w[R], 1, 1, () => {
+            o = B(T), o === R ? w[o].p(T, P) : (de(), A(w[R], 1, 1, () => {
                 w[R] = null
-            }), me(), s = w[o], s ? s.p(T, D) : (s = w[o] = k[o](T), s.c()), v(s, 1), s.m(r, u)), (!d || D & 2 && b !== (b = "chat-history-item " + (T[1] ? "current" : "") + " svelte-1hg40nj")) && z(e, "class", b)
+            }), me(), s = w[o], s ? s.p(T, P) : (s = w[o] = k[o](T), s.c()), v(s, 1), s.m(r, u)), (!d || P & 2 && b !== (b = "chat-history-item " + (T[1] ? "current" : "") + " svelte-1hg40nj")) && z(e, "class", b)
         },
         i(T) {
             d || (v(n.$$.fragment, T), v(s), v(a.$$.fragment, T), d = !0)
         },
         o(T) {
             A(n.$$.fragment, T), A(s), A(a.$$.fragment, T), d = !1
         },
@@ -5714,22 +5714,22 @@
         }, {
             readOnly: i[8]
         }, {
             maxlength: s = i[5] ?? void 0
         }, i[18]],
         T = {};
     for (let R = 0; R < B.length; R += 1) T = Z(T, B[R]);
-    let D = !i[12] && i[9] && $i(i),
+    let P = !i[12] && i[9] && $i(i),
         O = i[12] && en(i);
     return {
         c() {
-            e = V("div"), k && k.c(), t = $(), n = V("div"), w && w.c(), l = $(), f = V("textarea"), a = $(), D && D.c(), b = $(), O && O.c(), ve(f, T), h(f, "bx--text-area", !0), h(f, "bx--text-area--light", i[6]), h(f, "bx--text-area--invalid", i[12]), z(n, "data-invalid", u = i[12] || void 0), h(n, "bx--text-area__wrapper", !0), h(e, "bx--form-item", !0)
+            e = V("div"), k && k.c(), t = $(), n = V("div"), w && w.c(), l = $(), f = V("textarea"), a = $(), P && P.c(), b = $(), O && O.c(), ve(f, T), h(f, "bx--text-area", !0), h(f, "bx--text-area--light", i[6]), h(f, "bx--text-area--invalid", i[12]), z(n, "data-invalid", u = i[12] || void 0), h(n, "bx--text-area__wrapper", !0), h(e, "bx--form-item", !0)
         },
         m(R, U) {
-            I(R, e, U), k && k.m(e, null), M(e, t), M(e, n), w && w.m(n, null), M(n, l), M(n, f), f.autofocus && f.focus(), i[32](f), Et(f, i[0]), M(e, a), D && D.m(e, null), M(e, b), O && O.m(e, null), d = !0, g || (_ = [W(f, "input", i[33]), W(f, "change", i[25]), W(f, "input", i[26]), W(f, "keydown", i[27]), W(f, "keyup", i[28]), W(f, "focus", i[29]), W(f, "blur", i[30]), W(f, "paste", i[31]), W(e, "click", i[21]), W(e, "mouseover", i[22]), W(e, "mouseenter", i[23]), W(e, "mouseleave", i[24])], g = !0)
+            I(R, e, U), k && k.m(e, null), M(e, t), M(e, n), w && w.m(n, null), M(n, l), M(n, f), f.autofocus && f.focus(), i[32](f), Et(f, i[0]), M(e, a), P && P.m(e, null), M(e, b), O && O.m(e, null), d = !0, g || (_ = [W(f, "input", i[33]), W(f, "change", i[25]), W(f, "input", i[26]), W(f, "keydown", i[27]), W(f, "keyup", i[28]), W(f, "focus", i[29]), W(f, "blur", i[30]), W(f, "paste", i[31]), W(e, "click", i[21]), W(e, "mouseover", i[22]), W(e, "mouseenter", i[23]), W(e, "mouseleave", i[24])], g = !0)
         },
         p(R, U) {
             (R[10] || R[17].labelText) && !R[11] ? k ? (k.p(R, U), U[0] & 134144 && v(k, 1)) : (k = Xi(R), k.c(), v(k, 1), k.m(e, t)) : k && (de(), A(k, 1, 1, () => {
                 k = null
             }), me()), R[12] ? w ? U[0] & 4096 && v(w, 1) : (w = xi(), w.c(), v(w, 1), w.m(n, l)) : w && (de(), A(w, 1, 1, () => {
                 w = null
             }), me()), ve(f, T = pe(B, [(!d || U[0] & 4096 && r !== (r = R[12] || void 0)) && {
@@ -5748,24 +5748,24 @@
                 rows: R[4]
             }, (!d || U[0] & 4) && {
                 placeholder: R[2]
             }, (!d || U[0] & 256) && {
                 readOnly: R[8]
             }, (!d || U[0] & 32 && s !== (s = R[5] ?? void 0)) && {
                 maxlength: s
-            }, U[0] & 262144 && R[18]])), U[0] & 1 && Et(f, R[0]), h(f, "bx--text-area", !0), h(f, "bx--text-area--light", R[6]), h(f, "bx--text-area--invalid", R[12]), (!d || U[0] & 4096 && u !== (u = R[12] || void 0)) && z(n, "data-invalid", u), !R[12] && R[9] ? D ? D.p(R, U) : (D = $i(R), D.c(), D.m(e, b)) : D && (D.d(1), D = null), R[12] ? O ? O.p(R, U) : (O = en(R), O.c(), O.m(e, null)) : O && (O.d(1), O = null)
+            }, U[0] & 262144 && R[18]])), U[0] & 1 && Et(f, R[0]), h(f, "bx--text-area", !0), h(f, "bx--text-area--light", R[6]), h(f, "bx--text-area--invalid", R[12]), (!d || U[0] & 4096 && u !== (u = R[12] || void 0)) && z(n, "data-invalid", u), !R[12] && R[9] ? P ? P.p(R, U) : (P = $i(R), P.c(), P.m(e, b)) : P && (P.d(1), P = null), R[12] ? O ? O.p(R, U) : (O = en(R), O.c(), O.m(e, null)) : O && (O.d(1), O = null)
         },
         i(R) {
             d || (v(k), v(w), d = !0)
         },
         o(R) {
             A(k), A(w), d = !1
         },
         d(R) {
-            R && E(e), k && k.d(), w && w.d(), i[32](null), D && D.d(), O && O.d(), g = !1, Le(_)
+            R && E(e), k && k.d(), w && w.d(), i[32](null), P && P.d(), O && O.d(), g = !1, Le(_)
         }
     }
 }
 
 function ff(i, e, t) {
     let n;
     const l = ["value", "placeholder", "cols", "rows", "maxCount", "light", "disabled", "readonly", "helperText", "labelText", "hideLabel", "invalid", "invalidText", "id", "name", "ref"];
@@ -5792,85 +5792,85 @@
     } = e, {
         readonly: w = !1
     } = e, {
         helperText: B = ""
     } = e, {
         labelText: T = ""
     } = e, {
-        hideLabel: D = !1
+        hideLabel: P = !1
     } = e, {
         invalid: O = !1
     } = e, {
         invalidText: R = ""
     } = e, {
         id: U = "ccs-" + Math.random().toString(36)
     } = e, {
         name: q = void 0
     } = e, {
         ref: L = null
     } = e;
 
-    function C(P) {
-        J.call(this, i, P)
+    function C(D) {
+        J.call(this, i, D)
     }
 
-    function ne(P) {
-        J.call(this, i, P)
+    function ne(D) {
+        J.call(this, i, D)
     }
 
-    function j(P) {
-        J.call(this, i, P)
+    function j(D) {
+        J.call(this, i, D)
     }
 
-    function N(P) {
-        J.call(this, i, P)
+    function N(D) {
+        J.call(this, i, D)
     }
 
-    function Y(P) {
-        J.call(this, i, P)
+    function Y(D) {
+        J.call(this, i, D)
     }
 
-    function se(P) {
-        J.call(this, i, P)
+    function se(D) {
+        J.call(this, i, D)
     }
 
-    function ke(P) {
-        J.call(this, i, P)
+    function ke(D) {
+        J.call(this, i, D)
     }
 
-    function he(P) {
-        J.call(this, i, P)
+    function he(D) {
+        J.call(this, i, D)
     }
 
-    function F(P) {
-        J.call(this, i, P)
+    function F(D) {
+        J.call(this, i, D)
     }
 
-    function x(P) {
-        J.call(this, i, P)
+    function x(D) {
+        J.call(this, i, D)
     }
 
-    function Ce(P) {
-        J.call(this, i, P)
+    function Ce(D) {
+        J.call(this, i, D)
     }
 
-    function Ee(P) {
-        ze[P ? "unshift" : "push"](() => {
-            L = P, t(1, L)
+    function Ee(D) {
+        ze[D ? "unshift" : "push"](() => {
+            L = D, t(1, L)
         })
     }
 
     function Te() {
         u = this.value, t(0, u)
     }
-    return i.$$set = P => {
-        e = Z(Z({}, e), ce(P)), t(18, f = ie(e, l)), "value" in P && t(0, u = P.value), "placeholder" in P && t(2, a = P.placeholder), "cols" in P && t(3, b = P.cols), "rows" in P && t(4, d = P.rows), "maxCount" in P && t(5, g = P.maxCount), "light" in P && t(6, _ = P.light), "disabled" in P && t(7, k = P.disabled), "readonly" in P && t(8, w = P.readonly), "helperText" in P && t(9, B = P.helperText), "labelText" in P && t(10, T = P.labelText), "hideLabel" in P && t(11, D = P.hideLabel), "invalid" in P && t(12, O = P.invalid), "invalidText" in P && t(13, R = P.invalidText), "id" in P && t(14, U = P.id), "name" in P && t(15, q = P.name), "ref" in P && t(1, L = P.ref), "$$scope" in P && t(19, o = P.$$scope)
+    return i.$$set = D => {
+        e = Z(Z({}, e), ce(D)), t(18, f = ie(e, l)), "value" in D && t(0, u = D.value), "placeholder" in D && t(2, a = D.placeholder), "cols" in D && t(3, b = D.cols), "rows" in D && t(4, d = D.rows), "maxCount" in D && t(5, g = D.maxCount), "light" in D && t(6, _ = D.light), "disabled" in D && t(7, k = D.disabled), "readonly" in D && t(8, w = D.readonly), "helperText" in D && t(9, B = D.helperText), "labelText" in D && t(10, T = D.labelText), "hideLabel" in D && t(11, P = D.hideLabel), "invalid" in D && t(12, O = D.invalid), "invalidText" in D && t(13, R = D.invalidText), "id" in D && t(14, U = D.id), "name" in D && t(15, q = D.name), "ref" in D && t(1, L = D.ref), "$$scope" in D && t(19, o = D.$$scope)
     }, i.$$.update = () => {
         i.$$.dirty[0] & 16384 && t(16, n = `error-${U}`)
-    }, [u, L, a, b, d, g, _, k, w, B, T, D, O, R, U, q, n, s, f, o, r, C, ne, j, N, Y, se, ke, he, F, x, Ce, Ee, Te]
+    }, [u, L, a, b, d, g, _, k, w, B, T, P, O, R, U, q, n, s, f, o, r, C, ne, j, N, Y, se, ke, he, F, x, Ce, Ee, Te]
 }
 class sf extends ge {
     constructor(e) {
         super(), be(this, e, ff, of, _e, {
             value: 0,
             placeholder: 2,
             cols: 3,
@@ -6472,16 +6472,16 @@
             iconDescription: i[6]
         }
     });
     const k = i[13].title,
         w = Fe(k, i, i[12], sn),
         B = w || Df(i),
         T = i[13].subtitle,
-        D = Fe(T, i, i[12], fn),
-        O = D || Nf(i),
+        P = Fe(T, i, i[12], fn),
+        O = P || Nf(i),
         R = i[13].default,
         U = Fe(R, i, i[12], null),
         q = i[13].actions,
         L = Fe(q, i, i[12], on);
     let C = !i[5] && an(i),
         ne = [{
             role: i[2]
@@ -6495,15 +6495,15 @@
             e = V("div"), t = V("div"), X(n.$$.fragment), l = $(), f = V("div"), r = V("p"), B && B.c(), o = $(), s = V("div"), O && O.c(), u = $(), U && U.c(), a = $(), L && L.c(), b = $(), C && C.c(), h(r, "bx--inline-notification__title", !0), h(s, "bx--inline-notification__subtitle", !0), h(f, "bx--inline-notification__text-wrapper", !0), h(t, "bx--inline-notification__details", !0), ve(e, j), h(e, "bx--inline-notification", !0), h(e, "bx--inline-notification--low-contrast", i[1]), h(e, "bx--inline-notification--hide-close-button", i[5]), h(e, "bx--inline-notification--error", i[0] === "error"), h(e, "bx--inline-notification--info", i[0] === "info"), h(e, "bx--inline-notification--info-square", i[0] === "info-square"), h(e, "bx--inline-notification--success", i[0] === "success"), h(e, "bx--inline-notification--warning", i[0] === "warning"), h(e, "bx--inline-notification--warning-alt", i[0] === "warning-alt")
         },
         m(N, Y) {
             I(N, e, Y), M(e, t), G(n, t, null), M(t, l), M(t, f), M(f, r), B && B.m(r, null), M(f, o), M(f, s), O && O.m(s, null), M(f, u), U && U.m(f, null), M(e, a), L && L.m(e, null), M(e, b), C && C.m(e, null), d = !0, g || (_ = [W(e, "click", i[14]), W(e, "mouseover", i[15]), W(e, "mouseenter", i[16]), W(e, "mouseleave", i[17])], g = !0)
         },
         p(N, Y) {
             const se = {};
-            Y & 1 && (se.kind = N[0]), Y & 64 && (se.iconDescription = N[6]), n.$set(se), w ? w.p && (!d || Y & 4096) && Pe(w, k, N, N[12], d ? Se(k, N[12], Y, Pf) : De(N[12]), sn) : B && B.p && (!d || Y & 8) && B.p(N, d ? Y : -1), D ? D.p && (!d || Y & 4096) && Pe(D, T, N, N[12], d ? Se(T, N[12], Y, Sf) : De(N[12]), fn) : O && O.p && (!d || Y & 16) && O.p(N, d ? Y : -1), U && U.p && (!d || Y & 4096) && Pe(U, R, N, N[12], d ? Se(R, N[12], Y, null) : De(N[12]), null), L && L.p && (!d || Y & 4096) && Pe(L, q, N, N[12], d ? Se(q, N[12], Y, Ff) : De(N[12]), on), N[5] ? C && (de(), A(C, 1, 1, () => {
+            Y & 1 && (se.kind = N[0]), Y & 64 && (se.iconDescription = N[6]), n.$set(se), w ? w.p && (!d || Y & 4096) && Pe(w, k, N, N[12], d ? Se(k, N[12], Y, Pf) : De(N[12]), sn) : B && B.p && (!d || Y & 8) && B.p(N, d ? Y : -1), P ? P.p && (!d || Y & 4096) && Pe(P, T, N, N[12], d ? Se(T, N[12], Y, Sf) : De(N[12]), fn) : O && O.p && (!d || Y & 16) && O.p(N, d ? Y : -1), U && U.p && (!d || Y & 4096) && Pe(U, R, N, N[12], d ? Se(R, N[12], Y, null) : De(N[12]), null), L && L.p && (!d || Y & 4096) && Pe(L, q, N, N[12], d ? Se(q, N[12], Y, Ff) : De(N[12]), on), N[5] ? C && (de(), A(C, 1, 1, () => {
                 C = null
             }), me()) : C ? (C.p(N, Y), Y & 32 && v(C, 1)) : (C = an(N), C.c(), v(C, 1), C.m(e, null)), ve(e, j = pe(ne, [(!d || Y & 4) && {
                 role: N[2]
             }, (!d || Y & 1) && {
                 kind: N[0]
             }, Y & 1024 && N[10]])), h(e, "bx--inline-notification", !0), h(e, "bx--inline-notification--low-contrast", N[1]), h(e, "bx--inline-notification--hide-close-button", N[5]), h(e, "bx--inline-notification--error", N[0] === "error"), h(e, "bx--inline-notification--info", N[0] === "info"), h(e, "bx--inline-notification--info-square", N[0] === "info-square"), h(e, "bx--inline-notification--success", N[0] === "success"), h(e, "bx--inline-notification--warning", N[0] === "warning"), h(e, "bx--inline-notification--warning-alt", N[0] === "warning-alt")
         },
@@ -6645,22 +6645,22 @@
         {
             closeButtonDescription: k = "Close notification"
         } = e;
     const w = je();
     let B = !0,
         T;
 
-    function D(L) {
+    function P(L) {
         w("close", {
             timeout: L === !0
         }, {
             cancelable: !0
         }) && t(8, B = !1)
     }
-    at(() => (u && (T = setTimeout(() => D(!0), u)), () => {
+    at(() => (u && (T = setTimeout(() => P(!0), u)), () => {
         clearTimeout(T)
     }));
 
     function O(L) {
         J.call(this, i, L)
     }
 
@@ -6673,15 +6673,15 @@
     }
 
     function q(L) {
         J.call(this, i, L)
     }
     return i.$$set = L => {
         e = Z(Z({}, e), ce(L)), t(10, l = ie(e, n)), "kind" in L && t(0, o = L.kind), "lowContrast" in L && t(1, s = L.lowContrast), "timeout" in L && t(11, u = L.timeout), "role" in L && t(2, a = L.role), "title" in L && t(3, b = L.title), "subtitle" in L && t(4, d = L.subtitle), "hideCloseButton" in L && t(5, g = L.hideCloseButton), "statusIconDescription" in L && t(6, _ = L.statusIconDescription), "closeButtonDescription" in L && t(7, k = L.closeButtonDescription), "$$scope" in L && t(12, r = L.$$scope)
-    }, [o, s, a, b, d, g, _, k, B, D, l, u, r, f, O, R, U, q]
+    }, [o, s, a, b, d, g, _, k, B, P, l, u, r, f, O, R, U, q]
 }
 class Uf extends ge {
     constructor(e) {
         super(), be(this, e, Rf, Hf, _e, {
             kind: 0,
             lowContrast: 1,
             timeout: 11,
@@ -7438,15 +7438,15 @@
             K(e, n)
         }
     }
 }
 
 function _s(i) {
     let e, t, n, l, f, r, o, s, u, a, b = i[0].when + "",
-        d, g, _, k, w, B, T, D;
+        d, g, _, k, w, B, T, P;
     const O = [fs, os],
         R = [];
 
     function U(Y, se) {
         return Y[0].who === "human" ? 0 : 1
     }
     n = U(i), l = R[n] = O[n](i);
@@ -7463,15 +7463,15 @@
         return Y[0].kind === "querying" && Y[0].message === "" ? 0 : Y[0].kind === "canceling" ? 1 : Y[0].kind === "cancelled" ? 2 : Y[0].kind === "error" ? 3 : 4
     }
     return k = N(i), w = j[k] = ne[k](i), {
         c() {
             e = V("div"), t = V("div"), l.c(), f = $(), r = V("div"), s && s.c(), u = $(), a = V("div"), d = oe(b), g = $(), _ = V("div"), w.c(), z(t, "class", "avatar"), z(a, "class", "message-when svelte-11331u1"), z(_, "class", "message-message svelte-11331u1"), z(r, "class", "message svelte-11331u1"), z(e, "class", "conversation svelte-11331u1")
         },
         m(Y, se) {
-            I(Y, e, se), M(e, t), R[n].m(t, null), M(e, f), M(e, r), ~o && L[o].m(r, null), M(r, u), M(r, a), M(a, d), M(r, g), M(r, _), j[k].m(_, null), B = !0, T || (D = [W(r, "mouseenter", i[3]), W(r, "mouseleave", i[4])], T = !0)
+            I(Y, e, se), M(e, t), R[n].m(t, null), M(e, f), M(e, r), ~o && L[o].m(r, null), M(r, u), M(r, a), M(a, d), M(r, g), M(r, _), j[k].m(_, null), B = !0, T || (P = [W(r, "mouseenter", i[3]), W(r, "mouseleave", i[4])], T = !0)
         },
         p(Y, [se]) {
             let ke = n;
             n = U(Y), n !== ke && (de(), A(R[ke], 1, 1, () => {
                 R[ke] = null
             }), me(), l = R[n], l || (l = R[n] = O[n](Y), l.c()), v(l, 1), l.m(t, null));
             let he = o;
@@ -7486,15 +7486,15 @@
         i(Y) {
             B || (v(l), v(s), v(w), B = !0)
         },
         o(Y) {
             A(l), A(s), A(w), B = !1
         },
         d(Y) {
-            Y && E(e), R[n].d(), ~o && L[o].d(), j[k].d(), T = !1, Le(D)
+            Y && E(e), R[n].d(), ~o && L[o].d(), j[k].d(), T = !1, Le(P)
         }
     }
 }
 
 function bs(i, e, t) {
     let {
         message: n
@@ -7570,15 +7570,15 @@
     }
 }
 
 function vs(i) {
     let e;
     return {
         c() {
-            e = V("div"), e.innerHTML = `<h1>Welcome to the chat!</h1>
+            e = V("div"), e.innerHTML = `<h1>Welcome to the chat!</h1> 
                 <p>Start by typing a message below.</p>`, z(e, "class", "welcome svelte-1v6ibam")
         },
         m(t, n) {
             I(t, e, n)
         },
         p: ee,
         i: ee,
@@ -7675,17 +7675,17 @@
         c() {
             e = V("div"), t = V("div"), l.c(), f = $(), _ && _.c(), r = $(), o = V("div"), X(s.$$.fragment), z(t, "class", "chat-conversation svelte-1v6ibam"), z(o, "class", "chat-input svelte-1v6ibam"), z(e, "class", "chat-main svelte-1v6ibam")
         },
         m(B, T) {
             I(B, e, T), M(e, t), d[n].m(t, null), i[8](t), M(e, f), _ && _.m(e, null), M(e, r), M(e, o), G(s, o, null), a = !0
         },
         p(B, [T]) {
-            let D = n;
-            n = g(B), n === D ? d[n].p(B, T) : (de(), A(d[D], 1, 1, () => {
-                d[D] = null
+            let P = n;
+            n = g(B), n === P ? d[n].p(B, T) : (de(), A(d[P], 1, 1, () => {
+                d[P] = null
             }), me(), l = d[n], l ? l.p(B, T) : (l = d[n] = b[n](B), l.c()), v(l, 1), l.m(t, null)), B[3].kind ? _ ? (_.p(B, T), T & 8 && v(_, 1)) : (_ = gn(B), _.c(), v(_, 1), _.m(e, r)) : _ && (de(), A(_, 1, 1, () => {
                 _ = null
             }), me());
             const O = {};
             !u && T & 1 && (u = !0, O.ref = B[0], Oe(() => u = !1)), s.$set(O)
         },
         i(B) {
@@ -7747,19 +7747,23 @@
         T.kind === "querying" && (T.kind = void 0), a !== n ? nt.set(a) : t(4, d = [...d.slice(0, -1), T])
     }, Ne.on_responding = function(B) {
         let T = d.at(-1);
         T = {
             ...T,
             message: T.message + B.message
         }, t(4, d = [...d.slice(0, -1), T]), requestAnimationFrame(() => {
-            s.scrollTo(0, s.scrollHeight)
+            try {
+                s.scrollTo(0, s.scrollHeight)
+            } catch {}
         })
     }, Ne.on_conversation_loaded = function(B) {
         t(4, d = B.messages), requestAnimationFrame(() => {
-            s.scrollTo(0, s.scrollHeight)
+            try {
+                s.scrollTo(0, s.scrollHeight)
+            } catch {}
         })
     };
     const _ = B => {
         if (B.ctrlKey && B.keyCode === 13) {
             if (Ne.closed) return;
             if (d.length > 0 && d.at(-1).kind === "querying") {
                 t(3, b = {
@@ -7779,15 +7783,17 @@
                 kind: "querying"
             })]), B.target.value = "", Ne.sendJson({
                 event: "query",
                 query: T.message,
                 profile: u,
                 conversation: a === !0 ? null : a
             }), requestAnimationFrame(() => {
-                s.scrollTo(0, s.scrollHeight)
+                try {
+                    s.scrollTo(0, s.scrollHeight)
+                } catch {}
             })
         }
     };
     at(() => {
         !a || a === "" ? f.focus() : Ne.sendJson({
             event: "load_conversation",
             profile: u,
@@ -8327,46 +8333,46 @@
     }
 }
 
 function Ws(i) {
     let e, t, n, l, f, r, o, s, u, a, b, d, g, _, k, w;
     const B = i[12].labelText,
         T = Fe(B, i, i[11], Tn),
-        D = T || Vs(i),
+        P = T || Vs(i),
         O = i[12].labelA,
         R = Fe(O, i, i[11], wn),
         U = R || Ys(i),
         q = i[12].labelB,
         L = Fe(q, i, i[11], pn),
         C = L || Zs(i);
     let ne = [i[9], {
             style: g = i[9].style + "; user-select: none"
         }],
         j = {};
     for (let N = 0; N < ne.length; N += 1) j = Z(j, ne[N]);
     return {
         c() {
-            e = V("div"), t = V("input"), n = $(), l = V("label"), f = V("span"), D && D.c(), r = $(), o = V("span"), s = V("span"), U && U.c(), u = $(), a = V("span"), C && C.c(), z(t, "role", "switch"), z(t, "type", "checkbox"), t.checked = i[0], t.disabled = i[2], z(t, "id", i[7]), z(t, "name", i[8]), h(t, "bx--toggle-input", !0), h(t, "bx--toggle-input--small", i[1] === "sm"), h(f, "bx--visually-hidden", i[6]), z(s, "aria-hidden", "true"), h(s, "bx--toggle__text--off", !0), z(a, "aria-hidden", "true"), h(a, "bx--toggle__text--on", !0), z(o, "style", b = i[6] && "margin-top: 0"), h(o, "bx--toggle__switch", !0), z(l, "aria-label", d = i[5] ? void 0 : i[10]["aria-label"] || "Toggle"), z(l, "for", i[7]), h(l, "bx--toggle-input__label", !0), ve(e, j), h(e, "bx--form-item", !0)
+            e = V("div"), t = V("input"), n = $(), l = V("label"), f = V("span"), P && P.c(), r = $(), o = V("span"), s = V("span"), U && U.c(), u = $(), a = V("span"), C && C.c(), z(t, "role", "switch"), z(t, "type", "checkbox"), t.checked = i[0], t.disabled = i[2], z(t, "id", i[7]), z(t, "name", i[8]), h(t, "bx--toggle-input", !0), h(t, "bx--toggle-input--small", i[1] === "sm"), h(f, "bx--visually-hidden", i[6]), z(s, "aria-hidden", "true"), h(s, "bx--toggle__text--off", !0), z(a, "aria-hidden", "true"), h(a, "bx--toggle__text--on", !0), z(o, "style", b = i[6] && "margin-top: 0"), h(o, "bx--toggle__switch", !0), z(l, "aria-label", d = i[5] ? void 0 : i[10]["aria-label"] || "Toggle"), z(l, "for", i[7]), h(l, "bx--toggle-input__label", !0), ve(e, j), h(e, "bx--form-item", !0)
         },
         m(N, Y) {
-            I(N, e, Y), M(e, t), M(e, n), M(e, l), M(l, f), D && D.m(f, null), M(l, r), M(l, o), M(o, s), U && U.m(s, null), M(o, u), M(o, a), C && C.m(a, null), _ = !0, k || (w = [W(t, "change", i[21]), W(t, "change", i[17]), W(t, "keyup", i[22]), W(t, "keyup", i[18]), W(t, "focus", i[19]), W(t, "blur", i[20]), W(e, "click", i[13]), W(e, "mouseover", i[14]), W(e, "mouseenter", i[15]), W(e, "mouseleave", i[16])], k = !0)
+            I(N, e, Y), M(e, t), M(e, n), M(e, l), M(l, f), P && P.m(f, null), M(l, r), M(l, o), M(o, s), U && U.m(s, null), M(o, u), M(o, a), C && C.m(a, null), _ = !0, k || (w = [W(t, "change", i[21]), W(t, "change", i[17]), W(t, "keyup", i[22]), W(t, "keyup", i[18]), W(t, "focus", i[19]), W(t, "blur", i[20]), W(e, "click", i[13]), W(e, "mouseover", i[14]), W(e, "mouseenter", i[15]), W(e, "mouseleave", i[16])], k = !0)
         },
         p(N, [Y]) {
-            (!_ || Y & 1) && (t.checked = N[0]), (!_ || Y & 4) && (t.disabled = N[2]), (!_ || Y & 128) && z(t, "id", N[7]), (!_ || Y & 256) && z(t, "name", N[8]), (!_ || Y & 2) && h(t, "bx--toggle-input--small", N[1] === "sm"), T ? T.p && (!_ || Y & 2048) && Pe(T, B, N, N[11], _ ? Se(B, N[11], Y, Os) : De(N[11]), Tn) : D && D.p && (!_ || Y & 32) && D.p(N, _ ? Y : -1), (!_ || Y & 64) && h(f, "bx--visually-hidden", N[6]), R ? R.p && (!_ || Y & 2048) && Pe(R, O, N, N[11], _ ? Se(O, N[11], Y, qs) : De(N[11]), wn) : U && U.p && (!_ || Y & 8) && U.p(N, _ ? Y : -1), L ? L.p && (!_ || Y & 2048) && Pe(L, q, N, N[11], _ ? Se(q, N[11], Y, Us) : De(N[11]), pn) : C && C.p && (!_ || Y & 16) && C.p(N, _ ? Y : -1), (!_ || Y & 64 && b !== (b = N[6] && "margin-top: 0")) && z(o, "style", b), (!_ || Y & 1056 && d !== (d = N[5] ? void 0 : N[10]["aria-label"] || "Toggle")) && z(l, "aria-label", d), (!_ || Y & 128) && z(l, "for", N[7]), ve(e, j = pe(ne, [Y & 512 && N[9], (!_ || Y & 512 && g !== (g = N[9].style + "; user-select: none")) && {
+            (!_ || Y & 1) && (t.checked = N[0]), (!_ || Y & 4) && (t.disabled = N[2]), (!_ || Y & 128) && z(t, "id", N[7]), (!_ || Y & 256) && z(t, "name", N[8]), (!_ || Y & 2) && h(t, "bx--toggle-input--small", N[1] === "sm"), T ? T.p && (!_ || Y & 2048) && Pe(T, B, N, N[11], _ ? Se(B, N[11], Y, Os) : De(N[11]), Tn) : P && P.p && (!_ || Y & 32) && P.p(N, _ ? Y : -1), (!_ || Y & 64) && h(f, "bx--visually-hidden", N[6]), R ? R.p && (!_ || Y & 2048) && Pe(R, O, N, N[11], _ ? Se(O, N[11], Y, qs) : De(N[11]), wn) : U && U.p && (!_ || Y & 8) && U.p(N, _ ? Y : -1), L ? L.p && (!_ || Y & 2048) && Pe(L, q, N, N[11], _ ? Se(q, N[11], Y, Us) : De(N[11]), pn) : C && C.p && (!_ || Y & 16) && C.p(N, _ ? Y : -1), (!_ || Y & 64 && b !== (b = N[6] && "margin-top: 0")) && z(o, "style", b), (!_ || Y & 1056 && d !== (d = N[5] ? void 0 : N[10]["aria-label"] || "Toggle")) && z(l, "aria-label", d), (!_ || Y & 128) && z(l, "for", N[7]), ve(e, j = pe(ne, [Y & 512 && N[9], (!_ || Y & 512 && g !== (g = N[9].style + "; user-select: none")) && {
                 style: g
             }])), h(e, "bx--form-item", !0)
         },
         i(N) {
-            _ || (v(D, N), v(U, N), v(C, N), _ = !0)
+            _ || (v(P, N), v(U, N), v(C, N), _ = !0)
         },
         o(N) {
-            A(D, N), A(U, N), A(C, N), _ = !1
+            A(P, N), A(U, N), A(C, N), _ = !1
         },
         d(N) {
-            N && E(e), D && D.d(N), U && U.d(N), C && C.d(N), k = !1, Le(w)
+            N && E(e), P && P.d(N), U && U.d(N), C && C.d(N), k = !1, Le(w)
         }
     }
 }
 
 function Js(i, e, t) {
     const n = ["size", "toggled", "disabled", "labelA", "labelB", "labelText", "hideLabel", "id", "name"];
     let l = ie(e, n),
@@ -8407,15 +8413,15 @@
         J.call(this, i, j)
     }
 
     function T(j) {
         J.call(this, i, j)
     }
 
-    function D(j) {
+    function P(j) {
         J.call(this, i, j)
     }
 
     function O(j) {
         J.call(this, i, j)
     }
 
@@ -8442,15 +8448,15 @@
         };
     return i.$$set = j => {
         t(10, e = Z(Z({}, e), ce(j))), t(9, l = ie(e, n)), "size" in j && t(1, o = j.size), "toggled" in j && t(0, s = j.toggled), "disabled" in j && t(2, u = j.disabled), "labelA" in j && t(3, a = j.labelA), "labelB" in j && t(4, b = j.labelB), "labelText" in j && t(5, d = j.labelText), "hideLabel" in j && t(6, g = j.hideLabel), "id" in j && t(7, _ = j.id), "name" in j && t(8, k = j.name), "$$scope" in j && t(11, r = j.$$scope)
     }, i.$$.update = () => {
         i.$$.dirty & 1 && w("toggle", {
             toggled: s
         })
-    }, e = ce(e), [s, o, u, a, b, d, g, _, k, l, e, r, f, B, T, D, O, R, U, q, L, C, ne]
+    }, e = ce(e), [s, o, u, a, b, d, g, _, k, l, e, r, f, B, T, P, O, R, U, q, L, C, ne]
 }
 class js extends ge {
     constructor(e) {
         super(), be(this, e, Js, Ws, _e, {
             size: 1,
             toggled: 0,
             disabled: 2,
@@ -9304,15 +9310,15 @@
     }
 }
 
 function Mu(i) {
     let e, t, n, l, f, r, o, s, u, a, b, d = i[11] && En(),
         g = !i[11] && i[13] && In();
 
-    function _(T, D) {
+    function _(T, P) {
         return T[22] ? wu : pu
     }
     let k = _(i),
         w = k(i);
     r = new hu({
         props: {
             translateWithId: i[18],
@@ -9320,25 +9326,25 @@
         }
     }), r.$on("click", i[30]);
     let B = i[1] && Ln(i);
     return {
         c() {
             d && d.c(), e = $(), g && g.c(), t = $(), n = V("button"), l = V("span"), w.c(), f = $(), X(r.$$.fragment), o = $(), B && B.c(), s = He(), h(l, "bx--list-box__label", !0), z(n, "type", "button"), z(n, "tabindex", "0"), z(n, "aria-expanded", i[1]), n.disabled = i[9], z(n, "translatewithid", i[18]), z(n, "id", i[19]), h(n, "bx--list-box__field", !0)
         },
-        m(T, D) {
-            d && d.m(T, D), I(T, e, D), g && g.m(T, D), I(T, t, D), I(T, n, D), M(n, l), w.m(l, null), M(n, f), G(r, n, null), i[31](n), I(T, o, D), B && B.m(T, D), I(T, s, D), u = !0, a || (b = [W(n, "keydown", i[32]), W(n, "keyup", i[33])], a = !0)
+        m(T, P) {
+            d && d.m(T, P), I(T, e, P), g && g.m(T, P), I(T, t, P), I(T, n, P), M(n, l), w.m(l, null), M(n, f), G(r, n, null), i[31](n), I(T, o, P), B && B.m(T, P), I(T, s, P), u = !0, a || (b = [W(n, "keydown", i[32]), W(n, "keyup", i[33])], a = !0)
         },
-        p(T, D) {
-            T[11] ? d ? D[0] & 2048 && v(d, 1) : (d = En(), d.c(), v(d, 1), d.m(e.parentNode, e)) : d && (de(), A(d, 1, 1, () => {
+        p(T, P) {
+            T[11] ? d ? P[0] & 2048 && v(d, 1) : (d = En(), d.c(), v(d, 1), d.m(e.parentNode, e)) : d && (de(), A(d, 1, 1, () => {
                 d = null
-            }), me()), !T[11] && T[13] ? g ? D[0] & 10240 && v(g, 1) : (g = In(), g.c(), v(g, 1), g.m(t.parentNode, t)) : g && (de(), A(g, 1, 1, () => {
+            }), me()), !T[11] && T[13] ? g ? P[0] & 10240 && v(g, 1) : (g = In(), g.c(), v(g, 1), g.m(t.parentNode, t)) : g && (de(), A(g, 1, 1, () => {
                 g = null
-            }), me()), k === (k = _(T)) && w ? w.p(T, D) : (w.d(1), w = k(T), w && (w.c(), w.m(l, null)));
+            }), me()), k === (k = _(T)) && w ? w.p(T, P) : (w.d(1), w = k(T), w && (w.c(), w.m(l, null)));
             const O = {};
-            D[0] & 262144 && (O.translateWithId = T[18]), D[0] & 2 && (O.open = T[1]), r.$set(O), (!u || D[0] & 2) && z(n, "aria-expanded", T[1]), (!u || D[0] & 512) && (n.disabled = T[9]), (!u || D[0] & 262144) && z(n, "translatewithid", T[18]), (!u || D[0] & 524288) && z(n, "id", T[19]), T[1] ? B ? (B.p(T, D), D[0] & 2 && v(B, 1)) : (B = Ln(T), B.c(), v(B, 1), B.m(s.parentNode, s)) : B && (de(), A(B, 1, 1, () => {
+            P[0] & 262144 && (O.translateWithId = T[18]), P[0] & 2 && (O.open = T[1]), r.$set(O), (!u || P[0] & 2) && z(n, "aria-expanded", T[1]), (!u || P[0] & 512) && (n.disabled = T[9]), (!u || P[0] & 262144) && z(n, "translatewithid", T[18]), (!u || P[0] & 524288) && z(n, "id", T[19]), T[1] ? B ? (B.p(T, P), P[0] & 2 && v(B, 1)) : (B = Ln(T), B.c(), v(B, 1), B.m(s.parentNode, s)) : B && (de(), A(B, 1, 1, () => {
                 B = null
             }), me())
         },
         i(T) {
             u || (v(d), v(g), v(r.$$.fragment, T), v(B), u = !0)
         },
         o(T) {
@@ -9373,18 +9379,18 @@
     n = new iu({
         props: {
             role: void 0,
             type: i[5],
             size: i[7],
             name: i[20],
             "aria-label": i[28]["aria-label"],
-            class: `bx--dropdown
-      ` + (i[6] === "top" && "bx--list-box--up") + `
-      ` + (i[11] && "bx--dropdown--invalid") + `
-      ` + (!i[11] && i[13] && "bx--dropdown--warning") + `
+            class: `bx--dropdown 
+      ` + (i[6] === "top" && "bx--list-box--up") + ` 
+      ` + (i[11] && "bx--dropdown--invalid") + ` 
+      ` + (!i[11] && i[13] && "bx--dropdown--warning") + ` 
       ` + (i[1] && "bx--dropdown--open") + `
       ` + (i[7] === "sm" && "bx--dropdown--sm") + `
       ` + (i[7] === "xl" && "bx--dropdown--xl") + `
       ` + (i[23] && "bx--dropdown--inline") + `
       ` + (i[9] && "bx--dropdown--disabled") + `
       ` + (i[8] && "bx--dropdown--light"),
             disabled: i[9],
@@ -9412,18 +9418,18 @@
         },
         m(d, g) {
             I(d, e, g), s && s.m(e, null), M(e, t), G(n, e, null), M(e, l), u && u.m(e, null), f = !0, r || (o = W(window, "click", i[26]), r = !0)
         },
         p(d, g) {
             d[10] ? s ? s.p(d, g) : (s = Cn(d), s.c(), s.m(e, t)) : s && (s.d(1), s = null);
             const _ = {};
-            g[0] & 32 && (_.type = d[5]), g[0] & 128 && (_.size = d[7]), g[0] & 1048576 && (_.name = d[20]), g[0] & 268435456 && (_["aria-label"] = d[28]["aria-label"]), g[0] & 8399810 && (_.class = `bx--dropdown
-      ` + (d[6] === "top" && "bx--list-box--up") + `
-      ` + (d[11] && "bx--dropdown--invalid") + `
-      ` + (!d[11] && d[13] && "bx--dropdown--warning") + `
+            g[0] & 32 && (_.type = d[5]), g[0] & 128 && (_.size = d[7]), g[0] & 1048576 && (_.name = d[20]), g[0] & 268435456 && (_["aria-label"] = d[28]["aria-label"]), g[0] & 8399810 && (_.class = `bx--dropdown 
+      ` + (d[6] === "top" && "bx--list-box--up") + ` 
+      ` + (d[11] && "bx--dropdown--invalid") + ` 
+      ` + (!d[11] && d[13] && "bx--dropdown--warning") + ` 
       ` + (d[1] && "bx--dropdown--open") + `
       ` + (d[7] === "sm" && "bx--dropdown--sm") + `
       ` + (d[7] === "xl" && "bx--dropdown--xl") + `
       ` + (d[23] && "bx--dropdown--inline") + `
       ` + (d[9] && "bx--dropdown--disabled") + `
       ` + (d[8] && "bx--dropdown--light")), g[0] & 512 && (_.disabled = d[9]), g[0] & 2 && (_.open = d[1]), g[0] & 2048 && (_.invalid = d[11]), g[0] & 4096 && (_.invalidText = d[12]), g[0] & 256 && (_.light = d[8]), g[0] & 8192 && (_.warn = d[13]), g[0] & 16384 && (_.warnText = d[14]), g[0] & 7154207 | g[1] & 64 && (_.$$scope = {
                 dirty: g,
@@ -9477,15 +9483,15 @@
         {
             disabled: B = !1
         } = e,
         {
             titleText: T = ""
         } = e,
         {
-            invalid: D = !1
+            invalid: P = !1
         } = e,
         {
             invalidText: O = ""
         } = e,
         {
             warn: R = !1
         } = e,
@@ -9549,15 +9555,15 @@
     }
     const Te = le => {
             const {
                 key: Me
             } = le;
             ["Enter", "ArrowDown", "ArrowUp"].includes(Me) && le.preventDefault(), Me === "Enter" ? (t(1, k = !k), ke > -1 && u[ke].id !== b && (t(0, b = u[ke].id), F(), t(1, k = !1))) : Me === "Tab" ? (t(1, k = !1), Y.blur()) : Me === "ArrowDown" ? (k || t(1, k = !0), he(1)) : Me === "ArrowUp" ? (k || t(1, k = !0), he(-1)) : Me === "Escape" && t(1, k = !1)
         },
-        P = le => {
+        D = le => {
             const {
                 key: Me
             } = le;
             if ([" "].includes(Me)) le.preventDefault();
             else return;
             t(1, k = !k), ke > -1 && u[ke].id !== b && (t(0, b = u[ke].id), F(), t(1, k = !1))
         },
@@ -9573,18 +9579,18 @@
         },
         Ge = ({
             target: le
         }) => {
             B || t(1, k = Y.contains(le) ? !k : !1)
         };
     return i.$$set = le => {
-        t(28, e = Z(Z({}, e), ce(le))), t(27, r = ie(e, f)), "items" in le && t(3, u = le.items), "itemToString" in le && t(4, a = le.itemToString), "selectedId" in le && t(0, b = le.selectedId), "type" in le && t(5, d = le.type), "direction" in le && t(6, g = le.direction), "size" in le && t(7, _ = le.size), "open" in le && t(1, k = le.open), "light" in le && t(8, w = le.light), "disabled" in le && t(9, B = le.disabled), "titleText" in le && t(10, T = le.titleText), "invalid" in le && t(11, D = le.invalid), "invalidText" in le && t(12, O = le.invalidText), "warn" in le && t(13, R = le.warn), "warnText" in le && t(14, U = le.warnText), "helperText" in le && t(15, q = le.helperText), "label" in le && t(16, L = le.label), "hideLabel" in le && t(17, C = le.hideLabel), "translateWithId" in le && t(18, ne = le.translateWithId), "id" in le && t(19, j = le.id), "name" in le && t(20, N = le.name), "ref" in le && t(2, Y = le.ref), "$$scope" in le && t(37, s = le.$$scope)
+        t(28, e = Z(Z({}, e), ce(le))), t(27, r = ie(e, f)), "items" in le && t(3, u = le.items), "itemToString" in le && t(4, a = le.itemToString), "selectedId" in le && t(0, b = le.selectedId), "type" in le && t(5, d = le.type), "direction" in le && t(6, g = le.direction), "size" in le && t(7, _ = le.size), "open" in le && t(1, k = le.open), "light" in le && t(8, w = le.light), "disabled" in le && t(9, B = le.disabled), "titleText" in le && t(10, T = le.titleText), "invalid" in le && t(11, P = le.invalid), "invalidText" in le && t(12, O = le.invalidText), "warn" in le && t(13, R = le.warn), "warnText" in le && t(14, U = le.warnText), "helperText" in le && t(15, q = le.helperText), "label" in le && t(16, L = le.label), "hideLabel" in le && t(17, C = le.hideLabel), "translateWithId" in le && t(18, ne = le.translateWithId), "id" in le && t(19, j = le.id), "name" in le && t(20, N = le.name), "ref" in le && t(2, Y = le.ref), "$$scope" in le && t(37, s = le.$$scope)
     }, i.$$.update = () => {
         i.$$.dirty[0] & 32 && t(23, n = d === "inline"), i.$$.dirty[0] & 9 && t(22, l = u.find(le => le.id === b)), i.$$.dirty[0] & 2 && (k || t(21, ke = -1))
-    }, e = ce(e), [b, k, Y, u, a, d, g, _, w, B, T, D, O, R, U, q, L, C, ne, j, N, ke, l, n, he, F, x, r, e, o, Ce, Ee, Te, P, we, fe, Ge, s]
+    }, e = ce(e), [b, k, Y, u, a, d, g, _, w, B, T, P, O, R, U, q, L, C, ne, j, N, ke, l, n, he, F, x, r, e, o, Ce, Ee, Te, D, we, fe, Ge, s]
 }
 class Cu extends ge {
     constructor(e) {
         super(), be(this, e, Bu, zu, _e, {
             items: 3,
             itemToString: 4,
             selectedId: 0,
@@ -10240,15 +10246,15 @@
         d(n) {
             n && E(e)
         }
     }
 }
 
 function Ku(i) {
-    let e, t, n, l, f, r, o, s, u, a, b, d, g, _, k, w, B, T, D, O, R, U = i[18] && Un(i),
+    let e, t, n, l, f, r, o, s, u, a, b, d, g, _, k, w, B, T, P, O, R, U = i[18] && Un(i),
         q = !i[18] && (i[12] || i[25].labelText) && On(i),
         L = i[14] && Vn(),
         C = !i[14] && i[16] && Yn(),
         ne = [{
             "data-invalid": u = i[14] || void 0
         }, {
             "aria-invalid": a = i[14] || void 0
@@ -10275,52 +10281,52 @@
         ke = !i[14] && !i[16] && !i[24] && !i[18] && i[11] && Gn(i),
         he = !i[24] && !i[14] && i[16] && Kn(i);
     return {
         c() {
             e = V("div"), U && U.c(), t = $(), q && q.c(), n = $(), l = V("div"), f = V("div"), L && L.c(), r = $(), C && C.c(), o = $(), s = V("input"), g = $(), N && N.c(), _ = $(), Y && Y.c(), w = $(), se && se.c(), B = $(), ke && ke.c(), T = $(), he && he.c(), ve(s, j), h(s, "bx--text-input", !0), h(s, "bx--password-input", !0), h(s, "bx--text-input--light", i[9]), h(s, "bx--text-input--invalid", i[14]), h(s, "bx--text-input--warning", i[16]), h(s, "bx--text-input--sm", i[3] === "sm"), h(s, "bx--text-input--xl", i[3] === "xl"), z(f, "data-invalid", k = i[14] || void 0), h(f, "bx--text-input__field-wrapper", !0), h(f, "bx--text-input__field-wrapper--warning", i[16]), h(l, "bx--text-input__field-outer-wrapper", !0), h(l, "bx--text-input__field-outer-wrapper--inline", i[18]), h(e, "bx--form-item", !0), h(e, "bx--text-input-wrapper", !0), h(e, "bx--password-input-wrapper", !i[24]), h(e, "bx--text-input-wrapper--light", i[9]), h(e, "bx--text-input-wrapper--inline", i[18])
         },
         m(F, x) {
-            I(F, e, x), U && U.m(e, null), M(e, t), q && q.m(e, null), M(e, n), M(e, l), M(l, f), L && L.m(f, null), M(f, r), C && C.m(f, null), M(f, o), M(f, s), "value" in j && (s.value = j.value), s.autofocus && s.focus(), i[40](s), M(f, g), N && N.m(f, null), M(f, _), Y && Y.m(f, null), M(l, w), se && se.m(l, null), M(l, B), ke && ke.m(l, null), M(l, T), he && he.m(l, null), D = !0, O || (R = [W(s, "change", i[33]), W(s, "input", i[34]), W(s, "input", i[41]), W(s, "keydown", i[35]), W(s, "keyup", i[36]), W(s, "focus", i[37]), W(s, "blur", i[38]), W(s, "paste", i[39]), W(e, "click", i[29]), W(e, "mouseover", i[30]), W(e, "mouseenter", i[31]), W(e, "mouseleave", i[32])], O = !0)
+            I(F, e, x), U && U.m(e, null), M(e, t), q && q.m(e, null), M(e, n), M(e, l), M(l, f), L && L.m(f, null), M(f, r), C && C.m(f, null), M(f, o), M(f, s), "value" in j && (s.value = j.value), s.autofocus && s.focus(), i[40](s), M(f, g), N && N.m(f, null), M(f, _), Y && Y.m(f, null), M(l, w), se && se.m(l, null), M(l, B), ke && ke.m(l, null), M(l, T), he && he.m(l, null), P = !0, O || (R = [W(s, "change", i[33]), W(s, "input", i[34]), W(s, "input", i[41]), W(s, "keydown", i[35]), W(s, "keyup", i[36]), W(s, "focus", i[37]), W(s, "blur", i[38]), W(s, "paste", i[39]), W(e, "click", i[29]), W(e, "mouseover", i[30]), W(e, "mouseenter", i[31]), W(e, "mouseleave", i[32])], O = !0)
         },
         p(F, x) {
             F[18] ? U ? (U.p(F, x), x[0] & 262144 && v(U, 1)) : (U = Un(F), U.c(), v(U, 1), U.m(e, t)) : U && (de(), A(U, 1, 1, () => {
                 U = null
             }), me()), !F[18] && (F[12] || F[25].labelText) ? q ? (q.p(F, x), x[0] & 33820672 && v(q, 1)) : (q = On(F), q.c(), v(q, 1), q.m(e, n)) : q && (de(), A(q, 1, 1, () => {
                 q = null
             }), me()), F[14] ? L ? x[0] & 16384 && v(L, 1) : (L = Vn(), L.c(), v(L, 1), L.m(f, r)) : L && (de(), A(L, 1, 1, () => {
                 L = null
             }), me()), !F[14] && F[16] ? C ? x[0] & 81920 && v(C, 1) : (C = Yn(), C.c(), v(C, 1), C.m(f, o)) : C && (de(), A(C, 1, 1, () => {
                 C = null
-            }), me()), ve(s, j = pe(ne, [(!D || x[0] & 16384 && u !== (u = F[14] || void 0)) && {
+            }), me()), ve(s, j = pe(ne, [(!P || x[0] & 16384 && u !== (u = F[14] || void 0)) && {
                 "data-invalid": u
-            }, (!D || x[0] & 16384 && a !== (a = F[14] || void 0)) && {
+            }, (!P || x[0] & 16384 && a !== (a = F[14] || void 0)) && {
                 "aria-invalid": a
-            }, (!D || x[0] & 14764032 && b !== (b = F[14] ? F[22] : F[16] ? F[21] : F[11] ? F[23] : void 0)) && {
+            }, (!P || x[0] & 14764032 && b !== (b = F[14] ? F[22] : F[16] ? F[21] : F[11] ? F[23] : void 0)) && {
                 "aria-describedby": b
-            }, (!D || x[0] & 524288) && {
+            }, (!P || x[0] & 524288) && {
                 id: F[19]
-            }, (!D || x[0] & 1048576) && {
+            }, (!P || x[0] & 1048576) && {
                 name: F[20]
-            }, (!D || x[0] & 16) && {
+            }, (!P || x[0] & 16) && {
                 placeholder: F[4]
-            }, (!D || x[0] & 2) && {
+            }, (!P || x[0] & 2) && {
                 type: F[1]
-            }, (!D || x[0] & 1 && d !== (d = F[0] ?? "") && s.value !== d) && {
+            }, (!P || x[0] & 1 && d !== (d = F[0] ?? "") && s.value !== d) && {
                 value: d
-            }, (!D || x[0] & 1024) && {
+            }, (!P || x[0] & 1024) && {
                 disabled: F[10]
             }, x[0] & 67108864 && F[26]])), "value" in j && (s.value = j.value), h(s, "bx--text-input", !0), h(s, "bx--password-input", !0), h(s, "bx--text-input--light", F[9]), h(s, "bx--text-input--invalid", F[14]), h(s, "bx--text-input--warning", F[16]), h(s, "bx--text-input--sm", F[3] === "sm"), h(s, "bx--text-input--xl", F[3] === "xl"), F[24] && F[14] ? N ? N.p(F, x) : (N = Zn(F), N.c(), N.m(f, _)) : N && (N.d(1), N = null), F[24] && F[14] ? Y && (de(), A(Y, 1, 1, () => {
                 Y = null
-            }), me()) : Y ? (Y.p(F, x), x[0] & 16793600 && v(Y, 1)) : (Y = Wn(F), Y.c(), v(Y, 1), Y.m(f, null)), (!D || x[0] & 16384 && k !== (k = F[14] || void 0)) && z(f, "data-invalid", k), (!D || x[0] & 65536) && h(f, "bx--text-input__field-wrapper--warning", F[16]), !F[24] && F[14] ? se ? se.p(F, x) : (se = jn(F), se.c(), se.m(l, B)) : se && (se.d(1), se = null), !F[14] && !F[16] && !F[24] && !F[18] && F[11] ? ke ? ke.p(F, x) : (ke = Gn(F), ke.c(), ke.m(l, T)) : ke && (ke.d(1), ke = null), !F[24] && !F[14] && F[16] ? he ? he.p(F, x) : (he = Kn(F), he.c(), he.m(l, null)) : he && (he.d(1), he = null), (!D || x[0] & 262144) && h(l, "bx--text-input__field-outer-wrapper--inline", F[18]), (!D || x[0] & 16777216) && h(e, "bx--password-input-wrapper", !F[24]), (!D || x[0] & 512) && h(e, "bx--text-input-wrapper--light", F[9]), (!D || x[0] & 262144) && h(e, "bx--text-input-wrapper--inline", F[18])
+            }), me()) : Y ? (Y.p(F, x), x[0] & 16793600 && v(Y, 1)) : (Y = Wn(F), Y.c(), v(Y, 1), Y.m(f, null)), (!P || x[0] & 16384 && k !== (k = F[14] || void 0)) && z(f, "data-invalid", k), (!P || x[0] & 65536) && h(f, "bx--text-input__field-wrapper--warning", F[16]), !F[24] && F[14] ? se ? se.p(F, x) : (se = jn(F), se.c(), se.m(l, B)) : se && (se.d(1), se = null), !F[14] && !F[16] && !F[24] && !F[18] && F[11] ? ke ? ke.p(F, x) : (ke = Gn(F), ke.c(), ke.m(l, T)) : ke && (ke.d(1), ke = null), !F[24] && !F[14] && F[16] ? he ? he.p(F, x) : (he = Kn(F), he.c(), he.m(l, null)) : he && (he.d(1), he = null), (!P || x[0] & 262144) && h(l, "bx--text-input__field-outer-wrapper--inline", F[18]), (!P || x[0] & 16777216) && h(e, "bx--password-input-wrapper", !F[24]), (!P || x[0] & 512) && h(e, "bx--text-input-wrapper--light", F[9]), (!P || x[0] & 262144) && h(e, "bx--text-input-wrapper--inline", F[18])
         },
         i(F) {
-            D || (v(U), v(q), v(L), v(C), v(Y), D = !0)
+            P || (v(U), v(q), v(L), v(C), v(Y), P = !0)
         },
         o(F) {
-            A(U), A(q), A(L), A(C), A(Y), D = !1
+            A(U), A(q), A(L), A(C), A(Y), P = !1
         },
         d(F) {
             F && E(e), U && U.d(), q && q.d(), L && L.d(), C && C.d(), i[40](null), N && N.d(), Y && Y.d(), se && se.d(), ke && ke.d(), he && he.d(), O = !1, Le(R)
         }
     }
 }
 
@@ -10344,15 +10350,15 @@
     } = e, {
         hidePasswordLabel: w = "Hide password"
     } = e, {
         showPasswordLabel: B = "Show password"
     } = e, {
         tooltipAlignment: T = "center"
     } = e, {
-        tooltipPosition: D = "bottom"
+        tooltipPosition: P = "bottom"
     } = e, {
         light: O = !1
     } = e, {
         disabled: R = !1
     } = e, {
         helperText: U = ""
     } = e, {
@@ -10390,15 +10396,15 @@
         J.call(this, i, re)
     }
 
     function Te(re) {
         J.call(this, i, re)
     }
 
-    function P(re) {
+    function D(re) {
         J.call(this, i, re)
     }
 
     function we(re) {
         J.call(this, i, re)
     }
 
@@ -10432,18 +10438,18 @@
         }) => {
             t(0, g = re.value)
         },
         ue = () => {
             t(1, _ = _ === "password" ? "text" : "password")
         };
     return i.$$set = re => {
-        e = Z(Z({}, e), ce(re)), t(26, s = ie(e, o)), "size" in re && t(3, d = re.size), "value" in re && t(0, g = re.value), "type" in re && t(1, _ = re.type), "placeholder" in re && t(4, k = re.placeholder), "hidePasswordLabel" in re && t(5, w = re.hidePasswordLabel), "showPasswordLabel" in re && t(6, B = re.showPasswordLabel), "tooltipAlignment" in re && t(7, T = re.tooltipAlignment), "tooltipPosition" in re && t(8, D = re.tooltipPosition), "light" in re && t(9, O = re.light), "disabled" in re && t(10, R = re.disabled), "helperText" in re && t(11, U = re.helperText), "labelText" in re && t(12, q = re.labelText), "hideLabel" in re && t(13, L = re.hideLabel), "invalid" in re && t(14, C = re.invalid), "invalidText" in re && t(15, ne = re.invalidText), "warn" in re && t(16, j = re.warn), "warnText" in re && t(17, N = re.warnText), "inline" in re && t(18, Y = re.inline), "id" in re && t(19, se = re.id), "name" in re && t(20, ke = re.name), "ref" in re && t(2, he = re.ref), "$$scope" in re && t(27, a = re.$$scope)
+        e = Z(Z({}, e), ce(re)), t(26, s = ie(e, o)), "size" in re && t(3, d = re.size), "value" in re && t(0, g = re.value), "type" in re && t(1, _ = re.type), "placeholder" in re && t(4, k = re.placeholder), "hidePasswordLabel" in re && t(5, w = re.hidePasswordLabel), "showPasswordLabel" in re && t(6, B = re.showPasswordLabel), "tooltipAlignment" in re && t(7, T = re.tooltipAlignment), "tooltipPosition" in re && t(8, P = re.tooltipPosition), "light" in re && t(9, O = re.light), "disabled" in re && t(10, R = re.disabled), "helperText" in re && t(11, U = re.helperText), "labelText" in re && t(12, q = re.labelText), "hideLabel" in re && t(13, L = re.hideLabel), "invalid" in re && t(14, C = re.invalid), "invalidText" in re && t(15, ne = re.invalidText), "warn" in re && t(16, j = re.warn), "warnText" in re && t(17, N = re.warnText), "inline" in re && t(18, Y = re.inline), "id" in re && t(19, se = re.id), "name" in re && t(20, ke = re.name), "ref" in re && t(2, he = re.ref), "$$scope" in re && t(27, a = re.$$scope)
     }, i.$$.update = () => {
         i.$$.dirty[0] & 524288 && t(23, l = `helper-${se}`), i.$$.dirty[0] & 524288 && t(22, f = `error-${se}`), i.$$.dirty[0] & 524288 && t(21, r = `warn-${se}`)
-    }, t(24, n = !!F && F.isFluid), [g, _, he, d, k, w, B, T, D, O, R, U, q, L, C, ne, j, N, Y, se, ke, r, f, l, n, b, s, a, u, x, Ce, Ee, Te, P, we, fe, Ge, le, Me, Ye, ot, ft, ue]
+    }, t(24, n = !!F && F.isFluid), [g, _, he, d, k, w, B, T, P, O, R, U, q, L, C, ne, j, N, Y, se, ke, r, f, l, n, b, s, a, u, x, Ce, Ee, Te, D, we, fe, Ge, le, Me, Ye, ot, ft, ue]
 }
 class Qu extends ge {
     constructor(e) {
         super(), be(this, e, Xu, Ku, _e, {
             size: 3,
             value: 0,
             type: 1,
@@ -11404,16 +11410,16 @@
         },
         p(k, w) {
             i = k;
             const B = {};
             w & 1 && (B.value = i[25]), n.$set(B);
             const T = {};
             w & 1 && (T.disabled = i[5] === i[25]), r.$set(T);
-            const D = {};
-            w & 1 && (D.disabled = i[5] === i[25] || i[25] === "default"), s.$set(D), (!b || w & 1 && a !== (a = "profile-item " + (i[5] === i[25] ? "current" : "") + " svelte-1x82mf0")) && z(e, "class", a)
+            const P = {};
+            w & 1 && (P.disabled = i[5] === i[25] || i[25] === "default"), s.$set(P), (!b || w & 1 && a !== (a = "profile-item " + (i[5] === i[25] ? "current" : "") + " svelte-1x82mf0")) && z(e, "class", a)
         },
         i(k) {
             b || (v(n.$$.fragment, k), v(r.$$.fragment, k), v(s.$$.fragment, k), b = !0)
         },
         o(k) {
             A(n.$$.fragment, k), A(r.$$.fragment, k), A(s.$$.fragment, k), b = !1
         },
@@ -11559,15 +11565,15 @@
             t(4, u.kind = void 0, u)
         };
 
     function T(C) {
         o = C, t(2, o)
     }
 
-    function D(C) {
+    function P(C) {
         s = C, t(3, s)
     }
     const O = () => {
             t(1, r = null), t(4, u.kind = void 0, u)
         },
         R = () => {
             a(r)
@@ -11575,15 +11581,15 @@
         U = async C => {
             await b(C), t(1, r = C)
         }, q = C => a(C), L = C => {
             d(C)
         };
     return i.$$set = C => {
         "profiles" in C && t(0, l = C.profiles)
-    }, [l, r, o, s, u, f, a, b, d, g, _, k, w, B, T, D, O, R, U, q, L]
+    }, [l, r, o, s, u, f, a, b, d, g, _, k, w, B, T, P, O, R, U, q, L]
 }
 class ya extends ge {
     constructor(e) {
         super(), be(this, e, Ta, wa, _e, {
             profiles: 0
         })
     }
@@ -12125,17 +12131,17 @@
                 default: [Ea]
             },
             $$scope: {
                 ctx: i
             }
         }
     }), n.$on("click", i[10]);
-    let D = i[0],
+    let P = i[0],
         O = [];
-    for (let q = 0; q < D.length; q += 1) O[q] = sl(fl(i, D, q));
+    for (let q = 0; q < P.length; q += 1) O[q] = sl(fl(i, P, q));
     const R = q => A(O[q], 1, 1, () => {
         O[q] = null
     });
     let U = ul(i);
     return k = new ho({
         props: {
             $$slots: {
@@ -12158,34 +12164,34 @@
         },
         p(q, [L]) {
             const C = {};
             if (L & 8388608 && (C.$$scope = {
                     dirty: L,
                     ctx: q
                 }), n.$set(C), L & 25) {
-                D = q[0];
+                P = q[0];
                 let j;
-                for (j = 0; j < D.length; j += 1) {
-                    const N = fl(q, D, j);
+                for (j = 0; j < P.length; j += 1) {
+                    const N = fl(q, P, j);
                     O[j] ? (O[j].p(N, L), v(O[j], 1)) : (O[j] = sl(N), O[j].c(), v(O[j], 1), O[j].m(f, null))
                 }
-                for (de(), j = D.length; j < O.length; j += 1) R(j);
+                for (de(), j = P.length; j < O.length; j += 1) R(j);
                 me()
             }
             L & 8 && _e(a, a = q[3]) ? (de(), A(U, 1, 1, ee), me(), U = ul(q), U.c(), v(U, 1), U.m(u, null)) : U.p(q, L);
             const ne = {};
             L & 8388614 && (ne.$$scope = {
                 dirty: L,
                 ctx: q
             }), k.$set(ne)
         },
         i(q) {
             if (!w) {
                 v(n.$$.fragment, q);
-                for (let L = 0; L < D.length; L += 1) v(O[L]);
+                for (let L = 0; L < P.length; L += 1) v(O[L]);
                 v(U), v(k.$$.fragment, q), w = !0
             }
         },
         o(q) {
             A(n.$$.fragment, q), O = O.filter(Boolean);
             for (let L = 0; L < O.length; L += 1) A(O[L]);
             A(U), A(k.$$.fragment, q), w = !1
@@ -12239,15 +12245,15 @@
         nt.set(null), w.focus()
     };
 
     function T(q) {
         l = q, t(0, l)
     }
 
-    function D(q) {
+    function P(q) {
         w = q, t(5, w)
     }
 
     function O(q) {
         l = q, t(0, l)
     }
 
@@ -12256,15 +12262,15 @@
     }
 
     function U(q) {
         f = q, t(1, f)
     }
     return i.$$set = q => {
         "histories" in q && t(0, l = q.histories), "profiles" in q && t(1, f = q.profiles), "ingestable" in q && t(2, r = q.ingestable)
-    }, [l, f, r, o, b, w, d, g, _, k, B, T, D, O, R, U]
+    }, [l, f, r, o, b, w, d, g, _, k, B, T, P, O, R, U]
 }
 class Ua extends ge {
     constructor(e) {
         super(), be(this, e, Ra, Ha, _e, {
             histories: 0,
             profiles: 1,
             ingestable: 2
@@ -12316,15 +12322,15 @@
         props: {
             histories: i[0],
             profiles: i[1],
             ingestable: i[2]
         }
     }), {
         c() {
-            e = V("div"), t = V("header"), n = V("div"), n.innerHTML = `<h1 class="svelte-1uoml83"><img alt="favicon" src="./assets/favicon.png" class="svelte-1uoml83"/>
+            e = V("div"), t = V("header"), n = V("div"), n.innerHTML = `<h1 class="svelte-1uoml83"><img alt="favicon" src="./assets/favicon.png" class="svelte-1uoml83"/> 
                 <div>-GPT: Your personal, powerful and private GPT</div></h1>`, l = $(), f = V("div"), X(r.$$.fragment), o = $(), s = V("main"), X(u.$$.fragment), z(n, "class", "logo"), z(f, "class", "social"), z(t, "class", "svelte-1uoml83"), z(s, "class", "svelte-1uoml83"), z(e, "id", "main"), z(e, "class", "svelte-1uoml83")
         },
         m(b, d) {
             I(b, e, d), M(e, t), M(t, n), M(t, l), M(t, f), G(r, f, null), M(e, o), M(e, s), G(u, s, null), a = !0
         },
         p(b, [d]) {
             const g = {};
```

### Comparing `pxgpt-0.0.0rc0/pxgpt/logger.py` & `pxgpt-0.0.0rc1/pxgpt/logger.py`

 * *Files identical despite different names*

### Comparing `pxgpt-0.0.0rc0/pxgpt/manager.py` & `pxgpt-0.0.0rc1/pxgpt/manager.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,20 @@
 
 class Manager:
     """The ring manager
 
     Manages the rings and histories.
     """
 
-    def __init__(self, profile: str, serving: bool = False):
+    def __init__(
+        self,
+        profile: str,
+        serving: bool = False,
+        debug: bool = False,
+    ):
         """Initialize the manager
 
         Args:
             profile: The profile
             serving: Whether the manager is used for serving
                 Primarily used for determining whether to initialize the LLMs
                 for those rings that do not support async. Since we don't need
@@ -40,21 +45,21 @@
 
         self.config = FrozenDiot(ProfileConfig.detach(config))
         self.profile = profile
         self.logger = get_logger(self.config.log_level)
         if old_profile != profile:
             self.logger.info("Switched profile to %s", profile)
 
-        self.ring = self._create_ring(serving)
+        self.ring = self._create_ring(serving, debug)
 
     def close(self):
         """Close the manager"""
         del self.ring
 
-    def _create_ring(self, serving: bool):
+    def _create_ring(self, serving: bool, debug: bool):
         """Create the ring"""
         # Avoid changes to the config
         model_type = self.config.model.type
 
         def should_init_llm(ring_class):
             return not serving or not issubclass(
                 ring_class, NoAsyncSupportRing
@@ -63,36 +68,42 @@
         if model_type == "GPT4All":
             from .rings.gpt4all import GPT4AllRing
 
             return GPT4AllRing(
                 self.config,
                 self.profile,
                 init_llm=should_init_llm(GPT4AllRing),
+                debug=debug,
             )
         if model_type == "LlamaCpp":
             from .rings.llamacpp import LlamaCppRing
 
             return LlamaCppRing(
                 self.config,
                 self.profile,
                 init_llm=should_init_llm(LlamaCppRing),
+                debug=debug,
             )
         if model_type == "OpenAI":
             from .rings.openai import OpenAIRing
 
             return OpenAIRing(
-                self.config, self.profile, init_llm=should_init_llm(OpenAIRing)
+                self.config,
+                self.profile,
+                init_llm=should_init_llm(OpenAIRing),
+                debug=debug,
             )
         if model_type == "ChatOpenAI":
             from .rings.chatopenai import ChatOpenAIRing
 
             return ChatOpenAIRing(
                 self.config,
                 self.profile,
                 init_llm=should_init_llm(ChatOpenAIRing),
+                debug=debug,
             )
         else:
             raise ValueError(f"Unknown ring: {model_type}")
 
     def get_docs(self) -> Mapping[str, List[Mapping[str, str]]]:
         """Get the documents"""
         return self.ring.get_docs()
```

### Comparing `pxgpt-0.0.0rc0/pxgpt/rings/_callbacks.py` & `pxgpt-0.0.0rc1/pxgpt/rings/_callbacks.py`

 * *Files identical despite different names*

### Comparing `pxgpt-0.0.0rc0/pxgpt/rings/_llms.py` & `pxgpt-0.0.0rc1/pxgpt/rings/_llms.py`

 * *Files identical despite different names*

### Comparing `pxgpt-0.0.0rc0/pxgpt/rings/_mixins.py` & `pxgpt-0.0.0rc1/pxgpt/rings/_mixins.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 from abc import ABC
 from functools import cached_property
 from multiprocessing import Pool
 from pathlib import Path
 from typing import TYPE_CHECKING, List, Mapping
 
-from chromadb.config import Settings
 from langchain.document_loaders import (
     CSVLoader,
     EverNoteLoader,
     PyMuPDFLoader,
     TextLoader,
     UnstructuredEmailLoader,
     UnstructuredEPubLoader,
@@ -132,14 +131,16 @@
     @property
     def embeddings(self) -> Embeddings:
         """The embeddings"""
         raise NotImplementedError
 
     def db(self, texts: List[Document] | None = None) -> Chroma:
         """Get the database"""
+        from chromadb.config import Settings
+
         settings = Settings(
             chroma_db_impl=self.config.ingest.chroma_db_impl,
             persist_directory=self.persist_directory,
             anonymized_telemetry=self.config.ingest.chroma_anonymized_telemetry,
         )
         if texts is None:
             return Chroma(
```

### Comparing `pxgpt-0.0.0rc0/pxgpt/rings/base.py` & `pxgpt-0.0.0rc1/pxgpt/rings/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -55,23 +55,67 @@
         config: A Diot object that contains all the configuration
         logger: A logger object
         init_llm: Whether to initialize the LLMs in the constructor
     """
 
     MODEL: LLM | None = None
 
+    CHAT_PROMPT = textwrap.dedent(
+        """
+        As a language model, your task is to respond to any questions asked --
+        in a concise and truthful manner.
+        Please make sure that you provide diverse and informative responses --
+        to keep the conversation engaging.
+        Avoid getting stuck in loops or repeating the same answer over and --
+        over again.
+        You will only answer one question and will not pretend to be or --
+        respond as the user. Do not return more than one response at a time.
+        DO NOT RESPOND AS THE USER!
+        LM should only respond as LM.
+
+        Previous conversation:
+        {history}
+
+        Current conversation:
+        Human: {input}
+        AI:
+        """
+    ).strip().replace("--\n", "")
+
+    QC_PROMPT = textwrap.dedent(
+        """
+        Given the following conversation and a follow up question, --
+        rephrase the follow up question to be a standalone question, --
+        in its original language.
+        The new question should be grammatically correct and semantically --
+        similar to the original question.
+        If the chat history is not enough, you can keep the original question --
+        as is.
+
+        Chat History:
+        {chat_history}
+
+        Follow Up Input: {question}
+        Standalone Question:
+        """
+    ).strip().replace("--\n", "")
+
+    RETRIEVAL_PROMPT = None
+
     def __init__(
         self,
         config: Diot,
         profile: str,
         init_llm: bool = True,
+        debug: bool = False,
     ) -> None:
         """Initialize the ring"""
         self.config = config
         self.profile = profile
+        self.debug = debug
         self.logger = get_logger(config.log_level)
 
         if init_llm:
             self.llm = self._create_llm()
             self.qllm = self._create_qllm()
         else:
             self.llm = None
@@ -82,15 +126,15 @@
         else:
             self.logger.info("Entering chat mode")
 
     @property
     def model_args(self):
         """Get the model arg that will be passed to the model"""
         args = {k: v for k, v in self.config.model.items() if k != "type"}
-        args.update({"streaming": True, "verbose": False})
+        args.update({"streaming": True, "verbose": self.debug})
         return args
 
     @property
     def qmodel(self) -> Type[LLM]:
         """Get the qmodel class
 
         When qmodel is not found in config, then class of model will be used.
@@ -180,74 +224,57 @@
     def _create_chat_chain(self) -> Chain:
         """Create the chat chain object for chatting only, without documents
 
         A ConversationChain object is created.
         Custom rings can override this method to create a different chain.
         """
         self.logger.debug("Creating chat chain")
-        prompt_template = textwrap.dedent(
-            """
-            The following is a friendly conversation between a human and an AI.
-            The AI is talkative and provides lots of specific details from its
-            context. If the AI does not know the answer to a question,
-            it truthfully says it does not know. After answering a question,
-            the AI should NOT ask follow-up questions, followed by the "Human:"
-            prefix.
-
-            Previous conversation:
-            {history}
-
-            Current conversation:
-            Human: {input}
-            AI:"""
-        ).lstrip()
-        prompt = PromptTemplate.from_template(prompt_template)
-        return ConversationChain(llm=self.llm, prompt=prompt)
+
+        prompt = PromptTemplate.from_template(self.CHAT_PROMPT)
+        return ConversationChain(
+            llm=self.llm,
+            prompt=prompt,
+            verbose=self.debug,
+        )
 
     def _create_retrieval_chain(self) -> Chain:
         """Create the retrieval chain object for document retrieval
 
         A ConversationalRetrievalChain object is created.
         Custom rings can override this method to create a different chain.
         If you want to use the default chain, you can choose to use a
         different question condenser, or even not to use one. Then you must
         be aware that the "qmodel" section in the config will be ignored.
         """
         self.logger.debug("Creating retrieval chain")
-        main_chain = load_qa_chain(self.llm, verbose=False)
-        cqp = textwrap.dedent(
-            """
-            Given the following conversation and a follow up question,
-            rephrase the follow up question to be a standalone question,
-            in its original language. The new question should be
-            grammatically correct and semantically similar to the original
-            question. If the chat history is not enough, you can keep the
-            original question as is.
-
-            Chat History:
-            {chat_history}
-
-            Follow Up Input: {question}
-            Standalone question:"""
-        ).lstrip()
+        if self.RETRIEVAL_PROMPT:
+            main_chain = load_qa_chain(
+                self.llm,
+                verbose=self.debug,
+                prompt=PromptTemplate.from_template(self.RETRIEVAL_PROMPT),
+            )
+        else:
+            main_chain = load_qa_chain(self.llm, verbose=self.debug)
+
         condense_question_chain = LLMChain(
             llm=self.qllm,
-            prompt=PromptTemplate.from_template(cqp),
+            prompt=PromptTemplate.from_template(self.QC_PROMPT),
             verbose=False,
             tags=["qchain"],
         )
         return ConversationalRetrievalChain(
             retriever=self.db().as_retriever(
                 search_kwargs={"k": self.config.ingest.target_source_chunks}
             ),
             combine_docs_chain=main_chain,
             question_generator=condense_question_chain,
             return_source_documents=True,
             memory=DocumentRetrievalBufferMemory(memory_key="chat_history"),
             get_chat_history=lambda x: x,
+            verbose=self.debug,
         )
 
     @cached_property
     def chain(self):
         """The chain object for chatting or document retrieval"""
         if self.config.ingest.source_directory:
             return self._create_retrieval_chain()
@@ -328,14 +355,15 @@
     ) -> Mapping[str, Any]:
         """Query the model with a string
 
         Note that if you have different input keys for you chain, you should
         override this method.
         """
         self.logger.debug("Retrieval calling: %r", query)
+
         return self.chain(
             {"question": query, "chat_history": []},
             callbacks=callbacks,
             return_only_outputs=True,
         )
 
     async def _a_retrieval_chain_call(
@@ -424,15 +452,15 @@
     def __init__(self, *args, **kwargs):
         """Initialize the ring"""
         super().__init__(*args, **kwargs)
         self.spawned = None
 
     def __del__(self):
         """Terminate the spawned process"""
-        if self.spawned:
+        if hasattr(self, "spawned") and self.spawned:
             self.logger.debug("Terminating spawned process")
             self.spawned.terminate()
             self.spawned = None
 
     async def _a_call(
         self,
         query: str,
```

### Comparing `pxgpt-0.0.0rc0/pxgpt/rings/openai.py` & `pxgpt-0.0.0rc1/pxgpt/rings/openai.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Provides ring for OpenAI models, such as text-davinci-***."""
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Mapping
+from typing import TYPE_CHECKING, Any, Mapping
 from langchain.embeddings import OpenAIEmbeddings
 from langchain.llms import OpenAI
 from langchain.llms.base import LLM
 
 from .base import BaseRing
 
 if TYPE_CHECKING:
@@ -29,14 +29,21 @@
             )
         }
 
     @property
     def embeddings(self) -> Embeddings:
         return OpenAIEmbeddings(**self.credentials, **self.config.embeddings)
 
+    @property
+    def model_args(self) -> Mapping[str, Any]:
+        out = super().model_args
+        if "model_path" in out:
+            del out["model_path"]
+        return out
+
     def _create_llm(self) -> LLM:
         """Create the LLM object, pass the credentials to it"""
         self.logger.info("Creating LLM (%s)", self.config.model.type)
 
         return self.MODEL(**self.model_args, **self.credentials)
 
     def _create_qllm(self) -> LLM | None:
```

### Comparing `pxgpt-0.0.0rc0/pxgpt/serve.py` & `pxgpt-0.0.0rc1/pxgpt/serve.py`

 * *Files identical despite different names*

### Comparing `pxgpt-0.0.0rc0/pxgpt/ws.py` & `pxgpt-0.0.0rc1/pxgpt/ws.py`

 * *Files identical despite different names*

### Comparing `pxgpt-0.0.0rc0/pxgpt/zzz.py` & `pxgpt-0.0.0rc1/pxgpt/zzz.py`

 * *Files identical despite different names*

### Comparing `pxgpt-0.0.0rc0/setup.py` & `pxgpt-0.0.0rc1/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,36 +5,41 @@
 ['pxgpt', 'pxgpt.rings']
 
 package_data = \
 {'': ['*'], 'pxgpt': ['frontend/build/*', 'frontend/build/assets/*']}
 
 install_requires = \
 ['argx>=0.2.9,<0.3.0',
- 'chromadb>=0.3.29,<0.4.0',
- 'langchain>=0.0.232,<0.0.233',
+ 'faiss-cpu>=1.7.4,<2.0.0',
+ 'langchain>=0.0.234,<0.0.235',
+ 'pandas>=2.0.3,<3.0.0',
  'prompt-toolkit>=3.0.39,<4.0.0',
+ 'py>=1.11.0,<2.0.0',
+ 'pyarrow>=12.0.1,<13.0.0',
+ 'pymupdf>=1.22.5,<2.0.0',
  'python-simpleconf[yaml]>=0.6.0,<0.7.0',
- 'quart>=0.18.4,<0.19.0']
+ 'quart>=0.18.4,<0.19.0',
+ 'scikit-learn>=1.3.0,<2.0.0']
 
 extras_require = \
 {'all': ['gpt4all>=1.0.3,<2.0.0',
          'llama-cpp-python>=0.1.70,<0.2.0',
          'openai>=0.27.8,<0.28.0'],
  'gpt4all': ['gpt4all>=1.0.3,<2.0.0'],
  'llama-cpp': ['llama-cpp-python>=0.1.70,<0.2.0'],
- 'openai': ['openai>=0.27.8,<0.28.0']}
+ 'openai': ['openai>=0.27.8,<0.28.0', 'tiktoken>=0.4.0,<0.5.0']}
 
 entry_points = \
 {'console_scripts': ['pxgpt = pxgpt.cli:main']}
 
 setup_kwargs = {
     'name': 'pxgpt',
-    'version': '0.0.0rc0',
+    'version': '0.0.0rc1',
     'description': 'Your personal, powerful and private GPT.',
-    'long_description': '# <img src="pxgpt/frontend/public/assets/favicon.png" alt="p" width=28 />GPT: Your personal, powerful and private GPT\n\n## Features\n\n- Ingest of your own documents and talk to them.\n- Store your data locally on your device.\n- Choose from a variety of models, including OpenAI.\n- Support conversation history and memory.\n- Switch between profiles with different settings.\n- Support both web interface and command line interface.\n\n## Installation\n\n```shell\n# With all supported models\n$ pip install -U pxgpt[all]\n\n# With support for GPT4all only\n$ pip install -U pxgpt[gpt4all]\n\n# With support for llama-cpp only\n$ pip install -U pxgpt[llama-cpp]\n\n# With support for openai only\n$ pip install -U pxgpt[openai]\n```\n\n## Usage\n\n### Chat from CLI\n\n```shell\n$ 23:45:06 ❯ pxgpt chat\n\nWelcome to chat via the pxgpt CLI v0.0.0!\nHit \'Ctrl+c\' or \'Ctrl+d\' to exit.\n[2023-07-18 23:45:09,969] INFO Creating LLM (GPT4All)\nFound model file at  models/gpt4all/ggml-gpt4all-j-v1.3-groovy.bin\ngptj_model_load: loading model from \'models/gpt4all/ggml-gpt4all-j-v1.3-groovy.bin\' - please wait ...\ngptj_model_load: n_vocab = 50400\ngptj_model_load: n_ctx   = 2048\ngptj_model_load: n_embd  = 4096\ngptj_model_load: n_head  = 16\ngptj_model_load: n_layer = 28\ngptj_model_load: n_rot   = 64\ngptj_model_load: f16     = 2\ngptj_model_load: ggml ctx size = 5401.45 MB\ngptj_model_load: kv self size  =  896.00 MB\ngptj_model_load: ................................... done\ngptj_model_load: model size =  3609.38 MB / num tensors = 285\n[2023-07-18 23:45:11,741] INFO Entering chat mode\nLoaded conversation:  2023-07-16_23-11-27\nUse the up/down arrow keys to navigate history.\nUse /help to see the list of commands.\n\n>>> Hello?\n  Hi there! How may I help you today?\n\n>>> /help\nCommands:\n  - /help: List the commands\n  - /new: Start a new conversation\n  - /switch: Switch to a conversation\n  - /list: List all conversations\n  - /path: Show the path of the current conversation file\n  - /delete: Delete a conversation\n  - /rename: Rename a conversation\n  - /ingest: Ingest documents from the source directory\n  - /docs: List ingested and uningested documents in the source directory\n  - /exit: Exit the CLI\n\n>>>\n```\n\n### Chat from the web interface\n\n```shell\n$ pxgpt serve\n# Open http://localhost:7758 in your browser\n```\n\n![Web-interface](web-interface.png)\n\n### Configuration\n\nThe configuration files are loaded from the following paths:\n\n- `~/.config/pxgpt/config.yml`\n- `~/.pxgpt.config.yml`\n- `./.pxgpt.config.yml`\n\n#### Profiles\n\nNote that you need to define profiles in the configuration file. For example:\n\n```yaml\nopenai:  # The profile\n    model:\n        type: ChatOpenAI\n```\n\nThe configuration items are inherited from the `default` profile. For example:\n\n```yaml\ndefault:\n    credentials:\n        openai_api_key: sk-xxxxxxxxxxx\n\nopenai:\n    model:\n        type: ChatOpenAI\n```\n\nThen when you use `openai` profile, the configurations are expanded as:\n\n```yaml\nopenai:\n    credentials:\n        openai_api_key: sk-xxxxxxxxxxx\n    model:\n        type: ChatOpenAI\n```\n\nHigher-level configurations override lower-level configurations. For example:\n\nIf you define the `default` profile in `~/.config/pxgpt/config.yml` and the `openai` profile in `./.pxgpt.config.yml`, then the `openai` profile will inherit the `default` profile, as well.\n\n#### Configuration items\n\n- `log_level`: The log level for the logger in your teminal\n- `history_directory`: The directory to store the conversation history\n- `history_into_memory`: Whether to load the conversation history into memory\n  - You can turn this off if you are using small models\n- `credentials`: The credentials for the models.\n  For example, for OpenAI, you need to provide the `openai_api_key`.\n- `model`: Type of the model and arguments for it.\n  - `type`: The type of the model, supported models are: `GPT4All`, `LlamaCpp`, `ChatOpenAI` and `OpenAI`\n  - `<other>`: The arguments for the model. Passed to `langchain` llms.\n    - For `GPT4All`, you can pass the arguments listed in [here][1].\n    - For `LlamaCpp`, you can pass the arguments listed in [here][2].\n    - For `ChatOpenAI`, you can pass the arguments listed in [here][3].\n    - For `OpenAI`, you can pass the arguments listed in [here][4].\n- `qmodel`: The arguments for model used to condense questions\n  - `type`: Same as `model.type`, with and `Echo` model added, which is useful for models that don\'t do question condensing very well.\n  - `<other>`: Same as `model.<other>`.\n- `ingest`: The arguments for the ingestion.\n  - `source_directory`: The directory to ingest documents from.\n    - If not provided, we will enter the chat mode.\n  - `persist_directory`: The directory to save the vectorstore database.\n    - If not provided, will use `<source_directory>/.pxgpt-<model>-db`.\n  - `target_source_chunks`: The number of chunks to return against the query.\n  - `n_workers`: The number of workers to use for ingestion.\n  - `chunk_size` and `chunk_overlap`: The chunk size and overlap for the ingestion.\n- `embeddings`: The arguments for the embeddings.\n  - For `GPT4All`, you can pass the arguments listed in [here][5].\n  - For `LlamaCpp`, you can pass the arguments listed in [here][6].\n  - For `OpenAI` or `ChatOpenAI`, you can pass the arguments listed in [here][7].\n\n### Ingest documents\n\n```shell\n$ pxgpt ingest  # default profile\n$ pxgpt ingest --profile openai-docs\n# Will ingest documents under `ingest.source_directory` under `openai-docs` profile\n```\n\n## Credits\n\n`pxgpt` is Inspired by [privateGPT][8], with the addition of openai API support, history and memory support, and a web interface.\n\n## TODO\n\n- [ ] Support ingestion management (upload/download/delete/ingest documents) from the web interface\n- [ ] Support profile management (add/remove/modify) from the web interface\n- [ ] Build a docker image\n- [ ] Support more models\n\n## Q & A\n\n[QA.md](QA.md)\n\n[1]: https://api.python.langchain.com/en/latest/llms/langchain.llms.gpt4all.GPT4All.html#langchain.llms.gpt4all.GPT4All\n[2]: https://api.python.langchain.com/en/latest/llms/langchain.llms.llamacpp.LlamaCpp.html#langchain.llms.llamacpp.LlamaCpp\n[3]: https://api.python.langchain.com/en/latest/chat_models/langchain.chat_models.openai.ChatOpenAI.html#langchain.chat_models.openai.ChatOpenAI\n[4]: https://api.python.langchain.com/en/latest/llms/langchain.llms.openai.OpenAI.html#langchain.llms.openai.OpenAI\n[5]: https://api.python.langchain.com/en/latest/embeddings/langchain.embeddings.huggingface.HuggingFaceEmbeddings.html#langchain.embeddings.huggingface.HuggingFaceEmbeddings\n[6]: https://api.python.langchain.com/en/latest/embeddings/langchain.embeddings.llamacpp.LlamaCppEmbeddings.html#langchain.embeddings.llamacpp.LlamaCppEmbeddings\n[7]: https://api.python.langchain.com/en/latest/embeddings/langchain.embeddings.openai.OpenAIEmbeddings.html#langchain.embeddings.openai.OpenAIEmbeddings\n[8]: https://github.com/imartinez/privateGPT\n',
+    'long_description': '<div style="display: flex; align-items: center; justify-content: center; gap: .2rem">\n  <img src="pxgpt/frontend/public/assets/favicon.png" alt="px" style="width: 32px; height: 32px;" />\n  <div style="font-size: 24px; font-weight: bold">GPT</div>\n</div>\n<hr />\n<p style="text-align: center">Your personal, powerful and private GPT</p>\n\n\n\n## Features\n\n- Ingest of your own documents and talk to them.\n- Store your data locally on your device.\n- Choose from a variety of models, including OpenAI.\n- Support conversation history and memory.\n- Switch between profiles with different settings.\n- Support both web interface and command line interface.\n- Support Llama v2!\n\n## Installation\n\n```shell\n# With all supported models\n$ pip install -U pxgpt[all]\n\n# With support for GPT4all only\n$ pip install -U pxgpt[gpt4all]\n\n# With support for llama-cpp only\n$ pip install -U pxgpt[llama-cpp]\n\n# With support for openai only\n$ pip install -U pxgpt[openai]\n```\n\nThen copy the configuration from `.pxgpt.config-example.yml` to `.pxgpt.config.yml` and modify it to your needs.\n\n## Usage\n\n### Chat from CLI\n\n```shell\n$ 23:45:06 ❯ pxgpt chat\n\nWelcome to chat via the pxGPT CLI v0.0.0rc0!\nHit \'Ctrl+c\' or \'Ctrl+d\' to exit.\n[2023-07-20 20:03:22,716] INFO Switched profile to llamacpp-chat\n[2023-07-20 20:03:22,719] INFO Creating LLM (LlamaCpp)\nllama.cpp: loading model from models/llamacpp/llama-2-7b.ggmlv3.q4_0.bin\nllama_model_load_internal: format     = ggjt v3 (latest)\nllama_model_load_internal: n_vocab    = 32000\nllama_model_load_internal: n_ctx      = 512\nllama_model_load_internal: n_embd     = 4096\nllama_model_load_internal: n_mult     = 256\nllama_model_load_internal: n_head     = 32\nllama_model_load_internal: n_layer    = 32\nllama_model_load_internal: n_rot      = 128\nllama_model_load_internal: freq_base  = 10000.0\nllama_model_load_internal: freq_scale = 1\nllama_model_load_internal: ftype      = 2 (mostly Q4_0)\nllama_model_load_internal: n_ff       = 11008\nllama_model_load_internal: model size = 7B\nllama_model_load_internal: ggml ctx size =    0.08 MB\nllama_model_load_internal: mem required  = 5185.72 MB (+ 1026.00 MB per state)\nllama_new_context_with_model: kv self size  =  256.00 MB\n[2023-07-20 20:03:24,552] INFO Entering chat mode\nLoaded conversation:  2023-07-20_20-03-17\nUse the up/down arrow keys to navigate history.\nUse /help to see the list of commands.\n\n>>> Hello Llama 2, if you could choose a superpower, what would it be and why?\n I will answer this question in two parts. The first part is the super power that I will choose. The second part is why I chose this super power.\nIn the first part, the super power that I will choose is the ability to fly. This is because flying has many benefits. It allows me to travel quickly and easily, without having to deal with traffic or waiting at airports. Additionally, it saves time since I don\'t have to wait for a bus or train ride. Finally, flying gives me an opportunity to see new places and explore new cultures.\nIn the second part of my answer, I will explain why I chose this super power. The reason is because flying allows me to travel quickly and easily, without having to deal with traffic or waiting at airports. Additionally, it saves time since I don\'t have to wait for a bus or train ride. Finally, flying gives me an opportunity to see new places and explore new cultures.\n\n>>> /help\nCommands:\n  - /help: List the commands\n  - /new: Start a new conversation\n  - /switch: Switch to a conversation\n  - /list: List all conversations\n  - /path: Show the path of the current conversation file\n  - /delete: Delete a conversation\n  - /rename: Rename a conversation\n  - /ingest: Ingest documents from the source directory\n  - /docs: List ingested and uningested documents in the source directory\n  - /exit: Exit the CLI\n\n>>>\n```\n\n### Chat from the web interface\n\n```shell\n$ pxgpt serve\n# Open http://localhost:7758 in your browser\n```\n\n![Web-interface](web-interface.png)\n\n### Configuration\npx\nThe configuration files are loaded from the following paths:\n\n- `~/.config/pxgpt/config.yml`\n- `~/.pxgpt.config.yml`\n- `./.pxgpt.config.yml`\n\n#### Profiles\n\nNote that you need to define profiles in the configuration file. For example:\n\n```yaml\nopenai:  # The profile\n    model:\n        type: ChatOpenAI\n```\n\nThe configuration items are inherited from the `default` profile. For example:\n\n```yaml\ndefault:\n    credentials:\n        openai_api_key: sk-xxxxxxxxxxx\n\nopenai:\n    model:\n        type: ChatOpenAI\n```\n\nThen when you use `openai` profile, the configurations are expanded as:\n\n```yaml\nopenai:\n    credentials:\n        openai_api_key: sk-xxxxxxxxxxx\n    model:\n        type: ChatOpenAI\n```\n\nHigher-level configurations override lower-level configurations. For example:\n\nIf you define the `default` profile in `~/.config/pxgpt/config.yml` and the `openai` profile in `./.pxgpt.config.yml`, then the `openai` profile will inherit the `default` profile, as well.\n\n#### Configuration items\n\n- `log_level`: The log level for the logger in your teminal\n- `history_directory`: The directory to store the conversation history\n- `history_into_memory`: Whether to load the conversation history into memory\n  - You can turn this off if you are using small models\n- `credentials`: The credentials for the models.\n  For example, for OpenAI, you need to provide the `openai_api_key`.\n- `model`: Type of the model and arguments for it.\n  - `type`: The type of the model, supported models are: `GPT4All`, `LlamaCpp`, `ChatOpenAI` and `OpenAI`\n  - `<other>`: The arguments for the model. Passed to `langchain` llms.\n    - For `GPT4All`, you can pass the arguments listed in [here][1].\n    - For `LlamaCpp`, you can pass the arguments listed in [here][2].\n    - For `ChatOpenAI`, you can pass the arguments listed in [here][3].\n    - For `OpenAI`, you can pass the arguments listed in [here][4].\n- `qmodel`: The arguments for model used to condense questions\n  - `type`: Same as `model.type`, with and `Echo` model added, which is useful for models that don\'t do question condensing very well.\n  - `<other>`: Same as `model.<other>`.\n- `ingest`: The arguments for the ingestion.\n  - `source_directory`: The directory to ingest documents from.\n    - If not provided, we will enter the chat mode.\n  - `persist_directory`: The directory to save the vectorstore database.\n    - If not provided, will use `<source_directory>/.pxgpt-<model>-db`.\n  - `target_source_chunks`: The number of chunks to return against the query.\n  - `n_workers`: The number of workers to use for ingestion.\n  - `chunk_size` and `chunk_overlap`: The chunk size and overlap for the ingestion.\n- `embeddings`: The arguments for the embeddings.\n  - For `GPT4All`, you can pass the arguments listed in [here][5].\n  - For `LlamaCpp`, you can pass the arguments listed in [here][6].\n  - For `OpenAI` or `ChatOpenAI`, you can pass the arguments listed in [here][7].\n\n### Ingest documents\n\n```shell\n$ pxgpt ingest  # default profile\n$ pxgpt ingest --profile openai-docs\n# Will ingest documents under `ingest.source_directory` under `openai-docs` profile\n```\n\n## Credits\n\n`pxgpt` is Inspired by [privateGPT][8], with the addition of openai API support, history and memory support, and a web interface.\n\n## TODO\n\n- [ ] Support ingestion management (upload/download/delete/ingest documents) from the web interface\n- [ ] Support profile management (add/remove/modify) from the web interface\n- [ ] Use markdown to format the response on the web interface\n- [ ] Build a docker image\n- [ ] Support more models\n\n## Q & A\n\n[QA.md](QA.md)\n\n[1]: https://api.python.langchain.com/en/latest/llms/langchain.llms.gpt4all.GPT4All.html#langchain.llms.gpt4all.GPT4All\n[2]: https://api.python.langchain.com/en/latest/llms/langchain.llms.llamacpp.LlamaCpp.html#langchain.llms.llamacpp.LlamaCpp\n[3]: https://api.python.langchain.com/en/latest/chat_models/langchain.chat_models.openai.ChatOpenAI.html#langchain.chat_models.openai.ChatOpenAI\n[4]: https://api.python.langchain.com/en/latest/llms/langchain.llms.openai.OpenAI.html#langchain.llms.openai.OpenAI\n[5]: https://api.python.langchain.com/en/latest/embeddings/langchain.embeddings.gpt4all.GPT4AllEmbeddings.html#langchain.embeddings.gpt4all.GPT4AllEmbeddings\n[6]: https://api.python.langchain.com/en/latest/embeddings/langchain.embeddings.llamacpp.LlamaCppEmbeddings.html#langchain.embeddings.llamacpp.LlamaCppEmbeddings\n[7]: https://api.python.langchain.com/en/latest/embeddings/langchain.embeddings.openai.OpenAIEmbeddings.html#langchain.embeddings.openai.OpenAIEmbeddings\n[8]: https://github.com/imartinez/privateGPT\n',
     'author': 'pwwang',
     'author_email': 'pwwang@pwwang.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `pxgpt-0.0.0rc0/PKG-INFO` & `pxgpt-0.0.0rc1/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pxgpt
-Version: 0.0.0rc0
+Version: 0.0.0rc1
 Summary: Your personal, powerful and private GPT.
 License: Apache-2.0
 Author: pwwang
 Author-email: pwwang@pwwang.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
@@ -12,34 +12,48 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: all
 Provides-Extra: gpt4all
 Provides-Extra: llama-cpp
 Provides-Extra: openai
 Requires-Dist: argx (>=0.2.9,<0.3.0)
-Requires-Dist: chromadb (>=0.3.29,<0.4.0)
+Requires-Dist: faiss-cpu (>=1.7.4,<2.0.0)
 Requires-Dist: gpt4all (>=1.0.3,<2.0.0) ; extra == "gpt4all" or extra == "all"
-Requires-Dist: langchain (>=0.0.232,<0.0.233)
+Requires-Dist: langchain (>=0.0.234,<0.0.235)
 Requires-Dist: llama-cpp-python (>=0.1.70,<0.2.0) ; extra == "llama-cpp" or extra == "all"
 Requires-Dist: openai (>=0.27.8,<0.28.0) ; extra == "openai" or extra == "all"
+Requires-Dist: pandas (>=2.0.3,<3.0.0)
 Requires-Dist: prompt-toolkit (>=3.0.39,<4.0.0)
+Requires-Dist: py (>=1.11.0,<2.0.0)
+Requires-Dist: pyarrow (>=12.0.1,<13.0.0)
+Requires-Dist: pymupdf (>=1.22.5,<2.0.0)
 Requires-Dist: python-simpleconf[yaml] (>=0.6.0,<0.7.0)
 Requires-Dist: quart (>=0.18.4,<0.19.0)
+Requires-Dist: scikit-learn (>=1.3.0,<2.0.0)
+Requires-Dist: tiktoken (>=0.4.0,<0.5.0) ; extra == "openai"
 Description-Content-Type: text/markdown
 
-# <img src="pxgpt/frontend/public/assets/favicon.png" alt="p" width=28 />GPT: Your personal, powerful and private GPT
+<div style="display: flex; align-items: center; justify-content: center; gap: .2rem">
+  <img src="pxgpt/frontend/public/assets/favicon.png" alt="px" style="width: 32px; height: 32px;" />
+  <div style="font-size: 24px; font-weight: bold">GPT</div>
+</div>
+<hr />
+<p style="text-align: center">Your personal, powerful and private GPT</p>
+
+
 
 ## Features
 
 - Ingest of your own documents and talk to them.
 - Store your data locally on your device.
 - Choose from a variety of models, including OpenAI.
 - Support conversation history and memory.
 - Switch between profiles with different settings.
 - Support both web interface and command line interface.
+- Support Llama v2!
 
 ## Installation
 
 ```shell
 # With all supported models
 $ pip install -U pxgpt[all]
 
@@ -49,44 +63,53 @@
 # With support for llama-cpp only
 $ pip install -U pxgpt[llama-cpp]
 
 # With support for openai only
 $ pip install -U pxgpt[openai]
 ```
 
+Then copy the configuration from `.pxgpt.config-example.yml` to `.pxgpt.config.yml` and modify it to your needs.
+
 ## Usage
 
 ### Chat from CLI
 
 ```shell
 $ 23:45:06 ❯ pxgpt chat
 
-Welcome to chat via the pxgpt CLI v0.0.0!
+Welcome to chat via the pxGPT CLI v0.0.0rc0!
 Hit 'Ctrl+c' or 'Ctrl+d' to exit.
-[2023-07-18 23:45:09,969] INFO Creating LLM (GPT4All)
-Found model file at  models/gpt4all/ggml-gpt4all-j-v1.3-groovy.bin
-gptj_model_load: loading model from 'models/gpt4all/ggml-gpt4all-j-v1.3-groovy.bin' - please wait ...
-gptj_model_load: n_vocab = 50400
-gptj_model_load: n_ctx   = 2048
-gptj_model_load: n_embd  = 4096
-gptj_model_load: n_head  = 16
-gptj_model_load: n_layer = 28
-gptj_model_load: n_rot   = 64
-gptj_model_load: f16     = 2
-gptj_model_load: ggml ctx size = 5401.45 MB
-gptj_model_load: kv self size  =  896.00 MB
-gptj_model_load: ................................... done
-gptj_model_load: model size =  3609.38 MB / num tensors = 285
-[2023-07-18 23:45:11,741] INFO Entering chat mode
-Loaded conversation:  2023-07-16_23-11-27
+[2023-07-20 20:03:22,716] INFO Switched profile to llamacpp-chat
+[2023-07-20 20:03:22,719] INFO Creating LLM (LlamaCpp)
+llama.cpp: loading model from models/llamacpp/llama-2-7b.ggmlv3.q4_0.bin
+llama_model_load_internal: format     = ggjt v3 (latest)
+llama_model_load_internal: n_vocab    = 32000
+llama_model_load_internal: n_ctx      = 512
+llama_model_load_internal: n_embd     = 4096
+llama_model_load_internal: n_mult     = 256
+llama_model_load_internal: n_head     = 32
+llama_model_load_internal: n_layer    = 32
+llama_model_load_internal: n_rot      = 128
+llama_model_load_internal: freq_base  = 10000.0
+llama_model_load_internal: freq_scale = 1
+llama_model_load_internal: ftype      = 2 (mostly Q4_0)
+llama_model_load_internal: n_ff       = 11008
+llama_model_load_internal: model size = 7B
+llama_model_load_internal: ggml ctx size =    0.08 MB
+llama_model_load_internal: mem required  = 5185.72 MB (+ 1026.00 MB per state)
+llama_new_context_with_model: kv self size  =  256.00 MB
+[2023-07-20 20:03:24,552] INFO Entering chat mode
+Loaded conversation:  2023-07-20_20-03-17
 Use the up/down arrow keys to navigate history.
 Use /help to see the list of commands.
 
->>> Hello?
-  Hi there! How may I help you today?
+>>> Hello Llama 2, if you could choose a superpower, what would it be and why?
+ I will answer this question in two parts. The first part is the super power that I will choose. The second part is why I chose this super power.
+In the first part, the super power that I will choose is the ability to fly. This is because flying has many benefits. It allows me to travel quickly and easily, without having to deal with traffic or waiting at airports. Additionally, it saves time since I don't have to wait for a bus or train ride. Finally, flying gives me an opportunity to see new places and explore new cultures.
+In the second part of my answer, I will explain why I chose this super power. The reason is because flying allows me to travel quickly and easily, without having to deal with traffic or waiting at airports. Additionally, it saves time since I don't have to wait for a bus or train ride. Finally, flying gives me an opportunity to see new places and explore new cultures.
 
 >>> /help
 Commands:
   - /help: List the commands
   - /new: Start a new conversation
   - /switch: Switch to a conversation
   - /list: List all conversations
@@ -106,15 +129,15 @@
 $ pxgpt serve
 # Open http://localhost:7758 in your browser
 ```
 
 ![Web-interface](web-interface.png)
 
 ### Configuration
-
+px
 The configuration files are loaded from the following paths:
 
 - `~/.config/pxgpt/config.yml`
 - `~/.pxgpt.config.yml`
 - `./.pxgpt.config.yml`
 
 #### Profiles
@@ -196,23 +219,24 @@
 
 `pxgpt` is Inspired by [privateGPT][8], with the addition of openai API support, history and memory support, and a web interface.
 
 ## TODO
 
 - [ ] Support ingestion management (upload/download/delete/ingest documents) from the web interface
 - [ ] Support profile management (add/remove/modify) from the web interface
+- [ ] Use markdown to format the response on the web interface
 - [ ] Build a docker image
 - [ ] Support more models
 
 ## Q & A
 
 [QA.md](QA.md)
 
 [1]: https://api.python.langchain.com/en/latest/llms/langchain.llms.gpt4all.GPT4All.html#langchain.llms.gpt4all.GPT4All
 [2]: https://api.python.langchain.com/en/latest/llms/langchain.llms.llamacpp.LlamaCpp.html#langchain.llms.llamacpp.LlamaCpp
 [3]: https://api.python.langchain.com/en/latest/chat_models/langchain.chat_models.openai.ChatOpenAI.html#langchain.chat_models.openai.ChatOpenAI
 [4]: https://api.python.langchain.com/en/latest/llms/langchain.llms.openai.OpenAI.html#langchain.llms.openai.OpenAI
-[5]: https://api.python.langchain.com/en/latest/embeddings/langchain.embeddings.huggingface.HuggingFaceEmbeddings.html#langchain.embeddings.huggingface.HuggingFaceEmbeddings
+[5]: https://api.python.langchain.com/en/latest/embeddings/langchain.embeddings.gpt4all.GPT4AllEmbeddings.html#langchain.embeddings.gpt4all.GPT4AllEmbeddings
 [6]: https://api.python.langchain.com/en/latest/embeddings/langchain.embeddings.llamacpp.LlamaCppEmbeddings.html#langchain.embeddings.llamacpp.LlamaCppEmbeddings
 [7]: https://api.python.langchain.com/en/latest/embeddings/langchain.embeddings.openai.OpenAIEmbeddings.html#langchain.embeddings.openai.OpenAIEmbeddings
 [8]: https://github.com/imartinez/privateGPT
```

