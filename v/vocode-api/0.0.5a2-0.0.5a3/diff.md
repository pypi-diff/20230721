# Comparing `tmp/vocode_api-0.0.5a2.tar.gz` & `tmp/vocode_api-0.0.5a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vocode_api-0.0.5a2.tar", max compression
+gzip compressed data, was "vocode_api-0.0.5a3.tar", max compression
```

## Comparing `vocode_api-0.0.5a2.tar` & `vocode_api-0.0.5a3.tar`

### file list

```diff
@@ -1,109 +1,110 @@
--rw-r--r--   0        0        0     2777 2023-07-19 22:01:42.581733 vocode_api-0.0.5a2/README.md
--rw-r--r--   0        0        0      379 2023-07-19 22:01:42.581733 vocode_api-0.0.5a2/pyproject.toml
--rw-r--r--   0        0        0     4706 2023-07-19 22:01:42.581733 vocode_api-0.0.5a2/src/vocode/__init__.py
--rw-r--r--   0        0        0     2074 2023-07-19 22:01:42.581733 vocode_api-0.0.5a2/src/vocode/client.py
--rw-r--r--   0        0        0      348 2023-07-19 22:01:42.581733 vocode_api-0.0.5a2/src/vocode/core/__init__.py
--rw-r--r--   0        0        0      426 2023-07-19 22:01:42.581733 vocode_api-0.0.5a2/src/vocode/core/api_error.py
--rw-r--r--   0        0        0     1047 2023-07-19 22:01:42.581733 vocode_api-0.0.5a2/src/vocode/core/datetime_utils.py
--rw-r--r--   0        0        0     3710 2023-07-19 22:01:42.581733 vocode_api-0.0.5a2/src/vocode/core/jsonable_encoder.py
--rw-r--r--   0        0        0      385 2023-07-19 22:01:42.581733 vocode_api-0.0.5a2/src/vocode/core/remove_none_from_headers.py
--rw-r--r--   0        0        0      170 2023-07-19 22:01:42.581733 vocode_api-0.0.5a2/src/vocode/errors/__init__.py
--rw-r--r--   0        0        0      313 2023-07-19 22:01:42.581733 vocode_api-0.0.5a2/src/vocode/errors/unprocessable_entity_error.py
--rw-r--r--   0        0        0        0 2023-07-19 22:01:42.581733 vocode_api-0.0.5a2/src/vocode/py.typed
--rw-r--r--   0        0        0      220 2023-07-19 22:01:42.585733 vocode_api-0.0.5a2/src/vocode/resources/__init__.py
--rw-r--r--   0        0        0       65 2023-07-19 22:01:42.585733 vocode_api-0.0.5a2/src/vocode/resources/actions/__init__.py
--rw-r--r--   0        0        0     9264 2023-07-19 22:01:42.585733 vocode_api-0.0.5a2/src/vocode/resources/actions/client.py
--rw-r--r--   0        0        0       65 2023-07-19 22:01:42.585733 vocode_api-0.0.5a2/src/vocode/resources/agents/__init__.py
--rw-r--r--   0        0        0     8720 2023-07-19 22:01:42.585733 vocode_api-0.0.5a2/src/vocode/resources/agents/client.py
--rw-r--r--   0        0        0       65 2023-07-19 22:01:42.585733 vocode_api-0.0.5a2/src/vocode/resources/calls/__init__.py
--rw-r--r--   0        0        0    10802 2023-07-19 22:01:42.585733 vocode_api-0.0.5a2/src/vocode/resources/calls/client.py
--rw-r--r--   0        0        0       65 2023-07-19 22:01:42.585733 vocode_api-0.0.5a2/src/vocode/resources/numbers/__init__.py
--rw-r--r--   0        0        0    10652 2023-07-19 22:01:42.585733 vocode_api-0.0.5a2/src/vocode/resources/numbers/client.py
--rw-r--r--   0        0        0       65 2023-07-19 22:01:42.585733 vocode_api-0.0.5a2/src/vocode/resources/usage/__init__.py
--rw-r--r--   0        0        0     2159 2023-07-19 22:01:42.585733 vocode_api-0.0.5a2/src/vocode/resources/usage/client.py
--rw-r--r--   0        0        0       65 2023-07-19 22:01:42.585733 vocode_api-0.0.5a2/src/vocode/resources/voices/__init__.py
--rw-r--r--   0        0        0     9214 2023-07-19 22:01:42.585733 vocode_api-0.0.5a2/src/vocode/resources/voices/client.py
--rw-r--r--   0        0        0       65 2023-07-19 22:01:42.585733 vocode_api-0.0.5a2/src/vocode/resources/webhooks/__init__.py
--rw-r--r--   0        0        0     8808 2023-07-19 22:01:42.585733 vocode_api-0.0.5a2/src/vocode/resources/webhooks/client.py
--rw-r--r--   0        0        0     6970 2023-07-19 22:01:42.585733 vocode_api-0.0.5a2/src/vocode/types/__init__.py
--rw-r--r--   0        0        0      837 2023-07-19 22:01:42.585733 vocode_api-0.0.5a2/src/vocode/types/action_type.py
--rw-r--r--   0        0        0     1045 2023-07-19 22:01:42.585733 vocode_api-0.0.5a2/src/vocode/types/agent.py
--rw-r--r--   0        0        0      321 2023-07-19 22:01:42.585733 vocode_api-0.0.5a2/src/vocode/types/agent_actions_item.py
--rw-r--r--   0        0        0     1096 2023-07-19 22:01:42.585733 vocode_api-0.0.5a2/src/vocode/types/agent_params.py
--rw-r--r--   0        0        0      409 2023-07-19 22:01:42.585733 vocode_api-0.0.5a2/src/vocode/types/agent_params_actions_item.py
--rw-r--r--   0        0        0      332 2023-07-19 22:01:42.585733 vocode_api-0.0.5a2/src/vocode/types/agent_params_voice.py
--rw-r--r--   0        0        0      177 2023-07-19 22:01:42.585733 vocode_api-0.0.5a2/src/vocode/types/agent_params_webhook.py
--rw-r--r--   0        0        0     1360 2023-07-19 22:01:42.585733 vocode_api-0.0.5a2/src/vocode/types/agent_update_params.py
--rw-r--r--   0        0        0      368 2023-07-19 22:01:42.585733 vocode_api-0.0.5a2/src/vocode/types/agent_update_params_actions.py
--rw-r--r--   0        0        0      477 2023-07-19 22:01:42.585733 vocode_api-0.0.5a2/src/vocode/types/agent_update_params_actions_agent_update_params_actions_item.py
--rw-r--r--   0        0        0      177 2023-07-19 22:01:42.585733 vocode_api-0.0.5a2/src/vocode/types/agent_update_params_initial_message.py
--rw-r--r--   0        0        0      169 2023-07-19 22:01:42.585733 vocode_api-0.0.5a2/src/vocode/types/agent_update_params_prompt.py
--rw-r--r--   0        0        0      445 2023-07-19 22:01:42.585733 vocode_api-0.0.5a2/src/vocode/types/agent_update_params_voice.py
--rw-r--r--   0        0        0      246 2023-07-19 22:01:42.585733 vocode_api-0.0.5a2/src/vocode/types/agent_update_params_webhook.py
--rw-r--r--   0        0        0      269 2023-07-19 22:01:42.585733 vocode_api-0.0.5a2/src/vocode/types/agent_voice.py
--rw-r--r--   0        0        0      152 2023-07-19 22:01:42.585733 vocode_api-0.0.5a2/src/vocode/types/agent_webhook.py
--rw-r--r--   0        0        0      913 2023-07-19 22:01:42.585733 vocode_api-0.0.5a2/src/vocode/types/azure_voice.py
--rw-r--r--   0        0        0      873 2023-07-19 22:01:42.585733 vocode_api-0.0.5a2/src/vocode/types/azure_voice_params.py
--rw-r--r--   0        0        0     1197 2023-07-19 22:01:42.585733 vocode_api-0.0.5a2/src/vocode/types/azure_voice_update_params.py
--rw-r--r--   0        0        0      173 2023-07-19 22:01:42.585733 vocode_api-0.0.5a2/src/vocode/types/azure_voice_update_params_pitch.py
--rw-r--r--   0        0        0      172 2023-07-19 22:01:42.585733 vocode_api-0.0.5a2/src/vocode/types/azure_voice_update_params_rate.py
--rw-r--r--   0        0        0      177 2023-07-19 22:01:42.585733 vocode_api-0.0.5a2/src/vocode/types/azure_voice_update_params_voice_name.py
--rw-r--r--   0        0        0     1102 2023-07-19 22:01:42.585733 vocode_api-0.0.5a2/src/vocode/types/call.py
--rw-r--r--   0        0        0      143 2023-07-19 22:01:42.585733 vocode_api-0.0.5a2/src/vocode/types/call_agent.py
--rw-r--r--   0        0        0      832 2023-07-19 22:01:42.585733 vocode_api-0.0.5a2/src/vocode/types/call_status.py
--rw-r--r--   0        0        0      395 2023-07-19 22:01:42.585733 vocode_api-0.0.5a2/src/vocode/types/create_action_request.py
--rw-r--r--   0        0        0      320 2023-07-19 22:01:42.585733 vocode_api-0.0.5a2/src/vocode/types/create_action_response.py
--rw-r--r--   0        0        0      175 2023-07-19 22:01:42.585733 vocode_api-0.0.5a2/src/vocode/types/create_call_request_agent.py
--rw-r--r--   0        0        0      329 2023-07-19 22:01:42.585733 vocode_api-0.0.5a2/src/vocode/types/create_voice_request.py
--rw-r--r--   0        0        0      273 2023-07-19 22:01:42.585733 vocode_api-0.0.5a2/src/vocode/types/create_voice_response.py
--rw-r--r--   0        0        0      931 2023-07-19 22:01:42.585733 vocode_api-0.0.5a2/src/vocode/types/dtmf_action.py
--rw-r--r--   0        0        0      891 2023-07-19 22:01:42.585733 vocode_api-0.0.5a2/src/vocode/types/dtmf_action_params.py
--rw-r--r--   0        0        0      932 2023-07-19 22:01:42.585733 vocode_api-0.0.5a2/src/vocode/types/dtmf_action_update_params.py
--rw-r--r--   0        0        0      239 2023-07-19 22:01:42.585733 vocode_api-0.0.5a2/src/vocode/types/dtmf_action_update_params_config.py
--rw-r--r--   0        0        0      953 2023-07-19 22:01:42.585733 vocode_api-0.0.5a2/src/vocode/types/eleven_labs_voice.py
--rw-r--r--   0        0        0      913 2023-07-19 22:01:42.585733 vocode_api-0.0.5a2/src/vocode/types/eleven_labs_voice_params.py
--rw-r--r--   0        0        0     1455 2023-07-19 22:01:42.585733 vocode_api-0.0.5a2/src/vocode/types/eleven_labs_voice_update_params.py
--rw-r--r--   0        0        0      179 2023-07-19 22:01:42.585733 vocode_api-0.0.5a2/src/vocode/types/eleven_labs_voice_update_params_api_key.py
--rw-r--r--   0        0        0      190 2023-07-19 22:01:42.585733 vocode_api-0.0.5a2/src/vocode/types/eleven_labs_voice_update_params_similarity_boost.py
--rw-r--r--   0        0        0      184 2023-07-19 22:01:42.585733 vocode_api-0.0.5a2/src/vocode/types/eleven_labs_voice_update_params_stability.py
--rw-r--r--   0        0        0      180 2023-07-19 22:01:42.585733 vocode_api-0.0.5a2/src/vocode/types/eleven_labs_voice_update_params_voice_id.py
--rw-r--r--   0        0        0      736 2023-07-19 22:01:42.585733 vocode_api-0.0.5a2/src/vocode/types/empty_action_config.py
--rw-r--r--   0        0        0      942 2023-07-19 22:01:42.585733 vocode_api-0.0.5a2/src/vocode/types/end_conversation_action.py
--rw-r--r--   0        0        0      902 2023-07-19 22:01:42.585733 vocode_api-0.0.5a2/src/vocode/types/end_conversation_action_params.py
--rw-r--r--   0        0        0      977 2023-07-19 22:01:42.585733 vocode_api-0.0.5a2/src/vocode/types/end_conversation_action_update_params.py
--rw-r--r--   0        0        0      250 2023-07-19 22:01:42.585733 vocode_api-0.0.5a2/src/vocode/types/end_conversation_action_update_params_config.py
--rw-r--r--   0        0        0     1395 2023-07-19 22:01:42.585733 vocode_api-0.0.5a2/src/vocode/types/event_type.py
--rw-r--r--   0        0        0      317 2023-07-19 22:01:42.585733 vocode_api-0.0.5a2/src/vocode/types/get_action_response.py
--rw-r--r--   0        0        0      270 2023-07-19 22:01:42.585733 vocode_api-0.0.5a2/src/vocode/types/get_voice_response.py
--rw-r--r--   0        0        0      466 2023-07-19 22:01:42.585733 vocode_api-0.0.5a2/src/vocode/types/http_method.py
--rw-r--r--   0        0        0      843 2023-07-19 22:01:42.585733 vocode_api-0.0.5a2/src/vocode/types/http_validation_error.py
--rw-r--r--   0        0        0      323 2023-07-19 22:01:42.585733 vocode_api-0.0.5a2/src/vocode/types/list_actions_response_item.py
--rw-r--r--   0        0        0      276 2023-07-19 22:01:42.585733 vocode_api-0.0.5a2/src/vocode/types/list_voices_response_item.py
--rw-r--r--   0        0        0      900 2023-07-19 22:01:42.585733 vocode_api-0.0.5a2/src/vocode/types/phone_number.py
--rw-r--r--   0        0        0      157 2023-07-19 22:01:42.585733 vocode_api-0.0.5a2/src/vocode/types/phone_number_inbound_agent.py
--rw-r--r--   0        0        0      674 2023-07-19 22:01:42.585733 vocode_api-0.0.5a2/src/vocode/types/plan_type.py
--rw-r--r--   0        0        0      846 2023-07-19 22:01:42.585733 vocode_api-0.0.5a2/src/vocode/types/rime_voice.py
--rw-r--r--   0        0        0      806 2023-07-19 22:01:42.585733 vocode_api-0.0.5a2/src/vocode/types/rime_voice_params.py
--rw-r--r--   0        0        0      929 2023-07-19 22:01:42.585733 vocode_api-0.0.5a2/src/vocode/types/rime_voice_update_params.py
--rw-r--r--   0        0        0      174 2023-07-19 22:01:42.585733 vocode_api-0.0.5a2/src/vocode/types/rime_voice_update_params_speaker.py
--rw-r--r--   0        0        0      925 2023-07-19 22:01:42.585733 vocode_api-0.0.5a2/src/vocode/types/transfer_call_action.py
--rw-r--r--   0        0        0      965 2023-07-19 22:01:42.585733 vocode_api-0.0.5a2/src/vocode/types/transfer_call_action_update_params.py
--rw-r--r--   0        0        0      250 2023-07-19 22:01:42.585733 vocode_api-0.0.5a2/src/vocode/types/transfer_call_action_update_params_config.py
--rw-r--r--   0        0        0      760 2023-07-19 22:01:42.585733 vocode_api-0.0.5a2/src/vocode/types/transfer_call_config.py
--rw-r--r--   0        0        0      728 2023-07-19 22:01:42.585733 vocode_api-0.0.5a2/src/vocode/types/undefined.py
--rw-r--r--   0        0        0      443 2023-07-19 22:01:42.585733 vocode_api-0.0.5a2/src/vocode/types/update_action_request_body.py
--rw-r--r--   0        0        0      320 2023-07-19 22:01:42.585733 vocode_api-0.0.5a2/src/vocode/types/update_action_response.py
--rw-r--r--   0        0        0      203 2023-07-19 22:01:42.585733 vocode_api-0.0.5a2/src/vocode/types/update_number_request_inbound_agent.py
--rw-r--r--   0        0        0      390 2023-07-19 22:01:42.585733 vocode_api-0.0.5a2/src/vocode/types/update_voice_request_body.py
--rw-r--r--   0        0        0      273 2023-07-19 22:01:42.585733 vocode_api-0.0.5a2/src/vocode/types/update_voice_response.py
--rw-r--r--   0        0        0      866 2023-07-19 22:01:42.585733 vocode_api-0.0.5a2/src/vocode/types/usage.py
--rw-r--r--   0        0        0      869 2023-07-19 22:01:42.585733 vocode_api-0.0.5a2/src/vocode/types/validation_error.py
--rw-r--r--   0        0        0      128 2023-07-19 22:01:42.585733 vocode_api-0.0.5a2/src/vocode/types/validation_error_loc_item.py
--rw-r--r--   0        0        0      907 2023-07-19 22:01:42.585733 vocode_api-0.0.5a2/src/vocode/types/voice_type.py
--rw-r--r--   0        0        0      921 2023-07-19 22:01:42.585733 vocode_api-0.0.5a2/src/vocode/types/webhook.py
--rw-r--r--   0        0        0      898 2023-07-19 22:01:42.585733 vocode_api-0.0.5a2/src/vocode/types/webhook_params.py
--rw-r--r--   0        0        0     1124 2023-07-19 22:01:42.585733 vocode_api-0.0.5a2/src/vocode/types/webhook_update_params.py
--rw-r--r--   0        0        0      214 2023-07-19 22:01:42.585733 vocode_api-0.0.5a2/src/vocode/types/webhook_update_params_method.py
--rw-r--r--   0        0        0      231 2023-07-19 22:01:42.585733 vocode_api-0.0.5a2/src/vocode/types/webhook_update_params_subscriptions.py
--rw-r--r--   0        0        0      168 2023-07-19 22:01:42.585733 vocode_api-0.0.5a2/src/vocode/types/webhook_update_params_url.py
--rw-r--r--   0        0        0     3187 1970-01-01 00:00:00.000000 vocode_api-0.0.5a2/PKG-INFO
+-rw-r--r--   0        0        0     2777 2023-07-21 01:39:03.495167 vocode_api-0.0.5a3/README.md
+-rw-r--r--   0        0        0      379 2023-07-21 01:39:03.495167 vocode_api-0.0.5a3/pyproject.toml
+-rw-r--r--   0        0        0     4774 2023-07-21 01:39:03.495167 vocode_api-0.0.5a3/src/vocode/__init__.py
+-rw-r--r--   0        0        0     2207 2023-07-21 01:39:03.495167 vocode_api-0.0.5a3/src/vocode/client.py
+-rw-r--r--   0        0        0      348 2023-07-21 01:39:03.495167 vocode_api-0.0.5a3/src/vocode/core/__init__.py
+-rw-r--r--   0        0        0      426 2023-07-21 01:39:03.495167 vocode_api-0.0.5a3/src/vocode/core/api_error.py
+-rw-r--r--   0        0        0     1047 2023-07-21 01:39:03.495167 vocode_api-0.0.5a3/src/vocode/core/datetime_utils.py
+-rw-r--r--   0        0        0     3710 2023-07-21 01:39:03.495167 vocode_api-0.0.5a3/src/vocode/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      385 2023-07-21 01:39:03.495167 vocode_api-0.0.5a3/src/vocode/core/remove_none_from_headers.py
+-rw-r--r--   0        0        0      224 2023-07-21 01:39:03.495167 vocode_api-0.0.5a3/src/vocode/environment.py
+-rw-r--r--   0        0        0      170 2023-07-21 01:39:03.495167 vocode_api-0.0.5a3/src/vocode/errors/__init__.py
+-rw-r--r--   0        0        0      313 2023-07-21 01:39:03.495167 vocode_api-0.0.5a3/src/vocode/errors/unprocessable_entity_error.py
+-rw-r--r--   0        0        0        0 2023-07-21 01:39:03.495167 vocode_api-0.0.5a3/src/vocode/py.typed
+-rw-r--r--   0        0        0      220 2023-07-21 01:39:03.495167 vocode_api-0.0.5a3/src/vocode/resources/__init__.py
+-rw-r--r--   0        0        0       65 2023-07-21 01:39:03.495167 vocode_api-0.0.5a3/src/vocode/resources/actions/__init__.py
+-rw-r--r--   0        0        0     9447 2023-07-21 01:39:03.495167 vocode_api-0.0.5a3/src/vocode/resources/actions/client.py
+-rw-r--r--   0        0        0       65 2023-07-21 01:39:03.495167 vocode_api-0.0.5a3/src/vocode/resources/agents/__init__.py
+-rw-r--r--   0        0        0     8903 2023-07-21 01:39:03.495167 vocode_api-0.0.5a3/src/vocode/resources/agents/client.py
+-rw-r--r--   0        0        0       65 2023-07-21 01:39:03.495167 vocode_api-0.0.5a3/src/vocode/resources/calls/__init__.py
+-rw-r--r--   0        0        0    10997 2023-07-21 01:39:03.495167 vocode_api-0.0.5a3/src/vocode/resources/calls/client.py
+-rw-r--r--   0        0        0       65 2023-07-21 01:39:03.495167 vocode_api-0.0.5a3/src/vocode/resources/numbers/__init__.py
+-rw-r--r--   0        0        0    10847 2023-07-21 01:39:03.495167 vocode_api-0.0.5a3/src/vocode/resources/numbers/client.py
+-rw-r--r--   0        0        0       65 2023-07-21 01:39:03.495167 vocode_api-0.0.5a3/src/vocode/resources/usage/__init__.py
+-rw-r--r--   0        0        0     2306 2023-07-21 01:39:03.495167 vocode_api-0.0.5a3/src/vocode/resources/usage/client.py
+-rw-r--r--   0        0        0       65 2023-07-21 01:39:03.495167 vocode_api-0.0.5a3/src/vocode/resources/voices/__init__.py
+-rw-r--r--   0        0        0     9397 2023-07-21 01:39:03.495167 vocode_api-0.0.5a3/src/vocode/resources/voices/client.py
+-rw-r--r--   0        0        0       65 2023-07-21 01:39:03.495167 vocode_api-0.0.5a3/src/vocode/resources/webhooks/__init__.py
+-rw-r--r--   0        0        0     8991 2023-07-21 01:39:03.495167 vocode_api-0.0.5a3/src/vocode/resources/webhooks/client.py
+-rw-r--r--   0        0        0     6970 2023-07-21 01:39:03.495167 vocode_api-0.0.5a3/src/vocode/types/__init__.py
+-rw-r--r--   0        0        0      837 2023-07-21 01:39:03.495167 vocode_api-0.0.5a3/src/vocode/types/action_type.py
+-rw-r--r--   0        0        0     1045 2023-07-21 01:39:03.495167 vocode_api-0.0.5a3/src/vocode/types/agent.py
+-rw-r--r--   0        0        0      321 2023-07-21 01:39:03.495167 vocode_api-0.0.5a3/src/vocode/types/agent_actions_item.py
+-rw-r--r--   0        0        0     1096 2023-07-21 01:39:03.499167 vocode_api-0.0.5a3/src/vocode/types/agent_params.py
+-rw-r--r--   0        0        0      409 2023-07-21 01:39:03.499167 vocode_api-0.0.5a3/src/vocode/types/agent_params_actions_item.py
+-rw-r--r--   0        0        0      332 2023-07-21 01:39:03.499167 vocode_api-0.0.5a3/src/vocode/types/agent_params_voice.py
+-rw-r--r--   0        0        0      177 2023-07-21 01:39:03.499167 vocode_api-0.0.5a3/src/vocode/types/agent_params_webhook.py
+-rw-r--r--   0        0        0     1360 2023-07-21 01:39:03.499167 vocode_api-0.0.5a3/src/vocode/types/agent_update_params.py
+-rw-r--r--   0        0        0      368 2023-07-21 01:39:03.499167 vocode_api-0.0.5a3/src/vocode/types/agent_update_params_actions.py
+-rw-r--r--   0        0        0      477 2023-07-21 01:39:03.499167 vocode_api-0.0.5a3/src/vocode/types/agent_update_params_actions_agent_update_params_actions_item.py
+-rw-r--r--   0        0        0      177 2023-07-21 01:39:03.499167 vocode_api-0.0.5a3/src/vocode/types/agent_update_params_initial_message.py
+-rw-r--r--   0        0        0      169 2023-07-21 01:39:03.499167 vocode_api-0.0.5a3/src/vocode/types/agent_update_params_prompt.py
+-rw-r--r--   0        0        0      445 2023-07-21 01:39:03.499167 vocode_api-0.0.5a3/src/vocode/types/agent_update_params_voice.py
+-rw-r--r--   0        0        0      246 2023-07-21 01:39:03.499167 vocode_api-0.0.5a3/src/vocode/types/agent_update_params_webhook.py
+-rw-r--r--   0        0        0      269 2023-07-21 01:39:03.499167 vocode_api-0.0.5a3/src/vocode/types/agent_voice.py
+-rw-r--r--   0        0        0      152 2023-07-21 01:39:03.499167 vocode_api-0.0.5a3/src/vocode/types/agent_webhook.py
+-rw-r--r--   0        0        0      913 2023-07-21 01:39:03.499167 vocode_api-0.0.5a3/src/vocode/types/azure_voice.py
+-rw-r--r--   0        0        0      873 2023-07-21 01:39:03.499167 vocode_api-0.0.5a3/src/vocode/types/azure_voice_params.py
+-rw-r--r--   0        0        0     1197 2023-07-21 01:39:03.499167 vocode_api-0.0.5a3/src/vocode/types/azure_voice_update_params.py
+-rw-r--r--   0        0        0      173 2023-07-21 01:39:03.499167 vocode_api-0.0.5a3/src/vocode/types/azure_voice_update_params_pitch.py
+-rw-r--r--   0        0        0      172 2023-07-21 01:39:03.499167 vocode_api-0.0.5a3/src/vocode/types/azure_voice_update_params_rate.py
+-rw-r--r--   0        0        0      177 2023-07-21 01:39:03.499167 vocode_api-0.0.5a3/src/vocode/types/azure_voice_update_params_voice_name.py
+-rw-r--r--   0        0        0     1102 2023-07-21 01:39:03.499167 vocode_api-0.0.5a3/src/vocode/types/call.py
+-rw-r--r--   0        0        0      143 2023-07-21 01:39:03.499167 vocode_api-0.0.5a3/src/vocode/types/call_agent.py
+-rw-r--r--   0        0        0      832 2023-07-21 01:39:03.499167 vocode_api-0.0.5a3/src/vocode/types/call_status.py
+-rw-r--r--   0        0        0      395 2023-07-21 01:39:03.499167 vocode_api-0.0.5a3/src/vocode/types/create_action_request.py
+-rw-r--r--   0        0        0      320 2023-07-21 01:39:03.499167 vocode_api-0.0.5a3/src/vocode/types/create_action_response.py
+-rw-r--r--   0        0        0      175 2023-07-21 01:39:03.499167 vocode_api-0.0.5a3/src/vocode/types/create_call_request_agent.py
+-rw-r--r--   0        0        0      329 2023-07-21 01:39:03.499167 vocode_api-0.0.5a3/src/vocode/types/create_voice_request.py
+-rw-r--r--   0        0        0      273 2023-07-21 01:39:03.499167 vocode_api-0.0.5a3/src/vocode/types/create_voice_response.py
+-rw-r--r--   0        0        0      931 2023-07-21 01:39:03.499167 vocode_api-0.0.5a3/src/vocode/types/dtmf_action.py
+-rw-r--r--   0        0        0      891 2023-07-21 01:39:03.499167 vocode_api-0.0.5a3/src/vocode/types/dtmf_action_params.py
+-rw-r--r--   0        0        0      932 2023-07-21 01:39:03.499167 vocode_api-0.0.5a3/src/vocode/types/dtmf_action_update_params.py
+-rw-r--r--   0        0        0      239 2023-07-21 01:39:03.499167 vocode_api-0.0.5a3/src/vocode/types/dtmf_action_update_params_config.py
+-rw-r--r--   0        0        0      953 2023-07-21 01:39:03.499167 vocode_api-0.0.5a3/src/vocode/types/eleven_labs_voice.py
+-rw-r--r--   0        0        0      913 2023-07-21 01:39:03.499167 vocode_api-0.0.5a3/src/vocode/types/eleven_labs_voice_params.py
+-rw-r--r--   0        0        0     1455 2023-07-21 01:39:03.499167 vocode_api-0.0.5a3/src/vocode/types/eleven_labs_voice_update_params.py
+-rw-r--r--   0        0        0      179 2023-07-21 01:39:03.499167 vocode_api-0.0.5a3/src/vocode/types/eleven_labs_voice_update_params_api_key.py
+-rw-r--r--   0        0        0      190 2023-07-21 01:39:03.499167 vocode_api-0.0.5a3/src/vocode/types/eleven_labs_voice_update_params_similarity_boost.py
+-rw-r--r--   0        0        0      184 2023-07-21 01:39:03.499167 vocode_api-0.0.5a3/src/vocode/types/eleven_labs_voice_update_params_stability.py
+-rw-r--r--   0        0        0      180 2023-07-21 01:39:03.499167 vocode_api-0.0.5a3/src/vocode/types/eleven_labs_voice_update_params_voice_id.py
+-rw-r--r--   0        0        0      736 2023-07-21 01:39:03.499167 vocode_api-0.0.5a3/src/vocode/types/empty_action_config.py
+-rw-r--r--   0        0        0      942 2023-07-21 01:39:03.499167 vocode_api-0.0.5a3/src/vocode/types/end_conversation_action.py
+-rw-r--r--   0        0        0      902 2023-07-21 01:39:03.499167 vocode_api-0.0.5a3/src/vocode/types/end_conversation_action_params.py
+-rw-r--r--   0        0        0      977 2023-07-21 01:39:03.499167 vocode_api-0.0.5a3/src/vocode/types/end_conversation_action_update_params.py
+-rw-r--r--   0        0        0      250 2023-07-21 01:39:03.499167 vocode_api-0.0.5a3/src/vocode/types/end_conversation_action_update_params_config.py
+-rw-r--r--   0        0        0     1395 2023-07-21 01:39:03.499167 vocode_api-0.0.5a3/src/vocode/types/event_type.py
+-rw-r--r--   0        0        0      317 2023-07-21 01:39:03.499167 vocode_api-0.0.5a3/src/vocode/types/get_action_response.py
+-rw-r--r--   0        0        0      270 2023-07-21 01:39:03.499167 vocode_api-0.0.5a3/src/vocode/types/get_voice_response.py
+-rw-r--r--   0        0        0      466 2023-07-21 01:39:03.499167 vocode_api-0.0.5a3/src/vocode/types/http_method.py
+-rw-r--r--   0        0        0      843 2023-07-21 01:39:03.499167 vocode_api-0.0.5a3/src/vocode/types/http_validation_error.py
+-rw-r--r--   0        0        0      323 2023-07-21 01:39:03.499167 vocode_api-0.0.5a3/src/vocode/types/list_actions_response_item.py
+-rw-r--r--   0        0        0      276 2023-07-21 01:39:03.499167 vocode_api-0.0.5a3/src/vocode/types/list_voices_response_item.py
+-rw-r--r--   0        0        0      900 2023-07-21 01:39:03.499167 vocode_api-0.0.5a3/src/vocode/types/phone_number.py
+-rw-r--r--   0        0        0      157 2023-07-21 01:39:03.499167 vocode_api-0.0.5a3/src/vocode/types/phone_number_inbound_agent.py
+-rw-r--r--   0        0        0      674 2023-07-21 01:39:03.499167 vocode_api-0.0.5a3/src/vocode/types/plan_type.py
+-rw-r--r--   0        0        0      846 2023-07-21 01:39:03.499167 vocode_api-0.0.5a3/src/vocode/types/rime_voice.py
+-rw-r--r--   0        0        0      806 2023-07-21 01:39:03.499167 vocode_api-0.0.5a3/src/vocode/types/rime_voice_params.py
+-rw-r--r--   0        0        0      929 2023-07-21 01:39:03.499167 vocode_api-0.0.5a3/src/vocode/types/rime_voice_update_params.py
+-rw-r--r--   0        0        0      174 2023-07-21 01:39:03.499167 vocode_api-0.0.5a3/src/vocode/types/rime_voice_update_params_speaker.py
+-rw-r--r--   0        0        0      925 2023-07-21 01:39:03.499167 vocode_api-0.0.5a3/src/vocode/types/transfer_call_action.py
+-rw-r--r--   0        0        0      965 2023-07-21 01:39:03.499167 vocode_api-0.0.5a3/src/vocode/types/transfer_call_action_update_params.py
+-rw-r--r--   0        0        0      250 2023-07-21 01:39:03.499167 vocode_api-0.0.5a3/src/vocode/types/transfer_call_action_update_params_config.py
+-rw-r--r--   0        0        0      760 2023-07-21 01:39:03.499167 vocode_api-0.0.5a3/src/vocode/types/transfer_call_config.py
+-rw-r--r--   0        0        0      728 2023-07-21 01:39:03.499167 vocode_api-0.0.5a3/src/vocode/types/undefined.py
+-rw-r--r--   0        0        0      443 2023-07-21 01:39:03.499167 vocode_api-0.0.5a3/src/vocode/types/update_action_request_body.py
+-rw-r--r--   0        0        0      320 2023-07-21 01:39:03.499167 vocode_api-0.0.5a3/src/vocode/types/update_action_response.py
+-rw-r--r--   0        0        0      203 2023-07-21 01:39:03.499167 vocode_api-0.0.5a3/src/vocode/types/update_number_request_inbound_agent.py
+-rw-r--r--   0        0        0      390 2023-07-21 01:39:03.499167 vocode_api-0.0.5a3/src/vocode/types/update_voice_request_body.py
+-rw-r--r--   0        0        0      273 2023-07-21 01:39:03.499167 vocode_api-0.0.5a3/src/vocode/types/update_voice_response.py
+-rw-r--r--   0        0        0      866 2023-07-21 01:39:03.499167 vocode_api-0.0.5a3/src/vocode/types/usage.py
+-rw-r--r--   0        0        0      869 2023-07-21 01:39:03.499167 vocode_api-0.0.5a3/src/vocode/types/validation_error.py
+-rw-r--r--   0        0        0      128 2023-07-21 01:39:03.499167 vocode_api-0.0.5a3/src/vocode/types/validation_error_loc_item.py
+-rw-r--r--   0        0        0      907 2023-07-21 01:39:03.499167 vocode_api-0.0.5a3/src/vocode/types/voice_type.py
+-rw-r--r--   0        0        0      921 2023-07-21 01:39:03.499167 vocode_api-0.0.5a3/src/vocode/types/webhook.py
+-rw-r--r--   0        0        0      898 2023-07-21 01:39:03.499167 vocode_api-0.0.5a3/src/vocode/types/webhook_params.py
+-rw-r--r--   0        0        0     1124 2023-07-21 01:39:03.499167 vocode_api-0.0.5a3/src/vocode/types/webhook_update_params.py
+-rw-r--r--   0        0        0      214 2023-07-21 01:39:03.499167 vocode_api-0.0.5a3/src/vocode/types/webhook_update_params_method.py
+-rw-r--r--   0        0        0      231 2023-07-21 01:39:03.499167 vocode_api-0.0.5a3/src/vocode/types/webhook_update_params_subscriptions.py
+-rw-r--r--   0        0        0      168 2023-07-21 01:39:03.499167 vocode_api-0.0.5a3/src/vocode/types/webhook_update_params_url.py
+-rw-r--r--   0        0        0     3187 1970-01-01 00:00:00.000000 vocode_api-0.0.5a3/PKG-INFO
```

### Comparing `vocode_api-0.0.5a2/README.md` & `vocode_api-0.0.5a3/README.md`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.5a2/src/vocode/__init__.py` & `vocode_api-0.0.5a3/src/vocode/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # This file was auto-generated by Fern from our API Definition.
 
+from .environment import VocodeEnvironment
 from .errors import UnprocessableEntityError
 from .resources import actions, agents, calls, numbers, usage, voices, webhooks
 from .types import (
     ActionType,
     Agent,
     AgentActionsItem,
     AgentParams,
@@ -156,14 +157,15 @@
     "UpdateActionResponse",
     "UpdateNumberRequestInboundAgent",
     "UpdateVoiceRequestBody",
     "UpdateVoiceResponse",
     "Usage",
     "ValidationError",
     "ValidationErrorLocItem",
+    "VocodeEnvironment",
     "VoiceType",
     "Webhook",
     "WebhookParams",
     "WebhookUpdateParams",
     "WebhookUpdateParamsMethod",
     "WebhookUpdateParamsSubscriptions",
     "WebhookUpdateParamsUrl",
```

