# Comparing `tmp/swibots-1.3.7.tar.gz` & `tmp/swibots-1.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swibots-1.3.7.tar", last modified: Thu Jul 20 18:24:02 2023, max compression
+gzip compressed data, was "swibots-1.3.8.tar", last modified: Fri Jul 21 18:02:41 2023, max compression
```

## Comparing `swibots-1.3.7.tar` & `swibots-1.3.8.tar`

### file list

```diff
@@ -1,238 +1,250 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-07-20 18:24:02.110951 swibots-1.3.7/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1817 2023-07-20 18:24:02.110951 swibots-1.3.7/PKG-INFO
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1538 2023-07-15 16:34:05.000000 swibots-1.3.7/README.md
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       38 2023-07-20 18:24:02.110951 swibots-1.3.7/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      809 2023-07-20 18:23:50.000000 swibots-1.3.7/setup.py
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-07-20 18:24:02.086951 swibots-1.3.7/swibots/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      236 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/__init__.py
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-07-20 18:24:02.090951 swibots-1.3.7/swibots/api/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      140 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/api/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     2236 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/api/api_client.py
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-07-20 18:24:02.090951 swibots-1.3.7/swibots/api/auth/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       85 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/api/auth/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1220 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/api/auth/auth_client.py
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-07-20 18:24:02.090951 swibots-1.3.7/swibots/api/auth/controllers/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       73 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/api/auth/controllers/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1518 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/api/auth/controllers/user_controller.py
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-07-20 18:24:02.090951 swibots-1.3.7/swibots/api/auth/methods/
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)       94 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/api/auth/methods/__init__.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      650 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/api/auth/methods/get_me.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      837 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/api/auth/methods/login.py
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-07-20 18:24:02.090951 swibots-1.3.7/swibots/api/auth/models/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       56 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/api/auth/models/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     4642 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/api/auth/models/auth_user.py
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-07-20 18:24:02.090951 swibots-1.3.7/swibots/api/bot/
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)       83 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/api/bot/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1141 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/api/bot/bot_client.py
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-07-20 18:24:02.090951 swibots-1.3.7/swibots/api/bot/controllers/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       71 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/api/bot/controllers/__init__.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     1790 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/api/bot/controllers/bot_controller.py
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-07-20 18:24:02.090951 swibots-1.3.7/swibots/api/bot/methods/
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      209 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/api/bot/methods/__init__.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      540 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/api/bot/methods/delete_bot_info.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      582 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/api/bot/methods/get_bot_info.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      615 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/api/bot/methods/update_bot_info.py
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-07-20 18:24:02.090951 swibots-1.3.7/swibots/api/bot/models/
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      116 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/api/bot/models/__init__.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      955 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/api/bot/models/bot_command_info.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     1585 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/api/bot/models/bot_info.py
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-07-20 18:24:02.090951 swibots-1.3.7/swibots/api/chat/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      107 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/api/chat/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     5372 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/api/chat/chat_client.py
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-07-20 18:24:02.090951 swibots-1.3.7/swibots/api/chat/controllers/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       83 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/api/chat/controllers/__init__.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)    22730 2023-07-20 18:23:50.000000 swibots-1.3.7/swibots/api/chat/controllers/message_controller.py
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-07-20 18:24:02.094951 swibots-1.3.7/swibots/api/chat/events/
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      326 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/api/chat/events/__init__.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     2073 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/api/chat/events/callback_query_event.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     2731 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/api/chat/events/chat_event.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     2095 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/api/chat/events/command_event.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     2103 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/api/chat/events/inline_query_event.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     2434 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/api/chat/events/message_event.py
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-07-20 18:24:02.094951 swibots-1.3.7/swibots/api/chat/methods/
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     1709 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/api/chat/methods/__init__.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      654 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/api/chat/methods/answer_inline_query.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      693 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/api/chat/methods/clear_conversation.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      705 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/api/chat/methods/delete_message.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      707 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/api/chat/methods/delete_messages_from_user.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     1358 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/api/chat/methods/download_media.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      750 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/api/chat/methods/edit_message.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      853 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/api/chat/methods/edit_message_text.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      693 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/api/chat/methods/flag_message.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     1222 2023-07-17 15:05:23.000000 swibots-1.3.7/swibots/api/chat/methods/forward_message.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     1139 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/api/chat/methods/get_channel_chat_history.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      725 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/api/chat/methods/get_community_media_files.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      883 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/api/chat/methods/get_community_media_files_by_status.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      636 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/api/chat/methods/get_flag_messages.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     1090 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/api/chat/methods/get_group_chat_history.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      649 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/api/chat/methods/get_message.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      707 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/api/chat/methods/get_messages.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     1102 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/api/chat/methods/get_messages_between_users.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      560 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/api/chat/methods/get_unread_messages_count.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      785 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/api/chat/methods/get_user_media_files.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      912 2023-07-17 15:05:23.000000 swibots-1.3.7/swibots/api/chat/methods/reply_message.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     1063 2023-07-17 15:05:23.000000 swibots-1.3.7/swibots/api/chat/methods/reply_message_text.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      880 2023-07-17 15:05:23.000000 swibots-1.3.7/swibots/api/chat/methods/send_message.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     1136 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/api/chat/methods/send_text.py
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-07-20 18:24:02.098951 swibots-1.3.7/swibots/api/chat/models/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      305 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/api/chat/models/__init__.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      920 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/api/chat/models/group_chat_history.py
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-07-20 18:24:02.098951 swibots-1.3.7/swibots/api/chat/models/inline/
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      565 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/api/chat/models/inline/__init__.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     1371 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/api/chat/models/inline/base_typed_inline_query_result.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     2533 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/api/chat/models/inline/inline_query.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     1871 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/api/chat/models/inline/inline_query_answer.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      991 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/api/chat/models/inline/inline_query_result.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     1158 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/api/chat/models/inline/inline_query_result_article.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1273 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/api/chat/models/inline/inline_query_result_document.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1620 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/api/chat/models/inline/inline_query_result_photo.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1760 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/api/chat/models/inline/inline_query_result_video.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      581 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/api/chat/models/inline/input_message_content.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      201 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/api/chat/models/inline/types.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      853 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/api/chat/models/inline_keyboard_button.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      170 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/api/chat/models/inline_keyboard_color.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      146 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/api/chat/models/inline_keyboard_size.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     2864 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/api/chat/models/inline_markup.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)    13484 2023-07-20 18:23:50.000000 swibots-1.3.7/swibots/api/chat/models/message.py
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-07-20 18:24:02.098951 swibots-1.3.7/swibots/api/common/
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)       44 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/api/common/__init__.py
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-07-20 18:24:02.098951 swibots-1.3.7/swibots/api/common/events/
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)       46 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/api/common/events/__init__.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     2922 2023-07-20 06:32:08.000000 swibots-1.3.7/swibots/api/common/events/event.py
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-07-20 18:24:02.098951 swibots-1.3.7/swibots/api/common/models/
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      191 2023-07-17 15:05:23.000000 swibots-1.3.7/swibots/api/common/models/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      562 2023-07-17 15:05:23.000000 swibots-1.3.7/swibots/api/common/models/embed_inline_field.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     3248 2023-07-17 15:05:23.000000 swibots-1.3.7/swibots/api/common/models/embedded_media.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     2004 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/api/common/models/media.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     1603 2023-07-17 15:05:23.000000 swibots-1.3.7/swibots/api/common/models/media_upload_request.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     1725 2023-07-17 15:05:23.000000 swibots-1.3.7/swibots/api/common/models/user.py
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-07-20 18:24:02.098951 swibots-1.3.7/swibots/api/community/
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)       90 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/api/community/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     6693 2023-07-20 06:32:08.000000 swibots-1.3.7/swibots/api/community/community_client.py
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-07-20 18:24:02.098951 swibots-1.3.7/swibots/api/community/controllers/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      273 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/api/community/controllers/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1005 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/api/community/controllers/ban_controller.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      978 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/api/community/controllers/channel_controller.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     1867 2023-07-17 15:05:23.000000 swibots-1.3.7/swibots/api/community/controllers/community_controller.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      576 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/api/community/controllers/group_controller.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     2221 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/api/community/controllers/permissions_controller.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1633 2023-07-20 06:32:08.000000 swibots-1.3.7/swibots/api/community/controllers/restrict_controller.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1981 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/api/community/controllers/rolemember_controller.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1860 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/api/community/controllers/roles_controller.py
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-07-20 18:24:02.102951 swibots-1.3.7/swibots/api/community/events/
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      566 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/api/community/events/__init__.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     1387 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/api/community/events/channel_created_event.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     1387 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/api/community/events/channel_deleted_event.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     1387 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/api/community/events/channel_updated_event.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     2404 2023-07-17 15:05:23.000000 swibots-1.3.7/swibots/api/community/events/community_event.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     1383 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/api/community/events/community_updated_event.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     1381 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/api/community/events/group_created_event.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     1381 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/api/community/events/group_deleted_event.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     1381 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/api/community/events/group_updated_event.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     1380 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/api/community/events/member_joined_event.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     1377 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/api/community/events/member_left_event.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     1373 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/api/community/events/user_banned_event.py
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-07-20 18:24:02.102951 swibots-1.3.7/swibots/api/community/methods/
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      765 2023-07-20 06:32:08.000000 swibots-1.3.7/swibots/api/community/methods/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      450 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/api/community/methods/ban_user.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      637 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/api/community/methods/create_channel.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      815 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/api/community/methods/deduct_xp.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      643 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/api/community/methods/get_channel.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      866 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/api/community/methods/get_community.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      522 2023-07-17 15:05:23.000000 swibots-1.3.7/swibots/api/community/methods/get_community_member.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      619 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/api/community/methods/get_group.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     2946 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/api/community/methods/permission.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     2418 2023-07-20 06:32:08.000000 swibots-1.3.7/swibots/api/community/methods/restrict_user.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     2259 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/api/community/methods/rolemember.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     2222 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/api/community/methods/roles.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      686 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/api/community/methods/unban_user.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      637 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/api/community/methods/update_channel.py
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-07-20 18:24:02.106951 swibots-1.3.7/swibots/api/community/models/
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      439 2023-07-20 06:32:08.000000 swibots-1.3.7/swibots/api/community/models/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      733 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/api/community/models/baninfo.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     3563 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/api/community/models/channel.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     2954 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/api/community/models/community.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     2998 2023-07-17 15:05:23.000000 swibots-1.3.7/swibots/api/community/models/community_member.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     2720 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/api/community/models/group.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1460 2023-07-20 06:32:08.000000 swibots-1.3.7/swibots/api/community/models/restricteduser.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1218 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/api/community/models/role.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1464 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/api/community/models/rolemember.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     3176 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/api/community/models/rolepermission.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     9347 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/app.py
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-07-20 18:24:02.106951 swibots-1.3.7/swibots/base/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      262 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/base/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       69 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/base/rest_controller.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      370 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/base/rest_request.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      644 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/base/rest_response.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     4261 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/base/switch_client.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1180 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/base/switch_object.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      543 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/base/switch_ws_async_client.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     4598 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/bot_app.py
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-07-20 18:24:02.106951 swibots-1.3.7/swibots/bots/
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      201 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/bots/__init__.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     4646 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/bots/bot.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     1646 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/bots/bot_context.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      109 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/bots/constants.py
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-07-20 18:24:02.106951 swibots-1.3.7/swibots/bots/decorators/
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      999 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/bots/decorators/__init__.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      540 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/bots/decorators/on_callback_query.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      510 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/bots/decorators/on_channel_created.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      544 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/bots/decorators/on_channel_deleted.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      541 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/bots/decorators/on_channel_updated.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      574 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/bots/decorators/on_command.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      544 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/bots/decorators/on_community_updated.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      536 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/bots/decorators/on_group_created.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      536 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/bots/decorators/on_group_deleted.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      534 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/bots/decorators/on_group_updated.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      537 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/bots/decorators/on_inline_query.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      534 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/bots/decorators/on_member_joined.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      529 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/bots/decorators/on_member_left.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      503 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/bots/decorators/on_message.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      543 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/bots/decorators/on_unknown_command.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      509 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/bots/decorators/on_user_banned.py
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-07-20 18:24:02.106951 swibots-1.3.7/swibots/bots/filters/
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)       22 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/bots/filters/__init__.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     7785 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/bots/filters/filter.py
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-07-20 18:24:02.110951 swibots-1.3.7/swibots/bots/handlers/
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     1300 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/bots/handlers/__init__.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     1048 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/bots/handlers/base_handler.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      985 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/bots/handlers/callback_query_handler.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      681 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/bots/handlers/channel_created_handler.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      688 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/bots/handlers/channel_deleted_handler.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      734 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/bots/handlers/channel_updated_handler.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     1514 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/bots/handlers/command_handler.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      686 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/bots/handlers/community_updated_handler.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     1325 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/bots/handlers/event_handler.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      680 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/bots/handlers/group_created_handler.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      775 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/bots/handlers/group_deleted_handler.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      775 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/bots/handlers/group_updated_handler.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      867 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/bots/handlers/inline_query_handler.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      679 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/bots/handlers/member_joined_handler.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      674 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/bots/handlers/member_left_handler.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      960 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/bots/handlers/message_handler.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      885 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/bots/handlers/unknown_command_handler.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      670 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/bots/handlers/user_banned_handler.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      285 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/bots/register_command.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     1645 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/config.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1333 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/error.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      973 2023-07-20 06:32:08.000000 swibots-1.3.7/swibots/types.py
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-07-20 18:24:02.110951 swibots-1.3.7/swibots/utils/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       75 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/utils/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     5883 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/utils/rest_client.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     2684 2023-07-17 15:05:23.000000 swibots-1.3.7/swibots/utils/types.py
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-07-20 18:24:02.110951 swibots-1.3.7/swibots/utils/ws/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       48 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/utils/ws/__init__.py
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-07-20 18:24:02.110951 swibots-1.3.7/swibots/utils/ws/asyncstomp/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      150 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/utils/ws/asyncstomp/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     9787 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/utils/ws/asyncstomp/async_ws_client.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      980 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/utils/ws/asyncstomp/async_ws_subscription.py
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-07-20 18:24:02.110951 swibots-1.3.7/swibots/utils/ws/common/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      100 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/utils/ws/common/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1654 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/utils/ws/common/ws_frame.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      430 2023-07-15 16:34:05.000000 swibots-1.3.7/swibots/utils/ws/common/ws_message.py
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-07-20 18:24:02.090951 swibots-1.3.7/swibots.egg-info/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1817 2023-07-20 18:24:02.000000 swibots-1.3.7/swibots.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     8373 2023-07-20 18:24:02.000000 swibots-1.3.7/swibots.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2023-07-20 18:24:02.000000 swibots-1.3.7/swibots.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2023-07-20 18:24:02.000000 swibots-1.3.7/swibots.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        8 2023-07-20 18:24:02.000000 swibots-1.3.7/swibots.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-07-21 18:02:41.310771 swibots-1.3.8/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1817 2023-07-21 18:02:41.310771 swibots-1.3.8/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1538 2023-07-15 16:34:05.000000 swibots-1.3.8/README.md
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       38 2023-07-21 18:02:41.310771 swibots-1.3.8/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      809 2023-07-21 18:02:28.000000 swibots-1.3.8/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-07-21 18:02:41.178771 swibots-1.3.8/swibots/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      236 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/__init__.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-07-21 18:02:41.182771 swibots-1.3.8/swibots/api/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      162 2023-07-21 18:02:28.000000 swibots-1.3.8/swibots/api/__init__.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-07-21 18:02:41.182771 swibots-1.3.8/swibots/api/airdrop/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      105 2023-07-21 18:02:28.000000 swibots-1.3.8/swibots/api/airdrop/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      911 2023-07-21 18:02:28.000000 swibots-1.3.8/swibots/api/airdrop/client.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-07-21 18:02:41.182771 swibots-1.3.8/swibots/api/airdrop/controllers/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       55 2023-07-21 18:02:28.000000 swibots-1.3.8/swibots/api/airdrop/controllers/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      780 2023-07-21 18:02:28.000000 swibots-1.3.8/swibots/api/airdrop/controllers/tournament_controller.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-07-21 18:02:41.182771 swibots-1.3.8/swibots/api/airdrop/methods/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       90 2023-07-21 18:02:28.000000 swibots-1.3.8/swibots/api/airdrop/methods/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      458 2023-07-21 18:02:28.000000 swibots-1.3.8/swibots/api/airdrop/methods/get_referral.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-07-21 18:02:41.182771 swibots-1.3.8/swibots/api/airdrop/models/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       54 2023-07-21 18:02:28.000000 swibots-1.3.8/swibots/api/airdrop/models/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1244 2023-07-21 18:02:28.000000 swibots-1.3.8/swibots/api/airdrop/models/referral.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     2616 2023-07-21 18:02:28.000000 swibots-1.3.8/swibots/api/api_client.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-07-21 18:02:41.182771 swibots-1.3.8/swibots/api/auth/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       85 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/api/auth/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1220 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/api/auth/auth_client.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-07-21 18:02:41.186771 swibots-1.3.8/swibots/api/auth/controllers/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       73 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/api/auth/controllers/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1518 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/api/auth/controllers/user_controller.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-07-21 18:02:41.186771 swibots-1.3.8/swibots/api/auth/methods/
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)       94 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/api/auth/methods/__init__.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      650 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/api/auth/methods/get_me.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      837 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/api/auth/methods/login.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-07-21 18:02:41.190771 swibots-1.3.8/swibots/api/auth/models/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       56 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/api/auth/models/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     4642 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/api/auth/models/auth_user.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-07-21 18:02:41.190771 swibots-1.3.8/swibots/api/bot/
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)       83 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/api/bot/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1141 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/api/bot/bot_client.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-07-21 18:02:41.190771 swibots-1.3.8/swibots/api/bot/controllers/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       71 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/api/bot/controllers/__init__.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     1790 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/api/bot/controllers/bot_controller.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-07-21 18:02:41.194771 swibots-1.3.8/swibots/api/bot/methods/
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      209 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/api/bot/methods/__init__.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      540 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/api/bot/methods/delete_bot_info.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      582 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/api/bot/methods/get_bot_info.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      615 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/api/bot/methods/update_bot_info.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-07-21 18:02:41.198771 swibots-1.3.8/swibots/api/bot/models/
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      116 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/api/bot/models/__init__.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      955 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/api/bot/models/bot_command_info.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     1585 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/api/bot/models/bot_info.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-07-21 18:02:41.198771 swibots-1.3.8/swibots/api/chat/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      107 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/api/chat/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     5372 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/api/chat/chat_client.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-07-21 18:02:41.198771 swibots-1.3.8/swibots/api/chat/controllers/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       83 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/api/chat/controllers/__init__.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)    22730 2023-07-20 18:23:50.000000 swibots-1.3.8/swibots/api/chat/controllers/message_controller.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-07-21 18:02:41.202771 swibots-1.3.8/swibots/api/chat/events/
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      326 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/api/chat/events/__init__.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     2073 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/api/chat/events/callback_query_event.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     2731 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/api/chat/events/chat_event.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     2095 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/api/chat/events/command_event.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     2103 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/api/chat/events/inline_query_event.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     2434 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/api/chat/events/message_event.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-07-21 18:02:41.218771 swibots-1.3.8/swibots/api/chat/methods/
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     1709 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/api/chat/methods/__init__.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      654 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/api/chat/methods/answer_inline_query.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      693 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/api/chat/methods/clear_conversation.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      705 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/api/chat/methods/delete_message.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      707 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/api/chat/methods/delete_messages_from_user.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     1358 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/api/chat/methods/download_media.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      750 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/api/chat/methods/edit_message.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      853 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/api/chat/methods/edit_message_text.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      693 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/api/chat/methods/flag_message.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     1222 2023-07-17 15:05:23.000000 swibots-1.3.8/swibots/api/chat/methods/forward_message.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     1139 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/api/chat/methods/get_channel_chat_history.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      725 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/api/chat/methods/get_community_media_files.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      883 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/api/chat/methods/get_community_media_files_by_status.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      636 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/api/chat/methods/get_flag_messages.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     1090 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/api/chat/methods/get_group_chat_history.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      649 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/api/chat/methods/get_message.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      707 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/api/chat/methods/get_messages.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     1102 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/api/chat/methods/get_messages_between_users.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      560 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/api/chat/methods/get_unread_messages_count.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      785 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/api/chat/methods/get_user_media_files.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      912 2023-07-17 15:05:23.000000 swibots-1.3.8/swibots/api/chat/methods/reply_message.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     1063 2023-07-17 15:05:23.000000 swibots-1.3.8/swibots/api/chat/methods/reply_message_text.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      880 2023-07-17 15:05:23.000000 swibots-1.3.8/swibots/api/chat/methods/send_message.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     1136 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/api/chat/methods/send_text.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-07-21 18:02:41.226771 swibots-1.3.8/swibots/api/chat/models/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      305 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/api/chat/models/__init__.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      920 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/api/chat/models/group_chat_history.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-07-21 18:02:41.230771 swibots-1.3.8/swibots/api/chat/models/inline/
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      565 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/api/chat/models/inline/__init__.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     1371 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/api/chat/models/inline/base_typed_inline_query_result.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     2533 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/api/chat/models/inline/inline_query.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     1871 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/api/chat/models/inline/inline_query_answer.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      991 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/api/chat/models/inline/inline_query_result.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     1158 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/api/chat/models/inline/inline_query_result_article.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1273 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/api/chat/models/inline/inline_query_result_document.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1620 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/api/chat/models/inline/inline_query_result_photo.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1760 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/api/chat/models/inline/inline_query_result_video.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      581 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/api/chat/models/inline/input_message_content.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      201 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/api/chat/models/inline/types.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      853 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/api/chat/models/inline_keyboard_button.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      170 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/api/chat/models/inline_keyboard_color.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      146 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/api/chat/models/inline_keyboard_size.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     2864 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/api/chat/models/inline_markup.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)    13484 2023-07-20 18:23:50.000000 swibots-1.3.8/swibots/api/chat/models/message.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-07-21 18:02:41.230771 swibots-1.3.8/swibots/api/common/
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)       44 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/api/common/__init__.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-07-21 18:02:41.234771 swibots-1.3.8/swibots/api/common/events/
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)       46 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/api/common/events/__init__.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     2922 2023-07-20 06:32:08.000000 swibots-1.3.8/swibots/api/common/events/event.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-07-21 18:02:41.234771 swibots-1.3.8/swibots/api/common/models/
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      191 2023-07-17 15:05:23.000000 swibots-1.3.8/swibots/api/common/models/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      562 2023-07-17 15:05:23.000000 swibots-1.3.8/swibots/api/common/models/embed_inline_field.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     3223 2023-07-21 18:02:28.000000 swibots-1.3.8/swibots/api/common/models/embedded_media.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     2004 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/api/common/models/media.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     1603 2023-07-17 15:05:23.000000 swibots-1.3.8/swibots/api/common/models/media_upload_request.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     1879 2023-07-21 18:02:28.000000 swibots-1.3.8/swibots/api/common/models/user.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-07-21 18:02:41.234771 swibots-1.3.8/swibots/api/community/
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)       90 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/api/community/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     6693 2023-07-20 06:32:08.000000 swibots-1.3.8/swibots/api/community/community_client.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-07-21 18:02:41.242771 swibots-1.3.8/swibots/api/community/controllers/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      273 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/api/community/controllers/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1005 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/api/community/controllers/ban_controller.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      978 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/api/community/controllers/channel_controller.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     1867 2023-07-17 15:05:23.000000 swibots-1.3.8/swibots/api/community/controllers/community_controller.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      576 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/api/community/controllers/group_controller.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     2221 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/api/community/controllers/permissions_controller.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1633 2023-07-20 06:32:08.000000 swibots-1.3.8/swibots/api/community/controllers/restrict_controller.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1981 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/api/community/controllers/rolemember_controller.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1860 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/api/community/controllers/roles_controller.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-07-21 18:02:41.250771 swibots-1.3.8/swibots/api/community/events/
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      566 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/api/community/events/__init__.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     1387 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/api/community/events/channel_created_event.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     1387 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/api/community/events/channel_deleted_event.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     1387 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/api/community/events/channel_updated_event.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     2404 2023-07-17 15:05:23.000000 swibots-1.3.8/swibots/api/community/events/community_event.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     1383 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/api/community/events/community_updated_event.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     1381 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/api/community/events/group_created_event.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     1381 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/api/community/events/group_deleted_event.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     1381 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/api/community/events/group_updated_event.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     1380 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/api/community/events/member_joined_event.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     1377 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/api/community/events/member_left_event.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     1373 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/api/community/events/user_banned_event.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-07-21 18:02:41.258771 swibots-1.3.8/swibots/api/community/methods/
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      765 2023-07-20 06:32:08.000000 swibots-1.3.8/swibots/api/community/methods/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      450 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/api/community/methods/ban_user.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      637 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/api/community/methods/create_channel.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      815 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/api/community/methods/deduct_xp.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      643 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/api/community/methods/get_channel.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      866 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/api/community/methods/get_community.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      522 2023-07-17 15:05:23.000000 swibots-1.3.8/swibots/api/community/methods/get_community_member.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      619 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/api/community/methods/get_group.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     2946 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/api/community/methods/permission.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     2418 2023-07-20 06:32:08.000000 swibots-1.3.8/swibots/api/community/methods/restrict_user.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     2259 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/api/community/methods/rolemember.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     2222 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/api/community/methods/roles.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      686 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/api/community/methods/unban_user.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      637 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/api/community/methods/update_channel.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-07-21 18:02:41.262771 swibots-1.3.8/swibots/api/community/models/
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      439 2023-07-20 06:32:08.000000 swibots-1.3.8/swibots/api/community/models/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      733 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/api/community/models/baninfo.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     3563 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/api/community/models/channel.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     2954 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/api/community/models/community.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     2998 2023-07-17 15:05:23.000000 swibots-1.3.8/swibots/api/community/models/community_member.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     2720 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/api/community/models/group.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1460 2023-07-20 06:32:08.000000 swibots-1.3.8/swibots/api/community/models/restricteduser.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1218 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/api/community/models/role.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1464 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/api/community/models/rolemember.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     3176 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/api/community/models/rolepermission.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     9347 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/app.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-07-21 18:02:41.270771 swibots-1.3.8/swibots/base/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      262 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/base/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       69 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/base/rest_controller.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      370 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/base/rest_request.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      644 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/base/rest_response.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     4261 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/base/switch_client.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1180 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/base/switch_object.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      543 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/base/switch_ws_async_client.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     4598 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/bot_app.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-07-21 18:02:41.274771 swibots-1.3.8/swibots/bots/
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      201 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/bots/__init__.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     4646 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/bots/bot.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     1646 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/bots/bot_context.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      109 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/bots/constants.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-07-21 18:02:41.286771 swibots-1.3.8/swibots/bots/decorators/
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      999 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/bots/decorators/__init__.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      540 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/bots/decorators/on_callback_query.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      510 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/bots/decorators/on_channel_created.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      544 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/bots/decorators/on_channel_deleted.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      541 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/bots/decorators/on_channel_updated.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      574 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/bots/decorators/on_command.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      544 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/bots/decorators/on_community_updated.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      536 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/bots/decorators/on_group_created.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      536 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/bots/decorators/on_group_deleted.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      534 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/bots/decorators/on_group_updated.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      537 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/bots/decorators/on_inline_query.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      534 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/bots/decorators/on_member_joined.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      529 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/bots/decorators/on_member_left.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      503 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/bots/decorators/on_message.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      543 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/bots/decorators/on_unknown_command.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      509 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/bots/decorators/on_user_banned.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-07-21 18:02:41.286771 swibots-1.3.8/swibots/bots/filters/
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)       22 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/bots/filters/__init__.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     7785 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/bots/filters/filter.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-07-21 18:02:41.302771 swibots-1.3.8/swibots/bots/handlers/
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     1300 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/bots/handlers/__init__.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     1048 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/bots/handlers/base_handler.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      985 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/bots/handlers/callback_query_handler.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      681 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/bots/handlers/channel_created_handler.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      688 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/bots/handlers/channel_deleted_handler.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      734 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/bots/handlers/channel_updated_handler.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     1514 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/bots/handlers/command_handler.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      686 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/bots/handlers/community_updated_handler.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     1325 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/bots/handlers/event_handler.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      680 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/bots/handlers/group_created_handler.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      775 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/bots/handlers/group_deleted_handler.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      775 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/bots/handlers/group_updated_handler.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      867 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/bots/handlers/inline_query_handler.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      679 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/bots/handlers/member_joined_handler.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      674 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/bots/handlers/member_left_handler.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      960 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/bots/handlers/message_handler.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      885 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/bots/handlers/unknown_command_handler.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      670 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/bots/handlers/user_banned_handler.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      285 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/bots/register_command.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     1923 2023-07-21 18:02:28.000000 swibots-1.3.8/swibots/config.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1333 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/error.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)      973 2023-07-20 06:32:08.000000 swibots-1.3.8/swibots/types.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-07-21 18:02:41.302771 swibots-1.3.8/swibots/utils/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       75 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/utils/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     5883 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/utils/rest_client.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     2684 2023-07-17 15:05:23.000000 swibots-1.3.8/swibots/utils/types.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-07-21 18:02:41.302771 swibots-1.3.8/swibots/utils/ws/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       48 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/utils/ws/__init__.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-07-21 18:02:41.306771 swibots-1.3.8/swibots/utils/ws/asyncstomp/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      150 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/utils/ws/asyncstomp/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     9787 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/utils/ws/asyncstomp/async_ws_client.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      980 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/utils/ws/asyncstomp/async_ws_subscription.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-07-21 18:02:41.310771 swibots-1.3.8/swibots/utils/ws/common/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      100 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/utils/ws/common/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1654 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/utils/ws/common/ws_frame.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      430 2023-07-15 16:34:05.000000 swibots-1.3.8/swibots/utils/ws/common/ws_message.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-07-21 18:02:41.178771 swibots-1.3.8/swibots.egg-info/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1817 2023-07-21 18:02:41.000000 swibots-1.3.8/swibots.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     8698 2023-07-21 18:02:41.000000 swibots-1.3.8/swibots.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2023-07-21 18:02:41.000000 swibots-1.3.8/swibots.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2023-07-21 18:02:41.000000 swibots-1.3.8/swibots.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        8 2023-07-21 18:02:41.000000 swibots-1.3.8/swibots.egg-info/top_level.txt
```

### Comparing `swibots-1.3.7/PKG-INFO` & `swibots-1.3.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swibots
-Version: 1.3.7
+Version: 1.3.8
 Summary: Switch bot api
 Home-page: https://github.com/switchcollab/Switch-Bots-Python-Library
 Author: switchadmin
 Author-email: support@switch.pe
 License: LGPLv3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `swibots-1.3.7/README.md` & `swibots-1.3.8/README.md`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/setup.py` & `swibots-1.3.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     long_description = pypandoc.convert_file("README.md", "rst")
 except (IOError, ImportError):
     long_description = open("README.md").read()
 
 
 setup(
     name="swibots",
-    version="1.3.7",
+    version="1.3.8",
     packages=find_packages(),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/switchcollab/Switch-Bots-Python-Library",
     description="Switch bot api",
     author="switchadmin",
     author_email="support@switch.pe",
```

### Comparing `swibots-1.3.7/swibots/api/api_client.py` & `swibots-1.3.8/swibots/api/api_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,35 +1,38 @@
 import swibots
 from .auth import AuthClient
 from .chat import ChatClient
 from .community import CommunityClient
 from .bot import BotClient
 from .auth.models import AuthUser
+from .airdrop import AirdropClient
 
 from .auth.methods import AuthMethods
 from .bot.methods import BotMethods
 from .chat.methods import ChatMethods
 from .community.methods import CommunityMethods
-
+from .airdrop.methods import AirdropMethods
 
 class ApiClient(
     AuthMethods,
     BotMethods,
     ChatMethods,
     CommunityMethods,
+    AirdropMethods
 ):
     def __init__(self, **kwargs):
         """Initialize the client"""
         self._token: str = None
         self.__dict__.update(kwargs)
         self._chat_client: ChatClient = None
         self._auth_client: AuthClient = None
         self._community_client: CommunityClient = None
         self._bot_client: BotClient = None
         self._user: AuthUser = None
+        self._airdrop_client: AirdropClient = None
         self.initialize()
 
     def initialize(self):
         """Initialize the client"""
         self.chat_service.initialize()
         self.auth_service.initialize()
         self.community_service.initialize()
@@ -70,12 +73,19 @@
     def community_service(self) -> CommunityClient:
         """Get the community client"""
         if self._community_client is None:
             self._community_client = CommunityClient(self)
         return self._community_client
 
     @property
+    def airdrop_service(self) -> AirdropClient:
+        """Get the airdrop client"""
+        if self._airdrop_client is None:
+            self._airdrop_client = AirdropClient(self)
+        return self._airdrop_client
+
+    @property
     def bots_service(self) -> BotClient:
         """Get the bot client"""
         if self._bot_client is None:
             self._bot_client = BotClient(self)
         return self._bot_client
```

### Comparing `swibots-1.3.7/swibots/api/auth/auth_client.py` & `swibots-1.3.8/swibots/api/auth/auth_client.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/api/auth/controllers/user_controller.py` & `swibots-1.3.8/swibots/api/auth/controllers/user_controller.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/api/auth/methods/get_me.py` & `swibots-1.3.8/swibots/api/auth/methods/get_me.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/api/auth/methods/login.py` & `swibots-1.3.8/swibots/api/auth/methods/login.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/api/auth/models/auth_user.py` & `swibots-1.3.8/swibots/api/auth/models/auth_user.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/api/bot/bot_client.py` & `swibots-1.3.8/swibots/api/bot/bot_client.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/api/bot/controllers/bot_controller.py` & `swibots-1.3.8/swibots/api/bot/controllers/bot_controller.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/api/bot/methods/delete_bot_info.py` & `swibots-1.3.8/swibots/api/bot/methods/delete_bot_info.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/api/bot/methods/get_bot_info.py` & `swibots-1.3.8/swibots/api/bot/methods/get_bot_info.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/api/bot/methods/update_bot_info.py` & `swibots-1.3.8/swibots/api/bot/methods/update_bot_info.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/api/bot/models/bot_command_info.py` & `swibots-1.3.8/swibots/api/bot/models/bot_command_info.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/api/bot/models/bot_info.py` & `swibots-1.3.8/swibots/api/bot/models/bot_info.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/api/chat/chat_client.py` & `swibots-1.3.8/swibots/api/chat/chat_client.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/api/chat/controllers/message_controller.py` & `swibots-1.3.8/swibots/api/chat/controllers/message_controller.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/api/chat/events/callback_query_event.py` & `swibots-1.3.8/swibots/api/chat/events/callback_query_event.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/api/chat/events/chat_event.py` & `swibots-1.3.8/swibots/api/chat/events/chat_event.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/api/chat/events/command_event.py` & `swibots-1.3.8/swibots/api/chat/events/command_event.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/api/chat/events/inline_query_event.py` & `swibots-1.3.8/swibots/api/chat/events/inline_query_event.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/api/chat/events/message_event.py` & `swibots-1.3.8/swibots/api/chat/events/message_event.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/api/chat/methods/__init__.py` & `swibots-1.3.8/swibots/api/chat/methods/__init__.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/api/chat/methods/answer_inline_query.py` & `swibots-1.3.8/swibots/api/chat/methods/answer_inline_query.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/api/chat/methods/clear_conversation.py` & `swibots-1.3.8/swibots/api/chat/methods/clear_conversation.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/api/chat/methods/delete_message.py` & `swibots-1.3.8/swibots/api/chat/methods/delete_message.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/api/chat/methods/delete_messages_from_user.py` & `swibots-1.3.8/swibots/api/chat/methods/delete_messages_from_user.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/api/chat/methods/download_media.py` & `swibots-1.3.8/swibots/api/chat/methods/download_media.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/api/chat/methods/edit_message.py` & `swibots-1.3.8/swibots/api/chat/methods/edit_message.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/api/chat/methods/edit_message_text.py` & `swibots-1.3.8/swibots/api/chat/methods/edit_message_text.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/api/chat/methods/flag_message.py` & `swibots-1.3.8/swibots/api/chat/methods/flag_message.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/api/chat/methods/forward_message.py` & `swibots-1.3.8/swibots/api/chat/methods/forward_message.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/api/chat/methods/get_channel_chat_history.py` & `swibots-1.3.8/swibots/api/chat/methods/get_channel_chat_history.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/api/chat/methods/get_community_media_files.py` & `swibots-1.3.8/swibots/api/chat/methods/get_community_media_files.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/api/chat/methods/get_community_media_files_by_status.py` & `swibots-1.3.8/swibots/api/chat/methods/get_community_media_files_by_status.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/api/chat/methods/get_flag_messages.py` & `swibots-1.3.8/swibots/api/chat/methods/get_flag_messages.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/api/chat/methods/get_group_chat_history.py` & `swibots-1.3.8/swibots/api/chat/methods/get_group_chat_history.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/api/chat/methods/get_message.py` & `swibots-1.3.8/swibots/api/chat/methods/get_message.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/api/chat/methods/get_messages.py` & `swibots-1.3.8/swibots/api/chat/methods/get_messages.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/api/chat/methods/get_messages_between_users.py` & `swibots-1.3.8/swibots/api/chat/methods/get_messages_between_users.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/api/chat/methods/get_unread_messages_count.py` & `swibots-1.3.8/swibots/api/chat/methods/get_unread_messages_count.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/api/chat/methods/get_user_media_files.py` & `swibots-1.3.8/swibots/api/chat/methods/get_user_media_files.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/api/chat/methods/reply_message.py` & `swibots-1.3.8/swibots/api/chat/methods/reply_message.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/api/chat/methods/reply_message_text.py` & `swibots-1.3.8/swibots/api/chat/methods/reply_message_text.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/api/chat/methods/send_message.py` & `swibots-1.3.8/swibots/api/chat/methods/send_message.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/api/chat/methods/send_text.py` & `swibots-1.3.8/swibots/api/chat/methods/send_text.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/api/chat/models/group_chat_history.py` & `swibots-1.3.8/swibots/api/chat/models/group_chat_history.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/api/chat/models/inline/__init__.py` & `swibots-1.3.8/swibots/api/chat/models/inline/__init__.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/api/chat/models/inline/base_typed_inline_query_result.py` & `swibots-1.3.8/swibots/api/chat/models/inline/base_typed_inline_query_result.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/api/chat/models/inline/inline_query.py` & `swibots-1.3.8/swibots/api/chat/models/inline/inline_query.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/api/chat/models/inline/inline_query_answer.py` & `swibots-1.3.8/swibots/api/chat/models/inline/inline_query_answer.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/api/chat/models/inline/inline_query_result.py` & `swibots-1.3.8/swibots/api/chat/models/inline/inline_query_result.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/api/chat/models/inline/inline_query_result_article.py` & `swibots-1.3.8/swibots/api/chat/models/inline/inline_query_result_article.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/api/chat/models/inline/inline_query_result_document.py` & `swibots-1.3.8/swibots/api/chat/models/inline/inline_query_result_document.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/api/chat/models/inline/inline_query_result_photo.py` & `swibots-1.3.8/swibots/api/chat/models/inline/inline_query_result_photo.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/api/chat/models/inline/inline_query_result_video.py` & `swibots-1.3.8/swibots/api/chat/models/inline/inline_query_result_video.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/api/chat/models/inline/input_message_content.py` & `swibots-1.3.8/swibots/api/chat/models/inline/input_message_content.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/api/chat/models/inline_keyboard_button.py` & `swibots-1.3.8/swibots/api/chat/models/inline_keyboard_button.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/api/chat/models/inline_markup.py` & `swibots-1.3.8/swibots/api/chat/models/inline_markup.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/api/chat/models/message.py` & `swibots-1.3.8/swibots/api/chat/models/message.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/api/common/events/event.py` & `swibots-1.3.8/swibots/api/common/events/event.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/api/common/models/embed_inline_field.py` & `swibots-1.3.8/swibots/api/common/models/embed_inline_field.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/api/common/models/embedded_media.py` & `swibots-1.3.8/swibots/api/common/models/embedded_media.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,14 @@
             for j, b in enumerate(kb):
                 key = "embedMessage.inlineFields[{0}][{1}].key".format(i, j)
                 form_data[key] = b.key
                 title_key = "embedMessage.inlineFields[{0}][{1}].title".format(i, j)
                 form_data[title_key] = b.title
                 icon_key = "embedMessage.inlineFields[{0}][{1}].icon".format(i, j)
                 form_data[icon_key] = b.icon
-        print(form_data)
         return form_data
 
     def from_json(self, data: JSONDict | None) -> "EmbeddedMedia":
         if data is not None:
             self.thumbnail = data.get("coverPic")
             self.description = data.get("description")
             self.footer_icon = data.get("footerIcon")
```

### Comparing `swibots-1.3.7/swibots/api/common/models/media.py` & `swibots-1.3.8/swibots/api/common/models/media.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/api/common/models/media_upload_request.py` & `swibots-1.3.8/swibots/api/common/models/media_upload_request.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/api/common/models/user.py` & `swibots-1.3.8/swibots/api/common/models/user.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Optional
+from typing import Optional, List, Any
 from swibots.utils.types import JSONDict
 from swibots.base.switch_object import SwitchObject
 
 
 class User(SwitchObject):
     def __init__(
         self,
@@ -11,36 +11,39 @@
         username: Optional[str] = None,
         image_url: Optional[str] = None,
         active: Optional[bool] = None,
         deleted: Optional[bool] = None,
         role_info: Optional[str] = None,
         admin: Optional[bool] = None,
         is_bot: Optional[bool] = None,
+        tournaments: Optional[List[Any]] = None
     ):
         self.id = id
         self.name = name
         self.username = username
         self.image_url = image_url
         self.active = active
         self.deleted = deleted
         self.role_info = role_info
         self.admin = admin
         self.is_bot = is_bot
+        self.tournaments = tournaments
 
     def to_json(self) -> JSONDict:
         return {
             "id": self.id,
             "name": self.name,
             "username": self.username,
             "imageUrl": self.image_url,
             "active": self.active,
             "deleted": self.deleted,
             "roleInfo": self.role_info,
             "admin": self.admin,
             "is_bot": self.is_bot,
+            "tournamentsParticipated": self.tournaments
         }
 
     def from_json(self, data: Optional[JSONDict] = None) -> "User":
         if data is not None:
             self.id = data.get("id")
             self.name = data.get("name")
             self.username = data.get("username")
```

### Comparing `swibots-1.3.7/swibots/api/community/community_client.py` & `swibots-1.3.8/swibots/api/community/community_client.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/api/community/controllers/ban_controller.py` & `swibots-1.3.8/swibots/api/community/controllers/ban_controller.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/api/community/controllers/channel_controller.py` & `swibots-1.3.8/swibots/api/community/controllers/channel_controller.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/api/community/controllers/community_controller.py` & `swibots-1.3.8/swibots/api/community/controllers/community_controller.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/api/community/controllers/group_controller.py` & `swibots-1.3.8/swibots/api/community/controllers/group_controller.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/api/community/controllers/permissions_controller.py` & `swibots-1.3.8/swibots/api/community/controllers/permissions_controller.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/api/community/controllers/restrict_controller.py` & `swibots-1.3.8/swibots/api/community/controllers/restrict_controller.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/api/community/controllers/rolemember_controller.py` & `swibots-1.3.8/swibots/api/community/controllers/rolemember_controller.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/api/community/controllers/roles_controller.py` & `swibots-1.3.8/swibots/api/community/controllers/roles_controller.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/api/community/events/__init__.py` & `swibots-1.3.8/swibots/api/community/events/__init__.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/api/community/events/channel_created_event.py` & `swibots-1.3.8/swibots/api/community/events/channel_created_event.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/api/community/events/channel_deleted_event.py` & `swibots-1.3.8/swibots/api/community/events/channel_deleted_event.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/api/community/events/channel_updated_event.py` & `swibots-1.3.8/swibots/api/community/events/channel_updated_event.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/api/community/events/community_event.py` & `swibots-1.3.8/swibots/api/community/events/community_event.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/api/community/events/community_updated_event.py` & `swibots-1.3.8/swibots/api/community/events/community_updated_event.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/api/community/events/group_created_event.py` & `swibots-1.3.8/swibots/api/community/events/group_created_event.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/api/community/events/group_deleted_event.py` & `swibots-1.3.8/swibots/api/community/events/group_deleted_event.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/api/community/events/group_updated_event.py` & `swibots-1.3.8/swibots/api/community/events/group_updated_event.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/api/community/events/member_joined_event.py` & `swibots-1.3.8/swibots/api/community/events/member_joined_event.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/api/community/events/member_left_event.py` & `swibots-1.3.8/swibots/api/community/events/member_left_event.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/api/community/events/user_banned_event.py` & `swibots-1.3.8/swibots/api/community/events/user_banned_event.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/api/community/methods/__init__.py` & `swibots-1.3.8/swibots/api/community/methods/__init__.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/api/community/methods/create_channel.py` & `swibots-1.3.8/swibots/api/community/methods/create_channel.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/api/community/methods/deduct_xp.py` & `swibots-1.3.8/swibots/api/community/methods/deduct_xp.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/api/community/methods/get_channel.py` & `swibots-1.3.8/swibots/api/community/methods/get_channel.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/api/community/methods/get_community.py` & `swibots-1.3.8/swibots/api/community/methods/get_community.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/api/community/methods/get_community_member.py` & `swibots-1.3.8/swibots/api/community/methods/get_community_member.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/api/community/methods/get_group.py` & `swibots-1.3.8/swibots/api/community/methods/get_group.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/api/community/methods/permission.py` & `swibots-1.3.8/swibots/api/community/methods/permission.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/api/community/methods/restrict_user.py` & `swibots-1.3.8/swibots/api/community/methods/restrict_user.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/api/community/methods/rolemember.py` & `swibots-1.3.8/swibots/api/community/methods/rolemember.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/api/community/methods/roles.py` & `swibots-1.3.8/swibots/api/community/methods/roles.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/api/community/methods/unban_user.py` & `swibots-1.3.8/swibots/api/community/methods/unban_user.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/api/community/methods/update_channel.py` & `swibots-1.3.8/swibots/api/community/methods/update_channel.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/api/community/models/baninfo.py` & `swibots-1.3.8/swibots/api/community/models/baninfo.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/api/community/models/channel.py` & `swibots-1.3.8/swibots/api/community/models/channel.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/api/community/models/community.py` & `swibots-1.3.8/swibots/api/community/models/community.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/api/community/models/community_member.py` & `swibots-1.3.8/swibots/api/community/models/community_member.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/api/community/models/group.py` & `swibots-1.3.8/swibots/api/community/models/group.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/api/community/models/restricteduser.py` & `swibots-1.3.8/swibots/api/community/models/restricteduser.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/api/community/models/role.py` & `swibots-1.3.8/swibots/api/community/models/role.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/api/community/models/rolemember.py` & `swibots-1.3.8/swibots/api/community/models/rolemember.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/api/community/models/rolepermission.py` & `swibots-1.3.8/swibots/api/community/models/rolepermission.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/app.py` & `swibots-1.3.8/swibots/app.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/base/rest_response.py` & `swibots-1.3.8/swibots/base/rest_response.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/base/switch_client.py` & `swibots-1.3.8/swibots/base/switch_client.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/base/switch_object.py` & `swibots-1.3.8/swibots/base/switch_object.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/base/switch_ws_async_client.py` & `swibots-1.3.8/swibots/base/switch_ws_async_client.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/bot_app.py` & `swibots-1.3.8/swibots/bot_app.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/bots/bot.py` & `swibots-1.3.8/swibots/bots/bot.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/bots/bot_context.py` & `swibots-1.3.8/swibots/bots/bot_context.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/bots/decorators/__init__.py` & `swibots-1.3.8/swibots/bots/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/bots/decorators/on_callback_query.py` & `swibots-1.3.8/swibots/bots/decorators/on_callback_query.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/bots/decorators/on_channel_deleted.py` & `swibots-1.3.8/swibots/bots/decorators/on_channel_deleted.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/bots/decorators/on_channel_updated.py` & `swibots-1.3.8/swibots/bots/decorators/on_channel_updated.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/bots/decorators/on_command.py` & `swibots-1.3.8/swibots/bots/decorators/on_command.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/bots/decorators/on_community_updated.py` & `swibots-1.3.8/swibots/bots/decorators/on_community_updated.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/bots/decorators/on_group_created.py` & `swibots-1.3.8/swibots/bots/decorators/on_group_created.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/bots/decorators/on_group_deleted.py` & `swibots-1.3.8/swibots/bots/decorators/on_group_deleted.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/bots/decorators/on_group_updated.py` & `swibots-1.3.8/swibots/bots/decorators/on_group_updated.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/bots/decorators/on_inline_query.py` & `swibots-1.3.8/swibots/bots/decorators/on_inline_query.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/bots/decorators/on_member_joined.py` & `swibots-1.3.8/swibots/bots/decorators/on_member_joined.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/bots/decorators/on_member_left.py` & `swibots-1.3.8/swibots/bots/decorators/on_member_left.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/bots/decorators/on_unknown_command.py` & `swibots-1.3.8/swibots/bots/decorators/on_unknown_command.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/bots/filters/filter.py` & `swibots-1.3.8/swibots/bots/filters/filter.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/bots/handlers/__init__.py` & `swibots-1.3.8/swibots/bots/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/bots/handlers/base_handler.py` & `swibots-1.3.8/swibots/bots/handlers/base_handler.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/bots/handlers/callback_query_handler.py` & `swibots-1.3.8/swibots/bots/handlers/callback_query_handler.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/bots/handlers/channel_created_handler.py` & `swibots-1.3.8/swibots/bots/handlers/channel_created_handler.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/bots/handlers/channel_deleted_handler.py` & `swibots-1.3.8/swibots/bots/handlers/channel_deleted_handler.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/bots/handlers/channel_updated_handler.py` & `swibots-1.3.8/swibots/bots/handlers/channel_updated_handler.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/bots/handlers/command_handler.py` & `swibots-1.3.8/swibots/bots/handlers/command_handler.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/bots/handlers/community_updated_handler.py` & `swibots-1.3.8/swibots/bots/handlers/community_updated_handler.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/bots/handlers/event_handler.py` & `swibots-1.3.8/swibots/bots/handlers/event_handler.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/bots/handlers/group_created_handler.py` & `swibots-1.3.8/swibots/bots/handlers/group_created_handler.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/bots/handlers/group_deleted_handler.py` & `swibots-1.3.8/swibots/bots/handlers/group_deleted_handler.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/bots/handlers/group_updated_handler.py` & `swibots-1.3.8/swibots/bots/handlers/group_updated_handler.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/bots/handlers/inline_query_handler.py` & `swibots-1.3.8/swibots/bots/handlers/inline_query_handler.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/bots/handlers/member_joined_handler.py` & `swibots-1.3.8/swibots/bots/handlers/member_joined_handler.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/bots/handlers/member_left_handler.py` & `swibots-1.3.8/swibots/bots/handlers/member_left_handler.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/bots/handlers/message_handler.py` & `swibots-1.3.8/swibots/bots/handlers/message_handler.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/bots/handlers/unknown_command_handler.py` & `swibots-1.3.8/swibots/bots/handlers/unknown_command_handler.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/bots/handlers/user_banned_handler.py` & `swibots-1.3.8/swibots/bots/handlers/user_banned_handler.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/config.py` & `swibots-1.3.8/swibots/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,14 +8,17 @@
     },
     "BOT_SERVICE": {
         "BASE_URL": os.getenv("BOT_SERVICE_BASE_URL") or "https://chat.switch.pe",
     },
     "AUTH_SERVICE": {
         "BASE_URL": os.getenv("AUTH_SERVICE_BASE_URL") or "https://api-gateway.switch.pe/user-service",
     },
