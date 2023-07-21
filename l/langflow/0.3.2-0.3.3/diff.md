# Comparing `tmp/langflow-0.3.2.tar.gz` & `tmp/langflow-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langflow-0.3.2.tar", max compression
+gzip compressed data, was "langflow-0.3.3.tar", max compression
```

## Comparing `langflow-0.3.2.tar` & `langflow-0.3.3.tar`

### file list

```diff
@@ -1,167 +1,167 @@
--rw-r--r--   0        0        0     1065 2023-07-20 14:32:51.199155 langflow-0.3.2/LICENSE
--rw-r--r--   0        0        0    15271 2023-07-20 14:32:51.199155 langflow-0.3.2/README.md
--rw-r--r--   0        0        0     2650 2023-07-20 14:32:51.619157 langflow-0.3.2/pyproject.toml
--rw-r--r--   0        0        0      453 2023-07-20 14:32:51.619157 langflow-0.3.2/src/backend/langflow/__init__.py
--rw-r--r--   0        0        0     9675 2023-07-20 14:32:51.619157 langflow-0.3.2/src/backend/langflow/__main__.py
--rw-r--r--   0        0        0       61 2023-07-20 14:32:51.619157 langflow-0.3.2/src/backend/langflow/api/__init__.py
--rw-r--r--   0        0        0      423 2023-07-20 14:32:51.619157 langflow-0.3.2/src/backend/langflow/api/router.py
--rw-r--r--   0        0        0     2105 2023-07-20 14:32:51.619157 langflow-0.3.2/src/backend/langflow/api/utils.py
--rw-r--r--   0        0        0      436 2023-07-20 14:32:51.619157 langflow-0.3.2/src/backend/langflow/api/v1/__init__.py
--rw-r--r--   0        0        0     4486 2023-07-20 14:32:51.619157 langflow-0.3.2/src/backend/langflow/api/v1/base.py
--rw-r--r--   0        0        0     4946 2023-07-20 14:32:51.619157 langflow-0.3.2/src/backend/langflow/api/v1/callback.py
--rw-r--r--   0        0        0     7210 2023-07-20 14:32:51.619157 langflow-0.3.2/src/backend/langflow/api/v1/chat.py
--rw-r--r--   0        0        0     2484 2023-07-20 14:32:51.619157 langflow-0.3.2/src/backend/langflow/api/v1/endpoints.py
--rw-r--r--   0        0        0     2691 2023-07-20 14:32:51.619157 langflow-0.3.2/src/backend/langflow/api/v1/flow_styles.py
--rw-r--r--   0        0        0     3868 2023-07-20 14:32:51.619157 langflow-0.3.2/src/backend/langflow/api/v1/flows.py
--rw-r--r--   0        0        0     2355 2023-07-20 14:32:51.619157 langflow-0.3.2/src/backend/langflow/api/v1/schemas.py
--rw-r--r--   0        0        0     4439 2023-07-20 14:32:51.619157 langflow-0.3.2/src/backend/langflow/api/v1/validate.py
--rw-r--r--   0        0        0      152 2023-07-20 14:32:51.619157 langflow-0.3.2/src/backend/langflow/cache/__init__.py
--rw-r--r--   0        0        0     1815 2023-07-20 14:32:51.619157 langflow-0.3.2/src/backend/langflow/cache/base.py
--rw-r--r--   0        0        0     4554 2023-07-20 14:32:51.619157 langflow-0.3.2/src/backend/langflow/cache/flow.py
--rw-r--r--   0        0        0     4481 2023-07-20 14:32:51.619157 langflow-0.3.2/src/backend/langflow/cache/manager.py
--rw-r--r--   0        0        0     5062 2023-07-20 14:32:51.619157 langflow-0.3.2/src/backend/langflow/cache/utils.py
--rw-r--r--   0        0        0        0 2023-07-20 14:32:51.619157 langflow-0.3.2/src/backend/langflow/chat/__init__.py
--rw-r--r--   0        0        0       45 2023-07-20 14:32:51.619157 langflow-0.3.2/src/backend/langflow/chat/config.py
--rw-r--r--   0        0        0     8451 2023-07-20 14:32:51.619157 langflow-0.3.2/src/backend/langflow/chat/manager.py
--rw-r--r--   0        0        0     1272 2023-07-20 14:32:51.619157 langflow-0.3.2/src/backend/langflow/chat/utils.py
--rw-r--r--   0        0        0    13303 2023-07-20 14:32:51.619157 langflow-0.3.2/src/backend/langflow/config.yaml
--rw-r--r--   0        0        0        0 2023-07-20 14:32:51.619157 langflow-0.3.2/src/backend/langflow/custom/__init__.py
--rw-r--r--   0        0        0     1609 2023-07-20 14:32:51.619157 langflow-0.3.2/src/backend/langflow/custom/customs.py
--rw-r--r--   0        0        0        0 2023-07-20 14:32:51.619157 langflow-0.3.2/src/backend/langflow/database/__init__.py
--rw-r--r--   0        0        0     1357 2023-07-20 14:32:51.619157 langflow-0.3.2/src/backend/langflow/database/base.py
--rw-r--r--   0        0        0        0 2023-07-20 14:32:51.619157 langflow-0.3.2/src/backend/langflow/database/models/__init__.py
--rw-r--r--   0        0        0      363 2023-07-20 14:32:51.619157 langflow-0.3.2/src/backend/langflow/database/models/base.py
--rw-r--r--   0        0        0     1705 2023-07-20 14:32:51.619157 langflow-0.3.2/src/backend/langflow/database/models/flow.py
--rw-r--r--   0        0        0      831 2023-07-20 14:32:51.619157 langflow-0.3.2/src/backend/langflow/database/models/flow_style.py
--rw-r--r--   0        0        0      889 2023-07-20 14:34:07.715709 langflow-0.3.2/src/backend/langflow/frontend/assets/Facebook_Messenger_logo_2020-d4e5cbf1.svg
--rw-r--r--   0        0        0     3513 2023-07-20 14:34:07.715709 langflow-0.3.2/src/backend/langflow/frontend/assets/Midjourney_Emblem-3952311f.svg
--rw-r--r--   0        0        0     1578 2023-07-20 14:34:07.715709 langflow-0.3.2/src/backend/langflow/frontend/assets/Notion-logo-1b52a185.svg
--rw-r--r--   0        0        0     1705 2023-07-20 14:34:07.715709 langflow-0.3.2/src/backend/langflow/frontend/assets/QDrant-517d22b4.svg
--rw-r--r--   0        0        0     7249 2023-07-20 14:34:07.715709 langflow-0.3.2/src/backend/langflow/frontend/assets/Searx_logo-24248044.svg
--rw-r--r--   0        0        0     1106 2023-07-20 14:34:07.715709 langflow-0.3.2/src/backend/langflow/frontend/assets/Y_Combinator_logo-7356d194.svg
--rw-r--r--   0        0        0     2007 2023-07-20 14:34:07.715709 langflow-0.3.2/src/backend/langflow/frontend/assets/airbyte-6aa3c5fa.svg
--rw-r--r--   0        0        0     2763 2023-07-20 14:34:07.715709 langflow-0.3.2/src/backend/langflow/frontend/assets/anthropic_box-60809508.svg
--rw-r--r--   0        0        0     6783 2023-07-20 14:34:07.715709 langflow-0.3.2/src/backend/langflow/frontend/assets/bing-60c0c591.svg
--rw-r--r--   0        0        0      622 2023-07-20 14:34:07.715709 langflow-0.3.2/src/backend/langflow/frontend/assets/chroma-65ceac37.svg
--rw-r--r--   0        0        0     1450 2023-07-20 14:34:07.715709 langflow-0.3.2/src/backend/langflow/frontend/assets/cohere-f09153b9.svg
--rw-r--r--   0        0        0     1667 2023-07-20 14:34:07.715709 langflow-0.3.2/src/backend/langflow/frontend/assets/evernote-icon-135bbfd8.svg
--rw-r--r--   0        0        0     1111 2023-07-20 14:34:07.715709 langflow-0.3.2/src/backend/langflow/frontend/assets/gitbook-svgrepo-com-8beecec7.svg
--rw-r--r--   0        0        0     1054 2023-07-20 14:34:07.715709 langflow-0.3.2/src/backend/langflow/frontend/assets/google-1d6becdc.svg
--rw-r--r--   0        0        0    35286 2023-07-20 14:34:07.715709 langflow-0.3.2/src/backend/langflow/frontend/assets/hf-logo-942cad1c.svg
--rw-r--r--   0        0        0      789 2023-07-20 14:34:07.715709 langflow-0.3.2/src/backend/langflow/frontend/assets/ifixit-seeklogo.com-6846f6e5.svg
--rw-r--r--   0        0        0   211965 2023-07-20 14:34:07.715709 langflow-0.3.2/src/backend/langflow/frontend/assets/index-592d2574.css
--rw-r--r--   0        0        0  4268148 2023-07-20 14:34:07.719709 langflow-0.3.2/src/backend/langflow/frontend/assets/index-9bb007a7.js
--rw-r--r--   0        0        0    23161 2023-07-20 14:34:07.715709 langflow-0.3.2/src/backend/langflow/frontend/assets/male-technologist-d2e7de57.png
--rw-r--r--   0        0        0     2212 2023-07-20 14:34:07.715709 langflow-0.3.2/src/backend/langflow/frontend/assets/meta-icon-fc8308c0.svg
--rw-r--r--   0        0        0     1182 2023-07-20 14:34:07.715709 langflow-0.3.2/src/backend/langflow/frontend/assets/mongodb-icon-64a21d47.svg
--rw-r--r--   0        0        0     2509 2023-07-20 14:34:07.715709 langflow-0.3.2/src/backend/langflow/frontend/assets/openAI-2c85883b.svg
--rw-r--r--   0        0        0     2604 2023-07-20 14:34:07.715709 langflow-0.3.2/src/backend/langflow/frontend/assets/pinecone_logo-411e417b.svg
--rw-r--r--   0        0        0    26806 2023-07-20 14:34:07.715709 langflow-0.3.2/src/backend/langflow/frontend/assets/robot-95e1b00d.png
--rw-r--r--   0        0        0     1539 2023-07-20 14:34:07.715709 langflow-0.3.2/src/backend/langflow/frontend/assets/slack-icon-32084c4a.svg
--rw-r--r--   0        0        0     3248 2023-07-20 14:34:07.715709 langflow-0.3.2/src/backend/langflow/frontend/assets/supabase-icon-bdc56c95.svg
--rw-r--r--   0        0        0     1867 2023-07-20 14:34:07.715709 langflow-0.3.2/src/backend/langflow/frontend/assets/vertex_ai-a23b625d.svg
--rw-r--r--   0        0        0     4310 2023-07-20 14:34:07.719709 langflow-0.3.2/src/backend/langflow/frontend/assets/web-vitals-60d3425a.js
--rw-r--r--   0        0        0   104188 2023-07-20 14:34:07.715709 langflow-0.3.2/src/backend/langflow/frontend/favicon.ico
--rw-r--r--   0        0        0      724 2023-07-20 14:34:07.719709 langflow-0.3.2/src/backend/langflow/frontend/index.html
--rw-r--r--   0        0        0      764 2023-07-20 14:32:51.619157 langflow-0.3.2/src/backend/langflow/graph/__init__.py
--rw-r--r--   0        0        0        0 2023-07-20 14:32:51.619157 langflow-0.3.2/src/backend/langflow/graph/edge/__init__.py
--rw-r--r--   0        0        0     2349 2023-07-20 14:32:51.619157 langflow-0.3.2/src/backend/langflow/graph/edge/base.py
--rw-r--r--   0        0        0        0 2023-07-20 14:32:51.619157 langflow-0.3.2/src/backend/langflow/graph/graph/__init__.py
--rw-r--r--   0        0        0     7802 2023-07-20 14:32:51.619157 langflow-0.3.2/src/backend/langflow/graph/graph/base.py
--rw-r--r--   0        0        0     2014 2023-07-20 14:32:51.619157 langflow-0.3.2/src/backend/langflow/graph/graph/constants.py
--rw-r--r--   0        0        0        0 2023-07-20 14:32:51.619157 langflow-0.3.2/src/backend/langflow/graph/graph/utils.py
--rw-r--r--   0        0        0      642 2023-07-20 14:32:51.619157 langflow-0.3.2/src/backend/langflow/graph/utils.py
--rw-r--r--   0        0        0        0 2023-07-20 14:32:51.619157 langflow-0.3.2/src/backend/langflow/graph/vertex/__init__.py
--rw-r--r--   0        0        0     9589 2023-07-20 14:32:51.619157 langflow-0.3.2/src/backend/langflow/graph/vertex/base.py
--rw-r--r--   0        0        0        1 2023-07-20 14:32:51.619157 langflow-0.3.2/src/backend/langflow/graph/vertex/constants.py
--rw-r--r--   0        0        0     8205 2023-07-20 14:32:51.619157 langflow-0.3.2/src/backend/langflow/graph/vertex/types.py
--rw-r--r--   0        0        0        0 2023-07-20 14:32:51.619157 langflow-0.3.2/src/backend/langflow/interface/__init__.py
--rw-r--r--   0        0        0       84 2023-07-20 14:32:51.619157 langflow-0.3.2/src/backend/langflow/interface/agents/__init__.py
--rw-r--r--   0        0        0     2423 2023-07-20 14:32:51.619157 langflow-0.3.2/src/backend/langflow/interface/agents/base.py
--rw-r--r--   0        0        0    10224 2023-07-20 14:32:51.619157 langflow-0.3.2/src/backend/langflow/interface/agents/custom.py
--rw-r--r--   0        0        0     1447 2023-07-20 14:32:51.619157 langflow-0.3.2/src/backend/langflow/interface/agents/prebuilt.py
--rw-r--r--   0        0        0     4632 2023-07-20 14:32:51.619157 langflow-0.3.2/src/backend/langflow/interface/base.py
--rw-r--r--   0        0        0       84 2023-07-20 14:32:51.619157 langflow-0.3.2/src/backend/langflow/interface/chains/__init__.py
--rw-r--r--   0        0        0     2867 2023-07-20 14:32:51.619157 langflow-0.3.2/src/backend/langflow/interface/chains/base.py
--rw-r--r--   0        0        0     4843 2023-07-20 14:32:51.619157 langflow-0.3.2/src/backend/langflow/interface/chains/custom.py
--rw-r--r--   0        0        0     2306 2023-07-20 14:32:51.619157 langflow-0.3.2/src/backend/langflow/interface/custom_lists.py
--rw-r--r--   0        0        0        0 2023-07-20 14:32:51.619157 langflow-0.3.2/src/backend/langflow/interface/document_loaders/__init__.py
--rw-r--r--   0        0        0     1479 2023-07-20 14:32:51.619157 langflow-0.3.2/src/backend/langflow/interface/document_loaders/base.py
--rw-r--r--   0        0        0        0 2023-07-20 14:32:51.619157 langflow-0.3.2/src/backend/langflow/interface/embeddings/__init__.py
--rw-r--r--   0        0        0     1445 2023-07-20 14:32:51.619157 langflow-0.3.2/src/backend/langflow/interface/embeddings/base.py
--rw-r--r--   0        0        0      171 2023-07-20 14:32:51.619157 langflow-0.3.2/src/backend/langflow/interface/importing/__init__.py
--rw-r--r--   0        0        0     5625 2023-07-20 14:32:51.619157 langflow-0.3.2/src/backend/langflow/interface/importing/utils.py
--rw-r--r--   0        0        0        0 2023-07-20 14:32:51.619157 langflow-0.3.2/src/backend/langflow/interface/initialize/__init__.py
--rw-r--r--   0        0        0      385 2023-07-20 14:32:51.619157 langflow-0.3.2/src/backend/langflow/interface/initialize/llm.py
--rw-r--r--   0        0        0    20534 2023-07-20 14:32:51.619157 langflow-0.3.2/src/backend/langflow/interface/initialize/loading.py
--rw-r--r--   0        0        0     7704 2023-07-20 14:32:51.619157 langflow-0.3.2/src/backend/langflow/interface/initialize/vector_store.py
--rw-r--r--   0        0        0     1915 2023-07-20 14:32:51.619157 langflow-0.3.2/src/backend/langflow/interface/listing.py
--rw-r--r--   0        0        0       78 2023-07-20 14:32:51.619157 langflow-0.3.2/src/backend/langflow/interface/llms/__init__.py
--rw-r--r--   0        0        0     1355 2023-07-20 14:32:51.619157 langflow-0.3.2/src/backend/langflow/interface/llms/base.py
--rw-r--r--   0        0        0       88 2023-07-20 14:32:51.619157 langflow-0.3.2/src/backend/langflow/interface/memories/__init__.py
--rw-r--r--   0        0        0     2135 2023-07-20 14:32:51.619157 langflow-0.3.2/src/backend/langflow/interface/memories/base.py
--rw-r--r--   0        0        0        0 2023-07-20 14:32:51.623157 langflow-0.3.2/src/backend/langflow/interface/output_parsers/__init__.py
--rw-r--r--   0        0        0     2355 2023-07-20 14:32:51.623157 langflow-0.3.2/src/backend/langflow/interface/output_parsers/base.py
--rw-r--r--   0        0        0       87 2023-07-20 14:32:51.623157 langflow-0.3.2/src/backend/langflow/interface/prompts/__init__.py
--rw-r--r--   0        0        0     2459 2023-07-20 14:32:51.623157 langflow-0.3.2/src/backend/langflow/interface/prompts/base.py
--rw-r--r--   0        0        0     2483 2023-07-20 14:32:51.623157 langflow-0.3.2/src/backend/langflow/interface/prompts/custom.py
--rw-r--r--   0        0        0        0 2023-07-20 14:32:51.623157 langflow-0.3.2/src/backend/langflow/interface/retrievers/__init__.py
--rw-r--r--   0        0        0     2086 2023-07-20 14:32:51.623157 langflow-0.3.2/src/backend/langflow/interface/retrievers/base.py
--rw-r--r--   0        0        0     2764 2023-07-20 14:32:51.623157 langflow-0.3.2/src/backend/langflow/interface/run.py
--rw-r--r--   0        0        0      106 2023-07-20 14:32:51.623157 langflow-0.3.2/src/backend/langflow/interface/text_splitters/__init__.py
--rw-r--r--   0        0        0     1450 2023-07-20 14:32:51.623157 langflow-0.3.2/src/backend/langflow/interface/text_splitters/base.py
--rw-r--r--   0        0        0        0 2023-07-20 14:32:51.623157 langflow-0.3.2/src/backend/langflow/interface/toolkits/__init__.py
--rw-r--r--   0        0        0     2598 2023-07-20 14:32:51.623157 langflow-0.3.2/src/backend/langflow/interface/toolkits/base.py
--rw-r--r--   0        0        0        0 2023-07-20 14:32:51.623157 langflow-0.3.2/src/backend/langflow/interface/toolkits/custom.py
--rw-r--r--   0        0        0       81 2023-07-20 14:32:51.623157 langflow-0.3.2/src/backend/langflow/interface/tools/__init__.py
--rw-r--r--   0        0        0     5417 2023-07-20 14:32:51.623157 langflow-0.3.2/src/backend/langflow/interface/tools/base.py
--rw-r--r--   0        0        0      900 2023-07-20 14:32:51.623157 langflow-0.3.2/src/backend/langflow/interface/tools/constants.py
--rw-r--r--   0        0        0     1323 2023-07-20 14:32:51.623157 langflow-0.3.2/src/backend/langflow/interface/tools/custom.py
--rw-r--r--   0        0        0     4328 2023-07-20 14:32:51.623157 langflow-0.3.2/src/backend/langflow/interface/tools/util.py
--rw-r--r--   0        0        0     2063 2023-07-20 14:32:51.623157 langflow-0.3.2/src/backend/langflow/interface/types.py
--rw-r--r--   0        0        0        0 2023-07-20 14:32:51.623157 langflow-0.3.2/src/backend/langflow/interface/utilities/__init__.py
--rw-r--r--   0        0        0     2294 2023-07-20 14:32:51.623157 langflow-0.3.2/src/backend/langflow/interface/utilities/base.py
--rw-r--r--   0        0        0     2696 2023-07-20 14:32:51.623157 langflow-0.3.2/src/backend/langflow/interface/utils.py
--rw-r--r--   0        0        0        0 2023-07-20 14:32:51.623157 langflow-0.3.2/src/backend/langflow/interface/vector_store/__init__.py
--rw-r--r--   0        0        0     1813 2023-07-20 14:32:51.623157 langflow-0.3.2/src/backend/langflow/interface/vector_store/base.py
--rw-r--r--   0        0        0        0 2023-07-20 14:32:51.623157 langflow-0.3.2/src/backend/langflow/interface/wrappers/__init__.py
--rw-r--r--   0        0        0     1500 2023-07-20 14:32:51.623157 langflow-0.3.2/src/backend/langflow/interface/wrappers/base.py
--rw-r--r--   0        0        0       29 2023-07-20 14:32:51.623157 langflow-0.3.2/src/backend/langflow/jcloud.yml
--rw-r--r--   0        0        0      428 2023-07-20 14:32:51.623157 langflow-0.3.2/src/backend/langflow/lcserve.py
--rw-r--r--   0        0        0     2265 2023-07-20 14:32:51.623157 langflow-0.3.2/src/backend/langflow/main.py
--rw-r--r--   0        0        0        0 2023-07-20 14:32:51.623157 langflow-0.3.2/src/backend/langflow/processing/__init__.py
--rw-r--r--   0        0        0     1980 2023-07-20 14:32:51.623157 langflow-0.3.2/src/backend/langflow/processing/base.py
--rw-r--r--   0        0        0     8510 2023-07-20 14:32:51.623157 langflow-0.3.2/src/backend/langflow/processing/process.py
--rw-r--r--   0        0        0      579 2023-07-20 14:32:51.623157 langflow-0.3.2/src/backend/langflow/server.py
--rw-r--r--   0        0        0     3300 2023-07-20 14:32:51.623157 langflow-0.3.2/src/backend/langflow/settings.py
--rw-r--r--   0        0        0        0 2023-07-20 14:32:51.623157 langflow-0.3.2/src/backend/langflow/template/__init__.py
--rw-r--r--   0        0        0        0 2023-07-20 14:32:51.623157 langflow-0.3.2/src/backend/langflow/template/field/__init__.py
--rw-r--r--   0        0        0     1222 2023-07-20 14:32:51.623157 langflow-0.3.2/src/backend/langflow/template/field/base.py
--rw-r--r--   0        0        0      375 2023-07-20 14:32:51.623157 langflow-0.3.2/src/backend/langflow/template/frontend_node/__init__.py
--rw-r--r--   0        0        0     7032 2023-07-20 14:32:51.623157 langflow-0.3.2/src/backend/langflow/template/frontend_node/agents.py
--rw-r--r--   0        0        0     9742 2023-07-20 14:32:51.623157 langflow-0.3.2/src/backend/langflow/template/frontend_node/base.py
--rw-r--r--   0        0        0     7796 2023-07-20 14:32:51.623157 langflow-0.3.2/src/backend/langflow/template/frontend_node/chains.py
--rw-r--r--   0        0        0     1588 2023-07-20 14:32:51.623157 langflow-0.3.2/src/backend/langflow/template/frontend_node/constants.py
--rw-r--r--   0        0        0     8635 2023-07-20 14:32:51.623157 langflow-0.3.2/src/backend/langflow/template/frontend_node/documentloaders.py
--rw-r--r--   0        0        0     1680 2023-07-20 14:32:51.623157 langflow-0.3.2/src/backend/langflow/template/frontend_node/embeddings.py
--rw-r--r--   0        0        0        0 2023-07-20 14:32:51.623157 langflow-0.3.2/src/backend/langflow/template/frontend_node/formatter/__init__.py
--rw-r--r--   0        0        0      297 2023-07-20 14:32:51.623157 langflow-0.3.2/src/backend/langflow/template/frontend_node/formatter/base.py
--rw-r--r--   0        0        0     5569 2023-07-20 14:32:51.623157 langflow-0.3.2/src/backend/langflow/template/frontend_node/formatter/field_formatters.py
--rw-r--r--   0        0        0     5369 2023-07-20 14:32:51.623157 langflow-0.3.2/src/backend/langflow/template/frontend_node/llms.py
--rw-r--r--   0        0        0     6285 2023-07-20 14:32:51.623157 langflow-0.3.2/src/backend/langflow/template/frontend_node/memories.py
--rw-r--r--   0        0        0      364 2023-07-20 14:32:51.623157 langflow-0.3.2/src/backend/langflow/template/frontend_node/output_parsers.py
--rw-r--r--   0        0        0     3540 2023-07-20 14:32:51.623157 langflow-0.3.2/src/backend/langflow/template/frontend_node/prompts.py
--rw-r--r--   0        0        0      523 2023-07-20 14:32:51.623157 langflow-0.3.2/src/backend/langflow/template/frontend_node/retrievers.py
--rw-r--r--   0        0        0     2355 2023-07-20 14:32:51.623157 langflow-0.3.2/src/backend/langflow/template/frontend_node/textsplitters.py
--rw-r--r--   0        0        0     4007 2023-07-20 14:32:51.623157 langflow-0.3.2/src/backend/langflow/template/frontend_node/tools.py
--rw-r--r--   0        0        0      823 2023-07-20 14:32:51.623157 langflow-0.3.2/src/backend/langflow/template/frontend_node/utilities.py
--rw-r--r--   0        0        0     9428 2023-07-20 14:32:51.623157 langflow-0.3.2/src/backend/langflow/template/frontend_node/vectorstores.py
--rw-r--r--   0        0        0        0 2023-07-20 14:32:51.623157 langflow-0.3.2/src/backend/langflow/template/template/__init__.py
--rw-r--r--   0        0        0     1181 2023-07-20 14:32:51.623157 langflow-0.3.2/src/backend/langflow/template/template/base.py
--rw-r--r--   0        0        0        0 2023-07-20 14:32:51.623157 langflow-0.3.2/src/backend/langflow/utils/__init__.py
--rw-r--r--   0        0        0     1758 2023-07-20 14:32:51.623157 langflow-0.3.2/src/backend/langflow/utils/constants.py
--rw-r--r--   0        0        0      914 2023-07-20 14:32:51.623157 langflow-0.3.2/src/backend/langflow/utils/logger.py
--rw-r--r--   0        0        0     3169 2023-07-20 14:32:51.623157 langflow-0.3.2/src/backend/langflow/utils/payload.py
--rw-r--r--   0        0        0    11584 2023-07-20 14:32:51.623157 langflow-0.3.2/src/backend/langflow/utils/util.py
--rw-r--r--   0        0        0     5325 2023-07-20 14:32:51.623157 langflow-0.3.2/src/backend/langflow/utils/validate.py
--rw-r--r--   0        0        0    18152 1970-01-01 00:00:00.000000 langflow-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-07-21 21:05:36.817975 langflow-0.3.3/LICENSE
+-rw-r--r--   0        0        0    15271 2023-07-21 21:05:36.817975 langflow-0.3.3/README.md
+-rw-r--r--   0        0        0     2783 2023-07-21 21:05:37.217974 langflow-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0      453 2023-07-21 21:05:37.221974 langflow-0.3.3/src/backend/langflow/__init__.py
+-rw-r--r--   0        0        0     9675 2023-07-21 21:05:37.221974 langflow-0.3.3/src/backend/langflow/__main__.py
+-rw-r--r--   0        0        0       61 2023-07-21 21:05:37.221974 langflow-0.3.3/src/backend/langflow/api/__init__.py
+-rw-r--r--   0        0        0      423 2023-07-21 21:05:37.221974 langflow-0.3.3/src/backend/langflow/api/router.py
+-rw-r--r--   0        0        0     2105 2023-07-21 21:05:37.221974 langflow-0.3.3/src/backend/langflow/api/utils.py
+-rw-r--r--   0        0        0      436 2023-07-21 21:05:37.221974 langflow-0.3.3/src/backend/langflow/api/v1/__init__.py
+-rw-r--r--   0        0        0     4486 2023-07-21 21:05:37.221974 langflow-0.3.3/src/backend/langflow/api/v1/base.py
+-rw-r--r--   0        0        0     4946 2023-07-21 21:05:37.221974 langflow-0.3.3/src/backend/langflow/api/v1/callback.py
+-rw-r--r--   0        0        0     7210 2023-07-21 21:05:37.221974 langflow-0.3.3/src/backend/langflow/api/v1/chat.py
+-rw-r--r--   0        0        0     2484 2023-07-21 21:05:37.221974 langflow-0.3.3/src/backend/langflow/api/v1/endpoints.py
+-rw-r--r--   0        0        0     2691 2023-07-21 21:05:37.221974 langflow-0.3.3/src/backend/langflow/api/v1/flow_styles.py
+-rw-r--r--   0        0        0     3868 2023-07-21 21:05:37.221974 langflow-0.3.3/src/backend/langflow/api/v1/flows.py
+-rw-r--r--   0        0        0     2355 2023-07-21 21:05:37.221974 langflow-0.3.3/src/backend/langflow/api/v1/schemas.py
+-rw-r--r--   0        0        0     4439 2023-07-21 21:05:37.221974 langflow-0.3.3/src/backend/langflow/api/v1/validate.py
+-rw-r--r--   0        0        0      152 2023-07-21 21:05:37.221974 langflow-0.3.3/src/backend/langflow/cache/__init__.py
+-rw-r--r--   0        0        0     1815 2023-07-21 21:05:37.221974 langflow-0.3.3/src/backend/langflow/cache/base.py
+-rw-r--r--   0        0        0     4554 2023-07-21 21:05:37.221974 langflow-0.3.3/src/backend/langflow/cache/flow.py
+-rw-r--r--   0        0        0     4481 2023-07-21 21:05:37.221974 langflow-0.3.3/src/backend/langflow/cache/manager.py
+-rw-r--r--   0        0        0     5062 2023-07-21 21:05:37.221974 langflow-0.3.3/src/backend/langflow/cache/utils.py
+-rw-r--r--   0        0        0        0 2023-07-21 21:05:37.221974 langflow-0.3.3/src/backend/langflow/chat/__init__.py
+-rw-r--r--   0        0        0       45 2023-07-21 21:05:37.221974 langflow-0.3.3/src/backend/langflow/chat/config.py
+-rw-r--r--   0        0        0     8451 2023-07-21 21:05:37.221974 langflow-0.3.3/src/backend/langflow/chat/manager.py
+-rw-r--r--   0        0        0     1272 2023-07-21 21:05:37.221974 langflow-0.3.3/src/backend/langflow/chat/utils.py
+-rw-r--r--   0        0        0    13303 2023-07-21 21:05:37.221974 langflow-0.3.3/src/backend/langflow/config.yaml
+-rw-r--r--   0        0        0        0 2023-07-21 21:05:37.221974 langflow-0.3.3/src/backend/langflow/custom/__init__.py
+-rw-r--r--   0        0        0     1609 2023-07-21 21:05:37.221974 langflow-0.3.3/src/backend/langflow/custom/customs.py
+-rw-r--r--   0        0        0        0 2023-07-21 21:05:37.221974 langflow-0.3.3/src/backend/langflow/database/__init__.py
+-rw-r--r--   0        0        0     1357 2023-07-21 21:05:37.221974 langflow-0.3.3/src/backend/langflow/database/base.py
+-rw-r--r--   0        0        0        0 2023-07-21 21:05:37.221974 langflow-0.3.3/src/backend/langflow/database/models/__init__.py
+-rw-r--r--   0        0        0      363 2023-07-21 21:05:37.221974 langflow-0.3.3/src/backend/langflow/database/models/base.py
+-rw-r--r--   0        0        0     1705 2023-07-21 21:05:37.221974 langflow-0.3.3/src/backend/langflow/database/models/flow.py
+-rw-r--r--   0        0        0      831 2023-07-21 21:05:37.221974 langflow-0.3.3/src/backend/langflow/database/models/flow_style.py
+-rw-r--r--   0        0        0      889 2023-07-21 21:06:59.058208 langflow-0.3.3/src/backend/langflow/frontend/assets/Facebook_Messenger_logo_2020-d4e5cbf1.svg
+-rw-r--r--   0        0        0     3513 2023-07-21 21:06:59.058208 langflow-0.3.3/src/backend/langflow/frontend/assets/Midjourney_Emblem-3952311f.svg
+-rw-r--r--   0        0        0     1578 2023-07-21 21:06:59.058208 langflow-0.3.3/src/backend/langflow/frontend/assets/Notion-logo-1b52a185.svg
+-rw-r--r--   0        0        0     1705 2023-07-21 21:06:59.058208 langflow-0.3.3/src/backend/langflow/frontend/assets/QDrant-517d22b4.svg
+-rw-r--r--   0        0        0     7249 2023-07-21 21:06:59.058208 langflow-0.3.3/src/backend/langflow/frontend/assets/Searx_logo-24248044.svg
+-rw-r--r--   0        0        0     1106 2023-07-21 21:06:59.058208 langflow-0.3.3/src/backend/langflow/frontend/assets/Y_Combinator_logo-7356d194.svg
+-rw-r--r--   0        0        0     2007 2023-07-21 21:06:59.058208 langflow-0.3.3/src/backend/langflow/frontend/assets/airbyte-6aa3c5fa.svg
+-rw-r--r--   0        0        0     2763 2023-07-21 21:06:59.058208 langflow-0.3.3/src/backend/langflow/frontend/assets/anthropic_box-60809508.svg
+-rw-r--r--   0        0        0     6783 2023-07-21 21:06:59.058208 langflow-0.3.3/src/backend/langflow/frontend/assets/bing-60c0c591.svg
+-rw-r--r--   0        0        0      622 2023-07-21 21:06:59.058208 langflow-0.3.3/src/backend/langflow/frontend/assets/chroma-65ceac37.svg
+-rw-r--r--   0        0        0     1450 2023-07-21 21:06:59.058208 langflow-0.3.3/src/backend/langflow/frontend/assets/cohere-f09153b9.svg
+-rw-r--r--   0        0        0     1667 2023-07-21 21:06:59.058208 langflow-0.3.3/src/backend/langflow/frontend/assets/evernote-icon-135bbfd8.svg
+-rw-r--r--   0        0        0     1111 2023-07-21 21:06:59.058208 langflow-0.3.3/src/backend/langflow/frontend/assets/gitbook-svgrepo-com-8beecec7.svg
+-rw-r--r--   0        0        0     1054 2023-07-21 21:06:59.058208 langflow-0.3.3/src/backend/langflow/frontend/assets/google-1d6becdc.svg
+-rw-r--r--   0        0        0    35286 2023-07-21 21:06:59.058208 langflow-0.3.3/src/backend/langflow/frontend/assets/hf-logo-942cad1c.svg
+-rw-r--r--   0        0        0      789 2023-07-21 21:06:59.058208 langflow-0.3.3/src/backend/langflow/frontend/assets/ifixit-seeklogo.com-6846f6e5.svg
+-rw-r--r--   0        0        0   211965 2023-07-21 21:06:59.058208 langflow-0.3.3/src/backend/langflow/frontend/assets/index-592d2574.css
+-rw-r--r--   0        0        0  4268148 2023-07-21 21:06:59.062208 langflow-0.3.3/src/backend/langflow/frontend/assets/index-9bb007a7.js
+-rw-r--r--   0        0        0    23161 2023-07-21 21:06:59.058208 langflow-0.3.3/src/backend/langflow/frontend/assets/male-technologist-d2e7de57.png
+-rw-r--r--   0        0        0     2212 2023-07-21 21:06:59.058208 langflow-0.3.3/src/backend/langflow/frontend/assets/meta-icon-fc8308c0.svg
+-rw-r--r--   0        0        0     1182 2023-07-21 21:06:59.058208 langflow-0.3.3/src/backend/langflow/frontend/assets/mongodb-icon-64a21d47.svg
+-rw-r--r--   0        0        0     2509 2023-07-21 21:06:59.058208 langflow-0.3.3/src/backend/langflow/frontend/assets/openAI-2c85883b.svg
+-rw-r--r--   0        0        0     2604 2023-07-21 21:06:59.058208 langflow-0.3.3/src/backend/langflow/frontend/assets/pinecone_logo-411e417b.svg
+-rw-r--r--   0        0        0    26806 2023-07-21 21:06:59.058208 langflow-0.3.3/src/backend/langflow/frontend/assets/robot-95e1b00d.png
+-rw-r--r--   0        0        0     1539 2023-07-21 21:06:59.058208 langflow-0.3.3/src/backend/langflow/frontend/assets/slack-icon-32084c4a.svg
+-rw-r--r--   0        0        0     3248 2023-07-21 21:06:59.058208 langflow-0.3.3/src/backend/langflow/frontend/assets/supabase-icon-bdc56c95.svg
+-rw-r--r--   0        0        0     1867 2023-07-21 21:06:59.058208 langflow-0.3.3/src/backend/langflow/frontend/assets/vertex_ai-a23b625d.svg
+-rw-r--r--   0        0        0     4310 2023-07-21 21:06:59.058208 langflow-0.3.3/src/backend/langflow/frontend/assets/web-vitals-60d3425a.js
+-rw-r--r--   0        0        0   104188 2023-07-21 21:06:59.058208 langflow-0.3.3/src/backend/langflow/frontend/favicon.ico
+-rw-r--r--   0        0        0      724 2023-07-21 21:06:59.058208 langflow-0.3.3/src/backend/langflow/frontend/index.html
+-rw-r--r--   0        0        0      764 2023-07-21 21:05:37.221974 langflow-0.3.3/src/backend/langflow/graph/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-21 21:05:37.221974 langflow-0.3.3/src/backend/langflow/graph/edge/__init__.py
+-rw-r--r--   0        0        0     2349 2023-07-21 21:05:37.221974 langflow-0.3.3/src/backend/langflow/graph/edge/base.py
+-rw-r--r--   0        0        0        0 2023-07-21 21:05:37.221974 langflow-0.3.3/src/backend/langflow/graph/graph/__init__.py
+-rw-r--r--   0        0        0     7802 2023-07-21 21:05:37.221974 langflow-0.3.3/src/backend/langflow/graph/graph/base.py
+-rw-r--r--   0        0        0     2014 2023-07-21 21:05:37.221974 langflow-0.3.3/src/backend/langflow/graph/graph/constants.py
+-rw-r--r--   0        0        0        0 2023-07-21 21:05:37.221974 langflow-0.3.3/src/backend/langflow/graph/graph/utils.py
+-rw-r--r--   0        0        0      642 2023-07-21 21:05:37.221974 langflow-0.3.3/src/backend/langflow/graph/utils.py
+-rw-r--r--   0        0        0        0 2023-07-21 21:05:37.221974 langflow-0.3.3/src/backend/langflow/graph/vertex/__init__.py
+-rw-r--r--   0        0        0     9589 2023-07-21 21:05:37.221974 langflow-0.3.3/src/backend/langflow/graph/vertex/base.py
+-rw-r--r--   0        0        0        1 2023-07-21 21:05:37.221974 langflow-0.3.3/src/backend/langflow/graph/vertex/constants.py
+-rw-r--r--   0        0        0     8205 2023-07-21 21:05:37.221974 langflow-0.3.3/src/backend/langflow/graph/vertex/types.py
+-rw-r--r--   0        0        0        0 2023-07-21 21:05:37.221974 langflow-0.3.3/src/backend/langflow/interface/__init__.py
+-rw-r--r--   0        0        0       84 2023-07-21 21:05:37.221974 langflow-0.3.3/src/backend/langflow/interface/agents/__init__.py
+-rw-r--r--   0        0        0     2423 2023-07-21 21:05:37.221974 langflow-0.3.3/src/backend/langflow/interface/agents/base.py
+-rw-r--r--   0        0        0    10224 2023-07-21 21:05:37.221974 langflow-0.3.3/src/backend/langflow/interface/agents/custom.py
+-rw-r--r--   0        0        0     1447 2023-07-21 21:05:37.221974 langflow-0.3.3/src/backend/langflow/interface/agents/prebuilt.py
+-rw-r--r--   0        0        0     4632 2023-07-21 21:05:37.221974 langflow-0.3.3/src/backend/langflow/interface/base.py
+-rw-r--r--   0        0        0       84 2023-07-21 21:05:37.221974 langflow-0.3.3/src/backend/langflow/interface/chains/__init__.py
+-rw-r--r--   0        0        0     2867 2023-07-21 21:05:37.221974 langflow-0.3.3/src/backend/langflow/interface/chains/base.py
+-rw-r--r--   0        0        0     4843 2023-07-21 21:05:37.221974 langflow-0.3.3/src/backend/langflow/interface/chains/custom.py
+-rw-r--r--   0        0        0     2306 2023-07-21 21:05:37.221974 langflow-0.3.3/src/backend/langflow/interface/custom_lists.py
+-rw-r--r--   0        0        0        0 2023-07-21 21:05:37.221974 langflow-0.3.3/src/backend/langflow/interface/document_loaders/__init__.py
+-rw-r--r--   0        0        0     1479 2023-07-21 21:05:37.221974 langflow-0.3.3/src/backend/langflow/interface/document_loaders/base.py
+-rw-r--r--   0        0        0        0 2023-07-21 21:05:37.221974 langflow-0.3.3/src/backend/langflow/interface/embeddings/__init__.py
+-rw-r--r--   0        0        0     1445 2023-07-21 21:05:37.221974 langflow-0.3.3/src/backend/langflow/interface/embeddings/base.py
+-rw-r--r--   0        0        0      171 2023-07-21 21:05:37.221974 langflow-0.3.3/src/backend/langflow/interface/importing/__init__.py
+-rw-r--r--   0        0        0     5625 2023-07-21 21:05:37.221974 langflow-0.3.3/src/backend/langflow/interface/importing/utils.py
+-rw-r--r--   0        0        0        0 2023-07-21 21:05:37.221974 langflow-0.3.3/src/backend/langflow/interface/initialize/__init__.py
+-rw-r--r--   0        0        0      385 2023-07-21 21:05:37.221974 langflow-0.3.3/src/backend/langflow/interface/initialize/llm.py
+-rw-r--r--   0        0        0    20534 2023-07-21 21:05:37.221974 langflow-0.3.3/src/backend/langflow/interface/initialize/loading.py
+-rw-r--r--   0        0        0     7704 2023-07-21 21:05:37.221974 langflow-0.3.3/src/backend/langflow/interface/initialize/vector_store.py
+-rw-r--r--   0        0        0     1915 2023-07-21 21:05:37.221974 langflow-0.3.3/src/backend/langflow/interface/listing.py
+-rw-r--r--   0        0        0       78 2023-07-21 21:05:37.221974 langflow-0.3.3/src/backend/langflow/interface/llms/__init__.py
+-rw-r--r--   0        0        0     1355 2023-07-21 21:05:37.221974 langflow-0.3.3/src/backend/langflow/interface/llms/base.py
+-rw-r--r--   0        0        0       88 2023-07-21 21:05:37.221974 langflow-0.3.3/src/backend/langflow/interface/memories/__init__.py
+-rw-r--r--   0        0        0     2135 2023-07-21 21:05:37.221974 langflow-0.3.3/src/backend/langflow/interface/memories/base.py
+-rw-r--r--   0        0        0        0 2023-07-21 21:05:37.221974 langflow-0.3.3/src/backend/langflow/interface/output_parsers/__init__.py
+-rw-r--r--   0        0        0     2355 2023-07-21 21:05:37.221974 langflow-0.3.3/src/backend/langflow/interface/output_parsers/base.py
+-rw-r--r--   0        0        0       87 2023-07-21 21:05:37.221974 langflow-0.3.3/src/backend/langflow/interface/prompts/__init__.py
+-rw-r--r--   0        0        0     2459 2023-07-21 21:05:37.221974 langflow-0.3.3/src/backend/langflow/interface/prompts/base.py
+-rw-r--r--   0        0        0     2483 2023-07-21 21:05:37.221974 langflow-0.3.3/src/backend/langflow/interface/prompts/custom.py
+-rw-r--r--   0        0        0        0 2023-07-21 21:05:37.221974 langflow-0.3.3/src/backend/langflow/interface/retrievers/__init__.py
+-rw-r--r--   0        0        0     2086 2023-07-21 21:05:37.221974 langflow-0.3.3/src/backend/langflow/interface/retrievers/base.py
+-rw-r--r--   0        0        0     2764 2023-07-21 21:05:37.221974 langflow-0.3.3/src/backend/langflow/interface/run.py
+-rw-r--r--   0        0        0      106 2023-07-21 21:05:37.221974 langflow-0.3.3/src/backend/langflow/interface/text_splitters/__init__.py
+-rw-r--r--   0        0        0     1450 2023-07-21 21:05:37.221974 langflow-0.3.3/src/backend/langflow/interface/text_splitters/base.py
+-rw-r--r--   0        0        0        0 2023-07-21 21:05:37.221974 langflow-0.3.3/src/backend/langflow/interface/toolkits/__init__.py
+-rw-r--r--   0        0        0     2598 2023-07-21 21:05:37.221974 langflow-0.3.3/src/backend/langflow/interface/toolkits/base.py
+-rw-r--r--   0        0        0        0 2023-07-21 21:05:37.221974 langflow-0.3.3/src/backend/langflow/interface/toolkits/custom.py
+-rw-r--r--   0        0        0       81 2023-07-21 21:05:37.221974 langflow-0.3.3/src/backend/langflow/interface/tools/__init__.py
+-rw-r--r--   0        0        0     5417 2023-07-21 21:05:37.221974 langflow-0.3.3/src/backend/langflow/interface/tools/base.py
+-rw-r--r--   0        0        0      900 2023-07-21 21:05:37.221974 langflow-0.3.3/src/backend/langflow/interface/tools/constants.py
+-rw-r--r--   0        0        0     1323 2023-07-21 21:05:37.221974 langflow-0.3.3/src/backend/langflow/interface/tools/custom.py
+-rw-r--r--   0        0        0     4328 2023-07-21 21:05:37.221974 langflow-0.3.3/src/backend/langflow/interface/tools/util.py
+-rw-r--r--   0        0        0     2063 2023-07-21 21:05:37.221974 langflow-0.3.3/src/backend/langflow/interface/types.py
+-rw-r--r--   0        0        0        0 2023-07-21 21:05:37.221974 langflow-0.3.3/src/backend/langflow/interface/utilities/__init__.py
+-rw-r--r--   0        0        0     2294 2023-07-21 21:05:37.221974 langflow-0.3.3/src/backend/langflow/interface/utilities/base.py
+-rw-r--r--   0        0        0     2696 2023-07-21 21:05:37.221974 langflow-0.3.3/src/backend/langflow/interface/utils.py
+-rw-r--r--   0        0        0        0 2023-07-21 21:05:37.221974 langflow-0.3.3/src/backend/langflow/interface/vector_store/__init__.py
+-rw-r--r--   0        0        0     1813 2023-07-21 21:05:37.221974 langflow-0.3.3/src/backend/langflow/interface/vector_store/base.py
+-rw-r--r--   0        0        0        0 2023-07-21 21:05:37.221974 langflow-0.3.3/src/backend/langflow/interface/wrappers/__init__.py
+-rw-r--r--   0        0        0     1500 2023-07-21 21:05:37.221974 langflow-0.3.3/src/backend/langflow/interface/wrappers/base.py
+-rw-r--r--   0        0        0       29 2023-07-21 21:05:37.221974 langflow-0.3.3/src/backend/langflow/jcloud.yml
+-rw-r--r--   0        0        0      428 2023-07-21 21:05:37.221974 langflow-0.3.3/src/backend/langflow/lcserve.py
+-rw-r--r--   0        0        0     2265 2023-07-21 21:05:37.221974 langflow-0.3.3/src/backend/langflow/main.py
+-rw-r--r--   0        0        0        0 2023-07-21 21:05:37.221974 langflow-0.3.3/src/backend/langflow/processing/__init__.py
+-rw-r--r--   0        0        0     1980 2023-07-21 21:05:37.225974 langflow-0.3.3/src/backend/langflow/processing/base.py
+-rw-r--r--   0        0        0     8510 2023-07-21 21:05:37.225974 langflow-0.3.3/src/backend/langflow/processing/process.py
+-rw-r--r--   0        0        0      579 2023-07-21 21:05:37.225974 langflow-0.3.3/src/backend/langflow/server.py
+-rw-r--r--   0        0        0     3300 2023-07-21 21:05:37.225974 langflow-0.3.3/src/backend/langflow/settings.py
+-rw-r--r--   0        0        0        0 2023-07-21 21:05:37.225974 langflow-0.3.3/src/backend/langflow/template/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-21 21:05:37.225974 langflow-0.3.3/src/backend/langflow/template/field/__init__.py
+-rw-r--r--   0        0        0     1222 2023-07-21 21:05:37.225974 langflow-0.3.3/src/backend/langflow/template/field/base.py
+-rw-r--r--   0        0        0      375 2023-07-21 21:05:37.225974 langflow-0.3.3/src/backend/langflow/template/frontend_node/__init__.py
+-rw-r--r--   0        0        0     7032 2023-07-21 21:05:37.225974 langflow-0.3.3/src/backend/langflow/template/frontend_node/agents.py
+-rw-r--r--   0        0        0     9742 2023-07-21 21:05:37.225974 langflow-0.3.3/src/backend/langflow/template/frontend_node/base.py
+-rw-r--r--   0        0        0     7796 2023-07-21 21:05:37.225974 langflow-0.3.3/src/backend/langflow/template/frontend_node/chains.py
+-rw-r--r--   0        0        0     1609 2023-07-21 21:05:37.225974 langflow-0.3.3/src/backend/langflow/template/frontend_node/constants.py
+-rw-r--r--   0        0        0     8635 2023-07-21 21:05:37.225974 langflow-0.3.3/src/backend/langflow/template/frontend_node/documentloaders.py
+-rw-r--r--   0        0        0     1680 2023-07-21 21:05:37.225974 langflow-0.3.3/src/backend/langflow/template/frontend_node/embeddings.py
+-rw-r--r--   0        0        0        0 2023-07-21 21:05:37.225974 langflow-0.3.3/src/backend/langflow/template/frontend_node/formatter/__init__.py
+-rw-r--r--   0        0        0      297 2023-07-21 21:05:37.225974 langflow-0.3.3/src/backend/langflow/template/frontend_node/formatter/base.py
+-rw-r--r--   0        0        0     5569 2023-07-21 21:05:37.225974 langflow-0.3.3/src/backend/langflow/template/frontend_node/formatter/field_formatters.py
+-rw-r--r--   0        0        0     5369 2023-07-21 21:05:37.225974 langflow-0.3.3/src/backend/langflow/template/frontend_node/llms.py
+-rw-r--r--   0        0        0     6285 2023-07-21 21:05:37.225974 langflow-0.3.3/src/backend/langflow/template/frontend_node/memories.py
+-rw-r--r--   0        0        0      364 2023-07-21 21:05:37.225974 langflow-0.3.3/src/backend/langflow/template/frontend_node/output_parsers.py
+-rw-r--r--   0        0        0     3540 2023-07-21 21:05:37.225974 langflow-0.3.3/src/backend/langflow/template/frontend_node/prompts.py
+-rw-r--r--   0        0        0      523 2023-07-21 21:05:37.225974 langflow-0.3.3/src/backend/langflow/template/frontend_node/retrievers.py
+-rw-r--r--   0        0        0     2355 2023-07-21 21:05:37.225974 langflow-0.3.3/src/backend/langflow/template/frontend_node/textsplitters.py
+-rw-r--r--   0        0        0     4007 2023-07-21 21:05:37.225974 langflow-0.3.3/src/backend/langflow/template/frontend_node/tools.py
+-rw-r--r--   0        0        0      823 2023-07-21 21:05:37.225974 langflow-0.3.3/src/backend/langflow/template/frontend_node/utilities.py
+-rw-r--r--   0        0        0     9428 2023-07-21 21:05:37.225974 langflow-0.3.3/src/backend/langflow/template/frontend_node/vectorstores.py
+-rw-r--r--   0        0        0        0 2023-07-21 21:05:37.225974 langflow-0.3.3/src/backend/langflow/template/template/__init__.py
+-rw-r--r--   0        0        0     1181 2023-07-21 21:05:37.225974 langflow-0.3.3/src/backend/langflow/template/template/base.py
+-rw-r--r--   0        0        0        0 2023-07-21 21:05:37.225974 langflow-0.3.3/src/backend/langflow/utils/__init__.py
+-rw-r--r--   0        0        0     1758 2023-07-21 21:05:37.225974 langflow-0.3.3/src/backend/langflow/utils/constants.py
+-rw-r--r--   0        0        0      914 2023-07-21 21:05:37.225974 langflow-0.3.3/src/backend/langflow/utils/logger.py
+-rw-r--r--   0        0        0     3169 2023-07-21 21:05:37.225974 langflow-0.3.3/src/backend/langflow/utils/payload.py
+-rw-r--r--   0        0        0    11584 2023-07-21 21:05:37.225974 langflow-0.3.3/src/backend/langflow/utils/util.py
+-rw-r--r--   0        0        0     5325 2023-07-21 21:05:37.225974 langflow-0.3.3/src/backend/langflow/utils/validate.py
+-rw-r--r--   0        0        0    18139 1970-01-01 00:00:00.000000 langflow-0.3.3/PKG-INFO
```

### Comparing `langflow-0.3.2/LICENSE` & `langflow-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `langflow-0.3.2/README.md` & `langflow-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `langflow-0.3.2/pyproject.toml` & `langflow-0.3.3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 [tool.poetry]
 name = "langflow"