### Comparing `vocode_api-0.0.5a2/src/vocode/client.py` & `vocode_api-0.0.5a3/src/vocode/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 # This file was auto-generated by Fern from our API Definition.
 
+from .environment import VocodeEnvironment
 from .resources.actions.client import ActionsClient, AsyncActionsClient
 from .resources.agents.client import AgentsClient, AsyncAgentsClient
 from .resources.calls.client import AsyncCallsClient, CallsClient
 from .resources.numbers.client import AsyncNumbersClient, NumbersClient
 from .resources.usage.client import AsyncUsageClient, UsageClient
 from .resources.voices.client import AsyncVoicesClient, VoicesClient
 from .resources.webhooks.client import AsyncWebhooksClient, WebhooksClient
 
 
 class Vocode:
-    def __init__(self, *, environment: str, token: str):
+    def __init__(self, *, environment: VocodeEnvironment = VocodeEnvironment.PRODUCTION, token: str):
         self._environment = environment
         self._token = token
         self.numbers = NumbersClient(environment=self._environment, token=self._token)
         self.calls = CallsClient(environment=self._environment, token=self._token)
         self.usage = UsageClient(environment=self._environment, token=self._token)
         self.actions = ActionsClient(environment=self._environment, token=self._token)
         self.agents = AgentsClient(environment=self._environment, token=self._token)
         self.voices = VoicesClient(environment=self._environment, token=self._token)
         self.webhooks = WebhooksClient(environment=self._environment, token=self._token)
 
 
 class AsyncVocode:
