# Comparing `tmp/PyroFork-dev-2.2.5.dev202307219421.tar.gz` & `tmp/PyroFork-dev-2.2.5.dev202307219555.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyroFork-dev-2.2.5.dev202307219421.tar", last modified: Fri Jul 21 16:56:15 2023, max compression
+gzip compressed data, was "PyroFork-dev-2.2.5.dev202307219555.tar", last modified: Fri Jul 21 15:16:39 2023, max compression
```

## Comparing `PyroFork-dev-2.2.5.dev202307219421.tar` & `PyroFork-dev-2.2.5.dev202307219555.tar`

### file list

```diff
@@ -1,532 +1,529 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:56:15.527639 PyroFork-dev-2.2.5.dev202307219421/
--rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/COPYING.lesser
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     3917 2023-07-21 16:56:15.527639 PyroFork-dev-2.2.5.dev202307219421/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:56:15.407638 PyroFork-dev-2.2.5.dev202307219421/PyroFork_dev.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3917 2023-07-21 16:56:15.000000 PyroFork-dev-2.2.5.dev202307219421/PyroFork_dev.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20484 2023-07-21 16:56:15.000000 PyroFork-dev-2.2.5.dev202307219421/PyroFork_dev.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 16:56:15.000000 PyroFork-dev-2.2.5.dev202307219421/PyroFork_dev.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 16:56:15.000000 PyroFork-dev-2.2.5.dev202307219421/PyroFork_dev.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-21 16:56:15.000000 PyroFork-dev-2.2.5.dev202307219421/PyroFork_dev.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-21 16:56:15.000000 PyroFork-dev-2.2.5.dev202307219421/PyroFork_dev.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:56:15.407638 PyroFork-dev-2.2.5.dev202307219421/compiler/
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/compiler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:56:15.407638 PyroFork-dev-2.2.5.dev202307219421/compiler/api/
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/compiler/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22402 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/compiler/api/compiler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:56:15.407638 PyroFork-dev-2.2.5.dev202307219421/compiler/api/source/
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/compiler/api/source/auth_key.tl
--rw-r--r--   0 runner    (1001) docker     (123)   175007 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/compiler/api/source/main_api.tl
--rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/compiler/api/source/sys_msgs.tl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:56:15.411639 PyroFork-dev-2.2.5.dev202307219421/compiler/api/template/
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/compiler/api/template/combinator.txt
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/compiler/api/template/type.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:56:15.411639 PyroFork-dev-2.2.5.dev202307219421/compiler/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/compiler/docs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19579 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/compiler/docs/compiler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:56:15.411639 PyroFork-dev-2.2.5.dev202307219421/compiler/docs/template/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/compiler/docs/template/page.txt
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/compiler/docs/template/toctree.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:56:15.411639 PyroFork-dev-2.2.5.dev202307219421/compiler/errors/
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/compiler/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4917 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/compiler/errors/compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/compiler/errors/sort.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:56:15.415639 PyroFork-dev-2.2.5.dev202307219421/compiler/errors/source/
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/compiler/errors/source/303_SEE_OTHER.tsv
--rw-r--r--   0 runner    (1001) docker     (123)    22907 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/compiler/errors/source/400_BAD_REQUEST.tsv
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/compiler/errors/source/401_UNAUTHORIZED.tsv
--rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/compiler/errors/source/403_FORBIDDEN.tsv
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/compiler/errors/source/406_NOT_ACCEPTABLE.tsv
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/compiler/errors/source/420_FLOOD.tsv
--rw-r--r--   0 runner    (1001) docker     (123)     4298 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/compiler/errors/source/500_INTERNAL_SERVER_ERROR.tsv
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/compiler/errors/source/503_SERVICE_UNAVAILABLE.tsv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:56:15.415639 PyroFork-dev-2.2.5.dev202307219421/compiler/errors/template/
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/compiler/errors/template/class.txt
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/compiler/errors/template/sub_class.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:56:15.419639 PyroFork-dev-2.2.5.dev202307219421/pyrogram/
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-07-21 16:56:08.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    41006 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:56:15.419639 PyroFork-dev-2.2.5.dev202307219421/pyrogram/connection/
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/connection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/connection/connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:56:15.419639 PyroFork-dev-2.2.5.dev202307219421/pyrogram/connection/transport/
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/connection/transport/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:56:15.419639 PyroFork-dev-2.2.5.dev202307219421/pyrogram/connection/transport/tcp/
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/connection/transport/tcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4100 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/connection/transport/tcp/tcp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/connection/transport/tcp/tcp_abridged.py
--rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/connection/transport/tcp/tcp_abridged_o.py
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/connection/transport/tcp/tcp_full.py
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/connection/transport/tcp/tcp_intermediate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/connection/transport/tcp/tcp_intermediate_o.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:56:15.423639 PyroFork-dev-2.2.5.dev202307219421/pyrogram/crypto/
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/crypto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4013 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/crypto/aes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4762 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/crypto/mtproto.py
--rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/crypto/prime.py
--rw-r--r--   0 runner    (1001) docker     (123)    13437 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/crypto/rsa.py
--rw-r--r--   0 runner    (1001) docker     (123)    10085 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)   208021 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/emoji.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:56:15.427639 PyroFork-dev-2.2.5.dev202307219421/pyrogram/enums/
--rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/enums/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/enums/auto_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/enums/chat_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     4520 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/enums/chat_event_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/enums/chat_member_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/enums/chat_members_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/enums/chat_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/enums/message_entity_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/enums/message_media_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/enums/message_service_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/enums/messages_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/enums/next_code_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/enums/parse_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/enums/poll_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/enums/sent_code_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/enums/user_status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:56:15.427639 PyroFork-dev-2.2.5.dev202307219421/pyrogram/errors/
--rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/errors/rpc_error.py
--rw-r--r--   0 runner    (1001) docker     (123)    15154 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/file_id.py
--rw-r--r--   0 runner    (1001) docker     (123)    24836 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:56:15.431639 PyroFork-dev-2.2.5.dev202307219421/pyrogram/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/handlers/callback_query_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/handlers/chat_join_request_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/handlers/chat_member_updated_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/handlers/chosen_inline_result_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/handlers/deleted_messages_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/handlers/disconnect_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/handlers/edited_message_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/handlers/handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/handlers/inline_query_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/handlers/message_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/handlers/poll_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/handlers/raw_update_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/handlers/user_status_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:56:15.431639 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:56:15.435639 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/advanced/
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/advanced/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/advanced/invoke.py
--rw-r--r--   0 runner    (1001) docker     (123)     4560 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/advanced/resolve_peer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8164 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/advanced/save_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:56:15.439639 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/auth/
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/auth/accept_terms_of_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/auth/check_password.py
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/auth/connect.py
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/auth/disconnect.py
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/auth/get_password_hint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/auth/initialize.py
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/auth/log_out.py
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/auth/recover_password.py
--rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/auth/resend_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/auth/send_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/auth/send_recovery_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/auth/sign_in.py
--rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/auth/sign_in_bot.py
--rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/auth/sign_up.py
--rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/auth/terminate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:56:15.443639 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/bots/
--rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/bots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/bots/answer_callback_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     4990 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/bots/answer_inline_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/bots/answer_web_app_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/bots/delete_bot_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/bots/get_bot_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/bots/get_bot_default_privileges.py
--rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/bots/get_chat_menu_button.py
--rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/bots/get_game_high_scores.py
--rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/bots/get_inline_bot_results.py
--rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/bots/request_callback_answer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/bots/send_game.py
--rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/bots/send_inline_bot_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/bots/set_bot_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/bots/set_bot_default_privileges.py
--rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/bots/set_chat_menu_button.py
--rw-r--r--   0 runner    (1001) docker     (123)     3946 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/bots/set_game_score.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:56:15.459639 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/chats/
--rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/chats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/chats/add_chat_members.py
--rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/chats/archive_chats.py
--rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/chats/ban_chat_member.py
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/chats/close_forum_topic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/chats/close_general_topic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/chats/create_channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/chats/create_forum_topic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/chats/create_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/chats/create_supergroup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/chats/delete_channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/chats/delete_chat_photo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/chats/delete_forum_topic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/chats/delete_supergroup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/chats/delete_user_history.py
--rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/chats/edit_forum_topic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/chats/edit_general_topic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/chats/get_chat.py
--rw-r--r--   0 runner    (1001) docker     (123)     4032 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/chats/get_chat_event_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/chats/get_chat_member.py
--rw-r--r--   0 runner    (1001) docker     (123)     5282 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/chats/get_chat_members.py
--rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/chats/get_chat_members_count.py
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/chats/get_chat_online_count.py
--rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/chats/get_dialogs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/chats/get_dialogs_count.py
--rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/chats/get_forum_topics.py
--rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/chats/get_forum_topics_by_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/chats/get_nearby_chats.py
--rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/chats/get_send_as_chats.py
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/chats/hide_general_topic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/chats/join_chat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2605 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/chats/leave_chat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/chats/mark_chat_unread.py
--rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/chats/pin_chat_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/chats/promote_chat_member.py
--rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/chats/reopen_forum_topic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/chats/reopen_general_topic.py
--rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/chats/restrict_chat_member.py
--rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/chats/set_administrator_title.py
--rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/chats/set_chat_description.py
--rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/chats/set_chat_permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/chats/set_chat_photo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/chats/set_chat_protected_content.py
--rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/chats/set_chat_title.py
--rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/chats/set_chat_username.py
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/chats/set_send_as_chat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/chats/set_slow_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/chats/unarchive_chats.py
--rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/chats/unban_chat_member.py
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/chats/unhide_general_topic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/chats/unpin_all_chat_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/chats/unpin_chat_message.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:56:15.459639 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/contacts/
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/contacts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/contacts/add_contact.py
--rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/contacts/delete_contacts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/contacts/get_contacts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/contacts/get_contacts_count.py
--rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/contacts/import_contacts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:56:15.459639 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/decorators/
--rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/decorators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/decorators/on_callback_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/decorators/on_chat_join_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/decorators/on_chat_member_updated.py
--rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/decorators/on_chosen_inline_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/decorators/on_deleted_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/decorators/on_disconnect.py
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/decorators/on_edited_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/decorators/on_inline_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/decorators/on_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/decorators/on_poll.py
--rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/decorators/on_raw_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/decorators/on_user_status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:56:15.467639 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/invite_links/
--rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/invite_links/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/invite_links/approve_all_chat_join_requests.py
--rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/invite_links/approve_chat_join_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/invite_links/create_chat_invite_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/invite_links/decline_all_chat_join_requests.py
--rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/invite_links/decline_chat_join_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/invite_links/delete_chat_admin_invite_links.py
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/invite_links/delete_chat_invite_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     3533 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/invite_links/edit_chat_invite_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/invite_links/export_chat_invite_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/invite_links/get_chat_admin_invite_links.py
--rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/invite_links/get_chat_admin_invite_links_count.py
--rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/invite_links/get_chat_admins_with_invite_links.py
--rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/invite_links/get_chat_invite_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/invite_links/get_chat_invite_link_joiners.py
--rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/invite_links/get_chat_invite_link_joiners_count.py
--rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/invite_links/get_chat_join_requests.py
--rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/invite_links/revoke_chat_invite_link.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:56:15.479639 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/messages/
--rw-r--r--   0 runner    (1001) docker     (123)     3921 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/messages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5963 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/messages/copy_media_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     5423 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/messages/copy_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/messages/delete_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     7530 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/messages/download_media.py
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/messages/edit_inline_caption.py
--rw-r--r--   0 runner    (1001) docker     (123)    10375 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/messages/edit_inline_media.py
--rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/messages/edit_inline_reply_markup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/messages/edit_inline_text.py
--rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/messages/edit_message_caption.py
--rw-r--r--   0 runner    (1001) docker     (123)    13022 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/messages/edit_message_media.py
--rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/messages/edit_message_reply_markup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/messages/edit_message_text.py
--rw-r--r--   0 runner    (1001) docker     (123)     5018 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/messages/forward_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/messages/get_chat_history.py
--rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/messages/get_chat_history_count.py
--rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/messages/get_custom_emoji_stickers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/messages/get_discussion_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/messages/get_discussion_replies.py
--rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/messages/get_discussion_replies_count.py
--rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/messages/get_media_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     4741 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/messages/get_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/messages/inline_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/messages/read_chat_history.py
--rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/messages/retract_vote.py
--rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/messages/search_global.py
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/messages/search_global_count.py
--rw-r--r--   0 runner    (1001) docker     (123)     5349 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/messages/search_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/messages/search_messages_count.py
--rw-r--r--   0 runner    (1001) docker     (123)    12828 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/messages/send_animation.py
--rw-r--r--   0 runner    (1001) docker     (123)    11362 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/messages/send_audio.py
--rw-r--r--   0 runner    (1001) docker     (123)     5723 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/messages/send_cached_media.py
--rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/messages/send_chat_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     5111 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/messages/send_contact.py
--rw-r--r--   0 runner    (1001) docker     (123)     5085 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/messages/send_dice.py
--rw-r--r--   0 runner    (1001) docker     (123)    10712 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/messages/send_document.py
--rw-r--r--   0 runner    (1001) docker     (123)     4820 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/messages/send_location.py
--rw-r--r--   0 runner    (1001) docker     (123)    20821 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/messages/send_media_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     7509 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/messages/send_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     9682 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/messages/send_photo.py
--rw-r--r--   0 runner    (1001) docker     (123)     8315 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/messages/send_poll.py
--rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/messages/send_reaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     8582 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/messages/send_sticker.py
--rw-r--r--   0 runner    (1001) docker     (123)     5641 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/messages/send_venue.py
--rw-r--r--   0 runner    (1001) docker     (123)    12198 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/messages/send_video.py
--rw-r--r--   0 runner    (1001) docker     (123)     9556 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/messages/send_video_note.py
--rw-r--r--   0 runner    (1001) docker     (123)     9672 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/messages/send_voice.py
--rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/messages/stop_poll.py
--rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/messages/stream_media.py
--rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/messages/vote_poll.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:56:15.479639 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/password/
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/password/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/password/change_cloud_password.py
--rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/password/enable_cloud_password.py
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/password/remove_cloud_password.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:56:15.479639 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/stickers/
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/stickers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/stickers/add_sticker_to_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/stickers/create_sticker_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/stickers/get_sticker_set.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:56:15.483639 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/users/
--rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/users/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/users/block_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/users/delete_profile_photos.py
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/users/get_bot_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4421 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/users/get_chat_photos.py
--rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/users/get_chat_photos_count.py
--rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/users/get_common_chats.py
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/users/get_default_emoji_statuses.py
--rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/users/get_me.py
--rw-r--r--   0 runner    (1001) docker     (123)     2562 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/users/get_users.py
--rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/users/set_bot_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/users/set_emoji_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/users/set_profile_photo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/users/set_username.py
--rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/users/unblock_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/users/update_profile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:56:15.483639 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/utilities/add_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/utilities/compose.py
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/utilities/export_session_string.py
--rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/utilities/idle.py
--rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/utilities/remove_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/utilities/restart.py
--rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/utilities/run.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1554 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/utilities/run_sync.py
--rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/utilities/start.py
--rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/utilities/stop.py
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/utilities/stop_transmission.py
--rw-r--r--   0 runner    (1001) docker     (123)    61915 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/mime_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:56:15.483639 PyroFork-dev-2.2.5.dev202307219421/pyrogram/parser/
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8681 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/parser/html.py
--rw-r--r--   0 runner    (1001) docker     (123)     5770 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/parser/markdown.py
--rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/parser/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/parser/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:56:15.483639 PyroFork-dev-2.2.5.dev202307219421/pyrogram/raw/
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/raw/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:56:15.487639 PyroFork-dev-2.2.5.dev202307219421/pyrogram/raw/core/
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/raw/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/raw/core/future_salt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/raw/core/future_salts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/raw/core/gzip_packed.py
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/raw/core/list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/raw/core/message.py
--rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/raw/core/msg_container.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:56:15.487639 PyroFork-dev-2.2.5.dev202307219421/pyrogram/raw/core/primitives/
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/raw/core/primitives/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/raw/core/primitives/bool.py
--rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/raw/core/primitives/bytes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/raw/core/primitives/double.py
--rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/raw/core/primitives/int.py
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/raw/core/primitives/string.py
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/raw/core/primitives/vector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/raw/core/tl_object.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:56:15.487639 PyroFork-dev-2.2.5.dev202307219421/pyrogram/session/
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/session/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10513 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/session/auth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:56:15.487639 PyroFork-dev-2.2.5.dev202307219421/pyrogram/session/internals/
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/session/internals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/session/internals/data_center.py
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/session/internals/msg_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/session/internals/msg_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/session/internals/seq_no.py
--rw-r--r--   0 runner    (1001) docker     (123)    13018 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/session/session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:56:15.487639 PyroFork-dev-2.2.5.dev202307219421/pyrogram/storage/
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/storage/dummy_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/storage/file_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/storage/memory_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     6845 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/storage/mongo_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:56:15.487639 PyroFork-dev-2.2.5.dev202307219421/pyrogram/storage/sqlite/
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/storage/sqlite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/storage/sqlite/cursor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/storage/sqlite/sqlite.py
--rw-r--r--   0 runner    (1001) docker     (123)     6307 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/storage/sqlite_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/storage/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/sync.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:56:15.487639 PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:56:15.487639 PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/authorization/
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/authorization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/authorization/sent_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/authorization/terms_of_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:56:15.491639 PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/bots_and_keyboards/
--rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/bots_and_keyboards/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/bots_and_keyboards/bot_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/bots_and_keyboards/bot_command_scope.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/bots_and_keyboards/bot_command_scope_all_chat_administrators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/bots_and_keyboards/bot_command_scope_all_group_chats.py
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/bots_and_keyboards/bot_command_scope_all_private_chats.py
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/bots_and_keyboards/bot_command_scope_chat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_administrators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_member.py
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/bots_and_keyboards/bot_command_scope_default.py
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/bots_and_keyboards/bot_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/bots_and_keyboards/callback_game.py
--rw-r--r--   0 runner    (1001) docker     (123)    12797 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/bots_and_keyboards/callback_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/bots_and_keyboards/force_reply.py
--rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/bots_and_keyboards/game_high_score.py
--rw-r--r--   0 runner    (1001) docker     (123)     8120 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/bots_and_keyboards/inline_keyboard_button.py
--rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/bots_and_keyboards/inline_keyboard_markup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3514 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/bots_and_keyboards/keyboard_button.py
--rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/bots_and_keyboards/login_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/bots_and_keyboards/menu_button.py
--rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/bots_and_keyboards/menu_button_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/bots_and_keyboards/menu_button_default.py
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/bots_and_keyboards/menu_button_web_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/bots_and_keyboards/reply_keyboard_markup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/bots_and_keyboards/reply_keyboard_remove.py
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/bots_and_keyboards/sent_web_app_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/bots_and_keyboards/web_app_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:56:15.499639 PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/inline_mode/
--rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/inline_mode/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/inline_mode/chosen_inline_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     7298 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/inline_mode/inline_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/inline_mode/inline_query_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     5782 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/inline_mode/inline_query_result_animation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3304 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/inline_mode/inline_query_result_article.py
--rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/inline_mode/inline_query_result_audio.py
--rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/inline_mode/inline_query_result_cached_animation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/inline_mode/inline_query_result_cached_audio.py
--rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/inline_mode/inline_query_result_cached_document.py
--rw-r--r--   0 runner    (1001) docker     (123)     4312 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/inline_mode/inline_query_result_cached_photo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/inline_mode/inline_query_result_cached_sticker.py
--rw-r--r--   0 runner    (1001) docker     (123)     4394 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/inline_mode/inline_query_result_cached_video.py
--rw-r--r--   0 runner    (1001) docker     (123)     4202 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/inline_mode/inline_query_result_cached_voice.py
--rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/inline_mode/inline_query_result_contact.py
--rw-r--r--   0 runner    (1001) docker     (123)     5240 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/inline_mode/inline_query_result_document.py
--rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/inline_mode/inline_query_result_location.py
--rw-r--r--   0 runner    (1001) docker     (123)     5261 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/inline_mode/inline_query_result_photo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/inline_mode/inline_query_result_venue.py
--rw-r--r--   0 runner    (1001) docker     (123)     5474 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/inline_mode/inline_query_result_video.py
--rw-r--r--   0 runner    (1001) docker     (123)     4360 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/inline_mode/inline_query_result_voice.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:56:15.503639 PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/input_media/
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/input_media/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/input_media/input_media.py
--rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/input_media/input_media_animation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/input_media/input_media_audio.py
--rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/input_media/input_media_document.py
--rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/input_media/input_media_photo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/input_media/input_media_video.py
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/input_media/input_phone_contact.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:56:15.503639 PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/input_message_content/
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/input_message_content/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/input_message_content/input_message_content.py
--rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/input_message_content/input_text_message_content.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/list.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:56:15.511639 PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/messages_and_media/
--rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/messages_and_media/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4044 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/messages_and_media/animation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4069 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/messages_and_media/audio.py
--rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/messages_and_media/contact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/messages_and_media/dice.py
--rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/messages_and_media/document.py
--rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/messages_and_media/game.py
--rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/messages_and_media/location.py
--rw-r--r--   0 runner    (1001) docker     (123)   153586 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/messages_and_media/message.py
--rw-r--r--   0 runner    (1001) docker     (123)     4352 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/messages_and_media/message_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/messages_and_media/message_reactions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4309 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/messages_and_media/photo.py
--rw-r--r--   0 runner    (1001) docker     (123)     8016 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/messages_and_media/poll.py
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/messages_and_media/poll_option.py
--rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/messages_and_media/reaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     6909 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/messages_and_media/sticker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/messages_and_media/stickerset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/messages_and_media/stripped_thumbnail.py
--rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/messages_and_media/thumbnail.py
--rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/messages_and_media/venue.py
--rw-r--r--   0 runner    (1001) docker     (123)     4389 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/messages_and_media/video.py
--rw-r--r--   0 runner    (1001) docker     (123)     3601 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/messages_and_media/video_note.py
--rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/messages_and_media/voice.py
--rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/messages_and_media/web_app_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     6351 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/messages_and_media/web_page.py
--rw-r--r--   0 runner    (1001) docker     (123)     3862 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/object.py
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/update.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:56:15.523640 PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/user_and_chats/
--rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/user_and_chats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33966 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/user_and_chats/chat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/user_and_chats/chat_admin_with_invite_links.py
--rw-r--r--   0 runner    (1001) docker     (123)    22023 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/user_and_chats/chat_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     5514 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/user_and_chats/chat_event_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4579 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/user_and_chats/chat_invite_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/user_and_chats/chat_join_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/user_and_chats/chat_joined_by_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/user_and_chats/chat_joiner.py
--rw-r--r--   0 runner    (1001) docker     (123)     9444 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/user_and_chats/chat_member.py
--rw-r--r--   0 runner    (1001) docker     (123)     3674 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/user_and_chats/chat_member_updated.py
--rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/user_and_chats/chat_permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3967 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/user_and_chats/chat_photo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/user_and_chats/chat_preview.py
--rw-r--r--   0 runner    (1001) docker     (123)     5300 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/user_and_chats/chat_privileges.py
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/user_and_chats/chat_reactions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/user_and_chats/dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/user_and_chats/emoji_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     4979 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/user_and_chats/forum_topic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/user_and_chats/forum_topic_closed.py
--rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/user_and_chats/forum_topic_created.py
--rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/user_and_chats/forum_topic_edited.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/user_and_chats/forum_topic_reopened.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/user_and_chats/general_forum_topic_hidden.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/user_and_chats/general_forum_topic_unhidden.py
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/user_and_chats/invite_link_importer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/user_and_chats/peer_channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/user_and_chats/peer_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/user_and_chats/restriction.py
--rw-r--r--   0 runner    (1001) docker     (123)    13658 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/user_and_chats/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/user_and_chats/username.py
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/user_and_chats/video_chat_ended.py
--rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/user_and_chats/video_chat_members_invited.py
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/user_and_chats/video_chat_scheduled.py
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/user_and_chats/video_chat_started.py
--rw-r--r--   0 runner    (1001) docker     (123)    11166 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/pyrogram/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 16:56:15.527639 PyroFork-dev-2.2.5.dev202307219421/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3559 2023-07-21 16:56:08.000000 PyroFork-dev-2.2.5.dev202307219421/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:56:15.523640 PyroFork-dev-2.2.5.dev202307219421/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:56:15.523640 PyroFork-dev-2.2.5.dev202307219421/tests/filters/
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/tests/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/tests/filters/test_command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:56:15.527639 PyroFork-dev-2.2.5.dev202307219421/tests/parser/
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/tests/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6264 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/tests/parser/test_html.py
--rw-r--r--   0 runner    (1001) docker     (123)     8208 2023-07-21 16:55:58.000000 PyroFork-dev-2.2.5.dev202307219421/tests/test_file_id.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:16:39.504521 PyroFork-dev-2.2.5.dev202307219555/
+-rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/COPYING.lesser
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     3917 2023-07-21 15:16:39.500521 PyroFork-dev-2.2.5.dev202307219555/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:16:39.392519 PyroFork-dev-2.2.5.dev202307219555/PyroFork_dev.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3917 2023-07-21 15:16:39.000000 PyroFork-dev-2.2.5.dev202307219555/PyroFork_dev.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20360 2023-07-21 15:16:39.000000 PyroFork-dev-2.2.5.dev202307219555/PyroFork_dev.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 15:16:39.000000 PyroFork-dev-2.2.5.dev202307219555/PyroFork_dev.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 15:16:39.000000 PyroFork-dev-2.2.5.dev202307219555/PyroFork_dev.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-21 15:16:39.000000 PyroFork-dev-2.2.5.dev202307219555/PyroFork_dev.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-21 15:16:39.000000 PyroFork-dev-2.2.5.dev202307219555/PyroFork_dev.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:16:39.392519 PyroFork-dev-2.2.5.dev202307219555/compiler/
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/compiler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:16:39.392519 PyroFork-dev-2.2.5.dev202307219555/compiler/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/compiler/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22402 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/compiler/api/compiler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:16:39.396519 PyroFork-dev-2.2.5.dev202307219555/compiler/api/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/compiler/api/source/auth_key.tl
+-rw-r--r--   0 runner    (1001) docker     (123)   175007 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/compiler/api/source/main_api.tl
+-rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/compiler/api/source/sys_msgs.tl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:16:39.396519 PyroFork-dev-2.2.5.dev202307219555/compiler/api/template/
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/compiler/api/template/combinator.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/compiler/api/template/type.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:16:39.396519 PyroFork-dev-2.2.5.dev202307219555/compiler/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/compiler/docs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19579 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/compiler/docs/compiler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:16:39.396519 PyroFork-dev-2.2.5.dev202307219555/compiler/docs/template/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/compiler/docs/template/page.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/compiler/docs/template/toctree.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:16:39.396519 PyroFork-dev-2.2.5.dev202307219555/compiler/errors/
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/compiler/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4917 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/compiler/errors/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/compiler/errors/sort.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:16:39.400519 PyroFork-dev-2.2.5.dev202307219555/compiler/errors/source/
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/compiler/errors/source/303_SEE_OTHER.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)    22907 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/compiler/errors/source/400_BAD_REQUEST.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/compiler/errors/source/401_UNAUTHORIZED.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/compiler/errors/source/403_FORBIDDEN.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/compiler/errors/source/406_NOT_ACCEPTABLE.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/compiler/errors/source/420_FLOOD.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)     4298 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/compiler/errors/source/500_INTERNAL_SERVER_ERROR.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/compiler/errors/source/503_SERVICE_UNAVAILABLE.tsv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:16:39.400519 PyroFork-dev-2.2.5.dev202307219555/compiler/errors/template/
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/compiler/errors/template/class.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/compiler/errors/template/sub_class.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:16:39.400519 PyroFork-dev-2.2.5.dev202307219555/pyrogram/
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-07-21 15:16:31.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41006 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:16:39.404519 PyroFork-dev-2.2.5.dev202307219555/pyrogram/connection/
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/connection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/connection/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:16:39.404519 PyroFork-dev-2.2.5.dev202307219555/pyrogram/connection/transport/
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/connection/transport/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:16:39.404519 PyroFork-dev-2.2.5.dev202307219555/pyrogram/connection/transport/tcp/
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/connection/transport/tcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4100 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/connection/transport/tcp/tcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/connection/transport/tcp/tcp_abridged.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/connection/transport/tcp/tcp_abridged_o.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/connection/transport/tcp/tcp_full.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/connection/transport/tcp/tcp_intermediate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/connection/transport/tcp/tcp_intermediate_o.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:16:39.404519 PyroFork-dev-2.2.5.dev202307219555/pyrogram/crypto/
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/crypto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4013 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/crypto/aes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4762 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/crypto/mtproto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/crypto/prime.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13437 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/crypto/rsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10085 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)   208021 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/emoji.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:16:39.408520 PyroFork-dev-2.2.5.dev202307219555/pyrogram/enums/
+-rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/enums/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/enums/auto_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/enums/chat_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4520 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/enums/chat_event_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/enums/chat_member_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/enums/chat_members_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/enums/chat_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/enums/message_entity_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/enums/message_media_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/enums/message_service_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/enums/messages_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/enums/next_code_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/enums/parse_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/enums/poll_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/enums/sent_code_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/enums/user_status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:16:39.408520 PyroFork-dev-2.2.5.dev202307219555/pyrogram/errors/
+-rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/errors/rpc_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15154 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/file_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24836 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:16:39.412520 PyroFork-dev-2.2.5.dev202307219555/pyrogram/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/handlers/callback_query_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/handlers/chat_join_request_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/handlers/chat_member_updated_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/handlers/chosen_inline_result_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/handlers/deleted_messages_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/handlers/disconnect_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/handlers/edited_message_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/handlers/handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/handlers/inline_query_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/handlers/message_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/handlers/poll_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/handlers/raw_update_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/handlers/user_status_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:16:39.412520 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:16:39.412520 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/advanced/
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/advanced/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/advanced/invoke.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4560 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/advanced/resolve_peer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8164 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/advanced/save_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:16:39.416520 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/auth/accept_terms_of_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/auth/check_password.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/auth/connect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/auth/disconnect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/auth/get_password_hint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/auth/initialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/auth/log_out.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/auth/recover_password.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/auth/resend_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/auth/send_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/auth/send_recovery_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/auth/sign_in.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/auth/sign_in_bot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/auth/sign_up.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/auth/terminate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:16:39.420520 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/bots/
+-rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/bots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/bots/answer_callback_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4990 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/bots/answer_inline_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/bots/answer_web_app_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/bots/delete_bot_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/bots/get_bot_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/bots/get_bot_default_privileges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/bots/get_chat_menu_button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/bots/get_game_high_scores.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/bots/get_inline_bot_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/bots/request_callback_answer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/bots/send_game.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/bots/send_inline_bot_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/bots/set_bot_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/bots/set_bot_default_privileges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/bots/set_chat_menu_button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3946 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/bots/set_game_score.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:16:39.432520 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/chats/
+-rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/chats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/chats/add_chat_members.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/chats/archive_chats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/chats/ban_chat_member.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/chats/close_forum_topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/chats/close_general_topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/chats/create_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/chats/create_forum_topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/chats/create_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/chats/create_supergroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/chats/delete_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/chats/delete_chat_photo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/chats/delete_forum_topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/chats/delete_supergroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/chats/delete_user_history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/chats/edit_forum_topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/chats/edit_general_topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/chats/get_chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4032 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/chats/get_chat_event_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/chats/get_chat_member.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5282 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/chats/get_chat_members.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/chats/get_chat_members_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/chats/get_chat_online_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/chats/get_dialogs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/chats/get_dialogs_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/chats/get_forum_topics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/chats/get_forum_topics_by_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/chats/get_nearby_chats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/chats/get_send_as_chats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/chats/hide_general_topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/chats/join_chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2605 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/chats/leave_chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/chats/mark_chat_unread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/chats/pin_chat_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/chats/promote_chat_member.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/chats/reopen_forum_topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/chats/reopen_general_topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/chats/restrict_chat_member.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/chats/set_administrator_title.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/chats/set_chat_description.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/chats/set_chat_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/chats/set_chat_photo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/chats/set_chat_protected_content.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/chats/set_chat_title.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/chats/set_chat_username.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/chats/set_send_as_chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/chats/set_slow_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/chats/unarchive_chats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/chats/unban_chat_member.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/chats/unhide_general_topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/chats/unpin_all_chat_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/chats/unpin_chat_message.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:16:39.436520 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/contacts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/contacts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/contacts/add_contact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/contacts/delete_contacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/contacts/get_contacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/contacts/get_contacts_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/contacts/import_contacts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:16:39.436520 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/decorators/
+-rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/decorators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/decorators/on_callback_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/decorators/on_chat_join_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/decorators/on_chat_member_updated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/decorators/on_chosen_inline_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/decorators/on_deleted_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/decorators/on_disconnect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/decorators/on_edited_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/decorators/on_inline_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/decorators/on_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/decorators/on_poll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/decorators/on_raw_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/decorators/on_user_status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:16:39.440520 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/invite_links/
+-rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/invite_links/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/invite_links/approve_all_chat_join_requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/invite_links/approve_chat_join_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/invite_links/create_chat_invite_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/invite_links/decline_all_chat_join_requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/invite_links/decline_chat_join_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/invite_links/delete_chat_admin_invite_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/invite_links/delete_chat_invite_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3533 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/invite_links/edit_chat_invite_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/invite_links/export_chat_invite_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/invite_links/get_chat_admin_invite_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/invite_links/get_chat_admin_invite_links_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/invite_links/get_chat_admins_with_invite_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/invite_links/get_chat_invite_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/invite_links/get_chat_invite_link_joiners.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/invite_links/get_chat_invite_link_joiners_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/invite_links/get_chat_join_requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/invite_links/revoke_chat_invite_link.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:16:39.452520 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/messages/
+-rw-r--r--   0 runner    (1001) docker     (123)     3921 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/messages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5963 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/messages/copy_media_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5423 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/messages/copy_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/messages/delete_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7530 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/messages/download_media.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/messages/edit_inline_caption.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10375 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/messages/edit_inline_media.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/messages/edit_inline_reply_markup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/messages/edit_inline_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/messages/edit_message_caption.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13022 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/messages/edit_message_media.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/messages/edit_message_reply_markup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/messages/edit_message_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5018 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/messages/forward_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/messages/get_chat_history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/messages/get_chat_history_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/messages/get_custom_emoji_stickers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/messages/get_discussion_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/messages/get_discussion_replies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/messages/get_discussion_replies_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/messages/get_media_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4741 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/messages/get_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/messages/inline_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/messages/read_chat_history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/messages/retract_vote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/messages/search_global.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/messages/search_global_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5349 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/messages/search_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/messages/search_messages_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12828 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/messages/send_animation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11362 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/messages/send_audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5723 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/messages/send_cached_media.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/messages/send_chat_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5111 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/messages/send_contact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5085 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/messages/send_dice.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10712 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/messages/send_document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4820 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/messages/send_location.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20821 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/messages/send_media_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7509 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/messages/send_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9682 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/messages/send_photo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8315 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/messages/send_poll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/messages/send_reaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8582 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/messages/send_sticker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5641 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/messages/send_venue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12198 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/messages/send_video.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9556 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/messages/send_video_note.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9672 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/messages/send_voice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/messages/stop_poll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/messages/stream_media.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/messages/vote_poll.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:16:39.456520 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/password/
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/password/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/password/change_cloud_password.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/password/enable_cloud_password.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/password/remove_cloud_password.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:16:39.456520 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/stickers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/stickers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/stickers/add_sticker_to_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/stickers/create_sticker_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/stickers/get_sticker_set.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:16:39.460520 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/users/
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/users/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/users/block_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/users/delete_profile_photos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4421 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/users/get_chat_photos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/users/get_chat_photos_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/users/get_common_chats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/users/get_default_emoji_statuses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/users/get_me.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2562 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/users/get_users.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/users/set_emoji_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/users/set_profile_photo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/users/set_username.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/users/unblock_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/users/update_profile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:16:39.460520 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/utilities/add_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/utilities/compose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/utilities/export_session_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/utilities/idle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/utilities/remove_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/utilities/restart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/utilities/run.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1554 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/utilities/run_sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/utilities/start.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/utilities/stop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/utilities/stop_transmission.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61915 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/mime_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:16:39.464520 PyroFork-dev-2.2.5.dev202307219555/pyrogram/parser/
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8681 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/parser/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5770 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/parser/markdown.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/parser/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/parser/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:16:39.464520 PyroFork-dev-2.2.5.dev202307219555/pyrogram/raw/
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/raw/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:16:39.464520 PyroFork-dev-2.2.5.dev202307219555/pyrogram/raw/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/raw/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/raw/core/future_salt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/raw/core/future_salts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/raw/core/gzip_packed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/raw/core/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/raw/core/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/raw/core/msg_container.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:16:39.464520 PyroFork-dev-2.2.5.dev202307219555/pyrogram/raw/core/primitives/
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/raw/core/primitives/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/raw/core/primitives/bool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/raw/core/primitives/bytes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/raw/core/primitives/double.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/raw/core/primitives/int.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/raw/core/primitives/string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/raw/core/primitives/vector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/raw/core/tl_object.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:16:39.468520 PyroFork-dev-2.2.5.dev202307219555/pyrogram/session/
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/session/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10513 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/session/auth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:16:39.468520 PyroFork-dev-2.2.5.dev202307219555/pyrogram/session/internals/
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/session/internals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/session/internals/data_center.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/session/internals/msg_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/session/internals/msg_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/session/internals/seq_no.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13018 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/session/session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:16:39.468520 PyroFork-dev-2.2.5.dev202307219555/pyrogram/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/storage/dummy_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/storage/file_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/storage/memory_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6017 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/storage/mongo_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:16:39.472520 PyroFork-dev-2.2.5.dev202307219555/pyrogram/storage/sqlite/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/storage/sqlite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/storage/sqlite/cursor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/storage/sqlite/sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6307 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/storage/sqlite_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/storage/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/sync.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:16:39.472520 PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:16:39.472520 PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/authorization/
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/authorization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/authorization/sent_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/authorization/terms_of_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:16:39.476521 PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/bots_and_keyboards/
+-rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/bots_and_keyboards/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/bots_and_keyboards/bot_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/bots_and_keyboards/bot_command_scope.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/bots_and_keyboards/bot_command_scope_all_chat_administrators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/bots_and_keyboards/bot_command_scope_all_group_chats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/bots_and_keyboards/bot_command_scope_all_private_chats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/bots_and_keyboards/bot_command_scope_chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_administrators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_member.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/bots_and_keyboards/bot_command_scope_default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/bots_and_keyboards/callback_game.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12797 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/bots_and_keyboards/callback_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/bots_and_keyboards/force_reply.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/bots_and_keyboards/game_high_score.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8120 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/bots_and_keyboards/inline_keyboard_button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/bots_and_keyboards/inline_keyboard_markup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3514 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/bots_and_keyboards/keyboard_button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/bots_and_keyboards/login_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/bots_and_keyboards/menu_button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/bots_and_keyboards/menu_button_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/bots_and_keyboards/menu_button_default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/bots_and_keyboards/menu_button_web_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/bots_and_keyboards/reply_keyboard_markup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/bots_and_keyboards/reply_keyboard_remove.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/bots_and_keyboards/sent_web_app_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/bots_and_keyboards/web_app_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:16:39.484521 PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/inline_mode/
+-rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/inline_mode/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/inline_mode/chosen_inline_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7298 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/inline_mode/inline_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/inline_mode/inline_query_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5782 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/inline_mode/inline_query_result_animation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3304 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/inline_mode/inline_query_result_article.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/inline_mode/inline_query_result_audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/inline_mode/inline_query_result_cached_animation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/inline_mode/inline_query_result_cached_audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/inline_mode/inline_query_result_cached_document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4312 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/inline_mode/inline_query_result_cached_photo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/inline_mode/inline_query_result_cached_sticker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4394 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/inline_mode/inline_query_result_cached_video.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4202 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/inline_mode/inline_query_result_cached_voice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/inline_mode/inline_query_result_contact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5240 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/inline_mode/inline_query_result_document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/inline_mode/inline_query_result_location.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5261 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/inline_mode/inline_query_result_photo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/inline_mode/inline_query_result_venue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5474 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/inline_mode/inline_query_result_video.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4360 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/inline_mode/inline_query_result_voice.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:16:39.484521 PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/input_media/
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/input_media/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/input_media/input_media.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/input_media/input_media_animation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/input_media/input_media_audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/input_media/input_media_document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/input_media/input_media_photo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/input_media/input_media_video.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/input_media/input_phone_contact.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:16:39.484521 PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/input_message_content/
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/input_message_content/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/input_message_content/input_message_content.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/input_message_content/input_text_message_content.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/list.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:16:39.492521 PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/messages_and_media/
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/messages_and_media/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4044 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/messages_and_media/animation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4069 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/messages_and_media/audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/messages_and_media/contact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/messages_and_media/dice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/messages_and_media/document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/messages_and_media/game.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/messages_and_media/location.py
+-rw-r--r--   0 runner    (1001) docker     (123)   153586 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/messages_and_media/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4352 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/messages_and_media/message_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/messages_and_media/message_reactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4309 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/messages_and_media/photo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8016 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/messages_and_media/poll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/messages_and_media/poll_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/messages_and_media/reaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6909 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/messages_and_media/sticker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/messages_and_media/stickerset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/messages_and_media/stripped_thumbnail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/messages_and_media/thumbnail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/messages_and_media/venue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4389 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/messages_and_media/video.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3601 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/messages_and_media/video_note.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/messages_and_media/voice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/messages_and_media/web_app_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6351 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/messages_and_media/web_page.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3862 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:16:39.500521 PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/user_and_chats/
+-rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/user_and_chats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33966 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/user_and_chats/chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/user_and_chats/chat_admin_with_invite_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22023 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/user_and_chats/chat_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5514 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/user_and_chats/chat_event_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4579 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/user_and_chats/chat_invite_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/user_and_chats/chat_join_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/user_and_chats/chat_joined_by_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/user_and_chats/chat_joiner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9444 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/user_and_chats/chat_member.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3674 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/user_and_chats/chat_member_updated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/user_and_chats/chat_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3967 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/user_and_chats/chat_photo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/user_and_chats/chat_preview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5300 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/user_and_chats/chat_privileges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/user_and_chats/chat_reactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/user_and_chats/dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/user_and_chats/emoji_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4970 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/user_and_chats/forum_topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/user_and_chats/forum_topic_closed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/user_and_chats/forum_topic_created.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/user_and_chats/forum_topic_edited.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/user_and_chats/forum_topic_reopened.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/user_and_chats/general_forum_topic_hidden.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/user_and_chats/general_forum_topic_unhidden.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/user_and_chats/invite_link_importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/user_and_chats/peer_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/user_and_chats/peer_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/user_and_chats/restriction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13658 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/user_and_chats/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/user_and_chats/username.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/user_and_chats/video_chat_ended.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/user_and_chats/video_chat_members_invited.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/user_and_chats/video_chat_scheduled.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/user_and_chats/video_chat_started.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11166 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/pyrogram/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 15:16:39.504521 PyroFork-dev-2.2.5.dev202307219555/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3559 2023-07-21 15:16:31.000000 PyroFork-dev-2.2.5.dev202307219555/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:16:39.500521 PyroFork-dev-2.2.5.dev202307219555/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:16:39.500521 PyroFork-dev-2.2.5.dev202307219555/tests/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/tests/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/tests/filters/test_command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:16:39.500521 PyroFork-dev-2.2.5.dev202307219555/tests/parser/
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/tests/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6264 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/tests/parser/test_html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8208 2023-07-21 15:16:20.000000 PyroFork-dev-2.2.5.dev202307219555/tests/test_file_id.py
```

### Comparing `PyroFork-dev-2.2.5.dev202307219421/COPYING` & `PyroFork-dev-2.2.5.dev202307219555/COPYING`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/COPYING.lesser` & `PyroFork-dev-2.2.5.dev202307219555/COPYING.lesser`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/NOTICE` & `PyroFork-dev-2.2.5.dev202307219555/NOTICE`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/PKG-INFO` & `PyroFork-dev-2.2.5.dev202307219555/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyroFork-dev
-Version: 2.2.5.dev202307219421
+Version: 2.2.5.dev202307219555
 Summary: Elegant, modern and asynchronous Telegram MTProto API framework in Python for users and bots
 Home-page: https://github.com/Mayuri-Chan/pyrofork
 Download-URL: https://github.com/Mayuri-Chan/pyrofork/releases/latest
 Author: wulan17
 Author-email: mayuri@mayuri.my.id
 License: LGPLv3
 Project-URL: Tracker, https://github.com/Mayuri-Chan/pyrofork/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: PyroFork-dev Version: 2.2.5.dev202307219421
+Metadata-Version: 2.1 Name: PyroFork-dev Version: 2.2.5.dev202307219555
 Summary: Elegant, modern and asynchronous Telegram MTProto API framework in
 Python for users and bots Home-page: https://github.com/Mayuri-Chan/pyrofork
 Download-URL: https://github.com/Mayuri-Chan/pyrofork/releases/latest Author:
 wulan17 Author-email: mayuri@mayuri.my.id License: LGPLv3 Project-URL: Tracker,
 https://github.com/Mayuri-Chan/pyrofork/issues Project-URL: Source, https://
 github.com/Mayuri-Chan/pyrofork Project-URL: Documentation, https://
 pyrofork.mayuri.my.id Keywords: telegram chat messenger mtproto api client
```

