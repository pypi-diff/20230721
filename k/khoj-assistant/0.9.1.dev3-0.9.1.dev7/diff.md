# Comparing `tmp/khoj_assistant-0.9.1.dev3.tar.gz` & `tmp/khoj_assistant-0.9.1.dev7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Fri Jul 21 06:24:08 2023, max compression
+gzip compressed data, last modified: Fri Jul 21 20:24:05 2023, max compression
```

## Comparing `khoj_assistant-0.9.1.dev3.tar` & `khoj_assistant-0.9.1.dev7.tar`

### file list

```diff
@@ -1,82 +1,82 @@
--rw-r--r--   0        0        0        0 2023-07-21 06:24:08.000000 khoj_assistant-0.9.1.dev3/src/khoj/__init__.py
--rw-r--r--   0        0        0    13771 2023-07-21 06:24:08.000000 khoj_assistant-0.9.1.dev3/src/khoj/configure.py
--rw-r--r--   0        0        0     5316 2023-07-21 06:24:08.000000 khoj_assistant-0.9.1.dev3/src/khoj/main.py
--rw-r--r--   0        0        0        0 2023-07-21 06:24:08.000000 khoj_assistant-0.9.1.dev3/src/khoj/interface/desktop/__init__.py
--rw-r--r--   0        0        0     2355 2023-07-21 06:24:08.000000 khoj_assistant-0.9.1.dev3/src/khoj/interface/desktop/main_window.py
--rw-r--r--   0        0        0     1397 2023-07-21 06:24:08.000000 khoj_assistant-0.9.1.dev3/src/khoj/interface/desktop/system_tray.py
--rw-r--r--   0        0        0      582 2023-07-21 06:24:08.000000 khoj_assistant-0.9.1.dev3/src/khoj/interface/web/404.html
--rw-r--r--   0        0        0     5144 2023-07-21 06:24:08.000000 khoj_assistant-0.9.1.dev3/src/khoj/interface/web/base_config.html
--rw-r--r--   0        0        0      657 2023-07-21 06:24:08.000000 khoj_assistant-0.9.1.dev3/src/khoj/interface/web/base_processor_integration.html
--rw-r--r--   0        0        0    18018 2023-07-21 06:24:08.000000 khoj_assistant-0.9.1.dev3/src/khoj/interface/web/chat.html
--rw-r--r--   0        0        0    19687 2023-07-21 06:24:08.000000 khoj_assistant-0.9.1.dev3/src/khoj/interface/web/config.html
--rw-r--r--   0        0        0     7089 2023-07-21 06:24:08.000000 khoj_assistant-0.9.1.dev3/src/khoj/interface/web/content_type_github_input.html
--rw-r--r--   0        0        0     7322 2023-07-21 06:24:08.000000 khoj_assistant-0.9.1.dev3/src/khoj/interface/web/content_type_input.html
--rw-r--r--   0        0        0     3560 2023-07-21 06:24:08.000000 khoj_assistant-0.9.1.dev3/src/khoj/interface/web/content_type_notion_input.html
--rw-r--r--   0        0        0    18924 2023-07-21 06:24:08.000000 khoj_assistant-0.9.1.dev3/src/khoj/interface/web/index.html
--rw-r--r--   0        0        0      402 2023-07-21 06:24:08.000000 khoj_assistant-0.9.1.dev3/src/khoj/interface/web/khoj.webmanifest
--rw-r--r--   0        0        0      418 2023-07-21 06:24:08.000000 khoj_assistant-0.9.1.dev3/src/khoj/interface/web/khoj_chat.webmanifest
--rw-r--r--   0        0        0     3660 2023-07-21 06:24:08.000000 khoj_assistant-0.9.1.dev3/src/khoj/interface/web/processor_conversation_input.html
--rw-r--r--   0        0        0     2433 2023-07-21 06:24:08.000000 khoj_assistant-0.9.1.dev3/src/khoj/interface/web/assets/khoj.css
--rw-r--r--   0        0        0   275822 2023-07-21 06:24:08.000000 khoj_assistant-0.9.1.dev3/src/khoj/interface/web/assets/markdown-it.min.js
--rw-r--r--   0        0        0    58643 2023-07-21 06:24:08.000000 khoj_assistant-0.9.1.dev3/src/khoj/interface/web/assets/org.min.js
--rw-r--r--   0        0        0    73572 2023-07-21 06:24:08.000000 khoj_assistant-0.9.1.dev3/src/khoj/interface/web/assets/pico.min.css
--rw-r--r--   0        0        0    51584 2023-07-21 06:24:08.000000 khoj_assistant-0.9.1.dev3/src/khoj/interface/web/assets/icons/chat.svg
--rw-r--r--   0        0        0      549 2023-07-21 06:24:08.000000 khoj_assistant-0.9.1.dev3/src/khoj/interface/web/assets/icons/confirm-icon.svg
--rw-r--r--   0        0        0   205167 2023-07-21 06:24:08.000000 khoj_assistant-0.9.1.dev3/src/khoj/interface/web/assets/icons/favicon-128x128.ico
--rw-r--r--   0        0        0    12518 2023-07-21 06:24:08.000000 khoj_assistant-0.9.1.dev3/src/khoj/interface/web/assets/icons/favicon-128x128.png
--rw-r--r--   0        0        0    31531 2023-07-21 06:24:08.000000 khoj_assistant-0.9.1.dev3/src/khoj/interface/web/assets/icons/favicon.icns
--rw-r--r--   0        0        0      964 2023-07-21 06:24:08.000000 khoj_assistant-0.9.1.dev3/src/khoj/interface/web/assets/icons/github.svg
--rw-r--r--   0        0        0    13011 2023-07-21 06:24:08.000000 khoj_assistant-0.9.1.dev3/src/khoj/interface/web/assets/icons/khoj-logo-sideways-200.png
--rw-r--r--   0        0        0  1301428 2023-07-21 06:24:08.000000 khoj_assistant-0.9.1.dev3/src/khoj/interface/web/assets/icons/khoj-logo-sideways.svg
--rw-r--r--   0        0        0     4031 2023-07-21 06:24:08.000000 khoj_assistant-0.9.1.dev3/src/khoj/interface/web/assets/icons/logotype.svg
--rw-r--r--   0        0        0      283 2023-07-21 06:24:08.000000 khoj_assistant-0.9.1.dev3/src/khoj/interface/web/assets/icons/markdown.svg
--rw-r--r--   0        0        0     1578 2023-07-21 06:24:08.000000 khoj_assistant-0.9.1.dev3/src/khoj/interface/web/assets/icons/notion.svg
--rw-r--r--   0        0        0     7946 2023-07-21 06:24:08.000000 khoj_assistant-0.9.1.dev3/src/khoj/interface/web/assets/icons/org.svg
--rw-r--r--   0        0        0     2504 2023-07-21 06:24:08.000000 khoj_assistant-0.9.1.dev3/src/khoj/interface/web/assets/icons/pdf.svg
--rw-r--r--   0        0        0     1877 2023-07-21 06:24:08.000000 khoj_assistant-0.9.1.dev3/src/khoj/interface/web/assets/icons/question-mark-icon.svg
--rw-r--r--   0        0        0        0 2023-07-21 06:24:08.000000 khoj_assistant-0.9.1.dev3/src/khoj/processor/__init__.py
--rw-r--r--   0        0        0     4788 2023-07-21 06:24:08.000000 khoj_assistant-0.9.1.dev3/src/khoj/processor/text_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-07-21 06:24:08.000000 khoj_assistant-0.9.1.dev3/src/khoj/processor/conversation/__init__.py
--rw-r--r--   0        0        0     4824 2023-07-21 06:24:08.000000 khoj_assistant-0.9.1.dev3/src/khoj/processor/conversation/gpt.py
--rw-r--r--   0        0        0     3991 2023-07-21 06:24:08.000000 khoj_assistant-0.9.1.dev3/src/khoj/processor/conversation/prompts.py
--rw-r--r--   0        0        0     8304 2023-07-21 06:24:08.000000 khoj_assistant-0.9.1.dev3/src/khoj/processor/conversation/utils.py
--rw-r--r--   0        0        0        0 2023-07-21 06:24:08.000000 khoj_assistant-0.9.1.dev3/src/khoj/processor/github/__init__.py
--rw-r--r--   0        0        0    13274 2023-07-21 06:24:08.000000 khoj_assistant-0.9.1.dev3/src/khoj/processor/github/github_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-07-21 06:24:08.000000 khoj_assistant-0.9.1.dev3/src/khoj/processor/jsonl/__init__.py
--rw-r--r--   0        0        0     3578 2023-07-21 06:24:08.000000 khoj_assistant-0.9.1.dev3/src/khoj/processor/jsonl/jsonl_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-07-21 06:24:08.000000 khoj_assistant-0.9.1.dev3/src/khoj/processor/markdown/__init__.py
--rw-r--r--   0        0        0     7156 2023-07-21 06:24:08.000000 khoj_assistant-0.9.1.dev3/src/khoj/processor/markdown/markdown_to_jsonl.py
--rw-r--r--   0        0        0     9578 2023-07-21 06:24:08.000000 khoj_assistant-0.9.1.dev3/src/khoj/processor/notion/notion_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-07-21 06:24:08.000000 khoj_assistant-0.9.1.dev3/src/khoj/processor/org_mode/__init__.py
--rw-r--r--   0        0        0     7190 2023-07-21 06:24:08.000000 khoj_assistant-0.9.1.dev3/src/khoj/processor/org_mode/org_to_jsonl.py
--rw-r--r--   0        0        0    16881 2023-07-21 06:24:08.000000 khoj_assistant-0.9.1.dev3/src/khoj/processor/org_mode/orgnode.py
--rw-r--r--   0        0        0        0 2023-07-21 06:24:08.000000 khoj_assistant-0.9.1.dev3/src/khoj/processor/pdf/__init__.py
--rw-r--r--   0        0        0     5099 2023-07-21 06:24:08.000000 khoj_assistant-0.9.1.dev3/src/khoj/processor/pdf/pdf_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-07-21 06:24:08.000000 khoj_assistant-0.9.1.dev3/src/khoj/routers/__init__.py
--rw-r--r--   0        0        0    23782 2023-07-21 06:24:08.000000 khoj_assistant-0.9.1.dev3/src/khoj/routers/api.py
--rw-r--r--   0        0        0      167 2023-07-21 06:24:08.000000 khoj_assistant-0.9.1.dev3/src/khoj/routers/api_beta.py
--rw-r--r--   0        0        0     3657 2023-07-21 06:24:08.000000 khoj_assistant-0.9.1.dev3/src/khoj/routers/helpers.py
--rw-r--r--   0        0        0     6674 2023-07-21 06:24:08.000000 khoj_assistant-0.9.1.dev3/src/khoj/routers/web_client.py
--rw-r--r--   0        0        0        0 2023-07-21 06:24:08.000000 khoj_assistant-0.9.1.dev3/src/khoj/search_filter/__init__.py
--rw-r--r--   0        0        0      539 2023-07-21 06:24:08.000000 khoj_assistant-0.9.1.dev3/src/khoj/search_filter/base_filter.py
--rw-r--r--   0        0        0     7566 2023-07-21 06:24:08.000000 khoj_assistant-0.9.1.dev3/src/khoj/search_filter/date_filter.py
--rw-r--r--   0        0        0     2844 2023-07-21 06:24:08.000000 khoj_assistant-0.9.1.dev3/src/khoj/search_filter/file_filter.py
--rw-r--r--   0        0        0     3770 2023-07-21 06:24:08.000000 khoj_assistant-0.9.1.dev3/src/khoj/search_filter/word_filter.py
--rw-r--r--   0        0        0        0 2023-07-21 06:24:08.000000 khoj_assistant-0.9.1.dev3/src/khoj/search_type/__init__.py
--rw-r--r--   0        0        0    11434 2023-07-21 06:24:08.000000 khoj_assistant-0.9.1.dev3/src/khoj/search_type/image_search.py
--rw-r--r--   0        0        0    11134 2023-07-21 06:24:08.000000 khoj_assistant-0.9.1.dev3/src/khoj/search_type/text_search.py
--rw-r--r--   0        0        0        0 2023-07-21 06:24:08.000000 khoj_assistant-0.9.1.dev3/src/khoj/utils/__init__.py
--rw-r--r--   0        0        0     2619 2023-07-21 06:24:08.000000 khoj_assistant-0.9.1.dev3/src/khoj/utils/cli.py
--rw-r--r--   0        0        0     2303 2023-07-21 06:24:08.000000 khoj_assistant-0.9.1.dev3/src/khoj/utils/config.py
--rw-r--r--   0        0        0     2710 2023-07-21 06:24:08.000000 khoj_assistant-0.9.1.dev3/src/khoj/utils/constants.py
--rw-r--r--   0        0        0     6937 2023-07-21 06:24:08.000000 khoj_assistant-0.9.1.dev3/src/khoj/utils/helpers.py
--rw-r--r--   0        0        0     1233 2023-07-21 06:24:08.000000 khoj_assistant-0.9.1.dev3/src/khoj/utils/jsonl.py
--rw-r--r--   0        0        0     2463 2023-07-21 06:24:08.000000 khoj_assistant-0.9.1.dev3/src/khoj/utils/models.py
--rw-r--r--   0        0        0     4393 2023-07-21 06:24:08.000000 khoj_assistant-0.9.1.dev3/src/khoj/utils/rawconfig.py
--rw-r--r--   0        0        0     1113 2023-07-21 06:24:08.000000 khoj_assistant-0.9.1.dev3/src/khoj/utils/state.py
--rw-r--r--   0        0        0     1486 2023-07-21 06:24:08.000000 khoj_assistant-0.9.1.dev3/src/khoj/utils/yaml.py
--rw-r--r--   0        0        0      523 2023-07-21 06:24:08.000000 khoj_assistant-0.9.1.dev3/.gitignore
--rw-r--r--   0        0        0    32472 2023-07-21 06:24:08.000000 khoj_assistant-0.9.1.dev3/LICENSE
--rw-r--r--   0        0        0    24864 2023-07-21 06:24:08.000000 khoj_assistant-0.9.1.dev3/README.md
--rw-r--r--   0        0        0     2794 2023-07-21 06:24:08.000000 khoj_assistant-0.9.1.dev3/pyproject.toml
--rw-r--r--   0        0        0    27230 2023-07-21 06:24:08.000000 khoj_assistant-0.9.1.dev3/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-21 20:24:05.000000 khoj_assistant-0.9.1.dev7/src/khoj/__init__.py
+-rw-r--r--   0        0        0    13771 2023-07-21 20:24:05.000000 khoj_assistant-0.9.1.dev7/src/khoj/configure.py
+-rw-r--r--   0        0        0     5316 2023-07-21 20:24:05.000000 khoj_assistant-0.9.1.dev7/src/khoj/main.py
+-rw-r--r--   0        0        0        0 2023-07-21 20:24:05.000000 khoj_assistant-0.9.1.dev7/src/khoj/interface/desktop/__init__.py
+-rw-r--r--   0        0        0     2355 2023-07-21 20:24:05.000000 khoj_assistant-0.9.1.dev7/src/khoj/interface/desktop/main_window.py
+-rw-r--r--   0        0        0     1397 2023-07-21 20:24:05.000000 khoj_assistant-0.9.1.dev7/src/khoj/interface/desktop/system_tray.py
+-rw-r--r--   0        0        0      582 2023-07-21 20:24:05.000000 khoj_assistant-0.9.1.dev7/src/khoj/interface/web/404.html
+-rw-r--r--   0        0        0     5144 2023-07-21 20:24:05.000000 khoj_assistant-0.9.1.dev7/src/khoj/interface/web/base_config.html
+-rw-r--r--   0        0        0      657 2023-07-21 20:24:05.000000 khoj_assistant-0.9.1.dev7/src/khoj/interface/web/base_processor_integration.html
+-rw-r--r--   0        0        0    18018 2023-07-21 20:24:05.000000 khoj_assistant-0.9.1.dev7/src/khoj/interface/web/chat.html
+-rw-r--r--   0        0        0    19687 2023-07-21 20:24:05.000000 khoj_assistant-0.9.1.dev7/src/khoj/interface/web/config.html
+-rw-r--r--   0        0        0     7089 2023-07-21 20:24:05.000000 khoj_assistant-0.9.1.dev7/src/khoj/interface/web/content_type_github_input.html
+-rw-r--r--   0        0        0     7322 2023-07-21 20:24:05.000000 khoj_assistant-0.9.1.dev7/src/khoj/interface/web/content_type_input.html
+-rw-r--r--   0        0        0     3560 2023-07-21 20:24:05.000000 khoj_assistant-0.9.1.dev7/src/khoj/interface/web/content_type_notion_input.html
+-rw-r--r--   0        0        0    18924 2023-07-21 20:24:05.000000 khoj_assistant-0.9.1.dev7/src/khoj/interface/web/index.html
+-rw-r--r--   0        0        0      402 2023-07-21 20:24:05.000000 khoj_assistant-0.9.1.dev7/src/khoj/interface/web/khoj.webmanifest
+-rw-r--r--   0        0        0      418 2023-07-21 20:24:05.000000 khoj_assistant-0.9.1.dev7/src/khoj/interface/web/khoj_chat.webmanifest
+-rw-r--r--   0        0        0     3660 2023-07-21 20:24:05.000000 khoj_assistant-0.9.1.dev7/src/khoj/interface/web/processor_conversation_input.html
+-rw-r--r--   0        0        0     2433 2023-07-21 20:24:05.000000 khoj_assistant-0.9.1.dev7/src/khoj/interface/web/assets/khoj.css
+-rw-r--r--   0        0        0   275822 2023-07-21 20:24:05.000000 khoj_assistant-0.9.1.dev7/src/khoj/interface/web/assets/markdown-it.min.js
+-rw-r--r--   0        0        0    58643 2023-07-21 20:24:05.000000 khoj_assistant-0.9.1.dev7/src/khoj/interface/web/assets/org.min.js
+-rw-r--r--   0        0        0    73572 2023-07-21 20:24:05.000000 khoj_assistant-0.9.1.dev7/src/khoj/interface/web/assets/pico.min.css
+-rw-r--r--   0        0        0    51584 2023-07-21 20:24:05.000000 khoj_assistant-0.9.1.dev7/src/khoj/interface/web/assets/icons/chat.svg
+-rw-r--r--   0        0        0      549 2023-07-21 20:24:05.000000 khoj_assistant-0.9.1.dev7/src/khoj/interface/web/assets/icons/confirm-icon.svg
+-rw-r--r--   0        0        0   205167 2023-07-21 20:24:05.000000 khoj_assistant-0.9.1.dev7/src/khoj/interface/web/assets/icons/favicon-128x128.ico
+-rw-r--r--   0        0        0    12518 2023-07-21 20:24:05.000000 khoj_assistant-0.9.1.dev7/src/khoj/interface/web/assets/icons/favicon-128x128.png
+-rw-r--r--   0        0        0    31531 2023-07-21 20:24:05.000000 khoj_assistant-0.9.1.dev7/src/khoj/interface/web/assets/icons/favicon.icns
+-rw-r--r--   0        0        0      964 2023-07-21 20:24:05.000000 khoj_assistant-0.9.1.dev7/src/khoj/interface/web/assets/icons/github.svg
+-rw-r--r--   0        0        0    13011 2023-07-21 20:24:05.000000 khoj_assistant-0.9.1.dev7/src/khoj/interface/web/assets/icons/khoj-logo-sideways-200.png
+-rw-r--r--   0        0        0  1301428 2023-07-21 20:24:05.000000 khoj_assistant-0.9.1.dev7/src/khoj/interface/web/assets/icons/khoj-logo-sideways.svg
+-rw-r--r--   0        0        0     4031 2023-07-21 20:24:05.000000 khoj_assistant-0.9.1.dev7/src/khoj/interface/web/assets/icons/logotype.svg
+-rw-r--r--   0        0        0      283 2023-07-21 20:24:05.000000 khoj_assistant-0.9.1.dev7/src/khoj/interface/web/assets/icons/markdown.svg
+-rw-r--r--   0        0        0     1578 2023-07-21 20:24:05.000000 khoj_assistant-0.9.1.dev7/src/khoj/interface/web/assets/icons/notion.svg
+-rw-r--r--   0        0        0     7946 2023-07-21 20:24:05.000000 khoj_assistant-0.9.1.dev7/src/khoj/interface/web/assets/icons/org.svg
+-rw-r--r--   0        0        0     2504 2023-07-21 20:24:05.000000 khoj_assistant-0.9.1.dev7/src/khoj/interface/web/assets/icons/pdf.svg
+-rw-r--r--   0        0        0     1877 2023-07-21 20:24:05.000000 khoj_assistant-0.9.1.dev7/src/khoj/interface/web/assets/icons/question-mark-icon.svg
+-rw-r--r--   0        0        0        0 2023-07-21 20:24:05.000000 khoj_assistant-0.9.1.dev7/src/khoj/processor/__init__.py
+-rw-r--r--   0        0        0     4788 2023-07-21 20:24:05.000000 khoj_assistant-0.9.1.dev7/src/khoj/processor/text_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-07-21 20:24:05.000000 khoj_assistant-0.9.1.dev7/src/khoj/processor/conversation/__init__.py
+-rw-r--r--   0        0        0     4824 2023-07-21 20:24:05.000000 khoj_assistant-0.9.1.dev7/src/khoj/processor/conversation/gpt.py
+-rw-r--r--   0        0        0     3991 2023-07-21 20:24:05.000000 khoj_assistant-0.9.1.dev7/src/khoj/processor/conversation/prompts.py
+-rw-r--r--   0        0        0     8304 2023-07-21 20:24:05.000000 khoj_assistant-0.9.1.dev7/src/khoj/processor/conversation/utils.py
+-rw-r--r--   0        0        0        0 2023-07-21 20:24:05.000000 khoj_assistant-0.9.1.dev7/src/khoj/processor/github/__init__.py
+-rw-r--r--   0        0        0    13139 2023-07-21 20:24:05.000000 khoj_assistant-0.9.1.dev7/src/khoj/processor/github/github_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-07-21 20:24:05.000000 khoj_assistant-0.9.1.dev7/src/khoj/processor/jsonl/__init__.py
+-rw-r--r--   0        0        0     3578 2023-07-21 20:24:05.000000 khoj_assistant-0.9.1.dev7/src/khoj/processor/jsonl/jsonl_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-07-21 20:24:05.000000 khoj_assistant-0.9.1.dev7/src/khoj/processor/markdown/__init__.py
+-rw-r--r--   0        0        0     7156 2023-07-21 20:24:05.000000 khoj_assistant-0.9.1.dev7/src/khoj/processor/markdown/markdown_to_jsonl.py
+-rw-r--r--   0        0        0     9578 2023-07-21 20:24:05.000000 khoj_assistant-0.9.1.dev7/src/khoj/processor/notion/notion_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-07-21 20:24:05.000000 khoj_assistant-0.9.1.dev7/src/khoj/processor/org_mode/__init__.py
+-rw-r--r--   0        0        0     7190 2023-07-21 20:24:05.000000 khoj_assistant-0.9.1.dev7/src/khoj/processor/org_mode/org_to_jsonl.py
+-rw-r--r--   0        0        0    16881 2023-07-21 20:24:05.000000 khoj_assistant-0.9.1.dev7/src/khoj/processor/org_mode/orgnode.py
+-rw-r--r--   0        0        0        0 2023-07-21 20:24:05.000000 khoj_assistant-0.9.1.dev7/src/khoj/processor/pdf/__init__.py
+-rw-r--r--   0        0        0     5099 2023-07-21 20:24:05.000000 khoj_assistant-0.9.1.dev7/src/khoj/processor/pdf/pdf_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-07-21 20:24:05.000000 khoj_assistant-0.9.1.dev7/src/khoj/routers/__init__.py
+-rw-r--r--   0        0        0    23782 2023-07-21 20:24:05.000000 khoj_assistant-0.9.1.dev7/src/khoj/routers/api.py
+-rw-r--r--   0        0        0      167 2023-07-21 20:24:05.000000 khoj_assistant-0.9.1.dev7/src/khoj/routers/api_beta.py
+-rw-r--r--   0        0        0     3657 2023-07-21 20:24:05.000000 khoj_assistant-0.9.1.dev7/src/khoj/routers/helpers.py
+-rw-r--r--   0        0        0     6674 2023-07-21 20:24:05.000000 khoj_assistant-0.9.1.dev7/src/khoj/routers/web_client.py
+-rw-r--r--   0        0        0        0 2023-07-21 20:24:05.000000 khoj_assistant-0.9.1.dev7/src/khoj/search_filter/__init__.py
+-rw-r--r--   0        0        0      539 2023-07-21 20:24:05.000000 khoj_assistant-0.9.1.dev7/src/khoj/search_filter/base_filter.py
+-rw-r--r--   0        0        0     7566 2023-07-21 20:24:05.000000 khoj_assistant-0.9.1.dev7/src/khoj/search_filter/date_filter.py
+-rw-r--r--   0        0        0     2844 2023-07-21 20:24:05.000000 khoj_assistant-0.9.1.dev7/src/khoj/search_filter/file_filter.py
+-rw-r--r--   0        0        0     3770 2023-07-21 20:24:05.000000 khoj_assistant-0.9.1.dev7/src/khoj/search_filter/word_filter.py
+-rw-r--r--   0        0        0        0 2023-07-21 20:24:05.000000 khoj_assistant-0.9.1.dev7/src/khoj/search_type/__init__.py
+-rw-r--r--   0        0        0    11434 2023-07-21 20:24:05.000000 khoj_assistant-0.9.1.dev7/src/khoj/search_type/image_search.py
+-rw-r--r--   0        0        0    11134 2023-07-21 20:24:05.000000 khoj_assistant-0.9.1.dev7/src/khoj/search_type/text_search.py
+-rw-r--r--   0        0        0        0 2023-07-21 20:24:05.000000 khoj_assistant-0.9.1.dev7/src/khoj/utils/__init__.py
+-rw-r--r--   0        0        0     2619 2023-07-21 20:24:05.000000 khoj_assistant-0.9.1.dev7/src/khoj/utils/cli.py
+-rw-r--r--   0        0        0     2303 2023-07-21 20:24:05.000000 khoj_assistant-0.9.1.dev7/src/khoj/utils/config.py
+-rw-r--r--   0        0        0     2710 2023-07-21 20:24:05.000000 khoj_assistant-0.9.1.dev7/src/khoj/utils/constants.py
+-rw-r--r--   0        0        0     6937 2023-07-21 20:24:05.000000 khoj_assistant-0.9.1.dev7/src/khoj/utils/helpers.py
+-rw-r--r--   0        0        0     1233 2023-07-21 20:24:05.000000 khoj_assistant-0.9.1.dev7/src/khoj/utils/jsonl.py
+-rw-r--r--   0        0        0     2463 2023-07-21 20:24:05.000000 khoj_assistant-0.9.1.dev7/src/khoj/utils/models.py
+-rw-r--r--   0        0        0     4393 2023-07-21 20:24:05.000000 khoj_assistant-0.9.1.dev7/src/khoj/utils/rawconfig.py
+-rw-r--r--   0        0        0     1113 2023-07-21 20:24:05.000000 khoj_assistant-0.9.1.dev7/src/khoj/utils/state.py
+-rw-r--r--   0        0        0     1486 2023-07-21 20:24:05.000000 khoj_assistant-0.9.1.dev7/src/khoj/utils/yaml.py
+-rw-r--r--   0        0        0      523 2023-07-21 20:24:05.000000 khoj_assistant-0.9.1.dev7/.gitignore
+-rw-r--r--   0        0        0    32472 2023-07-21 20:24:05.000000 khoj_assistant-0.9.1.dev7/LICENSE
+-rw-r--r--   0        0        0    24864 2023-07-21 20:24:05.000000 khoj_assistant-0.9.1.dev7/README.md
+-rw-r--r--   0        0        0     2794 2023-07-21 20:24:05.000000 khoj_assistant-0.9.1.dev7/pyproject.toml
+-rw-r--r--   0        0        0    27230 2023-07-21 20:24:05.000000 khoj_assistant-0.9.1.dev7/PKG-INFO
```

### Comparing `khoj_assistant-0.9.1.dev3/src/khoj/configure.py` & `khoj_assistant-0.9.1.dev7/src/khoj/configure.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.9.1.dev3/src/khoj/main.py` & `khoj_assistant-0.9.1.dev7/src/khoj/main.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.9.1.dev3/src/khoj/interface/desktop/main_window.py` & `khoj_assistant-0.9.1.dev7/src/khoj/interface/desktop/main_window.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.9.1.dev3/src/khoj/interface/desktop/system_tray.py` & `khoj_assistant-0.9.1.dev7/src/khoj/interface/desktop/system_tray.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.9.1.dev3/src/khoj/interface/web/404.html` & `khoj_assistant-0.9.1.dev7/src/khoj/interface/web/404.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.9.1.dev3/src/khoj/interface/web/base_config.html` & `khoj_assistant-0.9.1.dev7/src/khoj/interface/web/base_config.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.9.1.dev3/src/khoj/interface/web/base_processor_integration.html` & `khoj_assistant-0.9.1.dev7/src/khoj/interface/web/base_processor_integration.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.9.1.dev3/src/khoj/interface/web/chat.html` & `khoj_assistant-0.9.1.dev7/src/khoj/interface/web/chat.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.9.1.dev3/src/khoj/interface/web/config.html` & `khoj_assistant-0.9.1.dev7/src/khoj/interface/web/config.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.9.1.dev3/src/khoj/interface/web/content_type_github_input.html` & `khoj_assistant-0.9.1.dev7/src/khoj/interface/web/content_type_github_input.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.9.1.dev3/src/khoj/interface/web/content_type_input.html` & `khoj_assistant-0.9.1.dev7/src/khoj/interface/web/content_type_input.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.9.1.dev3/src/khoj/interface/web/content_type_notion_input.html` & `khoj_assistant-0.9.1.dev7/src/khoj/interface/web/content_type_notion_input.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.9.1.dev3/src/khoj/interface/web/index.html` & `khoj_assistant-0.9.1.dev7/src/khoj/interface/web/index.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.9.1.dev3/src/khoj/interface/web/processor_conversation_input.html` & `khoj_assistant-0.9.1.dev7/src/khoj/interface/web/processor_conversation_input.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.9.1.dev3/src/khoj/interface/web/assets/khoj.css` & `khoj_assistant-0.9.1.dev7/src/khoj/interface/web/assets/khoj.css`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.9.1.dev3/src/khoj/interface/web/assets/markdown-it.min.js` & `khoj_assistant-0.9.1.dev7/src/khoj/interface/web/assets/markdown-it.min.js`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.9.1.dev3/src/khoj/interface/web/assets/org.min.js` & `khoj_assistant-0.9.1.dev7/src/khoj/interface/web/assets/org.min.js`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.9.1.dev3/src/khoj/interface/web/assets/pico.min.css` & `khoj_assistant-0.9.1.dev7/src/khoj/interface/web/assets/pico.min.css`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.9.1.dev3/src/khoj/interface/web/assets/icons/chat.svg` & `khoj_assistant-0.9.1.dev7/src/khoj/interface/web/assets/icons/chat.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.9.1.dev3/src/khoj/interface/web/assets/icons/confirm-icon.svg` & `khoj_assistant-0.9.1.dev7/src/khoj/interface/web/assets/icons/confirm-icon.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.9.1.dev3/src/khoj/interface/web/assets/icons/favicon-128x128.ico` & `khoj_assistant-0.9.1.dev7/src/khoj/interface/web/assets/icons/favicon-128x128.ico`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.9.1.dev3/src/khoj/interface/web/assets/icons/favicon-128x128.png` & `khoj_assistant-0.9.1.dev7/src/khoj/interface/web/assets/icons/favicon-128x128.png`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.9.1.dev3/src/khoj/interface/web/assets/icons/favicon.icns` & `khoj_assistant-0.9.1.dev7/src/khoj/interface/web/assets/icons/favicon.icns`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.9.1.dev3/src/khoj/interface/web/assets/icons/github.svg` & `khoj_assistant-0.9.1.dev7/src/khoj/interface/web/assets/icons/github.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.9.1.dev3/src/khoj/interface/web/assets/icons/khoj-logo-sideways-200.png` & `khoj_assistant-0.9.1.dev7/src/khoj/interface/web/assets/icons/khoj-logo-sideways-200.png`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.9.1.dev3/src/khoj/interface/web/assets/icons/khoj-logo-sideways.svg` & `khoj_assistant-0.9.1.dev7/src/khoj/interface/web/assets/icons/khoj-logo-sideways.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.9.1.dev3/src/khoj/interface/web/assets/icons/logotype.svg` & `khoj_assistant-0.9.1.dev7/src/khoj/interface/web/assets/icons/logotype.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.9.1.dev3/src/khoj/interface/web/assets/icons/notion.svg` & `khoj_assistant-0.9.1.dev7/src/khoj/interface/web/assets/icons/notion.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.9.1.dev3/src/khoj/interface/web/assets/icons/org.svg` & `khoj_assistant-0.9.1.dev7/src/khoj/interface/web/assets/icons/org.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.9.1.dev3/src/khoj/interface/web/assets/icons/pdf.svg` & `khoj_assistant-0.9.1.dev7/src/khoj/interface/web/assets/icons/pdf.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.9.1.dev3/src/khoj/interface/web/assets/icons/question-mark-icon.svg` & `khoj_assistant-0.9.1.dev7/src/khoj/interface/web/assets/icons/question-mark-icon.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.9.1.dev3/src/khoj/processor/text_to_jsonl.py` & `khoj_assistant-0.9.1.dev7/src/khoj/processor/text_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.9.1.dev3/src/khoj/processor/conversation/gpt.py` & `khoj_assistant-0.9.1.dev7/src/khoj/processor/conversation/gpt.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.9.1.dev3/src/khoj/processor/conversation/prompts.py` & `khoj_assistant-0.9.1.dev7/src/khoj/processor/conversation/prompts.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.9.1.dev3/src/khoj/processor/conversation/utils.py` & `khoj_assistant-0.9.1.dev7/src/khoj/processor/conversation/utils.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.9.1.dev3/src/khoj/processor/github/github_to_jsonl.py` & `khoj_assistant-0.9.1.dev7/src/khoj/processor/github/github_to_jsonl.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,20 +80,17 @@
             current_entries = TextToJsonl.split_entries_by_max_tokens(current_entries, max_tokens=256)
 
         return current_entries
 
     def update_entries_with_ids(self, current_entries, previous_entries):
         # Identify, mark and merge any new entries with previous entries
         with timer("Identify new or updated entries", logger):