-    def __init__(self, *, environment: str, token: str):
+    def __init__(self, *, environment: VocodeEnvironment = VocodeEnvironment.PRODUCTION, token: str):
         self._environment = environment
         self._token = token
         self.numbers = AsyncNumbersClient(environment=self._environment, token=self._token)
         self.calls = AsyncCallsClient(environment=self._environment, token=self._token)
         self.usage = AsyncUsageClient(environment=self._environment, token=self._token)
         self.actions = AsyncActionsClient(environment=self._environment, token=self._token)
         self.agents = AsyncAgentsClient(environment=self._environment, token=self._token)
```

### Comparing `vocode_api-0.0.5a2/src/vocode/core/datetime_utils.py` & `vocode_api-0.0.5a3/src/vocode/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.5a2/src/vocode/core/jsonable_encoder.py` & `vocode_api-0.0.5a3/src/vocode/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.5a2/src/vocode/resources/actions/client.py` & `vocode_api-0.0.5a3/src/vocode/resources/actions/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,33 +6,34 @@
 
 import httpx
 import pydantic
 
 from ...core.api_error import ApiError
 from ...core.jsonable_encoder import jsonable_encoder
 from ...core.remove_none_from_headers import remove_none_from_headers
+from ...environment import VocodeEnvironment
 from ...errors.unprocessable_entity_error import UnprocessableEntityError
 from ...types.create_action_request import CreateActionRequest
 from ...types.create_action_response import CreateActionResponse
 from ...types.get_action_response import GetActionResponse
 from ...types.http_validation_error import HttpValidationError
 from ...types.list_actions_response_item import ListActionsResponseItem
 from ...types.update_action_request_body import UpdateActionRequestBody
 from ...types.update_action_response import UpdateActionResponse
 
 
 class ActionsClient:
-    def __init__(self, *, environment: str, token: str):
+    def __init__(self, *, environment: VocodeEnvironment = VocodeEnvironment.PRODUCTION, token: str):
         self._environment = environment
         self._token = token
 
     def get_action(self, *, id: str) -> GetActionResponse:
         _response = httpx.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", "v1/actions"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "v1/actions"),
             params={"id": id},
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
@@ -44,15 +45,15 @@
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def list_actions(self) -> typing.List[ListActionsResponseItem]:
         _response = httpx.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", "v1/actions/list"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "v1/actions/list"),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.List[ListActionsResponseItem], _response.json())  # type: ignore
@@ -61,15 +62,15 @@
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def create_action(self, *, request: CreateActionRequest) -> CreateActionResponse:
         _response = httpx.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment}/", "v1/actions/create"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "v1/actions/create"),
             json=jsonable_encoder(request),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
@@ -81,15 +82,15 @@
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def update_action(self, *, id: str, request: UpdateActionRequestBody) -> UpdateActionResponse:
         _response = httpx.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment}/", "v1/actions/update"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "v1/actions/update"),
             params={"id": id},
             json=jsonable_encoder(request),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
             timeout=60,
         )
@@ -101,23 +102,23 @@
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
 class AsyncActionsClient:
-    def __init__(self, *, environment: str, token: str):
+    def __init__(self, *, environment: VocodeEnvironment = VocodeEnvironment.PRODUCTION, token: str):
         self._environment = environment
         self._token = token
 
     async def get_action(self, *, id: str) -> GetActionResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
