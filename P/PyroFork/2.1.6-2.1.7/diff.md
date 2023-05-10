# Comparing `tmp/PyroFork-2.1.6.tar.gz` & `tmp/PyroFork-2.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyroFork-2.1.6.tar", last modified: Sat Apr 15 10:26:23 2023, max compression
+gzip compressed data, was "PyroFork-2.1.7.tar", last modified: Wed May 10 12:32:17 2023, max compression
```

## Comparing `PyroFork-2.1.6.tar` & `PyroFork-2.1.7.tar`

### file list

```diff
@@ -1,522 +1,523 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:26:23.687001 PyroFork-2.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-04-15 10:26:08.000000 PyroFork-2.1.6/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-04-15 10:26:08.000000 PyroFork-2.1.6/COPYING.lesser
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-15 10:26:08.000000 PyroFork-2.1.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-04-15 10:26:08.000000 PyroFork-2.1.6/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     3897 2023-04-15 10:26:23.687001 PyroFork-2.1.6/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:26:23.562997 PyroFork-2.1.6/PyroFork.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3897 2023-04-15 10:26:23.000000 PyroFork-2.1.6/PyroFork.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20126 2023-04-15 10:26:23.000000 PyroFork-2.1.6/PyroFork.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 10:26:23.000000 PyroFork-2.1.6/PyroFork.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 10:26:23.000000 PyroFork-2.1.6/PyroFork.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-15 10:26:23.000000 PyroFork-2.1.6/PyroFork.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-15 10:26:23.000000 PyroFork-2.1.6/PyroFork.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-04-15 10:26:08.000000 PyroFork-2.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:26:23.562997 PyroFork-2.1.6/compiler/
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-04-15 10:26:08.000000 PyroFork-2.1.6/compiler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:26:23.562997 PyroFork-2.1.6/compiler/api/
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-04-15 10:26:08.000000 PyroFork-2.1.6/compiler/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22402 2023-04-15 10:26:08.000000 PyroFork-2.1.6/compiler/api/compiler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:26:23.562997 PyroFork-2.1.6/compiler/api/source/
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-04-15 10:26:08.000000 PyroFork-2.1.6/compiler/api/source/auth_key.tl
--rw-r--r--   0 runner    (1001) docker     (123)   166709 2023-04-15 10:26:08.000000 PyroFork-2.1.6/compiler/api/source/main_api.tl
--rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-04-15 10:26:08.000000 PyroFork-2.1.6/compiler/api/source/sys_msgs.tl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:26:23.566998 PyroFork-2.1.6/compiler/api/template/
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-15 10:26:08.000000 PyroFork-2.1.6/compiler/api/template/combinator.txt
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-04-15 10:26:08.000000 PyroFork-2.1.6/compiler/api/template/type.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:26:23.566998 PyroFork-2.1.6/compiler/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-04-15 10:26:08.000000 PyroFork-2.1.6/compiler/docs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20053 2023-04-15 10:26:08.000000 PyroFork-2.1.6/compiler/docs/compiler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:26:23.566998 PyroFork-2.1.6/compiler/docs/template/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-15 10:26:08.000000 PyroFork-2.1.6/compiler/docs/template/page.txt
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 10:26:08.000000 PyroFork-2.1.6/compiler/docs/template/toctree.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:26:23.566998 PyroFork-2.1.6/compiler/errors/
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-04-15 10:26:08.000000 PyroFork-2.1.6/compiler/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4917 2023-04-15 10:26:08.000000 PyroFork-2.1.6/compiler/errors/compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-04-15 10:26:08.000000 PyroFork-2.1.6/compiler/errors/sort.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:26:23.570998 PyroFork-2.1.6/compiler/errors/source/
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-04-15 10:26:08.000000 PyroFork-2.1.6/compiler/errors/source/303_SEE_OTHER.tsv
--rw-r--r--   0 runner    (1001) docker     (123)    22642 2023-04-15 10:26:08.000000 PyroFork-2.1.6/compiler/errors/source/400_BAD_REQUEST.tsv
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-04-15 10:26:08.000000 PyroFork-2.1.6/compiler/errors/source/401_UNAUTHORIZED.tsv
--rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-04-15 10:26:08.000000 PyroFork-2.1.6/compiler/errors/source/403_FORBIDDEN.tsv
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-04-15 10:26:08.000000 PyroFork-2.1.6/compiler/errors/source/406_NOT_ACCEPTABLE.tsv
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-04-15 10:26:08.000000 PyroFork-2.1.6/compiler/errors/source/420_FLOOD.tsv
--rw-r--r--   0 runner    (1001) docker     (123)     4219 2023-04-15 10:26:08.000000 PyroFork-2.1.6/compiler/errors/source/500_INTERNAL_SERVER_ERROR.tsv
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-15 10:26:08.000000 PyroFork-2.1.6/compiler/errors/source/503_SERVICE_UNAVAILABLE.tsv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:26:23.570998 PyroFork-2.1.6/compiler/errors/template/
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-04-15 10:26:08.000000 PyroFork-2.1.6/compiler/errors/template/class.txt
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-15 10:26:08.000000 PyroFork-2.1.6/compiler/errors/template/sub_class.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:26:23.574998 PyroFork-2.1.6/pyrogram/
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40417 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:26:23.574998 PyroFork-2.1.6/pyrogram/connection/
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/connection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/connection/connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:26:23.574998 PyroFork-2.1.6/pyrogram/connection/transport/
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/connection/transport/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:26:23.578998 PyroFork-2.1.6/pyrogram/connection/transport/tcp/
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/connection/transport/tcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4100 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/connection/transport/tcp/tcp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/connection/transport/tcp/tcp_abridged.py
--rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/connection/transport/tcp/tcp_abridged_o.py
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/connection/transport/tcp/tcp_full.py
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/connection/transport/tcp/tcp_intermediate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/connection/transport/tcp/tcp_intermediate_o.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:26:23.578998 PyroFork-2.1.6/pyrogram/crypto/
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/crypto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4013 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/crypto/aes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4767 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/crypto/mtproto.py
--rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/crypto/prime.py
--rw-r--r--   0 runner    (1001) docker     (123)    10791 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/crypto/rsa.py
--rw-r--r--   0 runner    (1001) docker     (123)    10085 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)   208021 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/emoji.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:26:23.582998 PyroFork-2.1.6/pyrogram/enums/
--rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/enums/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/enums/auto_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/enums/chat_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     4520 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/enums/chat_event_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/enums/chat_member_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/enums/chat_members_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/enums/chat_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/enums/message_entity_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/enums/message_media_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/enums/message_service_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/enums/messages_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/enums/next_code_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/enums/parse_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/enums/poll_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/enums/sent_code_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/enums/user_status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:26:23.586998 PyroFork-2.1.6/pyrogram/errors/
--rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/errors/rpc_error.py
--rw-r--r--   0 runner    (1001) docker     (123)    15154 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/file_id.py
--rw-r--r--   0 runner    (1001) docker     (123)    24836 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:26:23.590998 PyroFork-2.1.6/pyrogram/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/handlers/callback_query_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/handlers/chat_join_request_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/handlers/chat_member_updated_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/handlers/chosen_inline_result_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/handlers/deleted_messages_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/handlers/disconnect_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/handlers/edited_message_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/handlers/handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/handlers/inline_query_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/handlers/message_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/handlers/poll_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/handlers/raw_update_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/handlers/user_status_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:26:23.590998 PyroFork-2.1.6/pyrogram/methods/
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:26:23.590998 PyroFork-2.1.6/pyrogram/methods/advanced/
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/advanced/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/advanced/invoke.py
--rw-r--r--   0 runner    (1001) docker     (123)     4560 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/advanced/resolve_peer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8164 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/advanced/save_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:26:23.598998 PyroFork-2.1.6/pyrogram/methods/auth/
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/auth/accept_terms_of_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/auth/check_password.py
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/auth/connect.py
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/auth/disconnect.py
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/auth/get_password_hint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/auth/initialize.py
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/auth/log_out.py
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/auth/recover_password.py
--rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/auth/resend_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/auth/send_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/auth/send_recovery_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/auth/sign_in.py
--rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/auth/sign_in_bot.py
--rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/auth/sign_up.py
--rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/auth/terminate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:26:23.602999 PyroFork-2.1.6/pyrogram/methods/bots/
--rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/bots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/bots/answer_callback_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     4990 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/bots/answer_inline_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/bots/answer_web_app_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/bots/delete_bot_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/bots/get_bot_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/bots/get_bot_default_privileges.py
--rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/bots/get_chat_menu_button.py
--rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/bots/get_game_high_scores.py
--rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/bots/get_inline_bot_results.py
--rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/bots/request_callback_answer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/bots/send_game.py
--rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/bots/send_inline_bot_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/bots/set_bot_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/bots/set_bot_default_privileges.py
--rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/bots/set_chat_menu_button.py
--rw-r--r--   0 runner    (1001) docker     (123)     3946 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/bots/set_game_score.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:26:23.618999 PyroFork-2.1.6/pyrogram/methods/chats/
--rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/chats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/chats/add_chat_members.py
--rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/chats/archive_chats.py
--rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/chats/ban_chat_member.py
--rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/chats/close_forum_topic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/chats/close_general_topic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/chats/create_channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/chats/create_forum_topic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/chats/create_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/chats/create_supergroup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/chats/delete_channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/chats/delete_chat_photo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/chats/delete_forum_topic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/chats/delete_supergroup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/chats/delete_user_history.py
--rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/chats/edit_forum_topic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/chats/edit_general_topic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/chats/get_chat.py
--rw-r--r--   0 runner    (1001) docker     (123)     4032 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/chats/get_chat_event_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/chats/get_chat_member.py
--rw-r--r--   0 runner    (1001) docker     (123)     5282 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/chats/get_chat_members.py
--rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/chats/get_chat_members_count.py
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/chats/get_chat_online_count.py
--rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/chats/get_dialogs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/chats/get_dialogs_count.py
--rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/chats/get_forum_topics.py
--rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/chats/get_forum_topics_by_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/chats/get_nearby_chats.py
--rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/chats/get_send_as_chats.py
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/chats/hide_general_topic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/chats/join_chat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2605 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/chats/leave_chat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/chats/mark_chat_unread.py
--rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/chats/pin_chat_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/chats/promote_chat_member.py
--rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/chats/reopen_forum_topic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/chats/reopen_general_topic.py
--rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/chats/restrict_chat_member.py
--rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/chats/set_administrator_title.py
--rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/chats/set_chat_description.py
--rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/chats/set_chat_permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/chats/set_chat_photo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/chats/set_chat_protected_content.py
--rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/chats/set_chat_title.py
--rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/chats/set_chat_username.py
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/chats/set_send_as_chat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/chats/set_slow_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/chats/unarchive_chats.py
--rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/chats/unban_chat_member.py
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/chats/unhide_general_topic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/chats/unpin_all_chat_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/chats/unpin_chat_message.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:26:23.622999 PyroFork-2.1.6/pyrogram/methods/contacts/
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/contacts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/contacts/add_contact.py
--rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/contacts/delete_contacts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/contacts/get_contacts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/contacts/get_contacts_count.py
--rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/contacts/import_contacts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:26:23.626999 PyroFork-2.1.6/pyrogram/methods/decorators/
--rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/decorators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/decorators/on_callback_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/decorators/on_chat_join_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/decorators/on_chat_member_updated.py
--rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/decorators/on_chosen_inline_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/decorators/on_deleted_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/decorators/on_disconnect.py
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/decorators/on_edited_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/decorators/on_inline_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/decorators/on_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/decorators/on_poll.py
--rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/decorators/on_raw_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/decorators/on_user_status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:26:23.630999 PyroFork-2.1.6/pyrogram/methods/invite_links/
--rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/invite_links/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/invite_links/approve_all_chat_join_requests.py
--rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/invite_links/approve_chat_join_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/invite_links/create_chat_invite_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/invite_links/decline_all_chat_join_requests.py
--rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/invite_links/decline_chat_join_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/invite_links/delete_chat_admin_invite_links.py
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/invite_links/delete_chat_invite_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     3533 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/invite_links/edit_chat_invite_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/invite_links/export_chat_invite_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/invite_links/get_chat_admin_invite_links.py
--rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/invite_links/get_chat_admin_invite_links_count.py
--rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/invite_links/get_chat_admins_with_invite_links.py
--rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/invite_links/get_chat_invite_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/invite_links/get_chat_invite_link_joiners.py
--rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/invite_links/get_chat_invite_link_joiners_count.py
--rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/invite_links/get_chat_join_requests.py
--rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/invite_links/revoke_chat_invite_link.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:26:23.651000 PyroFork-2.1.6/pyrogram/methods/messages/
--rw-r--r--   0 runner    (1001) docker     (123)     3921 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/messages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5963 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/messages/copy_media_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     5423 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/messages/copy_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/messages/delete_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     7530 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/messages/download_media.py
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/messages/edit_inline_caption.py
--rw-r--r--   0 runner    (1001) docker     (123)    10375 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/messages/edit_inline_media.py
--rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/messages/edit_inline_reply_markup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/messages/edit_inline_text.py
--rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/messages/edit_message_caption.py
--rw-r--r--   0 runner    (1001) docker     (123)    13022 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/messages/edit_message_media.py
--rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/messages/edit_message_reply_markup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/messages/edit_message_text.py
--rw-r--r--   0 runner    (1001) docker     (123)     4824 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/messages/forward_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/messages/get_chat_history.py
--rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/messages/get_chat_history_count.py
--rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/messages/get_custom_emoji_stickers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/messages/get_discussion_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/messages/get_discussion_replies.py
--rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/messages/get_discussion_replies_count.py
--rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/messages/get_media_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     4741 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/messages/get_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/messages/inline_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/messages/read_chat_history.py
--rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/messages/retract_vote.py
--rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/messages/search_global.py
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/messages/search_global_count.py
--rw-r--r--   0 runner    (1001) docker     (123)     5349 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/messages/search_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/messages/search_messages_count.py
--rw-r--r--   0 runner    (1001) docker     (123)    12828 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/messages/send_animation.py
--rw-r--r--   0 runner    (1001) docker     (123)    11362 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/messages/send_audio.py
--rw-r--r--   0 runner    (1001) docker     (123)     5723 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/messages/send_cached_media.py
--rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/messages/send_chat_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     5111 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/messages/send_contact.py
--rw-r--r--   0 runner    (1001) docker     (123)     5085 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/messages/send_dice.py
--rw-r--r--   0 runner    (1001) docker     (123)    10712 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/messages/send_document.py
--rw-r--r--   0 runner    (1001) docker     (123)     4820 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/messages/send_location.py
--rw-r--r--   0 runner    (1001) docker     (123)    20821 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/messages/send_media_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     7509 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/messages/send_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     9682 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/messages/send_photo.py
--rw-r--r--   0 runner    (1001) docker     (123)     8315 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/messages/send_poll.py
--rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/messages/send_reaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     8582 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/messages/send_sticker.py
--rw-r--r--   0 runner    (1001) docker     (123)     5641 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/messages/send_venue.py
--rw-r--r--   0 runner    (1001) docker     (123)    12198 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/messages/send_video.py
--rw-r--r--   0 runner    (1001) docker     (123)     9556 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/messages/send_video_note.py
--rw-r--r--   0 runner    (1001) docker     (123)     9672 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/messages/send_voice.py
--rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/messages/stop_poll.py
--rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/messages/stream_media.py
--rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/messages/vote_poll.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:26:23.651000 PyroFork-2.1.6/pyrogram/methods/password/
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/password/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/password/change_cloud_password.py
--rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/password/enable_cloud_password.py
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/password/remove_cloud_password.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:26:23.651000 PyroFork-2.1.6/pyrogram/methods/stickers/
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/stickers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/stickers/add_sticker_to_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/stickers/create_sticker_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/stickers/get_sticker_set.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:26:23.655000 PyroFork-2.1.6/pyrogram/methods/users/
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/users/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/users/block_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/users/delete_profile_photos.py
--rw-r--r--   0 runner    (1001) docker     (123)     4421 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/users/get_chat_photos.py
--rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/users/get_chat_photos_count.py
--rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/users/get_common_chats.py
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/users/get_default_emoji_statuses.py
--rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/users/get_me.py
--rw-r--r--   0 runner    (1001) docker     (123)     2562 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/users/get_users.py
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/users/set_emoji_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/users/set_profile_photo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/users/set_username.py
--rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/users/unblock_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/users/update_profile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:26:23.655000 PyroFork-2.1.6/pyrogram/methods/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/utilities/add_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/utilities/compose.py
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/utilities/export_session_string.py
--rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/utilities/idle.py
--rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/utilities/remove_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/utilities/restart.py
--rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/utilities/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/utilities/start.py
--rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/utilities/stop.py
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/methods/utilities/stop_transmission.py
--rw-r--r--   0 runner    (1001) docker     (123)    61915 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/mime_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:26:23.655000 PyroFork-2.1.6/pyrogram/parser/
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8681 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/parser/html.py
--rw-r--r--   0 runner    (1001) docker     (123)     5770 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/parser/markdown.py
--rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/parser/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/parser/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:26:23.655000 PyroFork-2.1.6/pyrogram/raw/
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/raw/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:26:23.659000 PyroFork-2.1.6/pyrogram/raw/core/
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/raw/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/raw/core/future_salt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/raw/core/future_salts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/raw/core/gzip_packed.py
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/raw/core/list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/raw/core/message.py
--rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/raw/core/msg_container.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:26:23.659000 PyroFork-2.1.6/pyrogram/raw/core/primitives/
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/raw/core/primitives/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/raw/core/primitives/bool.py
--rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/raw/core/primitives/bytes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/raw/core/primitives/double.py
--rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/raw/core/primitives/int.py
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/raw/core/primitives/string.py
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/raw/core/primitives/vector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/raw/core/tl_object.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:26:23.659000 PyroFork-2.1.6/pyrogram/session/
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/session/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10513 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/session/auth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:26:23.659000 PyroFork-2.1.6/pyrogram/session/internals/
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/session/internals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/session/internals/data_center.py
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/session/internals/msg_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/session/internals/msg_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/session/internals/seq_no.py
--rw-r--r--   0 runner    (1001) docker     (123)    12440 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/session/session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:26:23.663000 PyroFork-2.1.6/pyrogram/storage/
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/storage/file_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/storage/memory_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     6382 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/storage/sqlite_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/storage/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/sync.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:26:23.663000 PyroFork-2.1.6/pyrogram/types/
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/types/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:26:23.663000 PyroFork-2.1.6/pyrogram/types/authorization/
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/types/authorization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/types/authorization/sent_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/types/authorization/terms_of_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:26:23.667000 PyroFork-2.1.6/pyrogram/types/bots_and_keyboards/
--rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/types/bots_and_keyboards/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/types/bots_and_keyboards/bot_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/types/bots_and_keyboards/bot_command_scope.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/types/bots_and_keyboards/bot_command_scope_all_chat_administrators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/types/bots_and_keyboards/bot_command_scope_all_group_chats.py
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/types/bots_and_keyboards/bot_command_scope_all_private_chats.py
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/types/bots_and_keyboards/bot_command_scope_chat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_administrators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_member.py
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/types/bots_and_keyboards/bot_command_scope_default.py
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/types/bots_and_keyboards/callback_game.py
--rw-r--r--   0 runner    (1001) docker     (123)    12797 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/types/bots_and_keyboards/callback_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/types/bots_and_keyboards/force_reply.py
--rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/types/bots_and_keyboards/game_high_score.py
--rw-r--r--   0 runner    (1001) docker     (123)     8120 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/types/bots_and_keyboards/inline_keyboard_button.py
--rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/types/bots_and_keyboards/inline_keyboard_markup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3514 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/types/bots_and_keyboards/keyboard_button.py
--rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/types/bots_and_keyboards/login_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/types/bots_and_keyboards/menu_button.py
--rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/types/bots_and_keyboards/menu_button_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/types/bots_and_keyboards/menu_button_default.py
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/types/bots_and_keyboards/menu_button_web_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/types/bots_and_keyboards/reply_keyboard_markup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/types/bots_and_keyboards/reply_keyboard_remove.py
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/types/bots_and_keyboards/sent_web_app_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/types/bots_and_keyboards/web_app_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:26:23.671001 PyroFork-2.1.6/pyrogram/types/inline_mode/
--rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/types/inline_mode/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/types/inline_mode/chosen_inline_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     7298 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/types/inline_mode/inline_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/types/inline_mode/inline_query_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     5782 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/types/inline_mode/inline_query_result_animation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3304 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/types/inline_mode/inline_query_result_article.py
--rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/types/inline_mode/inline_query_result_audio.py
--rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/types/inline_mode/inline_query_result_cached_animation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/types/inline_mode/inline_query_result_cached_audio.py
--rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/types/inline_mode/inline_query_result_cached_document.py
--rw-r--r--   0 runner    (1001) docker     (123)     4312 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/types/inline_mode/inline_query_result_cached_photo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/types/inline_mode/inline_query_result_cached_sticker.py
--rw-r--r--   0 runner    (1001) docker     (123)     4394 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/types/inline_mode/inline_query_result_cached_video.py
--rw-r--r--   0 runner    (1001) docker     (123)     4202 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/types/inline_mode/inline_query_result_cached_voice.py
--rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/types/inline_mode/inline_query_result_contact.py
--rw-r--r--   0 runner    (1001) docker     (123)     5240 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/types/inline_mode/inline_query_result_document.py
--rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/types/inline_mode/inline_query_result_location.py
--rw-r--r--   0 runner    (1001) docker     (123)     5261 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/types/inline_mode/inline_query_result_photo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/types/inline_mode/inline_query_result_venue.py
--rw-r--r--   0 runner    (1001) docker     (123)     5474 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/types/inline_mode/inline_query_result_video.py
--rw-r--r--   0 runner    (1001) docker     (123)     4360 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/types/inline_mode/inline_query_result_voice.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:26:23.671001 PyroFork-2.1.6/pyrogram/types/input_media/
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/types/input_media/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/types/input_media/input_media.py
--rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/types/input_media/input_media_animation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/types/input_media/input_media_audio.py
--rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/types/input_media/input_media_document.py
--rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/types/input_media/input_media_photo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/types/input_media/input_media_video.py
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/types/input_media/input_phone_contact.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:26:23.671001 PyroFork-2.1.6/pyrogram/types/input_message_content/
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/types/input_message_content/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/types/input_message_content/input_message_content.py
--rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/types/input_message_content/input_text_message_content.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/types/list.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:26:23.679001 PyroFork-2.1.6/pyrogram/types/messages_and_media/
--rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/types/messages_and_media/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4044 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/types/messages_and_media/animation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4069 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/types/messages_and_media/audio.py
--rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/types/messages_and_media/contact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/types/messages_and_media/dice.py
--rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/types/messages_and_media/document.py
--rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/types/messages_and_media/game.py
--rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/types/messages_and_media/location.py
--rw-r--r--   0 runner    (1001) docker     (123)   153174 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/types/messages_and_media/message.py
--rw-r--r--   0 runner    (1001) docker     (123)     4352 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/types/messages_and_media/message_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/types/messages_and_media/message_reactions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4309 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/types/messages_and_media/photo.py
--rw-r--r--   0 runner    (1001) docker     (123)     8016 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/types/messages_and_media/poll.py
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/types/messages_and_media/poll_option.py
--rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/types/messages_and_media/reaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     6909 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/types/messages_and_media/sticker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/types/messages_and_media/stickerset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/types/messages_and_media/stripped_thumbnail.py
--rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/types/messages_and_media/thumbnail.py
--rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/types/messages_and_media/venue.py
--rw-r--r--   0 runner    (1001) docker     (123)     4389 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/types/messages_and_media/video.py
--rw-r--r--   0 runner    (1001) docker     (123)     3601 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/types/messages_and_media/video_note.py
--rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/types/messages_and_media/voice.py
--rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/types/messages_and_media/web_app_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     6351 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/types/messages_and_media/web_page.py
--rw-r--r--   0 runner    (1001) docker     (123)     3862 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/types/object.py
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/types/update.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:26:23.683001 PyroFork-2.1.6/pyrogram/types/user_and_chats/
--rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/types/user_and_chats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33966 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/types/user_and_chats/chat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/types/user_and_chats/chat_admin_with_invite_links.py
--rw-r--r--   0 runner    (1001) docker     (123)    22023 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/types/user_and_chats/chat_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     5514 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/types/user_and_chats/chat_event_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4579 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/types/user_and_chats/chat_invite_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/types/user_and_chats/chat_join_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/types/user_and_chats/chat_joined_by_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/types/user_and_chats/chat_joiner.py
--rw-r--r--   0 runner    (1001) docker     (123)     9444 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/types/user_and_chats/chat_member.py
--rw-r--r--   0 runner    (1001) docker     (123)     3674 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/types/user_and_chats/chat_member_updated.py
--rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/types/user_and_chats/chat_permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3967 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/types/user_and_chats/chat_photo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/types/user_and_chats/chat_preview.py
--rw-r--r--   0 runner    (1001) docker     (123)     5300 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/types/user_and_chats/chat_privileges.py
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/types/user_and_chats/chat_reactions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/types/user_and_chats/dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/types/user_and_chats/emoji_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     4970 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/types/user_and_chats/forum_topic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/types/user_and_chats/forum_topic_closed.py
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/types/user_and_chats/forum_topic_created.py
--rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/types/user_and_chats/forum_topic_edited.py
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/types/user_and_chats/forum_topic_reopened.py
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/types/user_and_chats/general_forum_topic_hidden.py
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/types/user_and_chats/general_forum_topic_unhidden.py
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/types/user_and_chats/invite_link_importer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/types/user_and_chats/peer_channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/types/user_and_chats/peer_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/types/user_and_chats/restriction.py
--rw-r--r--   0 runner    (1001) docker     (123)    13658 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/types/user_and_chats/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/types/user_and_chats/username.py
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/types/user_and_chats/video_chat_ended.py
--rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/types/user_and_chats/video_chat_members_invited.py
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/types/user_and_chats/video_chat_scheduled.py
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/types/user_and_chats/video_chat_started.py
--rw-r--r--   0 runner    (1001) docker     (123)    10911 2023-04-15 10:26:08.000000 PyroFork-2.1.6/pyrogram/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-15 10:26:08.000000 PyroFork-2.1.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 10:26:23.687001 PyroFork-2.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3555 2023-04-15 10:26:08.000000 PyroFork-2.1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:26:23.683001 PyroFork-2.1.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-04-15 10:26:08.000000 PyroFork-2.1.6/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:26:23.687001 PyroFork-2.1.6/tests/filters/
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-04-15 10:26:08.000000 PyroFork-2.1.6/tests/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-04-15 10:26:08.000000 PyroFork-2.1.6/tests/filters/test_command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:26:23.687001 PyroFork-2.1.6/tests/parser/
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-04-15 10:26:08.000000 PyroFork-2.1.6/tests/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6264 2023-04-15 10:26:08.000000 PyroFork-2.1.6/tests/parser/test_html.py
--rw-r--r--   0 runner    (1001) docker     (123)     8208 2023-04-15 10:26:08.000000 PyroFork-2.1.6/tests/test_file_id.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:32:17.189087 PyroFork-2.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-05-10 12:31:59.000000 PyroFork-2.1.7/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-05-10 12:31:59.000000 PyroFork-2.1.7/COPYING.lesser
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-10 12:31:59.000000 PyroFork-2.1.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-05-10 12:31:59.000000 PyroFork-2.1.7/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     3897 2023-05-10 12:32:17.185087 PyroFork-2.1.7/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:32:17.125086 PyroFork-2.1.7/PyroFork.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3897 2023-05-10 12:32:17.000000 PyroFork-2.1.7/PyroFork.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20160 2023-05-10 12:32:17.000000 PyroFork-2.1.7/PyroFork.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 12:32:17.000000 PyroFork-2.1.7/PyroFork.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 12:32:16.000000 PyroFork-2.1.7/PyroFork.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-10 12:32:17.000000 PyroFork-2.1.7/PyroFork.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-10 12:32:17.000000 PyroFork-2.1.7/PyroFork.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-05-10 12:31:59.000000 PyroFork-2.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:32:17.125086 PyroFork-2.1.7/compiler/
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-10 12:31:59.000000 PyroFork-2.1.7/compiler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:32:17.125086 PyroFork-2.1.7/compiler/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-10 12:31:59.000000 PyroFork-2.1.7/compiler/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22402 2023-05-10 12:31:59.000000 PyroFork-2.1.7/compiler/api/compiler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:32:17.125086 PyroFork-2.1.7/compiler/api/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-05-10 12:31:59.000000 PyroFork-2.1.7/compiler/api/source/auth_key.tl
+-rw-r--r--   0 runner    (1001) docker     (123)   169763 2023-05-10 12:31:59.000000 PyroFork-2.1.7/compiler/api/source/main_api.tl
+-rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-05-10 12:31:59.000000 PyroFork-2.1.7/compiler/api/source/sys_msgs.tl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:32:17.125086 PyroFork-2.1.7/compiler/api/template/
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-05-10 12:31:59.000000 PyroFork-2.1.7/compiler/api/template/combinator.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-05-10 12:31:59.000000 PyroFork-2.1.7/compiler/api/template/type.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:32:17.125086 PyroFork-2.1.7/compiler/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-10 12:31:59.000000 PyroFork-2.1.7/compiler/docs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20053 2023-05-10 12:31:59.000000 PyroFork-2.1.7/compiler/docs/compiler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:32:17.125086 PyroFork-2.1.7/compiler/docs/template/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-10 12:31:59.000000 PyroFork-2.1.7/compiler/docs/template/page.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-10 12:31:59.000000 PyroFork-2.1.7/compiler/docs/template/toctree.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:32:17.125086 PyroFork-2.1.7/compiler/errors/
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-10 12:31:59.000000 PyroFork-2.1.7/compiler/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4917 2023-05-10 12:31:59.000000 PyroFork-2.1.7/compiler/errors/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-05-10 12:31:59.000000 PyroFork-2.1.7/compiler/errors/sort.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:32:17.129086 PyroFork-2.1.7/compiler/errors/source/
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-05-10 12:31:59.000000 PyroFork-2.1.7/compiler/errors/source/303_SEE_OTHER.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)    22642 2023-05-10 12:31:59.000000 PyroFork-2.1.7/compiler/errors/source/400_BAD_REQUEST.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-10 12:31:59.000000 PyroFork-2.1.7/compiler/errors/source/401_UNAUTHORIZED.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-05-10 12:31:59.000000 PyroFork-2.1.7/compiler/errors/source/403_FORBIDDEN.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-05-10 12:31:59.000000 PyroFork-2.1.7/compiler/errors/source/406_NOT_ACCEPTABLE.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-05-10 12:31:59.000000 PyroFork-2.1.7/compiler/errors/source/420_FLOOD.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)     4219 2023-05-10 12:31:59.000000 PyroFork-2.1.7/compiler/errors/source/500_INTERNAL_SERVER_ERROR.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-10 12:31:59.000000 PyroFork-2.1.7/compiler/errors/source/503_SERVICE_UNAVAILABLE.tsv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:32:17.129086 PyroFork-2.1.7/compiler/errors/template/
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-10 12:31:59.000000 PyroFork-2.1.7/compiler/errors/template/class.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-10 12:31:59.000000 PyroFork-2.1.7/compiler/errors/template/sub_class.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:32:17.129086 PyroFork-2.1.7/pyrogram/
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40779 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:32:17.129086 PyroFork-2.1.7/pyrogram/connection/
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/connection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/connection/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:32:17.129086 PyroFork-2.1.7/pyrogram/connection/transport/
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/connection/transport/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:32:17.133086 PyroFork-2.1.7/pyrogram/connection/transport/tcp/
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/connection/transport/tcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4100 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/connection/transport/tcp/tcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/connection/transport/tcp/tcp_abridged.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/connection/transport/tcp/tcp_abridged_o.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/connection/transport/tcp/tcp_full.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/connection/transport/tcp/tcp_intermediate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/connection/transport/tcp/tcp_intermediate_o.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:32:17.133086 PyroFork-2.1.7/pyrogram/crypto/
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/crypto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4013 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/crypto/aes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4767 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/crypto/mtproto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/crypto/prime.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13437 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/crypto/rsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10085 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)   208021 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/emoji.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:32:17.133086 PyroFork-2.1.7/pyrogram/enums/
+-rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/enums/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/enums/auto_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/enums/chat_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4520 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/enums/chat_event_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/enums/chat_member_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/enums/chat_members_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/enums/chat_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/enums/message_entity_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/enums/message_media_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/enums/message_service_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/enums/messages_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/enums/next_code_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/enums/parse_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/enums/poll_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/enums/sent_code_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/enums/user_status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:32:17.133086 PyroFork-2.1.7/pyrogram/errors/
+-rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/errors/rpc_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15154 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/file_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24836 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:32:17.137086 PyroFork-2.1.7/pyrogram/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/handlers/callback_query_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/handlers/chat_join_request_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/handlers/chat_member_updated_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/handlers/chosen_inline_result_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/handlers/deleted_messages_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/handlers/disconnect_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/handlers/edited_message_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/handlers/handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/handlers/inline_query_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/handlers/message_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/handlers/poll_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/handlers/raw_update_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/handlers/user_status_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:32:17.137086 PyroFork-2.1.7/pyrogram/methods/
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:32:17.137086 PyroFork-2.1.7/pyrogram/methods/advanced/
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/advanced/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/advanced/invoke.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4560 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/advanced/resolve_peer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8164 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/advanced/save_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:32:17.141086 PyroFork-2.1.7/pyrogram/methods/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/auth/accept_terms_of_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/auth/check_password.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/auth/connect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/auth/disconnect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/auth/get_password_hint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/auth/initialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/auth/log_out.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/auth/recover_password.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/auth/resend_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/auth/send_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/auth/send_recovery_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/auth/sign_in.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/auth/sign_in_bot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/auth/sign_up.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/auth/terminate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:32:17.141086 PyroFork-2.1.7/pyrogram/methods/bots/
+-rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/bots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/bots/answer_callback_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4990 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/bots/answer_inline_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/bots/answer_web_app_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/bots/delete_bot_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/bots/get_bot_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/bots/get_bot_default_privileges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/bots/get_chat_menu_button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/bots/get_game_high_scores.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/bots/get_inline_bot_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/bots/request_callback_answer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/bots/send_game.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/bots/send_inline_bot_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/bots/set_bot_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/bots/set_bot_default_privileges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/bots/set_chat_menu_button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3946 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/bots/set_game_score.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:32:17.149086 PyroFork-2.1.7/pyrogram/methods/chats/
+-rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/chats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/chats/add_chat_members.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/chats/archive_chats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/chats/ban_chat_member.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/chats/close_forum_topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/chats/close_general_topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/chats/create_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/chats/create_forum_topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/chats/create_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/chats/create_supergroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/chats/delete_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/chats/delete_chat_photo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/chats/delete_forum_topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/chats/delete_supergroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/chats/delete_user_history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/chats/edit_forum_topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/chats/edit_general_topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/chats/get_chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4032 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/chats/get_chat_event_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/chats/get_chat_member.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5282 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/chats/get_chat_members.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/chats/get_chat_members_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/chats/get_chat_online_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/chats/get_dialogs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/chats/get_dialogs_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/chats/get_forum_topics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/chats/get_forum_topics_by_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/chats/get_nearby_chats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/chats/get_send_as_chats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/chats/hide_general_topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/chats/join_chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2605 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/chats/leave_chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/chats/mark_chat_unread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/chats/pin_chat_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/chats/promote_chat_member.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/chats/reopen_forum_topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/chats/reopen_general_topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/chats/restrict_chat_member.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/chats/set_administrator_title.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/chats/set_chat_description.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/chats/set_chat_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/chats/set_chat_photo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/chats/set_chat_protected_content.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/chats/set_chat_title.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/chats/set_chat_username.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/chats/set_send_as_chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/chats/set_slow_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/chats/unarchive_chats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/chats/unban_chat_member.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/chats/unhide_general_topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/chats/unpin_all_chat_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/chats/unpin_chat_message.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:32:17.149086 PyroFork-2.1.7/pyrogram/methods/contacts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/contacts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/contacts/add_contact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/contacts/delete_contacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/contacts/get_contacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/contacts/get_contacts_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/contacts/import_contacts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:32:17.149086 PyroFork-2.1.7/pyrogram/methods/decorators/
+-rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/decorators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/decorators/on_callback_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/decorators/on_chat_join_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/decorators/on_chat_member_updated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/decorators/on_chosen_inline_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/decorators/on_deleted_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/decorators/on_disconnect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/decorators/on_edited_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/decorators/on_inline_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/decorators/on_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/decorators/on_poll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/decorators/on_raw_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/decorators/on_user_status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:32:17.153087 PyroFork-2.1.7/pyrogram/methods/invite_links/
+-rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/invite_links/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/invite_links/approve_all_chat_join_requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/invite_links/approve_chat_join_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/invite_links/create_chat_invite_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/invite_links/decline_all_chat_join_requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/invite_links/decline_chat_join_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/invite_links/delete_chat_admin_invite_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/invite_links/delete_chat_invite_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3533 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/invite_links/edit_chat_invite_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/invite_links/export_chat_invite_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/invite_links/get_chat_admin_invite_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/invite_links/get_chat_admin_invite_links_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/invite_links/get_chat_admins_with_invite_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/invite_links/get_chat_invite_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/invite_links/get_chat_invite_link_joiners.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/invite_links/get_chat_invite_link_joiners_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/invite_links/get_chat_join_requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/invite_links/revoke_chat_invite_link.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:32:17.161087 PyroFork-2.1.7/pyrogram/methods/messages/
+-rw-r--r--   0 runner    (1001) docker     (123)     3921 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/messages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5963 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/messages/copy_media_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5423 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/messages/copy_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/messages/delete_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7530 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/messages/download_media.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/messages/edit_inline_caption.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10375 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/messages/edit_inline_media.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/messages/edit_inline_reply_markup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/messages/edit_inline_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/messages/edit_message_caption.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13022 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/messages/edit_message_media.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/messages/edit_message_reply_markup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/messages/edit_message_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4824 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/messages/forward_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/messages/get_chat_history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/messages/get_chat_history_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/messages/get_custom_emoji_stickers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/messages/get_discussion_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/messages/get_discussion_replies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/messages/get_discussion_replies_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/messages/get_media_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4741 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/messages/get_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/messages/inline_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/messages/read_chat_history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/messages/retract_vote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/messages/search_global.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/messages/search_global_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5349 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/messages/search_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/messages/search_messages_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12828 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/messages/send_animation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11362 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/messages/send_audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5723 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/messages/send_cached_media.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/messages/send_chat_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5111 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/messages/send_contact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5085 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/messages/send_dice.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10712 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/messages/send_document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4820 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/messages/send_location.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20821 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/messages/send_media_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7509 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/messages/send_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9682 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/messages/send_photo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8315 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/messages/send_poll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/messages/send_reaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8582 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/messages/send_sticker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5641 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/messages/send_venue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12198 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/messages/send_video.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9556 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/messages/send_video_note.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9672 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/messages/send_voice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/messages/stop_poll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/messages/stream_media.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/messages/vote_poll.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:32:17.161087 PyroFork-2.1.7/pyrogram/methods/password/
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/password/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/password/change_cloud_password.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/password/enable_cloud_password.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/password/remove_cloud_password.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:32:17.161087 PyroFork-2.1.7/pyrogram/methods/stickers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/stickers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/stickers/add_sticker_to_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/stickers/create_sticker_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/stickers/get_sticker_set.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:32:17.161087 PyroFork-2.1.7/pyrogram/methods/users/
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/users/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/users/block_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/users/delete_profile_photos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4421 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/users/get_chat_photos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/users/get_chat_photos_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/users/get_common_chats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/users/get_default_emoji_statuses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/users/get_me.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2562 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/users/get_users.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/users/set_emoji_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/users/set_profile_photo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/users/set_username.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/users/unblock_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/users/update_profile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:32:17.165087 PyroFork-2.1.7/pyrogram/methods/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/utilities/add_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/utilities/compose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/utilities/export_session_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/utilities/idle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/utilities/remove_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/utilities/restart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/utilities/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/utilities/start.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/utilities/stop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/methods/utilities/stop_transmission.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61915 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/mime_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:32:17.165087 PyroFork-2.1.7/pyrogram/parser/
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8681 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/parser/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5770 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/parser/markdown.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/parser/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/parser/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:32:17.165087 PyroFork-2.1.7/pyrogram/raw/
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/raw/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:32:17.165087 PyroFork-2.1.7/pyrogram/raw/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/raw/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/raw/core/future_salt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/raw/core/future_salts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/raw/core/gzip_packed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/raw/core/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/raw/core/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/raw/core/msg_container.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:32:17.165087 PyroFork-2.1.7/pyrogram/raw/core/primitives/
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/raw/core/primitives/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/raw/core/primitives/bool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/raw/core/primitives/bytes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/raw/core/primitives/double.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/raw/core/primitives/int.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/raw/core/primitives/string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/raw/core/primitives/vector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/raw/core/tl_object.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:32:17.165087 PyroFork-2.1.7/pyrogram/session/
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/session/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10513 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/session/auth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:32:17.169087 PyroFork-2.1.7/pyrogram/session/internals/
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/session/internals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/session/internals/data_center.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/session/internals/msg_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/session/internals/msg_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/session/internals/seq_no.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12440 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/session/session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:32:17.169087 PyroFork-2.1.7/pyrogram/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/storage/file_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/storage/memory_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5105 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/storage/mongo_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6382 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/storage/sqlite_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/storage/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/sync.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:32:17.169087 PyroFork-2.1.7/pyrogram/types/
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/types/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:32:17.169087 PyroFork-2.1.7/pyrogram/types/authorization/
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/types/authorization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/types/authorization/sent_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/types/authorization/terms_of_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:32:17.173087 PyroFork-2.1.7/pyrogram/types/bots_and_keyboards/
+-rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/types/bots_and_keyboards/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/types/bots_and_keyboards/bot_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/types/bots_and_keyboards/bot_command_scope.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/types/bots_and_keyboards/bot_command_scope_all_chat_administrators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/types/bots_and_keyboards/bot_command_scope_all_group_chats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/types/bots_and_keyboards/bot_command_scope_all_private_chats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/types/bots_and_keyboards/bot_command_scope_chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_administrators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_member.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/types/bots_and_keyboards/bot_command_scope_default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/types/bots_and_keyboards/callback_game.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12797 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/types/bots_and_keyboards/callback_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/types/bots_and_keyboards/force_reply.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/types/bots_and_keyboards/game_high_score.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8120 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/types/bots_and_keyboards/inline_keyboard_button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/types/bots_and_keyboards/inline_keyboard_markup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3514 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/types/bots_and_keyboards/keyboard_button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/types/bots_and_keyboards/login_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/types/bots_and_keyboards/menu_button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/types/bots_and_keyboards/menu_button_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/types/bots_and_keyboards/menu_button_default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/types/bots_and_keyboards/menu_button_web_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/types/bots_and_keyboards/reply_keyboard_markup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/types/bots_and_keyboards/reply_keyboard_remove.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/types/bots_and_keyboards/sent_web_app_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/types/bots_and_keyboards/web_app_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:32:17.177087 PyroFork-2.1.7/pyrogram/types/inline_mode/
+-rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/types/inline_mode/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/types/inline_mode/chosen_inline_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7298 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/types/inline_mode/inline_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/types/inline_mode/inline_query_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5782 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/types/inline_mode/inline_query_result_animation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3304 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/types/inline_mode/inline_query_result_article.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/types/inline_mode/inline_query_result_audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/types/inline_mode/inline_query_result_cached_animation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/types/inline_mode/inline_query_result_cached_audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/types/inline_mode/inline_query_result_cached_document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4312 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/types/inline_mode/inline_query_result_cached_photo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/types/inline_mode/inline_query_result_cached_sticker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4394 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/types/inline_mode/inline_query_result_cached_video.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4202 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/types/inline_mode/inline_query_result_cached_voice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/types/inline_mode/inline_query_result_contact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5240 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/types/inline_mode/inline_query_result_document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/types/inline_mode/inline_query_result_location.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5261 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/types/inline_mode/inline_query_result_photo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/types/inline_mode/inline_query_result_venue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5474 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/types/inline_mode/inline_query_result_video.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4360 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/types/inline_mode/inline_query_result_voice.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:32:17.177087 PyroFork-2.1.7/pyrogram/types/input_media/
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/types/input_media/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/types/input_media/input_media.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/types/input_media/input_media_animation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/types/input_media/input_media_audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/types/input_media/input_media_document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/types/input_media/input_media_photo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/types/input_media/input_media_video.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/types/input_media/input_phone_contact.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:32:17.177087 PyroFork-2.1.7/pyrogram/types/input_message_content/
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/types/input_message_content/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/types/input_message_content/input_message_content.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/types/input_message_content/input_text_message_content.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/types/list.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:32:17.181087 PyroFork-2.1.7/pyrogram/types/messages_and_media/
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/types/messages_and_media/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4044 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/types/messages_and_media/animation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4069 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/types/messages_and_media/audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/types/messages_and_media/contact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/types/messages_and_media/dice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/types/messages_and_media/document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/types/messages_and_media/game.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/types/messages_and_media/location.py
+-rw-r--r--   0 runner    (1001) docker     (123)   153174 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/types/messages_and_media/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4352 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/types/messages_and_media/message_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/types/messages_and_media/message_reactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4309 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/types/messages_and_media/photo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8016 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/types/messages_and_media/poll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/types/messages_and_media/poll_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/types/messages_and_media/reaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6909 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/types/messages_and_media/sticker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/types/messages_and_media/stickerset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/types/messages_and_media/stripped_thumbnail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/types/messages_and_media/thumbnail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/types/messages_and_media/venue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4389 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/types/messages_and_media/video.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3601 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/types/messages_and_media/video_note.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/types/messages_and_media/voice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/types/messages_and_media/web_app_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6351 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/types/messages_and_media/web_page.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3862 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/types/object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/types/update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:32:17.185087 PyroFork-2.1.7/pyrogram/types/user_and_chats/
+-rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/types/user_and_chats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33966 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/types/user_and_chats/chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/types/user_and_chats/chat_admin_with_invite_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22023 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/types/user_and_chats/chat_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5514 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/types/user_and_chats/chat_event_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4579 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/types/user_and_chats/chat_invite_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/types/user_and_chats/chat_join_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/types/user_and_chats/chat_joined_by_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/types/user_and_chats/chat_joiner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9444 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/types/user_and_chats/chat_member.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3674 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/types/user_and_chats/chat_member_updated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/types/user_and_chats/chat_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3967 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/types/user_and_chats/chat_photo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/types/user_and_chats/chat_preview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5300 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/types/user_and_chats/chat_privileges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/types/user_and_chats/chat_reactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/types/user_and_chats/dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/types/user_and_chats/emoji_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4970 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/types/user_and_chats/forum_topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/types/user_and_chats/forum_topic_closed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/types/user_and_chats/forum_topic_created.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/types/user_and_chats/forum_topic_edited.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/types/user_and_chats/forum_topic_reopened.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/types/user_and_chats/general_forum_topic_hidden.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/types/user_and_chats/general_forum_topic_unhidden.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/types/user_and_chats/invite_link_importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/types/user_and_chats/peer_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/types/user_and_chats/peer_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/types/user_and_chats/restriction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13658 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/types/user_and_chats/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/types/user_and_chats/username.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/types/user_and_chats/video_chat_ended.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/types/user_and_chats/video_chat_members_invited.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/types/user_and_chats/video_chat_scheduled.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/types/user_and_chats/video_chat_started.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10911 2023-05-10 12:31:59.000000 PyroFork-2.1.7/pyrogram/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-10 12:31:59.000000 PyroFork-2.1.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 12:32:17.189087 PyroFork-2.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3555 2023-05-10 12:31:59.000000 PyroFork-2.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:32:17.185087 PyroFork-2.1.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-10 12:31:59.000000 PyroFork-2.1.7/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:32:17.185087 PyroFork-2.1.7/tests/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-05-10 12:31:59.000000 PyroFork-2.1.7/tests/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-05-10 12:31:59.000000 PyroFork-2.1.7/tests/filters/test_command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:32:17.185087 PyroFork-2.1.7/tests/parser/
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-10 12:31:59.000000 PyroFork-2.1.7/tests/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6264 2023-05-10 12:31:59.000000 PyroFork-2.1.7/tests/parser/test_html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8208 2023-05-10 12:31:59.000000 PyroFork-2.1.7/tests/test_file_id.py
```

### Comparing `PyroFork-2.1.6/COPYING` & `PyroFork-2.1.7/COPYING`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/COPYING.lesser` & `PyroFork-2.1.7/COPYING.lesser`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/NOTICE` & `PyroFork-2.1.7/NOTICE`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/PKG-INFO` & `PyroFork-2.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyroFork
-Version: 2.1.6
+Version: 2.1.7
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
-Metadata-Version: 2.1 Name: PyroFork Version: 2.1.6 Summary: Elegant, modern
+Metadata-Version: 2.1 Name: PyroFork Version: 2.1.7 Summary: Elegant, modern
 and asynchronous Telegram MTProto API framework in Python for users and bots
 Home-page: https://github.com/Mayuri-Chan/pyrofork Download-URL: https://
 github.com/Mayuri-Chan/pyrofork/releases/latest Author: wulan17 Author-email:
 mayuri@mayuri.my.id License: LGPLv3 Project-URL: Tracker, https://github.com/
 Mayuri-Chan/pyrofork/issues Project-URL: Source, https://github.com/Mayuri-
 Chan/pyrofork Project-URL: Documentation, https://pyrofork.mayuri.my.id
 Keywords: telegram chat messenger mtproto api client library python Classifier:
```

