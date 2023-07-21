# Comparing `tmp/napari-chatgpt-2023.7.21.tar.gz` & `tmp/napari-chatgpt-2023.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari-chatgpt-2023.7.21.tar", last modified: Fri Jul 21 18:56:29 2023, max compression
+gzip compressed data, was "napari-chatgpt-2023.7.7.tar", last modified: Fri Jul  7 20:54:06 2023, max compression
```

## Comparing `napari-chatgpt-2023.7.21.tar` & `napari-chatgpt-2023.7.7.tar`

### file list

```diff
@@ -1,257 +1,257 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:56:29.383230 napari-chatgpt-2023.7.21/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:56:29.315228 napari-chatgpt-2023.7.21/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:56:29.319228 napari-chatgpt-2023.7.21/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/.github/workflows/just_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:56:29.319228 napari-chatgpt-2023.7.21/.napari-hub/
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/.napari-hub/DESCRIPTION.md
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/.napari-hub/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    22105 2023-07-21 18:56:29.383230 napari-chatgpt-2023.7.21/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20845 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-07-21 18:56:29.383230 napari-chatgpt-2023.7.21/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:56:29.319228 napari-chatgpt-2023.7.21/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:56:29.319228 napari-chatgpt-2023.7.21/src/napari_chatgpt/
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:56:29.327228 napari-chatgpt-2023.7.21/src/napari_chatgpt/_sandbox/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/_sandbox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/_sandbox/agent_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/_sandbox/bard_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/_sandbox/beautiful_soup_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2940 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/_sandbox/conv_agent_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/_sandbox/duckduckgo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/_sandbox/enumerate_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/_sandbox/enumerate_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/_sandbox/google.py
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/_sandbox/gpt4all_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/_sandbox/gtts_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/_sandbox/lanchain_openai.py
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/_sandbox/openai_list_models.py
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/_sandbox/playwright_sandbox.py
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/_sandbox/speech_recognition_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)    12512 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/_sandbox/terminal.py
--rw-r--r--   0 runner    (1001) docker     (123)     3772 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/_sandbox/test.py
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/_sandbox/tts_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/_sandbox/whisper_cpp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:56:29.327228 napari-chatgpt-2023.7.21/src/napari_chatgpt/_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/_tests/test_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-21 18:56:29.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    13957 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:56:29.327228 napari-chatgpt-2023.7.21/src/napari_chatgpt/chat_server/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/chat_server/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:56:29.331228 napari-chatgpt-2023.7.21/src/napari_chatgpt/chat_server/callbacks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/chat_server/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5041 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/chat_server/callbacks/callbacks_handle_chat.py
--rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/chat_server/callbacks/callbacks_handler_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)     4813 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/chat_server/callbacks/callbacks_stdout.py
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/chat_server/chat_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11495 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/chat_server/chat_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:56:29.331228 napari-chatgpt-2023.7.21/src/napari_chatgpt/chat_server/demo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/chat_server/demo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/chat_server/demo/chat_server_demo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:56:29.335228 napari-chatgpt-2023.7.21/src/napari_chatgpt/chat_server/static/
--rw-r--r--   0 runner    (1001) docker     (123)  3642321 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/chat_server/static/_tailwind.css
--rw-r--r--   0 runner    (1001) docker     (123)     7344 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/chat_server/static/chat.js
--rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/chat_server/static/marked-highlight.js
--rw-r--r--   0 runner    (1001) docker     (123)     3971 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/chat_server/static/prism.css
--rw-r--r--   0 runner    (1001) docker     (123)    54713 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/chat_server/static/prism.js
--rw-r--r--   0 runner    (1001) docker     (123)    15800 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/chat_server/static/sunlight-min.js
--rw-r--r--   0 runner    (1001) docker     (123)     8654 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/chat_server/static/sunlight.dark.css
--rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/chat_server/static/sunlight.python-min.js
--rw-r--r--   0 runner    (1001) docker     (123)  3897394 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/chat_server/static/tailwind.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:56:29.339228 napari-chatgpt-2023.7.21/src/napari_chatgpt/chat_server/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     4075 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/chat_server/templates/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:56:29.343229 napari-chatgpt-2023.7.21/src/napari_chatgpt/llm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/llm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/llm/bard.py
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/llm/gpt4all.py
--rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/llm/llms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:56:29.343229 napari-chatgpt-2023.7.21/src/napari_chatgpt/llm/test/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:56:29.343229 napari-chatgpt-2023.7.21/src/napari_chatgpt/llm/test/.pytest_cache/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/llm/test/.pytest_cache/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/llm/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/llm/test/bard_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/napari.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:56:29.343229 napari-chatgpt-2023.7.21/src/napari_chatgpt/omega/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/omega/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:56:29.343229 napari-chatgpt-2023.7.21/src/napari_chatgpt/omega/memory/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/omega/memory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4069 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/omega/memory/memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/omega/napari_bridge.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:56:29.347229 napari-chatgpt-2023.7.21/src/napari_chatgpt/omega/omega_agent/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/omega/omega_agent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/omega/omega_agent/agent.py
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/omega/omega_agent/agent_executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/omega/omega_agent/agent_output_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     4397 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/omega/omega_agent/prompts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:56:29.347229 napari-chatgpt-2023.7.21/src/napari_chatgpt/omega/omega_agent/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/omega/omega_agent/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4356 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/omega/omega_agent/tests/agent_output_parser_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     6034 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/omega/omega_init.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:56:29.347229 napari-chatgpt-2023.7.21/src/napari_chatgpt/omega/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/omega/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/omega/tools/async_base_tool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:56:29.347229 napari-chatgpt-2023.7.21/src/napari_chatgpt/omega/tools/demo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/omega/tools/demo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/omega/tools/demo/tools_demo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:56:29.351229 napari-chatgpt-2023.7.21/src/napari_chatgpt/omega/tools/examples/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/omega/tools/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/omega/tools/examples/example_omega_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/omega/tools/instructions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:56:29.351229 napari-chatgpt-2023.7.21/src/napari_chatgpt/omega/tools/napari/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/omega/tools/napari/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13205 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/omega/tools/napari/cell_nuclei_segmentation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:56:29.355229 napari-chatgpt-2023.7.21/src/napari_chatgpt/omega/tools/napari/delegated_code/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/omega/tools/napari/delegated_code/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/omega/tools/napari/delegated_code/aydin_classic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/omega/tools/napari/delegated_code/aydin_fgr.py
--rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/omega/tools/napari/delegated_code/cellpose.py
--rw-r--r--   0 runner    (1001) docker     (123)     5703 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/omega/tools/napari/delegated_code/classic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/omega/tools/napari/delegated_code/stardist.py
--rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/omega/tools/napari/file_open_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)     7945 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/omega/tools/napari/image_denoising.py
--rw-r--r--   0 runner    (1001) docker     (123)     9000 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/omega/tools/napari/napari_base_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)     9654 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/omega/tools/napari/viewer_control_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)     4908 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/omega/tools/napari/viewer_query_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)     8271 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/omega/tools/napari/widget_maker_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/omega/tools/napari_plugin_tool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:56:29.355229 napari-chatgpt-2023.7.21/src/napari_chatgpt/omega/tools/search/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/omega/tools/search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3470 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/omega/tools/search/web_image_search_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/omega/tools/search/web_search_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/omega/tools/search/wikipedia_query_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/omega/tools/search/wikipedia_search_tool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:56:29.355229 napari-chatgpt-2023.7.21/src/napari_chatgpt/omega/tools/special/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/omega/tools/special/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/omega/tools/special/exception_catcher_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/omega/tools/special/file_download_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/omega/tools/special/functions_info_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/omega/tools/special/human_input_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/omega/tools/special/python_repl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:56:29.359229 napari-chatgpt-2023.7.21/src/napari_chatgpt/omega/tools/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/omega/tools/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/omega/tools/tests/functions_info_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/omega/tools/tests/web_search_tool_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/omega/tools/tests/wikipedia_search_tool_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:56:29.359229 napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:56:29.359229 napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/api_keys/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/api_keys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/api_keys/api_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     3025 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/api_keys/api_key_vault.py
--rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/api_keys/api_key_vault_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/api_keys/api_key_vault_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:56:29.359229 napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/api_keys/demo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/api_keys/demo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/api_keys/demo/api_key_vault_dialog_demo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:56:29.359229 napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/async_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/async_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/async_utils/run_async.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:56:29.359229 napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/download/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/download/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/download/download_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/download/gpt4all.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:56:29.363229 napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/download/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/download/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/download/test/download_files_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:56:29.363229 napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/images/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/images/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/images/normalize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:56:29.363229 napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/llm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/llm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/llm/summarizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:56:29.363229 napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/llm/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/llm/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/llm/test/summarizer_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:56:29.363229 napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/napari/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/napari/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:56:29.363229 napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/napari/demo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/napari/demo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/napari/demo/open_zarr_in_napari_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/napari/napari_viewer_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/napari/open_in_napari.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:56:29.363229 napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/napari/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/napari/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/napari/test/napari_viewer_info_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:56:29.367229 napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/omega_plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/omega_plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/omega_plugins/discover_omega_plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:56:29.367229 napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/omega_plugins/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/omega_plugins/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/omega_plugins/test/discover_omega_plugins_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:56:29.371229 napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/python/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/python/conda_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/python/dynamic_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/python/exception_description.py
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/python/exception_guard.py
--rw-r--r--   0 runner    (1001) docker     (123)     7704 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/python/fix_bad_fun_calls.py
--rw-r--r--   0 runner    (1001) docker     (123)     6032 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/python/fix_code_given_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/python/installed_packages.py
--rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/python/missing_packages.py
--rw-r--r--   0 runner    (1001) docker     (123)     3938 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/python/pip_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    12403 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/python/python_lang_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5444 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/python/required_imports.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:56:29.371229 napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/python/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/python/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/python/test/dynamic_import_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/python/test/exception_description_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/python/test/exception_guard_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/python/test/fix_bad_function_calls_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/python/test/fix_code_given_error_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/python/test/installed_packages_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/python/test/missing_libraries_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/python/test/python_lang_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/python/test/required_imports_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:56:29.371229 napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/qt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/qt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4945 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/qt/download_file_qt.py
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/qt/qt_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:56:29.375229 napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/strings/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/strings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/strings/camel_case_to_normal.py
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/strings/extract_code.py
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/strings/extract_urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/strings/filter_lines.py
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/strings/find_function_name.py
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/strings/find_integer_in_parenthesis.py
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/strings/python_code_cleanup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:56:29.375229 napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/strings/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/strings/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/strings/test/extract_code_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/strings/test/extract_url_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/strings/test/filter_lines_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/strings/test/find_function_name_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/strings/test/find_integer_in_parenthesis_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:56:29.379229 napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/system/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/system/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/system/folders.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:56:29.379229 napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/web/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/web/duckduckgo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/web/google.py
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/web/headers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/web/metasearch.py
--rw-r--r--   0 runner    (1001) docker     (123)     3442 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/web/scrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:56:29.379229 napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/web/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/web/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/web/test/duckduckgo_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/web/test/google_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/web/test/metasearch_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/web/test/scrapper_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/web/test/wikipedia_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/web/wikipedia.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 18:56:29.323228 napari-chatgpt-2023.7.21/src/napari_chatgpt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    22105 2023-07-21 18:56:29.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10056 2023-07-21 18:56:29.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 18:56:29.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-21 18:56:29.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-07-21 18:56:29.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-21 18:56:29.000000 napari-chatgpt-2023.7.21/src/napari_chatgpt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-07-21 18:56:11.000000 napari-chatgpt-2023.7.21/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:54:06.660058 napari-chatgpt-2023.7.7/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:54:06.564057 napari-chatgpt-2023.7.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:54:06.580057 napari-chatgpt-2023.7.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/.github/workflows/just_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2821 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:54:06.580057 napari-chatgpt-2023.7.7/.napari-hub/
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/.napari-hub/DESCRIPTION.md
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/.napari-hub/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    22104 2023-07-07 20:54:06.660058 napari-chatgpt-2023.7.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20845 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-07-07 20:54:06.660058 napari-chatgpt-2023.7.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:54:06.584058 napari-chatgpt-2023.7.7/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:54:06.584058 napari-chatgpt-2023.7.7/src/napari_chatgpt/
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:54:06.592058 napari-chatgpt-2023.7.7/src/napari_chatgpt/_sandbox/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/_sandbox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/_sandbox/agent_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/_sandbox/bard_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/_sandbox/beautiful_soup_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2940 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/_sandbox/conv_agent_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/_sandbox/duckduckgo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/_sandbox/enumerate_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/_sandbox/enumerate_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/_sandbox/google.py
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/_sandbox/gpt4all_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/_sandbox/gtts_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/_sandbox/lanchain_openai.py
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/_sandbox/openai_list_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/_sandbox/playwright_sandbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/_sandbox/speech_recognition_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12512 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/_sandbox/terminal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3772 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/_sandbox/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/_sandbox/tts_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/_sandbox/whisper_cpp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:54:06.596058 napari-chatgpt-2023.7.7/src/napari_chatgpt/_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/_tests/test_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-07 20:54:06.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14335 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:54:06.596058 napari-chatgpt-2023.7.7/src/napari_chatgpt/chat_server/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/chat_server/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:54:06.596058 napari-chatgpt-2023.7.7/src/napari_chatgpt/chat_server/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/chat_server/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5041 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/chat_server/callbacks/callbacks_handle_chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/chat_server/callbacks/callbacks_handler_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4813 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/chat_server/callbacks/callbacks_stdout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/chat_server/chat_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11495 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/chat_server/chat_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:54:06.596058 napari-chatgpt-2023.7.7/src/napari_chatgpt/chat_server/demo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/chat_server/demo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/chat_server/demo/chat_server_demo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:54:06.604058 napari-chatgpt-2023.7.7/src/napari_chatgpt/chat_server/static/
+-rw-r--r--   0 runner    (1001) docker     (123)  3642321 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/chat_server/static/_tailwind.css
+-rw-r--r--   0 runner    (1001) docker     (123)     7344 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/chat_server/static/chat.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/chat_server/static/marked-highlight.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3971 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/chat_server/static/prism.css
+-rw-r--r--   0 runner    (1001) docker     (123)    54713 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/chat_server/static/prism.js
+-rw-r--r--   0 runner    (1001) docker     (123)    15800 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/chat_server/static/sunlight-min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8654 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/chat_server/static/sunlight.dark.css
+-rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/chat_server/static/sunlight.python-min.js
+-rw-r--r--   0 runner    (1001) docker     (123)  3897394 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/chat_server/static/tailwind.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:54:06.612058 napari-chatgpt-2023.7.7/src/napari_chatgpt/chat_server/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     4075 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/chat_server/templates/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:54:06.612058 napari-chatgpt-2023.7.7/src/napari_chatgpt/llm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/llm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/llm/bard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/llm/gpt4all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/llm/llms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:54:06.612058 napari-chatgpt-2023.7.7/src/napari_chatgpt/llm/test/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:54:06.612058 napari-chatgpt-2023.7.7/src/napari_chatgpt/llm/test/.pytest_cache/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/llm/test/.pytest_cache/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/llm/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/llm/test/bard_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/napari.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:54:06.616058 napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:54:06.616058 napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/memory/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/memory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4069 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/memory/memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/napari_bridge.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:54:06.616058 napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/omega_agent/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/omega_agent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/omega_agent/agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/omega_agent/agent_executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/omega_agent/agent_output_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4397 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/omega_agent/prompts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:54:06.616058 napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/omega_agent/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/omega_agent/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4356 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/omega_agent/tests/agent_output_parser_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6034 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/omega_init.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:54:06.620058 napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/tools/async_base_tool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:54:06.620058 napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/tools/demo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/tools/demo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/tools/demo/tools_demo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:54:06.620058 napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/tools/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/tools/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/tools/examples/example_omega_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/tools/instructions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:54:06.624058 napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/tools/napari/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/tools/napari/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13168 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/tools/napari/cell_nuclei_segmentation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:54:06.628058 napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/tools/napari/delegated_code/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/tools/napari/delegated_code/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/tools/napari/delegated_code/aydin_classic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/tools/napari/delegated_code/aydin_fgr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/tools/napari/delegated_code/cellpose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5703 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/tools/napari/delegated_code/classic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/tools/napari/delegated_code/stardist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/tools/napari/file_open_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7908 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/tools/napari/image_denoising.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9000 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/tools/napari/napari_base_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9633 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/tools/napari/viewer_control_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4894 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/tools/napari/viewer_query_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8234 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/tools/napari/widget_maker_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/tools/napari_plugin_tool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:54:06.628058 napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/tools/search/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/tools/search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3470 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/tools/search/web_image_search_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/tools/search/web_search_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/tools/search/wikipedia_query_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/tools/search/wikipedia_search_tool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:54:06.632058 napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/tools/special/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/tools/special/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/tools/special/exception_catcher_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/tools/special/file_download_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/tools/special/functions_info_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/tools/special/human_input_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/tools/special/python_repl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:54:06.632058 napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/tools/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/tools/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/tools/tests/functions_info_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/tools/tests/web_search_tool_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/tools/tests/wikipedia_search_tool_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:54:06.632058 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:54:06.636058 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/api_keys/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/api_keys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/api_keys/api_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3025 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/api_keys/api_key_vault.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/api_keys/api_key_vault_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/api_keys/api_key_vault_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:54:06.636058 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/api_keys/demo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/api_keys/demo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/api_keys/demo/api_key_vault_dialog_demo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:54:06.636058 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/async_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/async_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/async_utils/run_async.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:54:06.636058 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/download/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/download/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/download/download_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/download/gpt4all.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:54:06.636058 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/download/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/download/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/download/test/download_files_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:54:06.640058 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/images/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/images/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/images/normalize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:54:06.640058 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/llm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/llm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/llm/summarizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:54:06.640058 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/llm/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/llm/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/llm/test/summarizer_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:54:06.640058 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/napari/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/napari/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:54:06.640058 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/napari/demo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/napari/demo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/napari/demo/open_zarr_in_napari_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/napari/napari_viewer_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/napari/open_in_napari.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:54:06.644058 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/napari/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/napari/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/napari/test/napari_viewer_info_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:54:06.644058 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/omega_plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/omega_plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/omega_plugins/discover_omega_plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:54:06.644058 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/omega_plugins/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/omega_plugins/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/omega_plugins/test/discover_omega_plugins_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:54:06.648058 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/python/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/python/conda_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/python/dynamic_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/python/exception_description.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/python/exception_guard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7704 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/python/fix_bad_fun_calls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6032 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/python/fix_code_given_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/python/installed_packages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/python/missing_packages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3938 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/python/pip_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12403 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/python/python_lang_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5444 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/python/required_imports.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:54:06.652058 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/python/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/python/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/python/test/dynamic_import_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/python/test/exception_description_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/python/test/exception_guard_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/python/test/fix_bad_function_calls_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/python/test/fix_code_given_error_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/python/test/installed_packages_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/python/test/missing_libraries_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/python/test/python_lang_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/python/test/required_imports_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:54:06.652058 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/qt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/qt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4945 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/qt/download_file_qt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/qt/qt_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:54:06.656058 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/strings/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/strings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/strings/camel_case_to_normal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/strings/extract_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/strings/extract_urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/strings/filter_lines.py
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/strings/find_function_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/strings/find_integer_in_parenthesis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/strings/python_code_cleanup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:54:06.660058 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/strings/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/strings/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/strings/test/extract_code_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/strings/test/extract_url_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/strings/test/filter_lines_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/strings/test/find_function_name_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/strings/test/find_integer_in_parenthesis_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:54:06.660058 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/system/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/system/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/system/folders.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:54:06.660058 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/web/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/web/duckduckgo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/web/google.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/web/headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/web/metasearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3442 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/web/scrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:54:06.660058 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/web/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/web/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/web/test/duckduckgo_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/web/test/google_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/web/test/metasearch_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/web/test/scrapper_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/web/test/wikipedia_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/web/wikipedia.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:54:06.588058 napari-chatgpt-2023.7.7/src/napari_chatgpt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    22104 2023-07-07 20:54:06.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10056 2023-07-07 20:54:06.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 20:54:06.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-07 20:54:06.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-07-07 20:54:06.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-07 20:54:06.000000 napari-chatgpt-2023.7.7/src/napari_chatgpt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-07-07 20:53:37.000000 napari-chatgpt-2023.7.7/tox.ini
```

### Comparing `napari-chatgpt-2023.7.21/.github/workflows/just_deploy.yml` & `napari-chatgpt-2023.7.7/.github/workflows/just_deploy.yml`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.7.21/.github/workflows/test_and_deploy.yml` & `napari-chatgpt-2023.7.7/.github/workflows/test_and_deploy.yml`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 jobs:
   test:
     name: ${{ matrix.platform }} py${{ matrix.python-version }}
     runs-on: ${{ matrix.platform }}
     strategy:
       matrix:
         platform: [ ubuntu-latest, windows-latest, macos-latest ]