-version = "0.3.2"
+version = "0.3.3"
 description = "A Python package with a built-in web application"
 authors = ["Logspace <contact@logspace.ai>"]
 maintainers = [
+    "Carlos Coelho <carlos@logspace.ai>",
     "Cristhian Zanforlin <cristhian.lousa@gmail.com>",
     "Gabriel Almeida <gabriel@logspace.ai>",
     "Gustavo Schaedler <gustavopoa@gmail.com>",
+    "Igor Carvalho <igorr.ackerman@gmail.com>",
     "Lucas Eduoli <lucaseduoli@gmail.com>",
     "Otávio Anovazzi <otavio2204@gmail.com>",
+    "Rodrigo Nader <rodrigo@logspace.ai>",
 ]
 repository = "https://github.com/logspace-ai/langflow"
 license = "MIT"
 readme = "README.md"
 keywords = ["nlp", "langchain", "openai", "gpt", "gui"]
 packages = [{ include = "langflow", from = "src/backend" }]
 include = ["src/backend/langflow/*", "src/backend/langflow/**/*"]
```

### Comparing `langflow-0.3.2/src/backend/langflow/__main__.py` & `langflow-0.3.3/src/backend/langflow/__main__.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.2/src/backend/langflow/api/utils.py` & `langflow-0.3.3/src/backend/langflow/api/utils.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.2/src/backend/langflow/api/v1/base.py` & `langflow-0.3.3/src/backend/langflow/api/v1/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.2/src/backend/langflow/api/v1/callback.py` & `langflow-0.3.3/src/backend/langflow/api/v1/callback.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.2/src/backend/langflow/api/v1/chat.py` & `langflow-0.3.3/src/backend/langflow/api/v1/chat.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.2/src/backend/langflow/api/v1/endpoints.py` & `langflow-0.3.3/src/backend/langflow/api/v1/endpoints.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.2/src/backend/langflow/api/v1/flow_styles.py` & `langflow-0.3.3/src/backend/langflow/api/v1/flow_styles.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.2/src/backend/langflow/api/v1/flows.py` & `langflow-0.3.3/src/backend/langflow/api/v1/flows.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.2/src/backend/langflow/api/v1/schemas.py` & `langflow-0.3.3/src/backend/langflow/api/v1/schemas.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.2/src/backend/langflow/api/v1/validate.py` & `langflow-0.3.3/src/backend/langflow/api/v1/validate.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.2/src/backend/langflow/cache/base.py` & `langflow-0.3.3/src/backend/langflow/cache/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.2/src/backend/langflow/cache/flow.py` & `langflow-0.3.3/src/backend/langflow/cache/flow.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.2/src/backend/langflow/cache/manager.py` & `langflow-0.3.3/src/backend/langflow/cache/manager.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.2/src/backend/langflow/cache/utils.py` & `langflow-0.3.3/src/backend/langflow/cache/utils.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.2/src/backend/langflow/chat/manager.py` & `langflow-0.3.3/src/backend/langflow/chat/manager.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.2/src/backend/langflow/chat/utils.py` & `langflow-0.3.3/src/backend/langflow/chat/utils.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.2/src/backend/langflow/config.yaml` & `langflow-0.3.3/src/backend/langflow/config.yaml`

 * *Files identical despite different names*

### Comparing `langflow-0.3.2/src/backend/langflow/custom/customs.py` & `langflow-0.3.3/src/backend/langflow/custom/customs.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.2/src/backend/langflow/database/base.py` & `langflow-0.3.3/src/backend/langflow/database/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.2/src/backend/langflow/database/models/flow.py` & `langflow-0.3.3/src/backend/langflow/database/models/flow.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.2/src/backend/langflow/database/models/flow_style.py` & `langflow-0.3.3/src/backend/langflow/database/models/flow_style.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.2/src/backend/langflow/frontend/assets/Facebook_Messenger_logo_2020-d4e5cbf1.svg` & `langflow-0.3.3/src/backend/langflow/frontend/assets/Facebook_Messenger_logo_2020-d4e5cbf1.svg`

 * *Files identical despite different names*

### Comparing `langflow-0.3.2/src/backend/langflow/frontend/assets/Midjourney_Emblem-3952311f.svg` & `langflow-0.3.3/src/backend/langflow/frontend/assets/Midjourney_Emblem-3952311f.svg`

 * *Files identical despite different names*

### Comparing `langflow-0.3.2/src/backend/langflow/frontend/assets/Notion-logo-1b52a185.svg` & `langflow-0.3.3/src/backend/langflow/frontend/assets/Notion-logo-1b52a185.svg`

 * *Files identical despite different names*

### Comparing `langflow-0.3.2/src/backend/langflow/frontend/assets/QDrant-517d22b4.svg` & `langflow-0.3.3/src/backend/langflow/frontend/assets/QDrant-517d22b4.svg`

 * *Files identical despite different names*

### Comparing `langflow-0.3.2/src/backend/langflow/frontend/assets/Searx_logo-24248044.svg` & `langflow-0.3.3/src/backend/langflow/frontend/assets/Searx_logo-24248044.svg`

 * *Files identical despite different names*

### Comparing `langflow-0.3.2/src/backend/langflow/frontend/assets/Y_Combinator_logo-7356d194.svg` & `langflow-0.3.3/src/backend/langflow/frontend/assets/Y_Combinator_logo-7356d194.svg`

 * *Files identical despite different names*

### Comparing `langflow-0.3.2/src/backend/langflow/frontend/assets/airbyte-6aa3c5fa.svg` & `langflow-0.3.3/src/backend/langflow/frontend/assets/airbyte-6aa3c5fa.svg`

 * *Files identical despite different names*

### Comparing `langflow-0.3.2/src/backend/langflow/frontend/assets/anthropic_box-60809508.svg` & `langflow-0.3.3/src/backend/langflow/frontend/assets/anthropic_box-60809508.svg`

 * *Files identical despite different names*

### Comparing `langflow-0.3.2/src/backend/langflow/frontend/assets/bing-60c0c591.svg` & `langflow-0.3.3/src/backend/langflow/frontend/assets/bing-60c0c591.svg`

 * *Files identical despite different names*

### Comparing `langflow-0.3.2/src/backend/langflow/frontend/assets/chroma-65ceac37.svg` & `langflow-0.3.3/src/backend/langflow/frontend/assets/chroma-65ceac37.svg`

 * *Files identical despite different names*

### Comparing `langflow-0.3.2/src/backend/langflow/frontend/assets/cohere-f09153b9.svg` & `langflow-0.3.3/src/backend/langflow/frontend/assets/cohere-f09153b9.svg`

 * *Files identical despite different names*

### Comparing `langflow-0.3.2/src/backend/langflow/frontend/assets/evernote-icon-135bbfd8.svg` & `langflow-0.3.3/src/backend/langflow/frontend/assets/evernote-icon-135bbfd8.svg`

 * *Files identical despite different names*

### Comparing `langflow-0.3.2/src/backend/langflow/frontend/assets/gitbook-svgrepo-com-8beecec7.svg` & `langflow-0.3.3/src/backend/langflow/frontend/assets/gitbook-svgrepo-com-8beecec7.svg`

 * *Files identical despite different names*

### Comparing `langflow-0.3.2/src/backend/langflow/frontend/assets/google-1d6becdc.svg` & `langflow-0.3.3/src/backend/langflow/frontend/assets/google-1d6becdc.svg`

 * *Files identical despite different names*

### Comparing `langflow-0.3.2/src/backend/langflow/frontend/assets/hf-logo-942cad1c.svg` & `langflow-0.3.3/src/backend/langflow/frontend/assets/hf-logo-942cad1c.svg`

 * *Files identical despite different names*

### Comparing `langflow-0.3.2/src/backend/langflow/frontend/assets/ifixit-seeklogo.com-6846f6e5.svg` & `langflow-0.3.3/src/backend/langflow/frontend/assets/ifixit-seeklogo.com-6846f6e5.svg`

 * *Files identical despite different names*

### Comparing `langflow-0.3.2/src/backend/langflow/frontend/assets/index-592d2574.css` & `langflow-0.3.3/src/backend/langflow/frontend/assets/index-592d2574.css`

 * *Files identical despite different names*

### Comparing `langflow-0.3.2/src/backend/langflow/frontend/assets/index-9bb007a7.js` & `langflow-0.3.3/src/backend/langflow/frontend/assets/index-9bb007a7.js`

 * *Files identical despite different names*

### Comparing `langflow-0.3.2/src/backend/langflow/frontend/assets/male-technologist-d2e7de57.png` & `langflow-0.3.3/src/backend/langflow/frontend/assets/male-technologist-d2e7de57.png`

 * *Files identical despite different names*

### Comparing `langflow-0.3.2/src/backend/langflow/frontend/assets/meta-icon-fc8308c0.svg` & `langflow-0.3.3/src/backend/langflow/frontend/assets/meta-icon-fc8308c0.svg`

 * *Files identical despite different names*

### Comparing `langflow-0.3.2/src/backend/langflow/frontend/assets/mongodb-icon-64a21d47.svg` & `langflow-0.3.3/src/backend/langflow/frontend/assets/mongodb-icon-64a21d47.svg`

 * *Files identical despite different names*

### Comparing `langflow-0.3.2/src/backend/langflow/frontend/assets/openAI-2c85883b.svg` & `langflow-0.3.3/src/backend/langflow/frontend/assets/openAI-2c85883b.svg`

 * *Files identical despite different names*

### Comparing `langflow-0.3.2/src/backend/langflow/frontend/assets/pinecone_logo-411e417b.svg` & `langflow-0.3.3/src/backend/langflow/frontend/assets/pinecone_logo-411e417b.svg`

 * *Files identical despite different names*

### Comparing `langflow-0.3.2/src/backend/langflow/frontend/assets/robot-95e1b00d.png` & `langflow-0.3.3/src/backend/langflow/frontend/assets/robot-95e1b00d.png`

 * *Files identical despite different names*

### Comparing `langflow-0.3.2/src/backend/langflow/frontend/assets/slack-icon-32084c4a.svg` & `langflow-0.3.3/src/backend/langflow/frontend/assets/slack-icon-32084c4a.svg`

 * *Files identical despite different names*

### Comparing `langflow-0.3.2/src/backend/langflow/frontend/assets/supabase-icon-bdc56c95.svg` & `langflow-0.3.3/src/backend/langflow/frontend/assets/supabase-icon-bdc56c95.svg`

 * *Files identical despite different names*

### Comparing `langflow-0.3.2/src/backend/langflow/frontend/assets/vertex_ai-a23b625d.svg` & `langflow-0.3.3/src/backend/langflow/frontend/assets/vertex_ai-a23b625d.svg`

 * *Files identical despite different names*

### Comparing `langflow-0.3.2/src/backend/langflow/frontend/assets/web-vitals-60d3425a.js` & `langflow-0.3.3/src/backend/langflow/frontend/assets/web-vitals-60d3425a.js`

 * *Files identical despite different names*

### Comparing `langflow-0.3.2/src/backend/langflow/frontend/favicon.ico` & `langflow-0.3.3/src/backend/langflow/frontend/favicon.ico`

 * *Files identical despite different names*

### Comparing `langflow-0.3.2/src/backend/langflow/frontend/index.html` & `langflow-0.3.3/src/backend/langflow/frontend/index.html`

 * *Files identical despite different names*

### Comparing `langflow-0.3.2/src/backend/langflow/graph/__init__.py` & `langflow-0.3.3/src/backend/langflow/graph/__init__.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.2/src/backend/langflow/graph/edge/base.py` & `langflow-0.3.3/src/backend/langflow/graph/edge/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.2/src/backend/langflow/graph/graph/base.py` & `langflow-0.3.3/src/backend/langflow/graph/graph/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.2/src/backend/langflow/graph/graph/constants.py` & `langflow-0.3.3/src/backend/langflow/graph/graph/constants.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.2/src/backend/langflow/graph/utils.py` & `langflow-0.3.3/src/backend/langflow/graph/utils.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.2/src/backend/langflow/graph/vertex/base.py` & `langflow-0.3.3/src/backend/langflow/graph/vertex/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.2/src/backend/langflow/graph/vertex/types.py` & `langflow-0.3.3/src/backend/langflow/graph/vertex/types.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.2/src/backend/langflow/interface/agents/base.py` & `langflow-0.3.3/src/backend/langflow/interface/agents/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.2/src/backend/langflow/interface/agents/custom.py` & `langflow-0.3.3/src/backend/langflow/interface/agents/custom.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.2/src/backend/langflow/interface/agents/prebuilt.py` & `langflow-0.3.3/src/backend/langflow/interface/agents/prebuilt.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.2/src/backend/langflow/interface/base.py` & `langflow-0.3.3/src/backend/langflow/interface/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.2/src/backend/langflow/interface/chains/base.py` & `langflow-0.3.3/src/backend/langflow/interface/chains/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.2/src/backend/langflow/interface/chains/custom.py` & `langflow-0.3.3/src/backend/langflow/interface/chains/custom.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.2/src/backend/langflow/interface/custom_lists.py` & `langflow-0.3.3/src/backend/langflow/interface/custom_lists.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.2/src/backend/langflow/interface/document_loaders/base.py` & `langflow-0.3.3/src/backend/langflow/interface/document_loaders/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.2/src/backend/langflow/interface/embeddings/base.py` & `langflow-0.3.3/src/backend/langflow/interface/embeddings/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.2/src/backend/langflow/interface/importing/utils.py` & `langflow-0.3.3/src/backend/langflow/interface/importing/utils.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.2/src/backend/langflow/interface/initialize/loading.py` & `langflow-0.3.3/src/backend/langflow/interface/initialize/loading.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.2/src/backend/langflow/interface/initialize/vector_store.py` & `langflow-0.3.3/src/backend/langflow/interface/initialize/vector_store.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.2/src/backend/langflow/interface/listing.py` & `langflow-0.3.3/src/backend/langflow/interface/listing.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.2/src/backend/langflow/interface/llms/base.py` & `langflow-0.3.3/src/backend/langflow/interface/llms/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.2/src/backend/langflow/interface/memories/base.py` & `langflow-0.3.3/src/backend/langflow/interface/memories/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.2/src/backend/langflow/interface/output_parsers/base.py` & `langflow-0.3.3/src/backend/langflow/interface/output_parsers/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.2/src/backend/langflow/interface/prompts/base.py` & `langflow-0.3.3/src/backend/langflow/interface/prompts/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.2/src/backend/langflow/interface/prompts/custom.py` & `langflow-0.3.3/src/backend/langflow/interface/prompts/custom.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.2/src/backend/langflow/interface/retrievers/base.py` & `langflow-0.3.3/src/backend/langflow/interface/retrievers/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.2/src/backend/langflow/interface/run.py` & `langflow-0.3.3/src/backend/langflow/interface/run.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.2/src/backend/langflow/interface/text_splitters/base.py` & `langflow-0.3.3/src/backend/langflow/interface/text_splitters/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.2/src/backend/langflow/interface/toolkits/base.py` & `langflow-0.3.3/src/backend/langflow/interface/toolkits/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.2/src/backend/langflow/interface/tools/base.py` & `langflow-0.3.3/src/backend/langflow/interface/tools/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.2/src/backend/langflow/interface/tools/constants.py` & `langflow-0.3.3/src/backend/langflow/interface/tools/constants.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.2/src/backend/langflow/interface/tools/custom.py` & `langflow-0.3.3/src/backend/langflow/interface/tools/custom.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.2/src/backend/langflow/interface/tools/util.py` & `langflow-0.3.3/src/backend/langflow/interface/tools/util.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.2/src/backend/langflow/interface/types.py` & `langflow-0.3.3/src/backend/langflow/interface/types.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.2/src/backend/langflow/interface/utilities/base.py` & `langflow-0.3.3/src/backend/langflow/interface/utilities/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.2/src/backend/langflow/interface/utils.py` & `langflow-0.3.3/src/backend/langflow/interface/utils.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.2/src/backend/langflow/interface/vector_store/base.py` & `langflow-0.3.3/src/backend/langflow/interface/vector_store/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.2/src/backend/langflow/interface/wrappers/base.py` & `langflow-0.3.3/src/backend/langflow/interface/wrappers/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.2/src/backend/langflow/main.py` & `langflow-0.3.3/src/backend/langflow/main.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.2/src/backend/langflow/processing/base.py` & `langflow-0.3.3/src/backend/langflow/processing/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.2/src/backend/langflow/processing/process.py` & `langflow-0.3.3/src/backend/langflow/processing/process.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.2/src/backend/langflow/server.py` & `langflow-0.3.3/src/backend/langflow/server.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.2/src/backend/langflow/settings.py` & `langflow-0.3.3/src/backend/langflow/settings.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.2/src/backend/langflow/template/field/base.py` & `langflow-0.3.3/src/backend/langflow/template/field/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.2/src/backend/langflow/template/frontend_node/agents.py` & `langflow-0.3.3/src/backend/langflow/template/frontend_node/agents.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.2/src/backend/langflow/template/frontend_node/base.py` & `langflow-0.3.3/src/backend/langflow/template/frontend_node/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.2/src/backend/langflow/template/frontend_node/chains.py` & `langflow-0.3.3/src/backend/langflow/template/frontend_node/chains.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.2/src/backend/langflow/template/frontend_node/constants.py` & `langflow-0.3.3/src/backend/langflow/template/frontend_node/constants.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,14 +4,15 @@
     "prefix",
     "examples",
     "temperature",
     "model_name",
     "headers",
     "max_value_length",
     "max_tokens",