### Comparing `PyroFork-2.1.6/PyroFork.egg-info/PKG-INFO` & `PyroFork-2.1.7/PyroFork.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyroFork
-Version: 2.1.6
+Version: 2.1.7
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
-Metadata-Version: 2.1 Name: PyroFork Version: 2.1.6 Summary: Elegant, modern
+Metadata-Version: 2.1 Name: PyroFork Version: 2.1.7 Summary: Elegant, modern
 and asynchronous Telegram MTProto API framework in Python for users and bots
 Home-page: https://github.com/Mayuri-Chan/pyrofork Download-URL: https://
 github.com/Mayuri-Chan/pyrofork/releases/latest Author: wulan17 Author-email:
 mayuri@mayuri.my.id License: LGPLv3 Project-URL: Tracker, https://github.com/
 Mayuri-Chan/pyrofork/issues Project-URL: Source, https://github.com/Mayuri-
 Chan/pyrofork Project-URL: Documentation, https://pyrofork.mayuri.my.id
 Keywords: telegram chat messenger mtproto api client library python Classifier:
```

### Comparing `PyroFork-2.1.6/PyroFork.egg-info/SOURCES.txt` & `PyroFork-2.1.7/PyroFork.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -331,14 +331,15 @@
 pyrogram/session/internals/data_center.py
 pyrogram/session/internals/msg_factory.py
 pyrogram/session/internals/msg_id.py
 pyrogram/session/internals/seq_no.py
 pyrogram/storage/__init__.py
 pyrogram/storage/file_storage.py
 pyrogram/storage/memory_storage.py