+    "AIRDROP_SERVICE": {
+        "BASE_URL": os.getenv("AIRDROP_SERVICE_BASE_URL") or "https://api-gateway.switch.pe/airdrop-service"
+    },
     "COMMUNITY_SERVICE": {
         "BASE_URL": os.getenv("COMMUNITY_SERVICE_BASE_URL") or "https://api-gateway.switch.pe/community-service",
         "WS_URL": os.getenv("COMMUNITY_SERVICE_WS_URL") or "wss://api-gateway.switch.pe/v1/websocket/community/ws",
     },
 }
 
 
@@ -32,10 +35,11 @@
         "BOT_SERVICE_BASE_URL") or "https://chat.switch.pe"
     APP_CONFIG["AUTH_SERVICE"]['BASE_URL'] = os.getenv(
         "AUTH_SERVICE_BASE_URL") or "https://api-gateway.switch.pe/user-service"
     APP_CONFIG["COMMUNITY_SERVICE"]['BASE_URL'] = os.getenv(
         "COMMUNITY_SERVICE_BASE_URL") or "https://api-gateway.switch.pe/community-service"
     APP_CONFIG["COMMUNITY_SERVICE"]['WS_URL'] = os.getenv(
         "COMMUNITY_SERVICE_WS_URL") or "wss://api-gateway.switch.pe/v1/websocket/community/ws"