-                urllib.parse.urljoin(f"{self._environment}/", "v1/actions"),
+                urllib.parse.urljoin(f"{self._environment.value}/", "v1/actions"),
                 params={"id": id},
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
@@ -130,15 +131,15 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def list_actions(self) -> typing.List[ListActionsResponseItem]:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
-                urllib.parse.urljoin(f"{self._environment}/", "v1/actions/list"),
+                urllib.parse.urljoin(f"{self._environment.value}/", "v1/actions/list"),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.List[ListActionsResponseItem], _response.json())  # type: ignore
@@ -148,15 +149,15 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def create_action(self, *, request: CreateActionRequest) -> CreateActionResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
-                urllib.parse.urljoin(f"{self._environment}/", "v1/actions/create"),
+                urllib.parse.urljoin(f"{self._environment.value}/", "v1/actions/create"),
                 json=jsonable_encoder(request),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
@@ -169,15 +170,15 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def update_action(self, *, id: str, request: UpdateActionRequestBody) -> UpdateActionResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
-                urllib.parse.urljoin(f"{self._environment}/", "v1/actions/update"),
+                urllib.parse.urljoin(f"{self._environment.value}/", "v1/actions/update"),
                 params={"id": id},
                 json=jsonable_encoder(request),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
                 timeout=60,
             )