+pyrogram/storage/mongo_storage.py
 pyrogram/storage/sqlite_storage.py
 pyrogram/storage/storage.py
 pyrogram/types/__init__.py
 pyrogram/types/list.py
 pyrogram/types/object.py
 pyrogram/types/update.py
 pyrogram/types/authorization/__init__.py
```

### Comparing `PyroFork-2.1.6/README.md` & `PyroFork-2.1.7/README.md`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/compiler/__init__.py` & `PyroFork-2.1.7/compiler/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/compiler/api/__init__.py` & `PyroFork-2.1.7/compiler/api/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/compiler/api/compiler.py` & `PyroFork-2.1.7/compiler/api/compiler.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/compiler/api/source/auth_key.tl` & `PyroFork-2.1.7/compiler/api/source/auth_key.tl`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/compiler/api/source/main_api.tl` & `PyroFork-2.1.7/compiler/api/source/main_api.tl`

 * *Files 1% similar despite different names*

```diff
@@ -108,15 +108,15 @@
 storage.filePdf#ae1e508d = storage.FileType;
 storage.fileMp3#528a0677 = storage.FileType;
 storage.fileMov#4b09ebbc = storage.FileType;
 storage.fileMp4#b3cea0e4 = storage.FileType;
 storage.fileWebp#1081464c = storage.FileType;
 
 userEmpty#d3bc4b7a id:long = User;
-user#8f97c628 flags:# self:flags.10?true contact:flags.11?true mutual_contact:flags.12?true deleted:flags.13?true bot:flags.14?true bot_chat_history:flags.15?true bot_nochats:flags.16?true verified:flags.17?true restricted:flags.18?true min:flags.20?true bot_inline_geo:flags.21?true support:flags.23?true scam:flags.24?true apply_min_photo:flags.25?true fake:flags.26?true bot_attach_menu:flags.27?true premium:flags.28?true attach_menu_enabled:flags.29?true flags2:# id:long access_hash:flags.0?long first_name:flags.1?string last_name:flags.2?string username:flags.3?string phone:flags.4?string photo:flags.5?UserProfilePhoto status:flags.6?UserStatus bot_info_version:flags.14?int restriction_reason:flags.18?Vector<RestrictionReason> bot_inline_placeholder:flags.19?string lang_code:flags.22?string emoji_status:flags.30?EmojiStatus usernames:flags2.0?Vector<Username> = User;
+user#8f97c628 flags:# self:flags.10?true contact:flags.11?true mutual_contact:flags.12?true deleted:flags.13?true bot:flags.14?true bot_chat_history:flags.15?true bot_nochats:flags.16?true verified:flags.17?true restricted:flags.18?true min:flags.20?true bot_inline_geo:flags.21?true support:flags.23?true scam:flags.24?true apply_min_photo:flags.25?true fake:flags.26?true bot_attach_menu:flags.27?true premium:flags.28?true attach_menu_enabled:flags.29?true flags2:# bot_can_edit:flags2.1?true id:long access_hash:flags.0?long first_name:flags.1?string last_name:flags.2?string username:flags.3?string phone:flags.4?string photo:flags.5?UserProfilePhoto status:flags.6?UserStatus bot_info_version:flags.14?int restriction_reason:flags.18?Vector<RestrictionReason> bot_inline_placeholder:flags.19?string lang_code:flags.22?string emoji_status:flags.30?EmojiStatus usernames:flags2.0?Vector<Username> = User;
 
 userProfilePhotoEmpty#4f11bae1 = UserProfilePhoto;
 userProfilePhoto#82d1f706 flags:# has_video:flags.0?true personal:flags.2?true photo_id:long stripped_thumb:flags.1?bytes dc_id:int = UserProfilePhoto;
 
 userStatusEmpty#9d05049 = UserStatus;
 userStatusOnline#edb93949 expires:int = UserStatus;
 userStatusOffline#8c703f was_online:int = UserStatus;
@@ -189,19 +189,21 @@
 messageActionInviteToGroupCall#502f92f7 call:InputGroupCall users:Vector<long> = MessageAction;
 messageActionSetMessagesTTL#3c134d7b flags:# period:int auto_setting_from:flags.0?long = MessageAction;
 messageActionGroupCallScheduled#b3a07661 call:InputGroupCall schedule_date:int = MessageAction;
 messageActionSetChatTheme#aa786345 emoticon:string = MessageAction;
 messageActionChatJoinedByRequest#ebbca3cb = MessageAction;
 messageActionWebViewDataSentMe#47dd8079 text:string data:string = MessageAction;
 messageActionWebViewDataSent#b4c38cb5 text:string = MessageAction;