+    "google_cse_id",
 ]
 
 DEFAULT_PROMPT = """
 I want you to act as a naming consultant for new companies.
 
 Here are some examples of good company names:
```

### Comparing `langflow-0.3.2/src/backend/langflow/template/frontend_node/documentloaders.py` & `langflow-0.3.3/src/backend/langflow/template/frontend_node/documentloaders.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.2/src/backend/langflow/template/frontend_node/embeddings.py` & `langflow-0.3.3/src/backend/langflow/template/frontend_node/embeddings.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.2/src/backend/langflow/template/frontend_node/formatter/field_formatters.py` & `langflow-0.3.3/src/backend/langflow/template/frontend_node/formatter/field_formatters.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.2/src/backend/langflow/template/frontend_node/llms.py` & `langflow-0.3.3/src/backend/langflow/template/frontend_node/llms.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.2/src/backend/langflow/template/frontend_node/memories.py` & `langflow-0.3.3/src/backend/langflow/template/frontend_node/memories.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.2/src/backend/langflow/template/frontend_node/prompts.py` & `langflow-0.3.3/src/backend/langflow/template/frontend_node/prompts.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.2/src/backend/langflow/template/frontend_node/retrievers.py` & `langflow-0.3.3/src/backend/langflow/template/frontend_node/retrievers.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.2/src/backend/langflow/template/frontend_node/textsplitters.py` & `langflow-0.3.3/src/backend/langflow/template/frontend_node/textsplitters.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.2/src/backend/langflow/template/frontend_node/tools.py` & `langflow-0.3.3/src/backend/langflow/template/frontend_node/tools.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.2/src/backend/langflow/template/frontend_node/utilities.py` & `langflow-0.3.3/src/backend/langflow/template/frontend_node/utilities.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.2/src/backend/langflow/template/frontend_node/vectorstores.py` & `langflow-0.3.3/src/backend/langflow/template/frontend_node/vectorstores.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.2/src/backend/langflow/template/template/base.py` & `langflow-0.3.3/src/backend/langflow/template/template/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.2/src/backend/langflow/utils/constants.py` & `langflow-0.3.3/src/backend/langflow/utils/constants.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.2/src/backend/langflow/utils/logger.py` & `langflow-0.3.3/src/backend/langflow/utils/logger.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.2/src/backend/langflow/utils/payload.py` & `langflow-0.3.3/src/backend/langflow/utils/payload.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.2/src/backend/langflow/utils/util.py` & `langflow-0.3.3/src/backend/langflow/utils/util.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.2/src/backend/langflow/utils/validate.py` & `langflow-0.3.3/src/backend/langflow/utils/validate.py`

 * *Files identical despite different names*

### Comparing `langflow-0.3.2/PKG-INFO` & `langflow-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: langflow
-Version: 0.3.2
+Version: 0.3.3
 Summary: A Python package with a built-in web application
 Home-page: https://github.com/logspace-ai/langflow
 License: MIT
 Keywords: nlp,langchain,openai,gpt,gui
 Author: Logspace
 Author-email: contact@logspace.ai
-Maintainer: Cristhian Zanforlin
-Maintainer-email: cristhian.lousa@gmail.com
+Maintainer: Carlos Coelho
+Maintainer-email: carlos@logspace.ai
 Requires-Python: >=3.9,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Provides-Extra: deploy
 Requires-Dist: anthropic (>=0.3.0,<0.4.0)
```

#### html2text {}

```diff
@@ -1,24 +1,24 @@
-Metadata-Version: 2.1 Name: langflow Version: 0.3.2 Summary: A Python package
+Metadata-Version: 2.1 Name: langflow Version: 0.3.3 Summary: A Python package
 with a built-in web application Home-page: https://github.com/logspace-ai/
 langflow License: MIT Keywords: nlp,langchain,openai,gpt,gui Author: Logspace
-Author-email: contact@logspace.ai Maintainer: Cristhian Zanforlin Maintainer-
-email: cristhian.lousa@gmail.com Requires-Python: >=3.9,<3.11 Classifier:
-License :: OSI Approved :: MIT License Classifier: Programming Language ::
-Python :: 3 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Programming Language :: Python :: 3.10 Provides-Extra: deploy Requires-Dist:
-anthropic (>=0.3.0,<0.4.0) Requires-Dist: appdirs (>=1.4.4,<2.0.0) Requires-
-Dist: beautifulsoup4 (>=4.12.2,<5.0.0) Requires-Dist: cachetools
-(>=5.3.1,<6.0.0) Requires-Dist: certifi (>=2023.5.7,<2024.0.0) Requires-Dist:
-chromadb (>=0.3.21,<0.4.0) Requires-Dist: cohere (>=4.11.0,<5.0.0) Requires-
-Dist: ctransformers (>=0.2.10,<0.3.0) Requires-Dist: docstring-parser
-(>=0.15,<0.16) Requires-Dist: faiss-cpu (>=1.7.4,<2.0.0) Requires-Dist: fake-
-useragent (>=1.1.3,<2.0.0) Requires-Dist: fastapi (>=0.100.0,<0.101.0)
-Requires-Dist: google-api-python-client (>=2.79.0,<3.0.0) Requires-Dist:
-google-cloud-aiplatform (>=1.26.1,<2.0.0) Requires-Dist: google-search-results
+Author-email: contact@logspace.ai Maintainer: Carlos Coelho Maintainer-email:
+carlos@logspace.ai Requires-Python: >=3.9,<3.11 Classifier: License :: OSI
+Approved :: MIT License Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
+Language :: Python :: 3.10 Provides-Extra: deploy Requires-Dist: anthropic
+(>=0.3.0,<0.4.0) Requires-Dist: appdirs (>=1.4.4,<2.0.0) Requires-Dist:
+beautifulsoup4 (>=4.12.2,<5.0.0) Requires-Dist: cachetools (>=5.3.1,<6.0.0)
+Requires-Dist: certifi (>=2023.5.7,<2024.0.0) Requires-Dist: chromadb
+(>=0.3.21,<0.4.0) Requires-Dist: cohere (>=4.11.0,<5.0.0) Requires-Dist:
+ctransformers (>=0.2.10,<0.3.0) Requires-Dist: docstring-parser (>=0.15,<0.16)
+Requires-Dist: faiss-cpu (>=1.7.4,<2.0.0) Requires-Dist: fake-useragent
+(>=1.1.3,<2.0.0) Requires-Dist: fastapi (>=0.100.0,<0.101.0) Requires-Dist:
+google-api-python-client (>=2.79.0,<3.0.0) Requires-Dist: google-cloud-
+aiplatform (>=1.26.1,<2.0.0) Requires-Dist: google-search-results
 (>=2.4.1,<3.0.0) Requires-Dist: gunicorn (>=20.1.0,<21.0.0) Requires-Dist:
 huggingface-hub (>=0.15.0,<0.16.0) Requires-Dist: jina (==3.15.2) Requires-
 Dist: langchain (>=0.0.237,<0.0.238) Requires-Dist: langchain-serve (>0.0.51) ;
 extra == "deploy" Requires-Dist: llama-cpp-python (>=0.1.0,<0.2.0) Requires-
 Dist: lxml (>=4.9.2,<5.0.0) Requires-Dist: multiprocess (>=0.70.14,<0.71.0)
 Requires-Dist: networkx (>=3.1,<4.0) Requires-Dist: openai (>=0.27.8,<0.28.0)
 Requires-Dist: orjson (>=3.9.1,<4.0.0) Requires-Dist: pandas (>=2.0.0,<3.0.0)
```