```

### Comparing `vocode_api-0.0.5a2/src/vocode/resources/agents/client.py` & `vocode_api-0.0.5a3/src/vocode/resources/agents/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,30 +6,31 @@
 
 import httpx
 import pydantic
 
 from ...core.api_error import ApiError
 from ...core.jsonable_encoder import jsonable_encoder
 from ...core.remove_none_from_headers import remove_none_from_headers
+from ...environment import VocodeEnvironment
 from ...errors.unprocessable_entity_error import UnprocessableEntityError
 from ...types.agent import Agent
 from ...types.agent_params import AgentParams
 from ...types.agent_update_params import AgentUpdateParams
 from ...types.http_validation_error import HttpValidationError
 
 
 class AgentsClient:
-    def __init__(self, *, environment: str, token: str):
+    def __init__(self, *, environment: VocodeEnvironment = VocodeEnvironment.PRODUCTION, token: str):
         self._environment = environment
         self._token = token
 
     def get_agent(self, *, id: str) -> Agent:
         _response = httpx.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", "v1/agents"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "v1/agents"),
             params={"id": id},
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
@@ -41,15 +42,15 @@
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def list_agents(self) -> typing.List[Agent]:
         _response = httpx.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", "v1/agents/list"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "v1/agents/list"),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.List[Agent], _response.json())  # type: ignore
@@ -58,15 +59,15 @@
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def create_agent(self, *, request: AgentParams) -> Agent:
         _response = httpx.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment}/", "v1/agents/create"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "v1/agents/create"),
             json=jsonable_encoder(request),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
@@ -78,15 +79,15 @@
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def update_agent(self, *, id: str, request: AgentUpdateParams) -> Agent:
         _response = httpx.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment}/", "v1/agents/update"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "v1/agents/update"),
             params={"id": id},
             json=jsonable_encoder(request),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
             timeout=60,
         )
@@ -98,23 +99,23 @@
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
 class AsyncAgentsClient:
-    def __init__(self, *, environment: str, token: str):
+    def __init__(self, *, environment: VocodeEnvironment = VocodeEnvironment.PRODUCTION, token: str):
         self._environment = environment
         self._token = token
 
     async def get_agent(self, *, id: str) -> Agent:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
-                urllib.parse.urljoin(f"{self._environment}/", "v1/agents"),
+                urllib.parse.urljoin(f"{self._environment.value}/", "v1/agents"),
                 params={"id": id},
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
@@ -127,15 +128,15 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def list_agents(self) -> typing.List[Agent]:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
-                urllib.parse.urljoin(f"{self._environment}/", "v1/agents/list"),
+                urllib.parse.urljoin(f"{self._environment.value}/", "v1/agents/list"),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.List[Agent], _response.json())  # type: ignore
@@ -145,15 +146,15 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def create_agent(self, *, request: AgentParams) -> Agent:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
-                urllib.parse.urljoin(f"{self._environment}/", "v1/agents/create"),
+                urllib.parse.urljoin(f"{self._environment.value}/", "v1/agents/create"),
                 json=jsonable_encoder(request),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
@@ -166,15 +167,15 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def update_agent(self, *, id: str, request: AgentUpdateParams) -> Agent:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
-                urllib.parse.urljoin(f"{self._environment}/", "v1/agents/update"),
+                urllib.parse.urljoin(f"{self._environment.value}/", "v1/agents/update"),
                 params={"id": id},
                 json=jsonable_encoder(request),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
                 timeout=60,
             )
```

### Comparing `vocode_api-0.0.5a2/src/vocode/resources/calls/client.py` & `vocode_api-0.0.5a3/src/vocode/resources/calls/client.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,29 +6,30 @@
 
 import httpx
 import pydantic
 
 from ...core.api_error import ApiError
 from ...core.jsonable_encoder import jsonable_encoder
 from ...core.remove_none_from_headers import remove_none_from_headers
+from ...environment import VocodeEnvironment
 from ...errors.unprocessable_entity_error import UnprocessableEntityError
 from ...types.call import Call
 from ...types.create_call_request_agent import CreateCallRequestAgent
 from ...types.http_validation_error import HttpValidationError
 
 
 class CallsClient:
-    def __init__(self, *, environment: str, token: str):
+    def __init__(self, *, environment: VocodeEnvironment = VocodeEnvironment.PRODUCTION, token: str):
         self._environment = environment
         self._token = token
 
     def list_calls(self) -> typing.List[Call]:
         _response = httpx.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", "v1/calls/list"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "v1/calls/list"),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.List[Call], _response.json())  # type: ignore
@@ -37,15 +38,15 @@
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def get_call(self, *, id: str) -> Call:
         _response = httpx.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", "v1/calls"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "v1/calls"),
             params={"id": id},
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
@@ -57,15 +58,15 @@
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def end_call(self, *, id: str) -> Call:
         _response = httpx.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment}/", "v1/calls/end"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "v1/calls/end"),
             params={"id": id},
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
@@ -77,15 +78,15 @@
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def create_call(self, *, from_number: str, to_number: str, goal: str, agent: CreateCallRequestAgent) -> Call:
         _response = httpx.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment}/", "v1/calls/create"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "v1/calls/create"),
             json=jsonable_encoder({"from_number": from_number, "to_number": to_number, "goal": goal, "agent": agent}),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
@@ -97,15 +98,15 @@
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def recording(self, *, id: str) -> typing.Any:
         _response = httpx.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", "v1/calls/recording"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "v1/calls/recording"),
             params={"id": id},
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
@@ -116,23 +117,23 @@
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
 class AsyncCallsClient:
-    def __init__(self, *, environment: str, token: str):
+    def __init__(self, *, environment: VocodeEnvironment = VocodeEnvironment.PRODUCTION, token: str):
         self._environment = environment
         self._token = token
 
     async def list_calls(self) -> typing.List[Call]:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
-                urllib.parse.urljoin(f"{self._environment}/", "v1/calls/list"),
+                urllib.parse.urljoin(f"{self._environment.value}/", "v1/calls/list"),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.List[Call], _response.json())  # type: ignore
@@ -142,15 +143,15 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def get_call(self, *, id: str) -> Call:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
-                urllib.parse.urljoin(f"{self._environment}/", "v1/calls"),
+                urllib.parse.urljoin(f"{self._environment.value}/", "v1/calls"),
                 params={"id": id},
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
@@ -163,15 +164,15 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def end_call(self, *, id: str) -> Call:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
-                urllib.parse.urljoin(f"{self._environment}/", "v1/calls/end"),
+                urllib.parse.urljoin(f"{self._environment.value}/", "v1/calls/end"),
                 params={"id": id},
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
@@ -184,15 +185,15 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def create_call(self, *, from_number: str, to_number: str, goal: str, agent: CreateCallRequestAgent) -> Call:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
-                urllib.parse.urljoin(f"{self._environment}/", "v1/calls/create"),
+                urllib.parse.urljoin(f"{self._environment.value}/", "v1/calls/create"),
                 json=jsonable_encoder(
                     {"from_number": from_number, "to_number": to_number, "goal": goal, "agent": agent}
                 ),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
                 timeout=60,
@@ -207,15 +208,15 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def recording(self, *, id: str) -> typing.Any:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
-                urllib.parse.urljoin(f"{self._environment}/", "v1/calls/recording"),
+                urllib.parse.urljoin(f"{self._environment.value}/", "v1/calls/recording"),
                 params={"id": id},
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
```

### Comparing `vocode_api-0.0.5a2/src/vocode/resources/numbers/client.py` & `vocode_api-0.0.5a3/src/vocode/resources/numbers/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,29 +6,30 @@
 
 import httpx
 import pydantic
 
 from ...core.api_error import ApiError
 from ...core.jsonable_encoder import jsonable_encoder
 from ...core.remove_none_from_headers import remove_none_from_headers
+from ...environment import VocodeEnvironment
 from ...errors.unprocessable_entity_error import UnprocessableEntityError
 from ...types.http_validation_error import HttpValidationError
 from ...types.phone_number import PhoneNumber
 from ...types.update_number_request_inbound_agent import UpdateNumberRequestInboundAgent
 
 
 class NumbersClient:
-    def __init__(self, *, environment: str, token: str):
+    def __init__(self, *, environment: VocodeEnvironment = VocodeEnvironment.PRODUCTION, token: str):
         self._environment = environment
         self._token = token
 
     def list_numbers(self) -> typing.List[PhoneNumber]:
         _response = httpx.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", "v1/numbers/list"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "v1/numbers/list"),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.List[PhoneNumber], _response.json())  # type: ignore