-messageActionGiftPremium#c83d6aec flags:# currency:string amount:long months:int cryptoCurrency:flags.0?string cryptoAmount:flags.0?long = MessageAction;
+messageActionGiftPremium#c83d6aec flags:# currency:string amount:long months:int crypto_currency:flags.0?string crypto_amount:flags.0?long = MessageAction;
 messageActionTopicCreate#d999256 flags:# title:string icon_color:int icon_emoji_id:flags.0?long = MessageAction;
 messageActionTopicEdit#c0944820 flags:# title:flags.0?string icon_emoji_id:flags.1?long closed:flags.2?Bool hidden:flags.3?Bool = MessageAction;
 messageActionSuggestProfilePhoto#57de635e photo:Photo = MessageAction;
 messageActionRequestedPeer#fe77345d button_id:int peer:Peer = MessageAction;
+messageActionSetChatWallPaper#bc44a927 wallpaper:WallPaper = MessageAction;
+messageActionSetSameChatWallPaper#c0787d6d wallpaper:WallPaper = MessageAction;
 
 dialog#d58a08c6 flags:# pinned:flags.2?true unread_mark:flags.3?true peer:Peer top_message:int read_inbox_max_id:int read_outbox_max_id:int unread_count:int unread_mentions_count:int unread_reactions_count:int notify_settings:PeerNotifySettings pts:flags.0?int draft:flags.1?DraftMessage folder_id:flags.4?int ttl_period:flags.5?int = Dialog;
 dialogFolder#71bd134c flags:# pinned:flags.2?true folder:Folder peer:Peer top_message:int unread_muted_peers_count:int unread_unmuted_peers_count:int unread_muted_messages_count:int unread_unmuted_messages_count:int = Dialog;
 
 photoEmpty#2331b22d id:long = Photo;
 photo#fb197a65 flags:# has_stickers:flags.0?true id:long access_hash:long file_reference:bytes date:int sizes:Vector<PhotoSize> video_sizes:flags.1?Vector<VideoSize> dc_id:int = Photo;
 
@@ -245,15 +247,15 @@
 inputReportReasonOther#c1e4a2b1 = ReportReason;
 inputReportReasonCopyright#9b89f93a = ReportReason;
 inputReportReasonGeoIrrelevant#dbd4feed = ReportReason;
 inputReportReasonFake#f5ddd6e7 = ReportReason;
 inputReportReasonIllegalDrugs#a8eb2be = ReportReason;
 inputReportReasonPersonalDetails#9ec7863d = ReportReason;
 
-userFull#f8d32aed flags:# blocked:flags.0?true phone_calls_available:flags.4?true phone_calls_private:flags.5?true can_pin_message:flags.7?true has_scheduled:flags.12?true video_calls_available:flags.13?true voice_messages_forbidden:flags.20?true translations_disabled:flags.23?true id:long about:flags.1?string settings:PeerSettings personal_photo:flags.21?Photo profile_photo:flags.2?Photo fallback_photo:flags.22?Photo notify_settings:PeerNotifySettings bot_info:flags.3?BotInfo pinned_msg_id:flags.6?int common_chats_count:int folder_id:flags.11?int ttl_period:flags.14?int theme_emoticon:flags.15?string private_forward_name:flags.16?string bot_group_admin_rights:flags.17?ChatAdminRights bot_broadcast_admin_rights:flags.18?ChatAdminRights premium_gifts:flags.19?Vector<PremiumGiftOption> = UserFull;
+userFull#93eadb53 flags:# blocked:flags.0?true phone_calls_available:flags.4?true phone_calls_private:flags.5?true can_pin_message:flags.7?true has_scheduled:flags.12?true video_calls_available:flags.13?true voice_messages_forbidden:flags.20?true translations_disabled:flags.23?true id:long about:flags.1?string settings:PeerSettings personal_photo:flags.21?Photo profile_photo:flags.2?Photo fallback_photo:flags.22?Photo notify_settings:PeerNotifySettings bot_info:flags.3?BotInfo pinned_msg_id:flags.6?int common_chats_count:int folder_id:flags.11?int ttl_period:flags.14?int theme_emoticon:flags.15?string private_forward_name:flags.16?string bot_group_admin_rights:flags.17?ChatAdminRights bot_broadcast_admin_rights:flags.18?ChatAdminRights premium_gifts:flags.19?Vector<PremiumGiftOption> wallpaper:flags.24?WallPaper = UserFull;
 
 contact#145ade0b user_id:long mutual:Bool = Contact;
 
 importedContact#c13e3c50 user_id:long client_id:long = ImportedContact;
 
 contactStatus#16d9703b user_id:long status:UserStatus = ContactStatus;
 
@@ -383,15 +385,15 @@
 updatePinnedMessages#ed85eab5 flags:# pinned:flags.0?true peer:Peer messages:Vector<int> pts:int pts_count:int = Update;
 updatePinnedChannelMessages#5bb98608 flags:# pinned:flags.0?true channel_id:long messages:Vector<int> pts:int pts_count:int = Update;
 updateChat#f89a6a4e chat_id:long = Update;
 updateGroupCallParticipants#f2ebdb4e call:InputGroupCall participants:Vector<GroupCallParticipant> version:int = Update;
 updateGroupCall#14b24500 chat_id:long call:GroupCall = Update;
 updatePeerHistoryTTL#bb9bb9a5 flags:# peer:Peer ttl_period:flags.0?int = Update;
 updateChatParticipant#d087663a flags:# chat_id:long date:int actor_id:long user_id:long prev_participant:flags.0?ChatParticipant new_participant:flags.1?ChatParticipant invite:flags.2?ExportedChatInvite qts:int = Update;
-updateChannelParticipant#985d3abb flags:# channel_id:long date:int actor_id:long user_id:long prev_participant:flags.0?ChannelParticipant new_participant:flags.1?ChannelParticipant invite:flags.2?ExportedChatInvite qts:int = Update;
+updateChannelParticipant#985d3abb flags:# via_chatlist:flags.3?true channel_id:long date:int actor_id:long user_id:long prev_participant:flags.0?ChannelParticipant new_participant:flags.1?ChannelParticipant invite:flags.2?ExportedChatInvite qts:int = Update;
 updateBotStopped#c4870a49 user_id:long date:int stopped:Bool qts:int = Update;
 updateGroupCallConnection#b783982 flags:# presentation:flags.0?true params:DataJSON = Update;
 updateBotCommands#4d712f2e peer:Peer bot_id:long commands:Vector<BotCommand> = Update;
 updatePendingJoinRequests#7063c3db peer:Peer requests_pending:int recent_requesters:Vector<long> = Update;
 updateBotChatInviteRequester#11dfa986 peer:Peer date:int user_id:long about:string invite:ExportedChatInvite qts:int = Update;
 updateMessageReactions#5e1b3cb8 flags:# peer:Peer msg_id:int top_msg_id:flags.0?int reactions:MessageReactions = Update;
 updateAttachMenuBots#17b7a20b = Update;
@@ -613,15 +615,15 @@
 botInfo#8f300b57 flags:# user_id:flags.0?long description:flags.1?string description_photo:flags.4?Photo description_document:flags.5?Document commands:flags.2?Vector<BotCommand> menu_button:flags.3?BotMenuButton = BotInfo;
 
 keyboardButton#a2fa4880 text:string = KeyboardButton;
 keyboardButtonUrl#258aff05 text:string url:string = KeyboardButton;
 keyboardButtonCallback#35bbdb6b flags:# requires_password:flags.0?true text:string data:bytes = KeyboardButton;
 keyboardButtonRequestPhone#b16a6c29 text:string = KeyboardButton;
 keyboardButtonRequestGeoLocation#fc796b3f text:string = KeyboardButton;
-keyboardButtonSwitchInline#568a748 flags:# same_peer:flags.0?true text:string query:string = KeyboardButton;
+keyboardButtonSwitchInline#93b9fbb5 flags:# same_peer:flags.0?true text:string query:string peer_types:flags.1?Vector<InlineQueryPeerType> = KeyboardButton;
 keyboardButtonGame#50f41ccf text:string = KeyboardButton;
 keyboardButtonBuy#afd93fbb text:string = KeyboardButton;
 keyboardButtonUrlAuth#10b78d29 flags:# text:string fwd_text:flags.0?string url:string button_id:int = KeyboardButton;
 inputKeyboardButtonUrlAuth#d02e7fd4 flags:# request_write_access:flags.0?true text:string fwd_text:flags.1?string url:string bot:InputUser = KeyboardButton;
 keyboardButtonRequestPoll#bbc7515d flags:# quiz:flags.0?Bool text:string = KeyboardButton;
 inputKeyboardButtonUserProfile#e988037b text:string user_id:InputUser = KeyboardButton;
 keyboardButtonUserProfile#308660c1 text:string user_id:long = KeyboardButton;
@@ -957,15 +959,15 @@
 channelAdminLogEventActionChangeLocation#e6b76ae prev_value:ChannelLocation new_value:ChannelLocation = ChannelAdminLogEventAction;
 channelAdminLogEventActionToggleSlowMode#53909779 prev_value:int new_value:int = ChannelAdminLogEventAction;
 channelAdminLogEventActionStartGroupCall#23209745 call:InputGroupCall = ChannelAdminLogEventAction;
 channelAdminLogEventActionDiscardGroupCall#db9f9140 call:InputGroupCall = ChannelAdminLogEventAction;
 channelAdminLogEventActionParticipantMute#f92424d2 participant:GroupCallParticipant = ChannelAdminLogEventAction;
 channelAdminLogEventActionParticipantUnmute#e64429c0 participant:GroupCallParticipant = ChannelAdminLogEventAction;
 channelAdminLogEventActionToggleGroupCallSetting#56d6a247 join_muted:Bool = ChannelAdminLogEventAction;
-channelAdminLogEventActionParticipantJoinByInvite#5cdada77 invite:ExportedChatInvite = ChannelAdminLogEventAction;
+channelAdminLogEventActionParticipantJoinByInvite#fe9fc158 flags:# via_chatlist:flags.0?true invite:ExportedChatInvite = ChannelAdminLogEventAction;
 channelAdminLogEventActionExportedInviteDelete#5a50fca4 invite:ExportedChatInvite = ChannelAdminLogEventAction;
 channelAdminLogEventActionExportedInviteRevoke#410a134e invite:ExportedChatInvite = ChannelAdminLogEventAction;
 channelAdminLogEventActionExportedInviteEdit#e90ebb59 prev_invite:ExportedChatInvite new_invite:ExportedChatInvite = ChannelAdminLogEventAction;
 channelAdminLogEventActionParticipantVolume#3e7f6847 participant:GroupCallParticipant = ChannelAdminLogEventAction;
 channelAdminLogEventActionChangeHistoryTTL#6e941a38 prev_value:int new_value:int = ChannelAdminLogEventAction;
 channelAdminLogEventActionParticipantJoinByRequest#afb6144a invite:ExportedChatInvite approved_by:long = ChannelAdminLogEventAction;
 channelAdminLogEventActionToggleNoForwards#cb2ac766 new_value:Bool = ChannelAdminLogEventAction;
@@ -1225,14 +1227,15 @@
 
 bankCardOpenUrl#f568028a url:string name:string = BankCardOpenUrl;
 
 payments.bankCardData#3e24e573 title:string open_urls:Vector<BankCardOpenUrl> = payments.BankCardData;
 
 dialogFilter#7438f7e8 flags:# contacts:flags.0?true non_contacts:flags.1?true groups:flags.2?true broadcasts:flags.3?true bots:flags.4?true exclude_muted:flags.11?true exclude_read:flags.12?true exclude_archived:flags.13?true id:int title:string emoticon:flags.25?string pinned_peers:Vector<InputPeer> include_peers:Vector<InputPeer> exclude_peers:Vector<InputPeer> = DialogFilter;
 dialogFilterDefault#363293ae = DialogFilter;
+dialogFilterChatlist#d64a04a8 flags:# has_my_invites:flags.26?true id:int title:string emoticon:flags.25?string pinned_peers:Vector<InputPeer> include_peers:Vector<InputPeer> = DialogFilter;
 
 dialogFilterSuggested#77744d4a filter:DialogFilter description:string = DialogFilterSuggested;
 
 statsDateRangeDays#b637edaf min_date:int max_date:int = StatsDateRangeDays;
 
 statsAbsValueAndPrev#cb43acde current:double previous:double = StatsAbsValueAndPrev;
 
@@ -1296,22 +1299,23 @@
 phone.groupParticipants#f47751b6 count:int participants:Vector<GroupCallParticipant> next_offset:string chats:Vector<Chat> users:Vector<User> version:int = phone.GroupParticipants;
 
 inlineQueryPeerTypeSameBotPM#3081ed9d = InlineQueryPeerType;
 inlineQueryPeerTypePM#833c0fac = InlineQueryPeerType;
 inlineQueryPeerTypeChat#d766c50a = InlineQueryPeerType;
 inlineQueryPeerTypeMegagroup#5ec4be43 = InlineQueryPeerType;
 inlineQueryPeerTypeBroadcast#6334ee9a = InlineQueryPeerType;
+inlineQueryPeerTypeBotPM#e3b2d0c = InlineQueryPeerType;
 
 messages.historyImport#1662af0b id:long = messages.HistoryImport;
 
 messages.historyImportParsed#5e0fb7b9 flags:# pm:flags.0?true group:flags.1?true title:flags.2?string = messages.HistoryImportParsed;
 
 messages.affectedFoundMessages#ef8d3e6c pts:int pts_count:int offset:int messages:Vector<int> = messages.AffectedFoundMessages;
 
-chatInviteImporter#8c5adfd9 flags:# requested:flags.0?true user_id:long date:int about:flags.2?string approved_by:flags.1?long = ChatInviteImporter;
+chatInviteImporter#8c5adfd9 flags:# requested:flags.0?true via_chatlist:flags.3?true user_id:long date:int about:flags.2?string approved_by:flags.1?long = ChatInviteImporter;
 
 messages.exportedChatInvites#bdc62dcc count:int invites:Vector<ExportedChatInvite> users:Vector<User> = messages.ExportedChatInvites;
 
 messages.exportedChatInvite#1871be50 invite:ExportedChatInvite users:Vector<User> = messages.ExportedChatInvite;
 messages.exportedChatInviteReplaced#222600ef invite:ExportedChatInvite new_invite:ExportedChatInvite users:Vector<User> = messages.ExportedChatInvite;
 
 messages.chatInviteImporters#81b6b00a count:int importers:Vector<ChatInviteImporter> users:Vector<User> = messages.ChatInviteImporters;
@@ -1522,14 +1526,29 @@
 
 appWebViewResultUrl#3c1b4f0d url:string = AppWebViewResult;
 
 inlineBotWebView#b57295d5 text:string url:string = InlineBotWebView;
 
 readParticipantDate#4a4ff172 user_id:long date:int = ReadParticipantDate;
 
+inputChatlistDialogFilter#f3e0da33 filter_id:int = InputChatlist;
+
+exportedChatlistInvite#c5181ac flags:# title:string url:string peers:Vector<Peer> = ExportedChatlistInvite;
+
+chatlists.exportedChatlistInvite#10e6e3a6 filter:DialogFilter invite:ExportedChatlistInvite = chatlists.ExportedChatlistInvite;
+
+chatlists.exportedInvites#10ab6dc7 invites:Vector<ExportedChatlistInvite> chats:Vector<Chat> users:Vector<User> = chatlists.ExportedInvites;
+
+chatlists.chatlistInviteAlready#fa87f659 filter_id:int missing_peers:Vector<Peer> already_peers:Vector<Peer> chats:Vector<Chat> users:Vector<User> = chatlists.ChatlistInvite;
+chatlists.chatlistInvite#1dcd839d flags:# title:string emoticon:flags.0?string peers:Vector<Peer> chats:Vector<Chat> users:Vector<User> = chatlists.ChatlistInvite;
+
+chatlists.chatlistUpdates#93bd878d missing_peers:Vector<Peer> chats:Vector<Chat> users:Vector<User> = chatlists.ChatlistUpdates;
+
+bots.botInfo#e8a775b0 name:string about:string description:string = bots.BotInfo;
+
 ---functions---
 
 invokeAfterMsg#cb9f372d {X:Type} msg_id:long query:!X = X;
 invokeAfterMsgs#3dc4b4f0 {X:Type} msg_ids:Vector<long> query:!X = X;
 initConnection#c1cd5ea9 {X:Type} flags:# api_id:int device_model:string system_version:string app_version:string system_lang_code:string lang_pack:string lang_code:string proxy:flags.0?InputClientProxy params:flags.1?JSONValue query:!X = X;
 invokeWithLayer#da9b0d0d {X:Type} layer:int query:!X = X;
 invokeWithoutUpdates#bf9459b7 {X:Type} query:!X = X;
@@ -1604,15 +1623,15 @@
 account.confirmPasswordEmail#8fdf1920 code:string = Bool;
 account.resendPasswordEmail#7a7f2a15 = Bool;
 account.cancelPasswordEmail#c1cbd5b6 = Bool;
 account.getContactSignUpNotification#9f07c728 = Bool;
 account.setContactSignUpNotification#cff43f61 silent:Bool = Bool;
 account.getNotifyExceptions#53577479 flags:# compare_sound:flags.1?true peer:flags.0?InputNotifyPeer = Updates;
 account.getWallPaper#fc8ddbea wallpaper:InputWallPaper = WallPaper;
-account.uploadWallPaper#dd853661 file:InputFile mime_type:string settings:WallPaperSettings = WallPaper;
+account.uploadWallPaper#e39a8f03 flags:# for_chat:flags.0?true file:InputFile mime_type:string settings:WallPaperSettings = WallPaper;
 account.saveWallPaper#6c5a5b37 wallpaper:InputWallPaper unsave:Bool settings:WallPaperSettings = Bool;
 account.installWallPaper#feed5769 wallpaper:InputWallPaper settings:WallPaperSettings = Bool;
 account.resetWallPapers#bb3b9804 = Bool;
 account.getAutoDownloadSettings#56da0b3f = account.AutoDownloadSettings;
 account.saveAutoDownloadSettings#76f36233 flags:# low:flags.0?true high:flags.1?true settings:AutoDownloadSettings = Bool;
 account.uploadTheme#1c3db333 flags:# file:InputFile thumb:flags.0?InputFile file_name:string mime_type:string = Document;
 account.createTheme#652e4400 flags:# slug:string title:string document:flags.2?InputDocument settings:flags.3?Vector<InputThemeSettings> = Theme;
@@ -1858,21 +1877,22 @@
 messages.getEmojiGroups#7488ce5b hash:int = messages.EmojiGroups;
 messages.getEmojiStatusGroups#2ecd56cd hash:int = messages.EmojiGroups;
 messages.getEmojiProfilePhotoGroups#21a548f3 hash:int = messages.EmojiGroups;
 messages.searchCustomEmoji#2c11c0d7 emoticon:string hash:long = EmojiList;
 messages.togglePeerTranslations#e47cb579 flags:# disabled:flags.0?true peer:InputPeer = Bool;
 messages.getBotApp#34fdc5c3 app:InputBotApp hash:long = messages.BotApp;
 messages.requestAppWebView#8c5a3b3c flags:# write_allowed:flags.0?true peer:InputPeer app:InputBotApp start_param:flags.1?string theme_params:flags.2?DataJSON platform:string = AppWebViewResult;