-            if not previous_entries:
-                entries_with_ids = list(enumerate(current_entries))
-            else:
-                entries_with_ids = TextToJsonl.mark_entries_for_update(
-                    current_entries, previous_entries, key="compiled", logger=logger
-                )
+            entries_with_ids = TextToJsonl.mark_entries_for_update(
+                current_entries, previous_entries, key="compiled", logger=logger
+            )
 
         with timer("Write github entries to JSONL file", logger):
             # Process Each Entry from All Notes Files
             entries = list(map(lambda entry: entry[1], entries_with_ids))
             jsonl_data = MarkdownToJsonl.convert_markdown_maps_to_jsonl(entries)
 
             # Compress JSONL formatted Data
```

### Comparing `khoj_assistant-0.9.1.dev3/src/khoj/processor/jsonl/jsonl_to_jsonl.py` & `khoj_assistant-0.9.1.dev7/src/khoj/processor/jsonl/jsonl_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.9.1.dev3/src/khoj/processor/markdown/markdown_to_jsonl.py` & `khoj_assistant-0.9.1.dev7/src/khoj/processor/markdown/markdown_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.9.1.dev3/src/khoj/processor/notion/notion_to_jsonl.py` & `khoj_assistant-0.9.1.dev7/src/khoj/processor/notion/notion_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.9.1.dev3/src/khoj/processor/org_mode/org_to_jsonl.py` & `khoj_assistant-0.9.1.dev7/src/khoj/processor/org_mode/org_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.9.1.dev3/src/khoj/processor/org_mode/orgnode.py` & `khoj_assistant-0.9.1.dev7/src/khoj/processor/org_mode/orgnode.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.9.1.dev3/src/khoj/processor/pdf/pdf_to_jsonl.py` & `khoj_assistant-0.9.1.dev7/src/khoj/processor/pdf/pdf_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.9.1.dev3/src/khoj/routers/api.py` & `khoj_assistant-0.9.1.dev7/src/khoj/routers/api.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.9.1.dev3/src/khoj/routers/helpers.py` & `khoj_assistant-0.9.1.dev7/src/khoj/routers/helpers.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.9.1.dev3/src/khoj/routers/web_client.py` & `khoj_assistant-0.9.1.dev7/src/khoj/routers/web_client.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.9.1.dev3/src/khoj/search_filter/base_filter.py` & `khoj_assistant-0.9.1.dev7/src/khoj/search_filter/base_filter.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.9.1.dev3/src/khoj/search_filter/date_filter.py` & `khoj_assistant-0.9.1.dev7/src/khoj/search_filter/date_filter.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.9.1.dev3/src/khoj/search_filter/file_filter.py` & `khoj_assistant-0.9.1.dev7/src/khoj/search_filter/file_filter.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.9.1.dev3/src/khoj/search_filter/word_filter.py` & `khoj_assistant-0.9.1.dev7/src/khoj/search_filter/word_filter.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.9.1.dev3/src/khoj/search_type/image_search.py` & `khoj_assistant-0.9.1.dev7/src/khoj/search_type/image_search.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.9.1.dev3/src/khoj/search_type/text_search.py` & `khoj_assistant-0.9.1.dev7/src/khoj/search_type/text_search.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.9.1.dev3/src/khoj/utils/cli.py` & `khoj_assistant-0.9.1.dev7/src/khoj/utils/cli.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.9.1.dev3/src/khoj/utils/config.py` & `khoj_assistant-0.9.1.dev7/src/khoj/utils/config.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.9.1.dev3/src/khoj/utils/constants.py` & `khoj_assistant-0.9.1.dev7/src/khoj/utils/constants.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.9.1.dev3/src/khoj/utils/helpers.py` & `khoj_assistant-0.9.1.dev7/src/khoj/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.9.1.dev3/src/khoj/utils/jsonl.py` & `khoj_assistant-0.9.1.dev7/src/khoj/utils/jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.9.1.dev3/src/khoj/utils/models.py` & `khoj_assistant-0.9.1.dev7/src/khoj/utils/models.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.9.1.dev3/src/khoj/utils/rawconfig.py` & `khoj_assistant-0.9.1.dev7/src/khoj/utils/rawconfig.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.9.1.dev3/src/khoj/utils/state.py` & `khoj_assistant-0.9.1.dev7/src/khoj/utils/state.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.9.1.dev3/src/khoj/utils/yaml.py` & `khoj_assistant-0.9.1.dev7/src/khoj/utils/yaml.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.9.1.dev3/.gitignore` & `khoj_assistant-0.9.1.dev7/.gitignore`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.9.1.dev3/LICENSE` & `khoj_assistant-0.9.1.dev7/LICENSE`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.9.1.dev3/README.md` & `khoj_assistant-0.9.1.dev7/README.md`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.9.1.dev3/pyproject.toml` & `khoj_assistant-0.9.1.dev7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.9.1.dev3/PKG-INFO` & `khoj_assistant-0.9.1.dev7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: khoj-assistant
-Version: 0.9.1.dev3
+Version: 0.9.1.dev7
 Summary: An AI personal assistant for your Digital Brain
 Project-URL: Homepage, https://github.com/khoj-ai/khoj#readme
 Project-URL: Issues, https://github.com/khoj-ai/khoj/issues
 Project-URL: Discussions, https://github.com/khoj-ai/khoj/discussions
 Project-URL: Releases, https://github.com/khoj-ai/khoj/releases
 Author: Debanjum Singh Solanky, Saba Imran
 License-Expression: GPL-3.0-or-later
```