### Comparing `PyroFork-dev-2.2.5.dev202307219421/PyroFork_dev.egg-info/PKG-INFO` & `PyroFork-dev-2.2.5.dev202307219555/PyroFork_dev.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyroFork-dev
-Version: 2.2.5.dev202307219421
+Version: 2.2.5.dev202307219555
 Summary: Elegant, modern and asynchronous Telegram MTProto API framework in Python for users and bots
 Home-page: https://github.com/Mayuri-Chan/pyrofork
 Download-URL: https://github.com/Mayuri-Chan/pyrofork/releases/latest
 Author: wulan17
 Author-email: mayuri@mayuri.my.id
 License: LGPLv3
 Project-URL: Tracker, https://github.com/Mayuri-Chan/pyrofork/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: PyroFork-dev Version: 2.2.5.dev202307219421
+Metadata-Version: 2.1 Name: PyroFork-dev Version: 2.2.5.dev202307219555
 Summary: Elegant, modern and asynchronous Telegram MTProto API framework in
 Python for users and bots Home-page: https://github.com/Mayuri-Chan/pyrofork
 Download-URL: https://github.com/Mayuri-Chan/pyrofork/releases/latest Author:
 wulan17 Author-email: mayuri@mayuri.my.id License: LGPLv3 Project-URL: Tracker,
 https://github.com/Mayuri-Chan/pyrofork/issues Project-URL: Source, https://
 github.com/Mayuri-Chan/pyrofork Project-URL: Documentation, https://
 pyrofork.mayuri.my.id Keywords: telegram chat messenger mtproto api client