@@ -37,15 +38,15 @@
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def get_number(self, *, phone_number: str) -> PhoneNumber:
         _response = httpx.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", "v1/numbers"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "v1/numbers"),
             params={"phone_number": phone_number},
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
@@ -57,15 +58,15 @@
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def buy_number(self) -> PhoneNumber:
         _response = httpx.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment}/", "v1/numbers/buy"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "v1/numbers/buy"),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PhoneNumber, _response.json())  # type: ignore
@@ -74,15 +75,15 @@
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def update_number(self, *, phone_number: str, inbound_agent: UpdateNumberRequestInboundAgent) -> PhoneNumber:
         _response = httpx.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment}/", "v1/numbers/update"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "v1/numbers/update"),
             params={"phone_number": phone_number},
             json=jsonable_encoder({"inbound_agent": inbound_agent}),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
             timeout=60,
         )
@@ -95,15 +96,15 @@
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def cancel_number(self, *, phone_number: str) -> PhoneNumber:
         _response = httpx.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment}/", "v1/numbers/cancel"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "v1/numbers/cancel"),
             params={"phone_number": phone_number},
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
@@ -114,23 +115,23 @@
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
 class AsyncNumbersClient:
-    def __init__(self, *, environment: str, token: str):
+    def __init__(self, *, environment: VocodeEnvironment = VocodeEnvironment.PRODUCTION, token: str):
         self._environment = environment
         self._token = token
 
     async def list_numbers(self) -> typing.List[PhoneNumber]:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
-                urllib.parse.urljoin(f"{self._environment}/", "v1/numbers/list"),
+                urllib.parse.urljoin(f"{self._environment.value}/", "v1/numbers/list"),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.List[PhoneNumber], _response.json())  # type: ignore
@@ -140,15 +141,15 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def get_number(self, *, phone_number: str) -> PhoneNumber:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
-                urllib.parse.urljoin(f"{self._environment}/", "v1/numbers"),
+                urllib.parse.urljoin(f"{self._environment.value}/", "v1/numbers"),
                 params={"phone_number": phone_number},
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
@@ -161,15 +162,15 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def buy_number(self) -> PhoneNumber:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
-                urllib.parse.urljoin(f"{self._environment}/", "v1/numbers/buy"),
+                urllib.parse.urljoin(f"{self._environment.value}/", "v1/numbers/buy"),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PhoneNumber, _response.json())  # type: ignore
@@ -179,15 +180,15 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def update_number(self, *, phone_number: str, inbound_agent: UpdateNumberRequestInboundAgent) -> PhoneNumber:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
-                urllib.parse.urljoin(f"{self._environment}/", "v1/numbers/update"),
+                urllib.parse.urljoin(f"{self._environment.value}/", "v1/numbers/update"),
                 params={"phone_number": phone_number},
                 json=jsonable_encoder({"inbound_agent": inbound_agent}),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
                 timeout=60,
             )
@@ -201,15 +202,15 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def cancel_number(self, *, phone_number: str) -> PhoneNumber:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
-                urllib.parse.urljoin(f"{self._environment}/", "v1/numbers/cancel"),
+                urllib.parse.urljoin(f"{self._environment.value}/", "v1/numbers/cancel"),
                 params={"phone_number": phone_number},
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
```

### Comparing `vocode_api-0.0.5a2/src/vocode/resources/usage/client.py` & `vocode_api-0.0.5a3/src/vocode/resources/usage/client.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,26 +4,27 @@
 from json.decoder import JSONDecodeError
 
 import httpx
 import pydantic
 
 from ...core.api_error import ApiError
 from ...core.remove_none_from_headers import remove_none_from_headers
+from ...environment import VocodeEnvironment
 from ...types.usage import Usage
 
 
 class UsageClient:
-    def __init__(self, *, environment: str, token: str):
+    def __init__(self, *, environment: VocodeEnvironment = VocodeEnvironment.PRODUCTION, token: str):
         self._environment = environment
         self._token = token
 
     def get_usage(self) -> Usage:
         _response = httpx.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", "v1/usage"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "v1/usage"),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(Usage, _response.json())  # type: ignore
@@ -31,23 +32,23 @@
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
 class AsyncUsageClient:
-    def __init__(self, *, environment: str, token: str):
+    def __init__(self, *, environment: VocodeEnvironment = VocodeEnvironment.PRODUCTION, token: str):
         self._environment = environment
         self._token = token
 
     async def get_usage(self) -> Usage:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
-                urllib.parse.urljoin(f"{self._environment}/", "v1/usage"),
+                urllib.parse.urljoin(f"{self._environment.value}/", "v1/usage"),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(Usage, _response.json())  # type: ignore
```

### Comparing `vocode_api-0.0.5a2/src/vocode/resources/voices/client.py` & `vocode_api-0.0.5a3/src/vocode/resources/voices/client.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,33 +6,34 @@
 
 import httpx
 import pydantic
 
 from ...core.api_error import ApiError
 from ...core.jsonable_encoder import jsonable_encoder
 from ...core.remove_none_from_headers import remove_none_from_headers
+from ...environment import VocodeEnvironment
 from ...errors.unprocessable_entity_error import UnprocessableEntityError
 from ...types.create_voice_request import CreateVoiceRequest
 from ...types.create_voice_response import CreateVoiceResponse
 from ...types.get_voice_response import GetVoiceResponse
 from ...types.http_validation_error import HttpValidationError
 from ...types.list_voices_response_item import ListVoicesResponseItem
 from ...types.update_voice_request_body import UpdateVoiceRequestBody
 from ...types.update_voice_response import UpdateVoiceResponse
 
 
 class VoicesClient:
-    def __init__(self, *, environment: str, token: str):
+    def __init__(self, *, environment: VocodeEnvironment = VocodeEnvironment.PRODUCTION, token: str):
         self._environment = environment
         self._token = token
 
     def get_voice(self, *, id: str) -> GetVoiceResponse:
         _response = httpx.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", "v1/voices"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "v1/voices"),
             params={"id": id},
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
@@ -44,15 +45,15 @@
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def list_voices(self) -> typing.List[ListVoicesResponseItem]:
         _response = httpx.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", "v1/voices/list"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "v1/voices/list"),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.List[ListVoicesResponseItem], _response.json())  # type: ignore
@@ -61,15 +62,15 @@
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def create_voice(self, *, request: CreateVoiceRequest) -> CreateVoiceResponse:
         _response = httpx.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment}/", "v1/voices/create"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "v1/voices/create"),
             json=jsonable_encoder(request),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
@@ -81,15 +82,15 @@
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def update_voice(self, *, id: str, request: UpdateVoiceRequestBody) -> UpdateVoiceResponse:
         _response = httpx.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment}/", "v1/voices/update"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "v1/voices/update"),
             params={"id": id},
             json=jsonable_encoder(request),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
             timeout=60,
         )
@@ -101,23 +102,23 @@
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
 class AsyncVoicesClient:
-    def __init__(self, *, environment: str, token: str):
+    def __init__(self, *, environment: VocodeEnvironment = VocodeEnvironment.PRODUCTION, token: str):
         self._environment = environment
         self._token = token
 
     async def get_voice(self, *, id: str) -> GetVoiceResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
-                urllib.parse.urljoin(f"{self._environment}/", "v1/voices"),
+                urllib.parse.urljoin(f"{self._environment.value}/", "v1/voices"),
                 params={"id": id},
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
@@ -130,15 +131,15 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def list_voices(self) -> typing.List[ListVoicesResponseItem]:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
-                urllib.parse.urljoin(f"{self._environment}/", "v1/voices/list"),
+                urllib.parse.urljoin(f"{self._environment.value}/", "v1/voices/list"),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.List[ListVoicesResponseItem], _response.json())  # type: ignore
@@ -148,15 +149,15 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def create_voice(self, *, request: CreateVoiceRequest) -> CreateVoiceResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
-                urllib.parse.urljoin(f"{self._environment}/", "v1/voices/create"),
+                urllib.parse.urljoin(f"{self._environment.value}/", "v1/voices/create"),
                 json=jsonable_encoder(request),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
@@ -169,15 +170,15 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def update_voice(self, *, id: str, request: UpdateVoiceRequestBody) -> UpdateVoiceResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
-                urllib.parse.urljoin(f"{self._environment}/", "v1/voices/update"),
+                urllib.parse.urljoin(f"{self._environment.value}/", "v1/voices/update"),
                 params={"id": id},
                 json=jsonable_encoder(request),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
                 timeout=60,
             )