+messages.setChatWallPaper#8ffacae1 flags:# peer:InputPeer wallpaper:flags.0?InputWallPaper settings:flags.2?WallPaperSettings id:flags.1?int = Updates;
 
 updates.getState#edd4882a = updates.State;
 updates.getDifference#25939651 flags:# pts:int pts_total_limit:flags.0?int date:int qts:int = updates.Difference;
 updates.getChannelDifference#3173d78 flags:# force:flags.0?true channel:InputChannel filter:ChannelMessagesFilter pts:int limit:int = updates.ChannelDifference;
 
-photos.updateProfilePhoto#1c3d5956 flags:# fallback:flags.0?true id:InputPhoto = photos.Photo;
-photos.uploadProfilePhoto#93c9a51 flags:# fallback:flags.3?true file:flags.0?InputFile video:flags.1?InputFile video_start_ts:flags.2?double video_emoji_markup:flags.4?VideoSize = photos.Photo;
+photos.updateProfilePhoto#9e82039 flags:# fallback:flags.0?true bot:flags.1?InputUser id:InputPhoto = photos.Photo;
+photos.uploadProfilePhoto#388a3b5 flags:# fallback:flags.3?true bot:flags.5?InputUser file:flags.0?InputFile video:flags.1?InputFile video_start_ts:flags.2?double video_emoji_markup:flags.4?VideoSize = photos.Photo;
 photos.deletePhotos#87cf7f2f id:Vector<InputPhoto> = Vector<long>;
 photos.getUserPhotos#91cd32a8 user_id:InputUser offset:int max_id:long limit:int = photos.Photos;
 photos.uploadContactProfilePhoto#e14c4a71 flags:# suggest:flags.3?true save:flags.4?true user_id:InputUser file:flags.0?InputFile video:flags.1?InputFile video_start_ts:flags.2?double video_emoji_markup:flags.5?VideoSize = photos.Photo;
 
 upload.saveFilePart#b304a621 file_id:long file_part:int bytes:bytes = Bool;
 upload.getFile#be5335be flags:# precise:flags.0?true cdn_supported:flags.1?true location:InputFileLocation offset:long limit:int = upload.File;
 upload.saveBigFilePart#de7b673d file_id:long file_part:int file_total_parts:int bytes:bytes = Bool;
@@ -1967,16 +1987,18 @@
 bots.setBotCommands#517165a scope:BotCommandScope lang_code:string commands:Vector<BotCommand> = Bool;
 bots.resetBotCommands#3d8de0f9 scope:BotCommandScope lang_code:string = Bool;
 bots.getBotCommands#e34c0dd6 scope:BotCommandScope lang_code:string = Vector<BotCommand>;
 bots.setBotMenuButton#4504d54f user_id:InputUser button:BotMenuButton = Bool;
 bots.getBotMenuButton#9c60eb28 user_id:InputUser = BotMenuButton;
 bots.setBotBroadcastDefaultAdminRights#788464e1 admin_rights:ChatAdminRights = Bool;
 bots.setBotGroupDefaultAdminRights#925ec9ea admin_rights:ChatAdminRights = Bool;
-bots.setBotInfo#a365df7a flags:# lang_code:string about:flags.0?string description:flags.1?string = Bool;
-bots.getBotInfo#75ec12e6 lang_code:string = Vector<string>;
+bots.setBotInfo#10cf3123 flags:# bot:flags.2?InputUser lang_code:string name:flags.3?string about:flags.0?string description:flags.1?string = Bool;
+bots.getBotInfo#dcd914fd flags:# bot:flags.0?InputUser lang_code:string = bots.BotInfo;
+bots.reorderUsernames#9709b1c2 bot:InputUser order:Vector<string> = Bool;
+bots.toggleUsername#53ca973 bot:InputUser username:string active:Bool = Bool;
 
 payments.getPaymentForm#37148dbb flags:# invoice:InputInvoice theme_params:flags.0?DataJSON = payments.PaymentForm;
 payments.getPaymentReceipt#2478d1cc peer:InputPeer msg_id:int = payments.PaymentReceipt;
 payments.validateRequestedInfo#b6c8f12b flags:# save:flags.0?true invoice:InputInvoice info:PaymentRequestedInfo = payments.ValidatedRequestedInfo;
 payments.sendPaymentForm#2d03522f flags:# form_id:long invoice:InputInvoice requested_info_id:flags.0?string shipping_option_id:flags.1?string credentials:InputPaymentCredentials tip_amount:flags.2?long = payments.PaymentResult;
 payments.getSavedInfo#227d824b = payments.SavedInfo;
 payments.clearSavedInfo#d83d70c1 flags:# credentials:flags.0?true info:flags.1?true = Bool;
@@ -2032,16 +2054,27 @@
 langpack.getLangPack#f2f2330a lang_pack:string lang_code:string = LangPackDifference;
 langpack.getStrings#efea3803 lang_pack:string lang_code:string keys:Vector<string> = Vector<LangPackString>;
 langpack.getDifference#cd984aa5 lang_pack:string lang_code:string from_version:int = LangPackDifference;
 langpack.getLanguages#42c6978f lang_pack:string = Vector<LangPackLanguage>;
 langpack.getLanguage#6a596502 lang_pack:string lang_code:string = LangPackLanguage;
 
 folders.editPeerFolders#6847d0ab folder_peers:Vector<InputFolderPeer> = Updates;
-folders.deleteFolder#1c295881 folder_id:int = Updates;
 
 stats.getBroadcastStats#ab42441a flags:# dark:flags.0?true channel:InputChannel = stats.BroadcastStats;
 stats.loadAsyncGraph#621d5fa0 flags:# token:string x:flags.0?long = StatsGraph;
 stats.getMegagroupStats#dcdf8607 flags:# dark:flags.0?true channel:InputChannel = stats.MegagroupStats;
 stats.getMessagePublicForwards#5630281b channel:InputChannel msg_id:int offset_rate:int offset_peer:InputPeer offset_id:int limit:int = messages.Messages;
 stats.getMessageStats#b6e0a3f5 flags:# dark:flags.0?true channel:InputChannel msg_id:int = stats.MessageStats;
 
-// LAYER 157
+chatlists.exportChatlistInvite#8472478e chatlist:InputChatlist title:string peers:Vector<InputPeer> = chatlists.ExportedChatlistInvite;
+chatlists.deleteExportedInvite#719c5c5e chatlist:InputChatlist slug:string = Bool;
+chatlists.editExportedInvite#653db63d flags:# chatlist:InputChatlist slug:string title:flags.1?string peers:flags.2?Vector<InputPeer> = ExportedChatlistInvite;
+chatlists.getExportedInvites#ce03da83 chatlist:InputChatlist = chatlists.ExportedInvites;
+chatlists.checkChatlistInvite#41c10fff slug:string = chatlists.ChatlistInvite;
+chatlists.joinChatlistInvite#a6b1e39a slug:string peers:Vector<InputPeer> = Updates;
+chatlists.getChatlistUpdates#89419521 chatlist:InputChatlist = chatlists.ChatlistUpdates;
+chatlists.joinChatlistUpdates#e089f8f5 chatlist:InputChatlist peers:Vector<InputPeer> = Updates;
+chatlists.hideChatlistUpdates#66e486fb chatlist:InputChatlist = Bool;
+chatlists.getLeaveChatlistSuggestions#fdbcd714 chatlist:InputChatlist = Vector<Peer>;
+chatlists.leaveChatlist#74fae13a chatlist:InputChatlist peers:Vector<InputPeer> = Updates;
+
+// LAYER 158
```

### Comparing `PyroFork-2.1.6/compiler/api/source/sys_msgs.tl` & `PyroFork-2.1.7/compiler/api/source/sys_msgs.tl`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/compiler/api/template/combinator.txt` & `PyroFork-2.1.7/compiler/api/template/combinator.txt`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/compiler/api/template/type.txt` & `PyroFork-2.1.7/compiler/api/template/type.txt`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/compiler/docs/__init__.py` & `PyroFork-2.1.7/compiler/docs/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/compiler/docs/compiler.py` & `PyroFork-2.1.7/compiler/docs/compiler.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/compiler/errors/__init__.py` & `PyroFork-2.1.7/compiler/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/compiler/errors/compiler.py` & `PyroFork-2.1.7/compiler/errors/compiler.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/compiler/errors/sort.py` & `PyroFork-2.1.7/compiler/errors/sort.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/compiler/errors/source/400_BAD_REQUEST.tsv` & `PyroFork-2.1.7/compiler/errors/source/400_BAD_REQUEST.tsv`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/compiler/errors/source/401_UNAUTHORIZED.tsv` & `PyroFork-2.1.7/compiler/errors/source/401_UNAUTHORIZED.tsv`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/compiler/errors/source/403_FORBIDDEN.tsv` & `PyroFork-2.1.7/compiler/errors/source/403_FORBIDDEN.tsv`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/compiler/errors/source/406_NOT_ACCEPTABLE.tsv` & `PyroFork-2.1.7/compiler/errors/source/406_NOT_ACCEPTABLE.tsv`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/compiler/errors/source/500_INTERNAL_SERVER_ERROR.tsv` & `PyroFork-2.1.7/compiler/errors/source/500_INTERNAL_SERVER_ERROR.tsv`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/__init__.py` & `PyroFork-2.1.7/pyrogram/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
 __fork_name__ = "PyroFork"
-__version__ = "2.1.6"
+__version__ = "2.1.7"
 __license__ = "GNU Lesser General Public License v3.0 (LGPL-3.0)"
 __copyright__ = "Copyright (C) 2017-present Dan <https://github.com/delivrance>"
 
 from concurrent.futures.thread import ThreadPoolExecutor
 
 
 class StopTransmission(Exception):
```

### Comparing `PyroFork-2.1.6/pyrogram/client.py` & `PyroFork-2.1.7/pyrogram/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     SessionPasswordNeeded,
     VolumeLocNotFound, ChannelPrivate,
     AuthBytesInvalid, BadRequest
 )
 from pyrogram.handlers.handler import Handler
 from pyrogram.methods import Methods
 from pyrogram.session import Auth, Session
-from pyrogram.storage import FileStorage, MemoryStorage
+from pyrogram.storage import FileStorage, MemoryStorage, MongoStorage
 from pyrogram.types import User, TermsOfService
 from pyrogram.utils import ainput
 from .dispatcher import Dispatcher
 from .file_id import FileId, FileType, ThumbnailSource
 from .mime_types import mime_types
 from .parser import Parser
 from .session.internals import MsgId
@@ -116,14 +116,18 @@
         in_memory (``bool``, *optional*):
             Pass True to start an in-memory session that will be discarded as soon as the client stops.
             In order to reconnect again using an in-memory session without having to login again, you can use
             :meth:`~pyrogram.Client.export_session_string` before stopping the client to get a session string you can
             pass to the ``session_string`` parameter.
             Defaults to False.
 
+        mongodb (``dict``, *optional*):
+            Mongodb config as dict, e.g.: *dict(uri="mongodb://...", db_name="pyrofork-session", remove_peers=False)*.
+            Only applicable for new sessions.
+
         phone_number (``str``, *optional*):
             Pass the phone number as string (with the Country Code prefix included) to avoid entering it manually.
             Only applicable for new sessions.
 
         phone_code (``str``, *optional*):
             Pass the phone code as string (for test numbers only) to avoid entering it manually.
             Only applicable for new sessions.
@@ -199,14 +203,15 @@
         lang_code: str = LANG_CODE,
         ipv6: bool = False,
         proxy: dict = None,
         test_mode: bool = False,
         bot_token: str = None,
         session_string: str = None,
         in_memory: bool = None,
+        mongodb: dict = None,
         phone_number: str = None,
         phone_code: str = None,
         password: str = None,
         workers: int = WORKERS,
         workdir: str = WORKDIR,
         plugins: dict = None,
         parse_mode: "enums.ParseMode" = enums.ParseMode.DEFAULT,
@@ -226,14 +231,15 @@
         self.lang_code = lang_code
         self.ipv6 = ipv6
         self.proxy = proxy
         self.test_mode = test_mode
         self.bot_token = bot_token
         self.session_string = session_string
         self.in_memory = in_memory
+        self.mongodb = mongodb
         self.phone_number = phone_number
         self.phone_code = phone_code
         self.password = password
         self.workers = workers
         self.workdir = Path(workdir)
         self.plugins = plugins
         self.parse_mode = parse_mode
@@ -244,14 +250,16 @@
 
         self.executor = ThreadPoolExecutor(self.workers, thread_name_prefix="Handler")
 
         if self.session_string:
             self.storage = MemoryStorage(self.name, self.session_string)
         elif self.in_memory:
             self.storage = MemoryStorage(self.name)
+        elif self.mongodb:
+            self.storage = MongoStorage(self.mongodb)
         else:
             self.storage = FileStorage(self.name, self.workdir)
 
         self.dispatcher = Dispatcher(self)
 
         self.rnd_id = MsgId
```

### Comparing `PyroFork-2.1.6/pyrogram/connection/__init__.py` & `PyroFork-2.1.7/pyrogram/connection/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/connection/connection.py` & `PyroFork-2.1.7/pyrogram/connection/connection.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/connection/transport/__init__.py` & `PyroFork-2.1.7/pyrogram/connection/transport/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/connection/transport/tcp/__init__.py` & `PyroFork-2.1.7/pyrogram/connection/transport/tcp/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/connection/transport/tcp/tcp.py` & `PyroFork-2.1.7/pyrogram/connection/transport/tcp/tcp.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/connection/transport/tcp/tcp_abridged.py` & `PyroFork-2.1.7/pyrogram/connection/transport/tcp/tcp_abridged.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/connection/transport/tcp/tcp_abridged_o.py` & `PyroFork-2.1.7/pyrogram/connection/transport/tcp/tcp_abridged_o.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/connection/transport/tcp/tcp_full.py` & `PyroFork-2.1.7/pyrogram/connection/transport/tcp/tcp_full.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/connection/transport/tcp/tcp_intermediate.py` & `PyroFork-2.1.7/pyrogram/connection/transport/tcp/tcp_intermediate.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/connection/transport/tcp/tcp_intermediate_o.py` & `PyroFork-2.1.7/pyrogram/connection/transport/tcp/tcp_intermediate_o.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/crypto/__init__.py` & `PyroFork-2.1.7/pyrogram/crypto/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/crypto/aes.py` & `PyroFork-2.1.7/pyrogram/crypto/aes.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/crypto/mtproto.py` & `PyroFork-2.1.7/pyrogram/crypto/mtproto.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/crypto/prime.py` & `PyroFork-2.1.7/pyrogram/crypto/prime.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/crypto/rsa.py` & `PyroFork-2.1.7/pyrogram/crypto/rsa.py`

 * *Files 17% similar despite different names*

```diff
@@ -149,33 +149,33 @@
             "8DC102A9C9B4C95EFFD9DD2DFE96C29BE647D6C69D66CA500843CFAED6E44019"
             "6F1DBE0E2E22163C61CA48C79116FA77216726749A976A1C4B0944B5121E8C01",
             16
         ),  # Modulus
         int("010001", 16)  # Exponent
     ),
 