```

### Comparing `PyroFork-dev-2.2.5.dev202307219421/PyroFork_dev.egg-info/SOURCES.txt` & `PyroFork-dev-2.2.5.dev202307219555/PyroFork_dev.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -277,22 +277,20 @@
 pyrogram/methods/stickers/__init__.py
 pyrogram/methods/stickers/add_sticker_to_set.py
 pyrogram/methods/stickers/create_sticker_set.py
 pyrogram/methods/stickers/get_sticker_set.py
 pyrogram/methods/users/__init__.py
 pyrogram/methods/users/block_user.py
 pyrogram/methods/users/delete_profile_photos.py
-pyrogram/methods/users/get_bot_info.py
 pyrogram/methods/users/get_chat_photos.py
 pyrogram/methods/users/get_chat_photos_count.py
 pyrogram/methods/users/get_common_chats.py
 pyrogram/methods/users/get_default_emoji_statuses.py
 pyrogram/methods/users/get_me.py
 pyrogram/methods/users/get_users.py
-pyrogram/methods/users/set_bot_info.py
 pyrogram/methods/users/set_emoji_status.py
 pyrogram/methods/users/set_profile_photo.py
 pyrogram/methods/users/set_username.py
 pyrogram/methods/users/unblock_user.py
 pyrogram/methods/users/update_profile.py
 pyrogram/methods/utilities/__init__.py
 pyrogram/methods/utilities/add_handler.py
@@ -358,15 +356,14 @@
 pyrogram/types/bots_and_keyboards/bot_command_scope_all_chat_administrators.py
 pyrogram/types/bots_and_keyboards/bot_command_scope_all_group_chats.py
 pyrogram/types/bots_and_keyboards/bot_command_scope_all_private_chats.py
 pyrogram/types/bots_and_keyboards/bot_command_scope_chat.py
 pyrogram/types/bots_and_keyboards/bot_command_scope_chat_administrators.py
 pyrogram/types/bots_and_keyboards/bot_command_scope_chat_member.py
 pyrogram/types/bots_and_keyboards/bot_command_scope_default.py
-pyrogram/types/bots_and_keyboards/bot_info.py
 pyrogram/types/bots_and_keyboards/callback_game.py
 pyrogram/types/bots_and_keyboards/callback_query.py
 pyrogram/types/bots_and_keyboards/force_reply.py
 pyrogram/types/bots_and_keyboards/game_high_score.py
 pyrogram/types/bots_and_keyboards/inline_keyboard_button.py
 pyrogram/types/bots_and_keyboards/inline_keyboard_markup.py
 pyrogram/types/bots_and_keyboards/keyboard_button.py
```

### Comparing `PyroFork-dev-2.2.5.dev202307219421/README.md` & `PyroFork-dev-2.2.5.dev202307219555/README.md`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/compiler/__init__.py` & `PyroFork-dev-2.2.5.dev202307219555/compiler/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/compiler/api/__init__.py` & `PyroFork-dev-2.2.5.dev202307219555/compiler/api/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/compiler/api/compiler.py` & `PyroFork-dev-2.2.5.dev202307219555/compiler/api/compiler.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/compiler/api/source/auth_key.tl` & `PyroFork-dev-2.2.5.dev202307219555/compiler/api/source/auth_key.tl`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/compiler/api/source/main_api.tl` & `PyroFork-dev-2.2.5.dev202307219555/compiler/api/source/main_api.tl`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/compiler/api/source/sys_msgs.tl` & `PyroFork-dev-2.2.5.dev202307219555/compiler/api/source/sys_msgs.tl`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/compiler/api/template/combinator.txt` & `PyroFork-dev-2.2.5.dev202307219555/compiler/api/template/combinator.txt`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/compiler/api/template/type.txt` & `PyroFork-dev-2.2.5.dev202307219555/compiler/api/template/type.txt`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/compiler/docs/__init__.py` & `PyroFork-dev-2.2.5.dev202307219555/compiler/docs/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/compiler/docs/compiler.py` & `PyroFork-dev-2.2.5.dev202307219555/compiler/docs/compiler.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/compiler/errors/__init__.py` & `PyroFork-dev-2.2.5.dev202307219555/compiler/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/compiler/errors/compiler.py` & `PyroFork-dev-2.2.5.dev202307219555/compiler/errors/compiler.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/compiler/errors/sort.py` & `PyroFork-dev-2.2.5.dev202307219555/compiler/errors/sort.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/compiler/errors/source/400_BAD_REQUEST.tsv` & `PyroFork-dev-2.2.5.dev202307219555/compiler/errors/source/400_BAD_REQUEST.tsv`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/compiler/errors/source/401_UNAUTHORIZED.tsv` & `PyroFork-dev-2.2.5.dev202307219555/compiler/errors/source/401_UNAUTHORIZED.tsv`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/compiler/errors/source/403_FORBIDDEN.tsv` & `PyroFork-dev-2.2.5.dev202307219555/compiler/errors/source/403_FORBIDDEN.tsv`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/compiler/errors/source/406_NOT_ACCEPTABLE.tsv` & `PyroFork-dev-2.2.5.dev202307219555/compiler/errors/source/406_NOT_ACCEPTABLE.tsv`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/compiler/errors/source/500_INTERNAL_SERVER_ERROR.tsv` & `PyroFork-dev-2.2.5.dev202307219555/compiler/errors/source/500_INTERNAL_SERVER_ERROR.tsv`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/__init__.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
 __fork_name__ = "PyroFork-dev"
-__version__ = "2.2.5.dev202307219421"
+__version__ = "2.2.5.dev202307219555"
 __license__ = "GNU Lesser General Public License v3.0 (LGPL-3.0)"
 __copyright__ = "Copyright (C) 2017-present Dan <https://github.com/delivrance>"
 
 from concurrent.futures.thread import ThreadPoolExecutor
 
 
 class StopTransmission(Exception):
```

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/client.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/client.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/connection/__init__.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/connection/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/connection/connection.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/connection/connection.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/connection/transport/__init__.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/connection/transport/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/connection/transport/tcp/__init__.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/connection/transport/tcp/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/connection/transport/tcp/tcp.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/connection/transport/tcp/tcp.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/connection/transport/tcp/tcp_abridged.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/connection/transport/tcp/tcp_abridged.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/connection/transport/tcp/tcp_abridged_o.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/connection/transport/tcp/tcp_abridged_o.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/connection/transport/tcp/tcp_full.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/connection/transport/tcp/tcp_full.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/connection/transport/tcp/tcp_intermediate.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/connection/transport/tcp/tcp_intermediate.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/connection/transport/tcp/tcp_intermediate_o.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/connection/transport/tcp/tcp_intermediate_o.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/crypto/__init__.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/crypto/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/crypto/aes.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/crypto/aes.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/crypto/mtproto.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/crypto/mtproto.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/crypto/prime.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/crypto/prime.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/crypto/rsa.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/crypto/rsa.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/dispatcher.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/dispatcher.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/emoji.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/emoji.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/enums/__init__.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/enums/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/enums/auto_name.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/enums/auto_name.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/enums/chat_action.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/enums/chat_action.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/enums/chat_event_action.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/enums/chat_event_action.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/enums/chat_member_status.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/enums/chat_member_status.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/enums/chat_members_filter.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/enums/chat_members_filter.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/enums/chat_type.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/enums/chat_type.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/enums/message_entity_type.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/enums/message_entity_type.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/enums/message_media_type.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/enums/message_media_type.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/enums/message_service_type.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/enums/message_service_type.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/enums/messages_filter.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/enums/messages_filter.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/enums/next_code_type.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/enums/next_code_type.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/enums/parse_mode.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/enums/parse_mode.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/enums/poll_type.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/enums/poll_type.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/enums/sent_code_type.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/enums/sent_code_type.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/enums/user_status.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/enums/user_status.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/errors/__init__.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/errors/rpc_error.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/errors/rpc_error.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/file_id.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/file_id.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/filters.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/filters.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/handlers/__init__.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/handlers/callback_query_handler.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/handlers/callback_query_handler.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/handlers/chat_join_request_handler.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/handlers/chat_join_request_handler.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/handlers/chat_member_updated_handler.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/handlers/chat_member_updated_handler.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/handlers/chosen_inline_result_handler.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/handlers/chosen_inline_result_handler.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/handlers/deleted_messages_handler.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/handlers/deleted_messages_handler.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/handlers/disconnect_handler.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/handlers/disconnect_handler.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/handlers/edited_message_handler.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/handlers/edited_message_handler.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/handlers/handler.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/handlers/handler.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/handlers/inline_query_handler.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/handlers/inline_query_handler.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/handlers/message_handler.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/handlers/message_handler.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/handlers/poll_handler.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/handlers/poll_handler.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/handlers/raw_update_handler.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/handlers/raw_update_handler.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/handlers/user_status_handler.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/handlers/user_status_handler.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/__init__.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/advanced/__init__.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/advanced/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/advanced/invoke.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/advanced/invoke.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/advanced/resolve_peer.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/advanced/resolve_peer.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/advanced/save_file.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/advanced/save_file.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/auth/__init__.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/auth/accept_terms_of_service.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/auth/accept_terms_of_service.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/auth/check_password.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/auth/check_password.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/auth/connect.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/auth/connect.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/auth/disconnect.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/auth/disconnect.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/auth/get_password_hint.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/auth/get_password_hint.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/auth/initialize.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/auth/initialize.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/auth/log_out.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/auth/log_out.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/auth/recover_password.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/auth/recover_password.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/auth/resend_code.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/auth/resend_code.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/auth/send_code.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/auth/send_code.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/auth/send_recovery_code.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/auth/send_recovery_code.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/auth/sign_in.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/auth/sign_in.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/auth/sign_in_bot.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/auth/sign_in_bot.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/auth/sign_up.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/auth/sign_up.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/auth/terminate.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/auth/terminate.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/bots/__init__.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/bots/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/bots/answer_callback_query.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/bots/answer_callback_query.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/bots/answer_inline_query.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/bots/answer_inline_query.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/bots/answer_web_app_query.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/bots/answer_web_app_query.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/bots/delete_bot_commands.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/bots/delete_bot_commands.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/bots/get_bot_commands.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/bots/get_bot_commands.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/bots/get_bot_default_privileges.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/bots/get_bot_default_privileges.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/bots/get_chat_menu_button.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/bots/get_chat_menu_button.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/bots/get_game_high_scores.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/bots/get_game_high_scores.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/bots/get_inline_bot_results.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/bots/get_inline_bot_results.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/bots/request_callback_answer.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/bots/request_callback_answer.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/bots/send_game.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/bots/send_game.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/bots/send_inline_bot_result.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/bots/send_inline_bot_result.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/bots/set_bot_commands.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/bots/set_bot_commands.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/bots/set_bot_default_privileges.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/bots/set_bot_default_privileges.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/bots/set_chat_menu_button.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/bots/set_chat_menu_button.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/bots/set_game_score.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/bots/set_game_score.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/chats/__init__.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/chats/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/chats/add_chat_members.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/chats/add_chat_members.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/chats/archive_chats.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/chats/archive_chats.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/chats/ban_chat_member.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/chats/ban_chat_member.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/chats/close_forum_topic.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/chats/close_forum_topic.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,24 @@
-#  Pyrofork - Telegram MTProto API Client Library for Python
-#  Copyright (C) 2022-present Mayuri-Chan <https://github.com/Mayuri-Chan>
+#  Pyrogram - Telegram MTProto API Client Library for Python
+#  Copyright (C) 2017-present Dan <https://github.com/delivrance>
 #
-#  This file is part of Pyrofork.
+#  This file is part of Pyrogram.
 #
-#  Pyrofork is free software: you can redistribute it and/or modify
+#  Pyrogram is free software: you can redistribute it and/or modify
 #  it under the terms of the GNU Lesser General Public License as published
 #  by the Free Software Foundation, either version 3 of the License, or
 #  (at your option) any later version.
 #
-#  Pyrofork is distributed in the hope that it will be useful,
+#  Pyrogram is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
-#  along with Pyrofork.  If not, see <http://www.gnu.org/licenses/>.
-
+#  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 import pyrogram
 from pyrogram import raw
 from pyrogram import types
 from typing import Union
 
 
 class CloseForumTopic:
```

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/chats/close_general_topic.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/chats/reopen_forum_topic.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,53 +1,56 @@
-#  Pyrofork - Telegram MTProto API Client Library for Python
-#  Copyright (C) 2022-present Mayuri-Chan <https://github.com/Mayuri-Chan>
+#  Pyrogram - Telegram MTProto API Client Library for Python
+#  Copyright (C) 2017-present Dan <https://github.com/delivrance>
 #
-#  This file is part of Pyrofork.
+#  This file is part of Pyrogram.
 #
-#  Pyrofork is free software: you can redistribute it and/or modify
+#  Pyrogram is free software: you can redistribute it and/or modify
 #  it under the terms of the GNU Lesser General Public License as published
 #  by the Free Software Foundation, either version 3 of the License, or
 #  (at your option) any later version.
 #
-#  Pyrofork is distributed in the hope that it will be useful,
+#  Pyrogram is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
-#  along with Pyrofork.  If not, see <http://www.gnu.org/licenses/>.
-
+#  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 import pyrogram
 from pyrogram import raw
 from pyrogram import types
 from typing import Union
 
 
-class CloseGeneralTopic:
-    async def close_general_topic(
+class ReopenForumTopic:
+    async def reopen_forum_topic(
         self: "pyrogram.Client",
-        chat_id: Union[int, str]
+        chat_id: Union[int, str],
+        topic_id: int
     ) -> bool:
-        """Close a forum topic.
+        """Reopen a forum topic.
 
         .. include:: /_includes/usable-by/users-bots.rst
 
         Parameters:
             chat_id (``int`` | ``str``):
                 Unique identifier (int) or username (str) of the target chat.
 
+            topic_id (``int``):
+                Unique identifier (int) of the target forum topic.
+
         Returns:
-            `bool`: On success, a True is returned.
+            `bool`: On success, a Boolean is returned.
 
         Example:
             .. code-block:: python
 
-                await app.close_general_topic(chat_id)
+                await app.reopen_forum_topic(chat_id, topic_id)
         """
         await self.invoke(
             raw.functions.channels.EditForumTopic(
                 channel=await self.resolve_peer(chat_id),
-                topic_id=1,
-                closed=True
+                topic_id=topic_id,
+                closed=False
             )
         )
         return True
```

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/chats/create_channel.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/chats/create_channel.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/chats/create_forum_topic.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/chats/create_forum_topic.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,24 @@
-#  Pyrofork - Telegram MTProto API Client Library for Python
-#  Copyright (C) 2022-present Mayuri-Chan <https://github.com/Mayuri-Chan>
+#  Pyrogram - Telegram MTProto API Client Library for Python
+#  Copyright (C) 2017-present Dan <https://github.com/delivrance>
 #
-#  This file is part of Pyrofork.
+#  This file is part of Pyrogram.
 #
-#  Pyrofork is free software: you can redistribute it and/or modify
+#  Pyrogram is free software: you can redistribute it and/or modify
 #  it under the terms of the GNU Lesser General Public License as published
 #  by the Free Software Foundation, either version 3 of the License, or
 #  (at your option) any later version.
 #
-#  Pyrofork is distributed in the hope that it will be useful,
+#  Pyrogram is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
-#  along with Pyrofork.  If not, see <http://www.gnu.org/licenses/>.
-
+#  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 import pyrogram
 from pyrogram import raw
 from pyrogram import types
 from typing import Union
 
 
 class CreateForumTopic:
```

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/chats/create_group.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/chats/create_group.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/chats/create_supergroup.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/chats/create_supergroup.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/chats/delete_channel.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/chats/delete_channel.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/chats/delete_chat_photo.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/chats/delete_chat_photo.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/chats/delete_forum_topic.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/chats/get_chat_online_count.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,60 +1,51 @@
-#  Pyrofork - Telegram MTProto API Client Library for Python
-#  Copyright (C) 2022-present Mayuri-Chan <https://github.com/Mayuri-Chan>
+#  Pyrogram - Telegram MTProto API Client Library for Python
+#  Copyright (C) 2017-present Dan <https://github.com/delivrance>
 #
-#  This file is part of Pyrofork.
+#  This file is part of Pyrogram.
 #
-#  Pyrofork is free software: you can redistribute it and/or modify
+#  Pyrogram is free software: you can redistribute it and/or modify
 #  it under the terms of the GNU Lesser General Public License as published
 #  by the Free Software Foundation, either version 3 of the License, or
 #  (at your option) any later version.
 #
-#  Pyrofork is distributed in the hope that it will be useful,
+#  Pyrogram is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
-#  along with Pyrofork.  If not, see <http://www.gnu.org/licenses/>.
+#  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
+
+from typing import Union
 
 import pyrogram
 from pyrogram import raw
-from pyrogram import types
-from typing import Union
 
 
-class DeleteForumTopic:
-    async def delete_forum_topic(
+class GetChatOnlineCount:
+    async def get_chat_online_count(
         self: "pyrogram.Client",
-        chat_id: Union[int, str],
-        topic_id: int
-    ) -> bool:
-        """Delete a forum topic.
+        chat_id: Union[int, str]
+    ) -> int:
+        """Get the number of members that are currently online in a chat.
 
-        .. include:: /_includes/usable-by/users-bots.rst
+        .. include:: /_includes/usable-by/users.rst
 
         Parameters:
             chat_id (``int`` | ``str``):
                 Unique identifier (int) or username (str) of the target chat.
 
-            topic_id (``int``):
-                Unique identifier (int) of the target forum topic.
-
         Returns:
-            `bool`: On success, a Boolean is returned.
+            ``int``: On success, the chat members online count is returned.
 
         Example:
             .. code-block:: python
 
-                await app.delete_forum_topic(chat_id, topic_id)
+                online = await app.get_chat_online_count(chat_id)
+                print(online)
         """
-        try:
-            await self.invoke(
-                raw.functions.channels.DeleteTopicHistory(
-                    channel=await self.resolve_peer(chat_id),
-                    top_msg_id=topic_id
-                )
+        return (await self.invoke(
+            raw.functions.messages.GetOnlines(
+                peer=await self.resolve_peer(chat_id)
             )
-        except Exception as e:
-            print(e)
-            return False
-        return True
+        )).onlines
```

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/chats/delete_supergroup.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/chats/delete_supergroup.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/chats/delete_user_history.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/chats/delete_user_history.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/chats/edit_forum_topic.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/chats/edit_forum_topic.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,24 @@
-#  Pyrofork - Telegram MTProto API Client Library for Python
-#  Copyright (C) 2022-present Mayuri-Chan <https://github.com/Mayuri-Chan>
+#  Pyrogram - Telegram MTProto API Client Library for Python
+#  Copyright (C) 2017-present Dan <https://github.com/delivrance>
 #
-#  This file is part of Pyrofork.
+#  This file is part of Pyrogram.
 #
-#  Pyrofork is free software: you can redistribute it and/or modify
+#  Pyrogram is free software: you can redistribute it and/or modify
 #  it under the terms of the GNU Lesser General Public License as published
 #  by the Free Software Foundation, either version 3 of the License, or
 #  (at your option) any later version.
 #
-#  Pyrofork is distributed in the hope that it will be useful,
+#  Pyrogram is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
-#  along with Pyrofork.  If not, see <http://www.gnu.org/licenses/>.
-
+#  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 import pyrogram
 from pyrogram import raw
 from pyrogram import types
 from typing import Union
 
 
 class EditForumTopic:
```

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/chats/edit_general_topic.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/chats/reopen_general_topic.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,57 +1,52 @@
-#  Pyrofork - Telegram MTProto API Client Library for Python
-#  Copyright (C) 2022-present Mayuri-Chan <https://github.com/Mayuri-Chan>
+#  Pyrogram - Telegram MTProto API Client Library for Python
+#  Copyright (C) 2017-present Dan <https://github.com/delivrance>
 #
-#  This file is part of Pyrofork.
+#  This file is part of Pyrogram.
 #
-#  Pyrofork is free software: you can redistribute it and/or modify
+#  Pyrogram is free software: you can redistribute it and/or modify
 #  it under the terms of the GNU Lesser General Public License as published
 #  by the Free Software Foundation, either version 3 of the License, or
 #  (at your option) any later version.
 #
-#  Pyrofork is distributed in the hope that it will be useful,
+#  Pyrogram is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
-#  along with Pyrofork.  If not, see <http://www.gnu.org/licenses/>.
-
+#  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 import pyrogram
 from pyrogram import raw
 from pyrogram import types
 from typing import Union
 
 
-class EditGeneralTopic:
-    async def edit_general_topic(
+class ReopenGeneralTopic:
+    async def reopen_general_topic(
         self: "pyrogram.Client",
-        chat_id: Union[int, str],
-        title: str
+        chat_id: Union[int, str]
     ) -> bool:
-        """Edit a general forum topic.
+        """Reopen a general forum topic.
 
         .. include:: /_includes/usable-by/users-bots.rst
 
         Parameters:
             chat_id (``int`` | ``str``):
                 Unique identifier (int) or username (str) of the target chat.
 
-            title (``str``):
-                The general forum topic title.
-
         Returns:
             `bool`: On success, a True is returned.
 
         Example:
             .. code-block:: python
 
-                await app.edit_general_topic(chat_id,"New Topic Title")
+                await app.reopen_general_topic(chat_id, topic_id)
         """
         await self.invoke(
             raw.functions.channels.EditForumTopic(
                 channel=await self.resolve_peer(chat_id),
                 topic_id=1,
-                title=title
+                closed=False
             )
         )
         return True
```

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/chats/get_chat.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/chats/get_chat.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/chats/get_chat_event_log.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/chats/get_chat_event_log.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/chats/get_chat_member.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/chats/get_chat_member.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/chats/get_chat_members.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/chats/get_chat_members.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/chats/get_chat_members_count.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/chats/get_chat_members_count.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/chats/get_chat_online_count.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/invite_links/approve_chat_join_request.py`

 * *Files 11% similar despite different names*

```diff
@@ -18,34 +18,40 @@
 
 from typing import Union
 
 import pyrogram
 from pyrogram import raw
 
 