+    APP_CONFIG['AIRDROP_SERVICE']['BASE_URL'] = os.getenv("AIRDROP_SERVICE_BASE_URL") or "https://api-gateway.switch.pe/airdrop-service"
 
 
 reload_config()
```

### Comparing `swibots-1.3.7/swibots/error.py` & `swibots-1.3.8/swibots/error.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/types.py` & `swibots-1.3.8/swibots/types.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/utils/rest_client.py` & `swibots-1.3.8/swibots/utils/rest_client.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/utils/types.py` & `swibots-1.3.8/swibots/utils/types.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/utils/ws/asyncstomp/async_ws_client.py` & `swibots-1.3.8/swibots/utils/ws/asyncstomp/async_ws_client.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/utils/ws/asyncstomp/async_ws_subscription.py` & `swibots-1.3.8/swibots/utils/ws/asyncstomp/async_ws_subscription.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots/utils/ws/common/ws_frame.py` & `swibots-1.3.8/swibots/utils/ws/common/ws_frame.py`

 * *Files identical despite different names*

### Comparing `swibots-1.3.7/swibots.egg-info/PKG-INFO` & `swibots-1.3.8/swibots.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swibots
-Version: 1.3.7
+Version: 1.3.8
 Summary: Switch bot api
 Home-page: https://github.com/switchcollab/Switch-Bots-Python-Library
 Author: switchadmin
 Author-email: support@switch.pe
 License: LGPLv3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `swibots-1.3.7/swibots.egg-info/SOURCES.txt` & `swibots-1.3.8/swibots.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,22 @@
 swibots.egg-info/PKG-INFO
 swibots.egg-info/SOURCES.txt
 swibots.egg-info/dependency_links.txt
 swibots.egg-info/requires.txt
 swibots.egg-info/top_level.txt
 swibots/api/__init__.py
 swibots/api/api_client.py
+swibots/api/airdrop/__init__.py
+swibots/api/airdrop/client.py
+swibots/api/airdrop/controllers/__init__.py
+swibots/api/airdrop/controllers/tournament_controller.py
+swibots/api/airdrop/methods/__init__.py
+swibots/api/airdrop/methods/get_referral.py
+swibots/api/airdrop/models/__init__.py
+swibots/api/airdrop/models/referral.py
 swibots/api/auth/__init__.py
 swibots/api/auth/auth_client.py
 swibots/api/auth/controllers/__init__.py
 swibots/api/auth/controllers/user_controller.py
 swibots/api/auth/methods/__init__.py
 swibots/api/auth/methods/get_me.py
 swibots/api/auth/methods/login.py
```