-    # 6427105915145367799
-    0x15931aac70e0d30f7 - (1 << 64): PublicKey(  # CDN DC-121
+    # -7395192255793472640
+    0x995effd323b5db80 - (1 << 64): PublicKey(  # CDN DC-121
         # -----BEGIN RSA PUBLIC KEY-----
-        # MIIBCgKCAQEA+Lf3PvgE1yxbJUCMaEAkV0QySTVpnaDjiednB5RbtNWjCeqSVakY
-        # HbqqGMIIv5WCGdFdrqOfMNcNSstPtSU6R9UmRw6tquOIykpSuUOje9H+4XVIKquj
-        # yL2ISdK+4ZOMl4hCMkqauw4bP1Sbr03vZRQbU6qEA04V4j879BAyBVhr3WG9+Zi+
-        # t5XfGSTgSExPYEl8rZNHYNV5RB+BuroVH2HLTOpT/mJVfikYpgjfWF5ldezV4Wo9
-        # LSH0cZGSFIaeJl8d0A8Eiy5B9gtBO8mL+XfQRKOOmr7a4BM4Ro2de5rr2i2od7hY
-        # Xd3DO9FRSl4y1zA8Am48Rfd95WHF3N/OmQIDAQAB
+        # MIIBCgKCAQEA4tWHcGJlElkxuxKQJwFjJaulmVHgdxNA3wgI2E8XbNnA88y51Xog
+        # V5m8BEYuTSP4llXZY4ZSJW5VlFXnmsJT/hmjyeFqqTajyAW6nb9vwZX291QvqD/1
+        # ZCFBy7TLvCM0lbNIEhcLMf33ZV8AetLAd+uRLF6QHosys5w0iJ7x+UbGwDxyfeic
+        # 8EJJnsKaXrUOwRycMRN+V/zDySa0EYl1u1EB1MDX1/jIV1IQEbLvdBH4vsVTVEdW
+        # KHlzOcFzT9qX/g8XibCPiHLJvqQb8hVibvs9NaANyClcBEt3mOucG1/46Lilkc/K
+        # d4nlCcohk0jIHNp8symUzNWRPUGmTs3SPwIDAQAB
         # -----END RSA PUBLIC KEY-----
         int(
-            "F8B7F73EF804D72C5B25408C6840245744324935699DA0E389E76707945BB4D5"
-            "A309EA9255A9181DBAAA18C208BF958219D15DAEA39F30D70D4ACB4FB5253A47"
-            "D526470EADAAE388CA4A52B943A37BD1FEE175482AABA3C8BD8849D2BEE1938C"
-            "978842324A9ABB0E1B3F549BAF4DEF65141B53AA84034E15E23F3BF410320558"
-            "6BDD61BDF998BEB795DF1924E0484C4F60497CAD934760D579441F81BABA151F"
-            "61CB4CEA53FE62557E2918A608DF585E6575ECD5E16A3D2D21F471919214869E"
-            "265F1DD00F048B2E41F60B413BC98BF977D044A38E9ABEDAE01338468D9D7B9A"
-            "EBDA2DA877B8585DDDC33BD1514A5E32D7303C026E3C45F77DE561C5DCDFCE99",
+            "E2D587706265125931BB129027016325ABA59951E0771340DF0808D84F176CD9"
+            "C0F3CCB9D57A205799BC04462E4D23F89655D9638652256E559455E79AC253FE"
+            "19A3C9E16AA936A3C805BA9DBF6FC195F6F7542FA83FF5642141CBB4CBBC2334"
+            "95B34812170B31FDF7655F007AD2C077EB912C5E901E8B32B39C34889EF1F946"
+            "C6C03C727DE89CF042499EC29A5EB50EC11C9C31137E57FCC3C926B4118975BB"
+            "5101D4C0D7D7F8C857521011B2EF7411F8BEC55354475628797339C1734FDA97"
+            "FE0F1789B08F8872C9BEA41BF215626EFB3D35A00DC8295C044B7798EB9C1B5F"
+            "F8E8B8A591CFCA7789E509CA219348C81CDA7CB32994CCD5913D41A64ECDD23F",
             16
         ),  # Modulus
         int("010001", 16)  # Exponent
     ),
 
     # 2685959930972952888
     0x1254672538e935938 - (1 << 64): PublicKey(  # CDN DC-140
@@ -195,14 +195,62 @@
             "D53ADD087A68AE5114A9AA5450D8595CC876A161435CBDB2026F8FBF00FEDCA0"
             "A067E9C079172CCCECC09C2B16C428EC776373149DB66AAB9A4DEBF7916B391E"
             "832AE5A7892E27DE0AB1B4451C55F90F1F2ECE3ACEF708BC2C5EE022066EE434"
             "4C7268D724AABAAC667667D727AC3F2956ED4BDAF7089DDE0AEB18A6652DA16F",
             16
         ),  # Modulus
         int("010001", 16)  # Exponent
+    ),
+
+    # -3997872768018684475
+    0xc884b3e62d09e5c5 - (1 << 64): PublicKey(  # CDN DC-201
+        # -----BEGIN RSA PUBLIC KEY-----
+        # MIIBCgKCAQEAug6fETVb7NkXYYu5ueZuM0pqw1heuqUrZNYomQN0lS0o7i6mAWwb
+        # 1/FiscFK+y4LQSSEx+oUzXAhjmll9fmb4e7PbUiXo8MuXO0Rj3e5416DXfTiOYGW
+        # XlFRV0aQzu8agy1epKwkFDidnmy7g5rJJV0q1+3eR+Jk2OEc/B6lMAOv3fBU6xhE
+        # ZByN9gqc6fvkNo13PQ8JYZUSGttzLlYy76uFmvFBhRsJU+LNQ2+bsTHwafSffVYl
+        # Z2boJOblvqbRWe453CzssaSWywGXOQmWvVbEe7F8q1ki/s7S8BxYWrhSLJ6bsu9V
+        # ZWnIHD9vB34QF8IABPRE93mhCOHBqJxSBQIDAQAB
+        # -----END RSA PUBLIC KEY-----
+        int(
+            "BA0E9F11355BECD917618BB9B9E66E334A6AC3585EBAA52B64D628990374952D"
+            "28EE2EA6016C1BD7F162B1C14AFB2E0B412484C7EA14CD70218E6965F5F99BE1"
+            "EECF6D4897A3C32E5CED118F77B9E35E835DF4E23981965E5151574690CEEF1A"
+            "832D5EA4AC2414389D9E6CBB839AC9255D2AD7EDDE47E264D8E11CFC1EA53003"
+            "AFDDF054EB1844641C8DF60A9CE9FBE4368D773D0F096195121ADB732E5632EF"
+            "AB859AF141851B0953E2CD436F9BB131F069F49F7D56256766E824E6E5BEA6D1"
+            "59EE39DC2CECB1A496CB0197390996BD56C47BB17CAB5922FECED2F01C585AB8"
+            "522C9E9BB2EF556569C81C3F6F077E1017C20004F444F779A108E1C1A89C5205",
+            16
+        ),  # Modulus
+        int("010001", 16)  # Exponent
+    ),
+
+    # -4960899639492471258
+    0xbb27580fd5b01626 - (1 << 64): PublicKey(  # CDN DC-203
+        # -----BEGIN RSA PUBLIC KEY-----
+        # MIIBCgKCAQEAv/L6td+mj7Dl81NHfu+Xf1KNtvZPR1tS5xFqkiUson1u7D2ulK05
+        # jM8HKvpV1o+1HPPqhaXhasvsX90u3TIHRQ0zuJKJxKAiZo3GK7phHozjAJ9VUFbO
+        # 7jKAa5BTE9tXgA5ZwJAiQWb3U6ykwRzk3fFRe5WaW7xfVUiepxyWGdr1eecoWCfB
+        # af1TCXfcS7vcyljNT03pwt2YyS5iXE5IB5wBB5yqSSm4GYtWWR67UjIsXBd77TRp
+        # foLGpfOdUHxBz4ZSj8D76m1zlpID5J2pF6bH4+ZCz0SUpv3j7bE8WFlvgMfwEPhw
+        # xMYidRGayq9YlLlYd4D+Yoq0U6jS3MWTRQIDAQAB
+        # -----END RSA PUBLIC KEY-----
+        int(
+            "BFF2FAB5DFA68FB0E5F353477EEF977F528DB6F64F475B52E7116A92252CA27D"
+            "6EEC3DAE94AD398CCF072AFA55D68FB51CF3EA85A5E16ACBEC5FDD2EDD320745"
+            "0D33B89289C4A022668DC62BBA611E8CE3009F555056CEEE32806B905313DB57"
+            "800E59C090224166F753ACA4C11CE4DDF1517B959A5BBC5F55489EA71C9619DA"
+            "F579E7285827C169FD530977DC4BBBDCCA58CD4F4DE9C2DD98C92E625C4E4807"
+            "9C01079CAA4929B8198B56591EBB52322C5C177BED34697E82C6A5F39D507C41"
+            "CF86528FC0FBEA6D73969203E49DA917A6C7E3E642CF4494A6FDE3EDB13C5859"
+            "6F80C7F010F870C4C62275119ACAAF5894B9587780FE628AB453A8D2DCC59345",
+            16
+        ),  # Modulus
+        int("010001", 16)  # Exponent
     )
 }
 
 
 def encrypt(data: bytes, fingerprint: int) -> bytes:
     return pow(
         int.from_bytes(data, "big"),
```

### Comparing `PyroFork-2.1.6/pyrogram/dispatcher.py` & `PyroFork-2.1.7/pyrogram/dispatcher.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/emoji.py` & `PyroFork-2.1.7/pyrogram/emoji.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/enums/__init__.py` & `PyroFork-2.1.7/pyrogram/enums/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/enums/auto_name.py` & `PyroFork-2.1.7/pyrogram/enums/auto_name.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/enums/chat_action.py` & `PyroFork-2.1.7/pyrogram/enums/chat_action.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/enums/chat_event_action.py` & `PyroFork-2.1.7/pyrogram/enums/chat_event_action.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/enums/chat_member_status.py` & `PyroFork-2.1.7/pyrogram/enums/chat_member_status.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/enums/chat_members_filter.py` & `PyroFork-2.1.7/pyrogram/enums/chat_members_filter.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/enums/chat_type.py` & `PyroFork-2.1.7/pyrogram/enums/chat_type.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/enums/message_entity_type.py` & `PyroFork-2.1.7/pyrogram/enums/message_entity_type.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/enums/message_media_type.py` & `PyroFork-2.1.7/pyrogram/enums/message_media_type.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/enums/message_service_type.py` & `PyroFork-2.1.7/pyrogram/enums/message_service_type.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/enums/messages_filter.py` & `PyroFork-2.1.7/pyrogram/enums/messages_filter.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/enums/next_code_type.py` & `PyroFork-2.1.7/pyrogram/enums/next_code_type.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/enums/parse_mode.py` & `PyroFork-2.1.7/pyrogram/enums/parse_mode.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/enums/poll_type.py` & `PyroFork-2.1.7/pyrogram/enums/poll_type.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/enums/sent_code_type.py` & `PyroFork-2.1.7/pyrogram/enums/sent_code_type.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/enums/user_status.py` & `PyroFork-2.1.7/pyrogram/enums/user_status.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/errors/__init__.py` & `PyroFork-2.1.7/pyrogram/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/errors/rpc_error.py` & `PyroFork-2.1.7/pyrogram/errors/rpc_error.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/file_id.py` & `PyroFork-2.1.7/pyrogram/file_id.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/filters.py` & `PyroFork-2.1.7/pyrogram/filters.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/handlers/__init__.py` & `PyroFork-2.1.7/pyrogram/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/handlers/callback_query_handler.py` & `PyroFork-2.1.7/pyrogram/handlers/callback_query_handler.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/handlers/chat_join_request_handler.py` & `PyroFork-2.1.7/pyrogram/handlers/chat_join_request_handler.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/handlers/chat_member_updated_handler.py` & `PyroFork-2.1.7/pyrogram/handlers/chat_member_updated_handler.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/handlers/chosen_inline_result_handler.py` & `PyroFork-2.1.7/pyrogram/handlers/chosen_inline_result_handler.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/handlers/deleted_messages_handler.py` & `PyroFork-2.1.7/pyrogram/handlers/deleted_messages_handler.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/handlers/disconnect_handler.py` & `PyroFork-2.1.7/pyrogram/handlers/disconnect_handler.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/handlers/edited_message_handler.py` & `PyroFork-2.1.7/pyrogram/handlers/edited_message_handler.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/handlers/handler.py` & `PyroFork-2.1.7/pyrogram/handlers/handler.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/handlers/inline_query_handler.py` & `PyroFork-2.1.7/pyrogram/handlers/inline_query_handler.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/handlers/message_handler.py` & `PyroFork-2.1.7/pyrogram/handlers/message_handler.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/handlers/poll_handler.py` & `PyroFork-2.1.7/pyrogram/handlers/poll_handler.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/handlers/raw_update_handler.py` & `PyroFork-2.1.7/pyrogram/handlers/raw_update_handler.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/handlers/user_status_handler.py` & `PyroFork-2.1.7/pyrogram/handlers/user_status_handler.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/__init__.py` & `PyroFork-2.1.7/pyrogram/methods/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/advanced/__init__.py` & `PyroFork-2.1.7/pyrogram/methods/advanced/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/advanced/invoke.py` & `PyroFork-2.1.7/pyrogram/methods/advanced/invoke.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/advanced/resolve_peer.py` & `PyroFork-2.1.7/pyrogram/methods/advanced/resolve_peer.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/advanced/save_file.py` & `PyroFork-2.1.7/pyrogram/methods/advanced/save_file.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/auth/__init__.py` & `PyroFork-2.1.7/pyrogram/methods/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/auth/accept_terms_of_service.py` & `PyroFork-2.1.7/pyrogram/methods/auth/accept_terms_of_service.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/auth/check_password.py` & `PyroFork-2.1.7/pyrogram/methods/auth/check_password.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/auth/connect.py` & `PyroFork-2.1.7/pyrogram/methods/auth/connect.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/auth/disconnect.py` & `PyroFork-2.1.7/pyrogram/methods/auth/disconnect.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/auth/get_password_hint.py` & `PyroFork-2.1.7/pyrogram/methods/auth/get_password_hint.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/auth/initialize.py` & `PyroFork-2.1.7/pyrogram/methods/auth/initialize.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/auth/log_out.py` & `PyroFork-2.1.7/pyrogram/methods/auth/log_out.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/auth/recover_password.py` & `PyroFork-2.1.7/pyrogram/methods/auth/recover_password.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/auth/resend_code.py` & `PyroFork-2.1.7/pyrogram/methods/auth/resend_code.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/auth/send_code.py` & `PyroFork-2.1.7/pyrogram/methods/auth/send_code.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/auth/send_recovery_code.py` & `PyroFork-2.1.7/pyrogram/methods/auth/send_recovery_code.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/auth/sign_in.py` & `PyroFork-2.1.7/pyrogram/methods/auth/sign_in.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/auth/sign_in_bot.py` & `PyroFork-2.1.7/pyrogram/methods/auth/sign_in_bot.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/auth/sign_up.py` & `PyroFork-2.1.7/pyrogram/methods/auth/sign_up.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/auth/terminate.py` & `PyroFork-2.1.7/pyrogram/methods/auth/terminate.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/bots/__init__.py` & `PyroFork-2.1.7/pyrogram/methods/bots/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/bots/answer_callback_query.py` & `PyroFork-2.1.7/pyrogram/methods/bots/answer_callback_query.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/bots/answer_inline_query.py` & `PyroFork-2.1.7/pyrogram/methods/bots/answer_inline_query.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/bots/answer_web_app_query.py` & `PyroFork-2.1.7/pyrogram/methods/bots/answer_web_app_query.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/bots/delete_bot_commands.py` & `PyroFork-2.1.7/pyrogram/methods/bots/delete_bot_commands.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/bots/get_bot_commands.py` & `PyroFork-2.1.7/pyrogram/methods/bots/get_bot_commands.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/bots/get_bot_default_privileges.py` & `PyroFork-2.1.7/pyrogram/methods/bots/get_bot_default_privileges.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/bots/get_chat_menu_button.py` & `PyroFork-2.1.7/pyrogram/methods/bots/get_chat_menu_button.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/bots/get_game_high_scores.py` & `PyroFork-2.1.7/pyrogram/methods/bots/get_game_high_scores.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/bots/get_inline_bot_results.py` & `PyroFork-2.1.7/pyrogram/methods/bots/get_inline_bot_results.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/bots/request_callback_answer.py` & `PyroFork-2.1.7/pyrogram/methods/bots/request_callback_answer.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/bots/send_game.py` & `PyroFork-2.1.7/pyrogram/methods/bots/send_game.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/bots/send_inline_bot_result.py` & `PyroFork-2.1.7/pyrogram/methods/bots/send_inline_bot_result.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/bots/set_bot_commands.py` & `PyroFork-2.1.7/pyrogram/methods/bots/set_bot_commands.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/bots/set_bot_default_privileges.py` & `PyroFork-2.1.7/pyrogram/methods/bots/set_bot_default_privileges.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/bots/set_chat_menu_button.py` & `PyroFork-2.1.7/pyrogram/methods/bots/set_chat_menu_button.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/bots/set_game_score.py` & `PyroFork-2.1.7/pyrogram/methods/bots/set_game_score.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/chats/__init__.py` & `PyroFork-2.1.7/pyrogram/methods/chats/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/chats/add_chat_members.py` & `PyroFork-2.1.7/pyrogram/methods/chats/add_chat_members.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/chats/archive_chats.py` & `PyroFork-2.1.7/pyrogram/methods/chats/archive_chats.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/chats/ban_chat_member.py` & `PyroFork-2.1.7/pyrogram/methods/chats/ban_chat_member.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/chats/close_forum_topic.py` & `PyroFork-2.1.7/pyrogram/methods/chats/close_forum_topic.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/chats/close_general_topic.py` & `PyroFork-2.1.7/pyrogram/methods/chats/close_general_topic.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/chats/create_channel.py` & `PyroFork-2.1.7/pyrogram/methods/chats/create_channel.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/chats/create_forum_topic.py` & `PyroFork-2.1.7/pyrogram/methods/chats/create_forum_topic.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/chats/create_group.py` & `PyroFork-2.1.7/pyrogram/methods/chats/create_group.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/chats/create_supergroup.py` & `PyroFork-2.1.7/pyrogram/methods/chats/create_supergroup.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/chats/delete_channel.py` & `PyroFork-2.1.7/pyrogram/methods/chats/delete_channel.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/chats/delete_chat_photo.py` & `PyroFork-2.1.7/pyrogram/methods/chats/delete_chat_photo.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/chats/delete_forum_topic.py` & `PyroFork-2.1.7/pyrogram/methods/chats/delete_forum_topic.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/chats/delete_supergroup.py` & `PyroFork-2.1.7/pyrogram/methods/chats/delete_supergroup.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/chats/delete_user_history.py` & `PyroFork-2.1.7/pyrogram/methods/chats/delete_user_history.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/chats/edit_forum_topic.py` & `PyroFork-2.1.7/pyrogram/methods/chats/edit_forum_topic.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/chats/edit_general_topic.py` & `PyroFork-2.1.7/pyrogram/methods/chats/edit_general_topic.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/chats/get_chat.py` & `PyroFork-2.1.7/pyrogram/methods/chats/get_chat.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/chats/get_chat_event_log.py` & `PyroFork-2.1.7/pyrogram/methods/chats/get_chat_event_log.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/chats/get_chat_member.py` & `PyroFork-2.1.7/pyrogram/methods/chats/get_chat_member.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/chats/get_chat_members.py` & `PyroFork-2.1.7/pyrogram/methods/chats/get_chat_members.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/chats/get_chat_members_count.py` & `PyroFork-2.1.7/pyrogram/methods/chats/get_chat_members_count.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/chats/get_chat_online_count.py` & `PyroFork-2.1.7/pyrogram/methods/chats/get_chat_online_count.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/chats/get_dialogs.py` & `PyroFork-2.1.7/pyrogram/methods/chats/get_dialogs.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/chats/get_dialogs_count.py` & `PyroFork-2.1.7/pyrogram/methods/chats/get_dialogs_count.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/chats/get_forum_topics.py` & `PyroFork-2.1.7/pyrogram/methods/chats/get_forum_topics.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/chats/get_forum_topics_by_id.py` & `PyroFork-2.1.7/pyrogram/methods/chats/get_forum_topics_by_id.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/chats/get_nearby_chats.py` & `PyroFork-2.1.7/pyrogram/methods/chats/get_nearby_chats.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/chats/get_send_as_chats.py` & `PyroFork-2.1.7/pyrogram/methods/chats/get_send_as_chats.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/chats/hide_general_topic.py` & `PyroFork-2.1.7/pyrogram/methods/chats/hide_general_topic.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/chats/join_chat.py` & `PyroFork-2.1.7/pyrogram/methods/chats/join_chat.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/chats/leave_chat.py` & `PyroFork-2.1.7/pyrogram/methods/chats/leave_chat.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/chats/mark_chat_unread.py` & `PyroFork-2.1.7/pyrogram/methods/chats/mark_chat_unread.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/chats/pin_chat_message.py` & `PyroFork-2.1.7/pyrogram/methods/chats/pin_chat_message.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/chats/promote_chat_member.py` & `PyroFork-2.1.7/pyrogram/methods/chats/promote_chat_member.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/chats/reopen_forum_topic.py` & `PyroFork-2.1.7/pyrogram/methods/chats/reopen_forum_topic.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/chats/reopen_general_topic.py` & `PyroFork-2.1.7/pyrogram/methods/chats/reopen_general_topic.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/chats/restrict_chat_member.py` & `PyroFork-2.1.7/pyrogram/methods/chats/restrict_chat_member.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/chats/set_administrator_title.py` & `PyroFork-2.1.7/pyrogram/methods/chats/set_administrator_title.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/chats/set_chat_description.py` & `PyroFork-2.1.7/pyrogram/methods/chats/set_chat_description.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/chats/set_chat_permissions.py` & `PyroFork-2.1.7/pyrogram/methods/chats/set_chat_permissions.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/chats/set_chat_photo.py` & `PyroFork-2.1.7/pyrogram/methods/chats/set_chat_photo.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/chats/set_chat_protected_content.py` & `PyroFork-2.1.7/pyrogram/methods/chats/set_chat_protected_content.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/chats/set_chat_title.py` & `PyroFork-2.1.7/pyrogram/methods/chats/set_chat_title.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/chats/set_chat_username.py` & `PyroFork-2.1.7/pyrogram/methods/chats/set_chat_username.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/chats/set_send_as_chat.py` & `PyroFork-2.1.7/pyrogram/methods/chats/set_send_as_chat.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/chats/set_slow_mode.py` & `PyroFork-2.1.7/pyrogram/methods/chats/set_slow_mode.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/chats/unarchive_chats.py` & `PyroFork-2.1.7/pyrogram/methods/chats/unarchive_chats.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/chats/unban_chat_member.py` & `PyroFork-2.1.7/pyrogram/methods/chats/unban_chat_member.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/chats/unhide_general_topic.py` & `PyroFork-2.1.7/pyrogram/methods/chats/unhide_general_topic.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/chats/unpin_all_chat_messages.py` & `PyroFork-2.1.7/pyrogram/methods/chats/unpin_all_chat_messages.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/chats/unpin_chat_message.py` & `PyroFork-2.1.7/pyrogram/methods/chats/unpin_chat_message.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/contacts/__init__.py` & `PyroFork-2.1.7/pyrogram/methods/contacts/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/contacts/add_contact.py` & `PyroFork-2.1.7/pyrogram/methods/contacts/add_contact.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/contacts/delete_contacts.py` & `PyroFork-2.1.7/pyrogram/methods/contacts/delete_contacts.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/contacts/get_contacts.py` & `PyroFork-2.1.7/pyrogram/methods/contacts/get_contacts.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/contacts/get_contacts_count.py` & `PyroFork-2.1.7/pyrogram/methods/contacts/get_contacts_count.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/contacts/import_contacts.py` & `PyroFork-2.1.7/pyrogram/methods/contacts/import_contacts.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/decorators/__init__.py` & `PyroFork-2.1.7/pyrogram/methods/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/decorators/on_callback_query.py` & `PyroFork-2.1.7/pyrogram/methods/decorators/on_callback_query.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/decorators/on_chat_join_request.py` & `PyroFork-2.1.7/pyrogram/methods/decorators/on_chat_join_request.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/decorators/on_chat_member_updated.py` & `PyroFork-2.1.7/pyrogram/methods/decorators/on_chat_member_updated.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/decorators/on_chosen_inline_result.py` & `PyroFork-2.1.7/pyrogram/methods/decorators/on_chosen_inline_result.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/decorators/on_deleted_messages.py` & `PyroFork-2.1.7/pyrogram/methods/decorators/on_deleted_messages.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/decorators/on_disconnect.py` & `PyroFork-2.1.7/pyrogram/methods/decorators/on_disconnect.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/decorators/on_edited_message.py` & `PyroFork-2.1.7/pyrogram/methods/decorators/on_edited_message.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/decorators/on_inline_query.py` & `PyroFork-2.1.7/pyrogram/methods/decorators/on_inline_query.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/decorators/on_message.py` & `PyroFork-2.1.7/pyrogram/methods/decorators/on_message.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/decorators/on_poll.py` & `PyroFork-2.1.7/pyrogram/methods/decorators/on_poll.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/decorators/on_raw_update.py` & `PyroFork-2.1.7/pyrogram/methods/decorators/on_raw_update.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/decorators/on_user_status.py` & `PyroFork-2.1.7/pyrogram/methods/decorators/on_user_status.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/invite_links/__init__.py` & `PyroFork-2.1.7/pyrogram/methods/invite_links/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/invite_links/approve_all_chat_join_requests.py` & `PyroFork-2.1.7/pyrogram/methods/invite_links/approve_all_chat_join_requests.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/invite_links/approve_chat_join_request.py` & `PyroFork-2.1.7/pyrogram/methods/invite_links/approve_chat_join_request.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/invite_links/create_chat_invite_link.py` & `PyroFork-2.1.7/pyrogram/methods/invite_links/create_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/invite_links/decline_all_chat_join_requests.py` & `PyroFork-2.1.7/pyrogram/methods/invite_links/decline_all_chat_join_requests.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/invite_links/decline_chat_join_request.py` & `PyroFork-2.1.7/pyrogram/methods/invite_links/decline_chat_join_request.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/invite_links/delete_chat_admin_invite_links.py` & `PyroFork-2.1.7/pyrogram/methods/invite_links/delete_chat_admin_invite_links.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/invite_links/delete_chat_invite_link.py` & `PyroFork-2.1.7/pyrogram/methods/invite_links/delete_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/invite_links/edit_chat_invite_link.py` & `PyroFork-2.1.7/pyrogram/methods/invite_links/edit_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/invite_links/export_chat_invite_link.py` & `PyroFork-2.1.7/pyrogram/methods/invite_links/export_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/invite_links/get_chat_admin_invite_links.py` & `PyroFork-2.1.7/pyrogram/methods/invite_links/get_chat_admin_invite_links.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/invite_links/get_chat_admin_invite_links_count.py` & `PyroFork-2.1.7/pyrogram/methods/invite_links/get_chat_admin_invite_links_count.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/invite_links/get_chat_admins_with_invite_links.py` & `PyroFork-2.1.7/pyrogram/methods/invite_links/get_chat_admins_with_invite_links.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/invite_links/get_chat_invite_link.py` & `PyroFork-2.1.7/pyrogram/methods/invite_links/get_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/invite_links/get_chat_invite_link_joiners.py` & `PyroFork-2.1.7/pyrogram/methods/invite_links/get_chat_invite_link_joiners.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/invite_links/get_chat_invite_link_joiners_count.py` & `PyroFork-2.1.7/pyrogram/methods/invite_links/get_chat_invite_link_joiners_count.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/invite_links/get_chat_join_requests.py` & `PyroFork-2.1.7/pyrogram/methods/invite_links/get_chat_join_requests.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/invite_links/revoke_chat_invite_link.py` & `PyroFork-2.1.7/pyrogram/methods/invite_links/revoke_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/messages/__init__.py` & `PyroFork-2.1.7/pyrogram/methods/messages/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/messages/copy_media_group.py` & `PyroFork-2.1.7/pyrogram/methods/messages/copy_media_group.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/messages/copy_message.py` & `PyroFork-2.1.7/pyrogram/methods/messages/copy_message.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/messages/delete_messages.py` & `PyroFork-2.1.7/pyrogram/methods/messages/delete_messages.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/messages/download_media.py` & `PyroFork-2.1.7/pyrogram/methods/messages/download_media.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/messages/edit_inline_caption.py` & `PyroFork-2.1.7/pyrogram/methods/messages/edit_inline_caption.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/messages/edit_inline_media.py` & `PyroFork-2.1.7/pyrogram/methods/messages/edit_inline_media.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/messages/edit_inline_reply_markup.py` & `PyroFork-2.1.7/pyrogram/methods/messages/edit_inline_reply_markup.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/messages/edit_inline_text.py` & `PyroFork-2.1.7/pyrogram/methods/messages/edit_inline_text.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/messages/edit_message_caption.py` & `PyroFork-2.1.7/pyrogram/methods/messages/edit_message_caption.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/messages/edit_message_media.py` & `PyroFork-2.1.7/pyrogram/methods/messages/edit_message_media.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/messages/edit_message_reply_markup.py` & `PyroFork-2.1.7/pyrogram/methods/messages/edit_message_reply_markup.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/messages/edit_message_text.py` & `PyroFork-2.1.7/pyrogram/methods/messages/edit_message_text.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/messages/forward_messages.py` & `PyroFork-2.1.7/pyrogram/methods/messages/forward_messages.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/messages/get_chat_history.py` & `PyroFork-2.1.7/pyrogram/methods/messages/get_chat_history.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/messages/get_chat_history_count.py` & `PyroFork-2.1.7/pyrogram/methods/messages/get_chat_history_count.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/messages/get_custom_emoji_stickers.py` & `PyroFork-2.1.7/pyrogram/methods/messages/get_custom_emoji_stickers.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/messages/get_discussion_message.py` & `PyroFork-2.1.7/pyrogram/methods/messages/get_discussion_message.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/messages/get_discussion_replies.py` & `PyroFork-2.1.7/pyrogram/methods/messages/get_discussion_replies.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/messages/get_discussion_replies_count.py` & `PyroFork-2.1.7/pyrogram/methods/messages/get_discussion_replies_count.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/messages/get_media_group.py` & `PyroFork-2.1.7/pyrogram/methods/messages/get_media_group.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/messages/get_messages.py` & `PyroFork-2.1.7/pyrogram/methods/messages/get_messages.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/messages/inline_session.py` & `PyroFork-2.1.7/pyrogram/methods/messages/inline_session.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/messages/read_chat_history.py` & `PyroFork-2.1.7/pyrogram/methods/messages/read_chat_history.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/messages/retract_vote.py` & `PyroFork-2.1.7/pyrogram/methods/messages/retract_vote.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/messages/search_global.py` & `PyroFork-2.1.7/pyrogram/methods/messages/search_global.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/messages/search_global_count.py` & `PyroFork-2.1.7/pyrogram/methods/messages/search_global_count.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/messages/search_messages.py` & `PyroFork-2.1.7/pyrogram/methods/messages/search_messages.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/messages/search_messages_count.py` & `PyroFork-2.1.7/pyrogram/methods/messages/search_messages_count.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/messages/send_animation.py` & `PyroFork-2.1.7/pyrogram/methods/messages/send_animation.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/messages/send_audio.py` & `PyroFork-2.1.7/pyrogram/methods/messages/send_audio.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/messages/send_cached_media.py` & `PyroFork-2.1.7/pyrogram/methods/messages/send_cached_media.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/messages/send_chat_action.py` & `PyroFork-2.1.7/pyrogram/methods/messages/send_chat_action.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/messages/send_contact.py` & `PyroFork-2.1.7/pyrogram/methods/messages/send_contact.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/messages/send_dice.py` & `PyroFork-2.1.7/pyrogram/methods/messages/send_dice.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/messages/send_document.py` & `PyroFork-2.1.7/pyrogram/methods/messages/send_document.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/messages/send_location.py` & `PyroFork-2.1.7/pyrogram/methods/messages/send_location.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/messages/send_media_group.py` & `PyroFork-2.1.7/pyrogram/methods/messages/send_media_group.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/messages/send_message.py` & `PyroFork-2.1.7/pyrogram/methods/messages/send_message.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/messages/send_photo.py` & `PyroFork-2.1.7/pyrogram/methods/messages/send_photo.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/messages/send_poll.py` & `PyroFork-2.1.7/pyrogram/methods/messages/send_poll.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/messages/send_reaction.py` & `PyroFork-2.1.7/pyrogram/methods/messages/send_reaction.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/messages/send_sticker.py` & `PyroFork-2.1.7/pyrogram/methods/messages/send_sticker.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/messages/send_venue.py` & `PyroFork-2.1.7/pyrogram/methods/messages/send_venue.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/messages/send_video.py` & `PyroFork-2.1.7/pyrogram/methods/messages/send_video.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/messages/send_video_note.py` & `PyroFork-2.1.7/pyrogram/methods/messages/send_video_note.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/messages/send_voice.py` & `PyroFork-2.1.7/pyrogram/methods/messages/send_voice.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/messages/stop_poll.py` & `PyroFork-2.1.7/pyrogram/methods/messages/stop_poll.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/messages/stream_media.py` & `PyroFork-2.1.7/pyrogram/methods/messages/stream_media.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/messages/vote_poll.py` & `PyroFork-2.1.7/pyrogram/methods/messages/vote_poll.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/password/__init__.py` & `PyroFork-2.1.7/pyrogram/methods/password/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/password/change_cloud_password.py` & `PyroFork-2.1.7/pyrogram/methods/password/change_cloud_password.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/password/enable_cloud_password.py` & `PyroFork-2.1.7/pyrogram/methods/password/enable_cloud_password.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/password/remove_cloud_password.py` & `PyroFork-2.1.7/pyrogram/methods/password/remove_cloud_password.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/stickers/__init__.py` & `PyroFork-2.1.7/pyrogram/methods/stickers/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/stickers/add_sticker_to_set.py` & `PyroFork-2.1.7/pyrogram/methods/stickers/add_sticker_to_set.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/stickers/create_sticker_set.py` & `PyroFork-2.1.7/pyrogram/methods/stickers/create_sticker_set.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/stickers/get_sticker_set.py` & `PyroFork-2.1.7/pyrogram/methods/stickers/get_sticker_set.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/users/__init__.py` & `PyroFork-2.1.7/pyrogram/methods/users/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/users/block_user.py` & `PyroFork-2.1.7/pyrogram/methods/users/block_user.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/users/delete_profile_photos.py` & `PyroFork-2.1.7/pyrogram/methods/users/delete_profile_photos.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/users/get_chat_photos.py` & `PyroFork-2.1.7/pyrogram/methods/users/get_chat_photos.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/users/get_chat_photos_count.py` & `PyroFork-2.1.7/pyrogram/methods/users/get_chat_photos_count.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/users/get_common_chats.py` & `PyroFork-2.1.7/pyrogram/methods/users/get_common_chats.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/users/get_default_emoji_statuses.py` & `PyroFork-2.1.7/pyrogram/methods/users/get_default_emoji_statuses.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/users/get_me.py` & `PyroFork-2.1.7/pyrogram/methods/users/get_me.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/users/get_users.py` & `PyroFork-2.1.7/pyrogram/methods/users/get_users.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/users/set_emoji_status.py` & `PyroFork-2.1.7/pyrogram/methods/users/set_emoji_status.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/users/set_profile_photo.py` & `PyroFork-2.1.7/pyrogram/methods/users/set_profile_photo.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/users/set_username.py` & `PyroFork-2.1.7/pyrogram/methods/users/set_username.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/users/unblock_user.py` & `PyroFork-2.1.7/pyrogram/methods/users/unblock_user.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/users/update_profile.py` & `PyroFork-2.1.7/pyrogram/methods/users/update_profile.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/utilities/__init__.py` & `PyroFork-2.1.7/pyrogram/methods/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/utilities/add_handler.py` & `PyroFork-2.1.7/pyrogram/methods/utilities/add_handler.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/utilities/compose.py` & `PyroFork-2.1.7/pyrogram/methods/utilities/compose.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/utilities/export_session_string.py` & `PyroFork-2.1.7/pyrogram/methods/utilities/export_session_string.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/utilities/idle.py` & `PyroFork-2.1.7/pyrogram/methods/utilities/idle.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/utilities/remove_handler.py` & `PyroFork-2.1.7/pyrogram/methods/utilities/remove_handler.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/utilities/restart.py` & `PyroFork-2.1.7/pyrogram/methods/utilities/restart.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/utilities/run.py` & `PyroFork-2.1.7/pyrogram/methods/utilities/run.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/utilities/start.py` & `PyroFork-2.1.7/pyrogram/methods/utilities/start.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/utilities/stop.py` & `PyroFork-2.1.7/pyrogram/methods/utilities/stop.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/methods/utilities/stop_transmission.py` & `PyroFork-2.1.7/pyrogram/methods/utilities/stop_transmission.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/mime_types.py` & `PyroFork-2.1.7/pyrogram/mime_types.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/parser/__init__.py` & `PyroFork-2.1.7/pyrogram/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/parser/html.py` & `PyroFork-2.1.7/pyrogram/parser/html.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/parser/markdown.py` & `PyroFork-2.1.7/pyrogram/parser/markdown.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/parser/parser.py` & `PyroFork-2.1.7/pyrogram/parser/parser.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/parser/utils.py` & `PyroFork-2.1.7/pyrogram/parser/utils.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/raw/__init__.py` & `PyroFork-2.1.7/pyrogram/raw/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/raw/core/__init__.py` & `PyroFork-2.1.7/pyrogram/raw/core/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/raw/core/future_salt.py` & `PyroFork-2.1.7/pyrogram/raw/core/future_salt.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/raw/core/future_salts.py` & `PyroFork-2.1.7/pyrogram/raw/core/future_salts.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/raw/core/gzip_packed.py` & `PyroFork-2.1.7/pyrogram/raw/core/gzip_packed.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/raw/core/list.py` & `PyroFork-2.1.7/pyrogram/raw/core/list.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/raw/core/message.py` & `PyroFork-2.1.7/pyrogram/raw/core/message.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/raw/core/msg_container.py` & `PyroFork-2.1.7/pyrogram/raw/core/msg_container.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/raw/core/primitives/__init__.py` & `PyroFork-2.1.7/pyrogram/raw/core/primitives/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/raw/core/primitives/bool.py` & `PyroFork-2.1.7/pyrogram/raw/core/primitives/bool.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/raw/core/primitives/bytes.py` & `PyroFork-2.1.7/pyrogram/raw/core/primitives/bytes.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/raw/core/primitives/double.py` & `PyroFork-2.1.7/pyrogram/raw/core/primitives/double.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/raw/core/primitives/int.py` & `PyroFork-2.1.7/pyrogram/raw/core/primitives/int.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/raw/core/primitives/string.py` & `PyroFork-2.1.7/pyrogram/raw/core/primitives/string.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/raw/core/primitives/vector.py` & `PyroFork-2.1.7/pyrogram/raw/core/primitives/vector.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/raw/core/tl_object.py` & `PyroFork-2.1.7/pyrogram/raw/core/tl_object.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/session/__init__.py` & `PyroFork-2.1.7/pyrogram/session/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/session/auth.py` & `PyroFork-2.1.7/pyrogram/session/auth.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/session/internals/__init__.py` & `PyroFork-2.1.7/pyrogram/session/internals/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/session/internals/data_center.py` & `PyroFork-2.1.7/pyrogram/session/internals/data_center.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,15 +27,16 @@
     }
 
     PROD = {
         1: "149.154.175.53",
         2: "149.154.167.51",
         3: "149.154.175.100",
         4: "149.154.167.91",
-        5: "91.108.56.130"
+        5: "91.108.56.130",
+        203: "91.105.192.100"
     }
 
     PROD_MEDIA = {
         2: "149.154.167.151",
         4: "149.154.164.250"
     }
 