-        python-version: [ '3.9', '3.10', '3.11' ]
+        python-version: [ '3.8', '3.9', '3.10' ]
 
     steps:
       - uses: actions/checkout@v3
 
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v4
         with:
```

### Comparing `napari-chatgpt-2023.7.21/.gitignore` & `napari-chatgpt-2023.7.7/.gitignore`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.7.21/.napari-hub/config.yml` & `napari-chatgpt-2023.7.7/.napari-hub/config.yml`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.7.21/.pre-commit-config.yaml` & `napari-chatgpt-2023.7.7/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.7.21/LICENSE` & `napari-chatgpt-2023.7.7/LICENSE`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.7.21/PKG-INFO` & `napari-chatgpt-2023.7.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-chatgpt
-Version: 2023.7.21
+Version: 2023.7.7
 Summary: A napari plugin to process and analyse images with chatGPT.
 Home-page: https://github.com/royerlab/napari-chatgpt
 Author: Loic A. Royer
 Author-email: royerloic@gmail.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/royerlab/napari-chatgpt/issues
 Project-URL: Documentation, https://github.com/royerlab/napari-chatgpt#README.md
@@ -18,15 +18,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Image Processing
-Requires-Python: >=3.9
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: testing
 License-File: LICENSE
 
 # napari-chatgpt
 
 ## Home of
```