```

### Comparing `vocode_api-0.0.5a2/src/vocode/resources/webhooks/client.py` & `vocode_api-0.0.5a3/src/vocode/resources/webhooks/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,30 +6,31 @@
 
 import httpx
 import pydantic
 
 from ...core.api_error import ApiError
 from ...core.jsonable_encoder import jsonable_encoder
 from ...core.remove_none_from_headers import remove_none_from_headers
+from ...environment import VocodeEnvironment
 from ...errors.unprocessable_entity_error import UnprocessableEntityError
 from ...types.http_validation_error import HttpValidationError
 from ...types.webhook import Webhook
 from ...types.webhook_params import WebhookParams
 from ...types.webhook_update_params import WebhookUpdateParams
 
 
 class WebhooksClient:
-    def __init__(self, *, environment: str, token: str):
+    def __init__(self, *, environment: VocodeEnvironment = VocodeEnvironment.PRODUCTION, token: str):
         self._environment = environment
         self._token = token
 
     def get_webhook(self, *, id: str) -> Webhook:
         _response = httpx.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", "v1/webhooks"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "v1/webhooks"),
             params={"id": id},
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
@@ -41,15 +42,15 @@
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def list_webhooks(self) -> typing.List[Webhook]:
         _response = httpx.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", "v1/webhooks/list"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "v1/webhooks/list"),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.List[Webhook], _response.json())  # type: ignore
@@ -58,15 +59,15 @@
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def create_webhook(self, *, request: WebhookParams) -> Webhook:
         _response = httpx.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment}/", "v1/webhooks/create"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "v1/webhooks/create"),
             json=jsonable_encoder(request),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
@@ -78,15 +79,15 @@
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def update_webhook(self, *, id: str, request: WebhookUpdateParams) -> Webhook:
         _response = httpx.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment}/", "v1/webhooks/update"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "v1/webhooks/update"),
             params={"id": id},
             json=jsonable_encoder(request),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
             timeout=60,
         )
@@ -98,23 +99,23 @@
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
 class AsyncWebhooksClient:
-    def __init__(self, *, environment: str, token: str):
+    def __init__(self, *, environment: VocodeEnvironment = VocodeEnvironment.PRODUCTION, token: str):
         self._environment = environment
         self._token = token
 
     async def get_webhook(self, *, id: str) -> Webhook:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
-                urllib.parse.urljoin(f"{self._environment}/", "v1/webhooks"),
+                urllib.parse.urljoin(f"{self._environment.value}/", "v1/webhooks"),
                 params={"id": id},
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
@@ -127,15 +128,15 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def list_webhooks(self) -> typing.List[Webhook]:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
-                urllib.parse.urljoin(f"{self._environment}/", "v1/webhooks/list"),
+                urllib.parse.urljoin(f"{self._environment.value}/", "v1/webhooks/list"),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.List[Webhook], _response.json())  # type: ignore
@@ -145,15 +146,15 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def create_webhook(self, *, request: WebhookParams) -> Webhook:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
-                urllib.parse.urljoin(f"{self._environment}/", "v1/webhooks/create"),
+                urllib.parse.urljoin(f"{self._environment.value}/", "v1/webhooks/create"),
                 json=jsonable_encoder(request),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
@@ -166,15 +167,15 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def update_webhook(self, *, id: str, request: WebhookUpdateParams) -> Webhook:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
-                urllib.parse.urljoin(f"{self._environment}/", "v1/webhooks/update"),
+                urllib.parse.urljoin(f"{self._environment.value}/", "v1/webhooks/update"),
                 params={"id": id},
                 json=jsonable_encoder(request),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
                 timeout=60,
             )
```

### Comparing `vocode_api-0.0.5a2/src/vocode/types/__init__.py` & `vocode_api-0.0.5a3/src/vocode/types/__init__.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.5a2/src/vocode/types/action_type.py` & `vocode_api-0.0.5a3/src/vocode/types/action_type.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.5a2/src/vocode/types/agent.py` & `vocode_api-0.0.5a3/src/vocode/types/agent.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.5a2/src/vocode/types/agent_params.py` & `vocode_api-0.0.5a3/src/vocode/types/agent_params.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.5a2/src/vocode/types/agent_update_params.py` & `vocode_api-0.0.5a3/src/vocode/types/agent_update_params.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.5a2/src/vocode/types/azure_voice.py` & `vocode_api-0.0.5a3/src/vocode/types/azure_voice.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.5a2/src/vocode/types/azure_voice_params.py` & `vocode_api-0.0.5a3/src/vocode/types/azure_voice_params.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.5a2/src/vocode/types/azure_voice_update_params.py` & `vocode_api-0.0.5a3/src/vocode/types/azure_voice_update_params.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.5a2/src/vocode/types/call.py` & `vocode_api-0.0.5a3/src/vocode/types/call.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.5a2/src/vocode/types/call_status.py` & `vocode_api-0.0.5a3/src/vocode/types/call_status.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.5a2/src/vocode/types/dtmf_action.py` & `vocode_api-0.0.5a3/src/vocode/types/dtmf_action.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.5a2/src/vocode/types/dtmf_action_params.py` & `vocode_api-0.0.5a3/src/vocode/types/dtmf_action_params.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.5a2/src/vocode/types/dtmf_action_update_params.py` & `vocode_api-0.0.5a3/src/vocode/types/dtmf_action_update_params.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.5a2/src/vocode/types/eleven_labs_voice.py` & `vocode_api-0.0.5a3/src/vocode/types/eleven_labs_voice.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.5a2/src/vocode/types/eleven_labs_voice_params.py` & `vocode_api-0.0.5a3/src/vocode/types/eleven_labs_voice_params.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.5a2/src/vocode/types/eleven_labs_voice_update_params.py` & `vocode_api-0.0.5a3/src/vocode/types/eleven_labs_voice_update_params.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.5a2/src/vocode/types/empty_action_config.py` & `vocode_api-0.0.5a3/src/vocode/types/empty_action_config.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.5a2/src/vocode/types/end_conversation_action.py` & `vocode_api-0.0.5a3/src/vocode/types/end_conversation_action.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.5a2/src/vocode/types/end_conversation_action_params.py` & `vocode_api-0.0.5a3/src/vocode/types/end_conversation_action_params.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.5a2/src/vocode/types/end_conversation_action_update_params.py` & `vocode_api-0.0.5a3/src/vocode/types/end_conversation_action_update_params.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.5a2/src/vocode/types/event_type.py` & `vocode_api-0.0.5a3/src/vocode/types/event_type.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.5a2/src/vocode/types/http_validation_error.py` & `vocode_api-0.0.5a3/src/vocode/types/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.5a2/src/vocode/types/phone_number.py` & `vocode_api-0.0.5a3/src/vocode/types/phone_number.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.5a2/src/vocode/types/plan_type.py` & `vocode_api-0.0.5a3/src/vocode/types/plan_type.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.5a2/src/vocode/types/rime_voice.py` & `vocode_api-0.0.5a3/src/vocode/types/rime_voice.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.5a2/src/vocode/types/rime_voice_params.py` & `vocode_api-0.0.5a3/src/vocode/types/rime_voice_params.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.5a2/src/vocode/types/rime_voice_update_params.py` & `vocode_api-0.0.5a3/src/vocode/types/rime_voice_update_params.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.5a2/src/vocode/types/transfer_call_action.py` & `vocode_api-0.0.5a3/src/vocode/types/transfer_call_action.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.5a2/src/vocode/types/transfer_call_action_update_params.py` & `vocode_api-0.0.5a3/src/vocode/types/transfer_call_action_update_params.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.5a2/src/vocode/types/transfer_call_config.py` & `vocode_api-0.0.5a3/src/vocode/types/transfer_call_config.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.5a2/src/vocode/types/undefined.py` & `vocode_api-0.0.5a3/src/vocode/types/undefined.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.5a2/src/vocode/types/usage.py` & `vocode_api-0.0.5a3/src/vocode/types/usage.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.5a2/src/vocode/types/validation_error.py` & `vocode_api-0.0.5a3/src/vocode/types/validation_error.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.5a2/src/vocode/types/voice_type.py` & `vocode_api-0.0.5a3/src/vocode/types/voice_type.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.5a2/src/vocode/types/webhook.py` & `vocode_api-0.0.5a3/src/vocode/types/webhook.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.5a2/src/vocode/types/webhook_params.py` & `vocode_api-0.0.5a3/src/vocode/types/webhook_params.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.5a2/src/vocode/types/webhook_update_params.py` & `vocode_api-0.0.5a3/src/vocode/types/webhook_update_params.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.5a2/PKG-INFO` & `vocode_api-0.0.5a3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vocode-api
-Version: 0.0.5a2
+Version: 0.0.5a3
 Summary: 
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