@@ -46,15 +47,16 @@
     }
 
     PROD_IPV6 = {
         1: "2001:b28:f23d:f001::a",
         2: "2001:67c:4e8:f002::a",
         3: "2001:b28:f23d:f003::a",
         4: "2001:67c:4e8:f004::a",
-        5: "2001:b28:f23f:f005::a"
+        5: "2001:b28:f23f:f005::a",
+        203: "2a0a:f280:0203:000a:5000:0000:0000:0100"
     }
 
     PROD_IPV6_MEDIA = {
         2: "2001:067c:04e8:f002:0000:0000:0000:000b",
         4: "2001:067c:04e8:f004:0000:0000:0000:000b"
     }
```

### Comparing `PyroFork-2.1.6/pyrogram/session/internals/msg_factory.py` & `PyroFork-2.1.7/pyrogram/session/internals/msg_factory.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/session/internals/msg_id.py` & `PyroFork-2.1.7/pyrogram/session/internals/msg_id.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/session/internals/seq_no.py` & `PyroFork-2.1.7/pyrogram/session/internals/seq_no.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/session/session.py` & `PyroFork-2.1.7/pyrogram/session/session.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/storage/__init__.py` & `PyroFork-2.1.7/tests/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,11 +11,7 @@
 #  Pyrogram is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