### Comparing `napari-chatgpt-2023.7.21/README.md` & `napari-chatgpt-2023.7.7/README.md`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.7.21/setup.cfg` & `napari-chatgpt-2023.7.7/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -30,19 +30,18 @@
 [options]
 packages = find:
 install_requires = 
 	numpy
 	magicgui
 	scikit-image
 	qtpy
-	langchain==0.0.235
+	langchain==0.0.208
 	fastapi
 	uvicorn
 	websockets
-	anthropic
 	openai
 	tiktoken
 	wikipedia
 	lxml
 	gTTS
 	playsound
 	matplotlib
@@ -54,15 +53,15 @@
 	scikit-video
 	pygpt4all==1.1.0
 	GoogleBard==1.0.2
 	transformers
 	cryptography
 	tabulate
 	numba
-python_requires = >=3.9
+python_requires = >=3.8
 include_package_data = True
 package_dir = 
 	=src
 setup_requires = setuptools_scm
 
 [options.packages.find]
 where = src
```

### Comparing `napari-chatgpt-2023.7.21/src/napari_chatgpt/_sandbox/beautiful_soup_demo.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/_sandbox/beautiful_soup_demo.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.7.21/src/napari_chatgpt/_sandbox/conv_agent_demo.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/_sandbox/conv_agent_demo.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.7.21/src/napari_chatgpt/_sandbox/enumerate_functions.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/_sandbox/enumerate_functions.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.7.21/src/napari_chatgpt/_sandbox/gpt4all_demo.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/_sandbox/gpt4all_demo.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.7.21/src/napari_chatgpt/_sandbox/lanchain_openai.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/_sandbox/lanchain_openai.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.7.21/src/napari_chatgpt/_sandbox/playwright_sandbox.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/_sandbox/playwright_sandbox.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.7.21/src/napari_chatgpt/_sandbox/speech_recognition_demo.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/_sandbox/speech_recognition_demo.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.7.21/src/napari_chatgpt/_sandbox/terminal.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/_sandbox/terminal.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.7.21/src/napari_chatgpt/_sandbox/test.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/_sandbox/test.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.7.21/src/napari_chatgpt/_sandbox/tts_demo.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/_sandbox/tts_demo.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.7.21/src/napari_chatgpt/_sandbox/whisper_cpp.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/_sandbox/whisper_cpp.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.7.21/src/napari_chatgpt/_tests/test_widget.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/_tests/test_widget.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.7.21/src/napari_chatgpt/_widget.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/_widget.py`

 * *Files 3% similar despite different names*

```diff
@@ -98,16 +98,22 @@
                     self.model_combo_box.addItem(model_id)
 
         # if is_package_installed('googlebard'):
         self.model_combo_box.addItem('bard')
 
         if is_package_installed('anthropic'):
             # Add Anthropic models to the combo box:
-            self.model_combo_box.addItem('claude-2')
-            self.model_combo_box.addItem('claude-instant-1')
+            self.model_combo_box.addItem('claude-v1')
+            self.model_combo_box.addItem('claude-v1-100k')
+            self.model_combo_box.addItem('claude-instant-v1')
+            self.model_combo_box.addItem('claude-instant-v1-100k')
+            self.model_combo_box.addItem('claude-v1.3')
+            self.model_combo_box.addItem('claude-v1.3-100k')
+            self.model_combo_box.addItem('claude-instant-v1.1')
+            self.model_combo_box.addItem('claude-instant-v1.1-100k')
 
         if is_package_installed('pygpt4all'):
             self.model_combo_box.addItem('ggml-mpt-7b-chat')
             self.model_combo_box.addItem('ggml-gpt4all-j-v1.3-groovy')
             self.model_combo_box.addItem('ggml-gpt4all-l13b-snoozy')
 
         # Connect the activated signal to a slot
```

### Comparing `napari-chatgpt-2023.7.21/src/napari_chatgpt/chat_server/callbacks/callbacks_handle_chat.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/chat_server/callbacks/callbacks_handle_chat.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.7.21/src/napari_chatgpt/chat_server/callbacks/callbacks_handler_tool.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/chat_server/callbacks/callbacks_handler_tool.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.7.21/src/napari_chatgpt/chat_server/callbacks/callbacks_stdout.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/chat_server/callbacks/callbacks_stdout.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.7.21/src/napari_chatgpt/chat_server/chat_server.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/chat_server/chat_server.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.7.21/src/napari_chatgpt/chat_server/static/_tailwind.css` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/chat_server/static/_tailwind.css`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.7.21/src/napari_chatgpt/chat_server/static/chat.js` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/chat_server/static/chat.js`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.7.21/src/napari_chatgpt/chat_server/static/marked-highlight.js` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/chat_server/static/marked-highlight.js`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.7.21/src/napari_chatgpt/chat_server/static/prism.css` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/chat_server/static/prism.css`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.7.21/src/napari_chatgpt/chat_server/static/prism.js` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/chat_server/static/prism.js`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.7.21/src/napari_chatgpt/chat_server/static/sunlight-min.js` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/chat_server/static/sunlight-min.js`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.7.21/src/napari_chatgpt/chat_server/static/sunlight.dark.css` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/chat_server/static/sunlight.dark.css`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.7.21/src/napari_chatgpt/chat_server/static/sunlight.python-min.js` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/chat_server/static/sunlight.python-min.js`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.7.21/src/napari_chatgpt/chat_server/static/tailwind.min.css` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/chat_server/static/tailwind.min.css`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.7.21/src/napari_chatgpt/chat_server/templates/index.html` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/chat_server/templates/index.html`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.7.21/src/napari_chatgpt/llm/bard.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/llm/bard.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.7.21/src/napari_chatgpt/llm/gpt4all.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/llm/gpt4all.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.7.21/src/napari_chatgpt/llm/llms.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/llm/llms.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.7.21/src/napari_chatgpt/omega/memory/memory.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/memory/memory.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.7.21/src/napari_chatgpt/omega/napari_bridge.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/napari_bridge.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.7.21/src/napari_chatgpt/omega/omega_agent/agent.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/omega_agent/agent.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.7.21/src/napari_chatgpt/omega/omega_agent/agent_output_parser.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/omega_agent/agent_output_parser.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.7.21/src/napari_chatgpt/omega/omega_agent/prompts.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/omega_agent/prompts.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.7.21/src/napari_chatgpt/omega/omega_agent/tests/agent_output_parser_tests.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/omega_agent/tests/agent_output_parser_tests.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.7.21/src/napari_chatgpt/omega/omega_init.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/omega_init.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.7.21/src/napari_chatgpt/omega/tools/async_base_tool.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/tools/async_base_tool.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.7.21/src/napari_chatgpt/omega/tools/demo/tools_demo.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/tools/demo/tools_demo.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.7.21/src/napari_chatgpt/omega/tools/examples/example_omega_tool.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/tools/examples/example_omega_tool.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.7.21/src/napari_chatgpt/omega/tools/instructions.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/tools/instructions.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.7.21/src/napari_chatgpt/omega/tools/napari/cell_nuclei_segmentation.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/tools/napari/cell_nuclei_segmentation.py`

 * *Files 1% similar despite different names*

```diff
@@ -191,15 +191,15 @@
     # generic_codegen_instructions: str = ''
 
     def _run_code(self, request: str, code: str, viewer: Viewer) -> str:
 
         try:
             with asection(f"CellNucleiSegmentationTool: query= {request} "):
                 # prepare code:
-                code = super()._prepare_code(code, do_fix_bad_calls=self.fix_bad_calls)
+                code = super()._prepare_code(code)
 
                 # lower case code:
                 code_lower = code.lower()
 
                 # Pick the right segmentation code:
                 if 'cellpose_segmentation(' in code_lower:
                     segmentation_code = _get_delegated_code('cellpose')
```

### Comparing `napari-chatgpt-2023.7.21/src/napari_chatgpt/omega/tools/napari/delegated_code/aydin_classic.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/tools/napari/delegated_code/aydin_classic.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.7.21/src/napari_chatgpt/omega/tools/napari/delegated_code/aydin_fgr.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/tools/napari/delegated_code/aydin_fgr.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.7.21/src/napari_chatgpt/omega/tools/napari/delegated_code/cellpose.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/tools/napari/delegated_code/cellpose.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.7.21/src/napari_chatgpt/omega/tools/napari/delegated_code/classic.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/tools/napari/delegated_code/classic.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.7.21/src/napari_chatgpt/omega/tools/napari/delegated_code/stardist.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/tools/napari/delegated_code/stardist.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.7.21/src/napari_chatgpt/omega/tools/napari/file_open_tool.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/tools/napari/file_open_tool.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.7.21/src/napari_chatgpt/omega/tools/napari/image_denoising.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/tools/napari/image_denoising.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,15 +108,15 @@
     # generic_codegen_instructions: str = ''
 
     def _run_code(self, request: str, code: str, viewer: Viewer) -> str:
 
         try:
             with asection(f"ImageDenoisingTool: query= {request} "):
                 # prepare code:
-                code = super()._prepare_code(code, do_fix_bad_calls=self.fix_bad_calls)
+                code = super()._prepare_code(code)
 
                 # lower case code:
                 code_lower = code.lower()
 
                 # Pick the right denoising code:
                 if 'aydin_classic_denoising(' in code_lower:
                     install_aydin()
```

### Comparing `napari-chatgpt-2023.7.21/src/napari_chatgpt/omega/tools/napari/napari_base_tool.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/tools/napari/napari_base_tool.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.7.21/src/napari_chatgpt/omega/tools/napari/viewer_control_tool.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/tools/napari/viewer_control_tool.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 #
 # """
 
 _instructions = \
 """
 **Instructions specific to controlling the viewer:**
 - If you need to add images, labels, points, shapes, surfaces, tracks, vectors, or any other type of layer that is not stored as an array, you may need additional code to read files from disk or download from a URL.
-- Unless explicitly stated in the request, the result of operations on layers should be a new layer in napari and should not modify the existing layers.
+- Unless explicitly stated in the request, the result of operations on layers should be a new layer in napari and not modify the existing layers.
 - Convert image arrays to the float type before processing. Intermediate or local image arrays should be of type float. Constants like `np.full()`, `np.ones()`, `np.zeros()`, etc., should be floats (e.g., 1.0).
 - If the request mentions "this," "that," or "the image/layer," it most likely refers to the last added image/layer.
 - If you are unsure about the layer being referred to, assume it is the last layer of the type most appropriate for the request.
 - If the request mentions the 'selected image', it most likely refers to the active or selected image layer.
 - To get the selected layer use: viewer.layers.selection.active
 - Important: At the end of your code add a print statement that states clearly and concisely what has been, or not, achieved. 
 - Do not create a new instance of `napari.Viewer()`. Use the existing instance provided in the variable `viewer`.
@@ -84,15 +84,15 @@
 
     def _run_code(self, request: str, code: str, viewer: Viewer) -> str:
 
         try:
             with asection(f"NapariViewerControlTool: request= {request} "):
 
                 # Prepare code:
-                code = super()._prepare_code(code, do_fix_bad_calls=self.fix_bad_calls)
+                code = super()._prepare_code(code, do_fix_bad_calls=True)
 
                 captured_output = self._run_code_catch_errors_fix_and_try_again(code,
                                                                            viewer=viewer,
                                                                            instructions=self.instructions,
                                                                            )
 
                 # Message:
```

### Comparing `napari-chatgpt-2023.7.21/src/napari_chatgpt/omega/tools/napari/viewer_query_tool.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/tools/napari/viewer_query_tool.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,15 +68,15 @@
     save_last_generated_code = False
 
     def _run_code(self, query: str, code: str, viewer: Viewer) -> str:
 
         try:
             with asection(f"NapariViewerQueryTool: query= {query} "):
                 # prepare code:
-                code = super()._prepare_code(code, do_fix_bad_calls=self.fix_bad_calls)
+                code = super()._prepare_code(code, do_fix_bad_calls=True)
 
                 # Load the code as module:
                 loaded_module = dynamic_import(code)
 
                 # get the function:
                 query = getattr(loaded_module, 'query')
```

### Comparing `napari-chatgpt-2023.7.21/src/napari_chatgpt/omega/tools/napari/widget_maker_tool.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/tools/napari/widget_maker_tool.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,15 +120,15 @@
     def _run_code(self, query: str, code: str, viewer: Viewer) -> str:
 
         try:
 
             with asection(f"NapariWidgetMakerTool: query= {query} "):
 
                 # Prepare code:
-                code = super()._prepare_code(code, do_fix_bad_calls=self.fix_bad_calls)
+                code = super()._prepare_code(code)
 
                 # Extracts function name:
                 function_name = find_function_name(code)
 
                 # If the function exists:
                 if function_name:
```

### Comparing `napari-chatgpt-2023.7.21/src/napari_chatgpt/omega/tools/search/web_image_search_tool.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/tools/search/web_image_search_tool.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.7.21/src/napari_chatgpt/omega/tools/search/web_search_tool.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/tools/search/web_search_tool.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.7.21/src/napari_chatgpt/omega/tools/search/wikipedia_query_tool.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/tools/search/wikipedia_query_tool.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.7.21/src/napari_chatgpt/omega/tools/search/wikipedia_search_tool.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/tools/search/wikipedia_search_tool.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.7.21/src/napari_chatgpt/omega/tools/special/exception_catcher_tool.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/tools/special/exception_catcher_tool.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.7.21/src/napari_chatgpt/omega/tools/special/file_download_tool.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/tools/special/file_download_tool.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.7.21/src/napari_chatgpt/omega/tools/special/functions_info_tool.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/tools/special/functions_info_tool.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.7.21/src/napari_chatgpt/omega/tools/special/human_input_tool.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/tools/special/human_input_tool.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.7.21/src/napari_chatgpt/omega/tools/special/python_repl.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/omega/tools/special/python_repl.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/api_keys/api_key.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/api_keys/api_key.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/api_keys/api_key_vault.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/api_keys/api_key_vault.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/api_keys/api_key_vault_dialog.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/api_keys/api_key_vault_dialog.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/api_keys/api_key_vault_test.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/api_keys/api_key_vault_test.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/api_keys/demo/api_key_vault_dialog_demo.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/api_keys/demo/api_key_vault_dialog_demo.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/async_utils/run_async.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/async_utils/run_async.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/download/download_files.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/download/download_files.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/download/gpt4all.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/download/gpt4all.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/download/test/download_files_test.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/download/test/download_files_test.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/images/normalize.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/images/normalize.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/llm/summarizer.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/llm/summarizer.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/llm/test/summarizer_test.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/llm/test/summarizer_test.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/napari/napari_viewer_info.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/napari/napari_viewer_info.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/napari/open_in_napari.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/napari/open_in_napari.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/napari/test/napari_viewer_info_test.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/napari/test/napari_viewer_info_test.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/omega_plugins/discover_omega_plugins.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/omega_plugins/discover_omega_plugins.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/python/conda_utils.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/python/conda_utils.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/python/dynamic_import.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/python/dynamic_import.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/python/exception_description.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/python/exception_description.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/python/exception_guard.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/python/exception_guard.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/python/fix_bad_fun_calls.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/python/fix_bad_fun_calls.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/python/fix_code_given_error.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/python/fix_code_given_error.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/python/installed_packages.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/python/installed_packages.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/python/missing_packages.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/python/missing_packages.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/python/pip_utils.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/python/pip_utils.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/python/python_lang_utils.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/python/python_lang_utils.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/python/required_imports.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/python/required_imports.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/python/test/dynamic_import_test.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/python/test/dynamic_import_test.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/python/test/exception_description_test.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/python/test/exception_description_test.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/python/test/fix_bad_function_calls_test.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/python/test/fix_bad_function_calls_test.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/python/test/fix_code_given_error_test.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/python/test/fix_code_given_error_test.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/python/test/missing_libraries_test.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/python/test/missing_libraries_test.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/python/test/python_lang_utils_test.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/python/test/python_lang_utils_test.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/python/test/required_imports_test.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/python/test/required_imports_test.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/qt/download_file_qt.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/qt/download_file_qt.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/strings/camel_case_to_normal.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/strings/camel_case_to_normal.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/strings/extract_urls.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/strings/extract_urls.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/strings/filter_lines.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/strings/filter_lines.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/strings/find_integer_in_parenthesis.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/strings/find_integer_in_parenthesis.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/strings/python_code_cleanup.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/strings/python_code_cleanup.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/strings/test/extract_code_test.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/strings/test/extract_code_test.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/strings/test/filter_lines_test.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/strings/test/filter_lines_test.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/web/duckduckgo.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/web/duckduckgo.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/web/google.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/web/google.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/web/headers.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/web/headers.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/web/metasearch.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/web/metasearch.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/web/scrapper.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/web/scrapper.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/web/test/duckduckgo_test.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/web/test/duckduckgo_test.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/web/test/metasearch_test.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/web/test/metasearch_test.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/web/test/wikipedia_test.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/web/test/wikipedia_test.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.7.21/src/napari_chatgpt/utils/web/wikipedia.py` & `napari-chatgpt-2023.7.7/src/napari_chatgpt/utils/web/wikipedia.py`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.7.21/src/napari_chatgpt.egg-info/PKG-INFO` & `napari-chatgpt-2023.7.7/src/napari_chatgpt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-chatgpt
-Version: 2023.7.21
+Version: 2023.7.7
 Summary: A napari plugin to process and analyse images with chatGPT.
 Home-page: https://github.com/royerlab/napari-chatgpt
 Author: Loic A. Royer
 Author-email: royerloic@gmail.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/royerlab/napari-chatgpt/issues
 Project-URL: Documentation, https://github.com/royerlab/napari-chatgpt#README.md
@@ -18,15 +18,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Image Processing
-Requires-Python: >=3.9
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: testing
 License-File: LICENSE
 
 # napari-chatgpt
 
 ## Home of
```

### Comparing `napari-chatgpt-2023.7.21/src/napari_chatgpt.egg-info/SOURCES.txt` & `napari-chatgpt-2023.7.7/src/napari_chatgpt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `napari-chatgpt-2023.7.21/tox.ini` & `napari-chatgpt-2023.7.7/tox.ini`

 * *Files identical despite different names*

