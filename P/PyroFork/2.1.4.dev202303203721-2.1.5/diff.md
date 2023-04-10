# Comparing `tmp/PyroFork-2.1.4.dev202303203721.tar.gz` & `tmp/PyroFork-2.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyroFork-2.1.4.dev202303203721.tar", last modified: Mon Mar 20 02:43:18 2023, max compression
+gzip compressed data, was "PyroFork-2.1.5.tar", last modified: Mon Apr 10 15:29:00 2023, max compression
```

## Comparing `PyroFork-2.1.4.dev202303203721.tar` & `PyroFork-2.1.5.tar`

### file list

```diff
@@ -1,515 +1,522 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 02:43:18.863853 PyroFork-2.1.4.dev202303203721/
--rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/COPYING.lesser
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-03-20 02:43:18.863853 PyroFork-2.1.4.dev202303203721/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 02:43:18.795849 PyroFork-2.1.4.dev202303203721/PyroFork.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-03-20 02:43:18.000000 PyroFork-2.1.4.dev202303203721/PyroFork.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19857 2023-03-20 02:43:18.000000 PyroFork-2.1.4.dev202303203721/PyroFork.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-20 02:43:18.000000 PyroFork-2.1.4.dev202303203721/PyroFork.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-20 02:43:18.000000 PyroFork-2.1.4.dev202303203721/PyroFork.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-03-20 02:43:18.000000 PyroFork-2.1.4.dev202303203721/PyroFork.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-20 02:43:18.000000 PyroFork-2.1.4.dev202303203721/PyroFork.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 02:43:18.795849 PyroFork-2.1.4.dev202303203721/compiler/
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/compiler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 02:43:18.795849 PyroFork-2.1.4.dev202303203721/compiler/api/
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/compiler/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22402 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/compiler/api/compiler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 02:43:18.795849 PyroFork-2.1.4.dev202303203721/compiler/api/source/
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/compiler/api/source/auth_key.tl
--rw-r--r--   0 runner    (1001) docker     (123)   166523 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/compiler/api/source/main_api.tl
--rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/compiler/api/source/sys_msgs.tl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 02:43:18.795849 PyroFork-2.1.4.dev202303203721/compiler/api/template/
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/compiler/api/template/combinator.txt
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/compiler/api/template/type.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 02:43:18.795849 PyroFork-2.1.4.dev202303203721/compiler/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/compiler/docs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19394 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/compiler/docs/compiler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 02:43:18.795849 PyroFork-2.1.4.dev202303203721/compiler/docs/template/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/compiler/docs/template/page.txt
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/compiler/docs/template/toctree.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 02:43:18.795849 PyroFork-2.1.4.dev202303203721/compiler/errors/
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/compiler/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4917 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/compiler/errors/compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/compiler/errors/sort.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 02:43:18.799850 PyroFork-2.1.4.dev202303203721/compiler/errors/source/
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/compiler/errors/source/303_SEE_OTHER.tsv
--rw-r--r--   0 runner    (1001) docker     (123)    22642 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/compiler/errors/source/400_BAD_REQUEST.tsv
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/compiler/errors/source/401_UNAUTHORIZED.tsv
--rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/compiler/errors/source/403_FORBIDDEN.tsv
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/compiler/errors/source/406_NOT_ACCEPTABLE.tsv
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/compiler/errors/source/420_FLOOD.tsv
--rw-r--r--   0 runner    (1001) docker     (123)     4219 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/compiler/errors/source/500_INTERNAL_SERVER_ERROR.tsv
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/compiler/errors/source/503_SERVICE_UNAVAILABLE.tsv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 02:43:18.799850 PyroFork-2.1.4.dev202303203721/compiler/errors/template/
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/compiler/errors/template/class.txt
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/compiler/errors/template/sub_class.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 02:43:18.799850 PyroFork-2.1.4.dev202303203721/pyrogram/
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-03-20 02:43:10.000000 PyroFork-2.1.4.dev202303203721/pyrogram/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    41979 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 02:43:18.799850 PyroFork-2.1.4.dev202303203721/pyrogram/connection/
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/connection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/connection/connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 02:43:18.799850 PyroFork-2.1.4.dev202303203721/pyrogram/connection/transport/
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/connection/transport/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 02:43:18.803850 PyroFork-2.1.4.dev202303203721/pyrogram/connection/transport/tcp/
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/connection/transport/tcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4095 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/connection/transport/tcp/tcp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/connection/transport/tcp/tcp_abridged.py
--rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/connection/transport/tcp/tcp_abridged_o.py
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/connection/transport/tcp/tcp_full.py
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/connection/transport/tcp/tcp_intermediate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/connection/transport/tcp/tcp_intermediate_o.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 02:43:18.803850 PyroFork-2.1.4.dev202303203721/pyrogram/crypto/
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/crypto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4013 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/crypto/aes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4018 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/crypto/mtproto.py
--rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/crypto/prime.py
--rw-r--r--   0 runner    (1001) docker     (123)    10791 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/crypto/rsa.py
--rw-r--r--   0 runner    (1001) docker     (123)    10054 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)   208021 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/emoji.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 02:43:18.803850 PyroFork-2.1.4.dev202303203721/pyrogram/enums/
--rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/enums/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/enums/auto_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/enums/chat_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     4520 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/enums/chat_event_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/enums/chat_member_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/enums/chat_members_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/enums/chat_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/enums/message_entity_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/enums/message_media_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/enums/message_service_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/enums/messages_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/enums/next_code_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/enums/parse_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/enums/poll_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/enums/sent_code_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/enums/user_status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 02:43:18.803850 PyroFork-2.1.4.dev202303203721/pyrogram/errors/
--rw-r--r--   0 runner    (1001) docker     (123)     2605 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/errors/rpc_error.py
--rw-r--r--   0 runner    (1001) docker     (123)    15154 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/file_id.py
--rw-r--r--   0 runner    (1001) docker     (123)    24836 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 02:43:18.807850 PyroFork-2.1.4.dev202303203721/pyrogram/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/handlers/callback_query_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/handlers/chat_join_request_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/handlers/chat_member_updated_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/handlers/chosen_inline_result_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/handlers/deleted_messages_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/handlers/disconnect_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/handlers/edited_message_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/handlers/handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/handlers/inline_query_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/handlers/message_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/handlers/poll_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/handlers/raw_update_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/handlers/user_status_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 02:43:18.807850 PyroFork-2.1.4.dev202303203721/pyrogram/methods/
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 02:43:18.807850 PyroFork-2.1.4.dev202303203721/pyrogram/methods/advanced/
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/advanced/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/advanced/invoke.py
--rw-r--r--   0 runner    (1001) docker     (123)     4560 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/advanced/resolve_peer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8421 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/advanced/save_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 02:43:18.811850 PyroFork-2.1.4.dev202303203721/pyrogram/methods/auth/
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/auth/accept_terms_of_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/auth/check_password.py
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/auth/connect.py
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/auth/disconnect.py
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/auth/get_password_hint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/auth/initialize.py
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/auth/log_out.py
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/auth/recover_password.py
--rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/auth/resend_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/auth/send_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/auth/send_recovery_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/auth/sign_in.py
--rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/auth/sign_in_bot.py
--rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/auth/sign_up.py
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/auth/terminate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 02:43:18.811850 PyroFork-2.1.4.dev202303203721/pyrogram/methods/bots/
--rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/bots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/bots/answer_callback_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     4990 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/bots/answer_inline_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/bots/answer_web_app_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/bots/delete_bot_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/bots/get_bot_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/bots/get_bot_default_privileges.py
--rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/bots/get_chat_menu_button.py
--rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/bots/get_game_high_scores.py
--rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/bots/get_inline_bot_results.py
--rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/bots/request_callback_answer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/bots/send_game.py
--rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/bots/send_inline_bot_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/bots/set_bot_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/bots/set_bot_default_privileges.py
--rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/bots/set_chat_menu_button.py
--rw-r--r--   0 runner    (1001) docker     (123)     3946 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/bots/set_game_score.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 02:43:18.819851 PyroFork-2.1.4.dev202303203721/pyrogram/methods/chats/
--rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/chats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/chats/add_chat_members.py
--rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/chats/archive_chats.py
--rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/chats/ban_chat_member.py
--rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/chats/close_forum_topic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/chats/close_general_topic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/chats/create_channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/chats/create_forum_topic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/chats/create_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/chats/create_supergroup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/chats/delete_channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/chats/delete_chat_photo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/chats/delete_forum_topic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/chats/delete_supergroup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/chats/delete_user_history.py
--rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/chats/edit_forum_topic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/chats/edit_general_topic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/chats/get_chat.py
--rw-r--r--   0 runner    (1001) docker     (123)     4032 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/chats/get_chat_event_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/chats/get_chat_member.py
--rw-r--r--   0 runner    (1001) docker     (123)     5282 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/chats/get_chat_members.py
--rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/chats/get_chat_members_count.py
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/chats/get_chat_online_count.py
--rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/chats/get_dialogs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/chats/get_dialogs_count.py
--rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/chats/get_forum_topics.py
--rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/chats/get_forum_topics_by_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/chats/get_nearby_chats.py
--rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/chats/get_send_as_chats.py
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/chats/hide_general_topic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/chats/join_chat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2605 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/chats/leave_chat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/chats/mark_chat_unread.py
--rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/chats/pin_chat_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/chats/promote_chat_member.py
--rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/chats/reopen_forum_topic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/chats/reopen_general_topic.py
--rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/chats/restrict_chat_member.py
--rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/chats/set_administrator_title.py
--rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/chats/set_chat_description.py
--rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/chats/set_chat_permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/chats/set_chat_photo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/chats/set_chat_protected_content.py
--rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/chats/set_chat_title.py
--rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/chats/set_chat_username.py
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/chats/set_send_as_chat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/chats/set_slow_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/chats/unarchive_chats.py
--rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/chats/unban_chat_member.py
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/chats/unhide_general_topic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/chats/unpin_all_chat_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/chats/unpin_chat_message.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 02:43:18.819851 PyroFork-2.1.4.dev202303203721/pyrogram/methods/contacts/
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/contacts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/contacts/add_contact.py
--rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/contacts/delete_contacts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/contacts/get_contacts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/contacts/get_contacts_count.py
--rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/contacts/import_contacts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 02:43:18.823851 PyroFork-2.1.4.dev202303203721/pyrogram/methods/decorators/
--rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/decorators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/decorators/on_callback_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/decorators/on_chat_join_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/decorators/on_chat_member_updated.py
--rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/decorators/on_chosen_inline_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/decorators/on_deleted_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/decorators/on_disconnect.py
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/decorators/on_edited_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/decorators/on_inline_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/decorators/on_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/decorators/on_poll.py
--rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/decorators/on_raw_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/decorators/on_user_status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 02:43:18.823851 PyroFork-2.1.4.dev202303203721/pyrogram/methods/invite_links/
--rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/invite_links/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/invite_links/approve_all_chat_join_requests.py
--rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/invite_links/approve_chat_join_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/invite_links/create_chat_invite_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/invite_links/decline_all_chat_join_requests.py
--rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/invite_links/decline_chat_join_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/invite_links/delete_chat_admin_invite_links.py
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/invite_links/delete_chat_invite_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     3533 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/invite_links/edit_chat_invite_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/invite_links/export_chat_invite_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/invite_links/get_chat_admin_invite_links.py
--rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/invite_links/get_chat_admin_invite_links_count.py
--rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/invite_links/get_chat_admins_with_invite_links.py
--rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/invite_links/get_chat_invite_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/invite_links/get_chat_invite_link_joiners.py
--rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/invite_links/get_chat_invite_link_joiners_count.py
--rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/invite_links/get_chat_join_requests.py
--rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/invite_links/revoke_chat_invite_link.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 02:43:18.831851 PyroFork-2.1.4.dev202303203721/pyrogram/methods/messages/
--rw-r--r--   0 runner    (1001) docker     (123)     3921 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/messages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5963 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/messages/copy_media_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     5423 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/messages/copy_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/messages/delete_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     7530 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/messages/download_media.py
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/messages/edit_inline_caption.py
--rw-r--r--   0 runner    (1001) docker     (123)    10375 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/messages/edit_inline_media.py
--rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/messages/edit_inline_reply_markup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/messages/edit_inline_text.py
--rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/messages/edit_message_caption.py
--rw-r--r--   0 runner    (1001) docker     (123)    13022 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/messages/edit_message_media.py
--rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/messages/edit_message_reply_markup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/messages/edit_message_text.py
--rw-r--r--   0 runner    (1001) docker     (123)     4824 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/messages/forward_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/messages/get_chat_history.py
--rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/messages/get_chat_history_count.py
--rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/messages/get_custom_emoji_stickers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/messages/get_discussion_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/messages/get_discussion_replies.py
--rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/messages/get_discussion_replies_count.py
--rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/messages/get_media_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     4741 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/messages/get_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/messages/inline_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/messages/read_chat_history.py
--rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/messages/retract_vote.py
--rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/messages/search_global.py
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/messages/search_global_count.py
--rw-r--r--   0 runner    (1001) docker     (123)     5349 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/messages/search_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/messages/search_messages_count.py
--rw-r--r--   0 runner    (1001) docker     (123)    12828 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/messages/send_animation.py
--rw-r--r--   0 runner    (1001) docker     (123)    11362 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/messages/send_audio.py
--rw-r--r--   0 runner    (1001) docker     (123)     5723 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/messages/send_cached_media.py
--rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/messages/send_chat_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     5111 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/messages/send_contact.py
--rw-r--r--   0 runner    (1001) docker     (123)     5085 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/messages/send_dice.py
--rw-r--r--   0 runner    (1001) docker     (123)    10712 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/messages/send_document.py
--rw-r--r--   0 runner    (1001) docker     (123)     4820 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/messages/send_location.py
--rw-r--r--   0 runner    (1001) docker     (123)    20821 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/messages/send_media_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     7509 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/messages/send_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     9682 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/messages/send_photo.py
--rw-r--r--   0 runner    (1001) docker     (123)     8315 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/messages/send_poll.py
--rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/messages/send_reaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     8582 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/messages/send_sticker.py
--rw-r--r--   0 runner    (1001) docker     (123)     5641 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/messages/send_venue.py
--rw-r--r--   0 runner    (1001) docker     (123)    12198 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/messages/send_video.py
--rw-r--r--   0 runner    (1001) docker     (123)     9556 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/messages/send_video_note.py
--rw-r--r--   0 runner    (1001) docker     (123)     9672 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/messages/send_voice.py
--rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/messages/stop_poll.py
--rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/messages/stream_media.py
--rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/messages/vote_poll.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 02:43:18.831851 PyroFork-2.1.4.dev202303203721/pyrogram/methods/password/
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/password/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/password/change_cloud_password.py
--rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/password/enable_cloud_password.py
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/password/remove_cloud_password.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 02:43:18.835852 PyroFork-2.1.4.dev202303203721/pyrogram/methods/users/
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/users/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/users/block_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/users/delete_profile_photos.py
--rw-r--r--   0 runner    (1001) docker     (123)     4421 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/users/get_chat_photos.py
--rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/users/get_chat_photos_count.py
--rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/users/get_common_chats.py
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/users/get_default_emoji_statuses.py
--rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/users/get_me.py
--rw-r--r--   0 runner    (1001) docker     (123)     2562 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/users/get_users.py
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/users/set_emoji_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/users/set_profile_photo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/users/set_username.py
--rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/users/unblock_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/users/update_profile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 02:43:18.839852 PyroFork-2.1.4.dev202303203721/pyrogram/methods/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/utilities/add_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/utilities/compose.py
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/utilities/export_session_string.py
--rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/utilities/idle.py
--rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/utilities/remove_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/utilities/restart.py
--rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/utilities/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/utilities/start.py
--rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/utilities/stop.py
--rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/methods/utilities/stop_transmission.py
--rw-r--r--   0 runner    (1001) docker     (123)    61915 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/mime_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 02:43:18.839852 PyroFork-2.1.4.dev202303203721/pyrogram/parser/
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8687 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/parser/html.py
--rw-r--r--   0 runner    (1001) docker     (123)     5770 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/parser/markdown.py
--rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/parser/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/parser/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 02:43:18.839852 PyroFork-2.1.4.dev202303203721/pyrogram/raw/
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/raw/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 02:43:18.843852 PyroFork-2.1.4.dev202303203721/pyrogram/raw/core/
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/raw/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/raw/core/future_salt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/raw/core/future_salts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/raw/core/gzip_packed.py
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/raw/core/list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/raw/core/message.py
--rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/raw/core/msg_container.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 02:43:18.843852 PyroFork-2.1.4.dev202303203721/pyrogram/raw/core/primitives/
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/raw/core/primitives/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/raw/core/primitives/bool.py
--rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/raw/core/primitives/bytes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/raw/core/primitives/double.py
--rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/raw/core/primitives/int.py
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/raw/core/primitives/string.py
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/raw/core/primitives/vector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/raw/core/tl_object.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 02:43:18.843852 PyroFork-2.1.4.dev202303203721/pyrogram/session/
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/session/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11446 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/session/auth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 02:43:18.843852 PyroFork-2.1.4.dev202303203721/pyrogram/session/internals/
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/session/internals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/session/internals/data_center.py
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/session/internals/msg_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/session/internals/msg_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/session/internals/seq_no.py
--rw-r--r--   0 runner    (1001) docker     (123)    13422 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/session/session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 02:43:18.843852 PyroFork-2.1.4.dev202303203721/pyrogram/storage/
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/storage/file_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/storage/memory_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     6224 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/storage/sqlite_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/storage/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/sync.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 02:43:18.843852 PyroFork-2.1.4.dev202303203721/pyrogram/types/
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/types/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 02:43:18.843852 PyroFork-2.1.4.dev202303203721/pyrogram/types/authorization/
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/types/authorization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/types/authorization/sent_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/types/authorization/terms_of_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 02:43:18.847852 PyroFork-2.1.4.dev202303203721/pyrogram/types/bots_and_keyboards/
--rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/types/bots_and_keyboards/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/types/bots_and_keyboards/bot_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/types/bots_and_keyboards/bot_command_scope.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/types/bots_and_keyboards/bot_command_scope_all_chat_administrators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/types/bots_and_keyboards/bot_command_scope_all_group_chats.py
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/types/bots_and_keyboards/bot_command_scope_all_private_chats.py
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/types/bots_and_keyboards/bot_command_scope_chat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_administrators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_member.py
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/types/bots_and_keyboards/bot_command_scope_default.py
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/types/bots_and_keyboards/callback_game.py
--rw-r--r--   0 runner    (1001) docker     (123)    12797 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/types/bots_and_keyboards/callback_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/types/bots_and_keyboards/force_reply.py
--rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/types/bots_and_keyboards/game_high_score.py
--rw-r--r--   0 runner    (1001) docker     (123)     8120 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/types/bots_and_keyboards/inline_keyboard_button.py
--rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/types/bots_and_keyboards/inline_keyboard_markup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3514 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/types/bots_and_keyboards/keyboard_button.py
--rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/types/bots_and_keyboards/login_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/types/bots_and_keyboards/menu_button.py
--rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/types/bots_and_keyboards/menu_button_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/types/bots_and_keyboards/menu_button_default.py
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/types/bots_and_keyboards/menu_button_web_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/types/bots_and_keyboards/reply_keyboard_markup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/types/bots_and_keyboards/reply_keyboard_remove.py
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/types/bots_and_keyboards/sent_web_app_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/types/bots_and_keyboards/web_app_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 02:43:18.851853 PyroFork-2.1.4.dev202303203721/pyrogram/types/inline_mode/
--rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/types/inline_mode/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/types/inline_mode/chosen_inline_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     7298 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/types/inline_mode/inline_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/types/inline_mode/inline_query_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     5776 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/types/inline_mode/inline_query_result_animation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3304 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/types/inline_mode/inline_query_result_article.py
--rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/types/inline_mode/inline_query_result_audio.py
--rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/types/inline_mode/inline_query_result_cached_animation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/types/inline_mode/inline_query_result_cached_audio.py
--rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/types/inline_mode/inline_query_result_cached_document.py
--rw-r--r--   0 runner    (1001) docker     (123)     4312 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/types/inline_mode/inline_query_result_cached_photo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/types/inline_mode/inline_query_result_cached_sticker.py
--rw-r--r--   0 runner    (1001) docker     (123)     4394 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/types/inline_mode/inline_query_result_cached_video.py
--rw-r--r--   0 runner    (1001) docker     (123)     4202 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/types/inline_mode/inline_query_result_cached_voice.py
--rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/types/inline_mode/inline_query_result_contact.py
--rw-r--r--   0 runner    (1001) docker     (123)     5240 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/types/inline_mode/inline_query_result_document.py
--rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/types/inline_mode/inline_query_result_location.py
--rw-r--r--   0 runner    (1001) docker     (123)     5261 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/types/inline_mode/inline_query_result_photo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/types/inline_mode/inline_query_result_venue.py
--rw-r--r--   0 runner    (1001) docker     (123)     5474 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/types/inline_mode/inline_query_result_video.py
--rw-r--r--   0 runner    (1001) docker     (123)     4360 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/types/inline_mode/inline_query_result_voice.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 02:43:18.855853 PyroFork-2.1.4.dev202303203721/pyrogram/types/input_media/
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/types/input_media/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/types/input_media/input_media.py
--rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/types/input_media/input_media_animation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/types/input_media/input_media_audio.py
--rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/types/input_media/input_media_document.py
--rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/types/input_media/input_media_photo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/types/input_media/input_media_video.py
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/types/input_media/input_phone_contact.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 02:43:18.855853 PyroFork-2.1.4.dev202303203721/pyrogram/types/input_message_content/
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/types/input_message_content/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/types/input_message_content/input_message_content.py
--rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/types/input_message_content/input_text_message_content.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/types/list.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 02:43:18.859853 PyroFork-2.1.4.dev202303203721/pyrogram/types/messages_and_media/
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/types/messages_and_media/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4044 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/types/messages_and_media/animation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4069 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/types/messages_and_media/audio.py
--rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/types/messages_and_media/contact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/types/messages_and_media/dice.py
--rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/types/messages_and_media/document.py
--rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/types/messages_and_media/game.py
--rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/types/messages_and_media/location.py
--rw-r--r--   0 runner    (1001) docker     (123)   152292 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/types/messages_and_media/message.py
--rw-r--r--   0 runner    (1001) docker     (123)     4352 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/types/messages_and_media/message_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/types/messages_and_media/message_reactions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4309 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/types/messages_and_media/photo.py
--rw-r--r--   0 runner    (1001) docker     (123)     7037 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/types/messages_and_media/poll.py
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/types/messages_and_media/poll_option.py
--rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/types/messages_and_media/reaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     6909 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/types/messages_and_media/sticker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/types/messages_and_media/stripped_thumbnail.py
--rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/types/messages_and_media/thumbnail.py
--rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/types/messages_and_media/venue.py
--rw-r--r--   0 runner    (1001) docker     (123)     4389 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/types/messages_and_media/video.py
--rw-r--r--   0 runner    (1001) docker     (123)     3601 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/types/messages_and_media/video_note.py
--rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/types/messages_and_media/voice.py
--rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/types/messages_and_media/web_app_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     6351 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/types/messages_and_media/web_page.py
--rw-r--r--   0 runner    (1001) docker     (123)     3862 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/types/object.py
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/types/update.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 02:43:18.863853 PyroFork-2.1.4.dev202303203721/pyrogram/types/user_and_chats/
--rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/types/user_and_chats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32771 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/types/user_and_chats/chat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/types/user_and_chats/chat_admin_with_invite_links.py
--rw-r--r--   0 runner    (1001) docker     (123)    22023 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/types/user_and_chats/chat_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     5514 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/types/user_and_chats/chat_event_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4579 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/types/user_and_chats/chat_invite_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/types/user_and_chats/chat_join_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/types/user_and_chats/chat_joined_by_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/types/user_and_chats/chat_joiner.py
--rw-r--r--   0 runner    (1001) docker     (123)     9444 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/types/user_and_chats/chat_member.py
--rw-r--r--   0 runner    (1001) docker     (123)     3674 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/types/user_and_chats/chat_member_updated.py
--rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/types/user_and_chats/chat_permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3967 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/types/user_and_chats/chat_photo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/types/user_and_chats/chat_preview.py
--rw-r--r--   0 runner    (1001) docker     (123)     5300 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/types/user_and_chats/chat_privileges.py
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/types/user_and_chats/chat_reactions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/types/user_and_chats/dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/types/user_and_chats/emoji_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     4970 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/types/user_and_chats/forum_topic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/types/user_and_chats/forum_topic_closed.py
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/types/user_and_chats/forum_topic_created.py
--rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/types/user_and_chats/forum_topic_edited.py
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/types/user_and_chats/forum_topic_reopened.py
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/types/user_and_chats/general_forum_topic_hidden.py
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/types/user_and_chats/general_forum_topic_unhidden.py
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/types/user_and_chats/invite_link_importer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/types/user_and_chats/peer_channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/types/user_and_chats/peer_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/types/user_and_chats/restriction.py
--rw-r--r--   0 runner    (1001) docker     (123)    12836 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/types/user_and_chats/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/types/user_and_chats/video_chat_ended.py
--rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/types/user_and_chats/video_chat_members_invited.py
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/types/user_and_chats/video_chat_scheduled.py
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/types/user_and_chats/video_chat_started.py
--rw-r--r--   0 runner    (1001) docker     (123)    10911 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/pyrogram/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-20 02:43:18.863853 PyroFork-2.1.4.dev202303203721/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3555 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 02:43:18.863853 PyroFork-2.1.4.dev202303203721/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 02:43:18.863853 PyroFork-2.1.4.dev202303203721/tests/filters/
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/tests/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/tests/filters/test_command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 02:43:18.863853 PyroFork-2.1.4.dev202303203721/tests/parser/
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/tests/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6264 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/tests/parser/test_html.py
--rw-r--r--   0 runner    (1001) docker     (123)     8208 2023-03-20 02:43:01.000000 PyroFork-2.1.4.dev202303203721/tests/test_file_id.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:29:00.941119 PyroFork-2.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-04-10 15:28:46.000000 PyroFork-2.1.5/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-04-10 15:28:46.000000 PyroFork-2.1.5/COPYING.lesser
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-10 15:28:46.000000 PyroFork-2.1.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-04-10 15:28:46.000000 PyroFork-2.1.5/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     3897 2023-04-10 15:29:00.941119 PyroFork-2.1.5/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:29:00.861117 PyroFork-2.1.5/PyroFork.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3897 2023-04-10 15:29:00.000000 PyroFork-2.1.5/PyroFork.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20126 2023-04-10 15:29:00.000000 PyroFork-2.1.5/PyroFork.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 15:29:00.000000 PyroFork-2.1.5/PyroFork.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 15:29:00.000000 PyroFork-2.1.5/PyroFork.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-10 15:29:00.000000 PyroFork-2.1.5/PyroFork.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-10 15:29:00.000000 PyroFork-2.1.5/PyroFork.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-04-10 15:28:46.000000 PyroFork-2.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:29:00.861117 PyroFork-2.1.5/compiler/
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-04-10 15:28:46.000000 PyroFork-2.1.5/compiler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:29:00.865118 PyroFork-2.1.5/compiler/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-04-10 15:28:46.000000 PyroFork-2.1.5/compiler/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22402 2023-04-10 15:28:46.000000 PyroFork-2.1.5/compiler/api/compiler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:29:00.865118 PyroFork-2.1.5/compiler/api/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-04-10 15:28:46.000000 PyroFork-2.1.5/compiler/api/source/auth_key.tl
+-rw-r--r--   0 runner    (1001) docker     (123)   166709 2023-04-10 15:28:46.000000 PyroFork-2.1.5/compiler/api/source/main_api.tl
+-rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-04-10 15:28:46.000000 PyroFork-2.1.5/compiler/api/source/sys_msgs.tl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:29:00.865118 PyroFork-2.1.5/compiler/api/template/
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-10 15:28:46.000000 PyroFork-2.1.5/compiler/api/template/combinator.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-04-10 15:28:46.000000 PyroFork-2.1.5/compiler/api/template/type.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:29:00.865118 PyroFork-2.1.5/compiler/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-04-10 15:28:46.000000 PyroFork-2.1.5/compiler/docs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19889 2023-04-10 15:28:46.000000 PyroFork-2.1.5/compiler/docs/compiler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:29:00.865118 PyroFork-2.1.5/compiler/docs/template/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-10 15:28:46.000000 PyroFork-2.1.5/compiler/docs/template/page.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-10 15:28:46.000000 PyroFork-2.1.5/compiler/docs/template/toctree.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:29:00.865118 PyroFork-2.1.5/compiler/errors/
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-04-10 15:28:46.000000 PyroFork-2.1.5/compiler/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4917 2023-04-10 15:28:46.000000 PyroFork-2.1.5/compiler/errors/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-04-10 15:28:46.000000 PyroFork-2.1.5/compiler/errors/sort.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:29:00.865118 PyroFork-2.1.5/compiler/errors/source/
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-04-10 15:28:46.000000 PyroFork-2.1.5/compiler/errors/source/303_SEE_OTHER.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)    22642 2023-04-10 15:28:46.000000 PyroFork-2.1.5/compiler/errors/source/400_BAD_REQUEST.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-04-10 15:28:46.000000 PyroFork-2.1.5/compiler/errors/source/401_UNAUTHORIZED.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-04-10 15:28:46.000000 PyroFork-2.1.5/compiler/errors/source/403_FORBIDDEN.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-04-10 15:28:46.000000 PyroFork-2.1.5/compiler/errors/source/406_NOT_ACCEPTABLE.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-04-10 15:28:46.000000 PyroFork-2.1.5/compiler/errors/source/420_FLOOD.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)     4219 2023-04-10 15:28:46.000000 PyroFork-2.1.5/compiler/errors/source/500_INTERNAL_SERVER_ERROR.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-10 15:28:46.000000 PyroFork-2.1.5/compiler/errors/source/503_SERVICE_UNAVAILABLE.tsv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:29:00.865118 PyroFork-2.1.5/compiler/errors/template/
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-04-10 15:28:46.000000 PyroFork-2.1.5/compiler/errors/template/class.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-10 15:28:46.000000 PyroFork-2.1.5/compiler/errors/template/sub_class.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:29:00.869118 PyroFork-2.1.5/pyrogram/
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40417 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:29:00.869118 PyroFork-2.1.5/pyrogram/connection/
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/connection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/connection/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:29:00.869118 PyroFork-2.1.5/pyrogram/connection/transport/
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/connection/transport/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:29:00.869118 PyroFork-2.1.5/pyrogram/connection/transport/tcp/
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/connection/transport/tcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4100 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/connection/transport/tcp/tcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/connection/transport/tcp/tcp_abridged.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/connection/transport/tcp/tcp_abridged_o.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/connection/transport/tcp/tcp_full.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/connection/transport/tcp/tcp_intermediate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/connection/transport/tcp/tcp_intermediate_o.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:29:00.869118 PyroFork-2.1.5/pyrogram/crypto/
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/crypto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4013 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/crypto/aes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4767 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/crypto/mtproto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/crypto/prime.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10791 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/crypto/rsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10085 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)   208021 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/emoji.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:29:00.873118 PyroFork-2.1.5/pyrogram/enums/
+-rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/enums/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/enums/auto_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/enums/chat_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4520 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/enums/chat_event_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/enums/chat_member_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/enums/chat_members_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/enums/chat_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/enums/message_entity_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/enums/message_media_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/enums/message_service_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/enums/messages_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/enums/next_code_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/enums/parse_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/enums/poll_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/enums/sent_code_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/enums/user_status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:29:00.873118 PyroFork-2.1.5/pyrogram/errors/
+-rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/errors/rpc_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15154 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/file_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24836 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:29:00.877118 PyroFork-2.1.5/pyrogram/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/handlers/callback_query_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/handlers/chat_join_request_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/handlers/chat_member_updated_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/handlers/chosen_inline_result_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/handlers/deleted_messages_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/handlers/disconnect_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/handlers/edited_message_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/handlers/handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/handlers/inline_query_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/handlers/message_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/handlers/poll_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/handlers/raw_update_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/handlers/user_status_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:29:00.877118 PyroFork-2.1.5/pyrogram/methods/
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:29:00.877118 PyroFork-2.1.5/pyrogram/methods/advanced/
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/advanced/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/advanced/invoke.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4560 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/advanced/resolve_peer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8164 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/advanced/save_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:29:00.881118 PyroFork-2.1.5/pyrogram/methods/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/auth/accept_terms_of_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/auth/check_password.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/auth/connect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/auth/disconnect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/auth/get_password_hint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/auth/initialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/auth/log_out.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/auth/recover_password.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/auth/resend_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/auth/send_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/auth/send_recovery_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/auth/sign_in.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/auth/sign_in_bot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/auth/sign_up.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/auth/terminate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:29:00.881118 PyroFork-2.1.5/pyrogram/methods/bots/
+-rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/bots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/bots/answer_callback_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4990 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/bots/answer_inline_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/bots/answer_web_app_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/bots/delete_bot_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/bots/get_bot_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/bots/get_bot_default_privileges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/bots/get_chat_menu_button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/bots/get_game_high_scores.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/bots/get_inline_bot_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/bots/request_callback_answer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/bots/send_game.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/bots/send_inline_bot_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/bots/set_bot_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/bots/set_bot_default_privileges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/bots/set_chat_menu_button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3946 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/bots/set_game_score.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:29:00.889118 PyroFork-2.1.5/pyrogram/methods/chats/
+-rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/chats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/chats/add_chat_members.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/chats/archive_chats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/chats/ban_chat_member.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/chats/close_forum_topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/chats/close_general_topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/chats/create_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/chats/create_forum_topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/chats/create_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/chats/create_supergroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/chats/delete_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/chats/delete_chat_photo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/chats/delete_forum_topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/chats/delete_supergroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/chats/delete_user_history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/chats/edit_forum_topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/chats/edit_general_topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/chats/get_chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4032 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/chats/get_chat_event_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/chats/get_chat_member.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5282 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/chats/get_chat_members.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/chats/get_chat_members_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/chats/get_chat_online_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/chats/get_dialogs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/chats/get_dialogs_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/chats/get_forum_topics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/chats/get_forum_topics_by_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/chats/get_nearby_chats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/chats/get_send_as_chats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/chats/hide_general_topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/chats/join_chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2605 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/chats/leave_chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/chats/mark_chat_unread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/chats/pin_chat_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/chats/promote_chat_member.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/chats/reopen_forum_topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/chats/reopen_general_topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/chats/restrict_chat_member.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/chats/set_administrator_title.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/chats/set_chat_description.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/chats/set_chat_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/chats/set_chat_photo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/chats/set_chat_protected_content.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/chats/set_chat_title.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/chats/set_chat_username.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/chats/set_send_as_chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/chats/set_slow_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/chats/unarchive_chats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/chats/unban_chat_member.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/chats/unhide_general_topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/chats/unpin_all_chat_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/chats/unpin_chat_message.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:29:00.889118 PyroFork-2.1.5/pyrogram/methods/contacts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/contacts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/contacts/add_contact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/contacts/delete_contacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/contacts/get_contacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/contacts/get_contacts_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/contacts/import_contacts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:29:00.893118 PyroFork-2.1.5/pyrogram/methods/decorators/
+-rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/decorators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/decorators/on_callback_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/decorators/on_chat_join_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/decorators/on_chat_member_updated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/decorators/on_chosen_inline_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/decorators/on_deleted_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/decorators/on_disconnect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/decorators/on_edited_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/decorators/on_inline_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/decorators/on_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/decorators/on_poll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/decorators/on_raw_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/decorators/on_user_status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:29:00.897118 PyroFork-2.1.5/pyrogram/methods/invite_links/
+-rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/invite_links/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/invite_links/approve_all_chat_join_requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/invite_links/approve_chat_join_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/invite_links/create_chat_invite_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/invite_links/decline_all_chat_join_requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/invite_links/decline_chat_join_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/invite_links/delete_chat_admin_invite_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/invite_links/delete_chat_invite_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3533 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/invite_links/edit_chat_invite_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/invite_links/export_chat_invite_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/invite_links/get_chat_admin_invite_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/invite_links/get_chat_admin_invite_links_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/invite_links/get_chat_admins_with_invite_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/invite_links/get_chat_invite_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/invite_links/get_chat_invite_link_joiners.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/invite_links/get_chat_invite_link_joiners_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/invite_links/get_chat_join_requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/invite_links/revoke_chat_invite_link.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:29:00.901118 PyroFork-2.1.5/pyrogram/methods/messages/
+-rw-r--r--   0 runner    (1001) docker     (123)     3921 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/messages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5963 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/messages/copy_media_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5423 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/messages/copy_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/messages/delete_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7530 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/messages/download_media.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/messages/edit_inline_caption.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10375 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/messages/edit_inline_media.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/messages/edit_inline_reply_markup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/messages/edit_inline_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/messages/edit_message_caption.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13022 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/messages/edit_message_media.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/messages/edit_message_reply_markup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/messages/edit_message_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4824 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/messages/forward_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/messages/get_chat_history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/messages/get_chat_history_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/messages/get_custom_emoji_stickers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/messages/get_discussion_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/messages/get_discussion_replies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/messages/get_discussion_replies_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/messages/get_media_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4741 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/messages/get_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/messages/inline_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/messages/read_chat_history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/messages/retract_vote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/messages/search_global.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/messages/search_global_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5349 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/messages/search_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/messages/search_messages_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12828 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/messages/send_animation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11362 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/messages/send_audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5723 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/messages/send_cached_media.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/messages/send_chat_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5111 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/messages/send_contact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5085 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/messages/send_dice.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10712 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/messages/send_document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4820 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/messages/send_location.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20821 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/messages/send_media_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7509 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/messages/send_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9682 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/messages/send_photo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8315 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/messages/send_poll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/messages/send_reaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8582 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/messages/send_sticker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5641 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/messages/send_venue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12198 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/messages/send_video.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9556 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/messages/send_video_note.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9672 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/messages/send_voice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/messages/stop_poll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/messages/stream_media.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/messages/vote_poll.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:29:00.901118 PyroFork-2.1.5/pyrogram/methods/password/
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/password/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/password/change_cloud_password.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/password/enable_cloud_password.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/password/remove_cloud_password.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:29:00.901118 PyroFork-2.1.5/pyrogram/methods/stickers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/stickers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/stickers/add_sticker_to_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/stickers/create_sticker_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/stickers/get_sticker_set.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:29:00.905118 PyroFork-2.1.5/pyrogram/methods/users/
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/users/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/users/block_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/users/delete_profile_photos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4421 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/users/get_chat_photos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/users/get_chat_photos_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/users/get_common_chats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/users/get_default_emoji_statuses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/users/get_me.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2562 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/users/get_users.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/users/set_emoji_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/users/set_profile_photo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/users/set_username.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/users/unblock_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/users/update_profile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:29:00.905118 PyroFork-2.1.5/pyrogram/methods/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/utilities/add_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/utilities/compose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/utilities/export_session_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/utilities/idle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/utilities/remove_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/utilities/restart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/utilities/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/utilities/start.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/utilities/stop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/methods/utilities/stop_transmission.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61915 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/mime_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:29:00.905118 PyroFork-2.1.5/pyrogram/parser/
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8681 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/parser/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5770 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/parser/markdown.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/parser/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/parser/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:29:00.905118 PyroFork-2.1.5/pyrogram/raw/
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/raw/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:29:00.909118 PyroFork-2.1.5/pyrogram/raw/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/raw/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/raw/core/future_salt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/raw/core/future_salts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/raw/core/gzip_packed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/raw/core/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/raw/core/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/raw/core/msg_container.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:29:00.909118 PyroFork-2.1.5/pyrogram/raw/core/primitives/
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/raw/core/primitives/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/raw/core/primitives/bool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/raw/core/primitives/bytes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/raw/core/primitives/double.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/raw/core/primitives/int.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/raw/core/primitives/string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/raw/core/primitives/vector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/raw/core/tl_object.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:29:00.909118 PyroFork-2.1.5/pyrogram/session/
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/session/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10513 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/session/auth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:29:00.913118 PyroFork-2.1.5/pyrogram/session/internals/
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/session/internals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/session/internals/data_center.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/session/internals/msg_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/session/internals/msg_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/session/internals/seq_no.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12440 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/session/session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:29:00.913118 PyroFork-2.1.5/pyrogram/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/storage/file_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/storage/memory_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6412 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/storage/sqlite_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/storage/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/sync.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:29:00.917118 PyroFork-2.1.5/pyrogram/types/
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/types/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:29:00.917118 PyroFork-2.1.5/pyrogram/types/authorization/
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/types/authorization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/types/authorization/sent_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/types/authorization/terms_of_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:29:00.921118 PyroFork-2.1.5/pyrogram/types/bots_and_keyboards/
+-rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/types/bots_and_keyboards/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/types/bots_and_keyboards/bot_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/types/bots_and_keyboards/bot_command_scope.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/types/bots_and_keyboards/bot_command_scope_all_chat_administrators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/types/bots_and_keyboards/bot_command_scope_all_group_chats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/types/bots_and_keyboards/bot_command_scope_all_private_chats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/types/bots_and_keyboards/bot_command_scope_chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_administrators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_member.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/types/bots_and_keyboards/bot_command_scope_default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/types/bots_and_keyboards/callback_game.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12797 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/types/bots_and_keyboards/callback_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/types/bots_and_keyboards/force_reply.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/types/bots_and_keyboards/game_high_score.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8120 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/types/bots_and_keyboards/inline_keyboard_button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/types/bots_and_keyboards/inline_keyboard_markup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3514 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/types/bots_and_keyboards/keyboard_button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/types/bots_and_keyboards/login_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/types/bots_and_keyboards/menu_button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/types/bots_and_keyboards/menu_button_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/types/bots_and_keyboards/menu_button_default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/types/bots_and_keyboards/menu_button_web_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/types/bots_and_keyboards/reply_keyboard_markup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/types/bots_and_keyboards/reply_keyboard_remove.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/types/bots_and_keyboards/sent_web_app_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/types/bots_and_keyboards/web_app_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:29:00.925119 PyroFork-2.1.5/pyrogram/types/inline_mode/
+-rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/types/inline_mode/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/types/inline_mode/chosen_inline_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7298 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/types/inline_mode/inline_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/types/inline_mode/inline_query_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5776 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/types/inline_mode/inline_query_result_animation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3304 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/types/inline_mode/inline_query_result_article.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/types/inline_mode/inline_query_result_audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/types/inline_mode/inline_query_result_cached_animation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/types/inline_mode/inline_query_result_cached_audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/types/inline_mode/inline_query_result_cached_document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4312 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/types/inline_mode/inline_query_result_cached_photo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/types/inline_mode/inline_query_result_cached_sticker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4394 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/types/inline_mode/inline_query_result_cached_video.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4202 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/types/inline_mode/inline_query_result_cached_voice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/types/inline_mode/inline_query_result_contact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5240 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/types/inline_mode/inline_query_result_document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/types/inline_mode/inline_query_result_location.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5261 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/types/inline_mode/inline_query_result_photo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/types/inline_mode/inline_query_result_venue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5474 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/types/inline_mode/inline_query_result_video.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4360 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/types/inline_mode/inline_query_result_voice.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:29:00.925119 PyroFork-2.1.5/pyrogram/types/input_media/
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/types/input_media/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/types/input_media/input_media.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/types/input_media/input_media_animation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/types/input_media/input_media_audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/types/input_media/input_media_document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/types/input_media/input_media_photo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/types/input_media/input_media_video.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/types/input_media/input_phone_contact.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:29:00.929118 PyroFork-2.1.5/pyrogram/types/input_message_content/
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/types/input_message_content/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/types/input_message_content/input_message_content.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/types/input_message_content/input_text_message_content.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/types/list.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:29:00.933119 PyroFork-2.1.5/pyrogram/types/messages_and_media/
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/types/messages_and_media/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4044 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/types/messages_and_media/animation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4069 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/types/messages_and_media/audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/types/messages_and_media/contact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/types/messages_and_media/dice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/types/messages_and_media/document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/types/messages_and_media/game.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/types/messages_and_media/location.py
+-rw-r--r--   0 runner    (1001) docker     (123)   152296 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/types/messages_and_media/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4352 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/types/messages_and_media/message_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/types/messages_and_media/message_reactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4309 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/types/messages_and_media/photo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7037 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/types/messages_and_media/poll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/types/messages_and_media/poll_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/types/messages_and_media/reaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6909 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/types/messages_and_media/sticker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/types/messages_and_media/stickerset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/types/messages_and_media/stripped_thumbnail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/types/messages_and_media/thumbnail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/types/messages_and_media/venue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4389 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/types/messages_and_media/video.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3601 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/types/messages_and_media/video_note.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/types/messages_and_media/voice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/types/messages_and_media/web_app_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6351 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/types/messages_and_media/web_page.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3862 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/types/object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/types/update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:29:00.937119 PyroFork-2.1.5/pyrogram/types/user_and_chats/
+-rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/types/user_and_chats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33942 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/types/user_and_chats/chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/types/user_and_chats/chat_admin_with_invite_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22023 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/types/user_and_chats/chat_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5514 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/types/user_and_chats/chat_event_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4579 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/types/user_and_chats/chat_invite_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/types/user_and_chats/chat_join_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/types/user_and_chats/chat_joined_by_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/types/user_and_chats/chat_joiner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9444 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/types/user_and_chats/chat_member.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3674 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/types/user_and_chats/chat_member_updated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/types/user_and_chats/chat_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3967 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/types/user_and_chats/chat_photo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/types/user_and_chats/chat_preview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5300 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/types/user_and_chats/chat_privileges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/types/user_and_chats/chat_reactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/types/user_and_chats/dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/types/user_and_chats/emoji_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4970 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/types/user_and_chats/forum_topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/types/user_and_chats/forum_topic_closed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/types/user_and_chats/forum_topic_created.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/types/user_and_chats/forum_topic_edited.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/types/user_and_chats/forum_topic_reopened.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/types/user_and_chats/general_forum_topic_hidden.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/types/user_and_chats/general_forum_topic_unhidden.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/types/user_and_chats/invite_link_importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/types/user_and_chats/peer_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/types/user_and_chats/peer_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/types/user_and_chats/restriction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13045 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/types/user_and_chats/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/types/user_and_chats/username.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/types/user_and_chats/video_chat_ended.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/types/user_and_chats/video_chat_members_invited.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/types/user_and_chats/video_chat_scheduled.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/types/user_and_chats/video_chat_started.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10911 2023-04-10 15:28:46.000000 PyroFork-2.1.5/pyrogram/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-10 15:28:46.000000 PyroFork-2.1.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 15:29:00.941119 PyroFork-2.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3555 2023-04-10 15:28:46.000000 PyroFork-2.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:29:00.937119 PyroFork-2.1.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-04-10 15:28:46.000000 PyroFork-2.1.5/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:29:00.937119 PyroFork-2.1.5/tests/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-04-10 15:28:46.000000 PyroFork-2.1.5/tests/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-04-10 15:28:46.000000 PyroFork-2.1.5/tests/filters/test_command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:29:00.941119 PyroFork-2.1.5/tests/parser/
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-04-10 15:28:46.000000 PyroFork-2.1.5/tests/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6264 2023-04-10 15:28:46.000000 PyroFork-2.1.5/tests/parser/test_html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8208 2023-04-10 15:28:46.000000 PyroFork-2.1.5/tests/test_file_id.py
```

### Comparing `PyroFork-2.1.4.dev202303203721/COPYING` & `PyroFork-2.1.5/COPYING`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/COPYING.lesser` & `PyroFork-2.1.5/COPYING.lesser`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/NOTICE` & `PyroFork-2.1.5/NOTICE`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/PKG-INFO` & `PyroFork-2.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyroFork
-Version: 2.1.4.dev202303203721
+Version: 2.1.5
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
@@ -1,14 +1,14 @@
-Metadata-Version: 2.1 Name: PyroFork Version: 2.1.4.dev202303203721 Summary:
-Elegant, modern and asynchronous Telegram MTProto API framework in Python for
-users and bots Home-page: https://github.com/Mayuri-Chan/pyrofork Download-URL:
-https://github.com/Mayuri-Chan/pyrofork/releases/latest Author: wulan17 Author-
-email: mayuri@mayuri.my.id License: LGPLv3 Project-URL: Tracker, https://
-github.com/Mayuri-Chan/pyrofork/issues Project-URL: Source, https://github.com/
-Mayuri-Chan/pyrofork Project-URL: Documentation, https://pyrofork.mayuri.my.id
+Metadata-Version: 2.1 Name: PyroFork Version: 2.1.5 Summary: Elegant, modern
+and asynchronous Telegram MTProto API framework in Python for users and bots
+Home-page: https://github.com/Mayuri-Chan/pyrofork Download-URL: https://
+github.com/Mayuri-Chan/pyrofork/releases/latest Author: wulan17 Author-email:
+mayuri@mayuri.my.id License: LGPLv3 Project-URL: Tracker, https://github.com/
+Mayuri-Chan/pyrofork/issues Project-URL: Source, https://github.com/Mayuri-
+Chan/pyrofork Project-URL: Documentation, https://pyrofork.mayuri.my.id
 Keywords: telegram chat messenger mtproto api client library python Classifier:
 Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
 Developers Classifier: Natural Language :: English Classifier: License :: OSI
 Approved :: GNU Lesser General Public License v3 (LGPLv3) Classifier: Operating
 System :: OS Independent Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
```

### Comparing `PyroFork-2.1.4.dev202303203721/PyroFork.egg-info/PKG-INFO` & `PyroFork-2.1.5/PyroFork.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyroFork
-Version: 2.1.4.dev202303203721
+Version: 2.1.5
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
@@ -1,14 +1,14 @@
-Metadata-Version: 2.1 Name: PyroFork Version: 2.1.4.dev202303203721 Summary:
-Elegant, modern and asynchronous Telegram MTProto API framework in Python for
-users and bots Home-page: https://github.com/Mayuri-Chan/pyrofork Download-URL:
-https://github.com/Mayuri-Chan/pyrofork/releases/latest Author: wulan17 Author-
-email: mayuri@mayuri.my.id License: LGPLv3 Project-URL: Tracker, https://
-github.com/Mayuri-Chan/pyrofork/issues Project-URL: Source, https://github.com/
-Mayuri-Chan/pyrofork Project-URL: Documentation, https://pyrofork.mayuri.my.id
+Metadata-Version: 2.1 Name: PyroFork Version: 2.1.5 Summary: Elegant, modern
+and asynchronous Telegram MTProto API framework in Python for users and bots
+Home-page: https://github.com/Mayuri-Chan/pyrofork Download-URL: https://
+github.com/Mayuri-Chan/pyrofork/releases/latest Author: wulan17 Author-email:
+mayuri@mayuri.my.id License: LGPLv3 Project-URL: Tracker, https://github.com/
+Mayuri-Chan/pyrofork/issues Project-URL: Source, https://github.com/Mayuri-
+Chan/pyrofork Project-URL: Documentation, https://pyrofork.mayuri.my.id
 Keywords: telegram chat messenger mtproto api client library python Classifier:
 Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
 Developers Classifier: Natural Language :: English Classifier: License :: OSI
 Approved :: GNU Lesser General Public License v3 (LGPLv3) Classifier: Operating
 System :: OS Independent Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
```

### Comparing `PyroFork-2.1.4.dev202303203721/PyroFork.egg-info/SOURCES.txt` & `PyroFork-2.1.5/PyroFork.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -270,14 +270,18 @@
 pyrogram/methods/messages/stop_poll.py
 pyrogram/methods/messages/stream_media.py
 pyrogram/methods/messages/vote_poll.py
 pyrogram/methods/password/__init__.py
 pyrogram/methods/password/change_cloud_password.py
 pyrogram/methods/password/enable_cloud_password.py
 pyrogram/methods/password/remove_cloud_password.py
+pyrogram/methods/stickers/__init__.py
+pyrogram/methods/stickers/add_sticker_to_set.py
+pyrogram/methods/stickers/create_sticker_set.py
+pyrogram/methods/stickers/get_sticker_set.py
 pyrogram/methods/users/__init__.py
 pyrogram/methods/users/block_user.py
 pyrogram/methods/users/delete_profile_photos.py
 pyrogram/methods/users/get_chat_photos.py
 pyrogram/methods/users/get_chat_photos_count.py
 pyrogram/methods/users/get_common_chats.py
 pyrogram/methods/users/get_default_emoji_statuses.py
@@ -410,14 +414,15 @@
 pyrogram/types/messages_and_media/message_entity.py
 pyrogram/types/messages_and_media/message_reactions.py
 pyrogram/types/messages_and_media/photo.py
 pyrogram/types/messages_and_media/poll.py
 pyrogram/types/messages_and_media/poll_option.py
 pyrogram/types/messages_and_media/reaction.py
 pyrogram/types/messages_and_media/sticker.py
+pyrogram/types/messages_and_media/stickerset.py
 pyrogram/types/messages_and_media/stripped_thumbnail.py
 pyrogram/types/messages_and_media/thumbnail.py
 pyrogram/types/messages_and_media/venue.py
 pyrogram/types/messages_and_media/video.py
 pyrogram/types/messages_and_media/video_note.py
 pyrogram/types/messages_and_media/voice.py
 pyrogram/types/messages_and_media/web_app_data.py
@@ -448,14 +453,15 @@
 pyrogram/types/user_and_chats/general_forum_topic_hidden.py
 pyrogram/types/user_and_chats/general_forum_topic_unhidden.py
 pyrogram/types/user_and_chats/invite_link_importer.py
 pyrogram/types/user_and_chats/peer_channel.py
 pyrogram/types/user_and_chats/peer_user.py
 pyrogram/types/user_and_chats/restriction.py
 pyrogram/types/user_and_chats/user.py
+pyrogram/types/user_and_chats/username.py
 pyrogram/types/user_and_chats/video_chat_ended.py
 pyrogram/types/user_and_chats/video_chat_members_invited.py
 pyrogram/types/user_and_chats/video_chat_scheduled.py
 pyrogram/types/user_and_chats/video_chat_started.py
 tests/__init__.py
 tests/test_file_id.py
 tests/filters/__init__.py
```

### Comparing `PyroFork-2.1.4.dev202303203721/README.md` & `PyroFork-2.1.5/README.md`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/compiler/__init__.py` & `PyroFork-2.1.5/compiler/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/compiler/api/__init__.py` & `PyroFork-2.1.5/compiler/api/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/compiler/api/compiler.py` & `PyroFork-2.1.5/compiler/api/compiler.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/compiler/api/source/auth_key.tl` & `PyroFork-2.1.5/compiler/api/source/auth_key.tl`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/compiler/api/source/main_api.tl` & `PyroFork-2.1.5/compiler/api/source/main_api.tl`

 * *Files 0% similar despite different names*

```diff
@@ -189,15 +189,15 @@
 messageActionInviteToGroupCall#502f92f7 call:InputGroupCall users:Vector<long> = MessageAction;
 messageActionSetMessagesTTL#3c134d7b flags:# period:int auto_setting_from:flags.0?long = MessageAction;
 messageActionGroupCallScheduled#b3a07661 call:InputGroupCall schedule_date:int = MessageAction;
 messageActionSetChatTheme#aa786345 emoticon:string = MessageAction;
 messageActionChatJoinedByRequest#ebbca3cb = MessageAction;
 messageActionWebViewDataSentMe#47dd8079 text:string data:string = MessageAction;
 messageActionWebViewDataSent#b4c38cb5 text:string = MessageAction;
-messageActionGiftPremium#aba0f5c6 currency:string amount:long months:int = MessageAction;
+messageActionGiftPremium#c83d6aec flags:# currency:string amount:long months:int cryptoCurrency:flags.0?string cryptoAmount:flags.0?long = MessageAction;
 messageActionTopicCreate#d999256 flags:# title:string icon_color:int icon_emoji_id:flags.0?long = MessageAction;
 messageActionTopicEdit#c0944820 flags:# title:flags.0?string icon_emoji_id:flags.1?long closed:flags.2?Bool hidden:flags.3?Bool = MessageAction;
 messageActionSuggestProfilePhoto#57de635e photo:Photo = MessageAction;
 messageActionRequestedPeer#fe77345d button_id:int peer:Peer = MessageAction;
 
 dialog#d58a08c6 flags:# pinned:flags.2?true unread_mark:flags.3?true peer:Peer top_message:int read_inbox_max_id:int read_outbox_max_id:int unread_count:int unread_mentions_count:int unread_reactions_count:int notify_settings:PeerNotifySettings pts:flags.0?int draft:flags.1?DraftMessage folder_id:flags.4?int ttl_period:flags.5?int = Dialog;
 dialogFolder#71bd134c flags:# pinned:flags.2?true folder:Folder peer:Peer top_message:int unread_muted_peers_count:int unread_unmuted_peers_count:int unread_muted_messages_count:int unread_unmuted_messages_count:int = Dialog;
@@ -735,15 +735,15 @@
 auth.codeTypeFragmentSms#6ed998c = auth.CodeType;
 
 auth.sentCodeTypeApp#3dbb5986 length:int = auth.SentCodeType;
 auth.sentCodeTypeSms#c000bba2 length:int = auth.SentCodeType;
 auth.sentCodeTypeCall#5353e5a7 length:int = auth.SentCodeType;
 auth.sentCodeTypeFlashCall#ab03c6d9 pattern:string = auth.SentCodeType;
 auth.sentCodeTypeMissedCall#82006484 prefix:string length:int = auth.SentCodeType;
-auth.sentCodeTypeEmailCode#5a159841 flags:# apple_signin_allowed:flags.0?true google_signin_allowed:flags.1?true email_pattern:string length:int next_phone_login_date:flags.2?int = auth.SentCodeType;
+auth.sentCodeTypeEmailCode#f450f59b flags:# apple_signin_allowed:flags.0?true google_signin_allowed:flags.1?true email_pattern:string length:int reset_available_period:flags.3?int reset_pending_date:flags.4?int = auth.SentCodeType;
 auth.sentCodeTypeSetUpEmailRequired#a5491dea flags:# apple_signin_allowed:flags.0?true google_signin_allowed:flags.1?true = auth.SentCodeType;
 auth.sentCodeTypeFragmentSms#d9565c39 url:string length:int = auth.SentCodeType;
 auth.sentCodeTypeFirebaseSms#e57b1432 flags:# nonce:flags.0?bytes receipt:flags.1?string push_timeout:flags.1?int length:int = auth.SentCodeType;
 
 messages.botCallbackAnswer#36585ea4 flags:# alert:flags.1?true has_url:flags.3?true native_ui:flags.4?true message:flags.0?string url:flags.2?string cache_time:int = messages.BotCallbackAnswer;
 
 messages.messageEditData#26b5dde6 flags:# caption:flags.0?true = messages.MessageEditData;
@@ -1553,14 +1553,15 @@
 auth.dropTempAuthKeys#8e48a188 except_auth_keys:Vector<long> = Bool;
 auth.exportLoginToken#b7e085fe api_id:int api_hash:string except_ids:Vector<long> = auth.LoginToken;
 auth.importLoginToken#95ac5ce4 token:bytes = auth.LoginToken;
 auth.acceptLoginToken#e894ad4d token:bytes = Authorization;
 auth.checkRecoveryPassword#d36bf79 code:string = Bool;
 auth.importWebTokenAuthorization#2db873a9 api_id:int api_hash:string web_auth_token:string = auth.Authorization;
 auth.requestFirebaseSms#89464b50 flags:# phone_number:string phone_code_hash:string safety_net_token:flags.0?string ios_push_secret:flags.1?string = Bool;
+auth.resetLoginEmail#7e960193 phone_number:string phone_code_hash:string = auth.SentCode;
 
 account.registerDevice#ec86017a flags:# no_muted:flags.0?true token_type:int token:string app_sandbox:Bool secret:bytes other_uids:Vector<long> = Bool;
 account.unregisterDevice#6a0d3206 token_type:int token:string other_uids:Vector<long> = Bool;
 account.updateNotifySettings#84be5b93 peer:InputNotifyPeer settings:InputPeerNotifySettings = Bool;
 account.getNotifySettings#12b3ad31 peer:InputNotifyPeer = PeerNotifySettings;
 account.resetNotifySettings#db7e1747 = Bool;
 account.updateProfile#78515775 flags:# first_name:flags.0?string last_name:flags.1?string about:flags.2?string = User;
@@ -2039,8 +2040,8 @@
 
 stats.getBroadcastStats#ab42441a flags:# dark:flags.0?true channel:InputChannel = stats.BroadcastStats;
 stats.loadAsyncGraph#621d5fa0 flags:# token:string x:flags.0?long = StatsGraph;
 stats.getMegagroupStats#dcdf8607 flags:# dark:flags.0?true channel:InputChannel = stats.MegagroupStats;
 stats.getMessagePublicForwards#5630281b channel:InputChannel msg_id:int offset_rate:int offset_peer:InputPeer offset_id:int limit:int = messages.Messages;
 stats.getMessageStats#b6e0a3f5 flags:# dark:flags.0?true channel:InputChannel msg_id:int = stats.MessageStats;
 
-// LAYER 155
+// LAYER 157
```

### Comparing `PyroFork-2.1.4.dev202303203721/compiler/api/source/sys_msgs.tl` & `PyroFork-2.1.5/compiler/api/source/sys_msgs.tl`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/compiler/api/template/combinator.txt` & `PyroFork-2.1.5/compiler/api/template/combinator.txt`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/compiler/api/template/type.txt` & `PyroFork-2.1.5/compiler/api/template/type.txt`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/compiler/docs/__init__.py` & `PyroFork-2.1.5/compiler/docs/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/compiler/docs/compiler.py` & `PyroFork-2.1.5/compiler/docs/compiler.py`

 * *Files 6% similar despite different names*

```diff
@@ -235,14 +235,24 @@
             set_slow_mode
             mark_chat_unread
             get_chat_event_log
             get_chat_online_count
             get_send_as_chats
             set_send_as_chat
             set_chat_protected_content
+            close_forum_topic
+            close_general_topic
+            create_forum_topic
+            delete_forum_topic
+            edit_forum_topic
+            edit_general_topic
+            hide_general_topic
+            reopen_forum_topic
+            reopen_general_topic
+            unhide_general_topic
         """,
         users="""
         Users
             get_me
             get_users
             get_chat_photos
             get_chat_photos_count
@@ -420,14 +430,20 @@
             VideoChatScheduled
             VideoChatStarted
             VideoChatEnded
             VideoChatMembersInvited
             WebAppData
             MessageReactions
             ChatReactions
+            ForumTopicCreated
+            ForumTopicEdited
+            ForumTopicClosed
+            ForumTopicReopened
+            GeneralTopicHidden
+            GeneralTopicUnhidden
         """,
         bot_keyboards="""
         Bot keyboards
             ReplyKeyboardMarkup
             KeyboardButton
             ReplyKeyboardRemove
             InlineKeyboardMarkup
```

### Comparing `PyroFork-2.1.4.dev202303203721/compiler/errors/__init__.py` & `PyroFork-2.1.5/compiler/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/compiler/errors/compiler.py` & `PyroFork-2.1.5/compiler/errors/compiler.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/compiler/errors/sort.py` & `PyroFork-2.1.5/compiler/errors/sort.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/compiler/errors/source/400_BAD_REQUEST.tsv` & `PyroFork-2.1.5/compiler/errors/source/400_BAD_REQUEST.tsv`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/compiler/errors/source/401_UNAUTHORIZED.tsv` & `PyroFork-2.1.5/compiler/errors/source/401_UNAUTHORIZED.tsv`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/compiler/errors/source/403_FORBIDDEN.tsv` & `PyroFork-2.1.5/compiler/errors/source/403_FORBIDDEN.tsv`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/compiler/errors/source/406_NOT_ACCEPTABLE.tsv` & `PyroFork-2.1.5/compiler/errors/source/406_NOT_ACCEPTABLE.tsv`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/compiler/errors/source/500_INTERNAL_SERVER_ERROR.tsv` & `PyroFork-2.1.5/compiler/errors/source/500_INTERNAL_SERVER_ERROR.tsv`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/__init__.py` & `PyroFork-2.1.5/pyrogram/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
-__fork_name__ = "PyroFork-dev"
-__version__ = "2.1.4.dev202303203721"
+__fork_name__ = "PyroFork"
+__version__ = "2.1.5"
 __license__ = "GNU Lesser General Public License v3.0 (LGPL-3.0)"
 __copyright__ = "Copyright (C) 2017-present Dan <https://github.com/delivrance>"
 
 from concurrent.futures.thread import ThreadPoolExecutor
 
 
 class StopTransmission(Exception):
```

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/client.py` & `PyroFork-2.1.5/pyrogram/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 import logging
 import os
 import platform
 import re
 import shutil
 import sys
 from concurrent.futures.thread import ThreadPoolExecutor
-from datetime import datetime, timedelta
 from hashlib import sha256
 from importlib import import_module
 from io import StringIO, BytesIO
 from mimetypes import MimeTypes
 from pathlib import Path
 from typing import Union, List, Optional, Callable, AsyncGenerator
 
@@ -40,15 +39,15 @@
 from pyrogram import raw
 from pyrogram import utils
 from pyrogram.crypto import aes
 from pyrogram.errors import CDNFileHashMismatch
 from pyrogram.errors import (
     SessionPasswordNeeded,
     VolumeLocNotFound, ChannelPrivate,
-    BadRequest
+    AuthBytesInvalid, BadRequest
 )
 from pyrogram.handlers.handler import Handler
 from pyrogram.methods import Methods
 from pyrogram.session import Auth, Session
 from pyrogram.storage import FileStorage, MemoryStorage
 from pyrogram.types import User, TermsOfService
 from pyrogram.utils import ainput
@@ -168,38 +167,28 @@
             of time. Flood wait exceptions requiring higher waiting times will be raised.
             Defaults to 10 seconds.
 
         hide_password (``bool``, *optional*):
             Pass True to hide the password when typing it during the login.
             Defaults to False, because ``getpass`` (the library used) is known to be problematic in some
             terminal environments.
-
-        max_concurrent_transmissions (``bool``, *optional*):
-            Set the maximum amount of concurrent transmissions (uploads & downloads).
-            A value that is too high may result in network related issues.
-            Defaults to 1.
     """
 
     APP_VERSION = f"Pyrogram {__version__}"
     DEVICE_MODEL = f"{platform.python_implementation()} {platform.python_version()}"
     SYSTEM_VERSION = f"{platform.system()} {platform.release()}"
 
     LANG_CODE = "en"
 
     PARENT_DIR = Path(sys.argv[0]).parent
 
     INVITE_LINK_RE = re.compile(r"^(?:https?://)?(?:www\.)?(?:t(?:elegram)?\.(?:org|me|dog)/(?:joinchat/|\+))([\w-]+)$")
     WORKERS = min(32, (os.cpu_count() or 0) + 4)  # os.cpu_count() can be None
     WORKDIR = PARENT_DIR
 
-    # Interval of seconds in which the updates watchdog will kick in
-    UPDATES_WATCHDOG_INTERVAL = 5 * 60
-
-    MAX_CONCURRENT_TRANSMISSIONS = 1
-
     mimetypes = MimeTypes()
     mimetypes.readfp(StringIO(mime_types))
 
     def __init__(
         self,
         name: str,
         api_id: Union[int, str] = None,
@@ -220,26 +209,25 @@
         workers: int = WORKERS,
         workdir: str = WORKDIR,
         plugins: dict = None,
         parse_mode: "enums.ParseMode" = enums.ParseMode.DEFAULT,
         no_updates: bool = None,
         takeout: bool = None,
         sleep_threshold: int = Session.SLEEP_THRESHOLD,
-        hide_password: bool = False,
-        max_concurrent_transmissions: int = MAX_CONCURRENT_TRANSMISSIONS
+        hide_password: bool = False
     ):
         super().__init__()
 
         self.name = name
         self.api_id = int(api_id) if api_id else None
         self.api_hash = api_hash
         self.app_version = app_version
         self.device_model = device_model
         self.system_version = system_version
-        self.lang_code = lang_code.lower()
+        self.lang_code = lang_code
         self.ipv6 = ipv6
         self.proxy = proxy
         self.test_mode = test_mode
         self.bot_token = bot_token
         self.session_string = session_string
         self.in_memory = in_memory
         self.phone_number = phone_number
@@ -249,15 +237,14 @@
         self.workdir = Path(workdir)
         self.plugins = plugins
         self.parse_mode = parse_mode
         self.no_updates = no_updates
         self.takeout = takeout
         self.sleep_threshold = sleep_threshold
         self.hide_password = hide_password
-        self.max_concurrent_transmissions = max_concurrent_transmissions
 
         self.executor = ThreadPoolExecutor(self.workers, thread_name_prefix="Handler")
 
         if self.session_string:
             self.storage = MemoryStorage(self.name, self.session_string)
         elif self.in_memory:
             self.storage = MemoryStorage(self.name)
@@ -271,35 +258,25 @@
         self.parser = Parser(self)
 
         self.session = None
 
         self.media_sessions = {}
         self.media_sessions_lock = asyncio.Lock()
 
-        self.save_file_semaphore = asyncio.Semaphore(self.max_concurrent_transmissions)
-        self.get_file_semaphore = asyncio.Semaphore(self.max_concurrent_transmissions)
-
         self.is_connected = None
         self.is_initialized = None
 
         self.takeout_id = None
 
         self.disconnect_handler = None
 
         self.me: Optional[User] = None
 
         self.message_cache = Cache(10000)
 
-        # Sometimes, for some reason, the server will stop sending updates and will only respond to pings.
-        # This watchdog will invoke updates.GetState in order to wake up the server and enable it sending updates again
-        # after some idle time has been detected.
-        self.updates_watchdog_task = None
-        self.updates_watchdog_event = asyncio.Event()
-        self.last_update_time = datetime.now()
-
         self.loop = asyncio.get_event_loop()
 
     def __enter__(self):
         return self.start()
 
     def __exit__(self, *args):
         try:
@@ -312,26 +289,14 @@
 
     async def __aexit__(self, *args):
         try:
             await self.stop()
         except ConnectionError:
             pass
 
-    async def updates_watchdog(self):
-        while True:
-            try:
-                await asyncio.wait_for(self.updates_watchdog_event.wait(), self.UPDATES_WATCHDOG_INTERVAL)
-            except asyncio.TimeoutError:
-                pass
-            else:
-                break
-
-            if datetime.now() - self.last_update_time > timedelta(seconds=self.UPDATES_WATCHDOG_INTERVAL):
-                await self.invoke(raw.functions.updates.GetState())
-
     async def authorize(self) -> User:
         if self.bot_token:
             return await self.sign_in_bot(self.bot_token)
 
         print(f"Welcome to Pyrogram (version {__version__})")
         print(f"Pyrogram is free software and comes with ABSOLUTELY NO WARRANTY. Licensed\n"
               f"under the terms of the {__license__}.\n")
@@ -405,15 +370,15 @@
                                     recovery_code = await ainput("Enter recovery code: ")
 
                                     try:
                                         return await self.recover_password(recovery_code)
                                     except BadRequest as e:
                                         print(e.MESSAGE)
                                     except Exception as e:
-                                        log.exception(e)
+                                        log.error(e, exc_info=True)
                                         raise
                             else:
                                 self.password = None
                         else:
                             return await self.check_password(self.password)
                     except BadRequest as e:
                         print(e.MESSAGE)
@@ -529,16 +494,14 @@
             parsed_peers.append((peer_id, access_hash, peer_type, username, phone_number))
 
         await self.storage.update_peers(parsed_peers)
 
         return is_min
 
     async def handle_updates(self, updates):
-        self.last_update_time = datetime.now()
-
         if isinstance(updates, (raw.types.Updates, raw.types.UpdatesCombined)):
             is_min = any((
                 await self.fetch_peers(updates.users),
                 await self.fetch_peers(updates.chats),
             ))
 
             users = {u.id: u for u in updates.users}
@@ -705,19 +668,19 @@
                 for path, handlers in include:
                     module_path = root + "." + path
                     warn_non_existent_functions = True
 
                     try:
                         module = import_module(module_path)
                     except ImportError:
-                        log.warning('[%s] [LOAD] Ignoring non-existent module "%s"', self.name, module_path)
+                        log.warning(f'[{self.name}] [LOAD] Ignoring non-existent module "{module_path}"')
                         continue
 
                     if "__path__" in dir(module):
-                        log.warning('[%s] [LOAD] Ignoring namespace "%s"', self.name, module_path)
+                        log.warning(f'[{self.name}] [LOAD] Ignoring namespace "{module_path}"')
                         continue
 
                     if handlers is None:
                         handlers = vars(module).keys()
                         warn_non_existent_functions = False
 
                     for name in handlers:
@@ -740,19 +703,19 @@
                 for path, handlers in exclude:
                     module_path = root + "." + path
                     warn_non_existent_functions = True
 
                     try:
                         module = import_module(module_path)
                     except ImportError:
-                        log.warning('[%s] [UNLOAD] Ignoring non-existent module "%s"', self.name, module_path)
+                        log.warning(f'[{self.name}] [UNLOAD] Ignoring non-existent module "{module_path}"')
                         continue
 
                     if "__path__" in dir(module):
-                        log.warning('[%s] [UNLOAD] Ignoring namespace "%s"', self.name, module_path)
+                        log.warning(f'[{self.name}] [UNLOAD] Ignoring namespace "{module_path}"')
                         continue
 
                     if handlers is None:
                         handlers = vars(module).keys()
                         warn_non_existent_functions = False
 
                     for name in handlers:
@@ -771,15 +734,15 @@
                                 log.warning('[{}] [UNLOAD] Ignoring non-existent function "{}" from "{}"'.format(
                                     self.name, name, module_path))
 
             if count > 0:
                 log.info('[{}] Successfully loaded {} plugin{} from "{}"'.format(
                     self.name, count, "s" if count > 1 else "", root))
             else:
-                log.warning('[%s] No plugin loaded from "%s"', self.name, root)
+                log.warning(f'[{self.name}] No plugin loaded from "{root}"')
 
     async def handle_download(self, packet):
         file_id, directory, file_name, in_memory, file_size, progress, progress_args = packet
 
         os.makedirs(directory, exist_ok=True) if not in_memory else None
         temp_file_path = os.path.abspath(re.sub("\\\\", "/", os.path.join(directory, file_name))) + ".temp"
         file = BytesIO() if in_memory else open(temp_file_path, "wb")
@@ -811,220 +774,234 @@
         file_id: FileId,
         file_size: int = 0,
         limit: int = 0,
         offset: int = 0,
         progress: Callable = None,
         progress_args: tuple = ()
     ) -> Optional[AsyncGenerator[bytes, None]]:
-        async with self.get_file_semaphore:
-            file_type = file_id.file_type
+        dc_id = file_id.dc_id
 
-            if file_type == FileType.CHAT_PHOTO:
-                if file_id.chat_id > 0:
-                    peer = raw.types.InputPeerUser(
-                        user_id=file_id.chat_id,
-                        access_hash=file_id.chat_access_hash
+        async with self.media_sessions_lock:
+            session = self.media_sessions.get(dc_id, None)
+
+            if session is None:
+                if dc_id != await self.storage.dc_id():
+                    session = Session(
+                        self, dc_id, await Auth(self, dc_id, await self.storage.test_mode()).create(),
+                        await self.storage.test_mode(), is_media=True
                     )
-                else:
-                    if file_id.chat_access_hash == 0:
-                        peer = raw.types.InputPeerChat(
-                            chat_id=-file_id.chat_id
+                    await session.start()
+
+                    for _ in range(3):
+                        exported_auth = await self.invoke(
+                            raw.functions.auth.ExportAuthorization(
+                                dc_id=dc_id
+                            )
                         )
+
+                        try:
+                            await session.invoke(
+                                raw.functions.auth.ImportAuthorization(
+                                    id=exported_auth.id,
+                                    bytes=exported_auth.bytes
+                                )
+                            )
+                        except AuthBytesInvalid:
+                            continue
+                        else:
+                            break
                     else:
-                        peer = raw.types.InputPeerChannel(
-                            channel_id=utils.get_channel_id(file_id.chat_id),
-                            access_hash=file_id.chat_access_hash
-                        )
+                        await session.stop()
+                        raise AuthBytesInvalid
+                else:
+                    session = Session(
+                        self, dc_id, await self.storage.auth_key(),
+                        await self.storage.test_mode(), is_media=True
+                    )
+                    await session.start()
 
-                location = raw.types.InputPeerPhotoFileLocation(
-                    peer=peer,
-                    photo_id=file_id.media_id,
-                    big=file_id.thumbnail_source == ThumbnailSource.CHAT_PHOTO_BIG
-                )
-            elif file_type == FileType.PHOTO:
-                location = raw.types.InputPhotoFileLocation(
-                    id=file_id.media_id,
-                    access_hash=file_id.access_hash,
-                    file_reference=file_id.file_reference,
-                    thumb_size=file_id.thumbnail_size
+                self.media_sessions[dc_id] = session
+
+        file_type = file_id.file_type
+
+        if file_type == FileType.CHAT_PHOTO:
+            if file_id.chat_id > 0:
+                peer = raw.types.InputPeerUser(
+                    user_id=file_id.chat_id,
+                    access_hash=file_id.chat_access_hash
                 )
             else:
-                location = raw.types.InputDocumentFileLocation(
-                    id=file_id.media_id,
-                    access_hash=file_id.access_hash,
-                    file_reference=file_id.file_reference,
-                    thumb_size=file_id.thumbnail_size
-                )
+                if file_id.chat_access_hash == 0:
+                    peer = raw.types.InputPeerChat(
+                        chat_id=-file_id.chat_id
+                    )
+                else:
+                    peer = raw.types.InputPeerChannel(
+                        channel_id=utils.get_channel_id(file_id.chat_id),
+                        access_hash=file_id.chat_access_hash
+                    )
+
+            location = raw.types.InputPeerPhotoFileLocation(
+                peer=peer,
+                photo_id=file_id.media_id,
+                big=file_id.thumbnail_source == ThumbnailSource.CHAT_PHOTO_BIG
+            )
+        elif file_type == FileType.PHOTO:
+            location = raw.types.InputPhotoFileLocation(
+                id=file_id.media_id,
+                access_hash=file_id.access_hash,
+                file_reference=file_id.file_reference,
+                thumb_size=file_id.thumbnail_size
+            )
+        else:
+            location = raw.types.InputDocumentFileLocation(
+                id=file_id.media_id,
+                access_hash=file_id.access_hash,
+                file_reference=file_id.file_reference,
+                thumb_size=file_id.thumbnail_size
+            )
 
-            current = 0
-            total = abs(limit) or (1 << 31) - 1
-            chunk_size = 1024 * 1024
-            offset_bytes = abs(offset) * chunk_size
-
-            dc_id = file_id.dc_id
-
-            session = Session(
-                self, dc_id,
-                await Auth(self, dc_id, await self.storage.test_mode()).create()
-                if dc_id != await self.storage.dc_id()
-                else await self.storage.auth_key(),
-                await self.storage.test_mode(),
-                is_media=True
+        current = 0
+        total = abs(limit) or (1 << 31) - 1
+        chunk_size = 1024 * 1024
+        offset_bytes = abs(offset) * chunk_size
+
+        try:
+            r = await session.invoke(
+                raw.functions.upload.GetFile(
+                    location=location,
+                    offset=offset_bytes,
+                    limit=chunk_size
+                ),
+                sleep_threshold=30
             )
 
-            try:
-                await session.start()
+            if isinstance(r, raw.types.upload.File):
+                while True:
+                    chunk = r.bytes
 
-                if dc_id != await self.storage.dc_id():
-                    exported_auth = await self.invoke(
-                        raw.functions.auth.ExportAuthorization(
-                            dc_id=dc_id
+                    yield chunk
+
+                    current += 1
+                    offset_bytes += chunk_size
+
+                    if progress:
+                        func = functools.partial(
+                            progress,
+                            min(offset_bytes, file_size)
+                            if file_size != 0
+                            else offset_bytes,
+                            file_size,
+                            *progress_args
                         )
+
+                        if inspect.iscoroutinefunction(progress):
+                            await func()
+                        else:
+                            await self.loop.run_in_executor(self.executor, func)
+
+                    if len(chunk) < chunk_size or current >= total:
+                        break
+
+                    r = await session.invoke(
+                        raw.functions.upload.GetFile(
+                            location=location,
+                            offset=offset_bytes,
+                            limit=chunk_size
+                        ),
+                        sleep_threshold=30
                     )
 
-                    await session.invoke(
-                        raw.functions.auth.ImportAuthorization(
-                            id=exported_auth.id,
-                            bytes=exported_auth.bytes
+            elif isinstance(r, raw.types.upload.FileCdnRedirect):
+                async with self.media_sessions_lock:
+                    cdn_session = self.media_sessions.get(r.dc_id, None)
+
+                    if cdn_session is None:
+                        cdn_session = Session(
+                            self, r.dc_id, await Auth(self, r.dc_id, await self.storage.test_mode()).create(),
+                            await self.storage.test_mode(), is_media=True, is_cdn=True
                         )
-                    )
 
-                r = await session.invoke(
-                    raw.functions.upload.GetFile(
-                        location=location,
-                        offset=offset_bytes,
-                        limit=chunk_size
-                    ),
-                    sleep_threshold=30
-                )
+                        await cdn_session.start()
 
-                if isinstance(r, raw.types.upload.File):
+                        self.media_sessions[r.dc_id] = cdn_session
+
+                try:
                     while True:
-                        chunk = r.bytes
+                        r2 = await cdn_session.invoke(
+                            raw.functions.upload.GetCdnFile(
+                                file_token=r.file_token,
+                                offset=offset_bytes,
+                                limit=chunk_size
+                            )
+                        )
+
+                        if isinstance(r2, raw.types.upload.CdnFileReuploadNeeded):
+                            try:
+                                await session.invoke(
+                                    raw.functions.upload.ReuploadCdnFile(
+                                        file_token=r.file_token,
+                                        request_token=r2.request_token
+                                    )
+                                )
+                            except VolumeLocNotFound:
+                                break
+                            else:
+                                continue
 
-                        yield chunk
+                        chunk = r2.bytes
+
+                        # https://core.telegram.org/cdn#decrypting-files
+                        decrypted_chunk = aes.ctr256_decrypt(
+                            chunk,
+                            r.encryption_key,
+                            bytearray(
+                                r.encryption_iv[:-4]
+                                + (offset_bytes // 16).to_bytes(4, "big")
+                            )
+                        )
+
+                        hashes = await session.invoke(
+                            raw.functions.upload.GetCdnFileHashes(
+                                file_token=r.file_token,
+                                offset=offset_bytes
+                            )
+                        )
+
+                        # https://core.telegram.org/cdn#verifying-files
+                        for i, h in enumerate(hashes):
+                            cdn_chunk = decrypted_chunk[h.limit * i: h.limit * (i + 1)]
+                            CDNFileHashMismatch.check(h.hash == sha256(cdn_chunk).digest())
+
+                        yield decrypted_chunk
 
                         current += 1
                         offset_bytes += chunk_size
 
                         if progress:
                             func = functools.partial(
                                 progress,
-                                min(offset_bytes, file_size)
-                                if file_size != 0
-                                else offset_bytes,
+                                min(offset_bytes, file_size) if file_size != 0 else offset_bytes,
                                 file_size,
                                 *progress_args
                             )
 
                             if inspect.iscoroutinefunction(progress):
                                 await func()
                             else:
                                 await self.loop.run_in_executor(self.executor, func)
 
                         if len(chunk) < chunk_size or current >= total:
                             break
-
-                        r = await session.invoke(
-                            raw.functions.upload.GetFile(
-                                location=location,
-                                offset=offset_bytes,
-                                limit=chunk_size
-                            ),
-                            sleep_threshold=30
-                        )
-
-                elif isinstance(r, raw.types.upload.FileCdnRedirect):
-                    cdn_session = Session(
-                        self, r.dc_id, await Auth(self, r.dc_id, await self.storage.test_mode()).create(),
-                        await self.storage.test_mode(), is_media=True, is_cdn=True
-                    )
-
-                    try:
-                        await cdn_session.start()
-
-                        while True:
-                            r2 = await cdn_session.invoke(
-                                raw.functions.upload.GetCdnFile(
-                                    file_token=r.file_token,
-                                    offset=offset_bytes,
-                                    limit=chunk_size
-                                )
-                            )
-
-                            if isinstance(r2, raw.types.upload.CdnFileReuploadNeeded):
-                                try:
-                                    await session.invoke(
-                                        raw.functions.upload.ReuploadCdnFile(
-                                            file_token=r.file_token,
-                                            request_token=r2.request_token
-                                        )
-                                    )
-                                except VolumeLocNotFound:
-                                    break
-                                else:
-                                    continue
-
-                            chunk = r2.bytes
-
-                            # https://core.telegram.org/cdn#decrypting-files
-                            decrypted_chunk = aes.ctr256_decrypt(
-                                chunk,
-                                r.encryption_key,
-                                bytearray(
-                                    r.encryption_iv[:-4]
-                                    + (offset_bytes // 16).to_bytes(4, "big")
-                                )
-                            )
-
-                            hashes = await session.invoke(
-                                raw.functions.upload.GetCdnFileHashes(
-                                    file_token=r.file_token,
-                                    offset=offset_bytes
-                                )
-                            )
-
-                            # https://core.telegram.org/cdn#verifying-files
-                            for i, h in enumerate(hashes):
-                                cdn_chunk = decrypted_chunk[h.limit * i: h.limit * (i + 1)]
-                                CDNFileHashMismatch.check(
-                                    h.hash == sha256(cdn_chunk).digest(),
-                                    "h.hash == sha256(cdn_chunk).digest()"
-                                )
-
-                            yield decrypted_chunk
-
-                            current += 1
-                            offset_bytes += chunk_size
-
-                            if progress:
-                                func = functools.partial(
-                                    progress,
-                                    min(offset_bytes, file_size) if file_size != 0 else offset_bytes,
-                                    file_size,
-                                    *progress_args
-                                )
-
-                                if inspect.iscoroutinefunction(progress):
-                                    await func()
-                                else:
-                                    await self.loop.run_in_executor(self.executor, func)
-
-                            if len(chunk) < chunk_size or current >= total:
-                                break
-                    except Exception as e:
-                        raise e
-                    finally:
-                        await cdn_session.stop()
-            except pyrogram.StopTransmission:
-                raise
-            except Exception as e:
-                log.exception(e)
-            finally:
-                await session.stop()
+                except Exception as e:
+                    raise e
+        except pyrogram.StopTransmission:
+            raise
+        except Exception as e:
+            log.error(e, exc_info=True)
 
     def guess_mime_type(self, filename: str) -> Optional[str]:
         return self.mimetypes.guess_type(filename)[0]
 
     def guess_extension(self, mime_type: str) -> Optional[str]:
         return self.mimetypes.guess_extension(mime_type)
```

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/connection/__init__.py` & `PyroFork-2.1.5/pyrogram/connection/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/connection/connection.py` & `PyroFork-2.1.5/pyrogram/connection/connection.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,57 +16,71 @@
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
 import asyncio
 import logging
 from typing import Optional
 
-from .transport import TCP, TCPAbridged
+from .transport import *
 from ..session.internals import DataCenter
 
 log = logging.getLogger(__name__)
 
 
 class Connection:
-    MAX_CONNECTION_ATTEMPTS = 3
+    MAX_RETRIES = 3
 
-    def __init__(self, dc_id: int, test_mode: bool, ipv6: bool, proxy: dict, media: bool = False):
+    MODES = {
+        0: TCPFull,
+        1: TCPAbridged,
+        2: TCPIntermediate,
+        3: TCPAbridgedO,
+        4: TCPIntermediateO
+    }
+
+    def __init__(self, dc_id: int, test_mode: bool, ipv6: bool, proxy: dict, media: bool = False, mode: int = 3):
         self.dc_id = dc_id
         self.test_mode = test_mode
         self.ipv6 = ipv6
         self.proxy = proxy
         self.media = media
-
         self.address = DataCenter(dc_id, test_mode, ipv6, media)
-        self.protocol: TCP = None
+        self.mode = self.MODES.get(mode, TCPAbridged)
+
+        self.protocol = None  # type: TCP
 
     async def connect(self):
-        for i in range(Connection.MAX_CONNECTION_ATTEMPTS):
-            self.protocol = TCPAbridged(self.ipv6, self.proxy)
+        for i in range(Connection.MAX_RETRIES):
+            self.protocol = self.mode(self.ipv6, self.proxy)
 
             try:
                 log.info("Connecting...")
                 await self.protocol.connect(self.address)
             except OSError as e:
-                log.warning("Unable to connect due to network issues: %s", e)
-                await self.protocol.close()
+                log.warning(f"Unable to connect due to network issues: {e}")
+                self.protocol.close()
                 await asyncio.sleep(1)
             else:
-                log.info("Connected! %s DC%s%s - IPv%s",
-                         "Test" if self.test_mode else "Production",
-                         self.dc_id,
-                         " (media)" if self.media else "",
-                         "6" if self.ipv6 else "4")
+                log.info("Connected! {} DC{}{} - IPv{} - {}".format(
+                    "Test" if self.test_mode else "Production",
+                    self.dc_id,
+                    " (media)" if self.media else "",
+                    "6" if self.ipv6 else "4",
+                    self.mode.__name__,
+                ))
                 break
         else:
             log.warning("Connection failed! Trying again...")
-            raise ConnectionError
+            raise TimeoutError
 
-    async def close(self):
-        await self.protocol.close()
+    def close(self):
+        self.protocol.close()
         log.info("Disconnected")
 
     async def send(self, data: bytes):
-        await self.protocol.send(data)
+        try:
+            await self.protocol.send(data)
+        except Exception as e:
+            raise OSError(e)
 
     async def recv(self) -> Optional[bytes]:
         return await self.protocol.recv()
```

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/connection/transport/__init__.py` & `PyroFork-2.1.5/pyrogram/connection/transport/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/connection/transport/tcp/__init__.py` & `PyroFork-2.1.5/pyrogram/connection/transport/tcp/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/connection/transport/tcp/tcp.py` & `PyroFork-2.1.5/pyrogram/connection/transport/tcp/tcp.py`

 * *Files 17% similar despite different names*

```diff
@@ -16,35 +16,42 @@
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
 import asyncio
 import ipaddress
 import logging
 import socket
+import time
 from concurrent.futures import ThreadPoolExecutor
 
-import socks
+try:
+    import socks
+except ImportError as e:
+    e.msg = (
+        "PySocks is missing and Pyrogram can't run without. "
+        "Please install it using \"pip3 install pysocks\"."
+    )
+
+    raise e
 
 log = logging.getLogger(__name__)
 
 
 class TCP:
     TIMEOUT = 10
 
     def __init__(self, ipv6: bool, proxy: dict):
         self.socket = None
 
-        self.reader = None
-        self.writer = None
+        self.reader = None  # type: asyncio.StreamReader
+        self.writer = None  # type: asyncio.StreamWriter
 
         self.lock = asyncio.Lock()
         self.loop = asyncio.get_event_loop()
 
-        self.proxy = proxy
-
         if proxy:
             hostname = proxy.get("hostname")
 
             try:
                 ip_address = ipaddress.ip_address(hostname)
             except ValueError:
                 self.socket = socks.socksocket(socket.AF_INET)
@@ -58,54 +65,49 @@
                 proxy_type=getattr(socks, proxy.get("scheme").upper()),
                 addr=hostname,
                 port=proxy.get("port", None),
                 username=proxy.get("username", None),
                 password=proxy.get("password", None)
             )
 
-            self.socket.settimeout(TCP.TIMEOUT)
-
-            log.info("Using proxy %s", hostname)
+            log.info(f"Using proxy {hostname}")
         else:
-            self.socket = socket.socket(
+            self.socket = socks.socksocket(
                 socket.AF_INET6 if ipv6
                 else socket.AF_INET
             )
 
-            self.socket.setblocking(False)
+        self.socket.settimeout(TCP.TIMEOUT)
 
     async def connect(self, address: tuple):
-        if self.proxy:
-            with ThreadPoolExecutor(1) as executor:
-                await self.loop.run_in_executor(executor, self.socket.connect, address)
-        else:
-            try:
-                await asyncio.wait_for(asyncio.get_event_loop().sock_connect(self.socket, address), TCP.TIMEOUT)
-            except asyncio.TimeoutError:  # Re-raise as TimeoutError. asyncio.TimeoutError is deprecated in 3.11
-                raise TimeoutError("Connection timed out")
+        # The socket used by the whole logic is blocking and thus it blocks when connecting.
+        # Offload the task to a thread executor to avoid blocking the main event loop.
+        with ThreadPoolExecutor(1) as executor:
+            await self.loop.run_in_executor(executor, self.socket.connect, address)
 
         self.reader, self.writer = await asyncio.open_connection(sock=self.socket)
 
-    async def close(self):
+    def close(self):
         try:
-            if self.writer is not None:
-                self.writer.close()
-                await asyncio.wait_for(self.writer.wait_closed(), TCP.TIMEOUT)
-        except Exception as e:
-            log.warning("Close exception: %s %s", type(e).__name__, e)
+            self.writer.close()
+        except AttributeError:
+            try:
+                self.socket.shutdown(socket.SHUT_RDWR)
+            except OSError:
+                pass
+            finally:
+                # A tiny sleep placed here helps avoiding .recv(n) hanging until the timeout.
+                # This is a workaround that seems to fix the occasional delayed stop of a client.
+                time.sleep(0.001)
+                self.socket.close()
 
     async def send(self, data: bytes):
         async with self.lock:
-            try:
-                if self.writer is not None:
-                    self.writer.write(data)
-                    await self.writer.drain()
-            except Exception as e:
-                log.warning("Send exception: %s %s", type(e).__name__, e)
-                raise OSError(e)
+            self.writer.write(data)
+            await self.writer.drain()
 
     async def recv(self, length: int = 0):
         data = b""
 
         while len(data) < length:
             try:
                 chunk = await asyncio.wait_for(
```

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/connection/transport/tcp/tcp_abridged.py` & `PyroFork-2.1.5/pyrogram/connection/transport/tcp/tcp_abridged.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/connection/transport/tcp/tcp_abridged_o.py` & `PyroFork-2.1.5/pyrogram/connection/transport/tcp/tcp_abridged_o.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/connection/transport/tcp/tcp_full.py` & `PyroFork-2.1.5/pyrogram/connection/transport/tcp/tcp_full.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/connection/transport/tcp/tcp_intermediate.py` & `PyroFork-2.1.5/pyrogram/connection/transport/tcp/tcp_intermediate.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/connection/transport/tcp/tcp_intermediate_o.py` & `PyroFork-2.1.5/pyrogram/connection/transport/tcp/tcp_intermediate_o.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/crypto/__init__.py` & `PyroFork-2.1.5/pyrogram/crypto/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/crypto/aes.py` & `PyroFork-2.1.5/pyrogram/crypto/aes.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/crypto/mtproto.py` & `PyroFork-2.1.5/pyrogram/crypto/mtproto.py`

 * *Files 25% similar despite different names*

```diff
@@ -12,21 +12,26 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
+import bisect
 from hashlib import sha256
 from io import BytesIO
 from os import urandom
+from typing import List
 
 from pyrogram.errors import SecurityCheckMismatch
 from pyrogram.raw.core import Message, Long
 from . import aes
+from ..session.internals import MsgId
+
+STORED_MSG_IDS_MAX_SIZE = 1000 * 2
 
 
 def kdf(auth_key: bytes, msg_key: bytes, outgoing: bool) -> tuple:
     # https://core.telegram.org/mtproto/description#defining-aes-key-and-initialization-vector
     x = 0 if outgoing else 8
 
     sha256_a = sha256(msg_key + auth_key[x: x + 36]).digest()
@@ -50,25 +55,26 @@
     return auth_key_id + msg_key + aes.ige256_encrypt(data + padding, aes_key, aes_iv)
 
 
 def unpack(
     b: BytesIO,
     session_id: bytes,
     auth_key: bytes,
-    auth_key_id: bytes
+    auth_key_id: bytes,
+    stored_msg_ids: List[int]
 ) -> Message:
-    SecurityCheckMismatch.check(b.read(8) == auth_key_id, "b.read(8) == auth_key_id")
+    SecurityCheckMismatch.check(b.read(8) == auth_key_id)
 
     msg_key = b.read(16)
     aes_key, aes_iv = kdf(auth_key, msg_key, False)
     data = BytesIO(aes.ige256_decrypt(b.read(), aes_key, aes_iv))
     data.read(8)  # Salt
 
     # https://core.telegram.org/mtproto/security_guidelines#checking-session-id
-    SecurityCheckMismatch.check(data.read(8) == session_id, "data.read(8) == session_id")
+    SecurityCheckMismatch.check(data.read(8) == session_id)
 
     try:
         message = Message.read(data)
     except KeyError as e:
         if e.args[0] == 0:
             raise ConnectionError(f"Received empty data. Check your internet connection.")
 
@@ -78,23 +84,44 @@
         left = [[left[i:i + 8] for i in range(0, len(left), 8)] for left in left]
         left = "\n".join(" ".join(x for x in left) for left in left)
 
         raise ValueError(f"The server sent an unknown constructor: {hex(e.args[0])}\n{left}")
 
     # https://core.telegram.org/mtproto/security_guidelines#checking-sha256-hash-value-of-msg-key
     # 96 = 88 + 8 (incoming message)
-    SecurityCheckMismatch.check(
-        msg_key == sha256(auth_key[96:96 + 32] + data.getvalue()).digest()[8:24],
-        "msg_key == sha256(auth_key[96:96 + 32] + data.getvalue()).digest()[8:24]"
-    )
+    SecurityCheckMismatch.check(msg_key == sha256(auth_key[96:96 + 32] + data.getvalue()).digest()[8:24])
 
     # https://core.telegram.org/mtproto/security_guidelines#checking-message-length
     data.seek(32)  # Get to the payload, skip salt (8) + session_id (8) + msg_id (8) + seq_no (4) + length (4)
     payload = data.read()
     padding = payload[message.length:]
-    SecurityCheckMismatch.check(12 <= len(padding) <= 1024, "12 <= len(padding) <= 1024")
-    SecurityCheckMismatch.check(len(payload) % 4 == 0, "len(payload) % 4 == 0")
+    SecurityCheckMismatch.check(12 <= len(padding) <= 1024)
+    SecurityCheckMismatch.check(len(payload) % 4 == 0)
 
     # https://core.telegram.org/mtproto/security_guidelines#checking-msg-id
-    SecurityCheckMismatch.check(message.msg_id % 2 != 0, "message.msg_id % 2 != 0")
+    SecurityCheckMismatch.check(message.msg_id % 2 != 0)
+
+    if len(stored_msg_ids) > STORED_MSG_IDS_MAX_SIZE:
+        del stored_msg_ids[:STORED_MSG_IDS_MAX_SIZE // 2]
+
+    if stored_msg_ids:
+        # Ignored message: msg_id is lower than all of the stored values
+        if message.msg_id < stored_msg_ids[0]:
+            raise SecurityCheckMismatch
+
+        # Ignored message: msg_id is equal to any of the stored values
+        if message.msg_id in stored_msg_ids:
+            raise SecurityCheckMismatch
+
+        time_diff = (message.msg_id - MsgId()) / 2 ** 32
+
+        # Ignored message: msg_id belongs over 30 seconds in the future
+        if time_diff > 30:
+            raise SecurityCheckMismatch
+
+        # Ignored message: msg_id belongs over 300 seconds in the past
+        if time_diff < -300:
+            raise SecurityCheckMismatch
+
+    bisect.insort(stored_msg_ids, message.msg_id)
 
     return message
```

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/crypto/prime.py` & `PyroFork-2.1.5/pyrogram/crypto/prime.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/crypto/rsa.py` & `PyroFork-2.1.5/pyrogram/crypto/rsa.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/dispatcher.py` & `PyroFork-2.1.5/pyrogram/dispatcher.py`

 * *Files 4% similar despite different names*

```diff
@@ -147,28 +147,28 @@
             for i in range(self.client.workers):
                 self.locks_list.append(asyncio.Lock())
 
                 self.handler_worker_tasks.append(
                     self.loop.create_task(self.handler_worker(self.locks_list[-1]))
                 )
 
-            log.info("Started %s HandlerTasks", self.client.workers)
+            log.info(f"Started {self.client.workers} HandlerTasks")
 
     async def stop(self):
         if not self.client.no_updates:
             for i in range(self.client.workers):
                 self.updates_queue.put_nowait(None)
 
             for i in self.handler_worker_tasks:
                 await i
 
             self.handler_worker_tasks.clear()
             self.groups.clear()
 
-            log.info("Stopped %s HandlerTasks", self.client.workers)
+            log.info(f"Stopped {self.client.workers} HandlerTasks")
 
     def add_handler(self, handler, group: int):
         async def fn():
             for lock in self.locks_list:
                 await lock.acquire()
 
             try:
@@ -222,15 +222,15 @@
                             args = None
 
                             if isinstance(handler, handler_type):
                                 try:
                                     if await handler.check(self.client, parsed_update):
                                         args = (parsed_update,)
                                 except Exception as e:
-                                    log.exception(e)
+                                    log.error(e, exc_info=True)
                                     continue
 
                             elif isinstance(handler, RawUpdateHandler):
                                 args = (update, users, chats)
 
                             if args is None:
                                 continue
@@ -246,14 +246,14 @@
                                         *args
                                     )
                             except pyrogram.StopPropagation:
                                 raise
                             except pyrogram.ContinuePropagation:
                                 continue
                             except Exception as e:
-                                log.exception(e)
+                                log.error(e, exc_info=True)
 
                             break
             except pyrogram.StopPropagation:
                 pass
             except Exception as e:
-                log.exception(e)
+                log.error(e, exc_info=True)
```

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/emoji.py` & `PyroFork-2.1.5/pyrogram/emoji.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/enums/__init__.py` & `PyroFork-2.1.5/pyrogram/enums/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/enums/auto_name.py` & `PyroFork-2.1.5/pyrogram/enums/auto_name.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/enums/chat_action.py` & `PyroFork-2.1.5/pyrogram/enums/chat_action.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/enums/chat_event_action.py` & `PyroFork-2.1.5/pyrogram/enums/chat_event_action.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/enums/chat_member_status.py` & `PyroFork-2.1.5/pyrogram/enums/chat_member_status.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/enums/chat_members_filter.py` & `PyroFork-2.1.5/pyrogram/enums/chat_members_filter.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/enums/chat_type.py` & `PyroFork-2.1.5/pyrogram/enums/chat_type.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/enums/message_entity_type.py` & `PyroFork-2.1.5/pyrogram/enums/message_entity_type.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/enums/message_media_type.py` & `PyroFork-2.1.5/pyrogram/enums/message_media_type.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/enums/message_service_type.py` & `PyroFork-2.1.5/pyrogram/enums/message_service_type.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/enums/messages_filter.py` & `PyroFork-2.1.5/pyrogram/enums/messages_filter.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/enums/next_code_type.py` & `PyroFork-2.1.5/pyrogram/enums/next_code_type.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/enums/parse_mode.py` & `PyroFork-2.1.5/pyrogram/enums/parse_mode.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/enums/poll_type.py` & `PyroFork-2.1.5/pyrogram/enums/poll_type.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/enums/sent_code_type.py` & `PyroFork-2.1.5/pyrogram/enums/sent_code_type.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/enums/user_status.py` & `PyroFork-2.1.5/pyrogram/enums/user_status.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/errors/__init__.py` & `PyroFork-2.1.5/pyrogram/errors/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -41,25 +41,25 @@
         super().__init__(f"[{code}] {description}")
 
 
 class SecurityError(Exception):
     """Generic security error."""
 
     @classmethod
-    def check(cls, cond: bool, msg: str):
+    def check(cls, cond: bool):
         """Raises this exception if the condition is false"""
         if not cond:
-            raise cls(f"Check failed: {msg}")
+            raise cls
 
 
 class SecurityCheckMismatch(SecurityError):
     """Raised when a security check mismatch occurs."""
 
-    def __init__(self, msg: str = None):
-        super().__init__("A security check mismatch has occurred." if msg is None else msg)
+    def __init__(self):
+        super().__init__("A security check mismatch has occurred.")
 
 
 class CDNFileHashMismatch(SecurityError):
     """Raised when a CDN file hash mismatch occurs."""
 
-    def __init__(self, msg: str = None):
-        super().__init__("A CDN file hash mismatch has occurred." if msg is None else msg)
+    def __init__(self):
+        super().__init__("A CDN file hash mismatch has occurred.")
```

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/errors/rpc_error.py` & `PyroFork-2.1.5/pyrogram/errors/rpc_error.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/file_id.py` & `PyroFork-2.1.5/pyrogram/file_id.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/filters.py` & `PyroFork-2.1.5/pyrogram/filters.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/handlers/__init__.py` & `PyroFork-2.1.5/pyrogram/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/handlers/callback_query_handler.py` & `PyroFork-2.1.5/pyrogram/handlers/callback_query_handler.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/handlers/chat_join_request_handler.py` & `PyroFork-2.1.5/pyrogram/handlers/chat_join_request_handler.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/handlers/chat_member_updated_handler.py` & `PyroFork-2.1.5/pyrogram/handlers/chat_member_updated_handler.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/handlers/chosen_inline_result_handler.py` & `PyroFork-2.1.5/pyrogram/handlers/chosen_inline_result_handler.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/handlers/deleted_messages_handler.py` & `PyroFork-2.1.5/pyrogram/handlers/deleted_messages_handler.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/handlers/disconnect_handler.py` & `PyroFork-2.1.5/pyrogram/handlers/disconnect_handler.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/handlers/edited_message_handler.py` & `PyroFork-2.1.5/pyrogram/handlers/edited_message_handler.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/handlers/handler.py` & `PyroFork-2.1.5/pyrogram/handlers/handler.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/handlers/inline_query_handler.py` & `PyroFork-2.1.5/pyrogram/handlers/inline_query_handler.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/handlers/message_handler.py` & `PyroFork-2.1.5/pyrogram/handlers/message_handler.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/handlers/poll_handler.py` & `PyroFork-2.1.5/pyrogram/handlers/poll_handler.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/handlers/raw_update_handler.py` & `PyroFork-2.1.5/pyrogram/handlers/raw_update_handler.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/handlers/user_status_handler.py` & `PyroFork-2.1.5/pyrogram/handlers/user_status_handler.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/__init__.py` & `PyroFork-2.1.5/pyrogram/methods/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,25 +21,27 @@
 from .bots import Bots
 from .chats import Chats
 from .contacts import Contacts
 from .decorators import Decorators
 from .invite_links import InviteLinks
 from .messages import Messages
 from .password import Password
+from .stickers import Stickers
 from .users import Users
 from .utilities import Utilities
 
 
 class Methods(
     Advanced,
     Auth,
     Bots,
     Contacts,
     Password,
     Chats,
+    Stickers,
     Users,
     Messages,
     Decorators,
     Utilities,
     InviteLinks,
 ):
     pass
```

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/advanced/__init__.py` & `PyroFork-2.1.5/pyrogram/methods/advanced/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/advanced/invoke.py` & `PyroFork-2.1.5/pyrogram/methods/advanced/invoke.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/advanced/resolve_peer.py` & `PyroFork-2.1.5/pyrogram/methods/advanced/resolve_peer.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/advanced/save_file.py` & `PyroFork-2.1.5/pyrogram/methods/advanced/save_file.py`

 * *Files 4% similar despite different names*

```diff
@@ -90,137 +90,141 @@
 
         Returns:
             ``InputFile``: On success, the uploaded file is returned in form of an InputFile object.
 
         Raises:
             RPCError: In case of a Telegram RPC error.
         """
-        async with self.save_file_semaphore:
-            if path is None:
-                return None
-
-            async def worker(session):
-                while True:
-                    data = await queue.get()
-
-                    if data is None:
-                        return
-
-                    try:
-                        await session.invoke(data)
-                    except Exception as e:
-                        log.exception(e)
+        if path is None:
+            return None
 
-            part_size = 512 * 1024
-
-            if isinstance(path, (str, PurePath)):
-                fp = open(path, "rb")
-            elif isinstance(path, io.IOBase):
-                fp = path
-            else:
-                raise ValueError("Invalid file. Expected a file path as string or a binary (not text) file pointer")
-
-            file_name = getattr(fp, "name", "file.jpg")
-
-            fp.seek(0, os.SEEK_END)
-            file_size = fp.tell()
-            fp.seek(0)
-
-            if file_size == 0:
-                raise ValueError("File size equals to 0 B")
-
-            file_size_limit_mib = 4000 if self.me.is_premium else 2000
-
-            if file_size > file_size_limit_mib * 1024 * 1024:
-                raise ValueError(f"Can't upload files bigger than {file_size_limit_mib} MiB")
-
-            file_total_parts = int(math.ceil(file_size / part_size))
-            is_big = file_size > 10 * 1024 * 1024
-            workers_count = 4 if is_big else 1
-            is_missing_part = file_id is not None
-            file_id = file_id or self.rnd_id()
-            md5_sum = md5() if not is_big and not is_missing_part else None
-            session = Session(
+        async def worker(session):
+            while True:
+                data = await queue.get()
+
+                if data is None:
+                    return
+
+                try:
+                    await session.invoke(data)
+                except Exception as e:
+                    log.error(e)
+
+        part_size = 512 * 1024
+
+        if isinstance(path, (str, PurePath)):
+            fp = open(path, "rb")
+        elif isinstance(path, io.IOBase):
+            fp = path
+        else:
+            raise ValueError("Invalid file. Expected a file path as string or a binary (not text) file pointer")
+
+        file_name = getattr(fp, "name", "file.jpg")
+
+        fp.seek(0, os.SEEK_END)
+        file_size = fp.tell()
+        fp.seek(0)
+
+        if file_size == 0:
+            raise ValueError("File size equals to 0 B")
+
+        file_size_limit_mib = 4000 if self.me.is_premium else 2000
+
+        if file_size > file_size_limit_mib * 1024 * 1024:
+            raise ValueError(f"Can't upload files bigger than {file_size_limit_mib} MiB")
+
+        file_total_parts = int(math.ceil(file_size / part_size))
+        is_big = file_size > 10 * 1024 * 1024
+        pool_size = 3 if is_big else 1
+        workers_count = 4 if is_big else 1
+        is_missing_part = file_id is not None
+        file_id = file_id or self.rnd_id()
+        md5_sum = md5() if not is_big and not is_missing_part else None
+        pool = [
+            Session(
                 self, await self.storage.dc_id(), await self.storage.auth_key(),
                 await self.storage.test_mode(), is_media=True
-            )
-            workers = [self.loop.create_task(worker(session)) for _ in range(workers_count)]
-            queue = asyncio.Queue(1)
+            ) for _ in range(pool_size)
+        ]
+        workers = [self.loop.create_task(worker(session)) for session in pool for _ in range(workers_count)]
+        queue = asyncio.Queue(16)
 
-            try:
+        try:
+            for session in pool:
                 await session.start()
 
-                fp.seek(part_size * file_part)
-
-                while True:
-                    chunk = fp.read(part_size)
-
-                    if not chunk:
-                        if not is_big and not is_missing_part:
-                            md5_sum = "".join([hex(i)[2:].zfill(2) for i in md5_sum.digest()])
-                        break
-
-                    if is_big:
-                        rpc = raw.functions.upload.SaveBigFilePart(
-                            file_id=file_id,
-                            file_part=file_part,
-                            file_total_parts=file_total_parts,
-                            bytes=chunk
-                        )
-                    else:
-                        rpc = raw.functions.upload.SaveFilePart(
-                            file_id=file_id,
-                            file_part=file_part,
-                            bytes=chunk
-                        )
-
-                    await queue.put(rpc)
+            fp.seek(part_size * file_part)
 
-                    if is_missing_part:
-                        return
+            while True:
+                chunk = fp.read(part_size)
 
+                if not chunk:
                     if not is_big and not is_missing_part:
-                        md5_sum.update(chunk)
+                        md5_sum = "".join([hex(i)[2:].zfill(2) for i in md5_sum.digest()])
+                    break
 
-                    file_part += 1
-
-                    if progress:
-                        func = functools.partial(
-                            progress,
-                            min(file_part * part_size, file_size),
-                            file_size,
-                            *progress_args
-                        )
-
-                        if inspect.iscoroutinefunction(progress):
-                            await func()
-                        else:
-                            await self.loop.run_in_executor(self.executor, func)
-            except StopTransmission:
-                raise
-            except Exception as e:
-                log.exception(e)
-            else:
                 if is_big:
-                    return raw.types.InputFileBig(
-                        id=file_id,
-                        parts=file_total_parts,
-                        name=file_name,
-
+                    rpc = raw.functions.upload.SaveBigFilePart(
+                        file_id=file_id,
+                        file_part=file_part,
+                        file_total_parts=file_total_parts,
+                        bytes=chunk
                     )
                 else:
-                    return raw.types.InputFile(
-                        id=file_id,
-                        parts=file_total_parts,
-                        name=file_name,
-                        md5_checksum=md5_sum
+                    rpc = raw.functions.upload.SaveFilePart(
+                        file_id=file_id,
+                        file_part=file_part,
+                        bytes=chunk
                     )
-            finally:
-                for _ in workers:
-                    await queue.put(None)
 
-                await asyncio.gather(*workers)
+                await queue.put(rpc)
+
+                if is_missing_part:
+                    return
+
+                if not is_big and not is_missing_part:
+                    md5_sum.update(chunk)
+
+                file_part += 1
+
+                if progress:
+                    func = functools.partial(
+                        progress,
+                        min(file_part * part_size, file_size),
+                        file_size,
+                        *progress_args
+                    )
 
+                    if inspect.iscoroutinefunction(progress):
+                        await func()
+                    else:
+                        await self.loop.run_in_executor(self.executor, func)
+        except StopTransmission:
+            raise
+        except Exception as e:
+            log.error(e, exc_info=True)
+        else:
+            if is_big:
+                return raw.types.InputFileBig(
+                    id=file_id,
+                    parts=file_total_parts,
+                    name=file_name,
+
+                )
+            else:
+                return raw.types.InputFile(
+                    id=file_id,
+                    parts=file_total_parts,
+                    name=file_name,
+                    md5_checksum=md5_sum
+                )
+        finally:
+            for _ in workers:
+                await queue.put(None)
+
+            await asyncio.gather(*workers)
+
+            for session in pool:
                 await session.stop()
 
-                if isinstance(path, (str, PurePath)):
-                    fp.close()
+            if isinstance(path, (str, PurePath)):
+                fp.close()
```

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/auth/__init__.py` & `PyroFork-2.1.5/pyrogram/methods/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/auth/accept_terms_of_service.py` & `PyroFork-2.1.5/pyrogram/methods/auth/accept_terms_of_service.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/auth/check_password.py` & `PyroFork-2.1.5/pyrogram/methods/auth/check_password.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/auth/connect.py` & `PyroFork-2.1.5/pyrogram/methods/auth/connect.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/auth/disconnect.py` & `PyroFork-2.1.5/pyrogram/methods/auth/disconnect.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/auth/get_password_hint.py` & `PyroFork-2.1.5/pyrogram/methods/auth/get_password_hint.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/auth/initialize.py` & `PyroFork-2.1.5/pyrogram/methods/utilities/stop.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,41 +12,58 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
-import asyncio
-import logging
-
 import pyrogram
 
-log = logging.getLogger(__name__)
-
 
-class Initialize:
-    async def initialize(
+class Stop:
+    async def stop(
         self: "pyrogram.Client",
+        block: bool = True
     ):
-        """Initialize the client by starting up workers.
+        """Stop the Client.
+
+        This method disconnects the client from Telegram and stops the underlying tasks.
 
-        This method will start updates and download workers.
-        It will also load plugins and start the internal dispatcher.
+        Parameters:
+            block (``bool``, *optional*):
+                Blocks the code execution until the client has been stopped. It is useful with ``block=False`` in case
+                you want to stop the own client *within* a handler in order not to cause a deadlock.
+                Defaults to True.
+
+        Returns:
+            :obj:`~pyrogram.Client`: The stopped client itself.
 
         Raises:
-            ConnectionError: In case you try to initialize a disconnected client or in case you try to initialize an
-                already initialized client.
-        """
-        if not self.is_connected:
-            raise ConnectionError("Can't initialize a disconnected client")
+            ConnectionError: In case you try to stop an already stopped client.
 
-        if self.is_initialized:
-            raise ConnectionError("Client is already initialized")
+        Example:
+            .. code-block:: python
 
-        self.load_plugins()
+                from pyrogram import Client
 
-        await self.dispatcher.start()
+                app = Client("my_account")
+
+
+                async def main():
+                    await app.start()
+                    ...  # Invoke API methods
+                    await app.stop()
+
+
+                app.run(main())
+        """
 
-        self.updates_watchdog_task = asyncio.create_task(self.updates_watchdog())
+        async def do_it():
+            await self.terminate()
+            await self.disconnect()
+
+        if block:
+            await do_it()
+        else:
+            self.loop.create_task(do_it())
 
-        self.is_initialized = True
+        return self
```

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/auth/log_out.py` & `PyroFork-2.1.5/pyrogram/methods/auth/log_out.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/auth/recover_password.py` & `PyroFork-2.1.5/pyrogram/methods/auth/recover_password.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/auth/resend_code.py` & `PyroFork-2.1.5/pyrogram/methods/auth/resend_code.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/auth/send_code.py` & `PyroFork-2.1.5/pyrogram/methods/auth/send_code.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/auth/send_recovery_code.py` & `PyroFork-2.1.5/pyrogram/methods/auth/send_recovery_code.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/auth/sign_in.py` & `PyroFork-2.1.5/pyrogram/methods/auth/sign_in.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/auth/sign_in_bot.py` & `PyroFork-2.1.5/pyrogram/methods/auth/sign_in_bot.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/auth/sign_up.py` & `PyroFork-2.1.5/pyrogram/methods/auth/sign_up.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/auth/terminate.py` & `PyroFork-2.1.5/pyrogram/methods/auth/terminate.py`

 * *Files 16% similar despite different names*

```diff
@@ -37,25 +37,18 @@
             ConnectionError: In case you try to terminate a client that is already terminated.
         """
         if not self.is_initialized:
             raise ConnectionError("Client is already terminated")
 
         if self.takeout_id:
             await self.invoke(raw.functions.account.FinishTakeoutSession())
-            log.warning("Takeout session %s finished", self.takeout_id)
+            log.warning(f"Takeout session {self.takeout_id} finished")
 
         await self.storage.save()
         await self.dispatcher.stop()
 
         for media_session in self.media_sessions.values():
             await media_session.stop()
 
         self.media_sessions.clear()
 
-        self.updates_watchdog_event.set()
-
-        if self.updates_watchdog_task is not None:
-            await self.updates_watchdog_task
-
-        self.updates_watchdog_event.clear()
-
         self.is_initialized = False
```

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/bots/__init__.py` & `PyroFork-2.1.5/pyrogram/methods/bots/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/bots/answer_callback_query.py` & `PyroFork-2.1.5/pyrogram/methods/bots/answer_callback_query.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/bots/answer_inline_query.py` & `PyroFork-2.1.5/pyrogram/methods/bots/answer_inline_query.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/bots/answer_web_app_query.py` & `PyroFork-2.1.5/pyrogram/methods/bots/answer_web_app_query.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/bots/delete_bot_commands.py` & `PyroFork-2.1.5/pyrogram/methods/bots/delete_bot_commands.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/bots/get_bot_commands.py` & `PyroFork-2.1.5/pyrogram/methods/bots/get_bot_commands.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/bots/get_bot_default_privileges.py` & `PyroFork-2.1.5/pyrogram/methods/bots/get_bot_default_privileges.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/bots/get_chat_menu_button.py` & `PyroFork-2.1.5/pyrogram/methods/bots/get_chat_menu_button.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/bots/get_game_high_scores.py` & `PyroFork-2.1.5/pyrogram/methods/bots/get_game_high_scores.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/bots/get_inline_bot_results.py` & `PyroFork-2.1.5/pyrogram/methods/bots/get_inline_bot_results.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/bots/request_callback_answer.py` & `PyroFork-2.1.5/pyrogram/methods/bots/request_callback_answer.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/bots/send_game.py` & `PyroFork-2.1.5/pyrogram/methods/bots/send_game.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/bots/send_inline_bot_result.py` & `PyroFork-2.1.5/pyrogram/methods/bots/send_inline_bot_result.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/bots/set_bot_commands.py` & `PyroFork-2.1.5/pyrogram/methods/bots/set_bot_commands.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/bots/set_bot_default_privileges.py` & `PyroFork-2.1.5/pyrogram/methods/bots/set_bot_default_privileges.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/bots/set_chat_menu_button.py` & `PyroFork-2.1.5/pyrogram/methods/bots/set_chat_menu_button.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/bots/set_game_score.py` & `PyroFork-2.1.5/pyrogram/methods/bots/set_game_score.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/chats/__init__.py` & `PyroFork-2.1.5/pyrogram/methods/chats/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/chats/add_chat_members.py` & `PyroFork-2.1.5/pyrogram/methods/chats/add_chat_members.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/chats/archive_chats.py` & `PyroFork-2.1.5/pyrogram/methods/chats/archive_chats.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/chats/ban_chat_member.py` & `PyroFork-2.1.5/pyrogram/methods/chats/ban_chat_member.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/chats/close_forum_topic.py` & `PyroFork-2.1.5/pyrogram/methods/chats/close_forum_topic.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/chats/close_general_topic.py` & `PyroFork-2.1.5/pyrogram/methods/chats/close_general_topic.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/chats/create_channel.py` & `PyroFork-2.1.5/pyrogram/methods/chats/create_channel.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/chats/create_forum_topic.py` & `PyroFork-2.1.5/pyrogram/methods/chats/create_forum_topic.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/chats/create_group.py` & `PyroFork-2.1.5/pyrogram/methods/chats/create_group.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/chats/create_supergroup.py` & `PyroFork-2.1.5/pyrogram/methods/chats/create_supergroup.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/chats/delete_channel.py` & `PyroFork-2.1.5/pyrogram/methods/chats/delete_channel.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/chats/delete_chat_photo.py` & `PyroFork-2.1.5/pyrogram/methods/chats/delete_chat_photo.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/chats/delete_forum_topic.py` & `PyroFork-2.1.5/pyrogram/methods/chats/delete_forum_topic.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/chats/delete_supergroup.py` & `PyroFork-2.1.5/pyrogram/methods/chats/delete_supergroup.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/chats/delete_user_history.py` & `PyroFork-2.1.5/pyrogram/methods/chats/delete_user_history.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/chats/edit_forum_topic.py` & `PyroFork-2.1.5/pyrogram/methods/chats/edit_forum_topic.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/chats/edit_general_topic.py` & `PyroFork-2.1.5/pyrogram/methods/chats/edit_general_topic.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/chats/get_chat.py` & `PyroFork-2.1.5/pyrogram/methods/chats/get_chat.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/chats/get_chat_event_log.py` & `PyroFork-2.1.5/pyrogram/methods/chats/get_chat_event_log.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/chats/get_chat_member.py` & `PyroFork-2.1.5/pyrogram/methods/chats/get_chat_member.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/chats/get_chat_members.py` & `PyroFork-2.1.5/pyrogram/methods/chats/get_chat_members.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/chats/get_chat_members_count.py` & `PyroFork-2.1.5/pyrogram/methods/chats/get_chat_members_count.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/chats/get_chat_online_count.py` & `PyroFork-2.1.5/pyrogram/methods/chats/get_chat_online_count.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/chats/get_dialogs.py` & `PyroFork-2.1.5/pyrogram/methods/chats/get_dialogs.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/chats/get_dialogs_count.py` & `PyroFork-2.1.5/pyrogram/methods/chats/get_dialogs_count.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/chats/get_forum_topics.py` & `PyroFork-2.1.5/pyrogram/methods/chats/get_forum_topics.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/chats/get_forum_topics_by_id.py` & `PyroFork-2.1.5/pyrogram/methods/chats/get_forum_topics_by_id.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/chats/get_nearby_chats.py` & `PyroFork-2.1.5/pyrogram/methods/chats/get_nearby_chats.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/chats/get_send_as_chats.py` & `PyroFork-2.1.5/pyrogram/methods/chats/get_send_as_chats.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/chats/hide_general_topic.py` & `PyroFork-2.1.5/pyrogram/methods/chats/hide_general_topic.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/chats/join_chat.py` & `PyroFork-2.1.5/pyrogram/methods/chats/join_chat.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/chats/leave_chat.py` & `PyroFork-2.1.5/pyrogram/methods/chats/leave_chat.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/chats/mark_chat_unread.py` & `PyroFork-2.1.5/pyrogram/methods/chats/mark_chat_unread.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/chats/pin_chat_message.py` & `PyroFork-2.1.5/pyrogram/methods/chats/pin_chat_message.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/chats/promote_chat_member.py` & `PyroFork-2.1.5/pyrogram/methods/chats/promote_chat_member.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/chats/reopen_forum_topic.py` & `PyroFork-2.1.5/pyrogram/methods/chats/reopen_forum_topic.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/chats/reopen_general_topic.py` & `PyroFork-2.1.5/pyrogram/methods/chats/reopen_general_topic.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/chats/restrict_chat_member.py` & `PyroFork-2.1.5/pyrogram/methods/chats/restrict_chat_member.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/chats/set_administrator_title.py` & `PyroFork-2.1.5/pyrogram/methods/chats/set_administrator_title.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/chats/set_chat_description.py` & `PyroFork-2.1.5/pyrogram/methods/chats/set_chat_description.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/chats/set_chat_permissions.py` & `PyroFork-2.1.5/pyrogram/methods/chats/set_chat_permissions.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/chats/set_chat_photo.py` & `PyroFork-2.1.5/pyrogram/methods/chats/set_chat_photo.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/chats/set_chat_protected_content.py` & `PyroFork-2.1.5/pyrogram/methods/chats/set_chat_protected_content.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/chats/set_chat_title.py` & `PyroFork-2.1.5/pyrogram/methods/chats/set_chat_title.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/chats/set_chat_username.py` & `PyroFork-2.1.5/pyrogram/methods/chats/set_chat_username.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/chats/set_send_as_chat.py` & `PyroFork-2.1.5/pyrogram/methods/chats/set_send_as_chat.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/chats/set_slow_mode.py` & `PyroFork-2.1.5/pyrogram/methods/chats/set_slow_mode.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/chats/unarchive_chats.py` & `PyroFork-2.1.5/pyrogram/methods/chats/unarchive_chats.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/chats/unban_chat_member.py` & `PyroFork-2.1.5/pyrogram/methods/chats/unban_chat_member.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/chats/unhide_general_topic.py` & `PyroFork-2.1.5/pyrogram/methods/chats/unhide_general_topic.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/chats/unpin_all_chat_messages.py` & `PyroFork-2.1.5/pyrogram/methods/chats/unpin_all_chat_messages.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/chats/unpin_chat_message.py` & `PyroFork-2.1.5/pyrogram/methods/chats/unpin_chat_message.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/contacts/__init__.py` & `PyroFork-2.1.5/pyrogram/methods/contacts/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/contacts/add_contact.py` & `PyroFork-2.1.5/pyrogram/methods/contacts/add_contact.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/contacts/delete_contacts.py` & `PyroFork-2.1.5/pyrogram/methods/contacts/delete_contacts.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/contacts/get_contacts.py` & `PyroFork-2.1.5/pyrogram/methods/contacts/get_contacts.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/contacts/get_contacts_count.py` & `PyroFork-2.1.5/pyrogram/methods/contacts/get_contacts_count.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/contacts/import_contacts.py` & `PyroFork-2.1.5/pyrogram/methods/contacts/import_contacts.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/decorators/__init__.py` & `PyroFork-2.1.5/pyrogram/methods/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/decorators/on_callback_query.py` & `PyroFork-2.1.5/pyrogram/methods/decorators/on_callback_query.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/decorators/on_chat_join_request.py` & `PyroFork-2.1.5/pyrogram/methods/decorators/on_chat_join_request.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/decorators/on_chat_member_updated.py` & `PyroFork-2.1.5/pyrogram/methods/decorators/on_chat_member_updated.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/decorators/on_chosen_inline_result.py` & `PyroFork-2.1.5/pyrogram/methods/decorators/on_chosen_inline_result.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/decorators/on_deleted_messages.py` & `PyroFork-2.1.5/pyrogram/methods/decorators/on_deleted_messages.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/decorators/on_disconnect.py` & `PyroFork-2.1.5/pyrogram/methods/decorators/on_disconnect.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/decorators/on_edited_message.py` & `PyroFork-2.1.5/pyrogram/methods/decorators/on_edited_message.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/decorators/on_inline_query.py` & `PyroFork-2.1.5/pyrogram/methods/decorators/on_inline_query.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/decorators/on_message.py` & `PyroFork-2.1.5/pyrogram/methods/decorators/on_message.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/decorators/on_poll.py` & `PyroFork-2.1.5/pyrogram/methods/decorators/on_poll.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/decorators/on_raw_update.py` & `PyroFork-2.1.5/pyrogram/methods/decorators/on_raw_update.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/decorators/on_user_status.py` & `PyroFork-2.1.5/pyrogram/methods/decorators/on_user_status.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/invite_links/__init__.py` & `PyroFork-2.1.5/pyrogram/methods/invite_links/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/invite_links/approve_all_chat_join_requests.py` & `PyroFork-2.1.5/pyrogram/methods/invite_links/approve_all_chat_join_requests.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/invite_links/approve_chat_join_request.py` & `PyroFork-2.1.5/pyrogram/methods/invite_links/approve_chat_join_request.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/invite_links/create_chat_invite_link.py` & `PyroFork-2.1.5/pyrogram/methods/invite_links/create_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/invite_links/decline_all_chat_join_requests.py` & `PyroFork-2.1.5/pyrogram/methods/invite_links/decline_all_chat_join_requests.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/invite_links/decline_chat_join_request.py` & `PyroFork-2.1.5/pyrogram/methods/invite_links/decline_chat_join_request.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/invite_links/delete_chat_admin_invite_links.py` & `PyroFork-2.1.5/pyrogram/methods/invite_links/delete_chat_admin_invite_links.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/invite_links/delete_chat_invite_link.py` & `PyroFork-2.1.5/pyrogram/methods/invite_links/delete_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/invite_links/edit_chat_invite_link.py` & `PyroFork-2.1.5/pyrogram/methods/invite_links/edit_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/invite_links/export_chat_invite_link.py` & `PyroFork-2.1.5/pyrogram/methods/invite_links/export_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/invite_links/get_chat_admin_invite_links.py` & `PyroFork-2.1.5/pyrogram/methods/invite_links/get_chat_admin_invite_links.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/invite_links/get_chat_admin_invite_links_count.py` & `PyroFork-2.1.5/pyrogram/methods/invite_links/get_chat_admin_invite_links_count.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/invite_links/get_chat_admins_with_invite_links.py` & `PyroFork-2.1.5/pyrogram/methods/invite_links/get_chat_admins_with_invite_links.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/invite_links/get_chat_invite_link.py` & `PyroFork-2.1.5/pyrogram/methods/invite_links/get_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/invite_links/get_chat_invite_link_joiners.py` & `PyroFork-2.1.5/pyrogram/methods/invite_links/get_chat_invite_link_joiners.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/invite_links/get_chat_invite_link_joiners_count.py` & `PyroFork-2.1.5/pyrogram/methods/invite_links/get_chat_invite_link_joiners_count.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/invite_links/get_chat_join_requests.py` & `PyroFork-2.1.5/pyrogram/methods/invite_links/get_chat_join_requests.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/invite_links/revoke_chat_invite_link.py` & `PyroFork-2.1.5/pyrogram/methods/invite_links/revoke_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/messages/__init__.py` & `PyroFork-2.1.5/pyrogram/methods/messages/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/messages/copy_media_group.py` & `PyroFork-2.1.5/pyrogram/methods/messages/copy_media_group.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/messages/copy_message.py` & `PyroFork-2.1.5/pyrogram/methods/messages/copy_message.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/messages/delete_messages.py` & `PyroFork-2.1.5/pyrogram/methods/messages/delete_messages.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/messages/download_media.py` & `PyroFork-2.1.5/pyrogram/methods/messages/download_media.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/messages/edit_inline_caption.py` & `PyroFork-2.1.5/pyrogram/methods/messages/edit_inline_caption.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/messages/edit_inline_media.py` & `PyroFork-2.1.5/pyrogram/methods/messages/edit_inline_media.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/messages/edit_inline_reply_markup.py` & `PyroFork-2.1.5/pyrogram/methods/messages/edit_inline_reply_markup.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/messages/edit_inline_text.py` & `PyroFork-2.1.5/pyrogram/methods/messages/edit_inline_text.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/messages/edit_message_caption.py` & `PyroFork-2.1.5/pyrogram/methods/messages/edit_message_caption.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/messages/edit_message_media.py` & `PyroFork-2.1.5/pyrogram/methods/messages/edit_message_media.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/messages/edit_message_reply_markup.py` & `PyroFork-2.1.5/pyrogram/methods/messages/edit_message_reply_markup.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/messages/edit_message_text.py` & `PyroFork-2.1.5/pyrogram/methods/messages/edit_message_text.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/messages/forward_messages.py` & `PyroFork-2.1.5/pyrogram/methods/messages/forward_messages.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/messages/get_chat_history.py` & `PyroFork-2.1.5/pyrogram/methods/messages/get_chat_history.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/messages/get_chat_history_count.py` & `PyroFork-2.1.5/pyrogram/methods/messages/get_chat_history_count.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/messages/get_custom_emoji_stickers.py` & `PyroFork-2.1.5/pyrogram/methods/messages/get_custom_emoji_stickers.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/messages/get_discussion_message.py` & `PyroFork-2.1.5/pyrogram/methods/messages/get_discussion_message.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/messages/get_discussion_replies.py` & `PyroFork-2.1.5/pyrogram/methods/messages/get_discussion_replies.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/messages/get_discussion_replies_count.py` & `PyroFork-2.1.5/pyrogram/methods/messages/get_discussion_replies_count.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/messages/get_media_group.py` & `PyroFork-2.1.5/pyrogram/methods/messages/get_media_group.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/messages/get_messages.py` & `PyroFork-2.1.5/pyrogram/methods/messages/get_messages.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/messages/inline_session.py` & `PyroFork-2.1.5/pyrogram/methods/messages/inline_session.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/messages/read_chat_history.py` & `PyroFork-2.1.5/pyrogram/methods/messages/read_chat_history.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/messages/retract_vote.py` & `PyroFork-2.1.5/pyrogram/methods/messages/retract_vote.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/messages/search_global.py` & `PyroFork-2.1.5/pyrogram/methods/messages/search_global.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/messages/search_global_count.py` & `PyroFork-2.1.5/pyrogram/methods/messages/search_global_count.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/messages/search_messages.py` & `PyroFork-2.1.5/pyrogram/methods/messages/search_messages.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/messages/search_messages_count.py` & `PyroFork-2.1.5/pyrogram/methods/messages/search_messages_count.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/messages/send_animation.py` & `PyroFork-2.1.5/pyrogram/methods/messages/send_animation.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/messages/send_audio.py` & `PyroFork-2.1.5/pyrogram/methods/messages/send_audio.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/messages/send_cached_media.py` & `PyroFork-2.1.5/pyrogram/methods/messages/send_cached_media.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/messages/send_chat_action.py` & `PyroFork-2.1.5/pyrogram/methods/messages/send_chat_action.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/messages/send_contact.py` & `PyroFork-2.1.5/pyrogram/methods/messages/send_contact.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/messages/send_dice.py` & `PyroFork-2.1.5/pyrogram/methods/messages/send_dice.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/messages/send_document.py` & `PyroFork-2.1.5/pyrogram/methods/messages/send_document.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/messages/send_location.py` & `PyroFork-2.1.5/pyrogram/methods/messages/send_location.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/messages/send_media_group.py` & `PyroFork-2.1.5/pyrogram/methods/messages/send_media_group.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/messages/send_message.py` & `PyroFork-2.1.5/pyrogram/methods/messages/send_message.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/messages/send_photo.py` & `PyroFork-2.1.5/pyrogram/methods/messages/send_photo.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/messages/send_poll.py` & `PyroFork-2.1.5/pyrogram/methods/messages/send_poll.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/messages/send_reaction.py` & `PyroFork-2.1.5/pyrogram/methods/messages/send_reaction.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/messages/send_sticker.py` & `PyroFork-2.1.5/pyrogram/methods/messages/send_sticker.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/messages/send_venue.py` & `PyroFork-2.1.5/pyrogram/methods/messages/send_venue.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/messages/send_video.py` & `PyroFork-2.1.5/pyrogram/methods/messages/send_video.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/messages/send_video_note.py` & `PyroFork-2.1.5/pyrogram/methods/messages/send_video_note.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/messages/send_voice.py` & `PyroFork-2.1.5/pyrogram/methods/messages/send_voice.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/messages/stop_poll.py` & `PyroFork-2.1.5/pyrogram/methods/messages/stop_poll.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/messages/stream_media.py` & `PyroFork-2.1.5/pyrogram/methods/messages/stream_media.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/messages/vote_poll.py` & `PyroFork-2.1.5/pyrogram/methods/messages/vote_poll.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/password/__init__.py` & `PyroFork-2.1.5/pyrogram/methods/password/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/password/change_cloud_password.py` & `PyroFork-2.1.5/pyrogram/methods/password/change_cloud_password.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/password/enable_cloud_password.py` & `PyroFork-2.1.5/pyrogram/methods/password/enable_cloud_password.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/password/remove_cloud_password.py` & `PyroFork-2.1.5/pyrogram/methods/password/remove_cloud_password.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/users/__init__.py` & `PyroFork-2.1.5/pyrogram/methods/users/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/users/block_user.py` & `PyroFork-2.1.5/pyrogram/methods/users/block_user.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/users/delete_profile_photos.py` & `PyroFork-2.1.5/pyrogram/methods/users/delete_profile_photos.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/users/get_chat_photos.py` & `PyroFork-2.1.5/pyrogram/methods/users/get_chat_photos.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/users/get_chat_photos_count.py` & `PyroFork-2.1.5/pyrogram/methods/users/get_chat_photos_count.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/users/get_common_chats.py` & `PyroFork-2.1.5/pyrogram/methods/users/get_common_chats.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/users/get_default_emoji_statuses.py` & `PyroFork-2.1.5/pyrogram/methods/users/get_default_emoji_statuses.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/users/get_me.py` & `PyroFork-2.1.5/pyrogram/methods/users/get_me.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/users/get_users.py` & `PyroFork-2.1.5/pyrogram/methods/users/get_users.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/users/set_emoji_status.py` & `PyroFork-2.1.5/pyrogram/methods/users/set_emoji_status.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/users/set_profile_photo.py` & `PyroFork-2.1.5/pyrogram/methods/users/set_profile_photo.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/users/set_username.py` & `PyroFork-2.1.5/pyrogram/methods/users/set_username.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/users/unblock_user.py` & `PyroFork-2.1.5/pyrogram/methods/users/unblock_user.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/users/update_profile.py` & `PyroFork-2.1.5/pyrogram/methods/users/update_profile.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/utilities/__init__.py` & `PyroFork-2.1.5/pyrogram/methods/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/utilities/add_handler.py` & `PyroFork-2.1.5/pyrogram/methods/utilities/add_handler.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/utilities/compose.py` & `PyroFork-2.1.5/pyrogram/methods/utilities/compose.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/utilities/export_session_string.py` & `PyroFork-2.1.5/pyrogram/methods/utilities/export_session_string.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/utilities/idle.py` & `PyroFork-2.1.5/pyrogram/methods/utilities/idle.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/utilities/remove_handler.py` & `PyroFork-2.1.5/pyrogram/methods/utilities/remove_handler.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/utilities/restart.py` & `PyroFork-2.1.5/pyrogram/methods/utilities/restart.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/utilities/run.py` & `PyroFork-2.1.5/pyrogram/methods/utilities/run.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/utilities/start.py` & `PyroFork-2.1.5/pyrogram/methods/utilities/start.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 
         try:
             if not is_authorized:
                 await self.authorize()
 
             if not await self.storage.is_bot() and self.takeout:
                 self.takeout_id = (await self.invoke(raw.functions.account.InitTakeoutSession())).id
-                log.warning("Takeout session %s initiated", self.takeout_id)
+                log.warning(f"Takeout session {self.takeout_id} initiated")
 
             await self.invoke(raw.functions.updates.GetState())
         except (Exception, KeyboardInterrupt):
             await self.disconnect()
             raise
         else:
             self.me = await self.get_me()
```

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/utilities/stop.py` & `PyroFork-2.1.5/pyrogram/methods/utilities/stop_transmission.py`

 * *Files 18% similar despite different names*

```diff
@@ -15,55 +15,29 @@
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
 import pyrogram
 
 
-class Stop:
-    async def stop(
-        self: "pyrogram.Client",
-        block: bool = True
-    ):
-        """Stop the Client.
-
-        This method disconnects the client from Telegram and stops the underlying tasks.
-
-        Parameters:
-            block (``bool``, *optional*):
-                Blocks the code execution until the client has been stopped. It is useful with ``block=False`` in case
-                you want to stop the own client *within* a handler in order not to cause a deadlock.
-                Defaults to True.
+class StopTransmission:
+    def stop_transmission(self):
+        """Stop downloading or uploading a file.
 
-        Returns:
-            :obj:`~pyrogram.Client`: The stopped client itself.
-
-        Raises:
-            ConnectionError: In case you try to stop an already stopped client.
+        This method must be called inside a progress callback function in order to stop the transmission at the
+        desired time. The progress callback is called every time a file chunk is uploaded/downloaded.
 
         Example:
             .. code-block:: python
 
-                from pyrogram import Client
-
-                app = Client("my_account")
-
-
-                async def main():
-                    await app.start()
-                    ...  # Invoke API methods
-                    await app.stop()
-
-
-                app.run(main())
+                # Stop transmission once the upload progress reaches 50%
+                async def progress(current, total, client):
+                    if (current * 100 / total) > 50:
+                        client.stop_transmission()
+
+                async with app:
+                    await app.send_document(
+                        "me", "file.zip",
+                        progress=progress,
+                        progress_args=(app,))
         """
-
-        async def do_it():
-            await self.terminate()
-            await self.disconnect()
-
-        if block:
-            await do_it()
-        else:
-            self.loop.create_task(do_it())
-
-        return self
+        raise pyrogram.StopTransmission
```

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/methods/utilities/stop_transmission.py` & `PyroFork-2.1.5/pyrogram/raw/core/primitives/string.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,32 +12,20 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
-import pyrogram
+from io import BytesIO
+from typing import cast
 
+from .bytes import Bytes
 
-class StopTransmission:
-    def stop_transmission(self):
-        """Stop downloading or uploading a file.
 
-        This method must be called inside a progress callback function in order to stop the transmission at the
-        desired time. The progress callback is called every time a file chunk is uploaded/downloaded.
+class String(Bytes):
+    @classmethod
+    def read(cls, data: BytesIO, *args) -> str:  # type: ignore
+        return cast(bytes, super(String, String).read(data)).decode(errors="replace")
 
-        Example:
-            .. code-block:: python
-
-                # Stop transmission once the upload progress reaches 50%
-                async def progress(current, total, client):
-                    if (current * 100 / total) > 50:
-                        client.stop_transmission()
-
-                async with app:
-                    await app.send_document(
-                        "me", "file.zip",
-                        progress=progress,
-                        progress_args=(app,))
-        """
-        raise pyrogram.StopTransmission
+    def __new__(cls, value: str) -> bytes:  # type: ignore
+        return super().__new__(cls, value.encode())
```

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/mime_types.py` & `PyroFork-2.1.5/pyrogram/mime_types.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/parser/__init__.py` & `PyroFork-2.1.5/pyrogram/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/parser/html.py` & `PyroFork-2.1.5/pyrogram/parser/html.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,15 +99,15 @@
     def handle_endtag(self, tag):
         try:
             self.entities.append(self.tag_entities[tag].pop())
         except (KeyError, IndexError):
             line, offset = self.getpos()
             offset += 1
 
-            log.debug("Unmatched closing tag </%s> at line %s:%s", tag, line, offset)
+            log.debug(f"Unmatched closing tag </{tag}> at line {line}:{offset}")
         else:
             if not self.tag_entities[tag]:
                 self.tag_entities.pop(tag)
 
     def error(self, message):
         pass
 
@@ -127,15 +127,15 @@
 
         if parser.tag_entities:
             unclosed_tags = []
 
             for tag, entities in parser.tag_entities.items():
                 unclosed_tags.append(f"<{tag}> (x{len(entities)})")
 
-            log.warning("Unclosed tags: %s", ", ".join(unclosed_tags))
+            log.warning(f"Unclosed tags: {', '.join(unclosed_tags)}")
 
         entities = []
 
         for entity in parser.entities:
             if isinstance(entity, raw.types.InputMessageEntityMentionName):
                 try:
                     if self.client is not None:
```

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/parser/markdown.py` & `PyroFork-2.1.5/pyrogram/parser/markdown.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/parser/parser.py` & `PyroFork-2.1.5/pyrogram/parser/parser.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/parser/utils.py` & `PyroFork-2.1.5/pyrogram/parser/utils.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/raw/__init__.py` & `PyroFork-2.1.5/pyrogram/raw/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/raw/core/__init__.py` & `PyroFork-2.1.5/pyrogram/raw/core/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/raw/core/future_salt.py` & `PyroFork-2.1.5/pyrogram/raw/core/future_salt.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/raw/core/future_salts.py` & `PyroFork-2.1.5/pyrogram/raw/core/future_salts.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/raw/core/gzip_packed.py` & `PyroFork-2.1.5/pyrogram/raw/core/gzip_packed.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/raw/core/list.py` & `PyroFork-2.1.5/pyrogram/raw/core/list.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/raw/core/message.py` & `PyroFork-2.1.5/pyrogram/raw/core/message.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/raw/core/msg_container.py` & `PyroFork-2.1.5/pyrogram/raw/core/msg_container.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/raw/core/primitives/__init__.py` & `PyroFork-2.1.5/pyrogram/raw/core/primitives/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/raw/core/primitives/bool.py` & `PyroFork-2.1.5/pyrogram/raw/core/primitives/bool.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/raw/core/primitives/bytes.py` & `PyroFork-2.1.5/pyrogram/raw/core/primitives/bytes.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/raw/core/primitives/double.py` & `PyroFork-2.1.5/pyrogram/raw/core/primitives/double.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/raw/core/primitives/int.py` & `PyroFork-2.1.5/pyrogram/raw/core/primitives/int.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/raw/core/primitives/string.py` & `PyroFork-2.1.5/pyrogram/types/user_and_chats/general_forum_topic_hidden.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,20 +12,18 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
-from io import BytesIO
-from typing import cast
+from ..object import Object
 
-from .bytes import Bytes
 
+class GeneralTopicHidden(Object):
+    """A service message about a general topic hidden in the chat.
 
-class String(Bytes):
-    @classmethod
-    def read(cls, data: BytesIO, *args) -> str:  # type: ignore
-        return cast(bytes, super(String, String).read(data)).decode(errors="replace")
+    Currently holds no information.
+    """
 
-    def __new__(cls, value: str) -> bytes:  # type: ignore
-        return super().__new__(cls, value.encode())
+    def __init__(self):
+        super().__init__()
```

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/raw/core/primitives/vector.py` & `PyroFork-2.1.5/pyrogram/raw/core/primitives/vector.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/raw/core/tl_object.py` & `PyroFork-2.1.5/pyrogram/raw/core/tl_object.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/session/__init__.py` & `PyroFork-2.1.5/pyrogram/session/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/session/auth.py` & `PyroFork-2.1.5/pyrogram/session/auth.py`

 * *Files 4% similar despite different names*

```diff
@@ -75,42 +75,42 @@
 
         # The server may close the connection at any time, causing the auth key creation to fail.
         # If that happens, just try again up to MAX_RETRIES times.
         while True:
             self.connection = Connection(self.dc_id, self.test_mode, self.ipv6, self.proxy)
 
             try:
-                log.info("Start creating a new auth key on DC%s", self.dc_id)
+                log.info(f"Start creating a new auth key on DC{self.dc_id}")
 
                 await self.connection.connect()
 
                 # Step 1; Step 2
                 nonce = int.from_bytes(urandom(16), "little", signed=True)
-                log.debug("Send req_pq: %s", nonce)
+                log.debug(f"Send req_pq: {nonce}")
                 res_pq = await self.invoke(raw.functions.ReqPqMulti(nonce=nonce))
-                log.debug("Got ResPq: %s", res_pq.server_nonce)
-                log.debug("Server public key fingerprints: %s", res_pq.server_public_key_fingerprints)
+                log.debug(f"Got ResPq: {res_pq.server_nonce}")
+                log.debug(f"Server public key fingerprints: {res_pq.server_public_key_fingerprints}")
 
                 for i in res_pq.server_public_key_fingerprints:
                     if i in rsa.server_public_keys:
-                        log.debug("Using fingerprint: %s", i)
+                        log.debug(f"Using fingerprint: {i}")
                         public_key_fingerprint = i
                         break
                     else:
-                        log.debug("Fingerprint unknown: %s", i)
+                        log.debug(f"Fingerprint unknown: {i}")
                 else:
                     raise Exception("Public key not found")
 
                 # Step 3
                 pq = int.from_bytes(res_pq.pq, "big")
-                log.debug("Start PQ factorization: %s", pq)
+                log.debug(f"Start PQ factorization: {pq}")
                 start = time.time()
                 g = prime.decompose(pq)
                 p, q = sorted((g, pq // g))  # p < q
-                log.debug("Done PQ factorization (%ss): %s %s", round(time.time() - start, 3), p, q)
+                log.debug(f"Done PQ factorization ({round(time.time() - start, 3)}s): {p} {q}")
 
                 # Step 4
                 server_nonce = res_pq.server_nonce
                 new_nonce = int.from_bytes(urandom(32), "little", signed=True)
 
                 data = raw.types.PQInnerData(
                     pq=res_pq.pq,
@@ -164,15 +164,15 @@
                 server_dh_inner_data = TLObject.read(BytesIO(answer))
 
                 log.debug("Done decrypting answer")
 
                 dh_prime = int.from_bytes(server_dh_inner_data.dh_prime, "big")
                 delta_time = server_dh_inner_data.server_time - time.time()
 
-                log.debug("Delta time: %s", round(delta_time, 3))
+                log.debug(f"Delta time: {round(delta_time, 3)}")
 
                 # Step 6
                 g = server_dh_inner_data.g
                 b = int.from_bytes(urandom(256), "big")
                 g_b = pow(g, b, dh_prime).to_bytes(256, "big")
 
                 retry_id = 0
@@ -207,75 +207,55 @@
 
                 # TODO: Handle errors
 
                 #######################
                 # Security checks
                 #######################
 
-                SecurityCheckMismatch.check(dh_prime == prime.CURRENT_DH_PRIME, "dh_prime == prime.CURRENT_DH_PRIME")
+                SecurityCheckMismatch.check(dh_prime == prime.CURRENT_DH_PRIME)
                 log.debug("DH parameters check: OK")
 
                 # https://core.telegram.org/mtproto/security_guidelines#g-a-and-g-b-validation
                 g_b = int.from_bytes(g_b, "big")
-                SecurityCheckMismatch.check(1 < g < dh_prime - 1, "1 < g < dh_prime - 1")
-                SecurityCheckMismatch.check(1 < g_a < dh_prime - 1, "1 < g_a < dh_prime - 1")
-                SecurityCheckMismatch.check(1 < g_b < dh_prime - 1, "1 < g_b < dh_prime - 1")
-                SecurityCheckMismatch.check(
-                    2 ** (2048 - 64) < g_a < dh_prime - 2 ** (2048 - 64),
-                    "2 ** (2048 - 64) < g_a < dh_prime - 2 ** (2048 - 64)"
-                )
-                SecurityCheckMismatch.check(
-                    2 ** (2048 - 64) < g_b < dh_prime - 2 ** (2048 - 64),
-                    "2 ** (2048 - 64) < g_b < dh_prime - 2 ** (2048 - 64)"
-                )
+                SecurityCheckMismatch.check(1 < g < dh_prime - 1)
+                SecurityCheckMismatch.check(1 < g_a < dh_prime - 1)
+                SecurityCheckMismatch.check(1 < g_b < dh_prime - 1)
+                SecurityCheckMismatch.check(2 ** (2048 - 64) < g_a < dh_prime - 2 ** (2048 - 64))
+                SecurityCheckMismatch.check(2 ** (2048 - 64) < g_b < dh_prime - 2 ** (2048 - 64))
                 log.debug("g_a and g_b validation: OK")
 
                 # https://core.telegram.org/mtproto/security_guidelines#checking-sha1-hash-values
                 answer = server_dh_inner_data.write()  # Call .write() to remove padding
-                SecurityCheckMismatch.check(
-                    answer_with_hash[:20] == sha1(answer).digest(),
-                    "answer_with_hash[:20] == sha1(answer).digest()"
-                )
+                SecurityCheckMismatch.check(answer_with_hash[:20] == sha1(answer).digest())
                 log.debug("SHA1 hash values check: OK")
 
                 # https://core.telegram.org/mtproto/security_guidelines#checking-nonce-server-nonce-and-new-nonce-fields
                 # 1st message
-                SecurityCheckMismatch.check(nonce == res_pq.nonce, "nonce == res_pq.nonce")
+                SecurityCheckMismatch.check(nonce == res_pq.nonce)
                 # 2nd message
                 server_nonce = int.from_bytes(server_nonce, "little", signed=True)
-                SecurityCheckMismatch.check(nonce == server_dh_params.nonce, "nonce == server_dh_params.nonce")
-                SecurityCheckMismatch.check(
-                    server_nonce == server_dh_params.server_nonce,
-                    "server_nonce == server_dh_params.server_nonce"
-                )
+                SecurityCheckMismatch.check(nonce == server_dh_params.nonce)
+                SecurityCheckMismatch.check(server_nonce == server_dh_params.server_nonce)
                 # 3rd message
-                SecurityCheckMismatch.check(
-                    nonce == set_client_dh_params_answer.nonce,
-                    "nonce == set_client_dh_params_answer.nonce"
-                )
-                SecurityCheckMismatch.check(
-                    server_nonce == set_client_dh_params_answer.server_nonce,
-                    "server_nonce == set_client_dh_params_answer.server_nonce"
-                )
+                SecurityCheckMismatch.check(nonce == set_client_dh_params_answer.nonce)
+                SecurityCheckMismatch.check(server_nonce == set_client_dh_params_answer.server_nonce)
                 server_nonce = server_nonce.to_bytes(16, "little", signed=True)
                 log.debug("Nonce fields check: OK")
 
                 # Step 9
                 server_salt = aes.xor(new_nonce[:8], server_nonce[:8])
 
-                log.debug("Server salt: %s", int.from_bytes(server_salt, "little"))
+                log.debug(f"Server salt: {int.from_bytes(server_salt, 'little')}")
 
-                log.info("Done auth key exchange: %s", set_client_dh_params_answer.__class__.__name__)
+                log.info(f"Done auth key exchange: {set_client_dh_params_answer.__class__.__name__}")
             except Exception as e:
-                log.info("Retrying due to %s: %s", type(e).__name__, e)
-
                 if retries_left:
                     retries_left -= 1
                 else:
                     raise e
 
                 await asyncio.sleep(1)
                 continue
             else:
                 return auth_key
             finally:
-                await self.connection.close()
+                self.connection.close()
```

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/session/internals/__init__.py` & `PyroFork-2.1.5/pyrogram/session/internals/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/session/internals/data_center.py` & `PyroFork-2.1.5/pyrogram/session/internals/data_center.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/session/internals/msg_factory.py` & `PyroFork-2.1.5/pyrogram/session/internals/msg_factory.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/session/internals/msg_id.py` & `PyroFork-2.1.5/pyrogram/types/bots_and_keyboards/callback_game.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,24 +12,18 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
-import logging
-import time
+from ..object import Object
 
-log = logging.getLogger(__name__)
 
+class CallbackGame(Object):
+    """Placeholder, currently holds no information.
 
-class MsgId:
-    last_time = 0
-    offset = 0
+    Use BotFather to set up your game.
+    """
 
-    def __new__(cls) -> int:
-        now = int(time.time())
-        cls.offset = (cls.offset + 4) if now == cls.last_time else 0
-        msg_id = (now * 2 ** 32) + cls.offset
-        cls.last_time = now
-
-        return msg_id
+    def __init__(self):
+        super().__init__()
```

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/session/internals/seq_no.py` & `PyroFork-2.1.5/pyrogram/session/internals/seq_no.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,19 +12,23 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
+from threading import Lock
+
 
 class SeqNo:
     def __init__(self):
         self.content_related_messages_sent = 0
+        self.lock = Lock()
 
     def __call__(self, is_content_related: bool) -> int:
-        seq_no = (self.content_related_messages_sent * 2) + (1 if is_content_related else 0)
+        with self.lock:
+            seq_no = (self.content_related_messages_sent * 2) + (1 if is_content_related else 0)
 
-        if is_content_related:
-            self.content_related_messages_sent += 1
+            if is_content_related:
+                self.content_related_messages_sent += 1
 
-        return seq_no
+            return seq_no
```

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/session/session.py` & `PyroFork-2.1.5/pyrogram/session/session.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
 import asyncio
-import bisect
 import logging
 import os
 from hashlib import sha1
 from io import BytesIO
 
 import pyrogram
 from pyrogram import raw
@@ -41,27 +40,20 @@
 class Result:
     def __init__(self):
         self.value = None
         self.event = asyncio.Event()
 
 
 class Session:
-    START_TIMEOUT = 2
+    START_TIMEOUT = 1
     WAIT_TIMEOUT = 15
     SLEEP_THRESHOLD = 10
-    MAX_RETRIES = 10
-    ACKS_THRESHOLD = 10
+    MAX_RETRIES = 5
+    ACKS_THRESHOLD = 8
     PING_INTERVAL = 5
-    STORED_MSG_IDS_MAX_SIZE = 1000 * 2
-
-    TRANSPORT_ERRORS = {
-        404: "auth key not found",
-        429: "transport flood",
-        444: "invalid DC"
-    }
 
     def __init__(
         self,
         client: "pyrogram.Client",
         dc_id: int,
         auth_key: bytes,
         test_mode: bool,
@@ -89,17 +81,17 @@
         self.results = {}
 
         self.stored_msg_ids = []
 
         self.ping_task = None
         self.ping_task_event = asyncio.Event()
 
-        self.recv_task = None
+        self.network_task = None
 
-        self.is_started = asyncio.Event()
+        self.is_connected = asyncio.Event()
 
         self.loop = asyncio.get_event_loop()
 
     async def start(self):
         while True:
             self.connection = Connection(
                 self.dc_id,
@@ -108,15 +100,15 @@
                 self.client.proxy,
                 self.is_media
             )
 
             try:
                 await self.connection.connect()
 
-                self.recv_task = self.loop.create_task(self.recv_worker())
+                self.network_task = self.loop.create_task(self.network_worker())
 
                 await self.send(raw.functions.Ping(ping_id=0), timeout=self.START_TIMEOUT)
 
                 if not self.is_cdn:
                     await self.send(
                         raw.functions.InvokeWithLayer(
                             layer=layer,
@@ -132,113 +124,98 @@
                             )
                         ),
                         timeout=self.START_TIMEOUT
                     )
 
                 self.ping_task = self.loop.create_task(self.ping_worker())
 
-                log.info("Session initialized: Layer %s", layer)
-                log.info("Device: %s - %s", self.client.device_model, self.client.app_version)
-                log.info("System: %s (%s)", self.client.system_version, self.client.lang_code)
+                log.info(f"Session initialized: Layer {layer}")
+                log.info(f"Device: {self.client.device_model} - {self.client.app_version}")
+                log.info(f"System: {self.client.system_version} ({self.client.lang_code.upper()})")
+
             except AuthKeyDuplicated as e:
                 await self.stop()
                 raise e
-            except (OSError, RPCError):
+            except (OSError, TimeoutError, RPCError):
                 await self.stop()
             except Exception as e:
                 await self.stop()
                 raise e
             else:
                 break
 
-        self.is_started.set()
+        self.is_connected.set()
 
         log.info("Session started")
 
     async def stop(self):
-        self.is_started.clear()
-
-        self.stored_msg_ids.clear()
+        self.is_connected.clear()
 
         self.ping_task_event.set()
 
         if self.ping_task is not None:
             await self.ping_task
 
         self.ping_task_event.clear()
 
-        await self.connection.close()
+        self.connection.close()
+
+        if self.network_task:
+            await self.network_task
 
-        if self.recv_task:
-            await self.recv_task
+        for i in self.results.values():
+            i.event.set()
 
         if not self.is_media and callable(self.client.disconnect_handler):
             try:
                 await self.client.disconnect_handler(self.client)
             except Exception as e:
-                log.exception(e)
+                log.error(e, exc_info=True)
 
         log.info("Session stopped")
 
     async def restart(self):
         await self.stop()
         await self.start()
 
     async def handle_packet(self, packet):
-        data = await self.loop.run_in_executor(
-            pyrogram.crypto_executor,
-            mtproto.unpack,
-            BytesIO(packet),
-            self.session_id,
-            self.auth_key,
-            self.auth_key_id
-        )
+        try:
+            data = await self.loop.run_in_executor(
+                pyrogram.crypto_executor,
+                mtproto.unpack,
+                BytesIO(packet),
+                self.session_id,
+                self.auth_key,
+                self.auth_key_id,
+                self.stored_msg_ids
+            )
+        except SecurityCheckMismatch:
+            return
 
         messages = (
             data.body.messages
             if isinstance(data.body, MsgContainer)
             else [data]
         )
 
-        log.debug("Received: %s", data)
+        # Call log.debug twice because calling it once by appending "data" to the previous string (i.e. f"Kind: {data}")
+        # will cause "data" to be evaluated as string every time instead of only when debug is actually enabled.
+        log.debug("Received:")
+        log.debug(data)
 
         for msg in messages:
+            if msg.seq_no == 0:
+                MsgId.set_server_time(msg.msg_id / (2 ** 32))
+
             if msg.seq_no % 2 != 0:
                 if msg.msg_id in self.pending_acks:
                     continue
                 else:
                     self.pending_acks.add(msg.msg_id)
 
-            try:
-                if len(self.stored_msg_ids) > Session.STORED_MSG_IDS_MAX_SIZE:
-                    del self.stored_msg_ids[:Session.STORED_MSG_IDS_MAX_SIZE // 2]
-
-                if self.stored_msg_ids:
-                    if msg.msg_id < self.stored_msg_ids[0]:
-                        raise SecurityCheckMismatch("The msg_id is lower than all the stored values")
-
-                    if msg.msg_id in self.stored_msg_ids:
-                        raise SecurityCheckMismatch("The msg_id is equal to any of the stored values")
-
-                    time_diff = (msg.msg_id - MsgId()) / 2 ** 32
-
-                    if time_diff > 30:
-                        raise SecurityCheckMismatch("The msg_id belongs to over 30 seconds in the future. "
-                                                    "Most likely the client time has to be synchronized.")
-
-                    if time_diff < -300:
-                        raise SecurityCheckMismatch("The msg_id belongs to over 300 seconds in the past. "
-                                                    "Most likely the client time has to be synchronized.")
-            except SecurityCheckMismatch as e:
-                log.warning("Discarding packet: %s", e)
-                await self.connection.close()
-                return
-            else:
-                bisect.insort(self.stored_msg_ids, msg.msg_id)
-
             if isinstance(msg.body, (raw.types.MsgDetailedInfo, raw.types.MsgNewDetailedInfo)):
                 self.pending_acks.add(msg.body.answer_msg_id)
                 continue
 
             if isinstance(msg.body, raw.types.NewSessionCreated):
                 continue
 
@@ -255,19 +232,19 @@
                     self.loop.create_task(self.client.handle_updates(msg.body))
 
             if msg_id in self.results:
                 self.results[msg_id].value = getattr(msg.body, "result", msg.body)
                 self.results[msg_id].event.set()
 
         if len(self.pending_acks) >= self.ACKS_THRESHOLD:
-            log.debug("Sending %s acks", len(self.pending_acks))
+            log.debug(f"Send {len(self.pending_acks)} acks")
 
             try:
                 await self.send(raw.types.MsgsAck(msg_ids=list(self.pending_acks)), False)
-            except OSError:
+            except (OSError, TimeoutError):
                 pass
             else:
                 self.pending_acks.clear()
 
     async def ping_worker(self):
         log.info("PingTask started")
 
@@ -281,35 +258,30 @@
 
             try:
                 await self.send(
                     raw.functions.PingDelayDisconnect(
                         ping_id=0, disconnect_delay=self.WAIT_TIMEOUT + 10
                     ), False
                 )
-            except (OSError, RPCError):
+            except (OSError, TimeoutError, RPCError):
                 pass
 
         log.info("PingTask stopped")
 
-    async def recv_worker(self):
+    async def network_worker(self):
         log.info("NetworkTask started")
 
         while True:
             packet = await self.connection.recv()
 
             if packet is None or len(packet) == 4:
                 if packet:
-                    error_code = -Int.read(BytesIO(packet))
+                    log.warning(f'Server sent "{Int.read(BytesIO(packet))}"')
 
-                    log.warning(
-                        "Server sent transport error: %s (%s)",
-                        error_code, Session.TRANSPORT_ERRORS.get(error_code, "unknown error")
-                    )
-
-                if self.is_started.is_set():
+                if self.is_connected.is_set():
                     self.loop.create_task(self.restart())
 
                 break
 
             self.loop.create_task(self.handle_packet(packet))
 
         log.info("NetworkTask stopped")
@@ -317,15 +289,18 @@
     async def send(self, data: TLObject, wait_response: bool = True, timeout: float = WAIT_TIMEOUT):
         message = self.msg_factory(data)
         msg_id = message.msg_id
 
         if wait_response:
             self.results[msg_id] = Result()
 
-        log.debug("Sent: %s", message)
+        # Call log.debug twice because calling it once by appending "data" to the previous string (i.e. f"Kind: {data}")
+        # will cause "data" to be evaluated as string every time instead of only when debug is actually enabled.
+        log.debug(f"Sent:")
+        log.debug(message)
 
         payload = await self.loop.run_in_executor(
             pyrogram.crypto_executor,
             mtproto.pack,
             message,
             self.salt,
             self.session_id,
@@ -340,44 +315,41 @@
             raise e
 
         if wait_response:
             try:
                 await asyncio.wait_for(self.results[msg_id].event.wait(), timeout)
             except asyncio.TimeoutError:
                 pass
-
-            result = self.results.pop(msg_id).value
+            finally:
+                result = self.results.pop(msg_id).value
 
             if result is None:
-                raise TimeoutError("Request timed out")
-
-            if isinstance(result, raw.types.RpcError):
+                raise TimeoutError
+            elif isinstance(result, raw.types.RpcError):
                 if isinstance(data, (raw.functions.InvokeWithoutUpdates, raw.functions.InvokeWithTakeout)):
                     data = data.query
 
                 RPCError.raise_it(result, type(data))
-
-            if isinstance(result, raw.types.BadMsgNotification):
-                log.warning("%s: %s", BadMsgNotification.__name__, BadMsgNotification(result.error_code))
-
-            if isinstance(result, raw.types.BadServerSalt):
+            elif isinstance(result, raw.types.BadMsgNotification):
+                raise BadMsgNotification(result.error_code)
+            elif isinstance(result, raw.types.BadServerSalt):
                 self.salt = result.new_server_salt
                 return await self.send(data, wait_response, timeout)
-
-            return result
+            else:
+                return result
 
     async def invoke(
         self,
         query: TLObject,
         retries: int = MAX_RETRIES,
         timeout: float = WAIT_TIMEOUT,
         sleep_threshold: float = SLEEP_THRESHOLD
     ):
         try:
-            await asyncio.wait_for(self.is_started.wait(), self.WAIT_TIMEOUT)
+            await asyncio.wait_for(self.is_connected.wait(), self.WAIT_TIMEOUT)
         except asyncio.TimeoutError:
             pass
 
         if isinstance(query, (raw.functions.InvokeWithoutUpdates, raw.functions.InvokeWithTakeout)):
             inner_query = query.query
         else:
             inner_query = query
@@ -389,24 +361,21 @@
                 return await self.send(query, timeout=timeout)
             except FloodWait as e:
                 amount = e.value
 
                 if amount > sleep_threshold >= 0:
                     raise
 
-                log.warning('[%s] Waiting for %s seconds before continuing (required by "%s")',
-                            self.client.name, amount, query_name)
+                log.warning(f'[{self.client.name}] Waiting for {amount} seconds before continuing '
+                            f'(required by "{query_name}")')
 
                 await asyncio.sleep(amount)
-            except (OSError, InternalServerError, ServiceUnavailable) as e:
+            except (OSError, TimeoutError, InternalServerError, ServiceUnavailable) as e:
                 if retries == 0:
                     raise e from None
 
                 (log.warning if retries < 2 else log.info)(
-                    '[%s] Retrying "%s" due to: %s',
-                    Session.MAX_RETRIES - retries + 1,
-                    query_name, str(e) or repr(e)
-                )
+                    f'[{Session.MAX_RETRIES - retries + 1}] Retrying "{query_name}" due to {str(e) or repr(e)}')
 
                 await asyncio.sleep(0.5)
 
                 return await self.invoke(query, retries - 1, timeout)
```

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/storage/__init__.py` & `PyroFork-2.1.5/pyrogram/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/storage/file_storage.py` & `PyroFork-2.1.5/pyrogram/storage/file_storage.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,21 +34,21 @@
 
         self.database = workdir / (self.name + self.FILE_EXTENSION)
 
     def update(self):
         version = self.version()
 
         if version == 1:
-            with self.conn:
+            with self.lock, self.conn:
                 self.conn.execute("DELETE FROM peers")
 
             version += 1
 
         if version == 2:
-            with self.conn:
+            with self.lock, self.conn:
                 self.conn.execute("ALTER TABLE sessions ADD api_id INTEGER")
 
             version += 1
 
         self.version(version)
 
     async def open(self):
@@ -59,11 +59,14 @@
 
         if not file_exists:
             self.create()
         else:
             self.update()
 
         with self.conn:
-            self.conn.execute("VACUUM")
+            try:  # Python 3.6.0 (exactly this version) is bugged and won't successfully execute the vacuum
+                self.conn.execute("VACUUM")
+            except sqlite3.OperationalError:
+                pass
 
     async def delete(self):
         os.remove(self.database)
```

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/storage/memory_storage.py` & `PyroFork-2.1.5/pyrogram/storage/memory_storage.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/storage/sqlite_storage.py` & `PyroFork-2.1.5/pyrogram/storage/sqlite_storage.py`

 * *Files 17% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
 import inspect
 import sqlite3
 import time
+from threading import Lock
 from typing import List, Tuple, Any
 
 from pyrogram import raw
 from .storage import Storage
 from .. import utils
 
 # language=SQLite
@@ -93,17 +94,18 @@
     VERSION = 3
     USERNAME_TTL = 8 * 60 * 60
 
     def __init__(self, name: str):
         super().__init__(name)
 
         self.conn = None  # type: sqlite3.Connection
+        self.lock = Lock()
 
     def create(self):
-        with self.conn:
+        with self.lock, self.conn:
             self.conn.executescript(SCHEMA)
 
             self.conn.execute(
                 "INSERT INTO version VALUES (?)",
                 (self.VERSION,)
             )
 
@@ -113,28 +115,32 @@
             )
 
     async def open(self):
         raise NotImplementedError
 
     async def save(self):
         await self.date(int(time.time()))
-        self.conn.commit()
+
+        with self.lock:
+            self.conn.commit()
 
     async def close(self):
-        self.conn.close()
+        with self.lock:
+            self.conn.close()
 
     async def delete(self):
         raise NotImplementedError
 
     async def update_peers(self, peers: List[Tuple[int, int, str, str, str]]):
-        self.conn.executemany(
-            "REPLACE INTO peers (id, access_hash, type, username, phone_number)"
-            "VALUES (?, ?, ?, ?, ?)",
-            peers
-        )
+        with self.lock:
+            self.conn.executemany(
+                "REPLACE INTO peers (id, access_hash, type, username, phone_number)"
+                "VALUES (?, ?, ?, ?, ?)",
+                peers
+            )
 
     async def get_peer_by_id(self, peer_id: int):
         r = self.conn.execute(
             "SELECT id, access_hash, type FROM peers WHERE id = ?",
             (peer_id,)
         ).fetchone()
 
@@ -175,15 +181,15 @@
         return self.conn.execute(
             f"SELECT {attr} FROM sessions"
         ).fetchone()[0]
 
     def _set(self, value: Any):
         attr = inspect.stack()[2].function
 
-        with self.conn:
+        with self.lock, self.conn:
             self.conn.execute(
                 f"UPDATE sessions SET {attr} = ?",
                 (value,)
             )
 
     def _accessor(self, value: Any = object):
         return self._get() if value == object else self._set(value)
@@ -211,12 +217,12 @@
 
     def version(self, value: int = object):
         if value == object:
             return self.conn.execute(
                 "SELECT number FROM version"
             ).fetchone()[0]
         else:
-            with self.conn:
+            with self.lock, self.conn:
                 self.conn.execute(
                     "UPDATE version SET number = ?",
                     (value,)
                 )
```

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/storage/storage.py` & `PyroFork-2.1.5/pyrogram/storage/storage.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/sync.py` & `PyroFork-2.1.5/pyrogram/sync.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/types/__init__.py` & `PyroFork-2.1.5/pyrogram/types/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/types/authorization/__init__.py` & `PyroFork-2.1.5/pyrogram/types/authorization/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/types/authorization/sent_code.py` & `PyroFork-2.1.5/pyrogram/types/authorization/sent_code.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/types/authorization/terms_of_service.py` & `PyroFork-2.1.5/pyrogram/types/authorization/terms_of_service.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/types/bots_and_keyboards/__init__.py` & `PyroFork-2.1.5/pyrogram/types/bots_and_keyboards/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/types/bots_and_keyboards/bot_command.py` & `PyroFork-2.1.5/pyrogram/types/bots_and_keyboards/bot_command.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/types/bots_and_keyboards/bot_command_scope.py` & `PyroFork-2.1.5/pyrogram/types/bots_and_keyboards/bot_command_scope.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/types/bots_and_keyboards/bot_command_scope_all_chat_administrators.py` & `PyroFork-2.1.5/pyrogram/types/bots_and_keyboards/bot_command_scope_all_chat_administrators.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/types/bots_and_keyboards/bot_command_scope_all_group_chats.py` & `PyroFork-2.1.5/pyrogram/types/bots_and_keyboards/bot_command_scope_all_group_chats.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/types/bots_and_keyboards/bot_command_scope_all_private_chats.py` & `PyroFork-2.1.5/pyrogram/types/bots_and_keyboards/bot_command_scope_all_private_chats.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/types/bots_and_keyboards/bot_command_scope_chat.py` & `PyroFork-2.1.5/pyrogram/types/bots_and_keyboards/bot_command_scope_chat.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_administrators.py` & `PyroFork-2.1.5/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_administrators.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_member.py` & `PyroFork-2.1.5/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_member.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/types/bots_and_keyboards/bot_command_scope_default.py` & `PyroFork-2.1.5/pyrogram/types/bots_and_keyboards/bot_command_scope_default.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/types/bots_and_keyboards/callback_game.py` & `PyroFork-2.1.5/pyrogram/types/user_and_chats/general_forum_topic_unhidden.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
 from ..object import Object
 
 
-class CallbackGame(Object):
-    """Placeholder, currently holds no information.
+class GeneralTopicUnhidden(Object):
+    """A service message about a general topic unhidden in the chat.
 
-    Use BotFather to set up your game.
+    Currently holds no information.
     """
 
     def __init__(self):
         super().__init__()
```

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/types/bots_and_keyboards/callback_query.py` & `PyroFork-2.1.5/pyrogram/types/bots_and_keyboards/callback_query.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/types/bots_and_keyboards/force_reply.py` & `PyroFork-2.1.5/pyrogram/types/bots_and_keyboards/force_reply.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/types/bots_and_keyboards/game_high_score.py` & `PyroFork-2.1.5/pyrogram/types/bots_and_keyboards/game_high_score.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/types/bots_and_keyboards/inline_keyboard_button.py` & `PyroFork-2.1.5/pyrogram/types/bots_and_keyboards/inline_keyboard_button.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/types/bots_and_keyboards/inline_keyboard_markup.py` & `PyroFork-2.1.5/pyrogram/types/bots_and_keyboards/inline_keyboard_markup.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/types/bots_and_keyboards/keyboard_button.py` & `PyroFork-2.1.5/pyrogram/types/bots_and_keyboards/keyboard_button.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/types/bots_and_keyboards/login_url.py` & `PyroFork-2.1.5/pyrogram/types/bots_and_keyboards/login_url.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/types/bots_and_keyboards/menu_button.py` & `PyroFork-2.1.5/pyrogram/types/bots_and_keyboards/menu_button.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/types/bots_and_keyboards/menu_button_commands.py` & `PyroFork-2.1.5/pyrogram/types/bots_and_keyboards/menu_button_commands.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/types/bots_and_keyboards/menu_button_default.py` & `PyroFork-2.1.5/pyrogram/types/bots_and_keyboards/menu_button_default.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/types/bots_and_keyboards/menu_button_web_app.py` & `PyroFork-2.1.5/pyrogram/types/bots_and_keyboards/menu_button_web_app.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/types/bots_and_keyboards/reply_keyboard_markup.py` & `PyroFork-2.1.5/pyrogram/types/bots_and_keyboards/reply_keyboard_markup.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/types/bots_and_keyboards/reply_keyboard_remove.py` & `PyroFork-2.1.5/pyrogram/types/bots_and_keyboards/reply_keyboard_remove.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/types/bots_and_keyboards/sent_web_app_message.py` & `PyroFork-2.1.5/pyrogram/types/bots_and_keyboards/sent_web_app_message.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/types/bots_and_keyboards/web_app_info.py` & `PyroFork-2.1.5/pyrogram/types/bots_and_keyboards/web_app_info.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/types/inline_mode/__init__.py` & `PyroFork-2.1.5/pyrogram/types/inline_mode/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/types/inline_mode/chosen_inline_result.py` & `PyroFork-2.1.5/pyrogram/types/inline_mode/chosen_inline_result.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/types/inline_mode/inline_query.py` & `PyroFork-2.1.5/pyrogram/types/inline_mode/inline_query.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/types/inline_mode/inline_query_result.py` & `PyroFork-2.1.5/pyrogram/types/inline_mode/inline_query_result.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/types/inline_mode/inline_query_result_animation.py` & `PyroFork-2.1.5/pyrogram/types/inline_mode/inline_query_result_animation.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/types/inline_mode/inline_query_result_article.py` & `PyroFork-2.1.5/pyrogram/types/inline_mode/inline_query_result_article.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/types/inline_mode/inline_query_result_audio.py` & `PyroFork-2.1.5/pyrogram/types/inline_mode/inline_query_result_audio.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/types/inline_mode/inline_query_result_cached_animation.py` & `PyroFork-2.1.5/pyrogram/types/inline_mode/inline_query_result_cached_animation.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/types/inline_mode/inline_query_result_cached_audio.py` & `PyroFork-2.1.5/pyrogram/types/inline_mode/inline_query_result_cached_audio.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/types/inline_mode/inline_query_result_cached_document.py` & `PyroFork-2.1.5/pyrogram/types/inline_mode/inline_query_result_cached_document.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/types/inline_mode/inline_query_result_cached_photo.py` & `PyroFork-2.1.5/pyrogram/types/inline_mode/inline_query_result_cached_photo.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/types/inline_mode/inline_query_result_cached_sticker.py` & `PyroFork-2.1.5/pyrogram/types/inline_mode/inline_query_result_cached_sticker.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/types/inline_mode/inline_query_result_cached_video.py` & `PyroFork-2.1.5/pyrogram/types/inline_mode/inline_query_result_cached_video.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/types/inline_mode/inline_query_result_cached_voice.py` & `PyroFork-2.1.5/pyrogram/types/inline_mode/inline_query_result_cached_voice.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/types/inline_mode/inline_query_result_contact.py` & `PyroFork-2.1.5/pyrogram/types/inline_mode/inline_query_result_contact.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/types/inline_mode/inline_query_result_document.py` & `PyroFork-2.1.5/pyrogram/types/inline_mode/inline_query_result_document.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/types/inline_mode/inline_query_result_location.py` & `PyroFork-2.1.5/pyrogram/types/inline_mode/inline_query_result_location.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/types/inline_mode/inline_query_result_photo.py` & `PyroFork-2.1.5/pyrogram/types/inline_mode/inline_query_result_photo.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/types/inline_mode/inline_query_result_venue.py` & `PyroFork-2.1.5/pyrogram/types/inline_mode/inline_query_result_venue.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/types/inline_mode/inline_query_result_video.py` & `PyroFork-2.1.5/pyrogram/types/inline_mode/inline_query_result_video.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/types/inline_mode/inline_query_result_voice.py` & `PyroFork-2.1.5/pyrogram/types/inline_mode/inline_query_result_voice.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/types/input_media/__init__.py` & `PyroFork-2.1.5/pyrogram/types/input_media/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/types/input_media/input_media.py` & `PyroFork-2.1.5/pyrogram/types/input_media/input_media.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/types/input_media/input_media_animation.py` & `PyroFork-2.1.5/pyrogram/types/input_media/input_media_animation.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/types/input_media/input_media_audio.py` & `PyroFork-2.1.5/pyrogram/types/input_media/input_media_audio.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/types/input_media/input_media_document.py` & `PyroFork-2.1.5/pyrogram/types/input_media/input_media_document.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/types/input_media/input_media_photo.py` & `PyroFork-2.1.5/pyrogram/types/input_media/input_media_photo.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/types/input_media/input_media_video.py` & `PyroFork-2.1.5/pyrogram/types/input_media/input_media_video.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/types/input_media/input_phone_contact.py` & `PyroFork-2.1.5/pyrogram/types/input_media/input_phone_contact.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/types/input_message_content/__init__.py` & `PyroFork-2.1.5/pyrogram/types/input_message_content/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/types/input_message_content/input_message_content.py` & `PyroFork-2.1.5/pyrogram/types/input_message_content/input_message_content.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/types/input_message_content/input_text_message_content.py` & `PyroFork-2.1.5/pyrogram/types/input_message_content/input_text_message_content.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/types/list.py` & `PyroFork-2.1.5/pyrogram/types/list.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/types/messages_and_media/__init__.py` & `PyroFork-2.1.5/pyrogram/types/messages_and_media/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,22 +26,23 @@
 from .message import Message
 from .message_entity import MessageEntity
 from .photo import Photo
 from .poll import Poll
 from .poll_option import PollOption
 from .reaction import Reaction
 from .sticker import Sticker
+from .stickerset import StickerSet
 from .stripped_thumbnail import StrippedThumbnail
 from .thumbnail import Thumbnail
 from .venue import Venue
 from .video import Video
 from .video_note import VideoNote
 from .voice import Voice
 from .web_app_data import WebAppData
 from .web_page import WebPage
 from .message_reactions import MessageReactions
 
 __all__ = [
     "Animation", "Audio", "Contact", "Document", "Game", "Location", "Message", "MessageEntity", "Photo", "Thumbnail",
-    "StrippedThumbnail", "Poll", "PollOption", "Sticker", "Venue", "Video", "VideoNote", "Voice", "WebPage", "Dice",
+    "StrippedThumbnail", "Poll", "PollOption", "Sticker", "StickerSet", "Venue", "Video", "VideoNote", "Voice", "WebPage", "Dice",
     "Reaction", "WebAppData", "MessageReactions"
 ]
```

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/types/messages_and_media/animation.py` & `PyroFork-2.1.5/pyrogram/types/messages_and_media/animation.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/types/messages_and_media/audio.py` & `PyroFork-2.1.5/pyrogram/types/messages_and_media/audio.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/types/messages_and_media/contact.py` & `PyroFork-2.1.5/pyrogram/types/messages_and_media/contact.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/types/messages_and_media/dice.py` & `PyroFork-2.1.5/pyrogram/types/messages_and_media/dice.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/types/messages_and_media/document.py` & `PyroFork-2.1.5/pyrogram/types/messages_and_media/document.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/types/messages_and_media/game.py` & `PyroFork-2.1.5/pyrogram/types/messages_and_media/game.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/types/messages_and_media/location.py` & `PyroFork-2.1.5/pyrogram/types/messages_and_media/location.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/types/messages_and_media/message.py` & `PyroFork-2.1.5/pyrogram/types/messages_and_media/message.py`

 * *Files 0% similar despite different names*

```diff
@@ -8320,1200 +8320,1200 @@
 000207f0: 2020 2020 2020 2020 5250 4345 7272 6f72          RPCError
 00020800: 3a20 496e 2063 6173 6520 6f66 2061 2054  : In case of a T
 00020810: 656c 6567 7261 6d20 5250 4320 6572 726f  elegram RPC erro
 00020820: 722e 0a20 2020 2020 2020 2022 2222 0a20  r..        """. 
 00020830: 2020 2020 2020 2069 6620 7365 6c66 2e73         if self.s
 00020840: 6572 7669 6365 3a0a 2020 2020 2020 2020  ervice:.        
 00020850: 2020 2020 6c6f 672e 7761 726e 696e 6728      log.warning(
-00020860: 2253 6572 7669 6365 206d 6573 7361 6765  "Service message
-00020870: 7320 6361 6e6e 6f74 2062 6520 636f 7069  s cannot be copi
-00020880: 6564 2e20 6368 6174 5f69 643a 2025 732c  ed. chat_id: %s,
-00020890: 206d 6573 7361 6765 5f69 643a 2025 7322   message_id: %s"
-000208a0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000208b0: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
-000208c0: 6861 742e 6964 2c20 7365 6c66 2e69 6429  hat.id, self.id)
-000208d0: 0a20 2020 2020 2020 2065 6c69 6620 7365  .        elif se
-000208e0: 6c66 2e67 616d 6520 616e 6420 6e6f 7420  lf.game and not 
-000208f0: 6177 6169 7420 7365 6c66 2e5f 636c 6965  await self._clie
-00020900: 6e74 2e73 746f 7261 6765 2e69 735f 626f  nt.storage.is_bo
-00020910: 7428 293a 0a20 2020 2020 2020 2020 2020  t():.           
-00020920: 206c 6f67 2e77 6172 6e69 6e67 2822 5573   log.warning("Us
-00020930: 6572 7320 6361 6e6e 6f74 2073 656e 6420  ers cannot send 
-00020940: 6d65 7373 6167 6573 2077 6974 6820 4761  messages with Ga
-00020950: 6d65 206d 6564 6961 2074 7970 652e 2063  me media type. c
-00020960: 6861 745f 6964 3a20 2573 2c20 6d65 7373  hat_id: %s, mess
-00020970: 6167 655f 6964 3a20 2573 222c 0a20 2020  age_id: %s",.   
-00020980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020990: 2020 2020 2073 656c 662e 6368 6174 2e69       self.chat.i
-000209a0: 642c 2073 656c 662e 6964 290a 2020 2020  d, self.id).    
-000209b0: 2020 2020 656c 6966 2073 656c 662e 656d      elif self.em
-000209c0: 7074 793a 0a20 2020 2020 2020 2020 2020  pty:.           
-000209d0: 206c 6f67 2e77 6172 6e69 6e67 2822 456d   log.warning("Em
-000209e0: 7074 7920 6d65 7373 6167 6573 2063 616e  pty messages can
-000209f0: 6e6f 7420 6265 2063 6f70 6965 642e 2229  not be copied.")
-00020a00: 0a20 2020 2020 2020 2065 6c69 6620 7365  .        elif se
-00020a10: 6c66 2e74 6578 743a 0a20 2020 2020 2020  lf.text:.       
-00020a20: 2020 2020 2072 6574 7572 6e20 6177 6169       return awai
-00020a30: 7420 7365 6c66 2e5f 636c 6965 6e74 2e73  t self._client.s
-00020a40: 656e 645f 6d65 7373 6167 6528 0a20 2020  end_message(.   
-00020a50: 2020 2020 2020 2020 2020 2020 2063 6861               cha
-00020a60: 745f 6964 2c0a 2020 2020 2020 2020 2020  t_id,.          
-00020a70: 2020 2020 2020 7465 7874 3d73 656c 662e        text=self.
-00020a80: 7465 7874 2c0a 2020 2020 2020 2020 2020  text,.          
-00020a90: 2020 2020 2020 656e 7469 7469 6573 3d73        entities=s
-00020aa0: 656c 662e 656e 7469 7469 6573 2c0a 2020  elf.entities,.  
-00020ab0: 2020 2020 2020 2020 2020 2020 2020 7061                pa
-00020ac0: 7273 655f 6d6f 6465 3d65 6e75 6d73 2e50  rse_mode=enums.P
-00020ad0: 6172 7365 4d6f 6465 2e44 4953 4142 4c45  arseMode.DISABLE
-00020ae0: 442c 0a20 2020 2020 2020 2020 2020 2020  D,.             
-00020af0: 2020 2064 6973 6162 6c65 5f77 6562 5f70     disable_web_p
-00020b00: 6167 655f 7072 6576 6965 773d 6e6f 7420  age_preview=not 
-00020b10: 7365 6c66 2e77 6562 5f70 6167 652c 0a20  self.web_page,. 
-00020b20: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-00020b30: 6973 6162 6c65 5f6e 6f74 6966 6963 6174  isable_notificat
-00020b40: 696f 6e3d 6469 7361 626c 655f 6e6f 7469  ion=disable_noti
-00020b50: 6669 6361 7469 6f6e 2c0a 2020 2020 2020  fication,.      
-00020b60: 2020 2020 2020 2020 2020 6d65 7373 6167            messag
-00020b70: 655f 7468 7265 6164 5f69 643d 6d65 7373  e_thread_id=mess
-00020b80: 6167 655f 7468 7265 6164 5f69 642c 0a20  age_thread_id,. 
-00020b90: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00020ba0: 6570 6c79 5f74 6f5f 6d65 7373 6167 655f  eply_to_message_
-00020bb0: 6964 3d72 6570 6c79 5f74 6f5f 6d65 7373  id=reply_to_mess
-00020bc0: 6167 655f 6964 2c0a 2020 2020 2020 2020  age_id,.        
-00020bd0: 2020 2020 2020 2020 7363 6865 6475 6c65          schedule
-00020be0: 5f64 6174 653d 7363 6865 6475 6c65 5f64  _date=schedule_d
-00020bf0: 6174 652c 0a20 2020 2020 2020 2020 2020  ate,.           
-00020c00: 2020 2020 2070 726f 7465 6374 5f63 6f6e       protect_con
-00020c10: 7465 6e74 3d70 726f 7465 6374 5f63 6f6e  tent=protect_con
-00020c20: 7465 6e74 2c0a 2020 2020 2020 2020 2020  tent,.          
-00020c30: 2020 2020 2020 7265 706c 795f 6d61 726b        reply_mark
-00020c40: 7570 3d73 656c 662e 7265 706c 795f 6d61  up=self.reply_ma
-00020c50: 726b 7570 2069 6620 7265 706c 795f 6d61  rkup if reply_ma
-00020c60: 726b 7570 2069 7320 6f62 6a65 6374 2065  rkup is object e
-00020c70: 6c73 6520 7265 706c 795f 6d61 726b 7570  lse reply_markup
-00020c80: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
-00020c90: 2020 2020 2020 2065 6c69 6620 7365 6c66         elif self
-00020ca0: 2e6d 6564 6961 3a0a 2020 2020 2020 2020  .media:.        
-00020cb0: 2020 2020 7365 6e64 5f6d 6564 6961 203d      send_media =
-00020cc0: 2070 6172 7469 616c 280a 2020 2020 2020   partial(.      
-00020cd0: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-00020ce0: 636c 6965 6e74 2e73 656e 645f 6361 6368  client.send_cach
-00020cf0: 6564 5f6d 6564 6961 2c0a 2020 2020 2020  ed_media,.      
-00020d00: 2020 2020 2020 2020 2020 6368 6174 5f69            chat_i
-00020d10: 643d 6368 6174 5f69 642c 0a20 2020 2020  d=chat_id,.     
-00020d20: 2020 2020 2020 2020 2020 2064 6973 6162             disab
-00020d30: 6c65 5f6e 6f74 6966 6963 6174 696f 6e3d  le_notification=
-00020d40: 6469 7361 626c 655f 6e6f 7469 6669 6361  disable_notifica
-00020d50: 7469 6f6e 2c0a 2020 2020 2020 2020 2020  tion,.          
-00020d60: 2020 2020 2020 6d65 7373 6167 655f 7468        message_th
-00020d70: 7265 6164 5f69 643d 6d65 7373 6167 655f  read_id=message_
-00020d80: 7468 7265 6164 5f69 642c 0a20 2020 2020  thread_id,.     
-00020d90: 2020 2020 2020 2020 2020 2072 6570 6c79             reply
-00020da0: 5f74 6f5f 6d65 7373 6167 655f 6964 3d72  _to_message_id=r
-00020db0: 6570 6c79 5f74 6f5f 6d65 7373 6167 655f  eply_to_message_
-00020dc0: 6964 2c0a 2020 2020 2020 2020 2020 2020  id,.            
-00020dd0: 2020 2020 7363 6865 6475 6c65 5f64 6174      schedule_dat
-00020de0: 653d 7363 6865 6475 6c65 5f64 6174 652c  e=schedule_date,
-00020df0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00020e00: 2070 726f 7465 6374 5f63 6f6e 7465 6e74   protect_content
-00020e10: 3d70 726f 7465 6374 5f63 6f6e 7465 6e74  =protect_content
-00020e20: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00020e30: 2020 7265 706c 795f 6d61 726b 7570 3d73    reply_markup=s
-00020e40: 656c 662e 7265 706c 795f 6d61 726b 7570  elf.reply_markup
-00020e50: 2069 6620 7265 706c 795f 6d61 726b 7570   if reply_markup
-00020e60: 2069 7320 6f62 6a65 6374 2065 6c73 6520   is object else 
-00020e70: 7265 706c 795f 6d61 726b 7570 0a20 2020  reply_markup.   
-00020e80: 2020 2020 2020 2020 2029 0a0a 2020 2020           )..    
-00020e90: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00020ea0: 7068 6f74 6f3a 0a20 2020 2020 2020 2020  photo:.         
-00020eb0: 2020 2020 2020 2066 696c 655f 6964 203d         file_id =
-00020ec0: 2073 656c 662e 7068 6f74 6f2e 6669 6c65   self.photo.file
-00020ed0: 5f69 640a 2020 2020 2020 2020 2020 2020  _id.            
-00020ee0: 656c 6966 2073 656c 662e 6175 6469 6f3a  elif self.audio:
-00020ef0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00020f00: 2066 696c 655f 6964 203d 2073 656c 662e   file_id = self.
-00020f10: 6175 6469 6f2e 6669 6c65 5f69 640a 2020  audio.file_id.  
-00020f20: 2020 2020 2020 2020 2020 656c 6966 2073            elif s
-00020f30: 656c 662e 646f 6375 6d65 6e74 3a0a 2020  elf.document:.  
-00020f40: 2020 2020 2020 2020 2020 2020 2020 6669                fi
-00020f50: 6c65 5f69 6420 3d20 7365 6c66 2e64 6f63  le_id = self.doc
-00020f60: 756d 656e 742e 6669 6c65 5f69 640a 2020  ument.file_id.  
-00020f70: 2020 2020 2020 2020 2020 656c 6966 2073            elif s
-00020f80: 656c 662e 7669 6465 6f3a 0a20 2020 2020  elf.video:.     
-00020f90: 2020 2020 2020 2020 2020 2066 696c 655f             file_
-00020fa0: 6964 203d 2073 656c 662e 7669 6465 6f2e  id = self.video.
-00020fb0: 6669 6c65 5f69 640a 2020 2020 2020 2020  file_id.        
-00020fc0: 2020 2020 656c 6966 2073 656c 662e 616e      elif self.an
-00020fd0: 696d 6174 696f 6e3a 0a20 2020 2020 2020  imation:.       
-00020fe0: 2020 2020 2020 2020 2066 696c 655f 6964           file_id
-00020ff0: 203d 2073 656c 662e 616e 696d 6174 696f   = self.animatio
-00021000: 6e2e 6669 6c65 5f69 640a 2020 2020 2020  n.file_id.      
-00021010: 2020 2020 2020 656c 6966 2073 656c 662e        elif self.
-00021020: 766f 6963 653a 0a20 2020 2020 2020 2020  voice:.         
-00021030: 2020 2020 2020 2066 696c 655f 6964 203d         file_id =
-00021040: 2073 656c 662e 766f 6963 652e 6669 6c65   self.voice.file
-00021050: 5f69 640a 2020 2020 2020 2020 2020 2020  _id.            
-00021060: 656c 6966 2073 656c 662e 7374 6963 6b65  elif self.sticke
-00021070: 723a 0a20 2020 2020 2020 2020 2020 2020  r:.             
-00021080: 2020 2066 696c 655f 6964 203d 2073 656c     file_id = sel
-00021090: 662e 7374 6963 6b65 722e 6669 6c65 5f69  f.sticker.file_i
-000210a0: 640a 2020 2020 2020 2020 2020 2020 656c  d.            el
-000210b0: 6966 2073 656c 662e 7669 6465 6f5f 6e6f  if self.video_no
-000210c0: 7465 3a0a 2020 2020 2020 2020 2020 2020  te:.            
-000210d0: 2020 2020 6669 6c65 5f69 6420 3d20 7365      file_id = se
-000210e0: 6c66 2e76 6964 656f 5f6e 6f74 652e 6669  lf.video_note.fi
-000210f0: 6c65 5f69 640a 2020 2020 2020 2020 2020  le_id.          
-00021100: 2020 656c 6966 2073 656c 662e 636f 6e74    elif self.cont
-00021110: 6163 743a 0a20 2020 2020 2020 2020 2020  act:.           
-00021120: 2020 2020 2072 6574 7572 6e20 6177 6169       return awai
-00021130: 7420 7365 6c66 2e5f 636c 6965 6e74 2e73  t self._client.s
-00021140: 656e 645f 636f 6e74 6163 7428 0a20 2020  end_contact(.   
-00021150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021160: 2063 6861 745f 6964 2c0a 2020 2020 2020   chat_id,.      
-00021170: 2020 2020 2020 2020 2020 2020 2020 7068                ph
-00021180: 6f6e 655f 6e75 6d62 6572 3d73 656c 662e  one_number=self.
-00021190: 636f 6e74 6163 742e 7068 6f6e 655f 6e75  contact.phone_nu
-000211a0: 6d62 6572 2c0a 2020 2020 2020 2020 2020  mber,.          
-000211b0: 2020 2020 2020 2020 2020 6669 7273 745f            first_
-000211c0: 6e61 6d65 3d73 656c 662e 636f 6e74 6163  name=self.contac
-000211d0: 742e 6669 7273 745f 6e61 6d65 2c0a 2020  t.first_name,.  
-000211e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000211f0: 2020 6c61 7374 5f6e 616d 653d 7365 6c66    last_name=self
-00021200: 2e63 6f6e 7461 6374 2e6c 6173 745f 6e61  .contact.last_na
-00021210: 6d65 2c0a 2020 2020 2020 2020 2020 2020  me,.            
-00021220: 2020 2020 2020 2020 7663 6172 643d 7365          vcard=se
-00021230: 6c66 2e63 6f6e 7461 6374 2e76 6361 7264  lf.contact.vcard
-00021240: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00021250: 2020 2020 2020 6469 7361 626c 655f 6e6f        disable_no
-00021260: 7469 6669 6361 7469 6f6e 3d64 6973 6162  tification=disab
-00021270: 6c65 5f6e 6f74 6966 6963 6174 696f 6e2c  le_notification,
-00021280: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00021290: 2020 2020 206d 6573 7361 6765 5f74 6872       message_thr
-000212a0: 6561 645f 6964 3d6d 6573 7361 6765 5f74  ead_id=message_t
-000212b0: 6872 6561 645f 6964 2c0a 2020 2020 2020  hread_id,.      
-000212c0: 2020 2020 2020 2020 2020 2020 2020 7363                sc
-000212d0: 6865 6475 6c65 5f64 6174 653d 7363 6865  hedule_date=sche
-000212e0: 6475 6c65 5f64 6174 650a 2020 2020 2020  dule_date.      
-000212f0: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-00021300: 2020 2020 2020 2020 656c 6966 2073 656c          elif sel
-00021310: 662e 6c6f 6361 7469 6f6e 3a0a 2020 2020  f.location:.    
-00021320: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00021330: 726e 2061 7761 6974 2073 656c 662e 5f63  rn await self._c
-00021340: 6c69 656e 742e 7365 6e64 5f6c 6f63 6174  lient.send_locat
-00021350: 696f 6e28 0a20 2020 2020 2020 2020 2020  ion(.           
-00021360: 2020 2020 2020 2020 2063 6861 745f 6964           chat_id
-00021370: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00021380: 2020 2020 2020 6c61 7469 7475 6465 3d73        latitude=s
-00021390: 656c 662e 6c6f 6361 7469 6f6e 2e6c 6174  elf.location.lat
-000213a0: 6974 7564 652c 0a20 2020 2020 2020 2020  itude,.         
-000213b0: 2020 2020 2020 2020 2020 206c 6f6e 6769             longi
-000213c0: 7475 6465 3d73 656c 662e 6c6f 6361 7469  tude=self.locati
-000213d0: 6f6e 2e6c 6f6e 6769 7475 6465 2c0a 2020  on.longitude,.  
-000213e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000213f0: 2020 6469 7361 626c 655f 6e6f 7469 6669    disable_notifi
-00021400: 6361 7469 6f6e 3d64 6973 6162 6c65 5f6e  cation=disable_n
-00021410: 6f74 6966 6963 6174 696f 6e2c 0a20 2020  otification,.   
-00021420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021430: 206d 6573 7361 6765 5f74 6872 6561 645f   message_thread_
-00021440: 6964 3d6d 6573 7361 6765 5f74 6872 6561  id=message_threa
-00021450: 645f 6964 2c0a 2020 2020 2020 2020 2020  d_id,.          
-00021460: 2020 2020 2020 2020 2020 7363 6865 6475            schedu
-00021470: 6c65 5f64 6174 653d 7363 6865 6475 6c65  le_date=schedule
-00021480: 5f64 6174 650a 2020 2020 2020 2020 2020  _date.          
-00021490: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-000214a0: 2020 2020 656c 6966 2073 656c 662e 7665      elif self.ve
-000214b0: 6e75 653a 0a20 2020 2020 2020 2020 2020  nue:.           
-000214c0: 2020 2020 2072 6574 7572 6e20 6177 6169       return awai
-000214d0: 7420 7365 6c66 2e5f 636c 6965 6e74 2e73  t self._client.s
-000214e0: 656e 645f 7665 6e75 6528 0a20 2020 2020  end_venue(.     
-000214f0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00021500: 6861 745f 6964 2c0a 2020 2020 2020 2020  hat_id,.        
-00021510: 2020 2020 2020 2020 2020 2020 6c61 7469              lati
-00021520: 7475 6465 3d73 656c 662e 7665 6e75 652e  tude=self.venue.
-00021530: 6c6f 6361 7469 6f6e 2e6c 6174 6974 7564  location.latitud
-00021540: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
-00021550: 2020 2020 2020 206c 6f6e 6769 7475 6465         longitude
-00021560: 3d73 656c 662e 7665 6e75 652e 6c6f 6361  =self.venue.loca
-00021570: 7469 6f6e 2e6c 6f6e 6769 7475 6465 2c0a  tion.longitude,.
-00021580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021590: 2020 2020 7469 746c 653d 7365 6c66 2e76      title=self.v
-000215a0: 656e 7565 2e74 6974 6c65 2c0a 2020 2020  enue.title,.    
+00020860: 6622 5365 7276 6963 6520 6d65 7373 6167  f"Service messag
+00020870: 6573 2063 616e 6e6f 7420 6265 2063 6f70  es cannot be cop
+00020880: 6965 642e 2022 0a20 2020 2020 2020 2020  ied. ".         
+00020890: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+000208a0: 2263 6861 745f 6964 3a20 7b73 656c 662e  "chat_id: {self.
+000208b0: 6368 6174 2e69 647d 2c20 6d65 7373 6167  chat.id}, messag
+000208c0: 655f 6964 3a20 7b73 656c 662e 6964 7d22  e_id: {self.id}"
+000208d0: 290a 2020 2020 2020 2020 656c 6966 2073  ).        elif s
+000208e0: 656c 662e 6761 6d65 2061 6e64 206e 6f74  elf.game and not
+000208f0: 2061 7761 6974 2073 656c 662e 5f63 6c69   await self._cli
+00020900: 656e 742e 7374 6f72 6167 652e 6973 5f62  ent.storage.is_b
+00020910: 6f74 2829 3a0a 2020 2020 2020 2020 2020  ot():.          
+00020920: 2020 6c6f 672e 7761 726e 696e 6728 6622    log.warning(f"
+00020930: 5573 6572 7320 6361 6e6e 6f74 2073 656e  Users cannot sen
+00020940: 6420 6d65 7373 6167 6573 2077 6974 6820  d messages with 
+00020950: 4761 6d65 206d 6564 6961 2074 7970 652e  Game media type.
+00020960: 2022 0a20 2020 2020 2020 2020 2020 2020   ".             
+00020970: 2020 2020 2020 2020 2020 2066 2263 6861             f"cha
+00020980: 745f 6964 3a20 7b73 656c 662e 6368 6174  t_id: {self.chat
+00020990: 2e69 647d 2c20 6d65 7373 6167 655f 6964  .id}, message_id
+000209a0: 3a20 7b73 656c 662e 6964 7d22 290a 2020  : {self.id}").  
+000209b0: 2020 2020 2020 656c 6966 2073 656c 662e        elif self.
+000209c0: 656d 7074 793a 0a20 2020 2020 2020 2020  empty:.         
+000209d0: 2020 206c 6f67 2e77 6172 6e69 6e67 2866     log.warning(f
+000209e0: 2245 6d70 7479 206d 6573 7361 6765 7320  "Empty messages 
+000209f0: 6361 6e6e 6f74 2062 6520 636f 7069 6564  cannot be copied
+00020a00: 2e20 2229 0a20 2020 2020 2020 2065 6c69  . ").        eli
+00020a10: 6620 7365 6c66 2e74 6578 743a 0a20 2020  f self.text:.   
+00020a20: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00020a30: 6177 6169 7420 7365 6c66 2e5f 636c 6965  await self._clie
+00020a40: 6e74 2e73 656e 645f 6d65 7373 6167 6528  nt.send_message(
+00020a50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00020a60: 2063 6861 745f 6964 2c0a 2020 2020 2020   chat_id,.      
+00020a70: 2020 2020 2020 2020 2020 7465 7874 3d73            text=s
+00020a80: 656c 662e 7465 7874 2c0a 2020 2020 2020  elf.text,.      
+00020a90: 2020 2020 2020 2020 2020 656e 7469 7469            entiti
+00020aa0: 6573 3d73 656c 662e 656e 7469 7469 6573  es=self.entities
+00020ab0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00020ac0: 2020 7061 7273 655f 6d6f 6465 3d65 6e75    parse_mode=enu
+00020ad0: 6d73 2e50 6172 7365 4d6f 6465 2e44 4953  ms.ParseMode.DIS
+00020ae0: 4142 4c45 442c 0a20 2020 2020 2020 2020  ABLED,.         
+00020af0: 2020 2020 2020 2064 6973 6162 6c65 5f77         disable_w
+00020b00: 6562 5f70 6167 655f 7072 6576 6965 773d  eb_page_preview=
+00020b10: 6e6f 7420 7365 6c66 2e77 6562 5f70 6167  not self.web_pag
+00020b20: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
+00020b30: 2020 2064 6973 6162 6c65 5f6e 6f74 6966     disable_notif
+00020b40: 6963 6174 696f 6e3d 6469 7361 626c 655f  ication=disable_
+00020b50: 6e6f 7469 6669 6361 7469 6f6e 2c0a 2020  notification,.  
+00020b60: 2020 2020 2020 2020 2020 2020 2020 6d65                me
+00020b70: 7373 6167 655f 7468 7265 6164 5f69 643d  ssage_thread_id=
+00020b80: 6d65 7373 6167 655f 7468 7265 6164 5f69  message_thread_i
+00020b90: 642c 0a20 2020 2020 2020 2020 2020 2020  d,.             
+00020ba0: 2020 2072 6570 6c79 5f74 6f5f 6d65 7373     reply_to_mess
+00020bb0: 6167 655f 6964 3d72 6570 6c79 5f74 6f5f  age_id=reply_to_
+00020bc0: 6d65 7373 6167 655f 6964 2c0a 2020 2020  message_id,.    
+00020bd0: 2020 2020 2020 2020 2020 2020 7363 6865              sche
+00020be0: 6475 6c65 5f64 6174 653d 7363 6865 6475  dule_date=schedu
+00020bf0: 6c65 5f64 6174 652c 0a20 2020 2020 2020  le_date,.       
+00020c00: 2020 2020 2020 2020 2070 726f 7465 6374           protect
+00020c10: 5f63 6f6e 7465 6e74 3d70 726f 7465 6374  _content=protect
+00020c20: 5f63 6f6e 7465 6e74 2c0a 2020 2020 2020  _content,.      
+00020c30: 2020 2020 2020 2020 2020 7265 706c 795f            reply_
+00020c40: 6d61 726b 7570 3d73 656c 662e 7265 706c  markup=self.repl
+00020c50: 795f 6d61 726b 7570 2069 6620 7265 706c  y_markup if repl
+00020c60: 795f 6d61 726b 7570 2069 7320 6f62 6a65  y_markup is obje
+00020c70: 6374 2065 6c73 6520 7265 706c 795f 6d61  ct else reply_ma
+00020c80: 726b 7570 0a20 2020 2020 2020 2020 2020  rkup.           
+00020c90: 2029 0a20 2020 2020 2020 2065 6c69 6620   ).        elif 
+00020ca0: 7365 6c66 2e6d 6564 6961 3a0a 2020 2020  self.media:.    
+00020cb0: 2020 2020 2020 2020 7365 6e64 5f6d 6564          send_med
+00020cc0: 6961 203d 2070 6172 7469 616c 280a 2020  ia = partial(.  
+00020cd0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00020ce0: 6c66 2e5f 636c 6965 6e74 2e73 656e 645f  lf._client.send_
+00020cf0: 6361 6368 6564 5f6d 6564 6961 2c0a 2020  cached_media,.  
+00020d00: 2020 2020 2020 2020 2020 2020 2020 6368                ch
+00020d10: 6174 5f69 643d 6368 6174 5f69 642c 0a20  at_id=chat_id,. 
+00020d20: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+00020d30: 6973 6162 6c65 5f6e 6f74 6966 6963 6174  isable_notificat
+00020d40: 696f 6e3d 6469 7361 626c 655f 6e6f 7469  ion=disable_noti
+00020d50: 6669 6361 7469 6f6e 2c0a 2020 2020 2020  fication,.      
+00020d60: 2020 2020 2020 2020 2020 6d65 7373 6167            messag
+00020d70: 655f 7468 7265 6164 5f69 643d 6d65 7373  e_thread_id=mess
+00020d80: 6167 655f 7468 7265 6164 5f69 642c 0a20  age_thread_id,. 
+00020d90: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00020da0: 6570 6c79 5f74 6f5f 6d65 7373 6167 655f  eply_to_message_
+00020db0: 6964 3d72 6570 6c79 5f74 6f5f 6d65 7373  id=reply_to_mess
+00020dc0: 6167 655f 6964 2c0a 2020 2020 2020 2020  age_id,.        
+00020dd0: 2020 2020 2020 2020 7363 6865 6475 6c65          schedule
+00020de0: 5f64 6174 653d 7363 6865 6475 6c65 5f64  _date=schedule_d
+00020df0: 6174 652c 0a20 2020 2020 2020 2020 2020  ate,.           
+00020e00: 2020 2020 2070 726f 7465 6374 5f63 6f6e       protect_con
+00020e10: 7465 6e74 3d70 726f 7465 6374 5f63 6f6e  tent=protect_con
+00020e20: 7465 6e74 2c0a 2020 2020 2020 2020 2020  tent,.          
+00020e30: 2020 2020 2020 7265 706c 795f 6d61 726b        reply_mark
+00020e40: 7570 3d73 656c 662e 7265 706c 795f 6d61  up=self.reply_ma
+00020e50: 726b 7570 2069 6620 7265 706c 795f 6d61  rkup if reply_ma
+00020e60: 726b 7570 2069 7320 6f62 6a65 6374 2065  rkup is object e
+00020e70: 6c73 6520 7265 706c 795f 6d61 726b 7570  lse reply_markup
+00020e80: 0a20 2020 2020 2020 2020 2020 2029 0a0a  .            )..
+00020e90: 2020 2020 2020 2020 2020 2020 6966 2073              if s
+00020ea0: 656c 662e 7068 6f74 6f3a 0a20 2020 2020  elf.photo:.     
+00020eb0: 2020 2020 2020 2020 2020 2066 696c 655f             file_
+00020ec0: 6964 203d 2073 656c 662e 7068 6f74 6f2e  id = self.photo.
+00020ed0: 6669 6c65 5f69 640a 2020 2020 2020 2020  file_id.        
+00020ee0: 2020 2020 656c 6966 2073 656c 662e 6175      elif self.au
+00020ef0: 6469 6f3a 0a20 2020 2020 2020 2020 2020  dio:.           
+00020f00: 2020 2020 2066 696c 655f 6964 203d 2073       file_id = s
+00020f10: 656c 662e 6175 6469 6f2e 6669 6c65 5f69  elf.audio.file_i
+00020f20: 640a 2020 2020 2020 2020 2020 2020 656c  d.            el
+00020f30: 6966 2073 656c 662e 646f 6375 6d65 6e74  if self.document
+00020f40: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00020f50: 2020 6669 6c65 5f69 6420 3d20 7365 6c66    file_id = self
+00020f60: 2e64 6f63 756d 656e 742e 6669 6c65 5f69  .document.file_i
+00020f70: 640a 2020 2020 2020 2020 2020 2020 656c  d.            el
+00020f80: 6966 2073 656c 662e 7669 6465 6f3a 0a20  if self.video:. 
+00020f90: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00020fa0: 696c 655f 6964 203d 2073 656c 662e 7669  ile_id = self.vi
+00020fb0: 6465 6f2e 6669 6c65 5f69 640a 2020 2020  deo.file_id.    
+00020fc0: 2020 2020 2020 2020 656c 6966 2073 656c          elif sel
+00020fd0: 662e 616e 696d 6174 696f 6e3a 0a20 2020  f.animation:.   
+00020fe0: 2020 2020 2020 2020 2020 2020 2066 696c               fil
+00020ff0: 655f 6964 203d 2073 656c 662e 616e 696d  e_id = self.anim
+00021000: 6174 696f 6e2e 6669 6c65 5f69 640a 2020  ation.file_id.  
+00021010: 2020 2020 2020 2020 2020 656c 6966 2073            elif s
+00021020: 656c 662e 766f 6963 653a 0a20 2020 2020  elf.voice:.     
+00021030: 2020 2020 2020 2020 2020 2066 696c 655f             file_
+00021040: 6964 203d 2073 656c 662e 766f 6963 652e  id = self.voice.
+00021050: 6669 6c65 5f69 640a 2020 2020 2020 2020  file_id.        
+00021060: 2020 2020 656c 6966 2073 656c 662e 7374      elif self.st
+00021070: 6963 6b65 723a 0a20 2020 2020 2020 2020  icker:.         
+00021080: 2020 2020 2020 2066 696c 655f 6964 203d         file_id =
+00021090: 2073 656c 662e 7374 6963 6b65 722e 6669   self.sticker.fi
+000210a0: 6c65 5f69 640a 2020 2020 2020 2020 2020  le_id.          
+000210b0: 2020 656c 6966 2073 656c 662e 7669 6465    elif self.vide
+000210c0: 6f5f 6e6f 7465 3a0a 2020 2020 2020 2020  o_note:.        
+000210d0: 2020 2020 2020 2020 6669 6c65 5f69 6420          file_id 
+000210e0: 3d20 7365 6c66 2e76 6964 656f 5f6e 6f74  = self.video_not
+000210f0: 652e 6669 6c65 5f69 640a 2020 2020 2020  e.file_id.      
+00021100: 2020 2020 2020 656c 6966 2073 656c 662e        elif self.
+00021110: 636f 6e74 6163 743a 0a20 2020 2020 2020  contact:.       
+00021120: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00021130: 6177 6169 7420 7365 6c66 2e5f 636c 6965  await self._clie
+00021140: 6e74 2e73 656e 645f 636f 6e74 6163 7428  nt.send_contact(
+00021150: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00021160: 2020 2020 2063 6861 745f 6964 2c0a 2020       chat_id,.  
+00021170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021180: 2020 7068 6f6e 655f 6e75 6d62 6572 3d73    phone_number=s
+00021190: 656c 662e 636f 6e74 6163 742e 7068 6f6e  elf.contact.phon
+000211a0: 655f 6e75 6d62 6572 2c0a 2020 2020 2020  e_number,.      
+000211b0: 2020 2020 2020 2020 2020 2020 2020 6669                fi
+000211c0: 7273 745f 6e61 6d65 3d73 656c 662e 636f  rst_name=self.co
+000211d0: 6e74 6163 742e 6669 7273 745f 6e61 6d65  ntact.first_name
+000211e0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000211f0: 2020 2020 2020 6c61 7374 5f6e 616d 653d        last_name=
+00021200: 7365 6c66 2e63 6f6e 7461 6374 2e6c 6173  self.contact.las
+00021210: 745f 6e61 6d65 2c0a 2020 2020 2020 2020  t_name,.        
+00021220: 2020 2020 2020 2020 2020 2020 7663 6172              vcar
+00021230: 643d 7365 6c66 2e63 6f6e 7461 6374 2e76  d=self.contact.v
+00021240: 6361 7264 2c0a 2020 2020 2020 2020 2020  card,.          
+00021250: 2020 2020 2020 2020 2020 6469 7361 626c            disabl
+00021260: 655f 6e6f 7469 6669 6361 7469 6f6e 3d64  e_notification=d
+00021270: 6973 6162 6c65 5f6e 6f74 6966 6963 6174  isable_notificat
+00021280: 696f 6e2c 0a20 2020 2020 2020 2020 2020  ion,.           
+00021290: 2020 2020 2020 2020 206d 6573 7361 6765           message
+000212a0: 5f74 6872 6561 645f 6964 3d6d 6573 7361  _thread_id=messa
+000212b0: 6765 5f74 6872 6561 645f 6964 2c0a 2020  ge_thread_id,.  
+000212c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000212d0: 2020 7363 6865 6475 6c65 5f64 6174 653d    schedule_date=
+000212e0: 7363 6865 6475 6c65 5f64 6174 650a 2020  schedule_date.  
+000212f0: 2020 2020 2020 2020 2020 2020 2020 290a                ).
+00021300: 2020 2020 2020 2020 2020 2020 656c 6966              elif
+00021310: 2073 656c 662e 6c6f 6361 7469 6f6e 3a0a   self.location:.
+00021320: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021330: 7265 7475 726e 2061 7761 6974 2073 656c  return await sel
+00021340: 662e 5f63 6c69 656e 742e 7365 6e64 5f6c  f._client.send_l
+00021350: 6f63 6174 696f 6e28 0a20 2020 2020 2020  ocation(.       
+00021360: 2020 2020 2020 2020 2020 2020 2063 6861               cha
+00021370: 745f 6964 2c0a 2020 2020 2020 2020 2020  t_id,.          
+00021380: 2020 2020 2020 2020 2020 6c61 7469 7475            latitu
+00021390: 6465 3d73 656c 662e 6c6f 6361 7469 6f6e  de=self.location
+000213a0: 2e6c 6174 6974 7564 652c 0a20 2020 2020  .latitude,.     
+000213b0: 2020 2020 2020 2020 2020 2020 2020 206c                 l
+000213c0: 6f6e 6769 7475 6465 3d73 656c 662e 6c6f  ongitude=self.lo
+000213d0: 6361 7469 6f6e 2e6c 6f6e 6769 7475 6465  cation.longitude
+000213e0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000213f0: 2020 2020 2020 6469 7361 626c 655f 6e6f        disable_no
+00021400: 7469 6669 6361 7469 6f6e 3d64 6973 6162  tification=disab
+00021410: 6c65 5f6e 6f74 6966 6963 6174 696f 6e2c  le_notification,
+00021420: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00021430: 2020 2020 206d 6573 7361 6765 5f74 6872       message_thr
+00021440: 6561 645f 6964 3d6d 6573 7361 6765 5f74  ead_id=message_t
+00021450: 6872 6561 645f 6964 2c0a 2020 2020 2020  hread_id,.      
+00021460: 2020 2020 2020 2020 2020 2020 2020 7363                sc
+00021470: 6865 6475 6c65 5f64 6174 653d 7363 6865  hedule_date=sche
+00021480: 6475 6c65 5f64 6174 650a 2020 2020 2020  dule_date.      
+00021490: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+000214a0: 2020 2020 2020 2020 656c 6966 2073 656c          elif sel
+000214b0: 662e 7665 6e75 653a 0a20 2020 2020 2020  f.venue:.       
+000214c0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+000214d0: 6177 6169 7420 7365 6c66 2e5f 636c 6965  await self._clie
+000214e0: 6e74 2e73 656e 645f 7665 6e75 6528 0a20  nt.send_venue(. 
+000214f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021500: 2020 2063 6861 745f 6964 2c0a 2020 2020     chat_id,.    
+00021510: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021520: 6c61 7469 7475 6465 3d73 656c 662e 7665  latitude=self.ve
+00021530: 6e75 652e 6c6f 6361 7469 6f6e 2e6c 6174  nue.location.lat
+00021540: 6974 7564 652c 0a20 2020 2020 2020 2020  itude,.         
+00021550: 2020 2020 2020 2020 2020 206c 6f6e 6769             longi
+00021560: 7475 6465 3d73 656c 662e 7665 6e75 652e  tude=self.venue.
+00021570: 6c6f 6361 7469 6f6e 2e6c 6f6e 6769 7475  location.longitu
+00021580: 6465 2c0a 2020 2020 2020 2020 2020 2020  de,.            
+00021590: 2020 2020 2020 2020 7469 746c 653d 7365          title=se
+000215a0: 6c66 2e76 656e 7565 2e74 6974 6c65 2c0a  lf.venue.title,.
 000215b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000215c0: 6164 6472 6573 733d 7365 6c66 2e76 656e  address=self.ven
-000215d0: 7565 2e61 6464 7265 7373 2c0a 2020 2020  ue.address,.    
+000215c0: 2020 2020 6164 6472 6573 733d 7365 6c66      address=self
+000215d0: 2e76 656e 7565 2e61 6464 7265 7373 2c0a  .venue.address,.
 000215e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000215f0: 666f 7572 7371 7561 7265 5f69 643d 7365  foursquare_id=se
-00021600: 6c66 2e76 656e 7565 2e66 6f75 7273 7175  lf.venue.foursqu
-00021610: 6172 655f 6964 2c0a 2020 2020 2020 2020  are_id,.        
-00021620: 2020 2020 2020 2020 2020 2020 666f 7572              four
-00021630: 7371 7561 7265 5f74 7970 653d 7365 6c66  square_type=self
-00021640: 2e76 656e 7565 2e66 6f75 7273 7175 6172  .venue.foursquar
-00021650: 655f 7479 7065 2c0a 2020 2020 2020 2020  e_type,.        
-00021660: 2020 2020 2020 2020 2020 2020 6469 7361              disa
-00021670: 626c 655f 6e6f 7469 6669 6361 7469 6f6e  ble_notification
-00021680: 3d64 6973 6162 6c65 5f6e 6f74 6966 6963  =disable_notific
-00021690: 6174 696f 6e2c 0a20 2020 2020 2020 2020  ation,.         
-000216a0: 2020 2020 2020 2020 2020 206d 6573 7361             messa
-000216b0: 6765 5f74 6872 6561 645f 6964 3d6d 6573  ge_thread_id=mes
-000216c0: 7361 6765 5f74 6872 6561 645f 6964 2c0a  sage_thread_id,.
-000216d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000216e0: 2020 2020 7363 6865 6475 6c65 5f64 6174      schedule_dat
-000216f0: 653d 7363 6865 6475 6c65 5f64 6174 650a  e=schedule_date.
-00021700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021710: 290a 2020 2020 2020 2020 2020 2020 656c  ).            el
-00021720: 6966 2073 656c 662e 706f 6c6c 3a0a 2020  if self.poll:.  
-00021730: 2020 2020 2020 2020 2020 2020 2020 7265                re
-00021740: 7475 726e 2061 7761 6974 2073 656c 662e  turn await self.
-00021750: 5f63 6c69 656e 742e 7365 6e64 5f70 6f6c  _client.send_pol
-00021760: 6c28 0a20 2020 2020 2020 2020 2020 2020  l(.             
-00021770: 2020 2020 2020 2063 6861 745f 6964 2c0a         chat_id,.
-00021780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021790: 2020 2020 7175 6573 7469 6f6e 3d73 656c      question=sel
-000217a0: 662e 706f 6c6c 2e71 7565 7374 696f 6e2c  f.poll.question,
-000217b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000217c0: 2020 2020 206f 7074 696f 6e73 3d5b 6f70       options=[op
-000217d0: 742e 7465 7874 2066 6f72 206f 7074 2069  t.text for opt i
-000217e0: 6e20 7365 6c66 2e70 6f6c 6c2e 6f70 7469  n self.poll.opti
-000217f0: 6f6e 735d 2c0a 2020 2020 2020 2020 2020  ons],.          
-00021800: 2020 2020 2020 2020 2020 6469 7361 626c            disabl
-00021810: 655f 6e6f 7469 6669 6361 7469 6f6e 3d64  e_notification=d
-00021820: 6973 6162 6c65 5f6e 6f74 6966 6963 6174  isable_notificat
-00021830: 696f 6e2c 0a20 2020 2020 2020 2020 2020  ion,.           
-00021840: 2020 2020 2020 2020 206d 6573 7361 6765           message
-00021850: 5f74 6872 6561 645f 6964 3d6d 6573 7361  _thread_id=messa
-00021860: 6765 5f74 6872 6561 645f 6964 2c0a 2020  ge_thread_id,.  
-00021870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021880: 2020 7363 6865 6475 6c65 5f64 6174 653d    schedule_date=
-00021890: 7363 6865 6475 6c65 5f64 6174 650a 2020  schedule_date.  
-000218a0: 2020 2020 2020 2020 2020 2020 2020 290a                ).
-000218b0: 2020 2020 2020 2020 2020 2020 656c 6966              elif
-000218c0: 2073 656c 662e 6761 6d65 3a0a 2020 2020   self.game:.    
-000218d0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-000218e0: 726e 2061 7761 6974 2073 656c 662e 5f63  rn await self._c
-000218f0: 6c69 656e 742e 7365 6e64 5f67 616d 6528  lient.send_game(
-00021900: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00021910: 2020 2020 2063 6861 745f 6964 2c0a 2020       chat_id,.  
-00021920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021930: 2020 6761 6d65 5f73 686f 7274 5f6e 616d    game_short_nam
-00021940: 653d 7365 6c66 2e67 616d 652e 7368 6f72  e=self.game.shor
-00021950: 745f 6e61 6d65 2c0a 2020 2020 2020 2020  t_name,.        
-00021960: 2020 2020 2020 2020 2020 2020 6469 7361              disa
-00021970: 626c 655f 6e6f 7469 6669 6361 7469 6f6e  ble_notification
-00021980: 3d64 6973 6162 6c65 5f6e 6f74 6966 6963  =disable_notific
-00021990: 6174 696f 6e2c 0a20 2020 2020 2020 2020  ation,.         
-000219a0: 2020 2020 2020 2020 2020 206d 6573 7361             messa
-000219b0: 6765 5f74 6872 6561 645f 6964 3d6d 6573  ge_thread_id=mes
-000219c0: 7361 6765 5f74 6872 6561 645f 6964 0a20  sage_thread_id. 
-000219d0: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-000219e0: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
-000219f0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-00021a00: 2020 2072 6169 7365 2056 616c 7565 4572     raise ValueEr
-00021a10: 726f 7228 2255 6e6b 6e6f 776e 206d 6564  ror("Unknown med
-00021a20: 6961 2074 7970 6522 290a 0a20 2020 2020  ia type")..     
-00021a30: 2020 2020 2020 2069 6620 7365 6c66 2e73         if self.s
-00021a40: 7469 636b 6572 206f 7220 7365 6c66 2e76  ticker or self.v
-00021a50: 6964 656f 5f6e 6f74 653a 2020 2320 5374  ideo_note:  # St
-00021a60: 6963 6b65 7220 616e 6420 5669 6465 6f4e  icker and VideoN
-00021a70: 6f74 6520 7368 6f75 6c64 2068 6176 6520  ote should have 
-00021a80: 6e6f 2063 6170 7469 6f6e 0a20 2020 2020  no caption.     
-00021a90: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00021aa0: 6e20 6177 6169 7420 7365 6e64 5f6d 6564  n await send_med
-00021ab0: 6961 280a 2020 2020 2020 2020 2020 2020  ia(.            
-00021ac0: 2020 2020 2020 2020 6669 6c65 5f69 643d          file_id=
-00021ad0: 6669 6c65 5f69 642c 0a20 2020 2020 2020  file_id,.       
-00021ae0: 2020 2020 2020 2020 2020 2020 206d 6573               mes
-00021af0: 7361 6765 5f74 6872 6561 645f 6964 3d6d  sage_thread_id=m
-00021b00: 6573 7361 6765 5f74 6872 6561 645f 6964  essage_thread_id
-00021b10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00021b20: 2029 0a20 2020 2020 2020 2020 2020 2065   ).            e
-00021b30: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-00021b40: 2020 2020 2069 6620 6361 7074 696f 6e20       if caption 
-00021b50: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
-00021b60: 2020 2020 2020 2020 2020 2020 2063 6170               cap
-00021b70: 7469 6f6e 203d 2073 656c 662e 6361 7074  tion = self.capt
-00021b80: 696f 6e20 6f72 2022 220a 2020 2020 2020  ion or "".      
-00021b90: 2020 2020 2020 2020 2020 2020 2020 6361                ca
-00021ba0: 7074 696f 6e5f 656e 7469 7469 6573 203d  ption_entities =
-00021bb0: 2073 656c 662e 6361 7074 696f 6e5f 656e   self.caption_en
-00021bc0: 7469 7469 6573 0a0a 2020 2020 2020 2020  tities..        
-00021bd0: 2020 2020 2020 2020 7265 7475 726e 2061          return a
-00021be0: 7761 6974 2073 656e 645f 6d65 6469 6128  wait send_media(
-00021bf0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00021c00: 2020 2020 2066 696c 655f 6964 3d66 696c       file_id=fil
-00021c10: 655f 6964 2c0a 2020 2020 2020 2020 2020  e_id,.          
-00021c20: 2020 2020 2020 2020 2020 6361 7074 696f            captio
-00021c30: 6e3d 6361 7074 696f 6e2c 0a20 2020 2020  n=caption,.     
-00021c40: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-00021c50: 6172 7365 5f6d 6f64 653d 7061 7273 655f  arse_mode=parse_
-00021c60: 6d6f 6465 2c0a 2020 2020 2020 2020 2020  mode,.          
-00021c70: 2020 2020 2020 2020 2020 6361 7074 696f            captio
-00021c80: 6e5f 656e 7469 7469 6573 3d63 6170 7469  n_entities=capti
-00021c90: 6f6e 5f65 6e74 6974 6965 732c 0a20 2020  on_entities,.   
-00021ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021cb0: 206d 6573 7361 6765 5f74 6872 6561 645f   message_thread_
-00021cc0: 6964 3d6d 6573 7361 6765 5f74 6872 6561  id=message_threa
-00021cd0: 645f 6964 0a20 2020 2020 2020 2020 2020  d_id.           
-00021ce0: 2020 2020 2029 0a20 2020 2020 2020 2065       ).        e
-00021cf0: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-00021d00: 2072 6169 7365 2056 616c 7565 4572 726f   raise ValueErro
-00021d10: 7228 2243 616e 2774 2063 6f70 7920 7468  r("Can't copy th
-00021d20: 6973 206d 6573 7361 6765 2229 0a0a 2020  is message")..  
-00021d30: 2020 6173 796e 6320 6465 6620 6465 6c65    async def dele
-00021d40: 7465 2873 656c 662c 2072 6576 6f6b 653a  te(self, revoke:
-00021d50: 2062 6f6f 6c20 3d20 5472 7565 293a 0a20   bool = True):. 
-00021d60: 2020 2020 2020 2022 2222 426f 756e 6420         """Bound 
-00021d70: 6d65 7468 6f64 202a 6465 6c65 7465 2a20  method *delete* 
-00021d80: 6f66 203a 6f62 6a3a 607e 7079 726f 6772  of :obj:`~pyrogr
-00021d90: 616d 2e74 7970 6573 2e4d 6573 7361 6765  am.types.Message
-00021da0: 602e 0a0a 2020 2020 2020 2020 5573 6520  `...        Use 
-00021db0: 6173 2061 2073 686f 7274 6375 7420 666f  as a shortcut fo
-00021dc0: 723a 0a0a 2020 2020 2020 2020 2e2e 2063  r:..        .. c
-00021dd0: 6f64 652d 626c 6f63 6b3a 3a20 7079 7468  ode-block:: pyth
-00021de0: 6f6e 0a0a 2020 2020 2020 2020 2020 2020  on..            
-00021df0: 6177 6169 7420 636c 6965 6e74 2e64 656c  await client.del
-00021e00: 6574 655f 6d65 7373 6167 6573 280a 2020  ete_messages(.  
-00021e10: 2020 2020 2020 2020 2020 2020 2020 6368                ch
-00021e20: 6174 5f69 643d 6368 6174 5f69 642c 0a20  at_id=chat_id,. 
-00021e30: 2020 2020 2020 2020 2020 2020 2020 206d                 m
-00021e40: 6573 7361 6765 5f69 6473 3d6d 6573 7361  essage_ids=messa
-00021e50: 6765 2e69 640a 2020 2020 2020 2020 2020  ge.id.          
-00021e60: 2020 290a 0a20 2020 2020 2020 2045 7861    )..        Exa
-00021e70: 6d70 6c65 3a0a 2020 2020 2020 2020 2020  mple:.          
-00021e80: 2020 2e2e 2063 6f64 652d 626c 6f63 6b3a    .. code-block:
-00021e90: 3a20 7079 7468 6f6e 0a0a 2020 2020 2020  : python..      
-00021ea0: 2020 2020 2020 2020 2020 6177 6169 7420            await 
-00021eb0: 6d65 7373 6167 652e 6465 6c65 7465 2829  message.delete()
-00021ec0: 0a0a 2020 2020 2020 2020 5061 7261 6d65  ..        Parame
-00021ed0: 7465 7273 3a0a 2020 2020 2020 2020 2020  ters:.          
-00021ee0: 2020 7265 766f 6b65 2028 6060 626f 6f6c    revoke (``bool
-00021ef0: 6060 2c20 2a6f 7074 696f 6e61 6c2a 293a  ``, *optional*):
-00021f00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00021f10: 2044 656c 6574 6573 206d 6573 7361 6765   Deletes message
-00021f20: 7320 6f6e 2062 6f74 6820 7061 7274 732e  s on both parts.
-00021f30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00021f40: 2054 6869 7320 6973 206f 6e6c 7920 666f   This is only fo
-00021f50: 7220 7072 6976 6174 6520 636c 6f75 6420  r private cloud 
-00021f60: 6368 6174 7320 616e 6420 6e6f 726d 616c  chats and normal
-00021f70: 2067 726f 7570 732c 206d 6573 7361 6765   groups, message
-00021f80: 7320 6f6e 0a20 2020 2020 2020 2020 2020  s on.           
-00021f90: 2020 2020 2063 6861 6e6e 656c 7320 616e       channels an
-00021fa0: 6420 7375 7065 7267 726f 7570 7320 6172  d supergroups ar
-00021fb0: 6520 616c 7761 7973 2072 6576 6f6b 6564  e always revoked
-00021fc0: 2028 692e 652e 3a20 6465 6c65 7465 6420   (i.e.: deleted 
-00021fd0: 666f 7220 6576 6572 796f 6e65 292e 0a20  for everyone).. 
-00021fe0: 2020 2020 2020 2020 2020 2020 2020 2044                 D
-00021ff0: 6566 6175 6c74 7320 746f 2054 7275 652e  efaults to True.
-00022000: 0a0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
-00022010: 733a 0a20 2020 2020 2020 2020 2020 2054  s:.            T
-00022020: 7275 6520 6f6e 2073 7563 6365 7373 2c20  rue on success, 
-00022030: 4661 6c73 6520 6f74 6865 7277 6973 652e  False otherwise.
-00022040: 0a0a 2020 2020 2020 2020 5261 6973 6573  ..        Raises
-00022050: 3a0a 2020 2020 2020 2020 2020 2020 5250  :.            RP
-00022060: 4345 7272 6f72 3a20 496e 2063 6173 6520  CError: In case 
-00022070: 6f66 2061 2054 656c 6567 7261 6d20 5250  of a Telegram RP
-00022080: 4320 6572 726f 722e 0a20 2020 2020 2020  C error..       
-00022090: 2022 2222 0a20 2020 2020 2020 2072 6574   """.        ret
-000220a0: 7572 6e20 6177 6169 7420 7365 6c66 2e5f  urn await self._
-000220b0: 636c 6965 6e74 2e64 656c 6574 655f 6d65  client.delete_me
-000220c0: 7373 6167 6573 280a 2020 2020 2020 2020  ssages(.        
-000220d0: 2020 2020 6368 6174 5f69 643d 7365 6c66      chat_id=self
-000220e0: 2e63 6861 742e 6964 2c0a 2020 2020 2020  .chat.id,.      
-000220f0: 2020 2020 2020 6d65 7373 6167 655f 6964        message_id
-00022100: 733d 7365 6c66 2e69 642c 0a20 2020 2020  s=self.id,.     
-00022110: 2020 2020 2020 2072 6576 6f6b 653d 7265         revoke=re
-00022120: 766f 6b65 0a20 2020 2020 2020 2029 0a0a  voke.        )..
-00022130: 2020 2020 6173 796e 6320 6465 6620 636c      async def cl
-00022140: 6963 6b28 7365 6c66 2c20 783a 2055 6e69  ick(self, x: Uni
-00022150: 6f6e 5b69 6e74 2c20 7374 725d 203d 2030  on[int, str] = 0
-00022160: 2c20 793a 2069 6e74 203d 204e 6f6e 652c  , y: int = None,
-00022170: 2071 756f 7465 3a20 626f 6f6c 203d 204e   quote: bool = N
-00022180: 6f6e 652c 2074 696d 656f 7574 3a20 696e  one, timeout: in
-00022190: 7420 3d20 3130 293a 0a20 2020 2020 2020  t = 10):.       
-000221a0: 2022 2222 426f 756e 6420 6d65 7468 6f64   """Bound method
-000221b0: 202a 636c 6963 6b2a 206f 6620 3a6f 626a   *click* of :obj
-000221c0: 3a60 7e70 7972 6f67 7261 6d2e 7479 7065  :`~pyrogram.type
-000221d0: 732e 4d65 7373 6167 6560 2e0a 0a20 2020  s.Message`...   
-000221e0: 2020 2020 2055 7365 2061 7320 6120 7368       Use as a sh
-000221f0: 6f72 7463 7574 2066 6f72 2063 6c69 636b  ortcut for click
-00022200: 696e 6720 6120 6275 7474 6f6e 2061 7474  ing a button att
-00022210: 6163 6865 6420 746f 2074 6865 206d 6573  ached to the mes
-00022220: 7361 6765 2069 6e73 7465 6164 206f 663a  sage instead of:
-00022230: 0a0a 2020 2020 2020 2020 2d20 436c 6963  ..        - Clic
-00022240: 6b69 6e67 2069 6e6c 696e 6520 6275 7474  king inline butt
-00022250: 6f6e 733a 0a0a 2020 2020 2020 2020 2e2e  ons:..        ..
-00022260: 2063 6f64 652d 626c 6f63 6b3a 3a20 7079   code-block:: py
-00022270: 7468 6f6e 0a0a 2020 2020 2020 2020 2020  thon..          
-00022280: 2020 6177 6169 7420 636c 6965 6e74 2e72    await client.r
-00022290: 6571 7565 7374 5f63 616c 6c62 6163 6b5f  equest_callback_
-000222a0: 616e 7377 6572 280a 2020 2020 2020 2020  answer(.        
-000222b0: 2020 2020 2020 2020 6368 6174 5f69 643d          chat_id=
-000222c0: 6d65 7373 6167 652e 6368 6174 2e69 642c  message.chat.id,
-000222d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000222e0: 206d 6573 7361 6765 5f69 643d 6d65 7373   message_id=mess
-000222f0: 6167 652e 6964 2c0a 2020 2020 2020 2020  age.id,.        
-00022300: 2020 2020 2020 2020 6361 6c6c 6261 636b          callback
-00022310: 5f64 6174 613d 6d65 7373 6167 652e 7265  _data=message.re
-00022320: 706c 795f 6d61 726b 7570 5b69 5d5b 6a5d  ply_markup[i][j]
-00022330: 2e63 616c 6c62 6163 6b5f 6461 7461 0a20  .callback_data. 
-00022340: 2020 2020 2020 2020 2020 2029 0a0a 2020             )..  
-00022350: 2020 2020 2020 2d20 436c 6963 6b69 6e67        - Clicking
-00022360: 206e 6f72 6d61 6c20 6275 7474 6f6e 733a   normal buttons:
-00022370: 0a0a 2020 2020 2020 2020 2e2e 2063 6f64  ..        .. cod
-00022380: 652d 626c 6f63 6b3a 3a20 7079 7468 6f6e  e-block:: python
-00022390: 0a0a 2020 2020 2020 2020 2020 2020 6177  ..            aw
-000223a0: 6169 7420 636c 6965 6e74 2e73 656e 645f  ait client.send_
-000223b0: 6d65 7373 6167 6528 0a20 2020 2020 2020  message(.       
-000223c0: 2020 2020 2020 2020 2063 6861 745f 6964           chat_id
-000223d0: 3d6d 6573 7361 6765 2e63 6861 742e 6964  =message.chat.id
-000223e0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000223f0: 2020 7465 7874 3d6d 6573 7361 6765 2e72    text=message.r
-00022400: 6570 6c79 5f6d 6172 6b75 705b 695d 5b6a  eply_markup[i][j
-00022410: 5d2e 7465 7874 0a20 2020 2020 2020 2020  ].text.         
-00022420: 2020 2029 0a0a 2020 2020 2020 2020 4578     )..        Ex
-00022430: 616d 706c 653a 0a20 2020 2020 2020 2020  ample:.         
-00022440: 2020 2054 6869 7320 6d65 7468 6f64 2063     This method c
-00022450: 616e 2062 6520 7573 6564 2069 6e20 7468  an be used in th
-00022460: 7265 6520 6469 6666 6572 656e 7420 7761  ree different wa
-00022470: 7973 3a0a 0a20 2020 2020 2020 2020 2020  ys:..           
-00022480: 2031 2e20 2050 6173 7320 6f6e 6520 696e   1.  Pass one in
-00022490: 7465 6765 7220 6172 6775 6d65 6e74 206f  teger argument o
-000224a0: 6e6c 7920 2865 2e67 2e3a 2060 602e 636c  nly (e.g.: ``.cl
-000224b0: 6963 6b28 3229 6060 2c20 746f 2063 6c69  ick(2)``, to cli
-000224c0: 636b 2061 2062 7574 746f 6e20 6174 2069  ck a button at i
-000224d0: 6e64 6578 2032 292e 0a20 2020 2020 2020  ndex 2)..       
-000224e0: 2020 2020 2020 2020 2042 7574 746f 6e73           Buttons
-000224f0: 2061 7265 2063 6f75 6e74 6564 206c 6566   are counted lef
-00022500: 7420 746f 2072 6967 6874 2c20 7374 6172  t to right, star
-00022510: 7469 6e67 2066 726f 6d20 7468 6520 746f  ting from the to
-00022520: 702e 0a0a 2020 2020 2020 2020 2020 2020  p...            
-00022530: 322e 2020 5061 7373 2074 776f 2069 6e74  2.  Pass two int
-00022540: 6567 6572 2061 7267 756d 656e 7473 2028  eger arguments (
-00022550: 652e 672e 3a20 6060 2e63 6c69 636b 2831  e.g.: ``.click(1
-00022560: 2c20 3029 6060 2c20 746f 2063 6c69 636b  , 0)``, to click
-00022570: 2061 2062 7574 746f 6e20 6174 2070 6f73   a button at pos
-00022580: 6974 696f 6e20 2831 2c20 3029 292e 0a20  ition (1, 0)).. 
-00022590: 2020 2020 2020 2020 2020 2020 2020 2054                 T
-000225a0: 6865 206f 7269 6769 6e20 2830 2c20 3029  he origin (0, 0)
-000225b0: 2069 7320 746f 702d 6c65 6674 2e0a 0a20   is top-left... 
-000225c0: 2020 2020 2020 2020 2020 2033 2e20 2050             3.  P
-000225d0: 6173 7320 6f6e 6520 7374 7269 6e67 2061  ass one string a
-000225e0: 7267 756d 656e 7420 6f6e 6c79 2028 652e  rgument only (e.
-000225f0: 672e 3a20 6060 2e63 6c69 636b 2822 5365  g.: ``.click("Se
-00022600: 7474 696e 6773 2229 6060 2c20 746f 2063  ttings")``, to c
-00022610: 6c69 636b 2061 2062 7574 746f 6e20 6279  lick a button by
-00022620: 2075 7369 6e67 2069 7473 206c 6162 656c   using its label
-00022630: 292e 0a20 2020 2020 2020 2020 2020 2020  )..             
-00022640: 2020 204f 6e6c 7920 7468 6520 6669 7273     Only the firs
-00022650: 7420 6d61 7463 6869 6e67 2062 7574 746f  t matching butto
-00022660: 6e20 7769 6c6c 2062 6520 7072 6573 7365  n will be presse
-00022670: 642e 0a0a 2020 2020 2020 2020 5061 7261  d...        Para
-00022680: 6d65 7465 7273 3a0a 2020 2020 2020 2020  meters:.        
-00022690: 2020 2020 7820 2860 6069 6e74 6060 207c      x (``int`` |
-000226a0: 2060 6073 7472 6060 293a 0a20 2020 2020   ``str``):.     
-000226b0: 2020 2020 2020 2020 2020 2055 7365 6420             Used 
-000226c0: 6173 2069 6e74 6567 6572 2069 6e64 6578  as integer index
-000226d0: 2c20 696e 7465 6765 7220 6162 7363 6973  , integer abscis
-000226e0: 7361 2028 696e 2070 6169 7220 7769 7468  sa (in pair with
-000226f0: 2079 2920 6f72 2061 7320 7374 7269 6e67   y) or as string
-00022700: 206c 6162 656c 2e0a 2020 2020 2020 2020   label..        
-00022710: 2020 2020 2020 2020 4465 6661 756c 7473          Defaults
-00022720: 2074 6f20 3020 2866 6972 7374 2062 7574   to 0 (first but
-00022730: 746f 6e29 2e0a 0a20 2020 2020 2020 2020  ton)...         
-00022740: 2020 2079 2028 6060 696e 7460 602c 202a     y (``int``, *
-00022750: 6f70 7469 6f6e 616c 2a29 3a0a 2020 2020  optional*):.    
-00022760: 2020 2020 2020 2020 2020 2020 5573 6564              Used
-00022770: 2061 7320 6f72 6469 6e61 7465 206f 6e6c   as ordinate onl
-00022780: 7920 2869 6e20 7061 6972 2077 6974 6820  y (in pair with 
-00022790: 7829 2e0a 0a20 2020 2020 2020 2020 2020  x)...           
-000227a0: 2071 756f 7465 2028 6060 626f 6f6c 6060   quote (``bool``
-000227b0: 2c20 2a6f 7074 696f 6e61 6c2a 293a 0a20  , *optional*):. 
-000227c0: 2020 2020 2020 2020 2020 2020 2020 2055                 U
-000227d0: 7365 6675 6c20 666f 7220 6e6f 726d 616c  seful for normal
-000227e0: 2062 7574 746f 6e73 206f 6e6c 792c 2077   buttons only, w
-000227f0: 6865 7265 2070 7265 7373 696e 6720 6974  here pressing it
-00022800: 2077 696c 6c20 7265 7375 6c74 2069 6e20   will result in 
-00022810: 6120 6e65 7720 6d65 7373 6167 6520 7365  a new message se
-00022820: 6e74 2e0a 2020 2020 2020 2020 2020 2020  nt..            
-00022830: 2020 2020 4966 2060 6054 7275 6560 602c      If ``True``,
-00022840: 2074 6865 206d 6573 7361 6765 2077 696c   the message wil
-00022850: 6c20 6265 2073 656e 7420 6173 2061 2072  l be sent as a r
-00022860: 6570 6c79 2074 6f20 7468 6973 206d 6573  eply to this mes
-00022870: 7361 6765 2e0a 2020 2020 2020 2020 2020  sage..          
-00022880: 2020 2020 2020 4465 6661 756c 7473 2074        Defaults t
-00022890: 6f20 6060 5472 7565 6060 2069 6e20 6772  o ``True`` in gr
-000228a0: 6f75 7020 6368 6174 7320 616e 6420 6060  oup chats and ``
-000228b0: 4661 6c73 6560 6020 696e 2070 7269 7661  False`` in priva
-000228c0: 7465 2063 6861 7473 2e0a 0a20 2020 2020  te chats...     
-000228d0: 2020 2020 2020 2074 696d 656f 7574 2028         timeout (
-000228e0: 6060 696e 7460 602c 202a 6f70 7469 6f6e  ``int``, *option
-000228f0: 616c 2a29 3a0a 2020 2020 2020 2020 2020  al*):.          
-00022900: 2020 2020 2020 5469 6d65 6f75 7420 696e        Timeout in
-00022910: 2073 6563 6f6e 6473 2e0a 0a20 2020 2020   seconds...     
-00022920: 2020 2052 6574 7572 6e73 3a0a 2020 2020     Returns:.    
-00022930: 2020 2020 2020 2020 2d20 2020 5468 6520          -   The 
-00022940: 7265 7375 6c74 206f 6620 3a6d 6574 683a  result of :meth:
-00022950: 607e 7079 726f 6772 616d 2e43 6c69 656e  `~pyrogram.Clien
-00022960: 742e 7265 7175 6573 745f 6361 6c6c 6261  t.request_callba
-00022970: 636b 5f61 6e73 7765 7260 2069 6e20 6361  ck_answer` in ca
-00022980: 7365 206f 6620 696e 6c69 6e65 2063 616c  se of inline cal
-00022990: 6c62 6163 6b20 6275 7474 6f6e 2063 6c69  lback button cli
-000229a0: 636b 732e 0a20 2020 2020 2020 2020 2020  cks..           
-000229b0: 202d 2020 2054 6865 2072 6573 756c 7420   -   The result 
-000229c0: 6f66 203a 6d65 7468 3a60 7e4d 6573 7361  of :meth:`~Messa
-000229d0: 6765 2e72 6570 6c79 2829 6020 696e 2063  ge.reply()` in c
-000229e0: 6173 6520 6f66 206e 6f72 6d61 6c20 6275  ase of normal bu
-000229f0: 7474 6f6e 2063 6c69 636b 732e 0a20 2020  tton clicks..   
-00022a00: 2020 2020 2020 2020 202d 2020 2041 2073           -   A s
-00022a10: 7472 696e 6720 696e 2063 6173 6520 7468  tring in case th
-00022a20: 6520 696e 6c69 6e65 2062 7574 746f 6e20  e inline button 
-00022a30: 6973 2061 2055 524c 2c20 6120 2a73 7769  is a URL, a *swi
-00022a40: 7463 685f 696e 6c69 6e65 5f71 7565 7279  tch_inline_query
-00022a50: 2a20 6f72 2061 0a20 2020 2020 2020 2020  * or a.         
-00022a60: 2020 2020 2020 202a 7377 6974 6368 5f69         *switch_i
-00022a70: 6e6c 696e 655f 7175 6572 795f 6375 7272  nline_query_curr
-00022a80: 656e 745f 6368 6174 2a20 6275 7474 6f6e  ent_chat* button
-00022a90: 2e0a 0a20 2020 2020 2020 2052 6169 7365  ...        Raise
-00022aa0: 733a 0a20 2020 2020 2020 2020 2020 2052  s:.            R
-00022ab0: 5043 4572 726f 723a 2049 6e20 6361 7365  PCError: In case
-00022ac0: 206f 6620 6120 5465 6c65 6772 616d 2052   of a Telegram R
-00022ad0: 5043 2065 7272 6f72 2e0a 2020 2020 2020  PC error..      
-00022ae0: 2020 2020 2020 5661 6c75 6545 7272 6f72        ValueError
-00022af0: 3a20 496e 2063 6173 6520 7468 6520 7072  : In case the pr
-00022b00: 6f76 6964 6564 2069 6e64 6578 206f 7220  ovided index or 
-00022b10: 706f 7369 7469 6f6e 2069 7320 6f75 7420  position is out 
-00022b20: 6f66 2072 616e 6765 206f 7220 7468 6520  of range or the 
-00022b30: 6275 7474 6f6e 206c 6162 656c 2077 6173  button label was
-00022b40: 206e 6f74 2066 6f75 6e64 2e0a 2020 2020   not found..    
-00022b50: 2020 2020 2020 2020 5469 6d65 6f75 7445          TimeoutE
-00022b60: 7272 6f72 3a20 496e 2063 6173 652c 2061  rror: In case, a
-00022b70: 6674 6572 2063 6c69 636b 696e 6720 616e  fter clicking an
-00022b80: 2069 6e6c 696e 6520 6275 7474 6f6e 2c20   inline button, 
-00022b90: 7468 6520 626f 7420 6661 696c 7320 746f  the bot fails to
-00022ba0: 2061 6e73 7765 7220 7769 7468 696e 2074   answer within t
-00022bb0: 6865 2074 696d 656f 7574 2e0a 2020 2020  he timeout..    
-00022bc0: 2020 2020 2222 220a 0a20 2020 2020 2020      """..       
-00022bd0: 2069 6620 6973 696e 7374 616e 6365 2873   if isinstance(s
-00022be0: 656c 662e 7265 706c 795f 6d61 726b 7570  elf.reply_markup
-00022bf0: 2c20 7479 7065 732e 5265 706c 794b 6579  , types.ReplyKey
-00022c00: 626f 6172 644d 6172 6b75 7029 3a0a 2020  boardMarkup):.  
-00022c10: 2020 2020 2020 2020 2020 6b65 7962 6f61            keyboa
-00022c20: 7264 203d 2073 656c 662e 7265 706c 795f  rd = self.reply_
-00022c30: 6d61 726b 7570 2e6b 6579 626f 6172 640a  markup.keyboard.
-00022c40: 2020 2020 2020 2020 2020 2020 6973 5f69              is_i
-00022c50: 6e6c 696e 6520 3d20 4661 6c73 650a 2020  nline = False.  
-00022c60: 2020 2020 2020 656c 6966 2069 7369 6e73        elif isins
-00022c70: 7461 6e63 6528 7365 6c66 2e72 6570 6c79  tance(self.reply
-00022c80: 5f6d 6172 6b75 702c 2074 7970 6573 2e49  _markup, types.I
-00022c90: 6e6c 696e 654b 6579 626f 6172 644d 6172  nlineKeyboardMar
-00022ca0: 6b75 7029 3a0a 2020 2020 2020 2020 2020  kup):.          
-00022cb0: 2020 6b65 7962 6f61 7264 203d 2073 656c    keyboard = sel
-00022cc0: 662e 7265 706c 795f 6d61 726b 7570 2e69  f.reply_markup.i
-00022cd0: 6e6c 696e 655f 6b65 7962 6f61 7264 0a20  nline_keyboard. 
-00022ce0: 2020 2020 2020 2020 2020 2069 735f 696e             is_in
-00022cf0: 6c69 6e65 203d 2054 7275 650a 2020 2020  line = True.    
-00022d00: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00022d10: 2020 2020 2020 7261 6973 6520 5661 6c75        raise Valu
-00022d20: 6545 7272 6f72 2822 5468 6520 6d65 7373  eError("The mess
-00022d30: 6167 6520 646f 6573 6e27 7420 636f 6e74  age doesn't cont
-00022d40: 6169 6e20 616e 7920 6b65 7962 6f61 7264  ain any keyboard
-00022d50: 2229 0a0a 2020 2020 2020 2020 6966 2069  ")..        if i
-00022d60: 7369 6e73 7461 6e63 6528 782c 2069 6e74  sinstance(x, int
-00022d70: 2920 616e 6420 7920 6973 204e 6f6e 653a  ) and y is None:
-00022d80: 0a20 2020 2020 2020 2020 2020 2074 7279  .            try
-00022d90: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00022da0: 2020 6275 7474 6f6e 203d 205b 0a20 2020    button = [.   
-00022db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022dc0: 2062 7574 746f 6e0a 2020 2020 2020 2020   button.        
-00022dd0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-00022de0: 726f 7720 696e 206b 6579 626f 6172 640a  row in keyboard.
-00022df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022e00: 2020 2020 666f 7220 6275 7474 6f6e 2069      for button i
-00022e10: 6e20 726f 770a 2020 2020 2020 2020 2020  n row.          
-00022e20: 2020 2020 2020 5d5b 785d 0a20 2020 2020        ][x].     
-00022e30: 2020 2020 2020 2065 7863 6570 7420 496e         except In
-00022e40: 6465 7845 7272 6f72 3a0a 2020 2020 2020  dexError:.      
-00022e50: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-00022e60: 5661 6c75 6545 7272 6f72 2866 2254 6865  ValueError(f"The
-00022e70: 2062 7574 746f 6e20 6174 2069 6e64 6578   button at index
-00022e80: 207b 787d 2064 6f65 736e 2774 2065 7869   {x} doesn't exi
-00022e90: 7374 2229 0a20 2020 2020 2020 2065 6c69  st").        eli
-00022ea0: 6620 6973 696e 7374 616e 6365 2878 2c20  f isinstance(x, 
-00022eb0: 696e 7429 2061 6e64 2069 7369 6e73 7461  int) and isinsta
-00022ec0: 6e63 6528 792c 2069 6e74 293a 0a20 2020  nce(y, int):.   
-00022ed0: 2020 2020 2020 2020 2074 7279 3a0a 2020           try:.  
-00022ee0: 2020 2020 2020 2020 2020 2020 2020 6275                bu
-00022ef0: 7474 6f6e 203d 206b 6579 626f 6172 645b  tton = keyboard[
-00022f00: 795d 5b78 5d0a 2020 2020 2020 2020 2020  y][x].          
-00022f10: 2020 6578 6365 7074 2049 6e64 6578 4572    except IndexEr
-00022f20: 726f 723a 0a20 2020 2020 2020 2020 2020  ror:.           
-00022f30: 2020 2020 2072 6169 7365 2056 616c 7565       raise Value
-00022f40: 4572 726f 7228 6622 5468 6520 6275 7474  Error(f"The butt
-00022f50: 6f6e 2061 7420 706f 7369 7469 6f6e 2028  on at position (
-00022f60: 7b78 7d2c 207b 797d 2920 646f 6573 6e27  {x}, {y}) doesn'
-00022f70: 7420 6578 6973 7422 290a 2020 2020 2020  t exist").      
-00022f80: 2020 656c 6966 2069 7369 6e73 7461 6e63    elif isinstanc
-00022f90: 6528 782c 2073 7472 2920 616e 6420 7920  e(x, str) and y 
-00022fa0: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
-00022fb0: 2020 2020 206c 6162 656c 203d 2078 2e65       label = x.e
-00022fc0: 6e63 6f64 6528 2275 7466 2d31 3622 2c20  ncode("utf-16", 
-00022fd0: 2273 7572 726f 6761 7465 7061 7373 2229  "surrogatepass")
-00022fe0: 2e64 6563 6f64 6528 2275 7466 2d31 3622  .decode("utf-16"
-00022ff0: 290a 0a20 2020 2020 2020 2020 2020 2074  )..            t
-00023000: 7279 3a0a 2020 2020 2020 2020 2020 2020  ry:.            
-00023010: 2020 2020 6275 7474 6f6e 203d 205b 0a20      button = [. 
-00023020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023030: 2020 2062 7574 746f 6e0a 2020 2020 2020     button.      
-00023040: 2020 2020 2020 2020 2020 2020 2020 666f                fo
-00023050: 7220 726f 7720 696e 206b 6579 626f 6172  r row in keyboar
-00023060: 640a 2020 2020 2020 2020 2020 2020 2020  d.              
-00023070: 2020 2020 2020 666f 7220 6275 7474 6f6e        for button
-00023080: 2069 6e20 726f 770a 2020 2020 2020 2020   in row.        
-00023090: 2020 2020 2020 2020 2020 2020 6966 206c              if l
-000230a0: 6162 656c 203d 3d20 6275 7474 6f6e 2e74  abel == button.t
-000230b0: 6578 740a 2020 2020 2020 2020 2020 2020  ext.            
-000230c0: 2020 2020 5d5b 305d 0a20 2020 2020 2020      ][0].       
-000230d0: 2020 2020 2065 7863 6570 7420 496e 6465       except Inde
-000230e0: 7845 7272 6f72 3a0a 2020 2020 2020 2020  xError:.        
-000230f0: 2020 2020 2020 2020 7261 6973 6520 5661          raise Va
-00023100: 6c75 6545 7272 6f72 2866 2254 6865 2062  lueError(f"The b
-00023110: 7574 746f 6e20 7769 7468 206c 6162 656c  utton with label
-00023120: 2027 7b78 7d27 2064 6f65 736e 2774 2065   '{x}' doesn't e
-00023130: 7869 7374 7322 290a 2020 2020 2020 2020  xists").        
-00023140: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-00023150: 2020 7261 6973 6520 5661 6c75 6545 7272    raise ValueErr
-00023160: 6f72 2822 496e 7661 6c69 6420 6172 6775  or("Invalid argu
-00023170: 6d65 6e74 7322 290a 0a20 2020 2020 2020  ments")..       
-00023180: 2069 6620 6973 5f69 6e6c 696e 653a 0a20   if is_inline:. 
-00023190: 2020 2020 2020 2020 2020 2069 6620 6275             if bu
-000231a0: 7474 6f6e 2e63 616c 6c62 6163 6b5f 6461  tton.callback_da
-000231b0: 7461 3a0a 2020 2020 2020 2020 2020 2020  ta:.            
-000231c0: 2020 2020 7265 7475 726e 2061 7761 6974      return await
-000231d0: 2073 656c 662e 5f63 6c69 656e 742e 7265   self._client.re
-000231e0: 7175 6573 745f 6361 6c6c 6261 636b 5f61  quest_callback_a
-000231f0: 6e73 7765 7228 0a20 2020 2020 2020 2020  nswer(.         
-00023200: 2020 2020 2020 2020 2020 2063 6861 745f             chat_
-00023210: 6964 3d73 656c 662e 6368 6174 2e69 642c  id=self.chat.id,
-00023220: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00023230: 2020 2020 206d 6573 7361 6765 5f69 643d       message_id=
-00023240: 7365 6c66 2e69 642c 0a20 2020 2020 2020  self.id,.       
-00023250: 2020 2020 2020 2020 2020 2020 2063 616c               cal
-00023260: 6c62 6163 6b5f 6461 7461 3d62 7574 746f  lback_data=butto
-00023270: 6e2e 6361 6c6c 6261 636b 5f64 6174 612c  n.callback_data,
-00023280: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00023290: 2020 2020 2074 696d 656f 7574 3d74 696d       timeout=tim
-000232a0: 656f 7574 0a20 2020 2020 2020 2020 2020  eout.           
-000232b0: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
-000232c0: 2020 2065 6c69 6620 6275 7474 6f6e 2e75     elif button.u
-000232d0: 726c 3a0a 2020 2020 2020 2020 2020 2020  rl:.            
-000232e0: 2020 2020 7265 7475 726e 2062 7574 746f      return butto
-000232f0: 6e2e 7572 6c0a 2020 2020 2020 2020 2020  n.url.          
-00023300: 2020 656c 6966 2062 7574 746f 6e2e 7377    elif button.sw
-00023310: 6974 6368 5f69 6e6c 696e 655f 7175 6572  itch_inline_quer
-00023320: 793a 0a20 2020 2020 2020 2020 2020 2020  y:.             
-00023330: 2020 2072 6574 7572 6e20 6275 7474 6f6e     return button
-00023340: 2e73 7769 7463 685f 696e 6c69 6e65 5f71  .switch_inline_q
-00023350: 7565 7279 0a20 2020 2020 2020 2020 2020  uery.           
-00023360: 2065 6c69 6620 6275 7474 6f6e 2e73 7769   elif button.swi
-00023370: 7463 685f 696e 6c69 6e65 5f71 7565 7279  tch_inline_query
-00023380: 5f63 7572 7265 6e74 5f63 6861 743a 0a20  _current_chat:. 
-00023390: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-000233a0: 6574 7572 6e20 6275 7474 6f6e 2e73 7769  eturn button.swi
-000233b0: 7463 685f 696e 6c69 6e65 5f71 7565 7279  tch_inline_query
-000233c0: 5f63 7572 7265 6e74 5f63 6861 740a 2020  _current_chat.  
-000233d0: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
-000233e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000233f0: 7261 6973 6520 5661 6c75 6545 7272 6f72  raise ValueError
-00023400: 2822 5468 6973 2062 7574 746f 6e20 6973  ("This button is
-00023410: 206e 6f74 2073 7570 706f 7274 6564 2079   not supported y
-00023420: 6574 2229 0a20 2020 2020 2020 2065 6c73  et").        els
-00023430: 653a 0a20 2020 2020 2020 2020 2020 2061  e:.            a
-00023440: 7761 6974 2073 656c 662e 7265 706c 7928  wait self.reply(
-00023450: 6275 7474 6f6e 2c20 7175 6f74 653d 7175  button, quote=qu
-00023460: 6f74 6529 0a0a 2020 2020 6173 796e 6320  ote)..    async 
-00023470: 6465 6620 7265 6163 7428 7365 6c66 2c20  def react(self, 
-00023480: 656d 6f6a 693a 2073 7472 203d 2022 222c  emoji: str = "",
-00023490: 2062 6967 3a20 626f 6f6c 203d 2046 616c   big: bool = Fal
-000234a0: 7365 2920 2d3e 2062 6f6f 6c3a 0a20 2020  se) -> bool:.   
-000234b0: 2020 2020 2022 2222 426f 756e 6420 6d65       """Bound me
-000234c0: 7468 6f64 202a 7265 6163 742a 206f 6620  thod *react* of 
-000234d0: 3a6f 626a 3a60 7e70 7972 6f67 7261 6d2e  :obj:`~pyrogram.
-000234e0: 7479 7065 732e 4d65 7373 6167 6560 2e0a  types.Message`..
-000234f0: 0a20 2020 2020 2020 2055 7365 2061 7320  .        Use as 
-00023500: 6120 7368 6f72 7463 7574 2066 6f72 3a0a  a shortcut for:.
-00023510: 0a20 2020 2020 2020 202e 2e20 636f 6465  .        .. code
-00023520: 2d62 6c6f 636b 3a3a 2070 7974 686f 6e0a  -block:: python.
-00023530: 0a20 2020 2020 2020 2020 2020 2061 7761  .            awa
-00023540: 6974 2063 6c69 656e 742e 7365 6e64 5f72  it client.send_r
-00023550: 6561 6374 696f 6e28 0a20 2020 2020 2020  eaction(.       
-00023560: 2020 2020 2020 2020 2063 6861 745f 6964           chat_id
-00023570: 3d63 6861 745f 6964 2c0a 2020 2020 2020  =chat_id,.      
-00023580: 2020 2020 2020 2020 2020 6d65 7373 6167            messag
-00023590: 655f 6964 3d6d 6573 7361 6765 2e69 642c  e_id=message.id,
-000235a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000235b0: 2065 6d6f 6a69 3d22 f09f 94a5 220a 2020   emoji="....".  
-000235c0: 2020 2020 2020 2020 2020 290a 0a20 2020            )..   
-000235d0: 2020 2020 2045 7861 6d70 6c65 3a0a 2020       Example:.  
-000235e0: 2020 2020 2020 2020 2020 2e2e 2063 6f64            .. cod
-000235f0: 652d 626c 6f63 6b3a 3a20 7079 7468 6f6e  e-block:: python
-00023600: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00023610: 2020 6177 6169 7420 6d65 7373 6167 652e    await message.
-00023620: 7265 6163 7428 656d 6f6a 693d 22f0 9f94  react(emoji="...
-00023630: a522 290a 0a20 2020 2020 2020 2050 6172  .")..        Par
-00023640: 616d 6574 6572 733a 0a20 2020 2020 2020  ameters:.       
-00023650: 2020 2020 2065 6d6f 6a69 2028 6060 7374       emoji (``st
-00023660: 7260 602c 202a 6f70 7469 6f6e 616c 2a29  r``, *optional*)
-00023670: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00023680: 2020 5265 6163 7469 6f6e 2065 6d6f 6a69    Reaction emoji
-00023690: 2e0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000236a0: 2020 5061 7373 2022 2220 6173 2065 6d6f    Pass "" as emo
-000236b0: 6a69 2028 6465 6661 756c 7429 2074 6f20  ji (default) to 
-000236c0: 7265 7472 6163 7420 7468 6520 7265 6163  retract the reac
-000236d0: 7469 6f6e 2e0a 2020 2020 2020 2020 2020  tion..          
-000236e0: 2020 200a 2020 2020 2020 2020 2020 2020     .            
-000236f0: 6269 6720 2860 6062 6f6f 6c60 602c 202a  big (``bool``, *
-00023700: 6f70 7469 6f6e 616c 2a29 3a0a 2020 2020  optional*):.    
-00023710: 2020 2020 2020 2020 2020 2020 5061 7373              Pass
-00023720: 2054 7275 6520 746f 2073 686f 7720 6120   True to show a 
-00023730: 6269 6767 6572 2061 6e64 206c 6f6e 6765  bigger and longe
-00023740: 7220 7265 6163 7469 6f6e 2e0a 2020 2020  r reaction..    
-00023750: 2020 2020 2020 2020 2020 2020 4465 6661              Defa
-00023760: 756c 7473 2074 6f20 4661 6c73 652e 0a0a  ults to False...
-00023770: 2020 2020 2020 2020 5265 7475 726e 733a          Returns:
-00023780: 0a20 2020 2020 2020 2020 2020 2060 6062  .            ``b
-00023790: 6f6f 6c60 603a 204f 6e20 7375 6363 6573  ool``: On succes
-000237a0: 732c 2054 7275 6520 6973 2072 6574 7572  s, True is retur
-000237b0: 6e65 642e 0a0a 2020 2020 2020 2020 5261  ned...        Ra
-000237c0: 6973 6573 3a0a 2020 2020 2020 2020 2020  ises:.          
-000237d0: 2020 5250 4345 7272 6f72 3a20 496e 2063    RPCError: In c
-000237e0: 6173 6520 6f66 2061 2054 656c 6567 7261  ase of a Telegra
-000237f0: 6d20 5250 4320 6572 726f 722e 0a20 2020  m RPC error..   
-00023800: 2020 2020 2022 2222 0a0a 2020 2020 2020       """..      
-00023810: 2020 7265 7475 726e 2061 7761 6974 2073    return await s
-00023820: 656c 662e 5f63 6c69 656e 742e 7365 6e64  elf._client.send
-00023830: 5f72 6561 6374 696f 6e28 0a20 2020 2020  _reaction(.     
-00023840: 2020 2020 2020 2063 6861 745f 6964 3d73         chat_id=s
-00023850: 656c 662e 6368 6174 2e69 642c 0a20 2020  elf.chat.id,.   
-00023860: 2020 2020 2020 2020 206d 6573 7361 6765           message
-00023870: 5f69 643d 7365 6c66 2e69 642c 0a20 2020  _id=self.id,.   
-00023880: 2020 2020 2020 2020 2065 6d6f 6a69 3d65           emoji=e
-00023890: 6d6f 6a69 2c0a 2020 2020 2020 2020 2020  moji,.          
-000238a0: 2020 6269 673d 6269 670a 2020 2020 2020    big=big.      
-000238b0: 2020 290a 0a20 2020 2061 7379 6e63 2064    )..    async d
-000238c0: 6566 2072 6574 7261 6374 5f76 6f74 6528  ef retract_vote(
-000238d0: 0a20 2020 2020 2020 2073 656c 662c 0a20  .        self,. 
-000238e0: 2020 2029 202d 3e20 2274 7970 6573 2e50     ) -> "types.P
-000238f0: 6f6c 6c22 3a0a 2020 2020 2020 2020 2222  oll":.        ""
-00023900: 2242 6f75 6e64 206d 6574 686f 6420 2a72  "Bound method *r
-00023910: 6574 7261 6374 5f76 6f74 652a 206f 6620  etract_vote* of 
-00023920: 3a6f 626a 3a60 7e70 7972 6f67 7261 6d2e  :obj:`~pyrogram.
-00023930: 7479 7065 732e 4d65 7373 6167 6560 2e0a  types.Message`..
-00023940: 0a20 2020 2020 2020 2055 7365 2061 7320  .        Use as 
-00023950: 6120 7368 6f72 7463 7574 2066 6f72 3a0a  a shortcut for:.
-00023960: 0a20 2020 2020 2020 202e 2e20 636f 6465  .        .. code
-00023970: 2d62 6c6f 636b 3a3a 2070 7974 686f 6e0a  -block:: python.
-00023980: 0a20 2020 2020 2020 2020 2020 2063 6c69  .            cli
-00023990: 656e 742e 7265 7472 6163 745f 766f 7465  ent.retract_vote
-000239a0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-000239b0: 2020 6368 6174 5f69 643d 6d65 7373 6167    chat_id=messag
-000239c0: 652e 6368 6174 2e69 642c 0a20 2020 2020  e.chat.id,.     
-000239d0: 2020 2020 2020 2020 2020 206d 6573 7361             messa
-000239e0: 6765 5f69 643d 6d65 7373 6167 655f 6964  ge_id=message_id
-000239f0: 2c0a 2020 2020 2020 2020 2020 2020 290a  ,.            ).
-00023a00: 0a20 2020 2020 2020 2045 7861 6d70 6c65  .        Example
-00023a10: 3a0a 2020 2020 2020 2020 2020 2020 2e2e  :.            ..
-00023a20: 2063 6f64 652d 626c 6f63 6b3a 3a20 7079   code-block:: py
-00023a30: 7468 6f6e 0a0a 2020 2020 2020 2020 2020  thon..          
-00023a40: 2020 2020 2020 6d65 7373 6167 652e 7265        message.re
-00023a50: 7472 6163 745f 766f 7465 2829 0a0a 2020  tract_vote()..  
-00023a60: 2020 2020 2020 5265 7475 726e 733a 0a20        Returns:. 
-00023a70: 2020 2020 2020 2020 2020 203a 6f62 6a3a             :obj:
-00023a80: 607e 7079 726f 6772 616d 2e74 7970 6573  `~pyrogram.types
-00023a90: 2e50 6f6c 6c60 3a20 4f6e 2073 7563 6365  .Poll`: On succe
-00023aa0: 7373 2c20 7468 6520 706f 6c6c 2077 6974  ss, the poll wit
-00023ab0: 6820 7468 6520 7265 7472 6163 7465 6420  h the retracted 
-00023ac0: 766f 7465 2069 7320 7265 7475 726e 6564  vote is returned
-00023ad0: 2e0a 0a20 2020 2020 2020 2052 6169 7365  ...        Raise
-00023ae0: 733a 0a20 2020 2020 2020 2020 2020 2052  s:.            R
-00023af0: 5043 4572 726f 723a 2049 6e20 6361 7365  PCError: In case
-00023b00: 206f 6620 6120 5465 6c65 6772 616d 2052   of a Telegram R
-00023b10: 5043 2065 7272 6f72 2e0a 2020 2020 2020  PC error..      
-00023b20: 2020 2222 220a 0a20 2020 2020 2020 2072    """..        r
-00023b30: 6574 7572 6e20 6177 6169 7420 7365 6c66  eturn await self
-00023b40: 2e5f 636c 6965 6e74 2e72 6574 7261 6374  ._client.retract
-00023b50: 5f76 6f74 6528 0a20 2020 2020 2020 2020  _vote(.         
-00023b60: 2020 2063 6861 745f 6964 3d73 656c 662e     chat_id=self.
-00023b70: 6368 6174 2e69 642c 0a20 2020 2020 2020  chat.id,.       
-00023b80: 2020 2020 206d 6573 7361 6765 5f69 643d       message_id=
-00023b90: 7365 6c66 2e69 640a 2020 2020 2020 2020  self.id.        
-00023ba0: 290a 0a20 2020 2061 7379 6e63 2064 6566  )..    async def
-00023bb0: 2064 6f77 6e6c 6f61 6428 0a20 2020 2020   download(.     
-00023bc0: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
-00023bd0: 2066 696c 655f 6e61 6d65 3a20 7374 7220   file_name: str 
-00023be0: 3d20 2222 2c0a 2020 2020 2020 2020 696e  = "",.        in
-00023bf0: 5f6d 656d 6f72 793a 2062 6f6f 6c20 3d20  _memory: bool = 
-00023c00: 4661 6c73 652c 0a20 2020 2020 2020 2062  False,.        b
-00023c10: 6c6f 636b 3a20 626f 6f6c 203d 2054 7275  lock: bool = Tru
-00023c20: 652c 0a20 2020 2020 2020 2070 726f 6772  e,.        progr
-00023c30: 6573 733a 2043 616c 6c61 626c 6520 3d20  ess: Callable = 
-00023c40: 4e6f 6e65 2c0a 2020 2020 2020 2020 7072  None,.        pr
-00023c50: 6f67 7265 7373 5f61 7267 733a 2074 7570  ogress_args: tup
-00023c60: 6c65 203d 2028 290a 2020 2020 2920 2d3e  le = ().    ) ->
-00023c70: 2073 7472 3a0a 2020 2020 2020 2020 2222   str:.        ""
-00023c80: 2242 6f75 6e64 206d 6574 686f 6420 2a64  "Bound method *d
-00023c90: 6f77 6e6c 6f61 642a 206f 6620 3a6f 626a  ownload* of :obj
-00023ca0: 3a60 7e70 7972 6f67 7261 6d2e 7479 7065  :`~pyrogram.type
-00023cb0: 732e 4d65 7373 6167 6560 2e0a 0a20 2020  s.Message`...   
-00023cc0: 2020 2020 2055 7365 2061 7320 6120 7368       Use as a sh
-00023cd0: 6f72 7463 7574 2066 6f72 3a0a 0a20 2020  ortcut for:..   
-00023ce0: 2020 2020 202e 2e20 636f 6465 2d62 6c6f       .. code-blo
-00023cf0: 636b 3a3a 2070 7974 686f 6e0a 0a20 2020  ck:: python..   
-00023d00: 2020 2020 2020 2020 2061 7761 6974 2063           await c
-00023d10: 6c69 656e 742e 646f 776e 6c6f 6164 5f6d  lient.download_m
-00023d20: 6564 6961 286d 6573 7361 6765 290a 0a20  edia(message).. 
-00023d30: 2020 2020 2020 2045 7861 6d70 6c65 3a0a         Example:.
-00023d40: 2020 2020 2020 2020 2020 2020 2e2e 2063              .. c
-00023d50: 6f64 652d 626c 6f63 6b3a 3a20 7079 7468  ode-block:: pyth
-00023d60: 6f6e 0a0a 2020 2020 2020 2020 2020 2020  on..            
-00023d70: 2020 2020 6177 6169 7420 6d65 7373 6167      await messag
-00023d80: 652e 646f 776e 6c6f 6164 2829 0a0a 2020  e.download()..  
-00023d90: 2020 2020 2020 5061 7261 6d65 7465 7273        Parameters
-00023da0: 3a0a 2020 2020 2020 2020 2020 2020 6669  :.            fi
-00023db0: 6c65 5f6e 616d 6520 2860 6073 7472 6060  le_name (``str``
-00023dc0: 2c20 2a6f 7074 696f 6e61 6c2a 293a 0a20  , *optional*):. 
-00023dd0: 2020 2020 2020 2020 2020 2020 2020 2041                 A
-00023de0: 2063 7573 746f 6d20 2a66 696c 655f 6e61   custom *file_na
-00023df0: 6d65 2a20 746f 2062 6520 7573 6564 2069  me* to be used i
-00023e00: 6e73 7465 6164 206f 6620 7468 6520 6f6e  nstead of the on
-00023e10: 6520 7072 6f76 6964 6564 2062 7920 5465  e provided by Te
-00023e20: 6c65 6772 616d 2e0a 2020 2020 2020 2020  legram..        
-00023e30: 2020 2020 2020 2020 4279 2064 6566 6175          By defau
-00023e40: 6c74 2c20 616c 6c20 6669 6c65 7320 6172  lt, all files ar
-00023e50: 6520 646f 776e 6c6f 6164 6564 2069 6e20  e downloaded in 
-00023e60: 7468 6520 2a64 6f77 6e6c 6f61 6473 2a20  the *downloads* 
-00023e70: 666f 6c64 6572 2069 6e20 796f 7572 2077  folder in your w
-00023e80: 6f72 6b69 6e67 2064 6972 6563 746f 7279  orking directory
-00023e90: 2e0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00023ea0: 2020 596f 7520 6361 6e20 616c 736f 2073    You can also s
-00023eb0: 7065 6369 6679 2061 2070 6174 6820 666f  pecify a path fo
-00023ec0: 7220 646f 776e 6c6f 6164 696e 6720 6669  r downloading fi
-00023ed0: 6c65 7320 696e 2061 2063 7573 746f 6d20  les in a custom 
-00023ee0: 6c6f 6361 7469 6f6e 3a20 7061 7468 7320  location: paths 
-00023ef0: 7468 6174 2065 6e64 2077 6974 6820 222f  that end with "/
-00023f00: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-00023f10: 2020 6172 6520 636f 6e73 6964 6572 6564    are considered
-00023f20: 2064 6972 6563 746f 7269 6573 2e20 416c   directories. Al
-00023f30: 6c20 6e6f 6e2d 6578 6973 7465 6e74 2066  l non-existent f
-00023f40: 6f6c 6465 7273 2077 696c 6c20 6265 2063  olders will be c
-00023f50: 7265 6174 6564 2061 7574 6f6d 6174 6963  reated automatic
-00023f60: 616c 6c79 2e0a 0a20 2020 2020 2020 2020  ally...         
-00023f70: 2020 2069 6e5f 6d65 6d6f 7279 2028 6060     in_memory (``
-00023f80: 626f 6f6c 6060 2c20 2a6f 7074 696f 6e61  bool``, *optiona
-00023f90: 6c2a 293a 0a20 2020 2020 2020 2020 2020  l*):.           
-00023fa0: 2020 2020 2050 6173 7320 5472 7565 2074       Pass True t
-00023fb0: 6f20 646f 776e 6c6f 6164 2074 6865 206d  o download the m
-00023fc0: 6564 6961 2069 6e2d 6d65 6d6f 7279 2e0a  edia in-memory..
-00023fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023fe0: 4120 6269 6e61 7279 2066 696c 652d 6c69  A binary file-li
-00023ff0: 6b65 206f 626a 6563 7420 7769 7468 2069  ke object with i
-00024000: 7473 2061 7474 7269 6275 7465 2022 2e6e  ts attribute ".n
-00024010: 616d 6522 2073 6574 2077 696c 6c20 6265  ame" set will be
-00024020: 2072 6574 7572 6e65 642e 0a20 2020 2020   returned..     
-00024030: 2020 2020 2020 2020 2020 2044 6566 6175             Defau
-00024040: 6c74 7320 746f 2046 616c 7365 2e0a 0a20  lts to False... 
-00024050: 2020 2020 2020 2020 2020 2062 6c6f 636b             block
-00024060: 2028 6060 626f 6f6c 6060 2c20 2a6f 7074   (``bool``, *opt
-00024070: 696f 6e61 6c2a 293a 0a20 2020 2020 2020  ional*):.       
-00024080: 2020 2020 2020 2020 2042 6c6f 636b 7320           Blocks 
-00024090: 7468 6520 636f 6465 2065 7865 6375 7469  the code executi
-000240a0: 6f6e 2075 6e74 696c 2074 6865 2066 696c  on until the fil
-000240b0: 6520 6861 7320 6265 656e 2064 6f77 6e6c  e has been downl
-000240c0: 6f61 6465 642e 0a20 2020 2020 2020 2020  oaded..         
-000240d0: 2020 2020 2020 2044 6566 6175 6c74 7320         Defaults 
-000240e0: 746f 2054 7275 652e 0a0a 2020 2020 2020  to True...      
-000240f0: 2020 2020 2020 7072 6f67 7265 7373 2028        progress (
-00024100: 6060 4361 6c6c 6162 6c65 6060 2c20 2a6f  ``Callable``, *o
-00024110: 7074 696f 6e61 6c2a 293a 0a20 2020 2020  ptional*):.     
-00024120: 2020 2020 2020 2020 2020 2050 6173 7320             Pass 
-00024130: 6120 6361 6c6c 6261 636b 2066 756e 6374  a callback funct
-00024140: 696f 6e20 746f 2076 6965 7720 7468 6520  ion to view the 
-00024150: 6669 6c65 2074 7261 6e73 6d69 7373 696f  file transmissio
-00024160: 6e20 7072 6f67 7265 7373 2e0a 2020 2020  n progress..    
-00024170: 2020 2020 2020 2020 2020 2020 5468 6520              The 
-00024180: 6675 6e63 7469 6f6e 206d 7573 7420 7461  function must ta
-00024190: 6b65 202a 2863 7572 7265 6e74 2c20 746f  ke *(current, to
-000241a0: 7461 6c29 2a20 6173 2070 6f73 6974 696f  tal)* as positio
-000241b0: 6e61 6c20 6172 6775 6d65 6e74 7320 286c  nal arguments (l
-000241c0: 6f6f 6b20 6174 204f 7468 6572 2050 6172  ook at Other Par
-000241d0: 616d 6574 6572 7320 6265 6c6f 7720 666f  ameters below fo
-000241e0: 7220 610a 2020 2020 2020 2020 2020 2020  r a.            
-000241f0: 2020 2020 6465 7461 696c 6564 2064 6573      detailed des
-00024200: 6372 6970 7469 6f6e 2920 616e 6420 7769  cription) and wi
-00024210: 6c6c 2062 6520 6361 6c6c 6564 2062 6163  ll be called bac
-00024220: 6b20 6561 6368 2074 696d 6520 6120 6e65  k each time a ne
-00024230: 7720 6669 6c65 2063 6875 6e6b 2068 6173  w file chunk has
-00024240: 2062 6565 6e20 7375 6363 6573 7366 756c   been successful
-00024250: 6c79 0a20 2020 2020 2020 2020 2020 2020  ly.             
-00024260: 2020 2074 7261 6e73 6d69 7474 6564 2e0a     transmitted..
-00024270: 0a20 2020 2020 2020 2020 2020 2070 726f  .            pro
-00024280: 6772 6573 735f 6172 6773 2028 6060 7475  gress_args (``tu
-00024290: 706c 6560 602c 202a 6f70 7469 6f6e 616c  ple``, *optional
-000242a0: 2a29 3a0a 2020 2020 2020 2020 2020 2020  *):.            
-000242b0: 2020 2020 4578 7472 6120 6375 7374 6f6d      Extra custom
-000242c0: 2061 7267 756d 656e 7473 2066 6f72 2074   arguments for t
-000242d0: 6865 2070 726f 6772 6573 7320 6361 6c6c  he progress call
-000242e0: 6261 636b 2066 756e 6374 696f 6e2e 0a20  back function.. 
-000242f0: 2020 2020 2020 2020 2020 2020 2020 2059                 Y
-00024300: 6f75 2063 616e 2070 6173 7320 616e 7974  ou can pass anyt
-00024310: 6869 6e67 2079 6f75 206e 6565 6420 746f  hing you need to
-00024320: 2062 6520 6176 6169 6c61 626c 6520 696e   be available in
-00024330: 2074 6865 2070 726f 6772 6573 7320 6361   the progress ca
-00024340: 6c6c 6261 636b 2073 636f 7065 3b20 666f  llback scope; fo
-00024350: 7220 6578 616d 706c 652c 2061 204d 6573  r example, a Mes
-00024360: 7361 6765 0a20 2020 2020 2020 2020 2020  sage.           
-00024370: 2020 2020 206f 626a 6563 7420 6f72 2061       object or a
-00024380: 2043 6c69 656e 7420 696e 7374 616e 6365   Client instance
-00024390: 2069 6e20 6f72 6465 7220 746f 2065 6469   in order to edi
-000243a0: 7420 7468 6520 6d65 7373 6167 6520 7769  t the message wi
-000243b0: 7468 2074 6865 2075 7064 6174 6564 2070  th the updated p
-000243c0: 726f 6772 6573 7320 7374 6174 7573 2e0a  rogress status..
-000243d0: 0a20 2020 2020 2020 204f 7468 6572 2050  .        Other P
-000243e0: 6172 616d 6574 6572 733a 0a20 2020 2020  arameters:.     
-000243f0: 2020 2020 2020 2063 7572 7265 6e74 2028         current (
-00024400: 6060 696e 7460 6029 3a0a 2020 2020 2020  ``int``):.      
-00024410: 2020 2020 2020 2020 2020 5468 6520 616d            The am
-00024420: 6f75 6e74 206f 6620 6279 7465 7320 7472  ount of bytes tr
-00024430: 616e 736d 6974 7465 6420 736f 2066 6172  ansmitted so far
-00024440: 2e0a 0a20 2020 2020 2020 2020 2020 2074  ...            t
-00024450: 6f74 616c 2028 6060 696e 7460 6029 3a0a  otal (``int``):.
-00024460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024470: 5468 6520 746f 7461 6c20 7369 7a65 206f  The total size o
-00024480: 6620 7468 6520 6669 6c65 2e0a 0a20 2020  f the file...   
-00024490: 2020 2020 2020 2020 202a 6172 6773 2028           *args (
-000244a0: 6060 7475 706c 6560 602c 202a 6f70 7469  ``tuple``, *opti
-000244b0: 6f6e 616c 2a29 3a0a 2020 2020 2020 2020  onal*):.        
-000244c0: 2020 2020 2020 2020 4578 7472 6120 6375          Extra cu
-000244d0: 7374 6f6d 2061 7267 756d 656e 7473 2061  stom arguments a
-000244e0: 7320 6465 6669 6e65 6420 696e 2074 6865  s defined in the
-000244f0: 2060 6070 726f 6772 6573 735f 6172 6773   ``progress_args
-00024500: 6060 2070 6172 616d 6574 6572 2e0a 2020  `` parameter..  
-00024510: 2020 2020 2020 2020 2020 2020 2020 596f                Yo
-00024520: 7520 6361 6e20 6569 7468 6572 206b 6565  u can either kee
-00024530: 7020 6060 2a61 7267 7360 6020 6f72 2061  p ``*args`` or a
-00024540: 6464 2065 7665 7279 2073 696e 676c 6520  dd every single 
-00024550: 6578 7472 6120 6172 6775 6d65 6e74 2069  extra argument i
-00024560: 6e20 796f 7572 2066 756e 6374 696f 6e20  n your function 
-00024570: 7369 676e 6174 7572 652e 0a0a 2020 2020  signature...    
-00024580: 2020 2020 5265 7475 726e 733a 0a20 2020      Returns:.   
-00024590: 2020 2020 2020 2020 204f 6e20 7375 6363           On succ
-000245a0: 6573 732c 2074 6865 2061 6273 6f6c 7574  ess, the absolut
-000245b0: 6520 7061 7468 206f 6620 7468 6520 646f  e path of the do
-000245c0: 776e 6c6f 6164 6564 2066 696c 6520 6173  wnloaded file as
-000245d0: 2073 7472 696e 6720 6973 2072 6574 7572   string is retur
-000245e0: 6e65 642c 204e 6f6e 6520 6f74 6865 7277  ned, None otherw
-000245f0: 6973 652e 0a0a 2020 2020 2020 2020 5261  ise...        Ra
-00024600: 6973 6573 3a0a 2020 2020 2020 2020 2020  ises:.          
-00024610: 2020 5250 4345 7272 6f72 3a20 496e 2063    RPCError: In c
-00024620: 6173 6520 6f66 2061 2054 656c 6567 7261  ase of a Telegra
-00024630: 6d20 5250 4320 6572 726f 722e 0a20 2020  m RPC error..   
-00024640: 2020 2020 2020 2020 2060 6056 616c 7565           ``Value
-00024650: 4572 726f 7260 603a 2049 6620 7468 6520  Error``: If the 
-00024660: 6d65 7373 6167 6520 646f 6573 6e27 7420  message doesn't 
-00024670: 636f 6e74 6169 6e20 616e 7920 646f 776e  contain any down
-00024680: 6c6f 6164 6162 6c65 206d 6564 6961 0a20  loadable media. 
-00024690: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-000246a0: 2020 2072 6574 7572 6e20 6177 6169 7420     return await 
-000246b0: 7365 6c66 2e5f 636c 6965 6e74 2e64 6f77  self._client.dow
-000246c0: 6e6c 6f61 645f 6d65 6469 6128 0a20 2020  nload_media(.   
-000246d0: 2020 2020 2020 2020 206d 6573 7361 6765           message
-000246e0: 3d73 656c 662c 0a20 2020 2020 2020 2020  =self,.         
-000246f0: 2020 2066 696c 655f 6e61 6d65 3d66 696c     file_name=fil
-00024700: 655f 6e61 6d65 2c0a 2020 2020 2020 2020  e_name,.        
-00024710: 2020 2020 696e 5f6d 656d 6f72 793d 696e      in_memory=in
-00024720: 5f6d 656d 6f72 792c 0a20 2020 2020 2020  _memory,.       
-00024730: 2020 2020 2062 6c6f 636b 3d62 6c6f 636b       block=block
-00024740: 2c0a 2020 2020 2020 2020 2020 2020 7072  ,.            pr
-00024750: 6f67 7265 7373 3d70 726f 6772 6573 732c  ogress=progress,
-00024760: 0a20 2020 2020 2020 2020 2020 2070 726f  .            pro
-00024770: 6772 6573 735f 6172 6773 3d70 726f 6772  gress_args=progr
-00024780: 6573 735f 6172 6773 2c0a 2020 2020 2020  ess_args,.      
-00024790: 2020 290a 0a20 2020 2061 7379 6e63 2064    )..    async d
-000247a0: 6566 2076 6f74 6528 0a20 2020 2020 2020  ef vote(.       
-000247b0: 2073 656c 662c 0a20 2020 2020 2020 206f   self,.        o
-000247c0: 7074 696f 6e3a 2069 6e74 2c0a 2020 2020  ption: int,.    
-000247d0: 2920 2d3e 2022 7479 7065 732e 506f 6c6c  ) -> "types.Poll
-000247e0: 223a 0a20 2020 2020 2020 2022 2222 426f  ":.        """Bo
-000247f0: 756e 6420 6d65 7468 6f64 202a 766f 7465  und method *vote
-00024800: 2a20 6f66 203a 6f62 6a3a 607e 7079 726f  * of :obj:`~pyro
-00024810: 6772 616d 2e74 7970 6573 2e4d 6573 7361  gram.types.Messa
-00024820: 6765 602e 0a0a 2020 2020 2020 2020 5573  ge`...        Us
-00024830: 6520 6173 2061 2073 686f 7274 6375 7420  e as a shortcut 
-00024840: 666f 723a 0a0a 2020 2020 2020 2020 2e2e  for:..        ..
-00024850: 2063 6f64 652d 626c 6f63 6b3a 3a20 7079   code-block:: py
-00024860: 7468 6f6e 0a0a 2020 2020 2020 2020 2020  thon..          
-00024870: 2020 636c 6965 6e74 2e76 6f74 655f 706f    client.vote_po
-00024880: 6c6c 280a 2020 2020 2020 2020 2020 2020  ll(.            
-00024890: 2020 2020 6368 6174 5f69 643d 6d65 7373      chat_id=mess
-000248a0: 6167 652e 6368 6174 2e69 642c 0a20 2020  age.chat.id,.   
-000248b0: 2020 2020 2020 2020 2020 2020 206d 6573               mes
-000248c0: 7361 6765 5f69 643d 6d65 7373 6167 652e  sage_id=message.
-000248d0: 6964 2c0a 2020 2020 2020 2020 2020 2020  id,.            
-000248e0: 2020 2020 6f70 7469 6f6e 3d31 0a20 2020      option=1.   
-000248f0: 2020 2020 2020 2020 2029 0a0a 2020 2020           )..    
-00024900: 2020 2020 4578 616d 706c 653a 0a20 2020      Example:.   
-00024910: 2020 2020 2020 2020 202e 2e20 636f 6465           .. code
-00024920: 2d62 6c6f 636b 3a3a 2070 7974 686f 6e0a  -block:: python.
-00024930: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00024940: 206d 6573 7361 6765 2e76 6f74 6528 3629   message.vote(6)
-00024950: 0a0a 2020 2020 2020 2020 5061 7261 6d65  ..        Parame
-00024960: 7465 7273 3a0a 2020 2020 2020 2020 2020  ters:.          
-00024970: 2020 6f70 7469 6f6e 2028 6060 696e 7460    option (``int`
-00024980: 6029 3a0a 2020 2020 2020 2020 2020 2020  `):.            
-00024990: 2020 2020 496e 6465 7820 6f66 2074 6865      Index of the
-000249a0: 2070 6f6c 6c20 6f70 7469 6f6e 2079 6f75   poll option you
-000249b0: 2077 616e 7420 746f 2076 6f74 6520 666f   want to vote fo
-000249c0: 7220 2830 2074 6f20 3929 2e0a 0a20 2020  r (0 to 9)...   
-000249d0: 2020 2020 2052 6574 7572 6e73 3a0a 2020       Returns:.  
-000249e0: 2020 2020 2020 2020 2020 3a6f 626a 3a60            :obj:`
-000249f0: 7e70 7972 6f67 7261 6d2e 7479 7065 732e  ~pyrogram.types.
-00024a00: 506f 6c6c 603a 204f 6e20 7375 6363 6573  Poll`: On succes
-00024a10: 732c 2074 6865 2070 6f6c 6c20 7769 7468  s, the poll with
-00024a20: 2074 6865 2063 686f 7365 6e20 6f70 7469   the chosen opti
-00024a30: 6f6e 2069 7320 7265 7475 726e 6564 2e0a  on is returned..
-00024a40: 0a20 2020 2020 2020 2052 6169 7365 733a  .        Raises:
-00024a50: 0a20 2020 2020 2020 2020 2020 2052 5043  .            RPC
-00024a60: 4572 726f 723a 2049 6e20 6361 7365 206f  Error: In case o
-00024a70: 6620 6120 5465 6c65 6772 616d 2052 5043  f a Telegram RPC
-00024a80: 2065 7272 6f72 2e0a 2020 2020 2020 2020   error..        
-00024a90: 2222 220a 0a20 2020 2020 2020 2072 6574  """..        ret
-00024aa0: 7572 6e20 6177 6169 7420 7365 6c66 2e5f  urn await self._
-00024ab0: 636c 6965 6e74 2e76 6f74 655f 706f 6c6c  client.vote_poll
-00024ac0: 280a 2020 2020 2020 2020 2020 2020 6368  (.            ch
-00024ad0: 6174 5f69 643d 7365 6c66 2e63 6861 742e  at_id=self.chat.
-00024ae0: 6964 2c0a 2020 2020 2020 2020 2020 2020  id,.            
-00024af0: 6d65 7373 6167 655f 6964 3d73 656c 662e  message_id=self.
-00024b00: 6964 2c0a 2020 2020 2020 2020 2020 2020  id,.            
-00024b10: 6f70 7469 6f6e 733d 6f70 7469 6f6e 0a20  options=option. 
-00024b20: 2020 2020 2020 2029 0a0a 2020 2020 6173         )..    as
-00024b30: 796e 6320 6465 6620 7069 6e28 7365 6c66  ync def pin(self
-00024b40: 2c20 6469 7361 626c 655f 6e6f 7469 6669  , disable_notifi
-00024b50: 6361 7469 6f6e 3a20 626f 6f6c 203d 2046  cation: bool = F
-00024b60: 616c 7365 2c20 626f 7468 5f73 6964 6573  alse, both_sides
-00024b70: 3a20 626f 6f6c 203d 2046 616c 7365 2920  : bool = False) 
-00024b80: 2d3e 2022 7479 7065 732e 4d65 7373 6167  -> "types.Messag
-00024b90: 6522 3a0a 2020 2020 2020 2020 2222 2242  e":.        """B
-00024ba0: 6f75 6e64 206d 6574 686f 6420 2a70 696e  ound method *pin
-00024bb0: 2a20 6f66 203a 6f62 6a3a 607e 7079 726f  * of :obj:`~pyro
-00024bc0: 6772 616d 2e74 7970 6573 2e4d 6573 7361  gram.types.Messa
-00024bd0: 6765 602e 0a0a 2020 2020 2020 2020 5573  ge`...        Us
-00024be0: 6520 6173 2061 2073 686f 7274 6375 7420  e as a shortcut 
-00024bf0: 666f 723a 0a0a 2020 2020 2020 2020 2e2e  for:..        ..
-00024c00: 2063 6f64 652d 626c 6f63 6b3a 3a20 7079   code-block:: py
-00024c10: 7468 6f6e 0a0a 2020 2020 2020 2020 2020  thon..          
-00024c20: 2020 6177 6169 7420 636c 6965 6e74 2e70    await client.p
-00024c30: 696e 5f63 6861 745f 6d65 7373 6167 6528  in_chat_message(
-00024c40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00024c50: 2063 6861 745f 6964 3d6d 6573 7361 6765   chat_id=message
-00024c60: 2e63 6861 742e 6964 2c0a 2020 2020 2020  .chat.id,.      
-00024c70: 2020 2020 2020 2020 2020 6d65 7373 6167            messag
-00024c80: 655f 6964 3d6d 6573 7361 6765 5f69 640a  e_id=message_id.
-00024c90: 2020 2020 2020 2020 2020 2020 290a 0a20              ).. 
-00024ca0: 2020 2020 2020 2045 7861 6d70 6c65 3a0a         Example:.
-00024cb0: 2020 2020 2020 2020 2020 2020 2e2e 2063              .. c
-00024cc0: 6f64 652d 626c 6f63 6b3a 3a20 7079 7468  ode-block:: pyth
-00024cd0: 6f6e 0a0a 2020 2020 2020 2020 2020 2020  on..            
-00024ce0: 2020 2020 6177 6169 7420 6d65 7373 6167      await messag
-00024cf0: 652e 7069 6e28 290a 0a20 2020 2020 2020  e.pin()..       
-00024d00: 2050 6172 616d 6574 6572 733a 0a20 2020   Parameters:.   
-00024d10: 2020 2020 2020 2020 2064 6973 6162 6c65           disable
-00024d20: 5f6e 6f74 6966 6963 6174 696f 6e20 2860  _notification (`
-00024d30: 6062 6f6f 6c60 6029 3a0a 2020 2020 2020  `bool``):.      
-00024d40: 2020 2020 2020 2020 2020 5061 7373 2054            Pass T
-00024d50: 7275 652c 2069 6620 6974 2069 7320 6e6f  rue, if it is no
-00024d60: 7420 6e65 6365 7373 6172 7920 746f 2073  t necessary to s
-00024d70: 656e 6420 6120 6e6f 7469 6669 6361 7469  end a notificati
-00024d80: 6f6e 2074 6f20 616c 6c20 6368 6174 206d  on to all chat m
-00024d90: 656d 6265 7273 2061 626f 7574 2074 6865  embers about the
-00024da0: 206e 6577 2070 696e 6e65 640a 2020 2020   new pinned.    
-00024db0: 2020 2020 2020 2020 2020 2020 6d65 7373              mess
-00024dc0: 6167 652e 204e 6f74 6966 6963 6174 696f  age. Notificatio
-00024dd0: 6e73 2061 7265 2061 6c77 6179 7320 6469  ns are always di
-00024de0: 7361 626c 6564 2069 6e20 6368 616e 6e65  sabled in channe
-00024df0: 6c73 2e0a 0a20 2020 2020 2020 2020 2020  ls...           
-00024e00: 2062 6f74 685f 7369 6465 7320 2860 6062   both_sides (``b
-00024e10: 6f6f 6c60 602c 202a 6f70 7469 6f6e 616c  ool``, *optional
-00024e20: 2a29 3a0a 2020 2020 2020 2020 2020 2020  *):.            
-00024e30: 2020 2020 5061 7373 2054 7275 6520 746f      Pass True to
-00024e40: 2070 696e 2074 6865 206d 6573 7361 6765   pin the message
-00024e50: 2066 6f72 2062 6f74 6820 7369 6465 7320   for both sides 
-00024e60: 2879 6f75 2061 6e64 2072 6563 6970 6965  (you and recipie
-00024e70: 6e74 292e 0a20 2020 2020 2020 2020 2020  nt)..           
-00024e80: 2020 2020 2041 7070 6c69 6361 626c 6520       Applicable 
-00024e90: 746f 2070 7269 7661 7465 2063 6861 7473  to private chats
-00024ea0: 206f 6e6c 792e 2044 6566 6175 6c74 7320   only. Defaults 
-00024eb0: 746f 2046 616c 7365 2e0a 0a20 2020 2020  to False...     
-00024ec0: 2020 2052 6574 7572 6e73 3a0a 2020 2020     Returns:.    
-00024ed0: 2020 2020 2020 2020 3a6f 626a 3a60 7e70          :obj:`~p
-00024ee0: 7972 6f67 7261 6d2e 7479 7065 732e 4d65  yrogram.types.Me
-00024ef0: 7373 6167 6560 3a20 4f6e 2073 7563 6365  ssage`: On succe
-00024f00: 7373 2c20 7468 6520 7365 7276 6963 6520  ss, the service 
-00024f10: 6d65 7373 6167 6520 6973 2072 6574 7572  message is retur
-00024f20: 6e65 642e 0a0a 2020 2020 2020 2020 5261  ned...        Ra
-00024f30: 6973 6573 3a0a 2020 2020 2020 2020 2020  ises:.          
-00024f40: 2020 5250 4345 7272 6f72 3a20 496e 2063    RPCError: In c
-00024f50: 6173 6520 6f66 2061 2054 656c 6567 7261  ase of a Telegra
-00024f60: 6d20 5250 4320 6572 726f 722e 0a20 2020  m RPC error..   
-00024f70: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00024f80: 2072 6574 7572 6e20 6177 6169 7420 7365   return await se
-00024f90: 6c66 2e5f 636c 6965 6e74 2e70 696e 5f63  lf._client.pin_c
-00024fa0: 6861 745f 6d65 7373 6167 6528 0a20 2020  hat_message(.   
-00024fb0: 2020 2020 2020 2020 2063 6861 745f 6964           chat_id
-00024fc0: 3d73 656c 662e 6368 6174 2e69 642c 0a20  =self.chat.id,. 
-00024fd0: 2020 2020 2020 2020 2020 206d 6573 7361             messa
-00024fe0: 6765 5f69 643d 7365 6c66 2e69 642c 0a20  ge_id=self.id,. 
-00024ff0: 2020 2020 2020 2020 2020 2064 6973 6162             disab
-00025000: 6c65 5f6e 6f74 6966 6963 6174 696f 6e3d  le_notification=
-00025010: 6469 7361 626c 655f 6e6f 7469 6669 6361  disable_notifica
-00025020: 7469 6f6e 2c0a 2020 2020 2020 2020 2020  tion,.          
-00025030: 2020 626f 7468 5f73 6964 6573 3d62 6f74    both_sides=bot
-00025040: 685f 7369 6465 730a 2020 2020 2020 2020  h_sides.        
-00025050: 290a 0a20 2020 2061 7379 6e63 2064 6566  )..    async def
-00025060: 2075 6e70 696e 2873 656c 6629 202d 3e20   unpin(self) -> 
-00025070: 626f 6f6c 3a0a 2020 2020 2020 2020 2222  bool:.        ""
-00025080: 2242 6f75 6e64 206d 6574 686f 6420 2a75  "Bound method *u
-00025090: 6e70 696e 2a20 6f66 203a 6f62 6a3a 607e  npin* of :obj:`~
-000250a0: 7079 726f 6772 616d 2e74 7970 6573 2e4d  pyrogram.types.M
-000250b0: 6573 7361 6765 602e 0a0a 2020 2020 2020  essage`...      
-000250c0: 2020 5573 6520 6173 2061 2073 686f 7274    Use as a short
-000250d0: 6375 7420 666f 723a 0a0a 2020 2020 2020  cut for:..      
-000250e0: 2020 2e2e 2063 6f64 652d 626c 6f63 6b3a    .. code-block:
-000250f0: 3a20 7079 7468 6f6e 0a0a 2020 2020 2020  : python..      
-00025100: 2020 2020 2020 6177 6169 7420 636c 6965        await clie
-00025110: 6e74 2e75 6e70 696e 5f63 6861 745f 6d65  nt.unpin_chat_me
-00025120: 7373 6167 6528 0a20 2020 2020 2020 2020  ssage(.         
-00025130: 2020 2020 2020 2063 6861 745f 6964 3d6d         chat_id=m
-00025140: 6573 7361 6765 2e63 6861 742e 6964 2c0a  essage.chat.id,.
-00025150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025160: 6d65 7373 6167 655f 6964 3d6d 6573 7361  message_id=messa
-00025170: 6765 5f69 640a 2020 2020 2020 2020 2020  ge_id.          
-00025180: 2020 290a 0a20 2020 2020 2020 2045 7861    )..        Exa
-00025190: 6d70 6c65 3a0a 2020 2020 2020 2020 2020  mple:.          
-000251a0: 2020 2e2e 2063 6f64 652d 626c 6f63 6b3a    .. code-block:
-000251b0: 3a20 7079 7468 6f6e 0a0a 2020 2020 2020  : python..      
-000251c0: 2020 2020 2020 2020 2020 6177 6169 7420            await 
-000251d0: 6d65 7373 6167 652e 756e 7069 6e28 290a  message.unpin().
-000251e0: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
-000251f0: 3a0a 2020 2020 2020 2020 2020 2020 5472  :.            Tr
-00025200: 7565 206f 6e20 7375 6363 6573 732e 0a0a  ue on success...
-00025210: 2020 2020 2020 2020 5261 6973 6573 3a0a          Raises:.
-00025220: 2020 2020 2020 2020 2020 2020 5250 4345              RPCE
-00025230: 7272 6f72 3a20 496e 2063 6173 6520 6f66  rror: In case of
-00025240: 2061 2054 656c 6567 7261 6d20 5250 4320   a Telegram RPC 
-00025250: 6572 726f 722e 0a20 2020 2020 2020 2022  error..        "
-00025260: 2222 0a20 2020 2020 2020 2072 6574 7572  "".        retur
-00025270: 6e20 6177 6169 7420 7365 6c66 2e5f 636c  n await self._cl
-00025280: 6965 6e74 2e75 6e70 696e 5f63 6861 745f  ient.unpin_chat_
-00025290: 6d65 7373 6167 6528 0a20 2020 2020 2020  message(.       
-000252a0: 2020 2020 2063 6861 745f 6964 3d73 656c       chat_id=sel
-000252b0: 662e 6368 6174 2e69 642c 0a20 2020 2020  f.chat.id,.     
-000252c0: 2020 2020 2020 206d 6573 7361 6765 5f69         message_i
-000252d0: 643d 7365 6c66 2e69 640a 2020 2020 2020  d=self.id.      
-000252e0: 2020 290a                                  ).
+000215f0: 2020 2020 666f 7572 7371 7561 7265 5f69      foursquare_i
+00021600: 643d 7365 6c66 2e76 656e 7565 2e66 6f75  d=self.venue.fou
+00021610: 7273 7175 6172 655f 6964 2c0a 2020 2020  rsquare_id,.    
+00021620: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021630: 666f 7572 7371 7561 7265 5f74 7970 653d  foursquare_type=
+00021640: 7365 6c66 2e76 656e 7565 2e66 6f75 7273  self.venue.fours
+00021650: 7175 6172 655f 7479 7065 2c0a 2020 2020  quare_type,.    
+00021660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021670: 6469 7361 626c 655f 6e6f 7469 6669 6361  disable_notifica
+00021680: 7469 6f6e 3d64 6973 6162 6c65 5f6e 6f74  tion=disable_not
+00021690: 6966 6963 6174 696f 6e2c 0a20 2020 2020  ification,.     
+000216a0: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+000216b0: 6573 7361 6765 5f74 6872 6561 645f 6964  essage_thread_id
+000216c0: 3d6d 6573 7361 6765 5f74 6872 6561 645f  =message_thread_
+000216d0: 6964 2c0a 2020 2020 2020 2020 2020 2020  id,.            
+000216e0: 2020 2020 2020 2020 7363 6865 6475 6c65          schedule
+000216f0: 5f64 6174 653d 7363 6865 6475 6c65 5f64  _date=schedule_d
+00021700: 6174 650a 2020 2020 2020 2020 2020 2020  ate.            
+00021710: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
+00021720: 2020 656c 6966 2073 656c 662e 706f 6c6c    elif self.poll
+00021730: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00021740: 2020 7265 7475 726e 2061 7761 6974 2073    return await s
+00021750: 656c 662e 5f63 6c69 656e 742e 7365 6e64  elf._client.send
+00021760: 5f70 6f6c 6c28 0a20 2020 2020 2020 2020  _poll(.         
+00021770: 2020 2020 2020 2020 2020 2063 6861 745f             chat_
+00021780: 6964 2c0a 2020 2020 2020 2020 2020 2020  id,.            
+00021790: 2020 2020 2020 2020 7175 6573 7469 6f6e          question
+000217a0: 3d73 656c 662e 706f 6c6c 2e71 7565 7374  =self.poll.quest
+000217b0: 696f 6e2c 0a20 2020 2020 2020 2020 2020  ion,.           
+000217c0: 2020 2020 2020 2020 206f 7074 696f 6e73           options
+000217d0: 3d5b 6f70 742e 7465 7874 2066 6f72 206f  =[opt.text for o
+000217e0: 7074 2069 6e20 7365 6c66 2e70 6f6c 6c2e  pt in self.poll.
+000217f0: 6f70 7469 6f6e 735d 2c0a 2020 2020 2020  options],.      
+00021800: 2020 2020 2020 2020 2020 2020 2020 6469                di
+00021810: 7361 626c 655f 6e6f 7469 6669 6361 7469  sable_notificati
+00021820: 6f6e 3d64 6973 6162 6c65 5f6e 6f74 6966  on=disable_notif
+00021830: 6963 6174 696f 6e2c 0a20 2020 2020 2020  ication,.       
+00021840: 2020 2020 2020 2020 2020 2020 206d 6573               mes
+00021850: 7361 6765 5f74 6872 6561 645f 6964 3d6d  sage_thread_id=m
+00021860: 6573 7361 6765 5f74 6872 6561 645f 6964  essage_thread_id
+00021870: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00021880: 2020 2020 2020 7363 6865 6475 6c65 5f64        schedule_d
+00021890: 6174 653d 7363 6865 6475 6c65 5f64 6174  ate=schedule_dat
+000218a0: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
+000218b0: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
+000218c0: 656c 6966 2073 656c 662e 6761 6d65 3a0a  elif self.game:.
+000218d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000218e0: 7265 7475 726e 2061 7761 6974 2073 656c  return await sel
+000218f0: 662e 5f63 6c69 656e 742e 7365 6e64 5f67  f._client.send_g
+00021900: 616d 6528 0a20 2020 2020 2020 2020 2020  ame(.           
+00021910: 2020 2020 2020 2020 2063 6861 745f 6964           chat_id
+00021920: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00021930: 2020 2020 2020 6761 6d65 5f73 686f 7274        game_short
+00021940: 5f6e 616d 653d 7365 6c66 2e67 616d 652e  _name=self.game.
+00021950: 7368 6f72 745f 6e61 6d65 2c0a 2020 2020  short_name,.    
+00021960: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021970: 6469 7361 626c 655f 6e6f 7469 6669 6361  disable_notifica
+00021980: 7469 6f6e 3d64 6973 6162 6c65 5f6e 6f74  tion=disable_not
+00021990: 6966 6963 6174 696f 6e2c 0a20 2020 2020  ification,.     
+000219a0: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+000219b0: 6573 7361 6765 5f74 6872 6561 645f 6964  essage_thread_id
+000219c0: 3d6d 6573 7361 6765 5f74 6872 6561 645f  =message_thread_
+000219d0: 6964 0a20 2020 2020 2020 2020 2020 2020  id.             
+000219e0: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
+000219f0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+00021a00: 2020 2020 2020 2072 6169 7365 2056 616c         raise Val
+00021a10: 7565 4572 726f 7228 2255 6e6b 6e6f 776e  ueError("Unknown
+00021a20: 206d 6564 6961 2074 7970 6522 290a 0a20   media type").. 
+00021a30: 2020 2020 2020 2020 2020 2069 6620 7365             if se
+00021a40: 6c66 2e73 7469 636b 6572 206f 7220 7365  lf.sticker or se
+00021a50: 6c66 2e76 6964 656f 5f6e 6f74 653a 2020  lf.video_note:  
+00021a60: 2320 5374 6963 6b65 7220 616e 6420 5669  # Sticker and Vi
+00021a70: 6465 6f4e 6f74 6520 7368 6f75 6c64 2068  deoNote should h
+00021a80: 6176 6520 6e6f 2063 6170 7469 6f6e 0a20  ave no caption. 
+00021a90: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00021aa0: 6574 7572 6e20 6177 6169 7420 7365 6e64  eturn await send
+00021ab0: 5f6d 6564 6961 280a 2020 2020 2020 2020  _media(.        
+00021ac0: 2020 2020 2020 2020 2020 2020 6669 6c65              file
+00021ad0: 5f69 643d 6669 6c65 5f69 642c 0a20 2020  _id=file_id,.   
+00021ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021af0: 206d 6573 7361 6765 5f74 6872 6561 645f   message_thread_
+00021b00: 6964 3d6d 6573 7361 6765 5f74 6872 6561  id=message_threa
+00021b10: 645f 6964 0a20 2020 2020 2020 2020 2020  d_id.           
+00021b20: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
+00021b30: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00021b40: 2020 2020 2020 2020 2069 6620 6361 7074           if capt
+00021b50: 696f 6e20 6973 204e 6f6e 653a 0a20 2020  ion is None:.   
+00021b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021b70: 2063 6170 7469 6f6e 203d 2073 656c 662e   caption = self.
+00021b80: 6361 7074 696f 6e20 6f72 2022 220a 2020  caption or "".  
+00021b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021ba0: 2020 6361 7074 696f 6e5f 656e 7469 7469    caption_entiti
+00021bb0: 6573 203d 2073 656c 662e 6361 7074 696f  es = self.captio
+00021bc0: 6e5f 656e 7469 7469 6573 0a0a 2020 2020  n_entities..    
+00021bd0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00021be0: 726e 2061 7761 6974 2073 656e 645f 6d65  rn await send_me
+00021bf0: 6469 6128 0a20 2020 2020 2020 2020 2020  dia(.           
+00021c00: 2020 2020 2020 2020 2066 696c 655f 6964           file_id
+00021c10: 3d66 696c 655f 6964 2c0a 2020 2020 2020  =file_id,.      
+00021c20: 2020 2020 2020 2020 2020 2020 2020 6361                ca
+00021c30: 7074 696f 6e3d 6361 7074 696f 6e2c 0a20  ption=caption,. 
+00021c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021c50: 2020 2070 6172 7365 5f6d 6f64 653d 7061     parse_mode=pa
+00021c60: 7273 655f 6d6f 6465 2c0a 2020 2020 2020  rse_mode,.      
+00021c70: 2020 2020 2020 2020 2020 2020 2020 6361                ca
+00021c80: 7074 696f 6e5f 656e 7469 7469 6573 3d63  ption_entities=c
+00021c90: 6170 7469 6f6e 5f65 6e74 6974 6965 732c  aption_entities,
+00021ca0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00021cb0: 2020 2020 206d 6573 7361 6765 5f74 6872       message_thr
+00021cc0: 6561 645f 6964 3d6d 6573 7361 6765 5f74  ead_id=message_t
+00021cd0: 6872 6561 645f 6964 0a20 2020 2020 2020  hread_id.       
+00021ce0: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+00021cf0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00021d00: 2020 2020 2072 6169 7365 2056 616c 7565       raise Value
+00021d10: 4572 726f 7228 2243 616e 2774 2063 6f70  Error("Can't cop
+00021d20: 7920 7468 6973 206d 6573 7361 6765 2229  y this message")
+00021d30: 0a0a 2020 2020 6173 796e 6320 6465 6620  ..    async def 
+00021d40: 6465 6c65 7465 2873 656c 662c 2072 6576  delete(self, rev
+00021d50: 6f6b 653a 2062 6f6f 6c20 3d20 5472 7565  oke: bool = True
+00021d60: 293a 0a20 2020 2020 2020 2022 2222 426f  ):.        """Bo
+00021d70: 756e 6420 6d65 7468 6f64 202a 6465 6c65  und method *dele
+00021d80: 7465 2a20 6f66 203a 6f62 6a3a 607e 7079  te* of :obj:`~py
+00021d90: 726f 6772 616d 2e74 7970 6573 2e4d 6573  rogram.types.Mes
+00021da0: 7361 6765 602e 0a0a 2020 2020 2020 2020  sage`...        
+00021db0: 5573 6520 6173 2061 2073 686f 7274 6375  Use as a shortcu
+00021dc0: 7420 666f 723a 0a0a 2020 2020 2020 2020  t for:..        
+00021dd0: 2e2e 2063 6f64 652d 626c 6f63 6b3a 3a20  .. code-block:: 
+00021de0: 7079 7468 6f6e 0a0a 2020 2020 2020 2020  python..        
+00021df0: 2020 2020 6177 6169 7420 636c 6965 6e74      await client
+00021e00: 2e64 656c 6574 655f 6d65 7373 6167 6573  .delete_messages
+00021e10: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00021e20: 2020 6368 6174 5f69 643d 6368 6174 5f69    chat_id=chat_i
+00021e30: 642c 0a20 2020 2020 2020 2020 2020 2020  d,.             
+00021e40: 2020 206d 6573 7361 6765 5f69 6473 3d6d     message_ids=m
+00021e50: 6573 7361 6765 2e69 640a 2020 2020 2020  essage.id.      
+00021e60: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
+00021e70: 2045 7861 6d70 6c65 3a0a 2020 2020 2020   Example:.      
+00021e80: 2020 2020 2020 2e2e 2063 6f64 652d 626c        .. code-bl
+00021e90: 6f63 6b3a 3a20 7079 7468 6f6e 0a0a 2020  ock:: python..  
+00021ea0: 2020 2020 2020 2020 2020 2020 2020 6177                aw
+00021eb0: 6169 7420 6d65 7373 6167 652e 6465 6c65  ait message.dele
+00021ec0: 7465 2829 0a0a 2020 2020 2020 2020 5061  te()..        Pa
+00021ed0: 7261 6d65 7465 7273 3a0a 2020 2020 2020  rameters:.      
+00021ee0: 2020 2020 2020 7265 766f 6b65 2028 6060        revoke (``
+00021ef0: 626f 6f6c 6060 2c20 2a6f 7074 696f 6e61  bool``, *optiona
+00021f00: 6c2a 293a 0a20 2020 2020 2020 2020 2020  l*):.           
+00021f10: 2020 2020 2044 656c 6574 6573 206d 6573       Deletes mes
+00021f20: 7361 6765 7320 6f6e 2062 6f74 6820 7061  sages on both pa
+00021f30: 7274 732e 0a20 2020 2020 2020 2020 2020  rts..           
+00021f40: 2020 2020 2054 6869 7320 6973 206f 6e6c       This is onl
+00021f50: 7920 666f 7220 7072 6976 6174 6520 636c  y for private cl
+00021f60: 6f75 6420 6368 6174 7320 616e 6420 6e6f  oud chats and no
+00021f70: 726d 616c 2067 726f 7570 732c 206d 6573  rmal groups, mes
+00021f80: 7361 6765 7320 6f6e 0a20 2020 2020 2020  sages on.       
+00021f90: 2020 2020 2020 2020 2063 6861 6e6e 656c           channel
+00021fa0: 7320 616e 6420 7375 7065 7267 726f 7570  s and supergroup
+00021fb0: 7320 6172 6520 616c 7761 7973 2072 6576  s are always rev
+00021fc0: 6f6b 6564 2028 692e 652e 3a20 6465 6c65  oked (i.e.: dele
+00021fd0: 7465 6420 666f 7220 6576 6572 796f 6e65  ted for everyone
+00021fe0: 292e 0a20 2020 2020 2020 2020 2020 2020  )..             
+00021ff0: 2020 2044 6566 6175 6c74 7320 746f 2054     Defaults to T
+00022000: 7275 652e 0a0a 2020 2020 2020 2020 5265  rue...        Re
+00022010: 7475 726e 733a 0a20 2020 2020 2020 2020  turns:.         
+00022020: 2020 2054 7275 6520 6f6e 2073 7563 6365     True on succe
+00022030: 7373 2c20 4661 6c73 6520 6f74 6865 7277  ss, False otherw
+00022040: 6973 652e 0a0a 2020 2020 2020 2020 5261  ise...        Ra
+00022050: 6973 6573 3a0a 2020 2020 2020 2020 2020  ises:.          
+00022060: 2020 5250 4345 7272 6f72 3a20 496e 2063    RPCError: In c
+00022070: 6173 6520 6f66 2061 2054 656c 6567 7261  ase of a Telegra
+00022080: 6d20 5250 4320 6572 726f 722e 0a20 2020  m RPC error..   
+00022090: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+000220a0: 2072 6574 7572 6e20 6177 6169 7420 7365   return await se
+000220b0: 6c66 2e5f 636c 6965 6e74 2e64 656c 6574  lf._client.delet
+000220c0: 655f 6d65 7373 6167 6573 280a 2020 2020  e_messages(.    
+000220d0: 2020 2020 2020 2020 6368 6174 5f69 643d          chat_id=
+000220e0: 7365 6c66 2e63 6861 742e 6964 2c0a 2020  self.chat.id,.  
+000220f0: 2020 2020 2020 2020 2020 6d65 7373 6167            messag
+00022100: 655f 6964 733d 7365 6c66 2e69 642c 0a20  e_ids=self.id,. 
+00022110: 2020 2020 2020 2020 2020 2072 6576 6f6b             revok
+00022120: 653d 7265 766f 6b65 0a20 2020 2020 2020  e=revoke.       
+00022130: 2029 0a0a 2020 2020 6173 796e 6320 6465   )..    async de
+00022140: 6620 636c 6963 6b28 7365 6c66 2c20 783a  f click(self, x:
+00022150: 2055 6e69 6f6e 5b69 6e74 2c20 7374 725d   Union[int, str]
+00022160: 203d 2030 2c20 793a 2069 6e74 203d 204e   = 0, y: int = N
+00022170: 6f6e 652c 2071 756f 7465 3a20 626f 6f6c  one, quote: bool
+00022180: 203d 204e 6f6e 652c 2074 696d 656f 7574   = None, timeout
+00022190: 3a20 696e 7420 3d20 3130 293a 0a20 2020  : int = 10):.   
+000221a0: 2020 2020 2022 2222 426f 756e 6420 6d65       """Bound me
+000221b0: 7468 6f64 202a 636c 6963 6b2a 206f 6620  thod *click* of 
+000221c0: 3a6f 626a 3a60 7e70 7972 6f67 7261 6d2e  :obj:`~pyrogram.
+000221d0: 7479 7065 732e 4d65 7373 6167 6560 2e0a  types.Message`..
+000221e0: 0a20 2020 2020 2020 2055 7365 2061 7320  .        Use as 
+000221f0: 6120 7368 6f72 7463 7574 2066 6f72 2063  a shortcut for c
+00022200: 6c69 636b 696e 6720 6120 6275 7474 6f6e  licking a button
+00022210: 2061 7474 6163 6865 6420 746f 2074 6865   attached to the
+00022220: 206d 6573 7361 6765 2069 6e73 7465 6164   message instead
+00022230: 206f 663a 0a0a 2020 2020 2020 2020 2d20   of:..        - 
+00022240: 436c 6963 6b69 6e67 2069 6e6c 696e 6520  Clicking inline 
+00022250: 6275 7474 6f6e 733a 0a0a 2020 2020 2020  buttons:..      
+00022260: 2020 2e2e 2063 6f64 652d 626c 6f63 6b3a    .. code-block:
+00022270: 3a20 7079 7468 6f6e 0a0a 2020 2020 2020  : python..      
+00022280: 2020 2020 2020 6177 6169 7420 636c 6965        await clie
+00022290: 6e74 2e72 6571 7565 7374 5f63 616c 6c62  nt.request_callb
+000222a0: 6163 6b5f 616e 7377 6572 280a 2020 2020  ack_answer(.    
+000222b0: 2020 2020 2020 2020 2020 2020 6368 6174              chat
+000222c0: 5f69 643d 6d65 7373 6167 652e 6368 6174  _id=message.chat
+000222d0: 2e69 642c 0a20 2020 2020 2020 2020 2020  .id,.           
+000222e0: 2020 2020 206d 6573 7361 6765 5f69 643d       message_id=
+000222f0: 6d65 7373 6167 652e 6964 2c0a 2020 2020  message.id,.    
+00022300: 2020 2020 2020 2020 2020 2020 6361 6c6c              call
+00022310: 6261 636b 5f64 6174 613d 6d65 7373 6167  back_data=messag
+00022320: 652e 7265 706c 795f 6d61 726b 7570 5b69  e.reply_markup[i
+00022330: 5d5b 6a5d 2e63 616c 6c62 6163 6b5f 6461  ][j].callback_da
+00022340: 7461 0a20 2020 2020 2020 2020 2020 2029  ta.            )
+00022350: 0a0a 2020 2020 2020 2020 2d20 436c 6963  ..        - Clic
+00022360: 6b69 6e67 206e 6f72 6d61 6c20 6275 7474  king normal butt
+00022370: 6f6e 733a 0a0a 2020 2020 2020 2020 2e2e  ons:..        ..
+00022380: 2063 6f64 652d 626c 6f63 6b3a 3a20 7079   code-block:: py
+00022390: 7468 6f6e 0a0a 2020 2020 2020 2020 2020  thon..          
+000223a0: 2020 6177 6169 7420 636c 6965 6e74 2e73    await client.s
+000223b0: 656e 645f 6d65 7373 6167 6528 0a20 2020  end_message(.   
+000223c0: 2020 2020 2020 2020 2020 2020 2063 6861               cha
+000223d0: 745f 6964 3d6d 6573 7361 6765 2e63 6861  t_id=message.cha
+000223e0: 742e 6964 2c0a 2020 2020 2020 2020 2020  t.id,.          
+000223f0: 2020 2020 2020 7465 7874 3d6d 6573 7361        text=messa
+00022400: 6765 2e72 6570 6c79 5f6d 6172 6b75 705b  ge.reply_markup[
+00022410: 695d 5b6a 5d2e 7465 7874 0a20 2020 2020  i][j].text.     
+00022420: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
+00022430: 2020 4578 616d 706c 653a 0a20 2020 2020    Example:.     
+00022440: 2020 2020 2020 2054 6869 7320 6d65 7468         This meth
+00022450: 6f64 2063 616e 2062 6520 7573 6564 2069  od can be used i
+00022460: 6e20 7468 7265 6520 6469 6666 6572 656e  n three differen
+00022470: 7420 7761 7973 3a0a 0a20 2020 2020 2020  t ways:..       
+00022480: 2020 2020 2031 2e20 2050 6173 7320 6f6e       1.  Pass on
+00022490: 6520 696e 7465 6765 7220 6172 6775 6d65  e integer argume
+000224a0: 6e74 206f 6e6c 7920 2865 2e67 2e3a 2060  nt only (e.g.: `
+000224b0: 602e 636c 6963 6b28 3229 6060 2c20 746f  `.click(2)``, to
+000224c0: 2063 6c69 636b 2061 2062 7574 746f 6e20   click a button 
+000224d0: 6174 2069 6e64 6578 2032 292e 0a20 2020  at index 2)..   
+000224e0: 2020 2020 2020 2020 2020 2020 2042 7574               But
+000224f0: 746f 6e73 2061 7265 2063 6f75 6e74 6564  tons are counted
+00022500: 206c 6566 7420 746f 2072 6967 6874 2c20   left to right, 
+00022510: 7374 6172 7469 6e67 2066 726f 6d20 7468  starting from th
+00022520: 6520 746f 702e 0a0a 2020 2020 2020 2020  e top...        
+00022530: 2020 2020 322e 2020 5061 7373 2074 776f      2.  Pass two
+00022540: 2069 6e74 6567 6572 2061 7267 756d 656e   integer argumen
+00022550: 7473 2028 652e 672e 3a20 6060 2e63 6c69  ts (e.g.: ``.cli
+00022560: 636b 2831 2c20 3029 6060 2c20 746f 2063  ck(1, 0)``, to c
+00022570: 6c69 636b 2061 2062 7574 746f 6e20 6174  lick a button at
+00022580: 2070 6f73 6974 696f 6e20 2831 2c20 3029   position (1, 0)
+00022590: 292e 0a20 2020 2020 2020 2020 2020 2020  )..             
+000225a0: 2020 2054 6865 206f 7269 6769 6e20 2830     The origin (0
+000225b0: 2c20 3029 2069 7320 746f 702d 6c65 6674  , 0) is top-left
+000225c0: 2e0a 0a20 2020 2020 2020 2020 2020 2033  ...            3
+000225d0: 2e20 2050 6173 7320 6f6e 6520 7374 7269  .  Pass one stri
+000225e0: 6e67 2061 7267 756d 656e 7420 6f6e 6c79  ng argument only
+000225f0: 2028 652e 672e 3a20 6060 2e63 6c69 636b   (e.g.: ``.click
+00022600: 2822 5365 7474 696e 6773 2229 6060 2c20  ("Settings")``, 
+00022610: 746f 2063 6c69 636b 2061 2062 7574 746f  to click a butto
+00022620: 6e20 6279 2075 7369 6e67 2069 7473 206c  n by using its l
+00022630: 6162 656c 292e 0a20 2020 2020 2020 2020  abel)..         
+00022640: 2020 2020 2020 204f 6e6c 7920 7468 6520         Only the 
+00022650: 6669 7273 7420 6d61 7463 6869 6e67 2062  first matching b
+00022660: 7574 746f 6e20 7769 6c6c 2062 6520 7072  utton will be pr
+00022670: 6573 7365 642e 0a0a 2020 2020 2020 2020  essed...        
+00022680: 5061 7261 6d65 7465 7273 3a0a 2020 2020  Parameters:.    
+00022690: 2020 2020 2020 2020 7820 2860 6069 6e74          x (``int
+000226a0: 6060 207c 2060 6073 7472 6060 293a 0a20  `` | ``str``):. 
+000226b0: 2020 2020 2020 2020 2020 2020 2020 2055                 U
+000226c0: 7365 6420 6173 2069 6e74 6567 6572 2069  sed as integer i
+000226d0: 6e64 6578 2c20 696e 7465 6765 7220 6162  ndex, integer ab
+000226e0: 7363 6973 7361 2028 696e 2070 6169 7220  scissa (in pair 
+000226f0: 7769 7468 2079 2920 6f72 2061 7320 7374  with y) or as st
+00022700: 7269 6e67 206c 6162 656c 2e0a 2020 2020  ring label..    
+00022710: 2020 2020 2020 2020 2020 2020 4465 6661              Defa
+00022720: 756c 7473 2074 6f20 3020 2866 6972 7374  ults to 0 (first
+00022730: 2062 7574 746f 6e29 2e0a 0a20 2020 2020   button)...     
+00022740: 2020 2020 2020 2079 2028 6060 696e 7460         y (``int`
+00022750: 602c 202a 6f70 7469 6f6e 616c 2a29 3a0a  `, *optional*):.
+00022760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022770: 5573 6564 2061 7320 6f72 6469 6e61 7465  Used as ordinate
+00022780: 206f 6e6c 7920 2869 6e20 7061 6972 2077   only (in pair w
+00022790: 6974 6820 7829 2e0a 0a20 2020 2020 2020  ith x)...       
+000227a0: 2020 2020 2071 756f 7465 2028 6060 626f       quote (``bo
+000227b0: 6f6c 6060 2c20 2a6f 7074 696f 6e61 6c2a  ol``, *optional*
+000227c0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+000227d0: 2020 2055 7365 6675 6c20 666f 7220 6e6f     Useful for no
+000227e0: 726d 616c 2062 7574 746f 6e73 206f 6e6c  rmal buttons onl
+000227f0: 792c 2077 6865 7265 2070 7265 7373 696e  y, where pressin
+00022800: 6720 6974 2077 696c 6c20 7265 7375 6c74  g it will result
+00022810: 2069 6e20 6120 6e65 7720 6d65 7373 6167   in a new messag
+00022820: 6520 7365 6e74 2e0a 2020 2020 2020 2020  e sent..        
+00022830: 2020 2020 2020 2020 4966 2060 6054 7275          If ``Tru
+00022840: 6560 602c 2074 6865 206d 6573 7361 6765  e``, the message
+00022850: 2077 696c 6c20 6265 2073 656e 7420 6173   will be sent as
+00022860: 2061 2072 6570 6c79 2074 6f20 7468 6973   a reply to this
+00022870: 206d 6573 7361 6765 2e0a 2020 2020 2020   message..      
+00022880: 2020 2020 2020 2020 2020 4465 6661 756c            Defaul
+00022890: 7473 2074 6f20 6060 5472 7565 6060 2069  ts to ``True`` i
+000228a0: 6e20 6772 6f75 7020 6368 6174 7320 616e  n group chats an
+000228b0: 6420 6060 4661 6c73 6560 6020 696e 2070  d ``False`` in p
+000228c0: 7269 7661 7465 2063 6861 7473 2e0a 0a20  rivate chats... 
+000228d0: 2020 2020 2020 2020 2020 2074 696d 656f             timeo
+000228e0: 7574 2028 6060 696e 7460 602c 202a 6f70  ut (``int``, *op
+000228f0: 7469 6f6e 616c 2a29 3a0a 2020 2020 2020  tional*):.      
+00022900: 2020 2020 2020 2020 2020 5469 6d65 6f75            Timeou
+00022910: 7420 696e 2073 6563 6f6e 6473 2e0a 0a20  t in seconds... 
+00022920: 2020 2020 2020 2052 6574 7572 6e73 3a0a         Returns:.
+00022930: 2020 2020 2020 2020 2020 2020 2d20 2020              -   
+00022940: 5468 6520 7265 7375 6c74 206f 6620 3a6d  The result of :m
+00022950: 6574 683a 607e 7079 726f 6772 616d 2e43  eth:`~pyrogram.C
+00022960: 6c69 656e 742e 7265 7175 6573 745f 6361  lient.request_ca
+00022970: 6c6c 6261 636b 5f61 6e73 7765 7260 2069  llback_answer` i
+00022980: 6e20 6361 7365 206f 6620 696e 6c69 6e65  n case of inline
+00022990: 2063 616c 6c62 6163 6b20 6275 7474 6f6e   callback button
+000229a0: 2063 6c69 636b 732e 0a20 2020 2020 2020   clicks..       
+000229b0: 2020 2020 202d 2020 2054 6865 2072 6573       -   The res
+000229c0: 756c 7420 6f66 203a 6d65 7468 3a60 7e4d  ult of :meth:`~M
+000229d0: 6573 7361 6765 2e72 6570 6c79 2829 6020  essage.reply()` 
+000229e0: 696e 2063 6173 6520 6f66 206e 6f72 6d61  in case of norma
+000229f0: 6c20 6275 7474 6f6e 2063 6c69 636b 732e  l button clicks.
+00022a00: 0a20 2020 2020 2020 2020 2020 202d 2020  .            -  
+00022a10: 2041 2073 7472 696e 6720 696e 2063 6173   A string in cas
+00022a20: 6520 7468 6520 696e 6c69 6e65 2062 7574  e the inline but
+00022a30: 746f 6e20 6973 2061 2055 524c 2c20 6120  ton is a URL, a 
+00022a40: 2a73 7769 7463 685f 696e 6c69 6e65 5f71  *switch_inline_q
+00022a50: 7565 7279 2a20 6f72 2061 0a20 2020 2020  uery* or a.     
+00022a60: 2020 2020 2020 2020 2020 202a 7377 6974             *swit
+00022a70: 6368 5f69 6e6c 696e 655f 7175 6572 795f  ch_inline_query_
+00022a80: 6375 7272 656e 745f 6368 6174 2a20 6275  current_chat* bu
+00022a90: 7474 6f6e 2e0a 0a20 2020 2020 2020 2052  tton...        R
+00022aa0: 6169 7365 733a 0a20 2020 2020 2020 2020  aises:.         
+00022ab0: 2020 2052 5043 4572 726f 723a 2049 6e20     RPCError: In 
+00022ac0: 6361 7365 206f 6620 6120 5465 6c65 6772  case of a Telegr
+00022ad0: 616d 2052 5043 2065 7272 6f72 2e0a 2020  am RPC error..  
+00022ae0: 2020 2020 2020 2020 2020 5661 6c75 6545            ValueE
+00022af0: 7272 6f72 3a20 496e 2063 6173 6520 7468  rror: In case th
+00022b00: 6520 7072 6f76 6964 6564 2069 6e64 6578  e provided index
+00022b10: 206f 7220 706f 7369 7469 6f6e 2069 7320   or position is 
+00022b20: 6f75 7420 6f66 2072 616e 6765 206f 7220  out of range or 
+00022b30: 7468 6520 6275 7474 6f6e 206c 6162 656c  the button label
+00022b40: 2077 6173 206e 6f74 2066 6f75 6e64 2e0a   was not found..
+00022b50: 2020 2020 2020 2020 2020 2020 5469 6d65              Time
+00022b60: 6f75 7445 7272 6f72 3a20 496e 2063 6173  outError: In cas
+00022b70: 652c 2061 6674 6572 2063 6c69 636b 696e  e, after clickin
+00022b80: 6720 616e 2069 6e6c 696e 6520 6275 7474  g an inline butt
+00022b90: 6f6e 2c20 7468 6520 626f 7420 6661 696c  on, the bot fail
+00022ba0: 7320 746f 2061 6e73 7765 7220 7769 7468  s to answer with
+00022bb0: 696e 2074 6865 2074 696d 656f 7574 2e0a  in the timeout..
+00022bc0: 2020 2020 2020 2020 2222 220a 0a20 2020          """..   
+00022bd0: 2020 2020 2069 6620 6973 696e 7374 616e       if isinstan
+00022be0: 6365 2873 656c 662e 7265 706c 795f 6d61  ce(self.reply_ma
+00022bf0: 726b 7570 2c20 7479 7065 732e 5265 706c  rkup, types.Repl
+00022c00: 794b 6579 626f 6172 644d 6172 6b75 7029  yKeyboardMarkup)
+00022c10: 3a0a 2020 2020 2020 2020 2020 2020 6b65  :.            ke
+00022c20: 7962 6f61 7264 203d 2073 656c 662e 7265  yboard = self.re
+00022c30: 706c 795f 6d61 726b 7570 2e6b 6579 626f  ply_markup.keybo
+00022c40: 6172 640a 2020 2020 2020 2020 2020 2020  ard.            
+00022c50: 6973 5f69 6e6c 696e 6520 3d20 4661 6c73  is_inline = Fals
+00022c60: 650a 2020 2020 2020 2020 656c 6966 2069  e.        elif i
+00022c70: 7369 6e73 7461 6e63 6528 7365 6c66 2e72  sinstance(self.r
+00022c80: 6570 6c79 5f6d 6172 6b75 702c 2074 7970  eply_markup, typ
+00022c90: 6573 2e49 6e6c 696e 654b 6579 626f 6172  es.InlineKeyboar
+00022ca0: 644d 6172 6b75 7029 3a0a 2020 2020 2020  dMarkup):.      
+00022cb0: 2020 2020 2020 6b65 7962 6f61 7264 203d        keyboard =
+00022cc0: 2073 656c 662e 7265 706c 795f 6d61 726b   self.reply_mark
+00022cd0: 7570 2e69 6e6c 696e 655f 6b65 7962 6f61  up.inline_keyboa
+00022ce0: 7264 0a20 2020 2020 2020 2020 2020 2069  rd.            i
+00022cf0: 735f 696e 6c69 6e65 203d 2054 7275 650a  s_inline = True.
+00022d00: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+00022d10: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+00022d20: 5661 6c75 6545 7272 6f72 2822 5468 6520  ValueError("The 
+00022d30: 6d65 7373 6167 6520 646f 6573 6e27 7420  message doesn't 
+00022d40: 636f 6e74 6169 6e20 616e 7920 6b65 7962  contain any keyb
+00022d50: 6f61 7264 2229 0a0a 2020 2020 2020 2020  oard")..        
+00022d60: 6966 2069 7369 6e73 7461 6e63 6528 782c  if isinstance(x,
+00022d70: 2069 6e74 2920 616e 6420 7920 6973 204e   int) and y is N
+00022d80: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00022d90: 2074 7279 3a0a 2020 2020 2020 2020 2020   try:.          
+00022da0: 2020 2020 2020 6275 7474 6f6e 203d 205b        button = [
+00022db0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00022dc0: 2020 2020 2062 7574 746f 6e0a 2020 2020       button.    
+00022dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022de0: 666f 7220 726f 7720 696e 206b 6579 626f  for row in keybo
+00022df0: 6172 640a 2020 2020 2020 2020 2020 2020  ard.            
+00022e00: 2020 2020 2020 2020 666f 7220 6275 7474          for butt
+00022e10: 6f6e 2069 6e20 726f 770a 2020 2020 2020  on in row.      
+00022e20: 2020 2020 2020 2020 2020 5d5b 785d 0a20            ][x]. 
+00022e30: 2020 2020 2020 2020 2020 2065 7863 6570             excep
+00022e40: 7420 496e 6465 7845 7272 6f72 3a0a 2020  t IndexError:.  
+00022e50: 2020 2020 2020 2020 2020 2020 2020 7261                ra
+00022e60: 6973 6520 5661 6c75 6545 7272 6f72 2866  ise ValueError(f
+00022e70: 2254 6865 2062 7574 746f 6e20 6174 2069  "The button at i
+00022e80: 6e64 6578 207b 787d 2064 6f65 736e 2774  ndex {x} doesn't
+00022e90: 2065 7869 7374 2229 0a20 2020 2020 2020   exist").       
+00022ea0: 2065 6c69 6620 6973 696e 7374 616e 6365   elif isinstance
+00022eb0: 2878 2c20 696e 7429 2061 6e64 2069 7369  (x, int) and isi
+00022ec0: 6e73 7461 6e63 6528 792c 2069 6e74 293a  nstance(y, int):
+00022ed0: 0a20 2020 2020 2020 2020 2020 2074 7279  .            try
+00022ee0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00022ef0: 2020 6275 7474 6f6e 203d 206b 6579 626f    button = keybo
+00022f00: 6172 645b 795d 5b78 5d0a 2020 2020 2020  ard[y][x].      
+00022f10: 2020 2020 2020 6578 6365 7074 2049 6e64        except Ind
+00022f20: 6578 4572 726f 723a 0a20 2020 2020 2020  exError:.       
+00022f30: 2020 2020 2020 2020 2072 6169 7365 2056           raise V
+00022f40: 616c 7565 4572 726f 7228 6622 5468 6520  alueError(f"The 
+00022f50: 6275 7474 6f6e 2061 7420 706f 7369 7469  button at positi
+00022f60: 6f6e 2028 7b78 7d2c 207b 797d 2920 646f  on ({x}, {y}) do
+00022f70: 6573 6e27 7420 6578 6973 7422 290a 2020  esn't exist").  
+00022f80: 2020 2020 2020 656c 6966 2069 7369 6e73        elif isins
+00022f90: 7461 6e63 6528 782c 2073 7472 2920 616e  tance(x, str) an
+00022fa0: 6420 7920 6973 204e 6f6e 653a 0a20 2020  d y is None:.   
+00022fb0: 2020 2020 2020 2020 206c 6162 656c 203d           label =
+00022fc0: 2078 2e65 6e63 6f64 6528 2275 7466 2d31   x.encode("utf-1
+00022fd0: 3622 2c20 2273 7572 726f 6761 7465 7061  6", "surrogatepa
+00022fe0: 7373 2229 2e64 6563 6f64 6528 2275 7466  ss").decode("utf
+00022ff0: 2d31 3622 290a 0a20 2020 2020 2020 2020  -16")..         
+00023000: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
+00023010: 2020 2020 2020 2020 6275 7474 6f6e 203d          button =
+00023020: 205b 0a20 2020 2020 2020 2020 2020 2020   [.             
+00023030: 2020 2020 2020 2062 7574 746f 6e0a 2020         button.  
+00023040: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023050: 2020 666f 7220 726f 7720 696e 206b 6579    for row in key
+00023060: 626f 6172 640a 2020 2020 2020 2020 2020  board.          
+00023070: 2020 2020 2020 2020 2020 666f 7220 6275            for bu
+00023080: 7474 6f6e 2069 6e20 726f 770a 2020 2020  tton in row.    
+00023090: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000230a0: 6966 206c 6162 656c 203d 3d20 6275 7474  if label == butt
+000230b0: 6f6e 2e74 6578 740a 2020 2020 2020 2020  on.text.        
+000230c0: 2020 2020 2020 2020 5d5b 305d 0a20 2020          ][0].   
+000230d0: 2020 2020 2020 2020 2065 7863 6570 7420           except 
+000230e0: 496e 6465 7845 7272 6f72 3a0a 2020 2020  IndexError:.    
+000230f0: 2020 2020 2020 2020 2020 2020 7261 6973              rais
+00023100: 6520 5661 6c75 6545 7272 6f72 2866 2254  e ValueError(f"T
+00023110: 6865 2062 7574 746f 6e20 7769 7468 206c  he button with l
+00023120: 6162 656c 2027 7b78 7d27 2064 6f65 736e  abel '{x}' doesn
+00023130: 2774 2065 7869 7374 7322 290a 2020 2020  't exists").    
+00023140: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00023150: 2020 2020 2020 7261 6973 6520 5661 6c75        raise Valu
+00023160: 6545 7272 6f72 2822 496e 7661 6c69 6420  eError("Invalid 
+00023170: 6172 6775 6d65 6e74 7322 290a 0a20 2020  arguments")..   
+00023180: 2020 2020 2069 6620 6973 5f69 6e6c 696e       if is_inlin
+00023190: 653a 0a20 2020 2020 2020 2020 2020 2069  e:.            i
+000231a0: 6620 6275 7474 6f6e 2e63 616c 6c62 6163  f button.callbac
+000231b0: 6b5f 6461 7461 3a0a 2020 2020 2020 2020  k_data:.        
+000231c0: 2020 2020 2020 2020 7265 7475 726e 2061          return a
+000231d0: 7761 6974 2073 656c 662e 5f63 6c69 656e  wait self._clien
+000231e0: 742e 7265 7175 6573 745f 6361 6c6c 6261  t.request_callba
+000231f0: 636b 5f61 6e73 7765 7228 0a20 2020 2020  ck_answer(.     
+00023200: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00023210: 6861 745f 6964 3d73 656c 662e 6368 6174  hat_id=self.chat
+00023220: 2e69 642c 0a20 2020 2020 2020 2020 2020  .id,.           
+00023230: 2020 2020 2020 2020 206d 6573 7361 6765           message
+00023240: 5f69 643d 7365 6c66 2e69 642c 0a20 2020  _id=self.id,.   
+00023250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023260: 2063 616c 6c62 6163 6b5f 6461 7461 3d62   callback_data=b
+00023270: 7574 746f 6e2e 6361 6c6c 6261 636b 5f64  utton.callback_d
+00023280: 6174 612c 0a20 2020 2020 2020 2020 2020  ata,.           
+00023290: 2020 2020 2020 2020 2074 696d 656f 7574           timeout
+000232a0: 3d74 696d 656f 7574 0a20 2020 2020 2020  =timeout.       
+000232b0: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+000232c0: 2020 2020 2020 2065 6c69 6620 6275 7474         elif butt
+000232d0: 6f6e 2e75 726c 3a0a 2020 2020 2020 2020  on.url:.        
+000232e0: 2020 2020 2020 2020 7265 7475 726e 2062          return b
+000232f0: 7574 746f 6e2e 7572 6c0a 2020 2020 2020  utton.url.      
+00023300: 2020 2020 2020 656c 6966 2062 7574 746f        elif butto
+00023310: 6e2e 7377 6974 6368 5f69 6e6c 696e 655f  n.switch_inline_
+00023320: 7175 6572 793a 0a20 2020 2020 2020 2020  query:.         
+00023330: 2020 2020 2020 2072 6574 7572 6e20 6275         return bu
+00023340: 7474 6f6e 2e73 7769 7463 685f 696e 6c69  tton.switch_inli
+00023350: 6e65 5f71 7565 7279 0a20 2020 2020 2020  ne_query.       
+00023360: 2020 2020 2065 6c69 6620 6275 7474 6f6e       elif button
+00023370: 2e73 7769 7463 685f 696e 6c69 6e65 5f71  .switch_inline_q
+00023380: 7565 7279 5f63 7572 7265 6e74 5f63 6861  uery_current_cha
+00023390: 743a 0a20 2020 2020 2020 2020 2020 2020  t:.             
+000233a0: 2020 2072 6574 7572 6e20 6275 7474 6f6e     return button
+000233b0: 2e73 7769 7463 685f 696e 6c69 6e65 5f71  .switch_inline_q
+000233c0: 7565 7279 5f63 7572 7265 6e74 5f63 6861  uery_current_cha
+000233d0: 740a 2020 2020 2020 2020 2020 2020 656c  t.            el
+000233e0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+000233f0: 2020 2020 7261 6973 6520 5661 6c75 6545      raise ValueE
+00023400: 7272 6f72 2822 5468 6973 2062 7574 746f  rror("This butto
+00023410: 6e20 6973 206e 6f74 2073 7570 706f 7274  n is not support
+00023420: 6564 2079 6574 2229 0a20 2020 2020 2020  ed yet").       
+00023430: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+00023440: 2020 2061 7761 6974 2073 656c 662e 7265     await self.re
+00023450: 706c 7928 6275 7474 6f6e 2c20 7175 6f74  ply(button, quot
+00023460: 653d 7175 6f74 6529 0a0a 2020 2020 6173  e=quote)..    as
+00023470: 796e 6320 6465 6620 7265 6163 7428 7365  ync def react(se
+00023480: 6c66 2c20 656d 6f6a 693a 2073 7472 203d  lf, emoji: str =
+00023490: 2022 222c 2062 6967 3a20 626f 6f6c 203d   "", big: bool =
+000234a0: 2046 616c 7365 2920 2d3e 2062 6f6f 6c3a   False) -> bool:
+000234b0: 0a20 2020 2020 2020 2022 2222 426f 756e  .        """Boun
+000234c0: 6420 6d65 7468 6f64 202a 7265 6163 742a  d method *react*
+000234d0: 206f 6620 3a6f 626a 3a60 7e70 7972 6f67   of :obj:`~pyrog
+000234e0: 7261 6d2e 7479 7065 732e 4d65 7373 6167  ram.types.Messag
+000234f0: 6560 2e0a 0a20 2020 2020 2020 2055 7365  e`...        Use
+00023500: 2061 7320 6120 7368 6f72 7463 7574 2066   as a shortcut f
+00023510: 6f72 3a0a 0a20 2020 2020 2020 202e 2e20  or:..        .. 
+00023520: 636f 6465 2d62 6c6f 636b 3a3a 2070 7974  code-block:: pyt
+00023530: 686f 6e0a 0a20 2020 2020 2020 2020 2020  hon..           
+00023540: 2061 7761 6974 2063 6c69 656e 742e 7365   await client.se
+00023550: 6e64 5f72 6561 6374 696f 6e28 0a20 2020  nd_reaction(.   
+00023560: 2020 2020 2020 2020 2020 2020 2063 6861               cha
+00023570: 745f 6964 3d63 6861 745f 6964 2c0a 2020  t_id=chat_id,.  
+00023580: 2020 2020 2020 2020 2020 2020 2020 6d65                me
+00023590: 7373 6167 655f 6964 3d6d 6573 7361 6765  ssage_id=message
+000235a0: 2e69 642c 0a20 2020 2020 2020 2020 2020  .id,.           
+000235b0: 2020 2020 2065 6d6f 6a69 3d22 f09f 94a5       emoji="....
+000235c0: 220a 2020 2020 2020 2020 2020 2020 290a  ".            ).
+000235d0: 0a20 2020 2020 2020 2045 7861 6d70 6c65  .        Example
+000235e0: 3a0a 2020 2020 2020 2020 2020 2020 2e2e  :.            ..
+000235f0: 2063 6f64 652d 626c 6f63 6b3a 3a20 7079   code-block:: py
+00023600: 7468 6f6e 0a0a 2020 2020 2020 2020 2020  thon..          
+00023610: 2020 2020 2020 6177 6169 7420 6d65 7373        await mess
+00023620: 6167 652e 7265 6163 7428 656d 6f6a 693d  age.react(emoji=
+00023630: 22f0 9f94 a522 290a 0a20 2020 2020 2020  "....")..       
+00023640: 2050 6172 616d 6574 6572 733a 0a20 2020   Parameters:.   
+00023650: 2020 2020 2020 2020 2065 6d6f 6a69 2028           emoji (
+00023660: 6060 7374 7260 602c 202a 6f70 7469 6f6e  ``str``, *option
+00023670: 616c 2a29 3a0a 2020 2020 2020 2020 2020  al*):.          
+00023680: 2020 2020 2020 5265 6163 7469 6f6e 2065        Reaction e
+00023690: 6d6f 6a69 2e0a 2020 2020 2020 2020 2020  moji..          
+000236a0: 2020 2020 2020 5061 7373 2022 2220 6173        Pass "" as
+000236b0: 2065 6d6f 6a69 2028 6465 6661 756c 7429   emoji (default)
+000236c0: 2074 6f20 7265 7472 6163 7420 7468 6520   to retract the 
+000236d0: 7265 6163 7469 6f6e 2e0a 2020 2020 2020  reaction..      
+000236e0: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+000236f0: 2020 2020 6269 6720 2860 6062 6f6f 6c60      big (``bool`
+00023700: 602c 202a 6f70 7469 6f6e 616c 2a29 3a0a  `, *optional*):.
+00023710: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023720: 5061 7373 2054 7275 6520 746f 2073 686f  Pass True to sho
+00023730: 7720 6120 6269 6767 6572 2061 6e64 206c  w a bigger and l
+00023740: 6f6e 6765 7220 7265 6163 7469 6f6e 2e0a  onger reaction..
+00023750: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023760: 4465 6661 756c 7473 2074 6f20 4661 6c73  Defaults to Fals
+00023770: 652e 0a0a 2020 2020 2020 2020 5265 7475  e...        Retu
+00023780: 726e 733a 0a20 2020 2020 2020 2020 2020  rns:.           
+00023790: 2060 6062 6f6f 6c60 603a 204f 6e20 7375   ``bool``: On su
+000237a0: 6363 6573 732c 2054 7275 6520 6973 2072  ccess, True is r
+000237b0: 6574 7572 6e65 642e 0a0a 2020 2020 2020  eturned...      
+000237c0: 2020 5261 6973 6573 3a0a 2020 2020 2020    Raises:.      
+000237d0: 2020 2020 2020 5250 4345 7272 6f72 3a20        RPCError: 
+000237e0: 496e 2063 6173 6520 6f66 2061 2054 656c  In case of a Tel
+000237f0: 6567 7261 6d20 5250 4320 6572 726f 722e  egram RPC error.
+00023800: 0a20 2020 2020 2020 2022 2222 0a0a 2020  .        """..  
+00023810: 2020 2020 2020 7265 7475 726e 2061 7761        return awa
+00023820: 6974 2073 656c 662e 5f63 6c69 656e 742e  it self._client.
+00023830: 7365 6e64 5f72 6561 6374 696f 6e28 0a20  send_reaction(. 
+00023840: 2020 2020 2020 2020 2020 2063 6861 745f             chat_
+00023850: 6964 3d73 656c 662e 6368 6174 2e69 642c  id=self.chat.id,
+00023860: 0a20 2020 2020 2020 2020 2020 206d 6573  .            mes
+00023870: 7361 6765 5f69 643d 7365 6c66 2e69 642c  sage_id=self.id,
+00023880: 0a20 2020 2020 2020 2020 2020 2065 6d6f  .            emo
+00023890: 6a69 3d65 6d6f 6a69 2c0a 2020 2020 2020  ji=emoji,.      
+000238a0: 2020 2020 2020 6269 673d 6269 670a 2020        big=big.  
+000238b0: 2020 2020 2020 290a 0a20 2020 2061 7379        )..    asy
+000238c0: 6e63 2064 6566 2072 6574 7261 6374 5f76  nc def retract_v
+000238d0: 6f74 6528 0a20 2020 2020 2020 2073 656c  ote(.        sel
+000238e0: 662c 0a20 2020 2029 202d 3e20 2274 7970  f,.    ) -> "typ
+000238f0: 6573 2e50 6f6c 6c22 3a0a 2020 2020 2020  es.Poll":.      
+00023900: 2020 2222 2242 6f75 6e64 206d 6574 686f    """Bound metho
+00023910: 6420 2a72 6574 7261 6374 5f76 6f74 652a  d *retract_vote*
+00023920: 206f 6620 3a6f 626a 3a60 7e70 7972 6f67   of :obj:`~pyrog
+00023930: 7261 6d2e 7479 7065 732e 4d65 7373 6167  ram.types.Messag
+00023940: 6560 2e0a 0a20 2020 2020 2020 2055 7365  e`...        Use
+00023950: 2061 7320 6120 7368 6f72 7463 7574 2066   as a shortcut f
+00023960: 6f72 3a0a 0a20 2020 2020 2020 202e 2e20  or:..        .. 
+00023970: 636f 6465 2d62 6c6f 636b 3a3a 2070 7974  code-block:: pyt
+00023980: 686f 6e0a 0a20 2020 2020 2020 2020 2020  hon..           
+00023990: 2063 6c69 656e 742e 7265 7472 6163 745f   client.retract_
+000239a0: 766f 7465 280a 2020 2020 2020 2020 2020  vote(.          
+000239b0: 2020 2020 2020 6368 6174 5f69 643d 6d65        chat_id=me
+000239c0: 7373 6167 652e 6368 6174 2e69 642c 0a20  ssage.chat.id,. 
+000239d0: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+000239e0: 6573 7361 6765 5f69 643d 6d65 7373 6167  essage_id=messag
+000239f0: 655f 6964 2c0a 2020 2020 2020 2020 2020  e_id,.          
+00023a00: 2020 290a 0a20 2020 2020 2020 2045 7861    )..        Exa
+00023a10: 6d70 6c65 3a0a 2020 2020 2020 2020 2020  mple:.          
+00023a20: 2020 2e2e 2063 6f64 652d 626c 6f63 6b3a    .. code-block:
+00023a30: 3a20 7079 7468 6f6e 0a0a 2020 2020 2020  : python..      
+00023a40: 2020 2020 2020 2020 2020 6d65 7373 6167            messag
+00023a50: 652e 7265 7472 6163 745f 766f 7465 2829  e.retract_vote()
+00023a60: 0a0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
+00023a70: 733a 0a20 2020 2020 2020 2020 2020 203a  s:.            :
+00023a80: 6f62 6a3a 607e 7079 726f 6772 616d 2e74  obj:`~pyrogram.t
+00023a90: 7970 6573 2e50 6f6c 6c60 3a20 4f6e 2073  ypes.Poll`: On s
+00023aa0: 7563 6365 7373 2c20 7468 6520 706f 6c6c  uccess, the poll
+00023ab0: 2077 6974 6820 7468 6520 7265 7472 6163   with the retrac
+00023ac0: 7465 6420 766f 7465 2069 7320 7265 7475  ted vote is retu
+00023ad0: 726e 6564 2e0a 0a20 2020 2020 2020 2052  rned...        R
+00023ae0: 6169 7365 733a 0a20 2020 2020 2020 2020  aises:.         
+00023af0: 2020 2052 5043 4572 726f 723a 2049 6e20     RPCError: In 
+00023b00: 6361 7365 206f 6620 6120 5465 6c65 6772  case of a Telegr
+00023b10: 616d 2052 5043 2065 7272 6f72 2e0a 2020  am RPC error..  
+00023b20: 2020 2020 2020 2222 220a 0a20 2020 2020        """..     
+00023b30: 2020 2072 6574 7572 6e20 6177 6169 7420     return await 
+00023b40: 7365 6c66 2e5f 636c 6965 6e74 2e72 6574  self._client.ret
+00023b50: 7261 6374 5f76 6f74 6528 0a20 2020 2020  ract_vote(.     
+00023b60: 2020 2020 2020 2063 6861 745f 6964 3d73         chat_id=s
+00023b70: 656c 662e 6368 6174 2e69 642c 0a20 2020  elf.chat.id,.   
+00023b80: 2020 2020 2020 2020 206d 6573 7361 6765           message
+00023b90: 5f69 643d 7365 6c66 2e69 640a 2020 2020  _id=self.id.    
+00023ba0: 2020 2020 290a 0a20 2020 2061 7379 6e63      )..    async
+00023bb0: 2064 6566 2064 6f77 6e6c 6f61 6428 0a20   def download(. 
+00023bc0: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
+00023bd0: 2020 2020 2066 696c 655f 6e61 6d65 3a20       file_name: 
+00023be0: 7374 7220 3d20 2222 2c0a 2020 2020 2020  str = "",.      
+00023bf0: 2020 696e 5f6d 656d 6f72 793a 2062 6f6f    in_memory: boo
+00023c00: 6c20 3d20 4661 6c73 652c 0a20 2020 2020  l = False,.     
+00023c10: 2020 2062 6c6f 636b 3a20 626f 6f6c 203d     block: bool =
+00023c20: 2054 7275 652c 0a20 2020 2020 2020 2070   True,.        p
+00023c30: 726f 6772 6573 733a 2043 616c 6c61 626c  rogress: Callabl
+00023c40: 6520 3d20 4e6f 6e65 2c0a 2020 2020 2020  e = None,.      
+00023c50: 2020 7072 6f67 7265 7373 5f61 7267 733a    progress_args:
+00023c60: 2074 7570 6c65 203d 2028 290a 2020 2020   tuple = ().    
+00023c70: 2920 2d3e 2073 7472 3a0a 2020 2020 2020  ) -> str:.      
+00023c80: 2020 2222 2242 6f75 6e64 206d 6574 686f    """Bound metho
+00023c90: 6420 2a64 6f77 6e6c 6f61 642a 206f 6620  d *download* of 
+00023ca0: 3a6f 626a 3a60 7e70 7972 6f67 7261 6d2e  :obj:`~pyrogram.
+00023cb0: 7479 7065 732e 4d65 7373 6167 6560 2e0a  types.Message`..
+00023cc0: 0a20 2020 2020 2020 2055 7365 2061 7320  .        Use as 
+00023cd0: 6120 7368 6f72 7463 7574 2066 6f72 3a0a  a shortcut for:.
+00023ce0: 0a20 2020 2020 2020 202e 2e20 636f 6465  .        .. code
+00023cf0: 2d62 6c6f 636b 3a3a 2070 7974 686f 6e0a  -block:: python.
+00023d00: 0a20 2020 2020 2020 2020 2020 2061 7761  .            awa
+00023d10: 6974 2063 6c69 656e 742e 646f 776e 6c6f  it client.downlo
+00023d20: 6164 5f6d 6564 6961 286d 6573 7361 6765  ad_media(message
+00023d30: 290a 0a20 2020 2020 2020 2045 7861 6d70  )..        Examp
+00023d40: 6c65 3a0a 2020 2020 2020 2020 2020 2020  le:.            
+00023d50: 2e2e 2063 6f64 652d 626c 6f63 6b3a 3a20  .. code-block:: 
+00023d60: 7079 7468 6f6e 0a0a 2020 2020 2020 2020  python..        
+00023d70: 2020 2020 2020 2020 6177 6169 7420 6d65          await me
+00023d80: 7373 6167 652e 646f 776e 6c6f 6164 2829  ssage.download()
+00023d90: 0a0a 2020 2020 2020 2020 5061 7261 6d65  ..        Parame
+00023da0: 7465 7273 3a0a 2020 2020 2020 2020 2020  ters:.          
+00023db0: 2020 6669 6c65 5f6e 616d 6520 2860 6073    file_name (``s
+00023dc0: 7472 6060 2c20 2a6f 7074 696f 6e61 6c2a  tr``, *optional*
+00023dd0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+00023de0: 2020 2041 2063 7573 746f 6d20 2a66 696c     A custom *fil
+00023df0: 655f 6e61 6d65 2a20 746f 2062 6520 7573  e_name* to be us
+00023e00: 6564 2069 6e73 7465 6164 206f 6620 7468  ed instead of th
+00023e10: 6520 6f6e 6520 7072 6f76 6964 6564 2062  e one provided b
+00023e20: 7920 5465 6c65 6772 616d 2e0a 2020 2020  y Telegram..    
+00023e30: 2020 2020 2020 2020 2020 2020 4279 2064              By d
+00023e40: 6566 6175 6c74 2c20 616c 6c20 6669 6c65  efault, all file
+00023e50: 7320 6172 6520 646f 776e 6c6f 6164 6564  s are downloaded
+00023e60: 2069 6e20 7468 6520 2a64 6f77 6e6c 6f61   in the *downloa
+00023e70: 6473 2a20 666f 6c64 6572 2069 6e20 796f  ds* folder in yo
+00023e80: 7572 2077 6f72 6b69 6e67 2064 6972 6563  ur working direc
+00023e90: 746f 7279 2e0a 2020 2020 2020 2020 2020  tory..          
+00023ea0: 2020 2020 2020 596f 7520 6361 6e20 616c        You can al
+00023eb0: 736f 2073 7065 6369 6679 2061 2070 6174  so specify a pat
+00023ec0: 6820 666f 7220 646f 776e 6c6f 6164 696e  h for downloadin
+00023ed0: 6720 6669 6c65 7320 696e 2061 2063 7573  g files in a cus
+00023ee0: 746f 6d20 6c6f 6361 7469 6f6e 3a20 7061  tom location: pa
+00023ef0: 7468 7320 7468 6174 2065 6e64 2077 6974  ths that end wit
+00023f00: 6820 222f 220a 2020 2020 2020 2020 2020  h "/".          
+00023f10: 2020 2020 2020 6172 6520 636f 6e73 6964        are consid
+00023f20: 6572 6564 2064 6972 6563 746f 7269 6573  ered directories
+00023f30: 2e20 416c 6c20 6e6f 6e2d 6578 6973 7465  . All non-existe
+00023f40: 6e74 2066 6f6c 6465 7273 2077 696c 6c20  nt folders will 
+00023f50: 6265 2063 7265 6174 6564 2061 7574 6f6d  be created autom
+00023f60: 6174 6963 616c 6c79 2e0a 0a20 2020 2020  atically...     
+00023f70: 2020 2020 2020 2069 6e5f 6d65 6d6f 7279         in_memory
+00023f80: 2028 6060 626f 6f6c 6060 2c20 2a6f 7074   (``bool``, *opt
+00023f90: 696f 6e61 6c2a 293a 0a20 2020 2020 2020  ional*):.       
+00023fa0: 2020 2020 2020 2020 2050 6173 7320 5472           Pass Tr
+00023fb0: 7565 2074 6f20 646f 776e 6c6f 6164 2074  ue to download t
+00023fc0: 6865 206d 6564 6961 2069 6e2d 6d65 6d6f  he media in-memo
+00023fd0: 7279 2e0a 2020 2020 2020 2020 2020 2020  ry..            
+00023fe0: 2020 2020 4120 6269 6e61 7279 2066 696c      A binary fil
+00023ff0: 652d 6c69 6b65 206f 626a 6563 7420 7769  e-like object wi
+00024000: 7468 2069 7473 2061 7474 7269 6275 7465  th its attribute
+00024010: 2022 2e6e 616d 6522 2073 6574 2077 696c   ".name" set wil
+00024020: 6c20 6265 2072 6574 7572 6e65 642e 0a20  l be returned.. 
+00024030: 2020 2020 2020 2020 2020 2020 2020 2044                 D
+00024040: 6566 6175 6c74 7320 746f 2046 616c 7365  efaults to False
+00024050: 2e0a 0a20 2020 2020 2020 2020 2020 2062  ...            b
+00024060: 6c6f 636b 2028 6060 626f 6f6c 6060 2c20  lock (``bool``, 
+00024070: 2a6f 7074 696f 6e61 6c2a 293a 0a20 2020  *optional*):.   
+00024080: 2020 2020 2020 2020 2020 2020 2042 6c6f               Blo
+00024090: 636b 7320 7468 6520 636f 6465 2065 7865  cks the code exe
+000240a0: 6375 7469 6f6e 2075 6e74 696c 2074 6865  cution until the
+000240b0: 2066 696c 6520 6861 7320 6265 656e 2064   file has been d
+000240c0: 6f77 6e6c 6f61 6465 642e 0a20 2020 2020  ownloaded..     
+000240d0: 2020 2020 2020 2020 2020 2044 6566 6175             Defau
+000240e0: 6c74 7320 746f 2054 7275 652e 0a0a 2020  lts to True...  
+000240f0: 2020 2020 2020 2020 2020 7072 6f67 7265            progre
+00024100: 7373 2028 6060 4361 6c6c 6162 6c65 6060  ss (``Callable``
+00024110: 2c20 2a6f 7074 696f 6e61 6c2a 293a 0a20  , *optional*):. 
+00024120: 2020 2020 2020 2020 2020 2020 2020 2050                 P
+00024130: 6173 7320 6120 6361 6c6c 6261 636b 2066  ass a callback f
+00024140: 756e 6374 696f 6e20 746f 2076 6965 7720  unction to view 
+00024150: 7468 6520 6669 6c65 2074 7261 6e73 6d69  the file transmi
+00024160: 7373 696f 6e20 7072 6f67 7265 7373 2e0a  ssion progress..
+00024170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00024180: 5468 6520 6675 6e63 7469 6f6e 206d 7573  The function mus
+00024190: 7420 7461 6b65 202a 2863 7572 7265 6e74  t take *(current
+000241a0: 2c20 746f 7461 6c29 2a20 6173 2070 6f73  , total)* as pos
+000241b0: 6974 696f 6e61 6c20 6172 6775 6d65 6e74  itional argument
+000241c0: 7320 286c 6f6f 6b20 6174 204f 7468 6572  s (look at Other
+000241d0: 2050 6172 616d 6574 6572 7320 6265 6c6f   Parameters belo
+000241e0: 7720 666f 7220 610a 2020 2020 2020 2020  w for a.        
+000241f0: 2020 2020 2020 2020 6465 7461 696c 6564          detailed
+00024200: 2064 6573 6372 6970 7469 6f6e 2920 616e   description) an
+00024210: 6420 7769 6c6c 2062 6520 6361 6c6c 6564  d will be called
+00024220: 2062 6163 6b20 6561 6368 2074 696d 6520   back each time 
+00024230: 6120 6e65 7720 6669 6c65 2063 6875 6e6b  a new file chunk
+00024240: 2068 6173 2062 6565 6e20 7375 6363 6573   has been succes
+00024250: 7366 756c 6c79 0a20 2020 2020 2020 2020  sfully.         
+00024260: 2020 2020 2020 2074 7261 6e73 6d69 7474         transmitt
+00024270: 6564 2e0a 0a20 2020 2020 2020 2020 2020  ed...           
+00024280: 2070 726f 6772 6573 735f 6172 6773 2028   progress_args (
+00024290: 6060 7475 706c 6560 602c 202a 6f70 7469  ``tuple``, *opti
+000242a0: 6f6e 616c 2a29 3a0a 2020 2020 2020 2020  onal*):.        
+000242b0: 2020 2020 2020 2020 4578 7472 6120 6375          Extra cu
+000242c0: 7374 6f6d 2061 7267 756d 656e 7473 2066  stom arguments f
+000242d0: 6f72 2074 6865 2070 726f 6772 6573 7320  or the progress 
+000242e0: 6361 6c6c 6261 636b 2066 756e 6374 696f  callback functio
+000242f0: 6e2e 0a20 2020 2020 2020 2020 2020 2020  n..             
+00024300: 2020 2059 6f75 2063 616e 2070 6173 7320     You can pass 
+00024310: 616e 7974 6869 6e67 2079 6f75 206e 6565  anything you nee
+00024320: 6420 746f 2062 6520 6176 6169 6c61 626c  d to be availabl
+00024330: 6520 696e 2074 6865 2070 726f 6772 6573  e in the progres
+00024340: 7320 6361 6c6c 6261 636b 2073 636f 7065  s callback scope
+00024350: 3b20 666f 7220 6578 616d 706c 652c 2061  ; for example, a
+00024360: 204d 6573 7361 6765 0a20 2020 2020 2020   Message.       
+00024370: 2020 2020 2020 2020 206f 626a 6563 7420           object 
+00024380: 6f72 2061 2043 6c69 656e 7420 696e 7374  or a Client inst
+00024390: 616e 6365 2069 6e20 6f72 6465 7220 746f  ance in order to
+000243a0: 2065 6469 7420 7468 6520 6d65 7373 6167   edit the messag
+000243b0: 6520 7769 7468 2074 6865 2075 7064 6174  e with the updat
+000243c0: 6564 2070 726f 6772 6573 7320 7374 6174  ed progress stat
+000243d0: 7573 2e0a 0a20 2020 2020 2020 204f 7468  us...        Oth
+000243e0: 6572 2050 6172 616d 6574 6572 733a 0a20  er Parameters:. 
+000243f0: 2020 2020 2020 2020 2020 2063 7572 7265             curre
+00024400: 6e74 2028 6060 696e 7460 6029 3a0a 2020  nt (``int``):.  
+00024410: 2020 2020 2020 2020 2020 2020 2020 5468                Th
+00024420: 6520 616d 6f75 6e74 206f 6620 6279 7465  e amount of byte
+00024430: 7320 7472 616e 736d 6974 7465 6420 736f  s transmitted so
+00024440: 2066 6172 2e0a 0a20 2020 2020 2020 2020   far...         
+00024450: 2020 2074 6f74 616c 2028 6060 696e 7460     total (``int`
+00024460: 6029 3a0a 2020 2020 2020 2020 2020 2020  `):.            
+00024470: 2020 2020 5468 6520 746f 7461 6c20 7369      The total si
+00024480: 7a65 206f 6620 7468 6520 6669 6c65 2e0a  ze of the file..
+00024490: 0a20 2020 2020 2020 2020 2020 202a 6172  .            *ar
+000244a0: 6773 2028 6060 7475 706c 6560 602c 202a  gs (``tuple``, *
+000244b0: 6f70 7469 6f6e 616c 2a29 3a0a 2020 2020  optional*):.    
+000244c0: 2020 2020 2020 2020 2020 2020 4578 7472              Extr
+000244d0: 6120 6375 7374 6f6d 2061 7267 756d 656e  a custom argumen
+000244e0: 7473 2061 7320 6465 6669 6e65 6420 696e  ts as defined in
+000244f0: 2074 6865 2060 6070 726f 6772 6573 735f   the ``progress_
+00024500: 6172 6773 6060 2070 6172 616d 6574 6572  args`` parameter
+00024510: 2e0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00024520: 2020 596f 7520 6361 6e20 6569 7468 6572    You can either
+00024530: 206b 6565 7020 6060 2a61 7267 7360 6020   keep ``*args`` 
+00024540: 6f72 2061 6464 2065 7665 7279 2073 696e  or add every sin
+00024550: 676c 6520 6578 7472 6120 6172 6775 6d65  gle extra argume
+00024560: 6e74 2069 6e20 796f 7572 2066 756e 6374  nt in your funct
+00024570: 696f 6e20 7369 676e 6174 7572 652e 0a0a  ion signature...
+00024580: 2020 2020 2020 2020 5265 7475 726e 733a          Returns:
+00024590: 0a20 2020 2020 2020 2020 2020 204f 6e20  .            On 
+000245a0: 7375 6363 6573 732c 2074 6865 2061 6273  success, the abs
+000245b0: 6f6c 7574 6520 7061 7468 206f 6620 7468  olute path of th
+000245c0: 6520 646f 776e 6c6f 6164 6564 2066 696c  e downloaded fil
+000245d0: 6520 6173 2073 7472 696e 6720 6973 2072  e as string is r
+000245e0: 6574 7572 6e65 642c 204e 6f6e 6520 6f74  eturned, None ot
+000245f0: 6865 7277 6973 652e 0a0a 2020 2020 2020  herwise...      
+00024600: 2020 5261 6973 6573 3a0a 2020 2020 2020    Raises:.      
+00024610: 2020 2020 2020 5250 4345 7272 6f72 3a20        RPCError: 
+00024620: 496e 2063 6173 6520 6f66 2061 2054 656c  In case of a Tel
+00024630: 6567 7261 6d20 5250 4320 6572 726f 722e  egram RPC error.
+00024640: 0a20 2020 2020 2020 2020 2020 2060 6056  .            ``V
+00024650: 616c 7565 4572 726f 7260 603a 2049 6620  alueError``: If 
+00024660: 7468 6520 6d65 7373 6167 6520 646f 6573  the message does
+00024670: 6e27 7420 636f 6e74 6169 6e20 616e 7920  n't contain any 
+00024680: 646f 776e 6c6f 6164 6162 6c65 206d 6564  downloadable med
+00024690: 6961 0a20 2020 2020 2020 2022 2222 0a20  ia.        """. 
+000246a0: 2020 2020 2020 2072 6574 7572 6e20 6177         return aw
+000246b0: 6169 7420 7365 6c66 2e5f 636c 6965 6e74  ait self._client
+000246c0: 2e64 6f77 6e6c 6f61 645f 6d65 6469 6128  .download_media(
+000246d0: 0a20 2020 2020 2020 2020 2020 206d 6573  .            mes
+000246e0: 7361 6765 3d73 656c 662c 0a20 2020 2020  sage=self,.     
+000246f0: 2020 2020 2020 2066 696c 655f 6e61 6d65         file_name
+00024700: 3d66 696c 655f 6e61 6d65 2c0a 2020 2020  =file_name,.    
+00024710: 2020 2020 2020 2020 696e 5f6d 656d 6f72          in_memor
+00024720: 793d 696e 5f6d 656d 6f72 792c 0a20 2020  y=in_memory,.   
+00024730: 2020 2020 2020 2020 2062 6c6f 636b 3d62           block=b
+00024740: 6c6f 636b 2c0a 2020 2020 2020 2020 2020  lock,.          
+00024750: 2020 7072 6f67 7265 7373 3d70 726f 6772    progress=progr
+00024760: 6573 732c 0a20 2020 2020 2020 2020 2020  ess,.           
+00024770: 2070 726f 6772 6573 735f 6172 6773 3d70   progress_args=p
+00024780: 726f 6772 6573 735f 6172 6773 2c0a 2020  rogress_args,.  
+00024790: 2020 2020 2020 290a 0a20 2020 2061 7379        )..    asy
+000247a0: 6e63 2064 6566 2076 6f74 6528 0a20 2020  nc def vote(.   
+000247b0: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
+000247c0: 2020 206f 7074 696f 6e3a 2069 6e74 2c0a     option: int,.
+000247d0: 2020 2020 2920 2d3e 2022 7479 7065 732e      ) -> "types.
+000247e0: 506f 6c6c 223a 0a20 2020 2020 2020 2022  Poll":.        "
+000247f0: 2222 426f 756e 6420 6d65 7468 6f64 202a  ""Bound method *
+00024800: 766f 7465 2a20 6f66 203a 6f62 6a3a 607e  vote* of :obj:`~
+00024810: 7079 726f 6772 616d 2e74 7970 6573 2e4d  pyrogram.types.M
+00024820: 6573 7361 6765 602e 0a0a 2020 2020 2020  essage`...      
+00024830: 2020 5573 6520 6173 2061 2073 686f 7274    Use as a short
+00024840: 6375 7420 666f 723a 0a0a 2020 2020 2020  cut for:..      
+00024850: 2020 2e2e 2063 6f64 652d 626c 6f63 6b3a    .. code-block:
+00024860: 3a20 7079 7468 6f6e 0a0a 2020 2020 2020  : python..      
+00024870: 2020 2020 2020 636c 6965 6e74 2e76 6f74        client.vot
+00024880: 655f 706f 6c6c 280a 2020 2020 2020 2020  e_poll(.        
+00024890: 2020 2020 2020 2020 6368 6174 5f69 643d          chat_id=
+000248a0: 6d65 7373 6167 652e 6368 6174 2e69 642c  message.chat.id,
+000248b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000248c0: 206d 6573 7361 6765 5f69 643d 6d65 7373   message_id=mess
+000248d0: 6167 652e 6964 2c0a 2020 2020 2020 2020  age.id,.        
+000248e0: 2020 2020 2020 2020 6f70 7469 6f6e 3d31          option=1
+000248f0: 0a20 2020 2020 2020 2020 2020 2029 0a0a  .            )..
+00024900: 2020 2020 2020 2020 4578 616d 706c 653a          Example:
+00024910: 0a20 2020 2020 2020 2020 2020 202e 2e20  .            .. 
+00024920: 636f 6465 2d62 6c6f 636b 3a3a 2070 7974  code-block:: pyt
+00024930: 686f 6e0a 0a20 2020 2020 2020 2020 2020  hon..           
+00024940: 2020 2020 206d 6573 7361 6765 2e76 6f74       message.vot
+00024950: 6528 3629 0a0a 2020 2020 2020 2020 5061  e(6)..        Pa
+00024960: 7261 6d65 7465 7273 3a0a 2020 2020 2020  rameters:.      
+00024970: 2020 2020 2020 6f70 7469 6f6e 2028 6060        option (``
+00024980: 696e 7460 6029 3a0a 2020 2020 2020 2020  int``):.        
+00024990: 2020 2020 2020 2020 496e 6465 7820 6f66          Index of
+000249a0: 2074 6865 2070 6f6c 6c20 6f70 7469 6f6e   the poll option
+000249b0: 2079 6f75 2077 616e 7420 746f 2076 6f74   you want to vot
+000249c0: 6520 666f 7220 2830 2074 6f20 3929 2e0a  e for (0 to 9)..
+000249d0: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
+000249e0: 3a0a 2020 2020 2020 2020 2020 2020 3a6f  :.            :o
+000249f0: 626a 3a60 7e70 7972 6f67 7261 6d2e 7479  bj:`~pyrogram.ty
+00024a00: 7065 732e 506f 6c6c 603a 204f 6e20 7375  pes.Poll`: On su
+00024a10: 6363 6573 732c 2074 6865 2070 6f6c 6c20  ccess, the poll 
+00024a20: 7769 7468 2074 6865 2063 686f 7365 6e20  with the chosen 
+00024a30: 6f70 7469 6f6e 2069 7320 7265 7475 726e  option is return
+00024a40: 6564 2e0a 0a20 2020 2020 2020 2052 6169  ed...        Rai
+00024a50: 7365 733a 0a20 2020 2020 2020 2020 2020  ses:.           
+00024a60: 2052 5043 4572 726f 723a 2049 6e20 6361   RPCError: In ca
+00024a70: 7365 206f 6620 6120 5465 6c65 6772 616d  se of a Telegram
+00024a80: 2052 5043 2065 7272 6f72 2e0a 2020 2020   RPC error..    
+00024a90: 2020 2020 2222 220a 0a20 2020 2020 2020      """..       
+00024aa0: 2072 6574 7572 6e20 6177 6169 7420 7365   return await se
+00024ab0: 6c66 2e5f 636c 6965 6e74 2e76 6f74 655f  lf._client.vote_
+00024ac0: 706f 6c6c 280a 2020 2020 2020 2020 2020  poll(.          
+00024ad0: 2020 6368 6174 5f69 643d 7365 6c66 2e63    chat_id=self.c
+00024ae0: 6861 742e 6964 2c0a 2020 2020 2020 2020  hat.id,.        
+00024af0: 2020 2020 6d65 7373 6167 655f 6964 3d73      message_id=s
+00024b00: 656c 662e 6964 2c0a 2020 2020 2020 2020  elf.id,.        
+00024b10: 2020 2020 6f70 7469 6f6e 733d 6f70 7469      options=opti
+00024b20: 6f6e 0a20 2020 2020 2020 2029 0a0a 2020  on.        )..  
+00024b30: 2020 6173 796e 6320 6465 6620 7069 6e28    async def pin(
+00024b40: 7365 6c66 2c20 6469 7361 626c 655f 6e6f  self, disable_no
+00024b50: 7469 6669 6361 7469 6f6e 3a20 626f 6f6c  tification: bool
+00024b60: 203d 2046 616c 7365 2c20 626f 7468 5f73   = False, both_s
+00024b70: 6964 6573 3a20 626f 6f6c 203d 2046 616c  ides: bool = Fal
+00024b80: 7365 2920 2d3e 2022 7479 7065 732e 4d65  se) -> "types.Me
+00024b90: 7373 6167 6522 3a0a 2020 2020 2020 2020  ssage":.        
+00024ba0: 2222 2242 6f75 6e64 206d 6574 686f 6420  """Bound method 
+00024bb0: 2a70 696e 2a20 6f66 203a 6f62 6a3a 607e  *pin* of :obj:`~
+00024bc0: 7079 726f 6772 616d 2e74 7970 6573 2e4d  pyrogram.types.M
+00024bd0: 6573 7361 6765 602e 0a0a 2020 2020 2020  essage`...      
+00024be0: 2020 5573 6520 6173 2061 2073 686f 7274    Use as a short
+00024bf0: 6375 7420 666f 723a 0a0a 2020 2020 2020  cut for:..      
+00024c00: 2020 2e2e 2063 6f64 652d 626c 6f63 6b3a    .. code-block:
+00024c10: 3a20 7079 7468 6f6e 0a0a 2020 2020 2020  : python..      
+00024c20: 2020 2020 2020 6177 6169 7420 636c 6965        await clie
+00024c30: 6e74 2e70 696e 5f63 6861 745f 6d65 7373  nt.pin_chat_mess
+00024c40: 6167 6528 0a20 2020 2020 2020 2020 2020  age(.           
+00024c50: 2020 2020 2063 6861 745f 6964 3d6d 6573       chat_id=mes
+00024c60: 7361 6765 2e63 6861 742e 6964 2c0a 2020  sage.chat.id,.  
+00024c70: 2020 2020 2020 2020 2020 2020 2020 6d65                me
+00024c80: 7373 6167 655f 6964 3d6d 6573 7361 6765  ssage_id=message
+00024c90: 5f69 640a 2020 2020 2020 2020 2020 2020  _id.            
+00024ca0: 290a 0a20 2020 2020 2020 2045 7861 6d70  )..        Examp
+00024cb0: 6c65 3a0a 2020 2020 2020 2020 2020 2020  le:.            
+00024cc0: 2e2e 2063 6f64 652d 626c 6f63 6b3a 3a20  .. code-block:: 
+00024cd0: 7079 7468 6f6e 0a0a 2020 2020 2020 2020  python..        
+00024ce0: 2020 2020 2020 2020 6177 6169 7420 6d65          await me
+00024cf0: 7373 6167 652e 7069 6e28 290a 0a20 2020  ssage.pin()..   
+00024d00: 2020 2020 2050 6172 616d 6574 6572 733a       Parameters:
+00024d10: 0a20 2020 2020 2020 2020 2020 2064 6973  .            dis
+00024d20: 6162 6c65 5f6e 6f74 6966 6963 6174 696f  able_notificatio
+00024d30: 6e20 2860 6062 6f6f 6c60 6029 3a0a 2020  n (``bool``):.  
+00024d40: 2020 2020 2020 2020 2020 2020 2020 5061                Pa
+00024d50: 7373 2054 7275 652c 2069 6620 6974 2069  ss True, if it i
+00024d60: 7320 6e6f 7420 6e65 6365 7373 6172 7920  s not necessary 
+00024d70: 746f 2073 656e 6420 6120 6e6f 7469 6669  to send a notifi
+00024d80: 6361 7469 6f6e 2074 6f20 616c 6c20 6368  cation to all ch
+00024d90: 6174 206d 656d 6265 7273 2061 626f 7574  at members about
+00024da0: 2074 6865 206e 6577 2070 696e 6e65 640a   the new pinned.
+00024db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00024dc0: 6d65 7373 6167 652e 204e 6f74 6966 6963  message. Notific
+00024dd0: 6174 696f 6e73 2061 7265 2061 6c77 6179  ations are alway
+00024de0: 7320 6469 7361 626c 6564 2069 6e20 6368  s disabled in ch
+00024df0: 616e 6e65 6c73 2e0a 0a20 2020 2020 2020  annels...       
+00024e00: 2020 2020 2062 6f74 685f 7369 6465 7320       both_sides 
+00024e10: 2860 6062 6f6f 6c60 602c 202a 6f70 7469  (``bool``, *opti
+00024e20: 6f6e 616c 2a29 3a0a 2020 2020 2020 2020  onal*):.        
+00024e30: 2020 2020 2020 2020 5061 7373 2054 7275          Pass Tru
+00024e40: 6520 746f 2070 696e 2074 6865 206d 6573  e to pin the mes
+00024e50: 7361 6765 2066 6f72 2062 6f74 6820 7369  sage for both si
+00024e60: 6465 7320 2879 6f75 2061 6e64 2072 6563  des (you and rec
+00024e70: 6970 6965 6e74 292e 0a20 2020 2020 2020  ipient)..       
+00024e80: 2020 2020 2020 2020 2041 7070 6c69 6361           Applica
+00024e90: 626c 6520 746f 2070 7269 7661 7465 2063  ble to private c
+00024ea0: 6861 7473 206f 6e6c 792e 2044 6566 6175  hats only. Defau
+00024eb0: 6c74 7320 746f 2046 616c 7365 2e0a 0a20  lts to False... 
+00024ec0: 2020 2020 2020 2052 6574 7572 6e73 3a0a         Returns:.
+00024ed0: 2020 2020 2020 2020 2020 2020 3a6f 626a              :obj
+00024ee0: 3a60 7e70 7972 6f67 7261 6d2e 7479 7065  :`~pyrogram.type
+00024ef0: 732e 4d65 7373 6167 6560 3a20 4f6e 2073  s.Message`: On s
+00024f00: 7563 6365 7373 2c20 7468 6520 7365 7276  uccess, the serv
+00024f10: 6963 6520 6d65 7373 6167 6520 6973 2072  ice message is r
+00024f20: 6574 7572 6e65 642e 0a0a 2020 2020 2020  eturned...      
+00024f30: 2020 5261 6973 6573 3a0a 2020 2020 2020    Raises:.      
+00024f40: 2020 2020 2020 5250 4345 7272 6f72 3a20        RPCError: 
+00024f50: 496e 2063 6173 6520 6f66 2061 2054 656c  In case of a Tel
+00024f60: 6567 7261 6d20 5250 4320 6572 726f 722e  egram RPC error.
+00024f70: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00024f80: 2020 2020 2072 6574 7572 6e20 6177 6169       return awai
+00024f90: 7420 7365 6c66 2e5f 636c 6965 6e74 2e70  t self._client.p
+00024fa0: 696e 5f63 6861 745f 6d65 7373 6167 6528  in_chat_message(
+00024fb0: 0a20 2020 2020 2020 2020 2020 2063 6861  .            cha
+00024fc0: 745f 6964 3d73 656c 662e 6368 6174 2e69  t_id=self.chat.i
+00024fd0: 642c 0a20 2020 2020 2020 2020 2020 206d  d,.            m
+00024fe0: 6573 7361 6765 5f69 643d 7365 6c66 2e69  essage_id=self.i
+00024ff0: 642c 0a20 2020 2020 2020 2020 2020 2064  d,.            d
+00025000: 6973 6162 6c65 5f6e 6f74 6966 6963 6174  isable_notificat
+00025010: 696f 6e3d 6469 7361 626c 655f 6e6f 7469  ion=disable_noti
+00025020: 6669 6361 7469 6f6e 2c0a 2020 2020 2020  fication,.      
+00025030: 2020 2020 2020 626f 7468 5f73 6964 6573        both_sides
+00025040: 3d62 6f74 685f 7369 6465 730a 2020 2020  =both_sides.    
+00025050: 2020 2020 290a 0a20 2020 2061 7379 6e63      )..    async
+00025060: 2064 6566 2075 6e70 696e 2873 656c 6629   def unpin(self)
+00025070: 202d 3e20 626f 6f6c 3a0a 2020 2020 2020   -> bool:.      
+00025080: 2020 2222 2242 6f75 6e64 206d 6574 686f    """Bound metho
+00025090: 6420 2a75 6e70 696e 2a20 6f66 203a 6f62  d *unpin* of :ob
+000250a0: 6a3a 607e 7079 726f 6772 616d 2e74 7970  j:`~pyrogram.typ
+000250b0: 6573 2e4d 6573 7361 6765 602e 0a0a 2020  es.Message`...  
+000250c0: 2020 2020 2020 5573 6520 6173 2061 2073        Use as a s
+000250d0: 686f 7274 6375 7420 666f 723a 0a0a 2020  hortcut for:..  
+000250e0: 2020 2020 2020 2e2e 2063 6f64 652d 626c        .. code-bl
+000250f0: 6f63 6b3a 3a20 7079 7468 6f6e 0a0a 2020  ock:: python..  
+00025100: 2020 2020 2020 2020 2020 6177 6169 7420            await 
+00025110: 636c 6965 6e74 2e75 6e70 696e 5f63 6861  client.unpin_cha
+00025120: 745f 6d65 7373 6167 6528 0a20 2020 2020  t_message(.     
+00025130: 2020 2020 2020 2020 2020 2063 6861 745f             chat_
+00025140: 6964 3d6d 6573 7361 6765 2e63 6861 742e  id=message.chat.
+00025150: 6964 2c0a 2020 2020 2020 2020 2020 2020  id,.            
+00025160: 2020 2020 6d65 7373 6167 655f 6964 3d6d      message_id=m
+00025170: 6573 7361 6765 5f69 640a 2020 2020 2020  essage_id.      
+00025180: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
+00025190: 2045 7861 6d70 6c65 3a0a 2020 2020 2020   Example:.      
+000251a0: 2020 2020 2020 2e2e 2063 6f64 652d 626c        .. code-bl
+000251b0: 6f63 6b3a 3a20 7079 7468 6f6e 0a0a 2020  ock:: python..  
+000251c0: 2020 2020 2020 2020 2020 2020 2020 6177                aw
+000251d0: 6169 7420 6d65 7373 6167 652e 756e 7069  ait message.unpi
+000251e0: 6e28 290a 0a20 2020 2020 2020 2052 6574  n()..        Ret
+000251f0: 7572 6e73 3a0a 2020 2020 2020 2020 2020  urns:.          
+00025200: 2020 5472 7565 206f 6e20 7375 6363 6573    True on succes
+00025210: 732e 0a0a 2020 2020 2020 2020 5261 6973  s...        Rais
+00025220: 6573 3a0a 2020 2020 2020 2020 2020 2020  es:.            
+00025230: 5250 4345 7272 6f72 3a20 496e 2063 6173  RPCError: In cas
+00025240: 6520 6f66 2061 2054 656c 6567 7261 6d20  e of a Telegram 
+00025250: 5250 4320 6572 726f 722e 0a20 2020 2020  RPC error..     
+00025260: 2020 2022 2222 0a20 2020 2020 2020 2072     """.        r
+00025270: 6574 7572 6e20 6177 6169 7420 7365 6c66  eturn await self
+00025280: 2e5f 636c 6965 6e74 2e75 6e70 696e 5f63  ._client.unpin_c
+00025290: 6861 745f 6d65 7373 6167 6528 0a20 2020  hat_message(.   
+000252a0: 2020 2020 2020 2020 2063 6861 745f 6964           chat_id
+000252b0: 3d73 656c 662e 6368 6174 2e69 642c 0a20  =self.chat.id,. 
+000252c0: 2020 2020 2020 2020 2020 206d 6573 7361             messa
+000252d0: 6765 5f69 643d 7365 6c66 2e69 640a 2020  ge_id=self.id.  
+000252e0: 2020 2020 2020 290a                            ).
```

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/types/messages_and_media/message_entity.py` & `PyroFork-2.1.5/pyrogram/types/messages_and_media/message_entity.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/types/messages_and_media/message_reactions.py` & `PyroFork-2.1.5/pyrogram/types/messages_and_media/message_reactions.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/types/messages_and_media/photo.py` & `PyroFork-2.1.5/pyrogram/types/messages_and_media/photo.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/types/messages_and_media/poll.py` & `PyroFork-2.1.5/pyrogram/types/messages_and_media/poll.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/types/messages_and_media/poll_option.py` & `PyroFork-2.1.5/pyrogram/types/messages_and_media/poll_option.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/types/messages_and_media/reaction.py` & `PyroFork-2.1.5/pyrogram/types/messages_and_media/reaction.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/types/messages_and_media/sticker.py` & `PyroFork-2.1.5/pyrogram/types/messages_and_media/sticker.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/types/messages_and_media/stripped_thumbnail.py` & `PyroFork-2.1.5/pyrogram/types/messages_and_media/stripped_thumbnail.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/types/messages_and_media/thumbnail.py` & `PyroFork-2.1.5/pyrogram/types/messages_and_media/thumbnail.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/types/messages_and_media/venue.py` & `PyroFork-2.1.5/pyrogram/types/messages_and_media/venue.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/types/messages_and_media/video.py` & `PyroFork-2.1.5/pyrogram/types/messages_and_media/video.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/types/messages_and_media/video_note.py` & `PyroFork-2.1.5/pyrogram/types/messages_and_media/video_note.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/types/messages_and_media/voice.py` & `PyroFork-2.1.5/pyrogram/types/messages_and_media/voice.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/types/messages_and_media/web_app_data.py` & `PyroFork-2.1.5/pyrogram/types/messages_and_media/web_app_data.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/types/messages_and_media/web_page.py` & `PyroFork-2.1.5/pyrogram/types/messages_and_media/web_page.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/types/object.py` & `PyroFork-2.1.5/pyrogram/types/object.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/types/update.py` & `PyroFork-2.1.5/pyrogram/types/update.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/types/user_and_chats/__init__.py` & `PyroFork-2.1.5/pyrogram/types/user_and_chats/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 from .chat_privileges import ChatPrivileges
 from .chat_reactions import ChatReactions
 from .dialog import Dialog
 from .emoji_status import EmojiStatus
 from .invite_link_importer import InviteLinkImporter
 from .restriction import Restriction
 from .user import User
+from .username import Username
 from .forum_topic import ForumTopic
 from .forum_topic_created import ForumTopicCreated
 from .forum_topic_closed import ForumTopicClosed
 from .forum_topic_reopened import ForumTopicReopened
 from .forum_topic_edited import ForumTopicEdited
 from .general_forum_topic_hidden import GeneralTopicHidden
 from .general_forum_topic_unhidden import GeneralTopicUnhidden
@@ -54,14 +55,15 @@
     "Chat",
     "ChatMember",
     "ChatPermissions",
     "ChatPhoto",
     "ChatPreview",
     "Dialog",
     "User",
+    "Username",
     "Restriction",
     "ChatEvent",
     "ChatEventFilter",
     "ChatInviteLink",
     "InviteLinkImporter",
     "ChatAdminWithInviteLinks",
     "ForumTopic",
```

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/types/user_and_chats/chat.py` & `PyroFork-2.1.5/pyrogram/types/user_and_chats/chat.py`

 * *Files 2% similar despite different names*

```diff
@@ -128,14 +128,21 @@
         send_as_chat (:obj:`~pyrogram.types.Chat`, *optional*):
             The default "send_as" chat.
             Returned only in :meth:`~pyrogram.Client.get_chat`.
 
         available_reactions (:obj:`~pyrogram.types.ChatReactions`, *optional*):
             Available reactions in the chat.
             Returned only in :meth:`~pyrogram.Client.get_chat`.
+
+        full_name (``str``, *property*):
+            Full name of the other party in a private chat, for private chats and bots.
+
+        usernames (List of :obj:`~pyrogram.types.Username`, *optional*):
+            List of all chat (fragment) usernames; for private chats, supergroups and channels.
+            Returned only in :meth:`~pyrogram.Client.get_chat`.
     """
 
     def __init__(
         self,
         *,
         client: "pyrogram.Client" = None,
         id: int,
@@ -162,15 +169,16 @@
         can_set_sticker_set: bool = None,
         members_count: int = None,
         restrictions: List["types.Restriction"] = None,
         permissions: "types.ChatPermissions" = None,
         distance: int = None,
         linked_chat: "types.Chat" = None,
         send_as_chat: "types.Chat" = None,
-        available_reactions: Optional["types.ChatReactions"] = None
+        available_reactions: Optional["types.ChatReactions"] = None,
+        usernames: List["types.Username"] = None
     ):
         super().__init__(client)
 
         self.id = id
         self.type = type
         self.is_verified = is_verified
         self.is_restricted = is_restricted
@@ -195,14 +203,19 @@
         self.members_count = members_count
         self.restrictions = restrictions
         self.permissions = permissions
         self.distance = distance
         self.linked_chat = linked_chat
         self.send_as_chat = send_as_chat
         self.available_reactions = available_reactions
+        self.usernames = usernames
+
+    @property
+    def full_name(self) -> str:
+        return " ".join(filter(None, [self.first_name, self.last_name])) or None
 
     @staticmethod
     def _parse_user_chat(client, user: raw.types.User) -> "Chat":
         peer_id = user.id
 
         return Chat(
             id=peer_id,
@@ -220,44 +233,58 @@
             dc_id=getattr(getattr(user, "photo", None), "dc_id", None),
             client=client
         )
 
     @staticmethod
     def _parse_chat_chat(client, chat: raw.types.Chat) -> "Chat":
         peer_id = -chat.id
+        active_usernames = getattr(channel, "usernames", [])
+        usernames = None
+        if len(active_usernames) >= 1:
+            usernames = []
+            for username in active_usernames:
+                usernames.append(types.Username._parse(username))
 
         return Chat(
             id=peer_id,
             type=enums.ChatType.GROUP,
             title=chat.title,
             is_creator=getattr(chat, "creator", None),
             photo=types.ChatPhoto._parse(client, getattr(chat, "photo", None), peer_id, 0),
             permissions=types.ChatPermissions._parse(getattr(chat, "default_banned_rights", None)),
             members_count=getattr(chat, "participants_count", None),
             dc_id=getattr(getattr(chat, "photo", None), "dc_id", None),
             has_protected_content=getattr(chat, "noforwards", None),
+            usernames=usernames,
             client=client
         )
 
     @staticmethod
     def _parse_channel_chat(client, channel: raw.types.Channel) -> "Chat":
         peer_id = utils.get_channel_id(channel.id)
         restriction_reason = getattr(channel, "restriction_reason", [])
+        active_usernames = getattr(channel, "usernames", [])
+        usernames = None
+        if len(active_usernames) >= 1:
+            usernames = []
+            for username in active_usernames:
+                usernames.append(types.Username._parse(username))
 
         return Chat(
             id=peer_id,
             type=enums.ChatType.SUPERGROUP if getattr(channel, "megagroup", None) else enums.ChatType.CHANNEL,
             is_verified=getattr(channel, "verified", None),
             is_restricted=getattr(channel, "restricted", None),
             is_creator=getattr(channel, "creator", None),
             is_scam=getattr(channel, "scam", None),
             is_fake=getattr(channel, "fake", None),
             is_forum=getattr(channel, "forum", None),
             title=channel.title,
             username=getattr(channel, "username", None),
+            usernames=usernames,
             photo=types.ChatPhoto._parse(client, getattr(channel, "photo", None), peer_id,
                                          getattr(channel, "access_hash", 0)),
             restrictions=types.List([types.Restriction._parse(r) for r in restriction_reason]) or None,
             permissions=types.ChatPermissions._parse(getattr(channel, "default_banned_rights", None)),
             members_count=getattr(channel, "participants_count", None),
             dc_id=getattr(getattr(channel, "photo", None), "dc_id", None),
             has_protected_content=getattr(channel, "noforwards", None),
```

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/types/user_and_chats/chat_admin_with_invite_links.py` & `PyroFork-2.1.5/pyrogram/types/user_and_chats/chat_admin_with_invite_links.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/types/user_and_chats/chat_event.py` & `PyroFork-2.1.5/pyrogram/types/user_and_chats/chat_event.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/types/user_and_chats/chat_event_filter.py` & `PyroFork-2.1.5/pyrogram/types/user_and_chats/chat_event_filter.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/types/user_and_chats/chat_invite_link.py` & `PyroFork-2.1.5/pyrogram/types/user_and_chats/chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/types/user_and_chats/chat_join_request.py` & `PyroFork-2.1.5/pyrogram/types/user_and_chats/chat_join_request.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/types/user_and_chats/chat_joined_by_request.py` & `PyroFork-2.1.5/pyrogram/types/user_and_chats/chat_joined_by_request.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/types/user_and_chats/chat_joiner.py` & `PyroFork-2.1.5/pyrogram/types/user_and_chats/chat_joiner.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/types/user_and_chats/chat_member.py` & `PyroFork-2.1.5/pyrogram/types/user_and_chats/chat_member.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/types/user_and_chats/chat_member_updated.py` & `PyroFork-2.1.5/pyrogram/types/user_and_chats/chat_member_updated.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/types/user_and_chats/chat_permissions.py` & `PyroFork-2.1.5/pyrogram/types/user_and_chats/chat_permissions.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/types/user_and_chats/chat_photo.py` & `PyroFork-2.1.5/pyrogram/types/user_and_chats/chat_photo.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/types/user_and_chats/chat_preview.py` & `PyroFork-2.1.5/pyrogram/types/user_and_chats/chat_preview.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/types/user_and_chats/chat_privileges.py` & `PyroFork-2.1.5/pyrogram/types/user_and_chats/chat_privileges.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/types/user_and_chats/chat_reactions.py` & `PyroFork-2.1.5/pyrogram/types/user_and_chats/chat_reactions.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/types/user_and_chats/dialog.py` & `PyroFork-2.1.5/pyrogram/types/user_and_chats/dialog.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/types/user_and_chats/emoji_status.py` & `PyroFork-2.1.5/pyrogram/types/user_and_chats/emoji_status.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/types/user_and_chats/forum_topic.py` & `PyroFork-2.1.5/pyrogram/types/user_and_chats/forum_topic.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/types/user_and_chats/forum_topic_closed.py` & `PyroFork-2.1.5/pyrogram/types/user_and_chats/forum_topic_closed.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/types/user_and_chats/forum_topic_created.py` & `PyroFork-2.1.5/pyrogram/types/user_and_chats/forum_topic_created.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/types/user_and_chats/forum_topic_edited.py` & `PyroFork-2.1.5/pyrogram/types/user_and_chats/forum_topic_edited.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/types/user_and_chats/forum_topic_reopened.py` & `PyroFork-2.1.5/pyrogram/types/user_and_chats/forum_topic_reopened.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/types/user_and_chats/general_forum_topic_hidden.py` & `PyroFork-2.1.5/pyrogram/types/user_and_chats/video_chat_started.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
 from ..object import Object
 
 
-class GeneralTopicHidden(Object):
-    """A service message about a general topic hidden in the chat.
+class VideoChatStarted(Object):
+    """A service message about a voice chat started in the chat.
 
     Currently holds no information.
     """
 
     def __init__(self):
         super().__init__()
```

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/types/user_and_chats/general_forum_topic_unhidden.py` & `PyroFork-2.1.5/pyrogram/types/user_and_chats/peer_user.py`

 * *Files 17% similar despite different names*

```diff
@@ -12,18 +12,35 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
+from pyrogram import raw
 from ..object import Object
 
 
-class GeneralTopicUnhidden(Object):
-    """A service message about a general topic unhidden in the chat.
+class PeerUser(Object):
+    """A PeerUser.
 
-    Currently holds no information.
+
+    Parameters:
+        user_id (``Integer``):
+            Id of the user.
     """
 
-    def __init__(self):
+    def __init__(
+        self, *,
+        user_id: int
+    ):
         super().__init__()
+
+        self.user_id = user_id
+
+    @staticmethod
+    def _parse(action: "raw.types.PeerUser") -> "PeerUser":
+
+
+        return PeerUser(
+            user_id=getattr(action,"user_id", None)
+        )
```

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/types/user_and_chats/invite_link_importer.py` & `PyroFork-2.1.5/pyrogram/types/user_and_chats/invite_link_importer.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/types/user_and_chats/peer_channel.py` & `PyroFork-2.1.5/pyrogram/types/user_and_chats/peer_channel.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/types/user_and_chats/peer_user.py` & `PyroFork-2.1.5/tests/filters/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,35 +12,25 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
-from pyrogram import raw
-from ..object import Object
+class Client:
+    def __init__(self):
+        self.me = User("username")
 
+    async def get_me(self):
+        return self.me
 
-class PeerUser(Object):
-    """A PeerUser.
 
+class User:
+    def __init__(self, username: str = None):
+        self.username = username
 
-    Parameters:
-        user_id (``Integer``):
-            Id of the user.
-    """
 
-    def __init__(
-        self, *,
-        user_id: int
-    ):
-        super().__init__()
-
-        self.user_id = user_id
-
-    @staticmethod
-    def _parse(action: "raw.types.PeerUser") -> "PeerUser":
-
-
-        return PeerUser(
-            user_id=getattr(action,"user_id", None)
-        )
+class Message:
+    def __init__(self, text: str = None, caption: str = None):
+        self.text = text
+        self.caption = caption
+        self.command = None
```

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/types/user_and_chats/restriction.py` & `PyroFork-2.1.5/pyrogram/types/user_and_chats/restriction.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/types/user_and_chats/user.py` & `PyroFork-2.1.5/pyrogram/types/user_and_chats/user.py`

 * *Files 3% similar despite different names*

```diff
@@ -136,14 +136,17 @@
         photo (:obj:`~pyrogram.types.ChatPhoto`, *optional*):
             User's or bot's current profile photo. Suitable for downloads only.
 
         restrictions (List of :obj:`~pyrogram.types.Restriction`, *optional*):
             The list of reasons why this bot might be unavailable to some users.
             This field is available only in case *is_restricted* is True.
 
+        full_name (``str``, *optional*):
+            User's or bot's full name.
+
         mention (``str``, *property*):
             Generate a text mention for this user.
             You can use ``user.mention()`` to mention the user using their first name (styled using html), or
             ``user.mention("another name")`` for a custom name. To choose a different style
             ("html" or "md"/"markdown") use ``user.mention(style="md")``.
     """
 
@@ -200,14 +203,18 @@
         self.emoji_status = emoji_status
         self.dc_id = dc_id
         self.phone_number = phone_number
         self.photo = photo
         self.restrictions = restrictions
 
     @property
+    def full_name(self) -> str:
+        return " ".join(filter(None, [self.first_name, self.last_name])) or None
+
+    @property
     def mention(self):
         return Link(
             f"tg://user?id={self.id}",
             self.first_name or "Deleted Account",
             self._client.parse_mode
         )
```

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/types/user_and_chats/video_chat_ended.py` & `PyroFork-2.1.5/pyrogram/types/user_and_chats/video_chat_ended.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/types/user_and_chats/video_chat_members_invited.py` & `PyroFork-2.1.5/pyrogram/types/user_and_chats/video_chat_members_invited.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/types/user_and_chats/video_chat_scheduled.py` & `PyroFork-2.1.5/pyrogram/types/user_and_chats/video_chat_scheduled.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/pyrogram/utils.py` & `PyroFork-2.1.5/pyrogram/utils.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/setup.py` & `PyroFork-2.1.5/setup.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/tests/__init__.py` & `PyroFork-2.1.5/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/tests/filters/__init__.py` & `PyroFork-2.1.5/pyrogram/types/user_and_chats/username.py`

 * *Files 21% similar despite different names*

```diff
@@ -12,25 +12,47 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
-class Client:
-    def __init__(self):
-        self.me = User("username")
+from pyrogram import raw
+from ..object import Object
 
-    async def get_me(self):
-        return self.me
 
+class Username(Object):
+    """A Username.
+
+
+    Parameters:
+        username (``String``):
+            The channel/user username.
+
+        editable (``bool``, *optional*):
+            Can the username edited.
+
+        active (``bool``, *optional*)
+            Is the username active.
+    """
+
+    def __init__(
+        self, *,
+        username: str,
+        editable: bool = None,
+        active: bool = None
+    ):
+        super().__init__()
 
-class User:
-    def __init__(self, username: str = None):
         self.username = username
+        self.editable = editable
+        self.active = active
+
+    @staticmethod
+    def _parse(action: "raw.types.Username") -> "Username":
 
 
-class Message:
-    def __init__(self, text: str = None, caption: str = None):
-        self.text = text
-        self.caption = caption
-        self.command = None
+        return Username(
+            username=getattr(action,"username", None),
+            editable=getattr(action,"editable", None),
+            active=getattr(action,"active", None)
+        )
```

### Comparing `PyroFork-2.1.4.dev202303203721/tests/filters/test_command.py` & `PyroFork-2.1.5/tests/filters/test_command.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/tests/parser/__init__.py` & `PyroFork-2.1.5/tests/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/tests/parser/test_html.py` & `PyroFork-2.1.5/tests/parser/test_html.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.4.dev202303203721/tests/test_file_id.py` & `PyroFork-2.1.5/tests/test_file_id.py`

 * *Files identical despite different names*