-
-from .file_storage import FileStorage
-from .memory_storage import MemoryStorage
-from .storage import Storage
```

### Comparing `PyroFork-2.1.6/pyrogram/storage/file_storage.py` & `PyroFork-2.1.7/pyrogram/storage/file_storage.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/storage/memory_storage.py` & `PyroFork-2.1.7/pyrogram/storage/memory_storage.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/storage/sqlite_storage.py` & `PyroFork-2.1.7/pyrogram/storage/sqlite_storage.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/storage/storage.py` & `PyroFork-2.1.7/pyrogram/storage/storage.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/sync.py` & `PyroFork-2.1.7/pyrogram/sync.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/types/__init__.py` & `PyroFork-2.1.7/pyrogram/types/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/types/authorization/__init__.py` & `PyroFork-2.1.7/pyrogram/types/authorization/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/types/authorization/sent_code.py` & `PyroFork-2.1.7/pyrogram/types/authorization/sent_code.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/types/authorization/terms_of_service.py` & `PyroFork-2.1.7/pyrogram/types/authorization/terms_of_service.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/types/bots_and_keyboards/__init__.py` & `PyroFork-2.1.7/pyrogram/types/bots_and_keyboards/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/types/bots_and_keyboards/bot_command.py` & `PyroFork-2.1.7/pyrogram/types/bots_and_keyboards/bot_command.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/types/bots_and_keyboards/bot_command_scope.py` & `PyroFork-2.1.7/pyrogram/types/bots_and_keyboards/bot_command_scope.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/types/bots_and_keyboards/bot_command_scope_all_chat_administrators.py` & `PyroFork-2.1.7/pyrogram/types/bots_and_keyboards/bot_command_scope_all_chat_administrators.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/types/bots_and_keyboards/bot_command_scope_all_group_chats.py` & `PyroFork-2.1.7/pyrogram/types/bots_and_keyboards/bot_command_scope_all_group_chats.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/types/bots_and_keyboards/bot_command_scope_all_private_chats.py` & `PyroFork-2.1.7/pyrogram/types/bots_and_keyboards/bot_command_scope_all_private_chats.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/types/bots_and_keyboards/bot_command_scope_chat.py` & `PyroFork-2.1.7/pyrogram/types/bots_and_keyboards/bot_command_scope_chat.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_administrators.py` & `PyroFork-2.1.7/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_administrators.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_member.py` & `PyroFork-2.1.7/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_member.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/types/bots_and_keyboards/bot_command_scope_default.py` & `PyroFork-2.1.7/pyrogram/types/bots_and_keyboards/bot_command_scope_default.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/types/bots_and_keyboards/callback_game.py` & `PyroFork-2.1.7/pyrogram/types/bots_and_keyboards/callback_game.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/types/bots_and_keyboards/callback_query.py` & `PyroFork-2.1.7/pyrogram/types/bots_and_keyboards/callback_query.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/types/bots_and_keyboards/force_reply.py` & `PyroFork-2.1.7/pyrogram/types/bots_and_keyboards/force_reply.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/types/bots_and_keyboards/game_high_score.py` & `PyroFork-2.1.7/pyrogram/types/bots_and_keyboards/game_high_score.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/types/bots_and_keyboards/inline_keyboard_button.py` & `PyroFork-2.1.7/pyrogram/types/bots_and_keyboards/inline_keyboard_button.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/types/bots_and_keyboards/inline_keyboard_markup.py` & `PyroFork-2.1.7/pyrogram/types/bots_and_keyboards/inline_keyboard_markup.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/types/bots_and_keyboards/keyboard_button.py` & `PyroFork-2.1.7/pyrogram/types/bots_and_keyboards/keyboard_button.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/types/bots_and_keyboards/login_url.py` & `PyroFork-2.1.7/pyrogram/types/bots_and_keyboards/login_url.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/types/bots_and_keyboards/menu_button.py` & `PyroFork-2.1.7/pyrogram/types/bots_and_keyboards/menu_button.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/types/bots_and_keyboards/menu_button_commands.py` & `PyroFork-2.1.7/pyrogram/types/bots_and_keyboards/menu_button_commands.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/types/bots_and_keyboards/menu_button_default.py` & `PyroFork-2.1.7/pyrogram/types/bots_and_keyboards/menu_button_default.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/types/bots_and_keyboards/menu_button_web_app.py` & `PyroFork-2.1.7/pyrogram/types/bots_and_keyboards/menu_button_web_app.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/types/bots_and_keyboards/reply_keyboard_markup.py` & `PyroFork-2.1.7/pyrogram/types/bots_and_keyboards/reply_keyboard_markup.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/types/bots_and_keyboards/reply_keyboard_remove.py` & `PyroFork-2.1.7/pyrogram/types/bots_and_keyboards/reply_keyboard_remove.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/types/bots_and_keyboards/sent_web_app_message.py` & `PyroFork-2.1.7/pyrogram/types/bots_and_keyboards/sent_web_app_message.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/types/bots_and_keyboards/web_app_info.py` & `PyroFork-2.1.7/pyrogram/types/bots_and_keyboards/web_app_info.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/types/inline_mode/__init__.py` & `PyroFork-2.1.7/pyrogram/types/inline_mode/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/types/inline_mode/chosen_inline_result.py` & `PyroFork-2.1.7/pyrogram/types/inline_mode/chosen_inline_result.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/types/inline_mode/inline_query.py` & `PyroFork-2.1.7/pyrogram/types/inline_mode/inline_query.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/types/inline_mode/inline_query_result.py` & `PyroFork-2.1.7/pyrogram/types/inline_mode/inline_query_result.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/types/inline_mode/inline_query_result_animation.py` & `PyroFork-2.1.7/pyrogram/types/inline_mode/inline_query_result_animation.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/types/inline_mode/inline_query_result_article.py` & `PyroFork-2.1.7/pyrogram/types/inline_mode/inline_query_result_article.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/types/inline_mode/inline_query_result_audio.py` & `PyroFork-2.1.7/pyrogram/types/inline_mode/inline_query_result_audio.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/types/inline_mode/inline_query_result_cached_animation.py` & `PyroFork-2.1.7/pyrogram/types/inline_mode/inline_query_result_cached_animation.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/types/inline_mode/inline_query_result_cached_audio.py` & `PyroFork-2.1.7/pyrogram/types/inline_mode/inline_query_result_cached_audio.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/types/inline_mode/inline_query_result_cached_document.py` & `PyroFork-2.1.7/pyrogram/types/inline_mode/inline_query_result_cached_document.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/types/inline_mode/inline_query_result_cached_photo.py` & `PyroFork-2.1.7/pyrogram/types/inline_mode/inline_query_result_cached_photo.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/types/inline_mode/inline_query_result_cached_sticker.py` & `PyroFork-2.1.7/pyrogram/types/inline_mode/inline_query_result_cached_sticker.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/types/inline_mode/inline_query_result_cached_video.py` & `PyroFork-2.1.7/pyrogram/types/inline_mode/inline_query_result_cached_video.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/types/inline_mode/inline_query_result_cached_voice.py` & `PyroFork-2.1.7/pyrogram/types/inline_mode/inline_query_result_cached_voice.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/types/inline_mode/inline_query_result_contact.py` & `PyroFork-2.1.7/pyrogram/types/inline_mode/inline_query_result_contact.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/types/inline_mode/inline_query_result_document.py` & `PyroFork-2.1.7/pyrogram/types/inline_mode/inline_query_result_document.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/types/inline_mode/inline_query_result_location.py` & `PyroFork-2.1.7/pyrogram/types/inline_mode/inline_query_result_location.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/types/inline_mode/inline_query_result_photo.py` & `PyroFork-2.1.7/pyrogram/types/inline_mode/inline_query_result_photo.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/types/inline_mode/inline_query_result_venue.py` & `PyroFork-2.1.7/pyrogram/types/inline_mode/inline_query_result_venue.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/types/inline_mode/inline_query_result_video.py` & `PyroFork-2.1.7/pyrogram/types/inline_mode/inline_query_result_video.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/types/inline_mode/inline_query_result_voice.py` & `PyroFork-2.1.7/pyrogram/types/inline_mode/inline_query_result_voice.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/types/input_media/__init__.py` & `PyroFork-2.1.7/pyrogram/types/input_media/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/types/input_media/input_media.py` & `PyroFork-2.1.7/pyrogram/types/input_media/input_media.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/types/input_media/input_media_animation.py` & `PyroFork-2.1.7/pyrogram/types/input_media/input_media_animation.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/types/input_media/input_media_audio.py` & `PyroFork-2.1.7/pyrogram/types/input_media/input_media_audio.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/types/input_media/input_media_document.py` & `PyroFork-2.1.7/pyrogram/types/input_media/input_media_document.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/types/input_media/input_media_photo.py` & `PyroFork-2.1.7/pyrogram/types/input_media/input_media_photo.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/types/input_media/input_media_video.py` & `PyroFork-2.1.7/pyrogram/types/input_media/input_media_video.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/types/input_media/input_phone_contact.py` & `PyroFork-2.1.7/pyrogram/types/input_media/input_phone_contact.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/types/input_message_content/__init__.py` & `PyroFork-2.1.7/pyrogram/types/input_message_content/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/types/input_message_content/input_message_content.py` & `PyroFork-2.1.7/pyrogram/types/input_message_content/input_message_content.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/types/input_message_content/input_text_message_content.py` & `PyroFork-2.1.7/pyrogram/types/input_message_content/input_text_message_content.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/types/list.py` & `PyroFork-2.1.7/pyrogram/types/list.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/types/messages_and_media/__init__.py` & `PyroFork-2.1.7/pyrogram/types/messages_and_media/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/types/messages_and_media/animation.py` & `PyroFork-2.1.7/pyrogram/types/messages_and_media/animation.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/types/messages_and_media/audio.py` & `PyroFork-2.1.7/pyrogram/types/messages_and_media/audio.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/types/messages_and_media/contact.py` & `PyroFork-2.1.7/pyrogram/types/messages_and_media/contact.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/types/messages_and_media/dice.py` & `PyroFork-2.1.7/pyrogram/types/messages_and_media/dice.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/types/messages_and_media/document.py` & `PyroFork-2.1.7/pyrogram/types/messages_and_media/document.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/types/messages_and_media/game.py` & `PyroFork-2.1.7/pyrogram/types/messages_and_media/game.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/types/messages_and_media/location.py` & `PyroFork-2.1.7/pyrogram/types/messages_and_media/location.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/types/messages_and_media/message.py` & `PyroFork-2.1.7/pyrogram/types/messages_and_media/message.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/types/messages_and_media/message_entity.py` & `PyroFork-2.1.7/pyrogram/types/messages_and_media/message_entity.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/types/messages_and_media/message_reactions.py` & `PyroFork-2.1.7/pyrogram/types/messages_and_media/message_reactions.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/types/messages_and_media/photo.py` & `PyroFork-2.1.7/pyrogram/types/messages_and_media/photo.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/types/messages_and_media/poll.py` & `PyroFork-2.1.7/pyrogram/types/messages_and_media/poll.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/types/messages_and_media/poll_option.py` & `PyroFork-2.1.7/pyrogram/types/messages_and_media/poll_option.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/types/messages_and_media/reaction.py` & `PyroFork-2.1.7/pyrogram/types/messages_and_media/reaction.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/types/messages_and_media/sticker.py` & `PyroFork-2.1.7/pyrogram/types/messages_and_media/sticker.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/types/messages_and_media/stickerset.py` & `PyroFork-2.1.7/pyrogram/types/messages_and_media/stickerset.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/types/messages_and_media/stripped_thumbnail.py` & `PyroFork-2.1.7/pyrogram/types/messages_and_media/stripped_thumbnail.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/types/messages_and_media/thumbnail.py` & `PyroFork-2.1.7/pyrogram/types/messages_and_media/thumbnail.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/types/messages_and_media/venue.py` & `PyroFork-2.1.7/pyrogram/types/messages_and_media/venue.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/types/messages_and_media/video.py` & `PyroFork-2.1.7/pyrogram/types/messages_and_media/video.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/types/messages_and_media/video_note.py` & `PyroFork-2.1.7/pyrogram/types/messages_and_media/video_note.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/types/messages_and_media/voice.py` & `PyroFork-2.1.7/pyrogram/types/messages_and_media/voice.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/types/messages_and_media/web_app_data.py` & `PyroFork-2.1.7/pyrogram/types/messages_and_media/web_app_data.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/types/messages_and_media/web_page.py` & `PyroFork-2.1.7/pyrogram/types/messages_and_media/web_page.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/types/object.py` & `PyroFork-2.1.7/pyrogram/types/object.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/types/update.py` & `PyroFork-2.1.7/pyrogram/types/update.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/types/user_and_chats/__init__.py` & `PyroFork-2.1.7/pyrogram/types/user_and_chats/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/types/user_and_chats/chat.py` & `PyroFork-2.1.7/pyrogram/types/user_and_chats/chat.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/types/user_and_chats/chat_admin_with_invite_links.py` & `PyroFork-2.1.7/pyrogram/types/user_and_chats/chat_admin_with_invite_links.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/types/user_and_chats/chat_event.py` & `PyroFork-2.1.7/pyrogram/types/user_and_chats/chat_event.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/types/user_and_chats/chat_event_filter.py` & `PyroFork-2.1.7/pyrogram/types/user_and_chats/chat_event_filter.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/types/user_and_chats/chat_invite_link.py` & `PyroFork-2.1.7/pyrogram/types/user_and_chats/chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/types/user_and_chats/chat_join_request.py` & `PyroFork-2.1.7/pyrogram/types/user_and_chats/chat_join_request.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/types/user_and_chats/chat_joined_by_request.py` & `PyroFork-2.1.7/pyrogram/types/user_and_chats/chat_joined_by_request.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/types/user_and_chats/chat_joiner.py` & `PyroFork-2.1.7/pyrogram/types/user_and_chats/chat_joiner.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/types/user_and_chats/chat_member.py` & `PyroFork-2.1.7/pyrogram/types/user_and_chats/chat_member.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/types/user_and_chats/chat_member_updated.py` & `PyroFork-2.1.7/pyrogram/types/user_and_chats/chat_member_updated.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/types/user_and_chats/chat_permissions.py` & `PyroFork-2.1.7/pyrogram/types/user_and_chats/chat_permissions.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/types/user_and_chats/chat_photo.py` & `PyroFork-2.1.7/pyrogram/types/user_and_chats/chat_photo.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/types/user_and_chats/chat_preview.py` & `PyroFork-2.1.7/pyrogram/types/user_and_chats/chat_preview.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/types/user_and_chats/chat_privileges.py` & `PyroFork-2.1.7/pyrogram/types/user_and_chats/chat_privileges.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/types/user_and_chats/chat_reactions.py` & `PyroFork-2.1.7/pyrogram/types/user_and_chats/chat_reactions.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/types/user_and_chats/dialog.py` & `PyroFork-2.1.7/pyrogram/types/user_and_chats/dialog.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/types/user_and_chats/emoji_status.py` & `PyroFork-2.1.7/pyrogram/types/user_and_chats/emoji_status.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/types/user_and_chats/forum_topic.py` & `PyroFork-2.1.7/pyrogram/types/user_and_chats/forum_topic.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/types/user_and_chats/forum_topic_closed.py` & `PyroFork-2.1.7/pyrogram/types/user_and_chats/forum_topic_closed.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/types/user_and_chats/forum_topic_created.py` & `PyroFork-2.1.7/pyrogram/types/user_and_chats/forum_topic_created.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/types/user_and_chats/forum_topic_edited.py` & `PyroFork-2.1.7/pyrogram/types/user_and_chats/forum_topic_edited.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/types/user_and_chats/forum_topic_reopened.py` & `PyroFork-2.1.7/pyrogram/types/user_and_chats/forum_topic_reopened.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/types/user_and_chats/general_forum_topic_hidden.py` & `PyroFork-2.1.7/pyrogram/types/user_and_chats/general_forum_topic_hidden.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/types/user_and_chats/general_forum_topic_unhidden.py` & `PyroFork-2.1.7/pyrogram/types/user_and_chats/general_forum_topic_unhidden.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/types/user_and_chats/invite_link_importer.py` & `PyroFork-2.1.7/pyrogram/types/user_and_chats/invite_link_importer.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/types/user_and_chats/peer_channel.py` & `PyroFork-2.1.7/pyrogram/types/user_and_chats/peer_channel.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/types/user_and_chats/peer_user.py` & `PyroFork-2.1.7/pyrogram/types/user_and_chats/peer_user.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/types/user_and_chats/restriction.py` & `PyroFork-2.1.7/pyrogram/types/user_and_chats/restriction.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/types/user_and_chats/user.py` & `PyroFork-2.1.7/pyrogram/types/user_and_chats/user.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/types/user_and_chats/username.py` & `PyroFork-2.1.7/pyrogram/types/user_and_chats/username.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/types/user_and_chats/video_chat_ended.py` & `PyroFork-2.1.7/pyrogram/types/user_and_chats/video_chat_ended.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/types/user_and_chats/video_chat_members_invited.py` & `PyroFork-2.1.7/pyrogram/types/user_and_chats/video_chat_members_invited.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/types/user_and_chats/video_chat_scheduled.py` & `PyroFork-2.1.7/pyrogram/types/user_and_chats/video_chat_scheduled.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/types/user_and_chats/video_chat_started.py` & `PyroFork-2.1.7/pyrogram/types/user_and_chats/video_chat_started.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/pyrogram/utils.py` & `PyroFork-2.1.7/pyrogram/utils.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/setup.py` & `PyroFork-2.1.7/setup.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/tests/__init__.py` & `PyroFork-2.1.7/tests/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/tests/filters/__init__.py` & `PyroFork-2.1.7/tests/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/tests/filters/test_command.py` & `PyroFork-2.1.7/tests/filters/test_command.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/tests/parser/test_html.py` & `PyroFork-2.1.7/tests/parser/test_html.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.1.6/tests/test_file_id.py` & `PyroFork-2.1.7/tests/test_file_id.py`

 * *Files identical despite different names*