-class GetChatOnlineCount:
-    async def get_chat_online_count(
+class ApproveChatJoinRequest:
+    async def approve_chat_join_request(
         self: "pyrogram.Client",
-        chat_id: Union[int, str]
-    ) -> int:
-        """Get the number of members that are currently online in a chat.
+        chat_id: Union[int, str],
+        user_id: int,
+    ) -> bool:
+        """Approve a chat join request.
 
-        .. include:: /_includes/usable-by/users.rst
+        You must be an administrator in the chat for this to work and must have the *can_invite_users* administrator
+        right.
+
+        .. include:: /_includes/usable-by/users-bots.rst
 
         Parameters:
             chat_id (``int`` | ``str``):
-                Unique identifier (int) or username (str) of the target chat.
-
-        Returns:
-            ``int``: On success, the chat members online count is returned.
+                Unique identifier for the target chat or username of the target channel/supergroup
+                (in the format @username).
 
-        Example:
-            .. code-block:: python
+            user_id (``int``):
+                Unique identifier of the target user.
 
-                online = await app.get_chat_online_count(chat_id)
-                print(online)
+        Returns:
+            ``bool``: True on success.
         """
-        return (await self.invoke(
-            raw.functions.messages.GetOnlines(
-                peer=await self.resolve_peer(chat_id)
+        await self.invoke(
+            raw.functions.messages.HideChatJoinRequest(
+                peer=await self.resolve_peer(chat_id),
+                user_id=await self.resolve_peer(user_id),
+                approved=True
             )
-        )).onlines
+        )
+
+        return True
```

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/chats/get_dialogs.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/chats/get_dialogs.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/chats/get_dialogs_count.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/chats/get_dialogs_count.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/chats/get_forum_topics.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/chats/get_forum_topics.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-#  Pyrofork - Telegram MTProto API Client Library for Python
-#  Copyright (C) 2022-present Mayuri-Chan <https://github.com/Mayuri-Chan>
+#  Pyrogram - Telegram MTProto API Client Library for Python
+#  Copyright (C) 2017-present Dan <https://github.com/delivrance>
 #
-#  This file is part of Pyrofork.
+#  This file is part of Pyrogram.
 #
-#  Pyrofork is free software: you can redistribute it and/or modify
+#  Pyrogram is free software: you can redistribute it and/or modify
 #  it under the terms of the GNU Lesser General Public License as published
 #  by the Free Software Foundation, either version 3 of the License, or
 #  (at your option) any later version.
 #
-#  Pyrofork is distributed in the hope that it will be useful,
+#  Pyrogram is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
-#  along with Pyrofork.  If not, see <http://www.gnu.org/licenses/>.
+#  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
 import logging
 from typing import Union, Optional, AsyncGenerator
 
 import pyrogram
 from pyrogram import raw
 from pyrogram import types
```

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/chats/get_forum_topics_by_id.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/chats/get_forum_topics_by_id.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-#  Pyrofork - Telegram MTProto API Client Library for Python
-#  Copyright (C) 2022-present Mayuri-Chan <https://github.com/Mayuri-Chan>
+#  Pyrogram - Telegram MTProto API Client Library for Python
+#  Copyright (C) 2017-present Dan <https://github.com/delivrance>
 #
-#  This file is part of Pyrofork.
+#  This file is part of Pyrogram.
 #
-#  Pyrofork is free software: you can redistribute it and/or modify
+#  Pyrogram is free software: you can redistribute it and/or modify
 #  it under the terms of the GNU Lesser General Public License as published
 #  by the Free Software Foundation, either version 3 of the License, or
 #  (at your option) any later version.
 #
-#  Pyrofork is distributed in the hope that it will be useful,
+#  Pyrogram is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
-#  along with Pyrofork.  If not, see <http://www.gnu.org/licenses/>.
+#  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
 import logging
 from typing import Union, List, Iterable
 
 import pyrogram
 from pyrogram import raw
 from pyrogram import types
```

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/chats/get_nearby_chats.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/chats/get_nearby_chats.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/chats/get_send_as_chats.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/chats/get_send_as_chats.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/chats/hide_general_topic.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/chats/hide_general_topic.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,24 @@
-#  Pyrofork - Telegram MTProto API Client Library for Python
-#  Copyright (C) 2022-present Mayuri-Chan <https://github.com/Mayuri-Chan>
+#  Pyrogram - Telegram MTProto API Client Library for Python
+#  Copyright (C) 2017-present Dan <https://github.com/delivrance>
 #
-#  This file is part of Pyrofork.
+#  This file is part of Pyrogram.
 #
-#  Pyrofork is free software: you can redistribute it and/or modify
+#  Pyrogram is free software: you can redistribute it and/or modify
 #  it under the terms of the GNU Lesser General Public License as published
 #  by the Free Software Foundation, either version 3 of the License, or
 #  (at your option) any later version.
 #
-#  Pyrofork is distributed in the hope that it will be useful,
+#  Pyrogram is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
-#  along with Pyrofork.  If not, see <http://www.gnu.org/licenses/>.
-
+#  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 import pyrogram
 from pyrogram import raw
 from pyrogram import types
 from typing import Union
 
 
 class HideGeneralTopic:
```

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/chats/join_chat.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/chats/join_chat.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/chats/leave_chat.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/chats/leave_chat.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/chats/mark_chat_unread.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/chats/mark_chat_unread.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/chats/pin_chat_message.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/chats/pin_chat_message.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/chats/promote_chat_member.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/chats/promote_chat_member.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/chats/reopen_forum_topic.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/chats/unhide_general_topic.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,57 +1,52 @@
-#  Pyrofork - Telegram MTProto API Client Library for Python
-#  Copyright (C) 2022-present Mayuri-Chan <https://github.com/Mayuri-Chan>
+#  Pyrogram - Telegram MTProto API Client Library for Python
+#  Copyright (C) 2017-present Dan <https://github.com/delivrance>
 #
-#  This file is part of Pyrofork.
+#  This file is part of Pyrogram.
 #
-#  Pyrofork is free software: you can redistribute it and/or modify
+#  Pyrogram is free software: you can redistribute it and/or modify
 #  it under the terms of the GNU Lesser General Public License as published
 #  by the Free Software Foundation, either version 3 of the License, or
 #  (at your option) any later version.
 #
-#  Pyrofork is distributed in the hope that it will be useful,
+#  Pyrogram is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
-#  along with Pyrofork.  If not, see <http://www.gnu.org/licenses/>.
-
+#  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 import pyrogram
 from pyrogram import raw
 from pyrogram import types
 from typing import Union
 
 
-class ReopenForumTopic:
-    async def reopen_forum_topic(
+class UnhideGeneralTopic:
+    async def unhide_general_topic(
         self: "pyrogram.Client",
-        chat_id: Union[int, str],
-        topic_id: int
+        chat_id: Union[int, str]
     ) -> bool:
-        """Reopen a forum topic.
+        """unhide a general forum topic.
 
         .. include:: /_includes/usable-by/users-bots.rst
 
         Parameters:
             chat_id (``int`` | ``str``):
                 Unique identifier (int) or username (str) of the target chat.
 
-            topic_id (``int``):
-                Unique identifier (int) of the target forum topic.
-
         Returns:
-            `bool`: On success, a Boolean is returned.
+            `bool`: On success, a True is returned.
 
         Example:
             .. code-block:: python
 
-                await app.reopen_forum_topic(chat_id, topic_id)
+                await app.unhide_general_topic(chat_id)
         """
         await self.invoke(
             raw.functions.channels.EditForumTopic(
                 channel=await self.resolve_peer(chat_id),
-                topic_id=topic_id,
-                closed=False
+                topic_id=1,
+                hidden=False
             )
         )
         return True
```

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/chats/reopen_general_topic.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/chats/delete_forum_topic.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,53 +1,59 @@
-#  Pyrofork - Telegram MTProto API Client Library for Python
-#  Copyright (C) 2022-present Mayuri-Chan <https://github.com/Mayuri-Chan>
+#  Pyrogram - Telegram MTProto API Client Library for Python
+#  Copyright (C) 2017-present Dan <https://github.com/delivrance>
 #
-#  This file is part of Pyrofork.
+#  This file is part of Pyrogram.
 #
-#  Pyrofork is free software: you can redistribute it and/or modify
+#  Pyrogram is free software: you can redistribute it and/or modify
 #  it under the terms of the GNU Lesser General Public License as published
 #  by the Free Software Foundation, either version 3 of the License, or
 #  (at your option) any later version.
 #
-#  Pyrofork is distributed in the hope that it will be useful,
+#  Pyrogram is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
-#  along with Pyrofork.  If not, see <http://www.gnu.org/licenses/>.
-
+#  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 import pyrogram
 from pyrogram import raw
 from pyrogram import types
 from typing import Union
 
 
-class ReopenGeneralTopic:
-    async def reopen_general_topic(
+class DeleteForumTopic:
+    async def delete_forum_topic(
         self: "pyrogram.Client",
-        chat_id: Union[int, str]
+        chat_id: Union[int, str],
+        topic_id: int
     ) -> bool:
-        """Reopen a general forum topic.
+        """Delete a forum topic.
 
         .. include:: /_includes/usable-by/users-bots.rst
 
         Parameters:
             chat_id (``int`` | ``str``):
                 Unique identifier (int) or username (str) of the target chat.
 
+            topic_id (``int``):
+                Unique identifier (int) of the target forum topic.
+
         Returns:
-            `bool`: On success, a True is returned.
+            `bool`: On success, a Boolean is returned.
 
         Example:
             .. code-block:: python
 
-                await app.reopen_general_topic(chat_id, topic_id)
+                await app.delete_forum_topic(chat_id, topic_id)
         """
-        await self.invoke(
-            raw.functions.channels.EditForumTopic(
-                channel=await self.resolve_peer(chat_id),
-                topic_id=1,
-                closed=False
+        try:
+            await self.invoke(
+                raw.functions.channels.DeleteTopicHistory(
+                    channel=await self.resolve_peer(chat_id),
+                    top_msg_id=topic_id
+                )
             )
-        )
+        except Exception as e:
+            print(e)
+            return False
         return True
```

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/chats/restrict_chat_member.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/chats/restrict_chat_member.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/chats/set_administrator_title.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/chats/set_administrator_title.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/chats/set_chat_description.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/chats/set_chat_description.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/chats/set_chat_permissions.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/chats/set_chat_permissions.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/chats/set_chat_photo.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/chats/set_chat_photo.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/chats/set_chat_protected_content.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/chats/set_chat_protected_content.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/chats/set_chat_title.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/chats/set_chat_title.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/chats/set_chat_username.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/chats/set_chat_username.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/chats/set_send_as_chat.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/chats/set_send_as_chat.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/chats/set_slow_mode.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/chats/set_slow_mode.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/chats/unarchive_chats.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/chats/unarchive_chats.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/chats/unban_chat_member.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/chats/unban_chat_member.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/chats/unhide_general_topic.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/invite_links/decline_chat_join_request.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,53 +1,57 @@
-#  Pyrofork - Telegram MTProto API Client Library for Python
-#  Copyright (C) 2022-present Mayuri-Chan <https://github.com/Mayuri-Chan>
+#  Pyrogram - Telegram MTProto API Client Library for Python
+#  Copyright (C) 2017-present Dan <https://github.com/delivrance>
 #
-#  This file is part of Pyrofork.
+#  This file is part of Pyrogram.
 #
-#  Pyrofork is free software: you can redistribute it and/or modify
+#  Pyrogram is free software: you can redistribute it and/or modify
 #  it under the terms of the GNU Lesser General Public License as published
 #  by the Free Software Foundation, either version 3 of the License, or
 #  (at your option) any later version.
 #
-#  Pyrofork is distributed in the hope that it will be useful,
+#  Pyrogram is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
-#  along with Pyrofork.  If not, see <http://www.gnu.org/licenses/>.
+#  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
+
+from typing import Union
 
 import pyrogram
 from pyrogram import raw
-from pyrogram import types
-from typing import Union
 
 
-class UnhideGeneralTopic:
-    async def unhide_general_topic(
+class DeclineChatJoinRequest:
+    async def decline_chat_join_request(
         self: "pyrogram.Client",
-        chat_id: Union[int, str]
+        chat_id: Union[int, str],
+        user_id: int,
     ) -> bool:
-        """unhide a general forum topic.
+        """Decline a chat join request.
+
+        You must be an administrator in the chat for this to work and must have the *can_invite_users* administrator
+        right.
 
         .. include:: /_includes/usable-by/users-bots.rst
 
         Parameters:
             chat_id (``int`` | ``str``):
-                Unique identifier (int) or username (str) of the target chat.
+                Unique identifier for the target chat or username of the target channel/supergroup
+                (in the format @username).
 
-        Returns:
-            `bool`: On success, a True is returned.
-
-        Example:
-            .. code-block:: python
+            user_id (``int``):
+                Unique identifier of the target user.
 
-                await app.unhide_general_topic(chat_id)
+        Returns:
+            ``bool``: True on success.
         """
         await self.invoke(
-            raw.functions.channels.EditForumTopic(
-                channel=await self.resolve_peer(chat_id),
-                topic_id=1,
-                hidden=False
+            raw.functions.messages.HideChatJoinRequest(
+                peer=await self.resolve_peer(chat_id),
+                user_id=await self.resolve_peer(user_id),
+                approved=False
             )
         )
+
         return True
```

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/chats/unpin_all_chat_messages.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/chats/unpin_all_chat_messages.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/chats/unpin_chat_message.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/chats/unpin_chat_message.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/contacts/__init__.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/contacts/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/contacts/add_contact.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/contacts/add_contact.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/contacts/delete_contacts.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/contacts/delete_contacts.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/contacts/get_contacts.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/contacts/get_contacts.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/contacts/get_contacts_count.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/contacts/get_contacts_count.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/contacts/import_contacts.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/contacts/import_contacts.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/decorators/__init__.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/decorators/on_callback_query.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/decorators/on_callback_query.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/decorators/on_chat_join_request.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/decorators/on_chat_join_request.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/decorators/on_chat_member_updated.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/decorators/on_chat_member_updated.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/decorators/on_chosen_inline_result.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/decorators/on_chosen_inline_result.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/decorators/on_deleted_messages.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/decorators/on_deleted_messages.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/decorators/on_disconnect.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/decorators/on_disconnect.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/decorators/on_edited_message.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/decorators/on_edited_message.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/decorators/on_inline_query.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/decorators/on_inline_query.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/decorators/on_message.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/decorators/on_message.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/decorators/on_poll.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/decorators/on_poll.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/decorators/on_raw_update.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/decorators/on_raw_update.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/decorators/on_user_status.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/decorators/on_user_status.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/invite_links/__init__.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/invite_links/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/invite_links/approve_all_chat_join_requests.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/invite_links/approve_all_chat_join_requests.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/invite_links/approve_chat_join_request.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/invite_links/delete_chat_admin_invite_links.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,40 +18,37 @@
 
 from typing import Union
 
 import pyrogram
 from pyrogram import raw
 
 
-class ApproveChatJoinRequest:
-    async def approve_chat_join_request(
+class DeleteChatAdminInviteLinks:
+    async def delete_chat_admin_invite_links(
         self: "pyrogram.Client",
         chat_id: Union[int, str],
-        user_id: int,
+        admin_id: Union[int, str],
     ) -> bool:
-        """Approve a chat join request.
+        """Delete all revoked invite links of an administrator.
 
-        You must be an administrator in the chat for this to work and must have the *can_invite_users* administrator
-        right.
-
-        .. include:: /_includes/usable-by/users-bots.rst
+        .. include:: /_includes/usable-by/users.rst
 
         Parameters:
             chat_id (``int`` | ``str``):
                 Unique identifier for the target chat or username of the target channel/supergroup
                 (in the format @username).
 
-            user_id (``int``):
-                Unique identifier of the target user.
+            admin_id (``int`` | ``str``):
+                Unique identifier (int) or username (str) of the target user.
+                For you yourself you can simply use "me" or "self".
+                For a contact that exists in your Telegram address book you can use his phone number (str).
 
         Returns:
-            ``bool``: True on success.
+            ``bool``: On success ``True`` is returned.
         """
-        await self.invoke(
-            raw.functions.messages.HideChatJoinRequest(
+
+        return await self.invoke(
+            raw.functions.messages.DeleteRevokedExportedChatInvites(
                 peer=await self.resolve_peer(chat_id),
-                user_id=await self.resolve_peer(user_id),
-                approved=True
+                admin_id=await self.resolve_peer(admin_id),
             )
         )
-
-        return True
```

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/invite_links/create_chat_invite_link.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/invite_links/create_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/invite_links/decline_all_chat_join_requests.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/invite_links/decline_all_chat_join_requests.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/invite_links/decline_chat_join_request.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/invite_links/get_chat_invite_link_joiners_count.py`

 * *Files 15% similar despite different names*

```diff
@@ -18,40 +18,39 @@
 
 from typing import Union
 
 import pyrogram
 from pyrogram import raw
 
 
-class DeclineChatJoinRequest:
-    async def decline_chat_join_request(
+class GetChatInviteLinkJoinersCount:
+    async def get_chat_invite_link_joiners_count(
         self: "pyrogram.Client",
         chat_id: Union[int, str],
-        user_id: int,
-    ) -> bool:
-        """Decline a chat join request.
+        invite_link: str
+    ) -> int:
+        """Get the count of the members who joined the chat with the invite link.
 
-        You must be an administrator in the chat for this to work and must have the *can_invite_users* administrator
-        right.
-
-        .. include:: /_includes/usable-by/users-bots.rst
+        .. include:: /_includes/usable-by/users.rst
 
         Parameters:
             chat_id (``int`` | ``str``):
                 Unique identifier for the target chat or username of the target channel/supergroup
                 (in the format @username).
 
-            user_id (``int``):
-                Unique identifier of the target user.
+            invite_link (str):
+                The invite link.
 
         Returns:
-            ``bool``: True on success.
+            ``int``: On success, the joined chat members count is returned.
         """
-        await self.invoke(
-            raw.functions.messages.HideChatJoinRequest(
+        r = await self.invoke(
+            raw.functions.messages.GetChatInviteImporters(
                 peer=await self.resolve_peer(chat_id),
-                user_id=await self.resolve_peer(user_id),
-                approved=False
+                link=invite_link,
+                limit=1,
+                offset_date=0,
+                offset_user=raw.types.InputUserEmpty()
             )
         )
 
-        return True
+        return r.count
```

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/invite_links/delete_chat_admin_invite_links.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/invite_links/get_chat_admin_invite_links_count.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,37 +18,45 @@
 
 from typing import Union
 
 import pyrogram
 from pyrogram import raw
 
 
-class DeleteChatAdminInviteLinks:
-    async def delete_chat_admin_invite_links(
+class GetChatAdminInviteLinksCount:
+    async def get_chat_admin_invite_links_count(
         self: "pyrogram.Client",
         chat_id: Union[int, str],
         admin_id: Union[int, str],
-    ) -> bool:
-        """Delete all revoked invite links of an administrator.
+        revoked: bool = False,
+    ) -> int:
+        """Get the count of the invite links created by an administrator in a chat.
 
         .. include:: /_includes/usable-by/users.rst
 
         Parameters:
             chat_id (``int`` | ``str``):
                 Unique identifier for the target chat or username of the target channel/supergroup
                 (in the format @username).
 
             admin_id (``int`` | ``str``):
                 Unique identifier (int) or username (str) of the target user.
                 For you yourself you can simply use "me" or "self".
                 For a contact that exists in your Telegram address book you can use his phone number (str).
 
+            revoked (``bool``, *optional*):
+                True, if you want to get revoked links instead.
+                Defaults to False (get active links only).
+
         Returns:
-            ``bool``: On success ``True`` is returned.
+            ``int``: On success, the invite links count is returned.
         """
-
-        return await self.invoke(
-            raw.functions.messages.DeleteRevokedExportedChatInvites(
+        r = await self.invoke(
+            raw.functions.messages.GetExportedChatInvites(
                 peer=await self.resolve_peer(chat_id),
                 admin_id=await self.resolve_peer(admin_id),
+                limit=1,
+                revoked=revoked
             )
         )
+
+        return r.count
```

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/invite_links/delete_chat_invite_link.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/invite_links/delete_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/invite_links/edit_chat_invite_link.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/invite_links/edit_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/invite_links/export_chat_invite_link.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/invite_links/export_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/invite_links/get_chat_admin_invite_links.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/invite_links/get_chat_admin_invite_links.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/invite_links/get_chat_admin_invite_links_count.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/invite_links/get_chat_admins_with_invite_links.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,48 +15,42 @@
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
 from typing import Union
 
 import pyrogram
-from pyrogram import raw
+from pyrogram import raw, types
 
 
-class GetChatAdminInviteLinksCount:
-    async def get_chat_admin_invite_links_count(
+class GetChatAdminsWithInviteLinks:
+    async def get_chat_admins_with_invite_links(
         self: "pyrogram.Client",
         chat_id: Union[int, str],
-        admin_id: Union[int, str],
-        revoked: bool = False,
-    ) -> int:
-        """Get the count of the invite links created by an administrator in a chat.
+    ):
+        """Get the list of the administrators that have exported invite links in a chat.
+
+        You must be the owner of a chat for this to work.
 
         .. include:: /_includes/usable-by/users.rst
 
         Parameters:
             chat_id (``int`` | ``str``):
                 Unique identifier for the target chat or username of the target channel/supergroup
                 (in the format @username).
 
-            admin_id (``int`` | ``str``):
-                Unique identifier (int) or username (str) of the target user.
-                For you yourself you can simply use "me" or "self".
-                For a contact that exists in your Telegram address book you can use his phone number (str).
-
-            revoked (``bool``, *optional*):
-                True, if you want to get revoked links instead.
-                Defaults to False (get active links only).
-
         Returns:
-            ``int``: On success, the invite links count is returned.
+            List of :obj:`~pyrogram.types.ChatAdminWithInviteLink`: On success, the list of admins that have exported
+            invite links is returned.
         """
         r = await self.invoke(
-            raw.functions.messages.GetExportedChatInvites(
-                peer=await self.resolve_peer(chat_id),
-                admin_id=await self.resolve_peer(admin_id),
-                limit=1,
-                revoked=revoked
+            raw.functions.messages.GetAdminsWithInvites(
+                peer=await self.resolve_peer(chat_id)
             )
         )
 
-        return r.count
+        users = {i.id: i for i in r.users}
+
+        return types.List(
+            types.ChatAdminWithInviteLinks._parse(self, admin, users)
+            for admin in r.admins
+        )
```

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/invite_links/get_chat_admins_with_invite_links.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/chats/close_general_topic.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,46 +11,42 @@
 #  Pyrogram is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
-
-from typing import Union
-
 import pyrogram
-from pyrogram import raw, types
+from pyrogram import raw
+from pyrogram import types
+from typing import Union
 
 
-class GetChatAdminsWithInviteLinks:
-    async def get_chat_admins_with_invite_links(
+class CloseGeneralTopic:
+    async def close_general_topic(
         self: "pyrogram.Client",
-        chat_id: Union[int, str],
-    ):
-        """Get the list of the administrators that have exported invite links in a chat.
-
-        You must be the owner of a chat for this to work.
+        chat_id: Union[int, str]
+    ) -> bool:
+        """Close a forum topic.
 
-        .. include:: /_includes/usable-by/users.rst
+        .. include:: /_includes/usable-by/users-bots.rst
 
         Parameters:
             chat_id (``int`` | ``str``):
-                Unique identifier for the target chat or username of the target channel/supergroup
-                (in the format @username).
+                Unique identifier (int) or username (str) of the target chat.
 
         Returns:
-            List of :obj:`~pyrogram.types.ChatAdminWithInviteLink`: On success, the list of admins that have exported
-            invite links is returned.
-        """
-        r = await self.invoke(
-            raw.functions.messages.GetAdminsWithInvites(
-                peer=await self.resolve_peer(chat_id)
-            )
-        )
+            `bool`: On success, a True is returned.
 
-        users = {i.id: i for i in r.users}
+        Example:
+            .. code-block:: python
 
-        return types.List(
-            types.ChatAdminWithInviteLinks._parse(self, admin, users)
-            for admin in r.admins
+                await app.close_general_topic(chat_id)
+        """
+        await self.invoke(
+            raw.functions.channels.EditForumTopic(
+                channel=await self.resolve_peer(chat_id),
+                topic_id=1,
+                closed=True
+            )
         )
+        return True
```

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/invite_links/get_chat_invite_link.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/invite_links/get_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/invite_links/get_chat_invite_link_joiners.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/invite_links/get_chat_invite_link_joiners.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/invite_links/get_chat_invite_link_joiners_count.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/users/block_user.py`

 * *Files 16% similar despite different names*

```diff
@@ -18,39 +18,37 @@
 
 from typing import Union
 
 import pyrogram
 from pyrogram import raw
 
 
-class GetChatInviteLinkJoinersCount:
-    async def get_chat_invite_link_joiners_count(
+class BlockUser:
+    async def block_user(
         self: "pyrogram.Client",
-        chat_id: Union[int, str],
-        invite_link: str
-    ) -> int:
-        """Get the count of the members who joined the chat with the invite link.
+        user_id: Union[int, str]
+    ) -> bool:
+        """Block a user.
 
         .. include:: /_includes/usable-by/users.rst
 
         Parameters:
-            chat_id (``int`` | ``str``):
-                Unique identifier for the target chat or username of the target channel/supergroup
-                (in the format @username).
-
-            invite_link (str):
-                The invite link.
+            user_id (``int`` | ``str``)::
+                Unique identifier (int) or username (str) of the target user.
+                For you yourself you can simply use "me" or "self".
+                For a contact that exists in your Telegram address book you can use his phone number (str).
 
         Returns:
-            ``int``: On success, the joined chat members count is returned.
+            ``bool``: True on success
+
+        Example:
+            .. code-block:: python
+
+                await app.block_user(user_id)
         """
-        r = await self.invoke(
-            raw.functions.messages.GetChatInviteImporters(
-                peer=await self.resolve_peer(chat_id),
-                link=invite_link,
-                limit=1,
-                offset_date=0,
-                offset_user=raw.types.InputUserEmpty()
+        return bool(
+            await self.invoke(
+                raw.functions.contacts.Block(
+                    id=await self.resolve_peer(user_id)
+                )
             )
         )
-
-        return r.count
```

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/invite_links/get_chat_join_requests.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/invite_links/get_chat_join_requests.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/invite_links/revoke_chat_invite_link.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/invite_links/revoke_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/messages/__init__.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/messages/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/messages/copy_media_group.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/messages/copy_media_group.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/messages/copy_message.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/messages/copy_message.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/messages/delete_messages.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/messages/delete_messages.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/messages/download_media.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/messages/download_media.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/messages/edit_inline_caption.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/messages/edit_inline_caption.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/messages/edit_inline_media.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/messages/edit_inline_media.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/messages/edit_inline_reply_markup.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/messages/edit_inline_reply_markup.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/messages/edit_inline_text.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/messages/edit_inline_text.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/messages/edit_message_caption.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/messages/edit_message_caption.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/messages/edit_message_media.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/messages/edit_message_media.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/messages/edit_message_reply_markup.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/messages/edit_message_reply_markup.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/messages/edit_message_text.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/messages/edit_message_text.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/messages/forward_messages.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/messages/forward_messages.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/messages/get_chat_history.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/messages/get_chat_history.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/messages/get_chat_history_count.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/messages/get_chat_history_count.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/messages/get_custom_emoji_stickers.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/messages/get_custom_emoji_stickers.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/messages/get_discussion_message.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/messages/get_discussion_message.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/messages/get_discussion_replies.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/messages/get_discussion_replies.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/messages/get_discussion_replies_count.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/messages/get_discussion_replies_count.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/messages/get_media_group.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/messages/get_media_group.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/messages/get_messages.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/messages/get_messages.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/messages/inline_session.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/messages/inline_session.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/messages/read_chat_history.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/messages/read_chat_history.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/messages/retract_vote.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/messages/retract_vote.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/messages/search_global.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/messages/search_global.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/messages/search_global_count.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/messages/search_global_count.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/messages/search_messages.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/messages/search_messages.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/messages/search_messages_count.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/messages/search_messages_count.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/messages/send_animation.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/messages/send_animation.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/messages/send_audio.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/messages/send_audio.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/messages/send_cached_media.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/messages/send_cached_media.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/messages/send_chat_action.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/messages/send_chat_action.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/messages/send_contact.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/messages/send_contact.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/messages/send_dice.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/messages/send_dice.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/messages/send_document.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/messages/send_document.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/messages/send_location.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/messages/send_location.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/messages/send_media_group.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/messages/send_media_group.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/messages/send_message.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/messages/send_message.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/messages/send_photo.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/messages/send_photo.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/messages/send_poll.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/messages/send_poll.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/messages/send_reaction.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/messages/send_reaction.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/messages/send_sticker.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/messages/send_sticker.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/messages/send_venue.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/messages/send_venue.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/messages/send_video.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/messages/send_video.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/messages/send_video_note.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/messages/send_video_note.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/messages/send_voice.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/messages/send_voice.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/messages/stop_poll.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/messages/stop_poll.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/messages/stream_media.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/messages/stream_media.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/messages/vote_poll.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/messages/vote_poll.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/password/__init__.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/password/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/password/change_cloud_password.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/password/change_cloud_password.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/password/enable_cloud_password.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/password/enable_cloud_password.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/password/remove_cloud_password.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/password/remove_cloud_password.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/stickers/__init__.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/stickers/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/stickers/add_sticker_to_set.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/stickers/add_sticker_to_set.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/stickers/create_sticker_set.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/stickers/create_sticker_set.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/stickers/get_sticker_set.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/stickers/get_sticker_set.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/users/__init__.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/users/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,39 +14,35 @@
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
 from .block_user import BlockUser
 from .delete_profile_photos import DeleteProfilePhotos
-from .get_bot_info import GetBotInfo
 from .get_chat_photos import GetChatPhotos
 from .get_chat_photos_count import GetChatPhotosCount
 from .get_common_chats import GetCommonChats
 from .get_default_emoji_statuses import GetDefaultEmojiStatuses
 from .get_me import GetMe
 from .get_users import GetUsers
-from .set_bot_info import SetBotInfo
 from .set_emoji_status import SetEmojiStatus
 from .set_profile_photo import SetProfilePhoto
 from .set_username import SetUsername
 from .unblock_user import UnblockUser
 from .update_profile import UpdateProfile
 
 
 class Users(
     BlockUser,
-    GetBotInfo,
     GetCommonChats,
     GetChatPhotos,
     SetProfilePhoto,
     DeleteProfilePhotos,
     GetUsers,
     GetMe,
-    SetBotInfo,
     SetUsername,
     GetChatPhotosCount,
     UnblockUser,
     UpdateProfile,
     GetDefaultEmojiStatuses,
     SetEmojiStatus
 ):
```

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/users/block_user.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/users/unblock_user.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,20 +18,20 @@
 
 from typing import Union
 
 import pyrogram
 from pyrogram import raw
 
 
-class BlockUser:
-    async def block_user(
+class UnblockUser:
+    async def unblock_user(
         self: "pyrogram.Client",
         user_id: Union[int, str]
     ) -> bool:
-        """Block a user.
+        """Unblock a user.
 
         .. include:: /_includes/usable-by/users.rst
 
         Parameters:
             user_id (``int`` | ``str``)::
                 Unique identifier (int) or username (str) of the target user.
                 For you yourself you can simply use "me" or "self".
@@ -39,16 +39,16 @@
 
         Returns:
             ``bool``: True on success
 
         Example:
             .. code-block:: python
 
-                await app.block_user(user_id)
+                await app.unblock_user(user_id)
         """
         return bool(
             await self.invoke(
-                raw.functions.contacts.Block(
+                raw.functions.contacts.Unblock(
                     id=await self.resolve_peer(user_id)
                 )
             )
         )
```

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/users/delete_profile_photos.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/users/delete_profile_photos.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/users/get_bot_info.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/users/set_username.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,48 +1,57 @@
-#  Pyrofork - Telegram MTProto API Client Library for Python
-#  Copyright (C) 2022-present Mayuri-Chan <https://github.com/Mayuri-Chan>
+#  Pyrogram - Telegram MTProto API Client Library for Python
+#  Copyright (C) 2017-present Dan <https://github.com/delivrance>
 #
-#  This file is part of Pyrofork.
+#  This file is part of Pyrogram.
 #
-#  Pyrofork is free software: you can redistribute it and/or modify
+#  Pyrogram is free software: you can redistribute it and/or modify
 #  it under the terms of the GNU Lesser General Public License as published
 #  by the Free Software Foundation, either version 3 of the License, or
 #  (at your option) any later version.
 #
-#  Pyrofork is distributed in the hope that it will be useful,
+#  Pyrogram is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
-#  along with Pyrofork.  If not, see <http://www.gnu.org/licenses/>.
+#  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
-from typing import Union
+from typing import Optional
 
 import pyrogram
 from pyrogram import raw
 
 
-class GetBotInfo:
-    async def get_bot_info(
+class SetUsername:
+    async def set_username(
         self: "pyrogram.Client",
-        lang_code: str,
-        bot: Union[int, str] = None
-    ) -> pyrogram.types.BotInfo:
-        """Get the bot info in given language.
+        username: Optional[str]
+    ) -> bool:
+        """Set your own username.
+
+        This method only works for users, not bots. Bot usernames must be changed via Bot Support or by recreating
+        them from scratch using BotFather. To set a channel or supergroup username you can use
+        :meth:`~pyrogram.Client.set_chat_username`.
 
-        .. include:: /_includes/usable-by/users-bots.rst
-
-        Note:
-            For userbot you can only use this method if you are the owner of target bot.
+        .. include:: /_includes/usable-by/users.rst
 
         Parameters:
-            lang_code ``str``:
-                A two-letter ISO 639-1 language code.
-            bot (``int`` | ``str``, *optional*):
-                Unique identifier (int) or username (str) of the target bot.
+            username (``str`` | ``None``):
+                Username to set. "" (empty string) or None to remove it.
+
+        Returns:
+            ``bool``: True on success.
+
+        Example:
+            .. code-block:: python
+
+                await app.set_username("new_username")
         """
-        peer = None
-        if bot:
-            peer = await self.resolve_peer(bot)
-        r = await self.invoke(raw.functions.bots.GetBotInfo(language_code=lang_code, bot=peer))
-        return r
+
+        return bool(
+            await self.invoke(
+                raw.functions.account.UpdateUsername(
+                    username=username or ""
+                )
+            )
+        )
```

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/users/get_chat_photos.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/users/get_chat_photos.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/users/get_chat_photos_count.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/users/get_chat_photos_count.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/users/get_common_chats.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/users/get_common_chats.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/users/get_default_emoji_statuses.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/users/get_default_emoji_statuses.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/users/get_me.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/users/get_me.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/users/get_users.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/users/get_users.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/users/set_bot_info.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/input_media/input_media_document.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,60 +1,65 @@
-#  Pyrofork - Telegram MTProto API Client Library for Python
-#  Copyright (C) 2022-present Mayuri-Chan <https://github.com/Mayuri-Chan>
+#  Pyrogram - Telegram MTProto API Client Library for Python
+#  Copyright (C) 2017-present Dan <https://github.com/delivrance>
 #
-#  This file is part of Pyrofork.
+#  This file is part of Pyrogram.
 #
-#  Pyrofork is free software: you can redistribute it and/or modify
+#  Pyrogram is free software: you can redistribute it and/or modify
 #  it under the terms of the GNU Lesser General Public License as published
 #  by the Free Software Foundation, either version 3 of the License, or
 #  (at your option) any later version.
 #
-#  Pyrofork is distributed in the hope that it will be useful,
+#  Pyrogram is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
-#  along with Pyrofork.  If not, see <http://www.gnu.org/licenses/>.
+#  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
-from typing import Union
+from typing import Optional, List, Union, BinaryIO
 
-import pyrogram
-from pyrogram import raw
+from .input_media import InputMedia
+from ..messages_and_media import MessageEntity
+from ... import enums
+
+
+class InputMediaDocument(InputMedia):
+    """A generic file to be sent inside an album.
+
+    Parameters:
+        media (``str`` | ``BinaryIO``):
+            File to send.
+            Pass a file_id as string to send a file that exists on the Telegram servers or
+            pass a file path as string to upload a new file that exists on your local machine or
+            pass a binary file-like object with its attribute “.name” set for in-memory uploads or
+            pass an HTTP URL as a string for Telegram to get a file from the Internet.
+
+        thumb (``str``):
+            Thumbnail of the file sent.
+            The thumbnail should be in JPEG format and less than 200 KB in size.
+            A thumbnail's width and height should not exceed 320 pixels.
+            Thumbnails can't be reused and can be only uploaded as a new file.
+
+        caption (``str``, *optional*):
+            Caption of the document to be sent, 0-1024 characters.
+            If not specified, the original caption is kept. Pass "" (empty string) to remove the caption.
+
+        parse_mode (:obj:`~pyrogram.enums.ParseMode`, *optional*):
+            By default, texts are parsed using both Markdown and HTML styles.
+            You can combine both syntaxes together.
+
+        caption_entities (List of :obj:`~pyrogram.types.MessageEntity`):
+            List of special entities that appear in the caption, which can be specified instead of *parse_mode*.
+    """
+
+    def __init__(
+        self,
+        media: Union[str, BinaryIO],
+        thumb: str = None,
+        caption: str = "",
+        parse_mode: Optional["enums.ParseMode"] = None,
+        caption_entities: List[MessageEntity] = None
+    ):
+        super().__init__(media, caption, parse_mode, caption_entities)
 
-
-class SetBotInfo:
-    async def set_bot_info(
-        self: "pyrogram.Client",
-        lang_code: str,
-        bot: Union[int, str] = None,
-        name: str = None,
-        about: str = None,
-        description: str = None
-    ) -> bool:
-        """Get the bot info in given language.
-
-        .. include:: /_includes/usable-by/users-bots.rst
-
-        Note:
-            For userbot you can only use this method if you are the owner of target bot.
-
-        Parameters:
-            lang_code ``str``:
-                A two-letter ISO 639-1 language code.
-            bot (``int`` | ``str``, *optional*) :
-                Unique identifier (int) or username (str) of the target bot.
-
-            name (``str``, *optional*):
-                The bot name.
-            
-            about (``str``, *optional*):
-                The bot bio.
-
-            description (``str``, *optional*):
-                Description of the bot;
-        """
-        peer = None
-        if bot:
-            peer = await self.resolve_peer(bot)
-        r = await self.invoke(raw.functions.bots.SetBotInfo(language_code=lang_code, bot=peer, name=name, about=about, description=description))
-        return bool(r)
+        self.thumb = thumb
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/users/set_emoji_status.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/users/set_emoji_status.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/users/set_profile_photo.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/users/set_profile_photo.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/users/set_username.py` & `PyroFork-dev-2.2.5.dev202307219555/tests/filters/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -12,46 +12,25 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
-from typing import Optional
+class Client:
+    def __init__(self):
+        self.me = User("username")
 
-import pyrogram
-from pyrogram import raw
+    async def get_me(self):
+        return self.me
 
 
-class SetUsername:
-    async def set_username(
-        self: "pyrogram.Client",
-        username: Optional[str]
-    ) -> bool:
-        """Set your own username.
+class User:
+    def __init__(self, username: str = None):
+        self.username = username
 
-        This method only works for users, not bots. Bot usernames must be changed via Bot Support or by recreating
-        them from scratch using BotFather. To set a channel or supergroup username you can use
-        :meth:`~pyrogram.Client.set_chat_username`.
 
-        .. include:: /_includes/usable-by/users.rst
-
-        Parameters:
-            username (``str`` | ``None``):
-                Username to set. "" (empty string) or None to remove it.
-
-        Returns:
-            ``bool``: True on success.
-
-        Example:
-            .. code-block:: python
-
-                await app.set_username("new_username")
-        """
-
-        return bool(
-            await self.invoke(
-                raw.functions.account.UpdateUsername(
-                    username=username or ""
-                )
-            )
-        )
+class Message:
+    def __init__(self, text: str = None, caption: str = None):
+        self.text = text
+        self.caption = caption
+        self.command = None
```

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/users/unblock_user.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/bots_and_keyboards/menu_button_web_app.py`

 * *Files 20% similar despite different names*

```diff
@@ -12,43 +12,40 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
-from typing import Union
-
 import pyrogram
-from pyrogram import raw
+from pyrogram import raw, types
+from .menu_button import MenuButton
+
 
+class MenuButtonWebApp(MenuButton):
+    """A menu button, which launches a `Web App <https://core.telegram.org/bots/webapps>`_.
 
-class UnblockUser:
-    async def unblock_user(
-        self: "pyrogram.Client",
-        user_id: Union[int, str]
-    ) -> bool:
-        """Unblock a user.
-
-        .. include:: /_includes/usable-by/users.rst
-
-        Parameters:
-            user_id (``int`` | ``str``)::
-                Unique identifier (int) or username (str) of the target user.
-                For you yourself you can simply use "me" or "self".
-                For a contact that exists in your Telegram address book you can use his phone number (str).
-
-        Returns:
-            ``bool``: True on success
-
-        Example:
-            .. code-block:: python
-
-                await app.unblock_user(user_id)
-        """
-        return bool(
-            await self.invoke(
-                raw.functions.contacts.Unblock(
-                    id=await self.resolve_peer(user_id)
-                )
-            )
+    Parameters:
+        text (``str``):
+            Text on the button
+
+        web_app (:obj:`~pyrogram.types.WebAppInfo`):
+            Description of the Web App that will be launched when the user presses the button.
+            The Web App will be able to send an arbitrary message on behalf of the user using the method
+            :meth:`~pyrogram.Client.answer_web_app_query`.
+    """
+
+    def __init__(
+        self,
+        text: str,
+        web_app: "types.WebAppInfo"
+    ):
+        super().__init__("web_app")
+
+        self.text = text
+        self.web_app = web_app
+
+    async def write(self, client: "pyrogram.Client") -> "raw.types.BotMenuButton":
+        return raw.types.BotMenuButton(
+            text=self.text,
+            url=self.web_app.url
         )
```

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/users/update_profile.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/users/update_profile.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/utilities/__init__.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/utilities/add_handler.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/utilities/add_handler.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/utilities/compose.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/utilities/compose.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/utilities/export_session_string.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/utilities/export_session_string.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/utilities/idle.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/utilities/idle.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/utilities/remove_handler.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/utilities/remove_handler.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/utilities/restart.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/utilities/restart.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/utilities/run.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/utilities/run.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/utilities/run_sync.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/utilities/run_sync.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/utilities/start.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/utilities/start.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/utilities/stop.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/utilities/stop.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/methods/utilities/stop_transmission.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/utilities/stop_transmission.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/mime_types.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/mime_types.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/parser/__init__.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/parser/html.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/parser/html.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/parser/markdown.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/parser/markdown.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/parser/parser.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/parser/parser.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/parser/utils.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/parser/utils.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/raw/__init__.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/raw/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/raw/core/__init__.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/raw/core/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/raw/core/future_salt.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/raw/core/future_salt.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/raw/core/future_salts.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/raw/core/future_salts.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/raw/core/gzip_packed.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/raw/core/gzip_packed.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/raw/core/list.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/raw/core/list.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/raw/core/message.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/raw/core/message.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/raw/core/msg_container.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/raw/core/msg_container.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/raw/core/primitives/__init__.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/raw/core/primitives/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/raw/core/primitives/bool.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/raw/core/primitives/bool.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/raw/core/primitives/bytes.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/raw/core/primitives/bytes.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/raw/core/primitives/double.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/raw/core/primitives/double.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/raw/core/primitives/int.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/raw/core/primitives/int.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/raw/core/primitives/string.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/raw/core/primitives/string.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/raw/core/primitives/vector.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/raw/core/primitives/vector.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/raw/core/tl_object.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/raw/core/tl_object.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/session/__init__.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/session/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/session/auth.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/session/auth.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/session/internals/__init__.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/session/internals/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/session/internals/data_center.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/session/internals/data_center.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/session/internals/msg_factory.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/session/internals/msg_factory.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/session/internals/msg_id.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/session/internals/msg_id.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/session/internals/seq_no.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/session/internals/seq_no.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/session/session.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/session/session.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/storage/__init__.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/storage/dummy_client.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/input_media/input_media_photo.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,62 +1,63 @@
-#  Pyrofork - Telegram MTProto API Client Library for Python
-#  Copyright (C) 2022-present Mayuri-Chan <https://github.com/Mayuri-Chan>
+#  Pyrogram - Telegram MTProto API Client Library for Python
+#  Copyright (C) 2017-present Dan <https://github.com/delivrance>
 #
-#  This file is part of Pyrofork.
+#  This file is part of Pyrogram.
 #
-#  Pyrofork is free software: you can redistribute it and/or modify
+#  Pyrogram is free software: you can redistribute it and/or modify
 #  it under the terms of the GNU Lesser General Public License as published
 #  by the Free Software Foundation, either version 3 of the License, or
 #  (at your option) any later version.
 #
-#  Pyrofork is distributed in the hope that it will be useful,
+#  Pyrogram is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
-#  along with Pyrofork.  If not, see <http://www.gnu.org/licenses/>.
+#  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
-from pymongo.client_session import TransactionOptions
-from bson.codec_options import CodecOptions
-from pymongo.read_concern import ReadConcern
-from pymongo.read_preferences import (
-    Nearest,
-    Primary,
-    PrimaryPreferred,
-    Secondary,
-    SecondaryPreferred,
-)
-from pymongo.write_concern import WriteConcern
-from typing import Any, Optional, Union
-
-try:
-    from typing import Protocol, runtime_checkable
-except ImportError:
-    from typing_extensions import Protocol, runtime_checkable
-
-ReadPreferences = Union[Primary, PrimaryPreferred, Secondary, SecondaryPreferred, Nearest]
-
-@runtime_checkable
-class DummyMongoClient(Protocol):
-    def __init__(self, *args: Any, **kwargs: Any) -> None:
-        raise NotImplementedError
+from typing import Optional, List, Union, BinaryIO
 
-    def get_database(
-        self,
-        name: Optional[str] = None,
-        *,
-        codec_options: Optional[CodecOptions] = None,
-        read_preference: Optional[ReadPreferences] = None,
-        write_concern: Optional[WriteConcern] = None,
-        read_concern: Optional[ReadConcern] = None,
-    ):
-        raise NotImplementedError
-    
-    async def start_session(
+from .input_media import InputMedia
+from ..messages_and_media import MessageEntity
+from ... import enums
+
+
+class InputMediaPhoto(InputMedia):
+    """A photo to be sent inside an album.
+    It is intended to be used with :obj:`~pyrogram.Client.send_media_group`.
+
+    Parameters:
+        media (``str`` | ``BinaryIO``):
+            Photo to send.
+            Pass a file_id as string to send a photo that exists on the Telegram servers or
+            pass a file path as string to upload a new photo that exists on your local machine or
+            pass a binary file-like object with its attribute “.name” set for in-memory uploads or
+            pass an HTTP URL as a string for Telegram to get a photo from the Internet.
+
+        caption (``str``, *optional*):
+            Caption of the photo to be sent, 0-1024 characters.
+            If not specified, the original caption is kept. Pass "" (empty string) to remove the caption.
+
+        parse_mode (:obj:`~pyrogram.enums.ParseMode`, *optional*):
+            By default, texts are parsed using both Markdown and HTML styles.
+            You can combine both syntaxes together.
+
+        caption_entities (List of :obj:`~pyrogram.types.MessageEntity`):
+            List of special entities that appear in the caption, which can be specified instead of *parse_mode*.
+
+        has_spoiler (``bool``, *optional*):
+            Pass True if the photo needs to be covered with a spoiler animation.
+    """
+
+    def __init__(
         self,
-        *,
-        causal_consistency: Optional[bool] = None,
-        default_transaction_options: Optional[TransactionOptions] = None,
-        snapshot: bool = False,
+        media: Union[str, BinaryIO],
+        caption: str = "",
+        parse_mode: Optional["enums.ParseMode"] = None,
+        caption_entities: List[MessageEntity] = None,
+        has_spoiler: bool = None
     ):
-        raise NotImplementedError
+        super().__init__(media, caption, parse_mode, caption_entities)
+
+        self.has_spoiler = has_spoiler
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/storage/file_storage.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/storage/file_storage.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/storage/memory_storage.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/storage/memory_storage.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/storage/mongo_storage.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/storage/mongo_storage.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,7 @@
-#  Pyrofork - Telegram MTProto API Client Library for Python
-#  Copyright (C) 2022-present Mayuri-Chan <https://github.com/Mayuri-Chan>
-#
-#  This file is part of Pyrofork.
-#
-#  Pyrofork is free software: you can redistribute it and/or modify
-#  it under the terms of the GNU Lesser General Public License as published
-#  by the Free Software Foundation, either version 3 of the License, or
-#  (at your option) any later version.
-#
-#  Pyrofork is distributed in the hope that it will be useful,
-#  but WITHOUT ANY WARRANTY; without even the implied warranty of
-#  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#  GNU Lesser General Public License for more details.
-#
-#  You should have received a copy of the GNU Lesser General Public License
-#  along with Pyrofork.  If not, see <http://www.gnu.org/licenses/>.
-
 import asyncio
 import inspect
 import time
 from typing import List, Tuple, Any
 
 from .dummy_client import DummyMongoClient
 from pymongo import MongoClient, UpdateOne
```

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/storage/sqlite/__init__.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/input_message_content/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,24 @@
-#  Pyrofork - Telegram MTProto API Client Library for Python
-#  Copyright (C) 2022-present Mayuri-Chan <https://github.com/Mayuri-Chan>
+#  Pyrogram - Telegram MTProto API Client Library for Python
+#  Copyright (C) 2017-present Dan <https://github.com/delivrance>
 #
-#  This file is part of Pyrofork.
+#  This file is part of Pyrogram.
 #
-#  Pyrofork is free software: you can redistribute it and/or modify
+#  Pyrogram is free software: you can redistribute it and/or modify
 #  it under the terms of the GNU Lesser General Public License as published
 #  by the Free Software Foundation, either version 3 of the License, or
 #  (at your option) any later version.
 #
-#  Pyrofork is distributed in the hope that it will be useful,
+#  Pyrogram is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
-#  along with Pyrofork.  If not, see <http://www.gnu.org/licenses/>.
+#  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
-from .cursor import AsyncCursor
-from .sqlite import AsyncSqlite
+from .input_message_content import InputMessageContent
+from .input_text_message_content import InputTextMessageContent
 
-__all__ = [AsyncSqlite, AsyncCursor]
+__all__ = [
+    "InputMessageContent", "InputTextMessageContent"
+]
```

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/storage/sqlite/cursor.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/list.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,30 @@
-#  Pyrofork - Telegram MTProto API Client Library for Python
-#  Copyright (C) 2022-present Mayuri-Chan <https://github.com/Mayuri-Chan>
+#  Pyrogram - Telegram MTProto API Client Library for Python
+#  Copyright (C) 2017-present Dan <https://github.com/delivrance>
 #
-#  This file is part of Pyrofork.
+#  This file is part of Pyrogram.
 #
-#  Pyrofork is free software: you can redistribute it and/or modify
+#  Pyrogram is free software: you can redistribute it and/or modify
 #  it under the terms of the GNU Lesser General Public License as published
 #  by the Free Software Foundation, either version 3 of the License, or
 #  (at your option) any later version.
 #
-#  Pyrofork is distributed in the hope that it will be useful,
+#  Pyrogram is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
-#  along with Pyrofork.  If not, see <http://www.gnu.org/licenses/>.
+#  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
-from pyrogram.utils import run_sync
-from sqlite3 import Cursor
-from threading import Thread
+from .object import Object
 
-class AsyncCursor(Thread):
-    def __init__(self, cursor: Cursor):
-        super().__init__()
-        self.cursor = cursor
 
-    async def fetchone(self):
-        return await run_sync(self.cursor.fetchone)
+class List(list):
+    __slots__ = []
+
+    def __str__(self):
+        # noinspection PyCallByClass
+        return Object.__str__(self)
+
+    def __repr__(self):
+        return f"pyrogram.types.List([{','.join(Object.__repr__(i) for i in self)}])"
```

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/storage/sqlite_storage.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/storage/sqlite_storage.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/storage/storage.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/storage/storage.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/sync.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/sync.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/__init__.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/authorization/__init__.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/authorization/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/authorization/sent_code.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/authorization/sent_code.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/authorization/terms_of_service.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/authorization/terms_of_service.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/bots_and_keyboards/__init__.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/bots_and_keyboards/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 from .bot_command_scope_all_chat_administrators import BotCommandScopeAllChatAdministrators
 from .bot_command_scope_all_group_chats import BotCommandScopeAllGroupChats
 from .bot_command_scope_all_private_chats import BotCommandScopeAllPrivateChats
 from .bot_command_scope_chat import BotCommandScopeChat
 from .bot_command_scope_chat_administrators import BotCommandScopeChatAdministrators
 from .bot_command_scope_chat_member import BotCommandScopeChatMember
 from .bot_command_scope_default import BotCommandScopeDefault
-from .bot_info import BotInfo
 from .callback_game import CallbackGame
 from .callback_query import CallbackQuery
 from .force_reply import ForceReply
 from .game_high_score import GameHighScore
 from .inline_keyboard_button import InlineKeyboardButton
 from .inline_keyboard_markup import InlineKeyboardMarkup
 from .keyboard_button import KeyboardButton
@@ -59,15 +58,14 @@
     "BotCommandScopeAllChatAdministrators",
     "BotCommandScopeAllGroupChats",
     "BotCommandScopeAllPrivateChats",
     "BotCommandScopeChat",
     "BotCommandScopeChatAdministrators",
     "BotCommandScopeChatMember",
     "BotCommandScopeDefault",
-    "BotInfo",
     "WebAppInfo",
     "MenuButton",
     "MenuButtonCommands",
     "MenuButtonWebApp",
     "MenuButtonDefault",
     "SentWebAppMessage"
 ]
```

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/bots_and_keyboards/bot_command.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/bots_and_keyboards/bot_command.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/bots_and_keyboards/bot_command_scope.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/bots_and_keyboards/bot_command_scope.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/bots_and_keyboards/bot_command_scope_all_chat_administrators.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/bots_and_keyboards/bot_command_scope_all_chat_administrators.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/bots_and_keyboards/bot_command_scope_all_group_chats.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/bots_and_keyboards/bot_command_scope_all_group_chats.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/bots_and_keyboards/bot_command_scope_all_private_chats.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/bots_and_keyboards/bot_command_scope_all_private_chats.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/bots_and_keyboards/bot_command_scope_chat.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/bots_and_keyboards/bot_command_scope_chat.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_administrators.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_administrators.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_member.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_member.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/bots_and_keyboards/bot_command_scope_default.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/bots_and_keyboards/bot_command_scope_default.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/bots_and_keyboards/bot_info.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/bots_and_keyboards/web_app_info.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,52 +1,37 @@
-#  Pyrofork - Telegram MTProto API Client Library for Python
-#  Copyright (C) 2022-present Mayuri-Chan <https://github.com/Mayuri-Chan>
+#  Pyrogram - Telegram MTProto API Client Library for Python
+#  Copyright (C) 2017-present Dan <https://github.com/delivrance>
 #
-#  This file is part of Pyrofork.
+#  This file is part of Pyrogram.
 #
-#  Pyrofork is free software: you can redistribute it and/or modify
+#  Pyrogram is free software: you can redistribute it and/or modify
 #  it under the terms of the GNU Lesser General Public License as published
 #  by the Free Software Foundation, either version 3 of the License, or
 #  (at your option) any later version.
 #
-#  Pyrofork is distributed in the hope that it will be useful,
+#  Pyrogram is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
-#  along with Pyrofork.  If not, see <http://www.gnu.org/licenses/>.
-
-from pyrogram import raw
+#  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
 from ..object import Object
 
 
-class BotInfo(Object):
-    """A bot Information.
+class WebAppInfo(Object):
+    """Contains information about a `Web App <https://core.telegram.org/bots/webapps>`_.
 
     Parameters:
-        name (``str``):
-            The bot name.
-        
-        about (``str``):
-            The bot bio.
-
-        description (``str``):
-            Description of the bot;
+        url (``str``):
+            An HTTPS URL of a Web App to be opened with additional data as specified in
+            `Initializing Web Apps <https://core.telegram.org/bots/webapps#initializing-web-apps>`_.
     """
 
-    def __init__(self, name: str, about: str, description: str):
+    def __init__(
+        self, *,
+        url: str,
+    ):
         super().__init__()
 
-        self.name = name
-        self.about = about
-        self.description = description
-
-    
-    @staticmethod
-    def _parse(bot_info: "raw.types.bots.BotInfo") -> "BotInfo":
-        return BotInfo(
-            name=getattr(bot_info,"name", None),
-            about=getattr(bot_info,"about", None),
-            description=getattr(bot_info,"description", None)
-        )
+        self.url = url
```

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/bots_and_keyboards/callback_game.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/bots_and_keyboards/callback_game.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/bots_and_keyboards/callback_query.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/bots_and_keyboards/callback_query.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/bots_and_keyboards/force_reply.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/bots_and_keyboards/force_reply.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/bots_and_keyboards/game_high_score.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/bots_and_keyboards/game_high_score.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/bots_and_keyboards/inline_keyboard_button.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/bots_and_keyboards/inline_keyboard_button.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/bots_and_keyboards/inline_keyboard_markup.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/bots_and_keyboards/inline_keyboard_markup.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/bots_and_keyboards/keyboard_button.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/bots_and_keyboards/keyboard_button.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/bots_and_keyboards/login_url.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/bots_and_keyboards/login_url.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/bots_and_keyboards/menu_button.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/bots_and_keyboards/menu_button.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/bots_and_keyboards/menu_button_commands.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/bots_and_keyboards/menu_button_commands.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/bots_and_keyboards/menu_button_default.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/bots_and_keyboards/menu_button_default.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/bots_and_keyboards/menu_button_web_app.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/messages_and_media/dice.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,39 +13,35 @@
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
 import pyrogram
-from pyrogram import raw, types
-from .menu_button import MenuButton
+from pyrogram import raw
+from ..object import Object
 
 
-class MenuButtonWebApp(MenuButton):
-    """A menu button, which launches a `Web App <https://core.telegram.org/bots/webapps>`_.
+class Dice(Object):
+    """A dice with a random value from 1 to 6 for currently supported base emoji.
 
     Parameters:
-        text (``str``):
-            Text on the button
+        emoji (``string``):
+            Emoji on which the dice throw animation is based.
 
-        web_app (:obj:`~pyrogram.types.WebAppInfo`):
-            Description of the Web App that will be launched when the user presses the button.
-            The Web App will be able to send an arbitrary message on behalf of the user using the method
-            :meth:`~pyrogram.Client.answer_web_app_query`.
+        value (``int``):
+            Value of the dice, 1-6 for currently supported base emoji.
     """
 
-    def __init__(
-        self,
-        text: str,
-        web_app: "types.WebAppInfo"
-    ):
-        super().__init__("web_app")
-
-        self.text = text
-        self.web_app = web_app
-
-    async def write(self, client: "pyrogram.Client") -> "raw.types.BotMenuButton":
-        return raw.types.BotMenuButton(
-            text=self.text,
-            url=self.web_app.url
+    def __init__(self, *, client: "pyrogram.Client" = None, emoji: str, value: int):
+        super().__init__(client)
+
+        self.emoji = emoji
+        self.value = value
+
+    @staticmethod
+    def _parse(client, dice: "raw.types.MessageMediaDice") -> "Dice":
+        return Dice(
+            emoji=dice.emoticon,
+            value=dice.value,
+            client=client
         )
```

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/bots_and_keyboards/reply_keyboard_markup.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/bots_and_keyboards/reply_keyboard_markup.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/bots_and_keyboards/reply_keyboard_remove.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/bots_and_keyboards/reply_keyboard_remove.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/bots_and_keyboards/sent_web_app_message.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/bots_and_keyboards/sent_web_app_message.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/bots_and_keyboards/web_app_info.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/user_and_chats/forum_topic_closed.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,23 +15,15 @@
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
 from ..object import Object
 
 
-class WebAppInfo(Object):
-    """Contains information about a `Web App <https://core.telegram.org/bots/webapps>`_.
+class ForumTopicClosed(Object):
+    """A service message about a forum topic closed in the chat.
 
-    Parameters:
-        url (``str``):
-            An HTTPS URL of a Web App to be opened with additional data as specified in
-            `Initializing Web Apps <https://core.telegram.org/bots/webapps#initializing-web-apps>`_.
+    Currently holds no information.
     """
 
-    def __init__(
-        self, *,
-        url: str,
-    ):
+    def __init__(self):
         super().__init__()
-
-        self.url = url
```

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/inline_mode/__init__.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/inline_mode/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/inline_mode/chosen_inline_result.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/inline_mode/chosen_inline_result.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/inline_mode/inline_query.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/inline_mode/inline_query.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/inline_mode/inline_query_result.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/inline_mode/inline_query_result.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/inline_mode/inline_query_result_animation.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/inline_mode/inline_query_result_animation.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/inline_mode/inline_query_result_article.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/inline_mode/inline_query_result_article.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/inline_mode/inline_query_result_audio.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/inline_mode/inline_query_result_audio.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/inline_mode/inline_query_result_cached_animation.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/inline_mode/inline_query_result_cached_animation.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/inline_mode/inline_query_result_cached_audio.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/inline_mode/inline_query_result_cached_audio.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/inline_mode/inline_query_result_cached_document.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/inline_mode/inline_query_result_cached_document.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/inline_mode/inline_query_result_cached_photo.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/inline_mode/inline_query_result_cached_photo.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/inline_mode/inline_query_result_cached_sticker.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/inline_mode/inline_query_result_cached_sticker.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/inline_mode/inline_query_result_cached_video.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/inline_mode/inline_query_result_cached_video.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/inline_mode/inline_query_result_cached_voice.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/inline_mode/inline_query_result_cached_voice.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/inline_mode/inline_query_result_contact.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/inline_mode/inline_query_result_contact.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/inline_mode/inline_query_result_document.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/inline_mode/inline_query_result_document.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/inline_mode/inline_query_result_location.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/inline_mode/inline_query_result_location.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/inline_mode/inline_query_result_photo.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/inline_mode/inline_query_result_photo.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/inline_mode/inline_query_result_venue.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/inline_mode/inline_query_result_venue.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/inline_mode/inline_query_result_video.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/inline_mode/inline_query_result_video.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/inline_mode/inline_query_result_voice.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/inline_mode/inline_query_result_voice.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/input_media/__init__.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/input_media/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/input_media/input_media.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/input_media/input_media.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/input_media/input_media_animation.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/input_media/input_media_animation.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/input_media/input_media_audio.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/input_media/input_media_audio.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/input_media/input_media_document.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/input_media/input_media_video.py`

 * *Files 18% similar despite different names*

```diff
@@ -19,47 +19,73 @@
 from typing import Optional, List, Union, BinaryIO
 
 from .input_media import InputMedia
 from ..messages_and_media import MessageEntity
 from ... import enums
 
 
-class InputMediaDocument(InputMedia):
-    """A generic file to be sent inside an album.
+class InputMediaVideo(InputMedia):
+    """A video to be sent inside an album.
+    It is intended to be used with :obj:`~pyrogram.Client.send_media_group`.
 
     Parameters:
         media (``str`` | ``BinaryIO``):
-            File to send.
-            Pass a file_id as string to send a file that exists on the Telegram servers or
-            pass a file path as string to upload a new file that exists on your local machine or
+            Video to send.
+            Pass a file_id as string to send a video that exists on the Telegram servers or
+            pass a file path as string to upload a new video that exists on your local machine or
             pass a binary file-like object with its attribute “.name” set for in-memory uploads or
-            pass an HTTP URL as a string for Telegram to get a file from the Internet.
+            pass an HTTP URL as a string for Telegram to get a video from the Internet.
 
         thumb (``str``):
-            Thumbnail of the file sent.
+            Thumbnail of the video sent.
             The thumbnail should be in JPEG format and less than 200 KB in size.
             A thumbnail's width and height should not exceed 320 pixels.
             Thumbnails can't be reused and can be only uploaded as a new file.
 
         caption (``str``, *optional*):
-            Caption of the document to be sent, 0-1024 characters.
+            Caption of the video to be sent, 0-1024 characters.
             If not specified, the original caption is kept. Pass "" (empty string) to remove the caption.
 
         parse_mode (:obj:`~pyrogram.enums.ParseMode`, *optional*):
             By default, texts are parsed using both Markdown and HTML styles.
             You can combine both syntaxes together.
 
         caption_entities (List of :obj:`~pyrogram.types.MessageEntity`):
             List of special entities that appear in the caption, which can be specified instead of *parse_mode*.
+
+        width (``int``, *optional*):
+            Video width.
+
+        height (``int``, *optional*):
+            Video height.
+
+        duration (``int``, *optional*):
+            Video duration.
+
+        supports_streaming (``bool``, *optional*):
+            Pass True, if the uploaded video is suitable for streaming.
+
+        has_spoiler (``bool``, *optional*):
+            Pass True if the photo needs to be covered with a spoiler animation.
     """
 
     def __init__(
         self,
         media: Union[str, BinaryIO],
         thumb: str = None,
         caption: str = "",
         parse_mode: Optional["enums.ParseMode"] = None,
-        caption_entities: List[MessageEntity] = None
+        caption_entities: List[MessageEntity] = None,
+        width: int = 0,
+        height: int = 0,
+        duration: int = 0,
+        supports_streaming: bool = True,
+        has_spoiler: bool = None,
     ):
         super().__init__(media, caption, parse_mode, caption_entities)
 
         self.thumb = thumb
+        self.width = width
+        self.height = height
+        self.duration = duration
+        self.supports_streaming = supports_streaming
+        self.has_spoiler = has_spoiler
```

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/input_media/input_media_photo.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/user_and_chats/invite_link_importer.py`

 * *Files 21% similar despite different names*

```diff
@@ -12,52 +12,50 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
-from typing import Optional, List, Union, BinaryIO
+from datetime import datetime
 
-from .input_media import InputMedia
-from ..messages_and_media import MessageEntity
-from ... import enums
+from pyrogram import raw, utils
+from pyrogram import types
+from ..object import Object
 
 
-class InputMediaPhoto(InputMedia):
-    """A photo to be sent inside an album.
-    It is intended to be used with :obj:`~pyrogram.Client.send_media_group`.
+class InviteLinkImporter(Object):
+    """The date and user of when someone has joined with an invite link.
 
     Parameters:
-        media (``str`` | ``BinaryIO``):
-            Photo to send.
-            Pass a file_id as string to send a photo that exists on the Telegram servers or
-            pass a file path as string to upload a new photo that exists on your local machine or
-            pass a binary file-like object with its attribute “.name” set for in-memory uploads or
-            pass an HTTP URL as a string for Telegram to get a photo from the Internet.
-
-        caption (``str``, *optional*):
-            Caption of the photo to be sent, 0-1024 characters.
-            If not specified, the original caption is kept. Pass "" (empty string) to remove the caption.
-
-        parse_mode (:obj:`~pyrogram.enums.ParseMode`, *optional*):
-            By default, texts are parsed using both Markdown and HTML styles.
-            You can combine both syntaxes together.
+        date (:py:obj:`~datetime.datetime`):
+            The time of when this user used the given link
 
-        caption_entities (List of :obj:`~pyrogram.types.MessageEntity`):
-            List of special entities that appear in the caption, which can be specified instead of *parse_mode*.
-
-        has_spoiler (``bool``, *optional*):
-            Pass True if the photo needs to be covered with a spoiler animation.
+        user (:obj:`~pyrogram.types.User`):
+            The user that has used the given invite link
     """
 
     def __init__(
-        self,
-        media: Union[str, BinaryIO],
-        caption: str = "",
-        parse_mode: Optional["enums.ParseMode"] = None,
-        caption_entities: List[MessageEntity] = None,
-        has_spoiler: bool = None
+        self, *,
+        date: datetime,
+        user: "types.User"
     ):
-        super().__init__(media, caption, parse_mode, caption_entities)
+        super().__init__(None)
+
+        self.date = date
+        self.user = user
+
+    @staticmethod
+    def _parse(client, invite_importers: "raw.types.messages.ChatInviteImporters"):
+        importers = types.List()
+
+        d = {i.id: i for i in invite_importers.users}
+
+        for j in invite_importers.importers:
+            importers.append(
+                InviteLinkImporter(
+                    date=utils.timestamp_to_datetime(j.date),
+                    user=types.User._parse(client=None, user=d[j.user_id])
+                )
+            )
 
-        self.has_spoiler = has_spoiler
+        return importers
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/input_media/input_media_video.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/messages_and_media/thumbnail.py`

 * *Files 24% similar despite different names*

```diff
@@ -12,80 +12,100 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
-from typing import Optional, List, Union, BinaryIO
+from typing import List, Optional, Union
 
-from .input_media import InputMedia
-from ..messages_and_media import MessageEntity
-from ... import enums
+import pyrogram
+from pyrogram import raw
+from pyrogram.file_id import FileId, FileType, FileUniqueId, FileUniqueType, ThumbnailSource
+from ..object import Object
 
 
-class InputMediaVideo(InputMedia):
-    """A video to be sent inside an album.
-    It is intended to be used with :obj:`~pyrogram.Client.send_media_group`.
+class Thumbnail(Object):
+    """One size of a photo or a file/sticker thumbnail.
 
     Parameters:
-        media (``str`` | ``BinaryIO``):
-            Video to send.
-            Pass a file_id as string to send a video that exists on the Telegram servers or
-            pass a file path as string to upload a new video that exists on your local machine or
-            pass a binary file-like object with its attribute “.name” set for in-memory uploads or
-            pass an HTTP URL as a string for Telegram to get a video from the Internet.
-
-        thumb (``str``):
-            Thumbnail of the video sent.
-            The thumbnail should be in JPEG format and less than 200 KB in size.
-            A thumbnail's width and height should not exceed 320 pixels.
-            Thumbnails can't be reused and can be only uploaded as a new file.
-
-        caption (``str``, *optional*):
-            Caption of the video to be sent, 0-1024 characters.
-            If not specified, the original caption is kept. Pass "" (empty string) to remove the caption.
-
-        parse_mode (:obj:`~pyrogram.enums.ParseMode`, *optional*):
-            By default, texts are parsed using both Markdown and HTML styles.
-            You can combine both syntaxes together.
-
-        caption_entities (List of :obj:`~pyrogram.types.MessageEntity`):
-            List of special entities that appear in the caption, which can be specified instead of *parse_mode*.
-
-        width (``int``, *optional*):
-            Video width.
-
-        height (``int``, *optional*):
-            Video height.
+        file_id (``str``):
+            Identifier for this file, which can be used to download or reuse the file.
 
-        duration (``int``, *optional*):
-            Video duration.
+        file_unique_id (``str``):
+            Unique identifier for this file, which is supposed to be the same over time and for different accounts.
+            Can't be used to download or reuse the file.
 
-        supports_streaming (``bool``, *optional*):
-            Pass True, if the uploaded video is suitable for streaming.
+        width (``int``):
+            Photo width.
 
-        has_spoiler (``bool``, *optional*):
-            Pass True if the photo needs to be covered with a spoiler animation.
+        height (``int``):
+            Photo height.
+
+        file_size (``int``):
+            File size.
     """
 
     def __init__(
         self,
-        media: Union[str, BinaryIO],
-        thumb: str = None,
-        caption: str = "",
-        parse_mode: Optional["enums.ParseMode"] = None,
-        caption_entities: List[MessageEntity] = None,
-        width: int = 0,
-        height: int = 0,
-        duration: int = 0,
-        supports_streaming: bool = True,
-        has_spoiler: bool = None,
+        *,
+        client: "pyrogram.Client" = None,
+        file_id: str,
+        file_unique_id: str,
+        width: int,
+        height: int,
+        file_size: int
     ):
-        super().__init__(media, caption, parse_mode, caption_entities)
+        super().__init__(client)
 
-        self.thumb = thumb
+        self.file_id = file_id
+        self.file_unique_id = file_unique_id
         self.width = width
         self.height = height
-        self.duration = duration
-        self.supports_streaming = supports_streaming
-        self.has_spoiler = has_spoiler
+        self.file_size = file_size
+
+    @staticmethod
+    def _parse(client, media: Union["raw.types.Photo", "raw.types.Document"]) -> Optional[List["Thumbnail"]]:
+        if isinstance(media, raw.types.Photo):
+            raw_thumbs = [i for i in media.sizes if isinstance(i, raw.types.PhotoSize)]
+            raw_thumbs.sort(key=lambda p: p.size)
+            raw_thumbs = raw_thumbs[:-1]
+
+            file_type = FileType.PHOTO
+        elif isinstance(media, raw.types.Document):
+            raw_thumbs = media.thumbs
+            file_type = FileType.THUMBNAIL
+        else:
+            return
+
+        parsed_thumbs = []
+
+        for thumb in raw_thumbs:
+            if not isinstance(thumb, raw.types.PhotoSize):
+                continue
+
+            parsed_thumbs.append(
+                Thumbnail(
+                    file_id=FileId(
+                        file_type=file_type,
+                        dc_id=media.dc_id,
+                        media_id=media.id,
+                        access_hash=media.access_hash,
+                        file_reference=media.file_reference,
+                        thumbnail_file_type=file_type,
+                        thumbnail_source=ThumbnailSource.THUMBNAIL,
+                        thumbnail_size=thumb.type,
+                        volume_id=0,
+                        local_id=0
+                    ).encode(),
+                    file_unique_id=FileUniqueId(
+                        file_unique_type=FileUniqueType.DOCUMENT,
+                        media_id=media.id
+                    ).encode(),
+                    width=thumb.w,
+                    height=thumb.h,
+                    file_size=thumb.size,
+                    client=client
+                )
+            )
+
+        return parsed_thumbs or None
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/input_media/input_phone_contact.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/input_media/input_phone_contact.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/input_message_content/__init__.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/input_message_content/input_message_content.py`

 * *Files 17% similar despite different names*

```diff
@@ -12,13 +12,29 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
-from .input_message_content import InputMessageContent
-from .input_text_message_content import InputTextMessageContent
+import pyrogram
 
-__all__ = [
-    "InputMessageContent", "InputTextMessageContent"
-]
+from ..object import Object
+
+"""- :obj:`~pyrogram.types.InputLocationMessageContent`
+    - :obj:`~pyrogram.types.InputVenueMessageContent`
+    - :obj:`~pyrogram.types.InputContactMessageContent`"""
+
+
+class InputMessageContent(Object):
+    """Content of a message to be sent as a result of an inline query.
+
+    Pyrogram currently supports the following types:
+
+    - :obj:`~pyrogram.types.InputTextMessageContent`
+    """
+
+    def __init__(self):
+        super().__init__()
+
+    async def write(self, client: "pyrogram.Client", reply_markup):
+        raise NotImplementedError
```

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/input_message_content/input_message_content.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/messages_and_media/location.py`

 * *Files 26% similar despite different names*

```diff
@@ -14,27 +14,42 @@
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
 import pyrogram
 
+from pyrogram import raw
 from ..object import Object
 
-"""- :obj:`~pyrogram.types.InputLocationMessageContent`
-    - :obj:`~pyrogram.types.InputVenueMessageContent`
-    - :obj:`~pyrogram.types.InputContactMessageContent`"""
 
+class Location(Object):
+    """A point on the map.
 
-class InputMessageContent(Object):
-    """Content of a message to be sent as a result of an inline query.
+    Parameters:
+        longitude (``float``):
+            Longitude as defined by sender.
 
-    Pyrogram currently supports the following types:
-
-    - :obj:`~pyrogram.types.InputTextMessageContent`
+        latitude (``float``):
+            Latitude as defined by sender.
     """
 
-    def __init__(self):
-        super().__init__()
-
-    async def write(self, client: "pyrogram.Client", reply_markup):
-        raise NotImplementedError
+    def __init__(
+        self,
+        *,
+        client: "pyrogram.Client" = None,
+        longitude: float,
+        latitude: float
+    ):
+        super().__init__(client)
+
+        self.longitude = longitude
+        self.latitude = latitude
+
+    @staticmethod
+    def _parse(client, geo_point: "raw.types.GeoPoint") -> "Location":
+        if isinstance(geo_point, raw.types.GeoPoint):
+            return Location(
+                longitude=geo_point.long,
+                latitude=geo_point.lat,
+                client=client
+            )
```

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/input_message_content/input_text_message_content.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/input_message_content/input_text_message_content.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/list.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/user_and_chats/chat_joined_by_request.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,19 +12,18 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
-from .object import Object
+from ..object import Object
 
 
-class List(list):
-    __slots__ = []
+class ChatJoinedByRequest(Object):
+    """A service message about a user join request approved in the chat.
 
-    def __str__(self):
-        # noinspection PyCallByClass
-        return Object.__str__(self)
+    Currently holds no information.
+    """
 
-    def __repr__(self):
-        return f"pyrogram.types.List([{','.join(Object.__repr__(i) for i in self)}])"
+    def __init__(self):
+        super().__init__()
```

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/messages_and_media/__init__.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/messages_and_media/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/messages_and_media/animation.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/messages_and_media/animation.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/messages_and_media/audio.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/messages_and_media/audio.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/messages_and_media/contact.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/messages_and_media/contact.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/messages_and_media/dice.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/user_and_chats/video_chat_scheduled.py`

 * *Files 20% similar despite different names*

```diff
@@ -12,36 +12,32 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
-import pyrogram
-from pyrogram import raw
+from datetime import datetime
+
+from pyrogram import raw, utils
 from ..object import Object
 
 
-class Dice(Object):
-    """A dice with a random value from 1 to 6 for currently supported base emoji.
+class VideoChatScheduled(Object):
+    """A service message about a voice chat scheduled in the chat.
 
     Parameters:
-        emoji (``string``):
-            Emoji on which the dice throw animation is based.
-
-        value (``int``):
-            Value of the dice, 1-6 for currently supported base emoji.
+        start_date (:py:obj:`~datetime.datetime`):
+            Point in time when the voice chat is supposed to be started by a chat administrator.
     """
 
-    def __init__(self, *, client: "pyrogram.Client" = None, emoji: str, value: int):
-        super().__init__(client)
+    def __init__(
+        self, *,
+        start_date: datetime
+    ):
+        super().__init__()
 
-        self.emoji = emoji
-        self.value = value
+        self.start_date = start_date
 
     @staticmethod
-    def _parse(client, dice: "raw.types.MessageMediaDice") -> "Dice":
-        return Dice(
-            emoji=dice.emoticon,
-            value=dice.value,
-            client=client
-        )
+    def _parse(action: "raw.types.MessageActionGroupCallScheduled") -> "VideoChatScheduled":
+        return VideoChatScheduled(start_date=utils.timestamp_to_datetime(action.schedule_date))
```

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/messages_and_media/document.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/messages_and_media/document.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/messages_and_media/game.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/messages_and_media/game.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/messages_and_media/location.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/messages_and_media/message_reactions.py`

 * *Files 20% similar despite different names*

```diff
@@ -12,44 +12,45 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
-import pyrogram
+from typing import Optional, List
 
-from pyrogram import raw
+import pyrogram
+from pyrogram import raw, types
 from ..object import Object
 
 
-class Location(Object):
-    """A point on the map.
+class MessageReactions(Object):
+    """Contains information about a message reactions.
 
     Parameters:
-        longitude (``float``):
-            Longitude as defined by sender.
-
-        latitude (``float``):
-            Latitude as defined by sender.
+        reactions (List of :obj:`~pyrogram.types.Reaction`):
+            Reactions list.
     """
 
     def __init__(
         self,
         *,
         client: "pyrogram.Client" = None,
-        longitude: float,
-        latitude: float
+        reactions: Optional[List["types.Reaction"]] = None,
     ):
         super().__init__(client)
 
-        self.longitude = longitude
-        self.latitude = latitude
+        self.reactions = reactions
 
     @staticmethod
-    def _parse(client, geo_point: "raw.types.GeoPoint") -> "Location":
-        if isinstance(geo_point, raw.types.GeoPoint):
-            return Location(
-                longitude=geo_point.long,
-                latitude=geo_point.lat,
-                client=client
-            )
+    def _parse(
+        client: "pyrogram.Client",
+        message_reactions: Optional["raw.base.MessageReactions"] = None
+    ) -> Optional["MessageReactions"]:
+        if not message_reactions:
+            return None
+
+        return MessageReactions(
+            client=client,
+            reactions=[types.Reaction._parse_count(client, reaction)
+                       for reaction in message_reactions.results]
+        )
```

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/messages_and_media/message.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/messages_and_media/message.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/messages_and_media/message_entity.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/messages_and_media/message_entity.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/messages_and_media/message_reactions.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/user_and_chats/forum_topic_created.py`

 * *Files 19% similar despite different names*

```diff
@@ -12,45 +12,47 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
-from typing import Optional, List
-
-import pyrogram
-from pyrogram import raw, types
+from pyrogram import raw
 from ..object import Object
 
 
-class MessageReactions(Object):
-    """Contains information about a message reactions.
+class ForumTopicCreated(Object):
+    """A service message about a new forum topic created in the chat.
+
 
     Parameters:
-        reactions (List of :obj:`~pyrogram.types.Reaction`):
-            Reactions list.
+        title (``String``):
+            Name of the topic.
+
+        icon_color (``Integer``):
+            Color of the topic icon in RGB format
+
+        icon_emoji_id (``Integer``, *optional*):
+            Unique identifier of the custom emoji shown as the topic icon
     """
 
     def __init__(
-        self,
-        *,
-        client: "pyrogram.Client" = None,
-        reactions: Optional[List["types.Reaction"]] = None,
+        self, *,
+        title: str,
+        icon_color: int,
+        icon_emoji_id: int = None
     ):
-        super().__init__(client)
+        super().__init__()
 
-        self.reactions = reactions
+        self.title = title
+        self.icon_color = icon_color
+        self.icon_emoji_id = icon_emoji_id
 
     @staticmethod
-    def _parse(
-        client: "pyrogram.Client",
-        message_reactions: Optional["raw.base.MessageReactions"] = None
-    ) -> Optional["MessageReactions"]:
-        if not message_reactions:
-            return None
-
-        return MessageReactions(
-            client=client,
-            reactions=[types.Reaction._parse_count(client, reaction)
-                       for reaction in message_reactions.results]
+    def _parse(action: "raw.types.MessageActionTopicCreate") -> "ForumTopicCreated":
+
+
+        return ForumTopicCreated(
+            title=getattr(action,"title", None),
+            icon_color=getattr(action,"icon_color", None),
+            icon_emoji_id=getattr(action,"icon_emoji_id", None)
         )
```

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/messages_and_media/photo.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/messages_and_media/photo.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/messages_and_media/poll.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/messages_and_media/poll.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/messages_and_media/poll_option.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/messages_and_media/poll_option.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/messages_and_media/reaction.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/messages_and_media/reaction.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/messages_and_media/sticker.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/messages_and_media/sticker.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/messages_and_media/stickerset.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/messages_and_media/stickerset.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/messages_and_media/stripped_thumbnail.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/messages_and_media/stripped_thumbnail.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/messages_and_media/thumbnail.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/messages_and_media/voice.py`

 * *Files 19% similar despite different names*

```diff
@@ -12,100 +12,85 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
-from typing import List, Optional, Union
+from datetime import datetime
 
 import pyrogram
-from pyrogram import raw
-from pyrogram.file_id import FileId, FileType, FileUniqueId, FileUniqueType, ThumbnailSource
+from pyrogram import raw, utils
+from pyrogram.file_id import FileId, FileType, FileUniqueId, FileUniqueType
 from ..object import Object
 
 
-class Thumbnail(Object):
-    """One size of a photo or a file/sticker thumbnail.
+class Voice(Object):
+    """A voice note.
 
     Parameters:
         file_id (``str``):
             Identifier for this file, which can be used to download or reuse the file.
 
         file_unique_id (``str``):
             Unique identifier for this file, which is supposed to be the same over time and for different accounts.
             Can't be used to download or reuse the file.
 
-        width (``int``):
-            Photo width.
+        duration (``int``):
+            Duration of the audio in seconds as defined by sender.
 
-        height (``int``):
-            Photo height.
+        waveform (``bytes``, *optional*):
+            Voice waveform.
 
-        file_size (``int``):
+        mime_type (``str``, *optional*):
+            MIME type of the file as defined by sender.
+
+        file_size (``int``, *optional*):
             File size.
+
+        date (:py:obj:`~datetime.datetime`, *optional*):
+            Date the voice was sent.
     """
 
     def __init__(
         self,
         *,
         client: "pyrogram.Client" = None,
         file_id: str,
         file_unique_id: str,
-        width: int,
-        height: int,
-        file_size: int
+        duration: int,
+        waveform: bytes = None,
+        mime_type: str = None,
+        file_size: int = None,
+        date: datetime = None
     ):
         super().__init__(client)
 
         self.file_id = file_id
         self.file_unique_id = file_unique_id
-        self.width = width
-        self.height = height
+        self.duration = duration
+        self.waveform = waveform
+        self.mime_type = mime_type
         self.file_size = file_size
+        self.date = date
 
     @staticmethod
-    def _parse(client, media: Union["raw.types.Photo", "raw.types.Document"]) -> Optional[List["Thumbnail"]]:
-        if isinstance(media, raw.types.Photo):
-            raw_thumbs = [i for i in media.sizes if isinstance(i, raw.types.PhotoSize)]
-            raw_thumbs.sort(key=lambda p: p.size)
-            raw_thumbs = raw_thumbs[:-1]
-
-            file_type = FileType.PHOTO
-        elif isinstance(media, raw.types.Document):
-            raw_thumbs = media.thumbs
-            file_type = FileType.THUMBNAIL
-        else:
-            return
-
-        parsed_thumbs = []
-
-        for thumb in raw_thumbs:
-            if not isinstance(thumb, raw.types.PhotoSize):
-                continue
-
-            parsed_thumbs.append(
-                Thumbnail(
-                    file_id=FileId(
-                        file_type=file_type,
-                        dc_id=media.dc_id,
-                        media_id=media.id,
-                        access_hash=media.access_hash,
-                        file_reference=media.file_reference,
-                        thumbnail_file_type=file_type,
-                        thumbnail_source=ThumbnailSource.THUMBNAIL,
-                        thumbnail_size=thumb.type,
-                        volume_id=0,
-                        local_id=0
-                    ).encode(),
-                    file_unique_id=FileUniqueId(
-                        file_unique_type=FileUniqueType.DOCUMENT,
-                        media_id=media.id
-                    ).encode(),
-                    width=thumb.w,
-                    height=thumb.h,
-                    file_size=thumb.size,
-                    client=client
-                )
-            )
-
-        return parsed_thumbs or None
+    def _parse(client, voice: "raw.types.Document", attributes: "raw.types.DocumentAttributeAudio") -> "Voice":
+        return Voice(
+            file_id=FileId(
+                file_type=FileType.VOICE,
+                dc_id=voice.dc_id,
+                media_id=voice.id,
+                access_hash=voice.access_hash,
+                file_reference=voice.file_reference
+            ).encode(),
+            file_unique_id=FileUniqueId(
+                file_unique_type=FileUniqueType.DOCUMENT,
+                media_id=voice.id
+            ).encode(),
+            duration=attributes.duration,
+            mime_type=voice.mime_type,
+            file_size=voice.size,
+            waveform=attributes.waveform,
+            date=utils.timestamp_to_datetime(voice.date),
+            client=client
+        )
```

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/messages_and_media/venue.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/messages_and_media/venue.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/messages_and_media/video.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/messages_and_media/video.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/messages_and_media/video_note.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/messages_and_media/video_note.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/messages_and_media/voice.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/user_and_chats/chat_joiner.py`

 * *Files 26% similar despite different names*

```diff
@@ -13,84 +13,70 @@
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
 from datetime import datetime
+from typing import Dict
 
 import pyrogram
-from pyrogram import raw, utils
-from pyrogram.file_id import FileId, FileType, FileUniqueId, FileUniqueType
+from pyrogram import raw, types, utils
 from ..object import Object
 
 
-class Voice(Object):
-    """A voice note.
+class ChatJoiner(Object):
+    """Contains information about a joiner member of a chat.
 
     Parameters:
-        file_id (``str``):
-            Identifier for this file, which can be used to download or reuse the file.
+        user (:obj:`~pyrogram.types.User`):
+            Information about the user.
 
-        file_unique_id (``str``):
-            Unique identifier for this file, which is supposed to be the same over time and for different accounts.
-            Can't be used to download or reuse the file.
+        date (:py:obj:`~datetime.datetime`):
+            Date when the user joined.
 
-        duration (``int``):
-            Duration of the audio in seconds as defined by sender.
+        bio (``str``, *optional*):
+            Bio of the user.
 
-        waveform (``bytes``, *optional*):
-            Voice waveform.
+        pending (``bool``, *optional*):
+            True in case the chat joiner has a pending request.
 
-        mime_type (``str``, *optional*):
-            MIME type of the file as defined by sender.
-
-        file_size (``int``, *optional*):
-            File size.
-
-        date (:py:obj:`~datetime.datetime`, *optional*):
-            Date the voice was sent.
+        approved_by (:obj:`~pyrogram.types.User`, *optional*):
+            Administrator who approved this chat joiner.
     """
 
     def __init__(
         self,
         *,
-        client: "pyrogram.Client" = None,
-        file_id: str,
-        file_unique_id: str,
-        duration: int,
-        waveform: bytes = None,
-        mime_type: str = None,
-        file_size: int = None,
-        date: datetime = None
+        client: "pyrogram.Client",
+        user: "types.User",
+        date: datetime = None,
+        bio: str = None,
+        pending: bool = None,
+        approved_by: "types.User" = None,
     ):
         super().__init__(client)
 
-        self.file_id = file_id
-        self.file_unique_id = file_unique_id
-        self.duration = duration
-        self.waveform = waveform
-        self.mime_type = mime_type
-        self.file_size = file_size
+        self.user = user
         self.date = date
+        self.bio = bio
+        self.pending = pending
+        self.approved_by = approved_by
 
     @staticmethod
-    def _parse(client, voice: "raw.types.Document", attributes: "raw.types.DocumentAttributeAudio") -> "Voice":
-        return Voice(
-            file_id=FileId(
-                file_type=FileType.VOICE,
-                dc_id=voice.dc_id,
-                media_id=voice.id,
-                access_hash=voice.access_hash,
-                file_reference=voice.file_reference
-            ).encode(),
-            file_unique_id=FileUniqueId(
-                file_unique_type=FileUniqueType.DOCUMENT,
-                media_id=voice.id
-            ).encode(),
-            duration=attributes.duration,
-            mime_type=voice.mime_type,
-            file_size=voice.size,
-            waveform=attributes.waveform,
-            date=utils.timestamp_to_datetime(voice.date),
+    def _parse(
+        client: "pyrogram.Client",
+        joiner: "raw.base.ChatInviteImporter",
+        users: Dict[int, "raw.base.User"],
+    ) -> "ChatJoiner":
+        return ChatJoiner(
+            user=types.User._parse(client, users[joiner.user_id]),
+            date=utils.timestamp_to_datetime(joiner.date),
+            pending=joiner.requested,
+            bio=joiner.about,
+            approved_by=(
+                types.User._parse(client, users[joiner.approved_by])
+                if joiner.approved_by
+                else None
+            ),
             client=client
         )
```

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/messages_and_media/web_app_data.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/messages_and_media/web_app_data.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/messages_and_media/web_page.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/messages_and_media/web_page.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/object.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/object.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/update.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/update.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/user_and_chats/__init__.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/user_and_chats/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/user_and_chats/chat.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/user_and_chats/chat.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/user_and_chats/chat_admin_with_invite_links.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/user_and_chats/chat_admin_with_invite_links.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/user_and_chats/chat_event.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/user_and_chats/chat_event.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/user_and_chats/chat_event_filter.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/user_and_chats/chat_event_filter.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/user_and_chats/chat_invite_link.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/user_and_chats/chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/user_and_chats/chat_join_request.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/user_and_chats/chat_join_request.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/user_and_chats/chat_joined_by_request.py` & `PyroFork-dev-2.2.5.dev202307219555/tests/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,17 @@
-#  Pyrofork - Telegram MTProto API Client Library for Python
-#  Copyright (C) 2022-present Mayuri-Chan <https://github.com/Mayuri-Chan>
+#  Pyrogram - Telegram MTProto API Client Library for Python
+#  Copyright (C) 2017-present Dan <https://github.com/delivrance>
 #
-#  This file is part of Pyrofork.
+#  This file is part of Pyrogram.
 #
-#  Pyrofork is free software: you can redistribute it and/or modify
+#  Pyrogram is free software: you can redistribute it and/or modify
 #  it under the terms of the GNU Lesser General Public License as published
 #  by the Free Software Foundation, either version 3 of the License, or
 #  (at your option) any later version.
 #
-#  Pyrofork is distributed in the hope that it will be useful,
+#  Pyrogram is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
-#  along with Pyrofork.  If not, see <http://www.gnu.org/licenses/>.
-
-from ..object import Object
-
-
-class ChatJoinedByRequest(Object):
-    """A service message about a user join request approved in the chat.
-
-    Currently holds no information.
-    """
-
-    def __init__(self):
-        super().__init__()
+#  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
```

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/user_and_chats/chat_member.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/user_and_chats/chat_member.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/user_and_chats/chat_member_updated.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/user_and_chats/chat_member_updated.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/user_and_chats/chat_permissions.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/user_and_chats/chat_permissions.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/user_and_chats/chat_photo.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/user_and_chats/chat_photo.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/user_and_chats/chat_preview.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/user_and_chats/chat_preview.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/user_and_chats/chat_privileges.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/user_and_chats/chat_privileges.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/user_and_chats/chat_reactions.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/user_and_chats/chat_reactions.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/user_and_chats/dialog.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/user_and_chats/dialog.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/user_and_chats/emoji_status.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/user_and_chats/emoji_status.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/user_and_chats/forum_topic.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/user_and_chats/forum_topic.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-#  Pyrofork - Telegram MTProto API Client Library for Python
-#  Copyright (C) 2022-present Mayuri-Chan <https://github.com/Mayuri-Chan>
+#  Pyrogram - Telegram MTProto API Client Library for Python
+#  Copyright (C) 2017-present Dan <https://github.com/delivrance>
 #
-#  This file is part of Pyrofork.
+#  This file is part of Pyrogram.
 #
-#  Pyrofork is free software: you can redistribute it and/or modify
+#  Pyrogram is free software: you can redistribute it and/or modify
 #  it under the terms of the GNU Lesser General Public License as published
 #  by the Free Software Foundation, either version 3 of the License, or
 #  (at your option) any later version.
 #
-#  Pyrofork is distributed in the hope that it will be useful,
+#  Pyrogram is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
-#  along with Pyrofork.  If not, see <http://www.gnu.org/licenses/>.
+#  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
 from pyrogram import raw, types
 from typing import Union
 from ..object import Object
 
 
 class ForumTopic(Object):
```

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/user_and_chats/forum_topic_closed.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/user_and_chats/video_chat_started.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-#  Pyrofork - Telegram MTProto API Client Library for Python
-#  Copyright (C) 2022-present Mayuri-Chan <https://github.com/Mayuri-Chan>
+#  Pyrogram - Telegram MTProto API Client Library for Python
+#  Copyright (C) 2017-present Dan <https://github.com/delivrance>
 #
-#  This file is part of Pyrofork.
+#  This file is part of Pyrogram.
 #
-#  Pyrofork is free software: you can redistribute it and/or modify
+#  Pyrogram is free software: you can redistribute it and/or modify
 #  it under the terms of the GNU Lesser General Public License as published
 #  by the Free Software Foundation, either version 3 of the License, or
 #  (at your option) any later version.
 #
-#  Pyrofork is distributed in the hope that it will be useful,
+#  Pyrogram is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
-#  along with Pyrofork.  If not, see <http://www.gnu.org/licenses/>.
+#  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
 from ..object import Object
 
 
-class ForumTopicClosed(Object):
-    """A service message about a forum topic closed in the chat.
+class VideoChatStarted(Object):
+    """A service message about a voice chat started in the chat.
 
     Currently holds no information.
     """
 
     def __init__(self):
         super().__init__()
```

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/user_and_chats/forum_topic_created.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/user_and_chats/forum_topic_edited.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,58 +1,58 @@
-#  Pyrofork - Telegram MTProto API Client Library for Python
-#  Copyright (C) 2022-present Mayuri-Chan <https://github.com/Mayuri-Chan>
+#  Pyrogram - Telegram MTProto API Client Library for Python
+#  Copyright (C) 2017-present Dan <https://github.com/delivrance>
 #
-#  This file is part of Pyrofork.
+#  This file is part of Pyrogram.
 #
-#  Pyrofork is free software: you can redistribute it and/or modify
+#  Pyrogram is free software: you can redistribute it and/or modify
 #  it under the terms of the GNU Lesser General Public License as published
 #  by the Free Software Foundation, either version 3 of the License, or
 #  (at your option) any later version.
 #
-#  Pyrofork is distributed in the hope that it will be useful,
+#  Pyrogram is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
-#  along with Pyrofork.  If not, see <http://www.gnu.org/licenses/>.
+#  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
 from pyrogram import raw
 from ..object import Object
 
 
-class ForumTopicCreated(Object):
-    """A service message about a new forum topic created in the chat.
+class ForumTopicEdited(Object):
+    """A service message about a forum topic renamed in the chat.
 
 
     Parameters:
         title (``String``):
             Name of the topic.
 
         icon_color (``Integer``):
             Color of the topic icon in RGB format
 
-        icon_emoji_id (``Integer``, *optional*):
+        icon_custom_emoji_id (``String``, *optional*):
             Unique identifier of the custom emoji shown as the topic icon
     """
 
     def __init__(
         self, *,
-        title: str,
-        icon_color: int,
-        icon_emoji_id: int = None
+        title: str = None,
+        icon_color: int = None,
+        icon_emoji_id: str = None
     ):
         super().__init__()
 
         self.title = title
         self.icon_color = icon_color
         self.icon_emoji_id = icon_emoji_id
 
     @staticmethod
-    def _parse(action: "raw.types.MessageActionTopicCreate") -> "ForumTopicCreated":
+    def _parse(action: "raw.types.MessageActionTopicEdit") -> "ForumTopicEdited":
 
 
-        return ForumTopicCreated(
+        return ForumTopicEdited(
             title=getattr(action,"title", None),
             icon_color=getattr(action,"icon_color", None),
             icon_emoji_id=getattr(action,"icon_emoji_id", None)
         )
```

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/user_and_chats/forum_topic_reopened.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/user_and_chats/forum_topic_reopened.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-#  Pyrofork - Telegram MTProto API Client Library for Python
-#  Copyright (C) 2022-present Mayuri-Chan <https://github.com/Mayuri-Chan>
+#  Pyrogram - Telegram MTProto API Client Library for Python
+#  Copyright (C) 2017-present Dan <https://github.com/delivrance>
 #
-#  This file is part of Pyrofork.
+#  This file is part of Pyrogram.
 #
-#  Pyrofork is free software: you can redistribute it and/or modify
+#  Pyrogram is free software: you can redistribute it and/or modify
 #  it under the terms of the GNU Lesser General Public License as published
 #  by the Free Software Foundation, either version 3 of the License, or
 #  (at your option) any later version.
 #
-#  Pyrofork is distributed in the hope that it will be useful,
+#  Pyrogram is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
-#  along with Pyrofork.  If not, see <http://www.gnu.org/licenses/>.
+#  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
 from ..object import Object
 
 
 class ForumTopicReopened(Object):
     """A service message about a forum topic reopened in the chat.
```

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/user_and_chats/general_forum_topic_hidden.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/user_and_chats/general_forum_topic_hidden.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-#  Pyrofork - Telegram MTProto API Client Library for Python
-#  Copyright (C) 2022-present Mayuri-Chan <https://github.com/Mayuri-Chan>
+#  Pyrogram - Telegram MTProto API Client Library for Python
+#  Copyright (C) 2017-present Dan <https://github.com/delivrance>
 #
-#  This file is part of Pyrofork.
+#  This file is part of Pyrogram.
 #
-#  Pyrofork is free software: you can redistribute it and/or modify
+#  Pyrogram is free software: you can redistribute it and/or modify
 #  it under the terms of the GNU Lesser General Public License as published
 #  by the Free Software Foundation, either version 3 of the License, or
 #  (at your option) any later version.
 #
-#  Pyrofork is distributed in the hope that it will be useful,
+#  Pyrogram is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
-#  along with Pyrofork.  If not, see <http://www.gnu.org/licenses/>.
+#  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
 from ..object import Object
 
 
 class GeneralTopicHidden(Object):
     """A service message about a general topic hidden in the chat.
```

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/user_and_chats/general_forum_topic_unhidden.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/user_and_chats/general_forum_topic_unhidden.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-#  Pyrofork - Telegram MTProto API Client Library for Python
-#  Copyright (C) 2022-present Mayuri-Chan <https://github.com/Mayuri-Chan>
+#  Pyrogram - Telegram MTProto API Client Library for Python
+#  Copyright (C) 2017-present Dan <https://github.com/delivrance>
 #
-#  This file is part of Pyrofork.
+#  This file is part of Pyrogram.
 #
-#  Pyrofork is free software: you can redistribute it and/or modify
+#  Pyrogram is free software: you can redistribute it and/or modify
 #  it under the terms of the GNU Lesser General Public License as published
 #  by the Free Software Foundation, either version 3 of the License, or
 #  (at your option) any later version.
 #
-#  Pyrofork is distributed in the hope that it will be useful,
+#  Pyrogram is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
-#  along with Pyrofork.  If not, see <http://www.gnu.org/licenses/>.
+#  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
 from ..object import Object
 
 
 class GeneralTopicUnhidden(Object):
     """A service message about a general topic unhidden in the chat.
```

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/user_and_chats/invite_link_importer.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/user_and_chats/video_chat_members_invited.py`

 * *Files 23% similar despite different names*

```diff
@@ -12,50 +12,39 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
-from datetime import datetime
+from typing import List, Dict
 
-from pyrogram import raw, utils
-from pyrogram import types
+from pyrogram import raw, types
 from ..object import Object
 
 
-class InviteLinkImporter(Object):
-    """The date and user of when someone has joined with an invite link.
+class VideoChatMembersInvited(Object):
+    """A service message about new members invited to a voice chat.
 
-    Parameters:
-        date (:py:obj:`~datetime.datetime`):
-            The time of when this user used the given link
 
-        user (:obj:`~pyrogram.types.User`):
-            The user that has used the given invite link
+    Parameters:
+        users (List of :obj:`~pyrogram.types.User`):
+            New members that were invited to the voice chat.
     """
 
     def __init__(
         self, *,
-        date: datetime,
-        user: "types.User"
+        users: List["types.User"]
     ):
-        super().__init__(None)
+        super().__init__()
 
-        self.date = date
-        self.user = user
+        self.users = users
 
     @staticmethod
-    def _parse(client, invite_importers: "raw.types.messages.ChatInviteImporters"):
-        importers = types.List()
-
-        d = {i.id: i for i in invite_importers.users}
-
-        for j in invite_importers.importers:
-            importers.append(
-                InviteLinkImporter(
-                    date=utils.timestamp_to_datetime(j.date),
-                    user=types.User._parse(client=None, user=d[j.user_id])
-                )
-            )
+    def _parse(
+        client,
+        action: "raw.types.MessageActionInviteToGroupCall",
+        users: Dict[int, "raw.types.User"]
+    ) -> "VideoChatMembersInvited":
+        users = [types.User._parse(client, users[i]) for i in action.users]
 
-        return importers
+        return VideoChatMembersInvited(users=users)
```

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/user_and_chats/peer_channel.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/user_and_chats/peer_channel.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-#  Pyrofork - Telegram MTProto API Client Library for Python
-#  Copyright (C) 2022-present Mayuri-Chan <https://github.com/Mayuri-Chan>
+#  Pyrogram - Telegram MTProto API Client Library for Python
+#  Copyright (C) 2017-present Dan <https://github.com/delivrance>
 #
-#  This file is part of Pyrofork.
+#  This file is part of Pyrogram.
 #
-#  Pyrofork is free software: you can redistribute it and/or modify
+#  Pyrogram is free software: you can redistribute it and/or modify
 #  it under the terms of the GNU Lesser General Public License as published
 #  by the Free Software Foundation, either version 3 of the License, or
 #  (at your option) any later version.
 #
-#  Pyrofork is distributed in the hope that it will be useful,
+#  Pyrogram is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
-#  along with Pyrofork.  If not, see <http://www.gnu.org/licenses/>.
+#  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
 from pyrogram import raw
 from ..object import Object
 
 
 class PeerChannel(Object):
     """A PeerChannel.
```

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/user_and_chats/peer_user.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/user_and_chats/peer_user.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,24 @@
-#  Pyrofork - Telegram MTProto API Client Library for Python
-#  Copyright (C) 2022-present Mayuri-Chan <https://github.com/Mayuri-Chan>
+#  Pyrogram - Telegram MTProto API Client Library for Python
+#  Copyright (C) 2017-present Dan <https://github.com/delivrance>
 #
-#  This file is part of Pyrofork.
+#  This file is part of Pyrogram.
 #
-#  Pyrofork is free software: you can redistribute it and/or modify
+#  Pyrogram is free software: you can redistribute it and/or modify
 #  it under the terms of the GNU Lesser General Public License as published
 #  by the Free Software Foundation, either version 3 of the License, or
 #  (at your option) any later version.
 #
-#  Pyrofork is distributed in the hope that it will be useful,
+#  Pyrogram is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
-#  along with Pyrofork.  If not, see <http://www.gnu.org/licenses/>.
-
+#  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
 from pyrogram import raw
 from ..object import Object
 
 
 class PeerUser(Object):
     """A PeerUser.
```

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/user_and_chats/restriction.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/user_and_chats/restriction.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/user_and_chats/user.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/user_and_chats/user.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/user_and_chats/username.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/user_and_chats/username.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/user_and_chats/video_chat_ended.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/types/user_and_chats/video_chat_ended.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/types/user_and_chats/video_chat_members_invited.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/methods/chats/edit_general_topic.py`

 * *Files 25% similar despite different names*

```diff
@@ -11,40 +11,46 @@
 #  Pyrogram is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
-
-from typing import List, Dict
-
-from pyrogram import raw, types
-from ..object import Object
-
-
-class VideoChatMembersInvited(Object):
-    """A service message about new members invited to a voice chat.
-
-
-    Parameters:
-        users (List of :obj:`~pyrogram.types.User`):
-            New members that were invited to the voice chat.
-    """
-
-    def __init__(
-        self, *,
-        users: List["types.User"]
-    ):
-        super().__init__()
-
-        self.users = users
-
-    @staticmethod
-    def _parse(
-        client,
-        action: "raw.types.MessageActionInviteToGroupCall",
-        users: Dict[int, "raw.types.User"]
-    ) -> "VideoChatMembersInvited":
-        users = [types.User._parse(client, users[i]) for i in action.users]
-
-        return VideoChatMembersInvited(users=users)
+import pyrogram
+from pyrogram import raw
+from pyrogram import types
+from typing import Union
+
+
+class EditGeneralTopic:
+    async def edit_general_topic(
+        self: "pyrogram.Client",
+        chat_id: Union[int, str],
+        title: str
+    ) -> bool:
+        """Edit a general forum topic.
+
+        .. include:: /_includes/usable-by/users-bots.rst
+
+        Parameters:
+            chat_id (``int`` | ``str``):
+                Unique identifier (int) or username (str) of the target chat.
+
+            title (``str``):
+                The general forum topic title.
+
+        Returns:
+            `bool`: On success, a True is returned.
+
+        Example:
+            .. code-block:: python
+
+                await app.edit_general_topic(chat_id,"New Topic Title")
+        """
+        await self.invoke(
+            raw.functions.channels.EditForumTopic(
+                channel=await self.resolve_peer(chat_id),
+                topic_id=1,
+                title=title
+            )
+        )
+        return True
```

### Comparing `PyroFork-dev-2.2.5.dev202307219421/pyrogram/utils.py` & `PyroFork-dev-2.2.5.dev202307219555/pyrogram/utils.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/setup.py` & `PyroFork-dev-2.2.5.dev202307219555/setup.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/tests/__init__.py` & `PyroFork-dev-2.2.5.dev202307219555/tests/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/tests/filters/test_command.py` & `PyroFork-dev-2.2.5.dev202307219555/tests/filters/test_command.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/tests/parser/test_html.py` & `PyroFork-dev-2.2.5.dev202307219555/tests/parser/test_html.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.5.dev202307219421/tests/test_file_id.py` & `PyroFork-dev-2.2.5.dev202307219555/tests/test_file_id.py`

 * *Files identical despite different names*

