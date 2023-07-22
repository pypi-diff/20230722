# Comparing `tmp/PyroFork-2.2.4.tar.gz` & `tmp/PyroFork-2.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyroFork-2.2.4.tar", last modified: Tue Jun 27 11:58:21 2023, max compression
+gzip compressed data, was "PyroFork-2.2.5.tar", last modified: Tue Jul  4 04:28:15 2023, max compression
```

## Comparing `PyroFork-2.2.4.tar` & `PyroFork-2.2.5.tar`

### file list

```diff
@@ -1,529 +1,529 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:58:21.567395 PyroFork-2.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-06-27 11:58:00.000000 PyroFork-2.2.4/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-06-27 11:58:00.000000 PyroFork-2.2.4/COPYING.lesser
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-27 11:58:00.000000 PyroFork-2.2.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-06-27 11:58:00.000000 PyroFork-2.2.4/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     3897 2023-06-27 11:58:21.567395 PyroFork-2.2.4/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:58:21.495394 PyroFork-2.2.4/PyroFork.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3897 2023-06-27 11:58:21.000000 PyroFork-2.2.4/PyroFork.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20336 2023-06-27 11:58:21.000000 PyroFork-2.2.4/PyroFork.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 11:58:21.000000 PyroFork-2.2.4/PyroFork.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 11:58:21.000000 PyroFork-2.2.4/PyroFork.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-27 11:58:21.000000 PyroFork-2.2.4/PyroFork.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-27 11:58:21.000000 PyroFork-2.2.4/PyroFork.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-06-27 11:58:00.000000 PyroFork-2.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:58:21.495394 PyroFork-2.2.4/compiler/
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-06-27 11:58:00.000000 PyroFork-2.2.4/compiler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:58:21.495394 PyroFork-2.2.4/compiler/api/
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-06-27 11:58:00.000000 PyroFork-2.2.4/compiler/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22402 2023-06-27 11:58:00.000000 PyroFork-2.2.4/compiler/api/compiler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:58:21.495394 PyroFork-2.2.4/compiler/api/source/
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-06-27 11:58:00.000000 PyroFork-2.2.4/compiler/api/source/auth_key.tl
--rw-r--r--   0 runner    (1001) docker     (123)   169763 2023-06-27 11:58:00.000000 PyroFork-2.2.4/compiler/api/source/main_api.tl
--rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-06-27 11:58:00.000000 PyroFork-2.2.4/compiler/api/source/sys_msgs.tl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:58:21.495394 PyroFork-2.2.4/compiler/api/template/
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-06-27 11:58:00.000000 PyroFork-2.2.4/compiler/api/template/combinator.txt
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-06-27 11:58:00.000000 PyroFork-2.2.4/compiler/api/template/type.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:58:21.495394 PyroFork-2.2.4/compiler/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-06-27 11:58:00.000000 PyroFork-2.2.4/compiler/docs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20074 2023-06-27 11:58:00.000000 PyroFork-2.2.4/compiler/docs/compiler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:58:21.495394 PyroFork-2.2.4/compiler/docs/template/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-27 11:58:00.000000 PyroFork-2.2.4/compiler/docs/template/page.txt
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-27 11:58:00.000000 PyroFork-2.2.4/compiler/docs/template/toctree.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:58:21.495394 PyroFork-2.2.4/compiler/errors/
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-06-27 11:58:00.000000 PyroFork-2.2.4/compiler/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4917 2023-06-27 11:58:00.000000 PyroFork-2.2.4/compiler/errors/compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-06-27 11:58:00.000000 PyroFork-2.2.4/compiler/errors/sort.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:58:21.499394 PyroFork-2.2.4/compiler/errors/source/
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-06-27 11:58:00.000000 PyroFork-2.2.4/compiler/errors/source/303_SEE_OTHER.tsv
--rw-r--r--   0 runner    (1001) docker     (123)    22642 2023-06-27 11:58:00.000000 PyroFork-2.2.4/compiler/errors/source/400_BAD_REQUEST.tsv
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-06-27 11:58:00.000000 PyroFork-2.2.4/compiler/errors/source/401_UNAUTHORIZED.tsv
--rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-06-27 11:58:00.000000 PyroFork-2.2.4/compiler/errors/source/403_FORBIDDEN.tsv
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-06-27 11:58:00.000000 PyroFork-2.2.4/compiler/errors/source/406_NOT_ACCEPTABLE.tsv
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-06-27 11:58:00.000000 PyroFork-2.2.4/compiler/errors/source/420_FLOOD.tsv
--rw-r--r--   0 runner    (1001) docker     (123)     4219 2023-06-27 11:58:00.000000 PyroFork-2.2.4/compiler/errors/source/500_INTERNAL_SERVER_ERROR.tsv
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-27 11:58:00.000000 PyroFork-2.2.4/compiler/errors/source/503_SERVICE_UNAVAILABLE.tsv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:58:21.499394 PyroFork-2.2.4/compiler/errors/template/
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-06-27 11:58:00.000000 PyroFork-2.2.4/compiler/errors/template/class.txt
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-27 11:58:00.000000 PyroFork-2.2.4/compiler/errors/template/sub_class.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:58:21.499394 PyroFork-2.2.4/pyrogram/
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    41005 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:58:21.499394 PyroFork-2.2.4/pyrogram/connection/
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/connection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/connection/connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:58:21.499394 PyroFork-2.2.4/pyrogram/connection/transport/
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/connection/transport/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:58:21.499394 PyroFork-2.2.4/pyrogram/connection/transport/tcp/
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/connection/transport/tcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4100 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/connection/transport/tcp/tcp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/connection/transport/tcp/tcp_abridged.py
--rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/connection/transport/tcp/tcp_abridged_o.py
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/connection/transport/tcp/tcp_full.py
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/connection/transport/tcp/tcp_intermediate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/connection/transport/tcp/tcp_intermediate_o.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:58:21.503394 PyroFork-2.2.4/pyrogram/crypto/
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/crypto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4013 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/crypto/aes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4767 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/crypto/mtproto.py
--rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/crypto/prime.py
--rw-r--r--   0 runner    (1001) docker     (123)    13437 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/crypto/rsa.py
--rw-r--r--   0 runner    (1001) docker     (123)    10085 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)   208021 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/emoji.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:58:21.503394 PyroFork-2.2.4/pyrogram/enums/
--rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/enums/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/enums/auto_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/enums/chat_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     4520 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/enums/chat_event_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/enums/chat_member_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/enums/chat_members_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/enums/chat_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/enums/message_entity_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/enums/message_media_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/enums/message_service_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/enums/messages_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/enums/next_code_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/enums/parse_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/enums/poll_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/enums/sent_code_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/enums/user_status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:58:21.503394 PyroFork-2.2.4/pyrogram/errors/
--rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/errors/rpc_error.py
--rw-r--r--   0 runner    (1001) docker     (123)    15154 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/file_id.py
--rw-r--r--   0 runner    (1001) docker     (123)    24836 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:58:21.507394 PyroFork-2.2.4/pyrogram/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/handlers/callback_query_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/handlers/chat_join_request_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/handlers/chat_member_updated_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/handlers/chosen_inline_result_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/handlers/deleted_messages_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/handlers/disconnect_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/handlers/edited_message_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/handlers/handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/handlers/inline_query_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/handlers/message_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/handlers/poll_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/handlers/raw_update_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/handlers/user_status_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:58:21.507394 PyroFork-2.2.4/pyrogram/methods/
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:58:21.507394 PyroFork-2.2.4/pyrogram/methods/advanced/
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/advanced/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/advanced/invoke.py
--rw-r--r--   0 runner    (1001) docker     (123)     4560 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/advanced/resolve_peer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8164 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/advanced/save_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:58:21.511394 PyroFork-2.2.4/pyrogram/methods/auth/
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/auth/accept_terms_of_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/auth/check_password.py
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/auth/connect.py
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/auth/disconnect.py
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/auth/get_password_hint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/auth/initialize.py
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/auth/log_out.py
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/auth/recover_password.py
--rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/auth/resend_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/auth/send_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/auth/send_recovery_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/auth/sign_in.py
--rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/auth/sign_in_bot.py
--rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/auth/sign_up.py
--rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/auth/terminate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:58:21.511394 PyroFork-2.2.4/pyrogram/methods/bots/
--rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/bots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/bots/answer_callback_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     4990 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/bots/answer_inline_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/bots/answer_web_app_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/bots/delete_bot_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/bots/get_bot_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/bots/get_bot_default_privileges.py
--rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/bots/get_chat_menu_button.py
--rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/bots/get_game_high_scores.py
--rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/bots/get_inline_bot_results.py
--rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/bots/request_callback_answer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/bots/send_game.py
--rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/bots/send_inline_bot_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/bots/set_bot_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/bots/set_bot_default_privileges.py
--rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/bots/set_chat_menu_button.py
--rw-r--r--   0 runner    (1001) docker     (123)     3946 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/bots/set_game_score.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:58:21.519394 PyroFork-2.2.4/pyrogram/methods/chats/
--rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/chats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/chats/add_chat_members.py
--rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/chats/archive_chats.py
--rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/chats/ban_chat_member.py
--rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/chats/close_forum_topic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/chats/close_general_topic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/chats/create_channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/chats/create_forum_topic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/chats/create_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/chats/create_supergroup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/chats/delete_channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/chats/delete_chat_photo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/chats/delete_forum_topic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/chats/delete_supergroup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/chats/delete_user_history.py
--rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/chats/edit_forum_topic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/chats/edit_general_topic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/chats/get_chat.py
--rw-r--r--   0 runner    (1001) docker     (123)     4032 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/chats/get_chat_event_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/chats/get_chat_member.py
--rw-r--r--   0 runner    (1001) docker     (123)     5282 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/chats/get_chat_members.py
--rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/chats/get_chat_members_count.py
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/chats/get_chat_online_count.py
--rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/chats/get_dialogs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/chats/get_dialogs_count.py
--rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/chats/get_forum_topics.py
--rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/chats/get_forum_topics_by_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/chats/get_nearby_chats.py
--rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/chats/get_send_as_chats.py
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/chats/hide_general_topic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/chats/join_chat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2605 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/chats/leave_chat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/chats/mark_chat_unread.py
--rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/chats/pin_chat_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/chats/promote_chat_member.py
--rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/chats/reopen_forum_topic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/chats/reopen_general_topic.py
--rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/chats/restrict_chat_member.py
--rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/chats/set_administrator_title.py
--rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/chats/set_chat_description.py
--rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/chats/set_chat_permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/chats/set_chat_photo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/chats/set_chat_protected_content.py
--rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/chats/set_chat_title.py
--rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/chats/set_chat_username.py
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/chats/set_send_as_chat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/chats/set_slow_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/chats/unarchive_chats.py
--rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/chats/unban_chat_member.py
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/chats/unhide_general_topic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/chats/unpin_all_chat_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/chats/unpin_chat_message.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:58:21.523394 PyroFork-2.2.4/pyrogram/methods/contacts/
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/contacts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/contacts/add_contact.py
--rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/contacts/delete_contacts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/contacts/get_contacts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/contacts/get_contacts_count.py
--rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/contacts/import_contacts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:58:21.523394 PyroFork-2.2.4/pyrogram/methods/decorators/
--rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/decorators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/decorators/on_callback_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/decorators/on_chat_join_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/decorators/on_chat_member_updated.py
--rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/decorators/on_chosen_inline_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/decorators/on_deleted_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/decorators/on_disconnect.py
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/decorators/on_edited_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/decorators/on_inline_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/decorators/on_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/decorators/on_poll.py
--rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/decorators/on_raw_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/decorators/on_user_status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:58:21.527394 PyroFork-2.2.4/pyrogram/methods/invite_links/
--rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/invite_links/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/invite_links/approve_all_chat_join_requests.py
--rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/invite_links/approve_chat_join_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/invite_links/create_chat_invite_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/invite_links/decline_all_chat_join_requests.py
--rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/invite_links/decline_chat_join_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/invite_links/delete_chat_admin_invite_links.py
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/invite_links/delete_chat_invite_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     3533 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/invite_links/edit_chat_invite_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/invite_links/export_chat_invite_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/invite_links/get_chat_admin_invite_links.py
--rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/invite_links/get_chat_admin_invite_links_count.py
--rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/invite_links/get_chat_admins_with_invite_links.py
--rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/invite_links/get_chat_invite_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/invite_links/get_chat_invite_link_joiners.py
--rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/invite_links/get_chat_invite_link_joiners_count.py
--rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/invite_links/get_chat_join_requests.py
--rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/invite_links/revoke_chat_invite_link.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:58:21.535395 PyroFork-2.2.4/pyrogram/methods/messages/
--rw-r--r--   0 runner    (1001) docker     (123)     3921 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/messages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5963 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/messages/copy_media_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     5423 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/messages/copy_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/messages/delete_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     7530 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/messages/download_media.py
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/messages/edit_inline_caption.py
--rw-r--r--   0 runner    (1001) docker     (123)    10375 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/messages/edit_inline_media.py
--rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/messages/edit_inline_reply_markup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/messages/edit_inline_text.py
--rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/messages/edit_message_caption.py
--rw-r--r--   0 runner    (1001) docker     (123)    13022 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/messages/edit_message_media.py
--rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/messages/edit_message_reply_markup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/messages/edit_message_text.py
--rw-r--r--   0 runner    (1001) docker     (123)     5018 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/messages/forward_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/messages/get_chat_history.py
--rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/messages/get_chat_history_count.py
--rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/messages/get_custom_emoji_stickers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/messages/get_discussion_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/messages/get_discussion_replies.py
--rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/messages/get_discussion_replies_count.py
--rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/messages/get_media_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     4741 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/messages/get_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/messages/inline_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/messages/read_chat_history.py
--rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/messages/retract_vote.py
--rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/messages/search_global.py
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/messages/search_global_count.py
--rw-r--r--   0 runner    (1001) docker     (123)     5349 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/messages/search_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/messages/search_messages_count.py
--rw-r--r--   0 runner    (1001) docker     (123)    12828 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/messages/send_animation.py
--rw-r--r--   0 runner    (1001) docker     (123)    11362 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/messages/send_audio.py
--rw-r--r--   0 runner    (1001) docker     (123)     5723 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/messages/send_cached_media.py
--rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/messages/send_chat_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     5111 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/messages/send_contact.py
--rw-r--r--   0 runner    (1001) docker     (123)     5085 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/messages/send_dice.py
--rw-r--r--   0 runner    (1001) docker     (123)    10712 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/messages/send_document.py
--rw-r--r--   0 runner    (1001) docker     (123)     4820 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/messages/send_location.py
--rw-r--r--   0 runner    (1001) docker     (123)    20821 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/messages/send_media_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     7509 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/messages/send_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     9682 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/messages/send_photo.py
--rw-r--r--   0 runner    (1001) docker     (123)     8315 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/messages/send_poll.py
--rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/messages/send_reaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     8582 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/messages/send_sticker.py
--rw-r--r--   0 runner    (1001) docker     (123)     5641 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/messages/send_venue.py
--rw-r--r--   0 runner    (1001) docker     (123)    12198 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/messages/send_video.py
--rw-r--r--   0 runner    (1001) docker     (123)     9556 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/messages/send_video_note.py
--rw-r--r--   0 runner    (1001) docker     (123)     9672 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/messages/send_voice.py
--rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/messages/stop_poll.py
--rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/messages/stream_media.py
--rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/messages/vote_poll.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:58:21.535395 PyroFork-2.2.4/pyrogram/methods/password/
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/password/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/password/change_cloud_password.py
--rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/password/enable_cloud_password.py
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/password/remove_cloud_password.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:58:21.535395 PyroFork-2.2.4/pyrogram/methods/stickers/
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/stickers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/stickers/add_sticker_to_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/stickers/create_sticker_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/stickers/get_sticker_set.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:58:21.539394 PyroFork-2.2.4/pyrogram/methods/users/
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/users/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/users/block_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/users/delete_profile_photos.py
--rw-r--r--   0 runner    (1001) docker     (123)     4421 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/users/get_chat_photos.py
--rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/users/get_chat_photos_count.py
--rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/users/get_common_chats.py
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/users/get_default_emoji_statuses.py
--rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/users/get_me.py
--rw-r--r--   0 runner    (1001) docker     (123)     2562 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/users/get_users.py
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/users/set_emoji_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/users/set_profile_photo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/users/set_username.py
--rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/users/unblock_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/users/update_profile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:58:21.539394 PyroFork-2.2.4/pyrogram/methods/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/utilities/add_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/utilities/compose.py
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/utilities/export_session_string.py
--rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/utilities/idle.py
--rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/utilities/remove_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/utilities/restart.py
--rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/utilities/run.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1554 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/utilities/run_sync.py
--rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/utilities/start.py
--rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/utilities/stop.py
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/methods/utilities/stop_transmission.py
--rw-r--r--   0 runner    (1001) docker     (123)    61915 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/mime_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:58:21.539394 PyroFork-2.2.4/pyrogram/parser/
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8681 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/parser/html.py
--rw-r--r--   0 runner    (1001) docker     (123)     5770 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/parser/markdown.py
--rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/parser/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/parser/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:58:21.539394 PyroFork-2.2.4/pyrogram/raw/
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/raw/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:58:21.543395 PyroFork-2.2.4/pyrogram/raw/core/
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/raw/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/raw/core/future_salt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/raw/core/future_salts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/raw/core/gzip_packed.py
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/raw/core/list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/raw/core/message.py
--rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/raw/core/msg_container.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:58:21.543395 PyroFork-2.2.4/pyrogram/raw/core/primitives/
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/raw/core/primitives/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/raw/core/primitives/bool.py
--rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/raw/core/primitives/bytes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/raw/core/primitives/double.py
--rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/raw/core/primitives/int.py
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/raw/core/primitives/string.py
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/raw/core/primitives/vector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/raw/core/tl_object.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:58:21.543395 PyroFork-2.2.4/pyrogram/session/
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/session/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10513 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/session/auth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:58:21.543395 PyroFork-2.2.4/pyrogram/session/internals/
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/session/internals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/session/internals/data_center.py
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/session/internals/msg_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/session/internals/msg_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/session/internals/seq_no.py
--rw-r--r--   0 runner    (1001) docker     (123)    12440 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/session/session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:58:21.543395 PyroFork-2.2.4/pyrogram/storage/
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/storage/dummy_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/storage/file_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/storage/memory_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     6017 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/storage/mongo_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:58:21.547395 PyroFork-2.2.4/pyrogram/storage/sqlite/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/storage/sqlite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/storage/sqlite/cursor.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/storage/sqlite/sqlite.py
--rw-r--r--   0 runner    (1001) docker     (123)     6307 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/storage/sqlite_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/storage/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/sync.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:58:21.547395 PyroFork-2.2.4/pyrogram/types/
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/types/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:58:21.547395 PyroFork-2.2.4/pyrogram/types/authorization/
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/types/authorization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/types/authorization/sent_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/types/authorization/terms_of_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:58:21.551395 PyroFork-2.2.4/pyrogram/types/bots_and_keyboards/
--rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/types/bots_and_keyboards/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/types/bots_and_keyboards/bot_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/types/bots_and_keyboards/bot_command_scope.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/types/bots_and_keyboards/bot_command_scope_all_chat_administrators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/types/bots_and_keyboards/bot_command_scope_all_group_chats.py
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/types/bots_and_keyboards/bot_command_scope_all_private_chats.py
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/types/bots_and_keyboards/bot_command_scope_chat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_administrators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_member.py
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/types/bots_and_keyboards/bot_command_scope_default.py
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/types/bots_and_keyboards/callback_game.py
--rw-r--r--   0 runner    (1001) docker     (123)    12797 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/types/bots_and_keyboards/callback_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/types/bots_and_keyboards/force_reply.py
--rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/types/bots_and_keyboards/game_high_score.py
--rw-r--r--   0 runner    (1001) docker     (123)     8120 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/types/bots_and_keyboards/inline_keyboard_button.py
--rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/types/bots_and_keyboards/inline_keyboard_markup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3514 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/types/bots_and_keyboards/keyboard_button.py
--rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/types/bots_and_keyboards/login_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/types/bots_and_keyboards/menu_button.py
--rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/types/bots_and_keyboards/menu_button_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/types/bots_and_keyboards/menu_button_default.py
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/types/bots_and_keyboards/menu_button_web_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/types/bots_and_keyboards/reply_keyboard_markup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/types/bots_and_keyboards/reply_keyboard_remove.py
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/types/bots_and_keyboards/sent_web_app_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/types/bots_and_keyboards/web_app_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:58:21.555395 PyroFork-2.2.4/pyrogram/types/inline_mode/
--rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/types/inline_mode/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/types/inline_mode/chosen_inline_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     7298 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/types/inline_mode/inline_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/types/inline_mode/inline_query_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     5782 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/types/inline_mode/inline_query_result_animation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3304 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/types/inline_mode/inline_query_result_article.py
--rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/types/inline_mode/inline_query_result_audio.py
--rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/types/inline_mode/inline_query_result_cached_animation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/types/inline_mode/inline_query_result_cached_audio.py
--rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/types/inline_mode/inline_query_result_cached_document.py
--rw-r--r--   0 runner    (1001) docker     (123)     4312 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/types/inline_mode/inline_query_result_cached_photo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/types/inline_mode/inline_query_result_cached_sticker.py
--rw-r--r--   0 runner    (1001) docker     (123)     4394 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/types/inline_mode/inline_query_result_cached_video.py
--rw-r--r--   0 runner    (1001) docker     (123)     4202 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/types/inline_mode/inline_query_result_cached_voice.py
--rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/types/inline_mode/inline_query_result_contact.py
--rw-r--r--   0 runner    (1001) docker     (123)     5240 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/types/inline_mode/inline_query_result_document.py
--rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/types/inline_mode/inline_query_result_location.py
--rw-r--r--   0 runner    (1001) docker     (123)     5261 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/types/inline_mode/inline_query_result_photo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/types/inline_mode/inline_query_result_venue.py
--rw-r--r--   0 runner    (1001) docker     (123)     5474 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/types/inline_mode/inline_query_result_video.py
--rw-r--r--   0 runner    (1001) docker     (123)     4360 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/types/inline_mode/inline_query_result_voice.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:58:21.555395 PyroFork-2.2.4/pyrogram/types/input_media/
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/types/input_media/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/types/input_media/input_media.py
--rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/types/input_media/input_media_animation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/types/input_media/input_media_audio.py
--rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/types/input_media/input_media_document.py
--rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/types/input_media/input_media_photo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/types/input_media/input_media_video.py
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/types/input_media/input_phone_contact.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:58:21.555395 PyroFork-2.2.4/pyrogram/types/input_message_content/
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/types/input_message_content/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/types/input_message_content/input_message_content.py
--rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/types/input_message_content/input_text_message_content.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/types/list.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:58:21.559395 PyroFork-2.2.4/pyrogram/types/messages_and_media/
--rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/types/messages_and_media/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4044 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/types/messages_and_media/animation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4069 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/types/messages_and_media/audio.py
--rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/types/messages_and_media/contact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/types/messages_and_media/dice.py
--rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/types/messages_and_media/document.py
--rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/types/messages_and_media/game.py
--rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/types/messages_and_media/location.py
--rw-r--r--   0 runner    (1001) docker     (123)   153586 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/types/messages_and_media/message.py
--rw-r--r--   0 runner    (1001) docker     (123)     4352 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/types/messages_and_media/message_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/types/messages_and_media/message_reactions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4309 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/types/messages_and_media/photo.py
--rw-r--r--   0 runner    (1001) docker     (123)     8016 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/types/messages_and_media/poll.py
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/types/messages_and_media/poll_option.py
--rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/types/messages_and_media/reaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     6909 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/types/messages_and_media/sticker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/types/messages_and_media/stickerset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/types/messages_and_media/stripped_thumbnail.py
--rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/types/messages_and_media/thumbnail.py
--rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/types/messages_and_media/venue.py
--rw-r--r--   0 runner    (1001) docker     (123)     4389 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/types/messages_and_media/video.py
--rw-r--r--   0 runner    (1001) docker     (123)     3601 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/types/messages_and_media/video_note.py
--rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/types/messages_and_media/voice.py
--rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/types/messages_and_media/web_app_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     6351 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/types/messages_and_media/web_page.py
--rw-r--r--   0 runner    (1001) docker     (123)     3862 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/types/object.py
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/types/update.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:58:21.567395 PyroFork-2.2.4/pyrogram/types/user_and_chats/
--rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/types/user_and_chats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33966 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/types/user_and_chats/chat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/types/user_and_chats/chat_admin_with_invite_links.py
--rw-r--r--   0 runner    (1001) docker     (123)    22023 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/types/user_and_chats/chat_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     5514 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/types/user_and_chats/chat_event_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4579 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/types/user_and_chats/chat_invite_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/types/user_and_chats/chat_join_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/types/user_and_chats/chat_joined_by_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/types/user_and_chats/chat_joiner.py
--rw-r--r--   0 runner    (1001) docker     (123)     9444 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/types/user_and_chats/chat_member.py
--rw-r--r--   0 runner    (1001) docker     (123)     3674 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/types/user_and_chats/chat_member_updated.py
--rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/types/user_and_chats/chat_permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3967 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/types/user_and_chats/chat_photo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/types/user_and_chats/chat_preview.py
--rw-r--r--   0 runner    (1001) docker     (123)     5300 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/types/user_and_chats/chat_privileges.py
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/types/user_and_chats/chat_reactions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/types/user_and_chats/dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/types/user_and_chats/emoji_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     4970 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/types/user_and_chats/forum_topic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/types/user_and_chats/forum_topic_closed.py
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/types/user_and_chats/forum_topic_created.py
--rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/types/user_and_chats/forum_topic_edited.py
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/types/user_and_chats/forum_topic_reopened.py
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/types/user_and_chats/general_forum_topic_hidden.py
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/types/user_and_chats/general_forum_topic_unhidden.py
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/types/user_and_chats/invite_link_importer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/types/user_and_chats/peer_channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/types/user_and_chats/peer_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/types/user_and_chats/restriction.py
--rw-r--r--   0 runner    (1001) docker     (123)    13658 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/types/user_and_chats/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/types/user_and_chats/username.py
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/types/user_and_chats/video_chat_ended.py
--rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/types/user_and_chats/video_chat_members_invited.py
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/types/user_and_chats/video_chat_scheduled.py
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/types/user_and_chats/video_chat_started.py
--rw-r--r--   0 runner    (1001) docker     (123)    11166 2023-06-27 11:58:00.000000 PyroFork-2.2.4/pyrogram/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-27 11:58:00.000000 PyroFork-2.2.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 11:58:21.567395 PyroFork-2.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3555 2023-06-27 11:58:00.000000 PyroFork-2.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:58:21.567395 PyroFork-2.2.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-06-27 11:58:00.000000 PyroFork-2.2.4/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:58:21.567395 PyroFork-2.2.4/tests/filters/
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-06-27 11:58:00.000000 PyroFork-2.2.4/tests/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-06-27 11:58:00.000000 PyroFork-2.2.4/tests/filters/test_command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:58:21.567395 PyroFork-2.2.4/tests/parser/
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-06-27 11:58:00.000000 PyroFork-2.2.4/tests/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6264 2023-06-27 11:58:00.000000 PyroFork-2.2.4/tests/parser/test_html.py
--rw-r--r--   0 runner    (1001) docker     (123)     8208 2023-06-27 11:58:00.000000 PyroFork-2.2.4/tests/test_file_id.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 04:28:15.467418 PyroFork-2.2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-07-04 04:27:59.000000 PyroFork-2.2.5/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-07-04 04:27:59.000000 PyroFork-2.2.5/COPYING.lesser
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-04 04:27:59.000000 PyroFork-2.2.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-07-04 04:27:59.000000 PyroFork-2.2.5/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     3897 2023-07-04 04:28:15.467418 PyroFork-2.2.5/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 04:28:15.387417 PyroFork-2.2.5/PyroFork.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3897 2023-07-04 04:28:15.000000 PyroFork-2.2.5/PyroFork.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20336 2023-07-04 04:28:15.000000 PyroFork-2.2.5/PyroFork.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 04:28:15.000000 PyroFork-2.2.5/PyroFork.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 04:28:15.000000 PyroFork-2.2.5/PyroFork.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-04 04:28:15.000000 PyroFork-2.2.5/PyroFork.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-04 04:28:15.000000 PyroFork-2.2.5/PyroFork.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-07-04 04:27:59.000000 PyroFork-2.2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 04:28:15.387417 PyroFork-2.2.5/compiler/
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-04 04:27:59.000000 PyroFork-2.2.5/compiler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 04:28:15.387417 PyroFork-2.2.5/compiler/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-04 04:27:59.000000 PyroFork-2.2.5/compiler/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22402 2023-07-04 04:27:59.000000 PyroFork-2.2.5/compiler/api/compiler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 04:28:15.387417 PyroFork-2.2.5/compiler/api/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-07-04 04:27:59.000000 PyroFork-2.2.5/compiler/api/source/auth_key.tl
+-rw-r--r--   0 runner    (1001) docker     (123)   169763 2023-07-04 04:27:59.000000 PyroFork-2.2.5/compiler/api/source/main_api.tl
+-rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-07-04 04:27:59.000000 PyroFork-2.2.5/compiler/api/source/sys_msgs.tl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 04:28:15.391417 PyroFork-2.2.5/compiler/api/template/
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-04 04:27:59.000000 PyroFork-2.2.5/compiler/api/template/combinator.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-07-04 04:27:59.000000 PyroFork-2.2.5/compiler/api/template/type.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 04:28:15.391417 PyroFork-2.2.5/compiler/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-04 04:27:59.000000 PyroFork-2.2.5/compiler/docs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20074 2023-07-04 04:27:59.000000 PyroFork-2.2.5/compiler/docs/compiler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 04:28:15.391417 PyroFork-2.2.5/compiler/docs/template/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-04 04:27:59.000000 PyroFork-2.2.5/compiler/docs/template/page.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-04 04:27:59.000000 PyroFork-2.2.5/compiler/docs/template/toctree.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 04:28:15.391417 PyroFork-2.2.5/compiler/errors/
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-04 04:27:59.000000 PyroFork-2.2.5/compiler/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4917 2023-07-04 04:27:59.000000 PyroFork-2.2.5/compiler/errors/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-07-04 04:27:59.000000 PyroFork-2.2.5/compiler/errors/sort.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 04:28:15.395418 PyroFork-2.2.5/compiler/errors/source/
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-07-04 04:27:59.000000 PyroFork-2.2.5/compiler/errors/source/303_SEE_OTHER.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)    22712 2023-07-04 04:27:59.000000 PyroFork-2.2.5/compiler/errors/source/400_BAD_REQUEST.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-04 04:27:59.000000 PyroFork-2.2.5/compiler/errors/source/401_UNAUTHORIZED.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-07-04 04:27:59.000000 PyroFork-2.2.5/compiler/errors/source/403_FORBIDDEN.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-07-04 04:27:59.000000 PyroFork-2.2.5/compiler/errors/source/406_NOT_ACCEPTABLE.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-07-04 04:27:59.000000 PyroFork-2.2.5/compiler/errors/source/420_FLOOD.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)     4219 2023-07-04 04:27:59.000000 PyroFork-2.2.5/compiler/errors/source/500_INTERNAL_SERVER_ERROR.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-04 04:27:59.000000 PyroFork-2.2.5/compiler/errors/source/503_SERVICE_UNAVAILABLE.tsv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 04:28:15.395418 PyroFork-2.2.5/compiler/errors/template/
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-04 04:27:59.000000 PyroFork-2.2.5/compiler/errors/template/class.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-04 04:27:59.000000 PyroFork-2.2.5/compiler/errors/template/sub_class.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 04:28:15.399417 PyroFork-2.2.5/pyrogram/
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41006 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 04:28:15.399417 PyroFork-2.2.5/pyrogram/connection/
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/connection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/connection/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 04:28:15.399417 PyroFork-2.2.5/pyrogram/connection/transport/
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/connection/transport/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 04:28:15.399417 PyroFork-2.2.5/pyrogram/connection/transport/tcp/
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/connection/transport/tcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4100 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/connection/transport/tcp/tcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/connection/transport/tcp/tcp_abridged.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/connection/transport/tcp/tcp_abridged_o.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/connection/transport/tcp/tcp_full.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/connection/transport/tcp/tcp_intermediate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/connection/transport/tcp/tcp_intermediate_o.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 04:28:15.403417 PyroFork-2.2.5/pyrogram/crypto/
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/crypto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4013 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/crypto/aes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4762 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/crypto/mtproto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/crypto/prime.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13437 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/crypto/rsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10085 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)   208021 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/emoji.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 04:28:15.407417 PyroFork-2.2.5/pyrogram/enums/
+-rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/enums/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/enums/auto_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/enums/chat_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4520 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/enums/chat_event_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/enums/chat_member_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/enums/chat_members_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/enums/chat_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/enums/message_entity_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/enums/message_media_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/enums/message_service_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/enums/messages_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/enums/next_code_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/enums/parse_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/enums/poll_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/enums/sent_code_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/enums/user_status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 04:28:15.407417 PyroFork-2.2.5/pyrogram/errors/
+-rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/errors/rpc_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15154 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/file_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24836 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 04:28:15.411418 PyroFork-2.2.5/pyrogram/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/handlers/callback_query_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/handlers/chat_join_request_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/handlers/chat_member_updated_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/handlers/chosen_inline_result_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/handlers/deleted_messages_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/handlers/disconnect_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/handlers/edited_message_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/handlers/handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/handlers/inline_query_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/handlers/message_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/handlers/poll_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/handlers/raw_update_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/handlers/user_status_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 04:28:15.411418 PyroFork-2.2.5/pyrogram/methods/
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 04:28:15.411418 PyroFork-2.2.5/pyrogram/methods/advanced/
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/advanced/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/advanced/invoke.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4560 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/advanced/resolve_peer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8164 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/advanced/save_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 04:28:15.415418 PyroFork-2.2.5/pyrogram/methods/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/auth/accept_terms_of_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/auth/check_password.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/auth/connect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/auth/disconnect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/auth/get_password_hint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/auth/initialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/auth/log_out.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/auth/recover_password.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/auth/resend_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/auth/send_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/auth/send_recovery_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/auth/sign_in.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/auth/sign_in_bot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/auth/sign_up.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/auth/terminate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 04:28:15.423418 PyroFork-2.2.5/pyrogram/methods/bots/
+-rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/bots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/bots/answer_callback_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4990 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/bots/answer_inline_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/bots/answer_web_app_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/bots/delete_bot_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/bots/get_bot_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/bots/get_bot_default_privileges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/bots/get_chat_menu_button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/bots/get_game_high_scores.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/bots/get_inline_bot_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/bots/request_callback_answer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/bots/send_game.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/bots/send_inline_bot_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/bots/set_bot_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/bots/set_bot_default_privileges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/bots/set_chat_menu_button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3946 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/bots/set_game_score.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 04:28:15.435418 PyroFork-2.2.5/pyrogram/methods/chats/
+-rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/chats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/chats/add_chat_members.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/chats/archive_chats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/chats/ban_chat_member.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/chats/close_forum_topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/chats/close_general_topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/chats/create_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/chats/create_forum_topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/chats/create_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/chats/create_supergroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/chats/delete_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/chats/delete_chat_photo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/chats/delete_forum_topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/chats/delete_supergroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/chats/delete_user_history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/chats/edit_forum_topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/chats/edit_general_topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/chats/get_chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4032 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/chats/get_chat_event_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/chats/get_chat_member.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5282 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/chats/get_chat_members.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/chats/get_chat_members_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/chats/get_chat_online_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/chats/get_dialogs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/chats/get_dialogs_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/chats/get_forum_topics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/chats/get_forum_topics_by_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/chats/get_nearby_chats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/chats/get_send_as_chats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/chats/hide_general_topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/chats/join_chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2605 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/chats/leave_chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/chats/mark_chat_unread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/chats/pin_chat_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/chats/promote_chat_member.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/chats/reopen_forum_topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/chats/reopen_general_topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/chats/restrict_chat_member.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/chats/set_administrator_title.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/chats/set_chat_description.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/chats/set_chat_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/chats/set_chat_photo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/chats/set_chat_protected_content.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/chats/set_chat_title.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/chats/set_chat_username.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/chats/set_send_as_chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/chats/set_slow_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/chats/unarchive_chats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/chats/unban_chat_member.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/chats/unhide_general_topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/chats/unpin_all_chat_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/chats/unpin_chat_message.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 04:28:15.435418 PyroFork-2.2.5/pyrogram/methods/contacts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/contacts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/contacts/add_contact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/contacts/delete_contacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/contacts/get_contacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/contacts/get_contacts_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/contacts/import_contacts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 04:28:15.435418 PyroFork-2.2.5/pyrogram/methods/decorators/
+-rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/decorators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/decorators/on_callback_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/decorators/on_chat_join_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/decorators/on_chat_member_updated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/decorators/on_chosen_inline_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/decorators/on_deleted_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/decorators/on_disconnect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/decorators/on_edited_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/decorators/on_inline_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/decorators/on_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/decorators/on_poll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/decorators/on_raw_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/decorators/on_user_status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 04:28:15.439418 PyroFork-2.2.5/pyrogram/methods/invite_links/
+-rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/invite_links/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/invite_links/approve_all_chat_join_requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/invite_links/approve_chat_join_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/invite_links/create_chat_invite_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/invite_links/decline_all_chat_join_requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/invite_links/decline_chat_join_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/invite_links/delete_chat_admin_invite_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/invite_links/delete_chat_invite_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3533 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/invite_links/edit_chat_invite_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/invite_links/export_chat_invite_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/invite_links/get_chat_admin_invite_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/invite_links/get_chat_admin_invite_links_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/invite_links/get_chat_admins_with_invite_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/invite_links/get_chat_invite_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/invite_links/get_chat_invite_link_joiners.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/invite_links/get_chat_invite_link_joiners_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/invite_links/get_chat_join_requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/invite_links/revoke_chat_invite_link.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 04:28:15.443418 PyroFork-2.2.5/pyrogram/methods/messages/
+-rw-r--r--   0 runner    (1001) docker     (123)     3921 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/messages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5963 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/messages/copy_media_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5423 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/messages/copy_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/messages/delete_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7530 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/messages/download_media.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/messages/edit_inline_caption.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10375 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/messages/edit_inline_media.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/messages/edit_inline_reply_markup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/messages/edit_inline_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/messages/edit_message_caption.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13022 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/messages/edit_message_media.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/messages/edit_message_reply_markup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/messages/edit_message_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5018 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/messages/forward_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/messages/get_chat_history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/messages/get_chat_history_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/messages/get_custom_emoji_stickers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/messages/get_discussion_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/messages/get_discussion_replies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/messages/get_discussion_replies_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/messages/get_media_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4741 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/messages/get_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/messages/inline_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/messages/read_chat_history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/messages/retract_vote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/messages/search_global.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/messages/search_global_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5349 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/messages/search_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/messages/search_messages_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12828 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/messages/send_animation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11362 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/messages/send_audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5723 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/messages/send_cached_media.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/messages/send_chat_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5111 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/messages/send_contact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5085 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/messages/send_dice.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10712 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/messages/send_document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4820 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/messages/send_location.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20821 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/messages/send_media_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7509 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/messages/send_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9682 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/messages/send_photo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8315 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/messages/send_poll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/messages/send_reaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8582 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/messages/send_sticker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5641 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/messages/send_venue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12198 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/messages/send_video.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9556 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/messages/send_video_note.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9672 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/messages/send_voice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/messages/stop_poll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/messages/stream_media.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/messages/vote_poll.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 04:28:15.447418 PyroFork-2.2.5/pyrogram/methods/password/
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/password/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/password/change_cloud_password.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/password/enable_cloud_password.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/password/remove_cloud_password.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 04:28:15.447418 PyroFork-2.2.5/pyrogram/methods/stickers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/stickers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/stickers/add_sticker_to_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/stickers/create_sticker_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/stickers/get_sticker_set.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 04:28:15.447418 PyroFork-2.2.5/pyrogram/methods/users/
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/users/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/users/block_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/users/delete_profile_photos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4421 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/users/get_chat_photos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/users/get_chat_photos_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/users/get_common_chats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/users/get_default_emoji_statuses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/users/get_me.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2562 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/users/get_users.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/users/set_emoji_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/users/set_profile_photo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/users/set_username.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/users/unblock_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/users/update_profile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 04:28:15.447418 PyroFork-2.2.5/pyrogram/methods/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/utilities/add_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/utilities/compose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/utilities/export_session_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/utilities/idle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/utilities/remove_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/utilities/restart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/utilities/run.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1554 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/utilities/run_sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/utilities/start.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/utilities/stop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/methods/utilities/stop_transmission.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61915 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/mime_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 04:28:15.451418 PyroFork-2.2.5/pyrogram/parser/
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8681 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/parser/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5770 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/parser/markdown.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/parser/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/parser/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 04:28:15.451418 PyroFork-2.2.5/pyrogram/raw/
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/raw/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 04:28:15.451418 PyroFork-2.2.5/pyrogram/raw/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/raw/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/raw/core/future_salt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/raw/core/future_salts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/raw/core/gzip_packed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/raw/core/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/raw/core/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/raw/core/msg_container.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 04:28:15.451418 PyroFork-2.2.5/pyrogram/raw/core/primitives/
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/raw/core/primitives/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/raw/core/primitives/bool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/raw/core/primitives/bytes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/raw/core/primitives/double.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/raw/core/primitives/int.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/raw/core/primitives/string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/raw/core/primitives/vector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/raw/core/tl_object.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 04:28:15.451418 PyroFork-2.2.5/pyrogram/session/
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/session/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10513 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/session/auth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 04:28:15.451418 PyroFork-2.2.5/pyrogram/session/internals/
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/session/internals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/session/internals/data_center.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/session/internals/msg_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/session/internals/msg_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/session/internals/seq_no.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13018 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/session/session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 04:28:15.451418 PyroFork-2.2.5/pyrogram/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/storage/dummy_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/storage/file_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/storage/memory_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6017 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/storage/mongo_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 04:28:15.451418 PyroFork-2.2.5/pyrogram/storage/sqlite/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/storage/sqlite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/storage/sqlite/cursor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/storage/sqlite/sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6307 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/storage/sqlite_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/storage/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/sync.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 04:28:15.455418 PyroFork-2.2.5/pyrogram/types/
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/types/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 04:28:15.455418 PyroFork-2.2.5/pyrogram/types/authorization/
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/types/authorization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/types/authorization/sent_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/types/authorization/terms_of_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 04:28:15.455418 PyroFork-2.2.5/pyrogram/types/bots_and_keyboards/
+-rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/types/bots_and_keyboards/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/types/bots_and_keyboards/bot_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/types/bots_and_keyboards/bot_command_scope.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/types/bots_and_keyboards/bot_command_scope_all_chat_administrators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/types/bots_and_keyboards/bot_command_scope_all_group_chats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/types/bots_and_keyboards/bot_command_scope_all_private_chats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/types/bots_and_keyboards/bot_command_scope_chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_administrators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_member.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/types/bots_and_keyboards/bot_command_scope_default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/types/bots_and_keyboards/callback_game.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12797 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/types/bots_and_keyboards/callback_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/types/bots_and_keyboards/force_reply.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/types/bots_and_keyboards/game_high_score.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8120 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/types/bots_and_keyboards/inline_keyboard_button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/types/bots_and_keyboards/inline_keyboard_markup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3514 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/types/bots_and_keyboards/keyboard_button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/types/bots_and_keyboards/login_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/types/bots_and_keyboards/menu_button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/types/bots_and_keyboards/menu_button_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/types/bots_and_keyboards/menu_button_default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/types/bots_and_keyboards/menu_button_web_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/types/bots_and_keyboards/reply_keyboard_markup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/types/bots_and_keyboards/reply_keyboard_remove.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/types/bots_and_keyboards/sent_web_app_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/types/bots_and_keyboards/web_app_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 04:28:15.459418 PyroFork-2.2.5/pyrogram/types/inline_mode/
+-rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/types/inline_mode/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/types/inline_mode/chosen_inline_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7298 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/types/inline_mode/inline_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/types/inline_mode/inline_query_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5782 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/types/inline_mode/inline_query_result_animation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3304 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/types/inline_mode/inline_query_result_article.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/types/inline_mode/inline_query_result_audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/types/inline_mode/inline_query_result_cached_animation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/types/inline_mode/inline_query_result_cached_audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/types/inline_mode/inline_query_result_cached_document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4312 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/types/inline_mode/inline_query_result_cached_photo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/types/inline_mode/inline_query_result_cached_sticker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4394 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/types/inline_mode/inline_query_result_cached_video.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4202 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/types/inline_mode/inline_query_result_cached_voice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/types/inline_mode/inline_query_result_contact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5240 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/types/inline_mode/inline_query_result_document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/types/inline_mode/inline_query_result_location.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5261 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/types/inline_mode/inline_query_result_photo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/types/inline_mode/inline_query_result_venue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5474 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/types/inline_mode/inline_query_result_video.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4360 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/types/inline_mode/inline_query_result_voice.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 04:28:15.459418 PyroFork-2.2.5/pyrogram/types/input_media/
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/types/input_media/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/types/input_media/input_media.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/types/input_media/input_media_animation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/types/input_media/input_media_audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/types/input_media/input_media_document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/types/input_media/input_media_photo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/types/input_media/input_media_video.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/types/input_media/input_phone_contact.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 04:28:15.459418 PyroFork-2.2.5/pyrogram/types/input_message_content/
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/types/input_message_content/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/types/input_message_content/input_message_content.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/types/input_message_content/input_text_message_content.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/types/list.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 04:28:15.463418 PyroFork-2.2.5/pyrogram/types/messages_and_media/
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/types/messages_and_media/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4044 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/types/messages_and_media/animation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4069 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/types/messages_and_media/audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/types/messages_and_media/contact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/types/messages_and_media/dice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/types/messages_and_media/document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/types/messages_and_media/game.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/types/messages_and_media/location.py
+-rw-r--r--   0 runner    (1001) docker     (123)   153586 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/types/messages_and_media/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4352 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/types/messages_and_media/message_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/types/messages_and_media/message_reactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4309 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/types/messages_and_media/photo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8016 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/types/messages_and_media/poll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/types/messages_and_media/poll_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/types/messages_and_media/reaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6909 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/types/messages_and_media/sticker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/types/messages_and_media/stickerset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/types/messages_and_media/stripped_thumbnail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/types/messages_and_media/thumbnail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/types/messages_and_media/venue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4389 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/types/messages_and_media/video.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3601 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/types/messages_and_media/video_note.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/types/messages_and_media/voice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/types/messages_and_media/web_app_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6351 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/types/messages_and_media/web_page.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3862 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/types/object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/types/update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 04:28:15.467418 PyroFork-2.2.5/pyrogram/types/user_and_chats/
+-rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/types/user_and_chats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33966 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/types/user_and_chats/chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/types/user_and_chats/chat_admin_with_invite_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22023 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/types/user_and_chats/chat_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5514 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/types/user_and_chats/chat_event_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4579 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/types/user_and_chats/chat_invite_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/types/user_and_chats/chat_join_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/types/user_and_chats/chat_joined_by_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/types/user_and_chats/chat_joiner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9444 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/types/user_and_chats/chat_member.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3674 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/types/user_and_chats/chat_member_updated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/types/user_and_chats/chat_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3967 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/types/user_and_chats/chat_photo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/types/user_and_chats/chat_preview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5300 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/types/user_and_chats/chat_privileges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/types/user_and_chats/chat_reactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/types/user_and_chats/dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/types/user_and_chats/emoji_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4970 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/types/user_and_chats/forum_topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/types/user_and_chats/forum_topic_closed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/types/user_and_chats/forum_topic_created.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/types/user_and_chats/forum_topic_edited.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/types/user_and_chats/forum_topic_reopened.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/types/user_and_chats/general_forum_topic_hidden.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/types/user_and_chats/general_forum_topic_unhidden.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/types/user_and_chats/invite_link_importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/types/user_and_chats/peer_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/types/user_and_chats/peer_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/types/user_and_chats/restriction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13658 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/types/user_and_chats/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/types/user_and_chats/username.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/types/user_and_chats/video_chat_ended.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/types/user_and_chats/video_chat_members_invited.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/types/user_and_chats/video_chat_scheduled.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/types/user_and_chats/video_chat_started.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11166 2023-07-04 04:27:59.000000 PyroFork-2.2.5/pyrogram/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-04 04:27:59.000000 PyroFork-2.2.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 04:28:15.471418 PyroFork-2.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3555 2023-07-04 04:27:59.000000 PyroFork-2.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 04:28:15.467418 PyroFork-2.2.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-04 04:27:59.000000 PyroFork-2.2.5/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 04:28:15.467418 PyroFork-2.2.5/tests/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-07-04 04:27:59.000000 PyroFork-2.2.5/tests/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-07-04 04:27:59.000000 PyroFork-2.2.5/tests/filters/test_command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 04:28:15.467418 PyroFork-2.2.5/tests/parser/
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-04 04:27:59.000000 PyroFork-2.2.5/tests/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6264 2023-07-04 04:27:59.000000 PyroFork-2.2.5/tests/parser/test_html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8208 2023-07-04 04:27:59.000000 PyroFork-2.2.5/tests/test_file_id.py
```

### Comparing `PyroFork-2.2.4/COPYING` & `PyroFork-2.2.5/COPYING`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/COPYING.lesser` & `PyroFork-2.2.5/COPYING.lesser`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/NOTICE` & `PyroFork-2.2.5/NOTICE`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/PKG-INFO` & `PyroFork-2.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyroFork
-Version: 2.2.4
+Version: 2.2.5
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
-Metadata-Version: 2.1 Name: PyroFork Version: 2.2.4 Summary: Elegant, modern
+Metadata-Version: 2.1 Name: PyroFork Version: 2.2.5 Summary: Elegant, modern
 and asynchronous Telegram MTProto API framework in Python for users and bots
 Home-page: https://github.com/Mayuri-Chan/pyrofork Download-URL: https://
 github.com/Mayuri-Chan/pyrofork/releases/latest Author: wulan17 Author-email:
 mayuri@mayuri.my.id License: LGPLv3 Project-URL: Tracker, https://github.com/
 Mayuri-Chan/pyrofork/issues Project-URL: Source, https://github.com/Mayuri-
 Chan/pyrofork Project-URL: Documentation, https://pyrofork.mayuri.my.id
 Keywords: telegram chat messenger mtproto api client library python Classifier:
```

### Comparing `PyroFork-2.2.4/PyroFork.egg-info/PKG-INFO` & `PyroFork-2.2.5/PyroFork.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyroFork
-Version: 2.2.4
+Version: 2.2.5
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
-Metadata-Version: 2.1 Name: PyroFork Version: 2.2.4 Summary: Elegant, modern
+Metadata-Version: 2.1 Name: PyroFork Version: 2.2.5 Summary: Elegant, modern
 and asynchronous Telegram MTProto API framework in Python for users and bots
 Home-page: https://github.com/Mayuri-Chan/pyrofork Download-URL: https://
 github.com/Mayuri-Chan/pyrofork/releases/latest Author: wulan17 Author-email:
 mayuri@mayuri.my.id License: LGPLv3 Project-URL: Tracker, https://github.com/
 Mayuri-Chan/pyrofork/issues Project-URL: Source, https://github.com/Mayuri-
 Chan/pyrofork Project-URL: Documentation, https://pyrofork.mayuri.my.id
 Keywords: telegram chat messenger mtproto api client library python Classifier:
```

### Comparing `PyroFork-2.2.4/PyroFork.egg-info/SOURCES.txt` & `PyroFork-2.2.5/PyroFork.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/README.md` & `PyroFork-2.2.5/README.md`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/compiler/__init__.py` & `PyroFork-2.2.5/compiler/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/compiler/api/__init__.py` & `PyroFork-2.2.5/compiler/api/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/compiler/api/compiler.py` & `PyroFork-2.2.5/compiler/api/compiler.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/compiler/api/source/auth_key.tl` & `PyroFork-2.2.5/compiler/api/source/auth_key.tl`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/compiler/api/source/main_api.tl` & `PyroFork-2.2.5/compiler/api/source/main_api.tl`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/compiler/api/source/sys_msgs.tl` & `PyroFork-2.2.5/compiler/api/source/sys_msgs.tl`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/compiler/api/template/combinator.txt` & `PyroFork-2.2.5/compiler/api/template/combinator.txt`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/compiler/api/template/type.txt` & `PyroFork-2.2.5/compiler/api/template/type.txt`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/compiler/docs/__init__.py` & `PyroFork-2.2.5/compiler/docs/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/compiler/docs/compiler.py` & `PyroFork-2.2.5/compiler/docs/compiler.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/compiler/errors/__init__.py` & `PyroFork-2.2.5/compiler/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/compiler/errors/compiler.py` & `PyroFork-2.2.5/compiler/errors/compiler.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/compiler/errors/sort.py` & `PyroFork-2.2.5/compiler/errors/sort.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/compiler/errors/source/400_BAD_REQUEST.tsv` & `PyroFork-2.2.5/compiler/errors/source/400_BAD_REQUEST.tsv`

 * *Files 0% similar despite different names*

```diff
@@ -308,14 +308,16 @@
 THEME_FILE_INVALID	Invalid theme file provided
 THEME_FORMAT_INVALID	Invalid theme format provided
 THEME_INVALID	Invalid theme provided
 THEME_MIME_INVALID	You cannot create this theme because the mime-type is invalid
 TMP_PASSWORD_DISABLED	The temporary password is disabled
 TMP_PASSWORD_INVALID	The temporary password is invalid
 TOKEN_INVALID	The provided token is invalid
+TOPIC_CLOSED	The topic was closed
+TOPIC_DELETED	The topic was deleted
 TTL_DAYS_INVALID	The provided TTL days is invalid
 TTL_MEDIA_INVALID	The media does not support self-destruction
 TYPES_EMPTY	The types parameter is empty
 TYPE_CONSTRUCTOR_INVALID	The type constructor is invalid
 UNTIL_DATE_INVALID	That date parameter is invalid
 URL_INVALID	The URL provided is invalid
 USAGE_LIMIT_INVALID	The usage limit is invalid
```

### Comparing `PyroFork-2.2.4/compiler/errors/source/401_UNAUTHORIZED.tsv` & `PyroFork-2.2.5/compiler/errors/source/401_UNAUTHORIZED.tsv`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/compiler/errors/source/403_FORBIDDEN.tsv` & `PyroFork-2.2.5/compiler/errors/source/403_FORBIDDEN.tsv`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/compiler/errors/source/406_NOT_ACCEPTABLE.tsv` & `PyroFork-2.2.5/compiler/errors/source/406_NOT_ACCEPTABLE.tsv`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/compiler/errors/source/500_INTERNAL_SERVER_ERROR.tsv` & `PyroFork-2.2.5/compiler/errors/source/500_INTERNAL_SERVER_ERROR.tsv`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/__init__.py` & `PyroFork-2.2.5/pyrogram/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
 __fork_name__ = "PyroFork"
-__version__ = "2.2.4"
+__version__ = "2.2.5"
 __license__ = "GNU Lesser General Public License v3.0 (LGPL-3.0)"
 __copyright__ = "Copyright (C) 2017-present Dan <https://github.com/delivrance>"
 
 from concurrent.futures.thread import ThreadPoolExecutor
 
 
 class StopTransmission(Exception):
```

### Comparing `PyroFork-2.2.4/pyrogram/client.py` & `PyroFork-2.2.5/pyrogram/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -120,15 +120,15 @@
             pass to the ``session_string`` parameter.
             Defaults to False.
 
         mongodb (``dict``, *optional*):
             Mongodb config as dict, e.g.: *dict(connection=async_pymongo.AsyncClient("mongodb://..."), remove_peers=False)*.
             Only applicable for new sessions.
         
-        storage (`obj:~pyrogram.storage.Storage`, *optional*):
+        storage (:obj:`~pyrogram.storage.Storage`, *optional*):
             Custom session storage.
 
         phone_number (``str``, *optional*):
             Pass the phone number as string (with the Country Code prefix included) to avoid entering it manually.
             Only applicable for new sessions.
 
         phone_code (``str``, *optional*):
```

### Comparing `PyroFork-2.2.4/pyrogram/connection/__init__.py` & `PyroFork-2.2.5/pyrogram/connection/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/connection/connection.py` & `PyroFork-2.2.5/pyrogram/connection/connection.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/connection/transport/__init__.py` & `PyroFork-2.2.5/pyrogram/connection/transport/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/connection/transport/tcp/__init__.py` & `PyroFork-2.2.5/pyrogram/connection/transport/tcp/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/connection/transport/tcp/tcp.py` & `PyroFork-2.2.5/pyrogram/connection/transport/tcp/tcp.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/connection/transport/tcp/tcp_abridged.py` & `PyroFork-2.2.5/pyrogram/connection/transport/tcp/tcp_abridged.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/connection/transport/tcp/tcp_abridged_o.py` & `PyroFork-2.2.5/pyrogram/connection/transport/tcp/tcp_abridged_o.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/connection/transport/tcp/tcp_full.py` & `PyroFork-2.2.5/pyrogram/connection/transport/tcp/tcp_full.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/connection/transport/tcp/tcp_intermediate.py` & `PyroFork-2.2.5/pyrogram/connection/transport/tcp/tcp_intermediate.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/connection/transport/tcp/tcp_intermediate_o.py` & `PyroFork-2.2.5/pyrogram/connection/transport/tcp/tcp_intermediate_o.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/crypto/__init__.py` & `PyroFork-2.2.5/pyrogram/crypto/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/crypto/aes.py` & `PyroFork-2.2.5/pyrogram/crypto/aes.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/crypto/mtproto.py` & `PyroFork-2.2.5/pyrogram/crypto/mtproto.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 from typing import List
 
 from pyrogram.errors import SecurityCheckMismatch
 from pyrogram.raw.core import Message, Long
 from . import aes
 from ..session.internals import MsgId
 
-STORED_MSG_IDS_MAX_SIZE = 1000 * 2
+STORED_MSG_IDS_MAX_SIZE = 500
 
 
 def kdf(auth_key: bytes, msg_key: bytes, outgoing: bool) -> tuple:
     # https://core.telegram.org/mtproto/description#defining-aes-key-and-initialization-vector
     x = 0 if outgoing else 8
 
     sha256_a = sha256(msg_key + auth_key[x: x + 36]).digest()
```

### Comparing `PyroFork-2.2.4/pyrogram/crypto/prime.py` & `PyroFork-2.2.5/pyrogram/crypto/prime.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/crypto/rsa.py` & `PyroFork-2.2.5/pyrogram/crypto/rsa.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/dispatcher.py` & `PyroFork-2.2.5/pyrogram/dispatcher.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/emoji.py` & `PyroFork-2.2.5/pyrogram/emoji.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/enums/__init__.py` & `PyroFork-2.2.5/pyrogram/enums/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/enums/auto_name.py` & `PyroFork-2.2.5/pyrogram/enums/auto_name.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/enums/chat_action.py` & `PyroFork-2.2.5/pyrogram/enums/chat_action.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/enums/chat_event_action.py` & `PyroFork-2.2.5/pyrogram/enums/chat_event_action.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/enums/chat_member_status.py` & `PyroFork-2.2.5/pyrogram/enums/chat_member_status.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/enums/chat_members_filter.py` & `PyroFork-2.2.5/pyrogram/enums/chat_members_filter.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/enums/chat_type.py` & `PyroFork-2.2.5/pyrogram/enums/chat_type.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/enums/message_entity_type.py` & `PyroFork-2.2.5/pyrogram/enums/message_entity_type.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/enums/message_media_type.py` & `PyroFork-2.2.5/pyrogram/enums/message_media_type.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/enums/message_service_type.py` & `PyroFork-2.2.5/pyrogram/enums/message_service_type.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/enums/messages_filter.py` & `PyroFork-2.2.5/pyrogram/enums/messages_filter.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/enums/next_code_type.py` & `PyroFork-2.2.5/pyrogram/enums/next_code_type.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/enums/parse_mode.py` & `PyroFork-2.2.5/pyrogram/enums/parse_mode.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/enums/poll_type.py` & `PyroFork-2.2.5/pyrogram/enums/poll_type.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/enums/sent_code_type.py` & `PyroFork-2.2.5/pyrogram/enums/sent_code_type.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/enums/user_status.py` & `PyroFork-2.2.5/pyrogram/enums/user_status.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/errors/__init__.py` & `PyroFork-2.2.5/pyrogram/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/errors/rpc_error.py` & `PyroFork-2.2.5/pyrogram/errors/rpc_error.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/file_id.py` & `PyroFork-2.2.5/pyrogram/file_id.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/filters.py` & `PyroFork-2.2.5/pyrogram/filters.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/handlers/__init__.py` & `PyroFork-2.2.5/pyrogram/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/handlers/callback_query_handler.py` & `PyroFork-2.2.5/pyrogram/handlers/callback_query_handler.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/handlers/chat_join_request_handler.py` & `PyroFork-2.2.5/pyrogram/handlers/chat_join_request_handler.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/handlers/chat_member_updated_handler.py` & `PyroFork-2.2.5/pyrogram/handlers/chat_member_updated_handler.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/handlers/chosen_inline_result_handler.py` & `PyroFork-2.2.5/pyrogram/handlers/chosen_inline_result_handler.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/handlers/deleted_messages_handler.py` & `PyroFork-2.2.5/pyrogram/handlers/deleted_messages_handler.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/handlers/disconnect_handler.py` & `PyroFork-2.2.5/pyrogram/handlers/disconnect_handler.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/handlers/edited_message_handler.py` & `PyroFork-2.2.5/pyrogram/handlers/edited_message_handler.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/handlers/handler.py` & `PyroFork-2.2.5/pyrogram/handlers/handler.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/handlers/inline_query_handler.py` & `PyroFork-2.2.5/pyrogram/handlers/inline_query_handler.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/handlers/message_handler.py` & `PyroFork-2.2.5/pyrogram/handlers/message_handler.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/handlers/poll_handler.py` & `PyroFork-2.2.5/pyrogram/handlers/poll_handler.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/handlers/raw_update_handler.py` & `PyroFork-2.2.5/pyrogram/handlers/raw_update_handler.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/handlers/user_status_handler.py` & `PyroFork-2.2.5/pyrogram/handlers/user_status_handler.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/__init__.py` & `PyroFork-2.2.5/pyrogram/methods/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/advanced/__init__.py` & `PyroFork-2.2.5/pyrogram/methods/advanced/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/advanced/invoke.py` & `PyroFork-2.2.5/pyrogram/methods/advanced/invoke.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/advanced/resolve_peer.py` & `PyroFork-2.2.5/pyrogram/methods/advanced/resolve_peer.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/advanced/save_file.py` & `PyroFork-2.2.5/pyrogram/methods/advanced/save_file.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/auth/__init__.py` & `PyroFork-2.2.5/pyrogram/methods/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/auth/accept_terms_of_service.py` & `PyroFork-2.2.5/pyrogram/methods/auth/accept_terms_of_service.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/auth/check_password.py` & `PyroFork-2.2.5/pyrogram/methods/auth/check_password.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/auth/connect.py` & `PyroFork-2.2.5/pyrogram/methods/auth/connect.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/auth/disconnect.py` & `PyroFork-2.2.5/pyrogram/methods/auth/disconnect.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/auth/get_password_hint.py` & `PyroFork-2.2.5/pyrogram/methods/auth/get_password_hint.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/auth/initialize.py` & `PyroFork-2.2.5/pyrogram/methods/auth/initialize.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/auth/log_out.py` & `PyroFork-2.2.5/pyrogram/methods/auth/log_out.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/auth/recover_password.py` & `PyroFork-2.2.5/pyrogram/methods/auth/recover_password.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/auth/resend_code.py` & `PyroFork-2.2.5/pyrogram/methods/auth/resend_code.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/auth/send_code.py` & `PyroFork-2.2.5/pyrogram/methods/auth/send_code.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/auth/send_recovery_code.py` & `PyroFork-2.2.5/pyrogram/methods/auth/send_recovery_code.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/auth/sign_in.py` & `PyroFork-2.2.5/pyrogram/methods/auth/sign_in.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/auth/sign_in_bot.py` & `PyroFork-2.2.5/pyrogram/methods/auth/sign_in_bot.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/auth/sign_up.py` & `PyroFork-2.2.5/pyrogram/methods/auth/sign_up.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/auth/terminate.py` & `PyroFork-2.2.5/pyrogram/methods/auth/terminate.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/bots/__init__.py` & `PyroFork-2.2.5/pyrogram/methods/bots/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/bots/answer_callback_query.py` & `PyroFork-2.2.5/pyrogram/methods/bots/answer_callback_query.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/bots/answer_inline_query.py` & `PyroFork-2.2.5/pyrogram/methods/bots/answer_inline_query.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/bots/answer_web_app_query.py` & `PyroFork-2.2.5/pyrogram/methods/bots/answer_web_app_query.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/bots/delete_bot_commands.py` & `PyroFork-2.2.5/pyrogram/methods/bots/delete_bot_commands.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/bots/get_bot_commands.py` & `PyroFork-2.2.5/pyrogram/methods/bots/get_bot_commands.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/bots/get_bot_default_privileges.py` & `PyroFork-2.2.5/pyrogram/methods/bots/get_bot_default_privileges.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/bots/get_chat_menu_button.py` & `PyroFork-2.2.5/pyrogram/methods/bots/get_chat_menu_button.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/bots/get_game_high_scores.py` & `PyroFork-2.2.5/pyrogram/methods/bots/get_game_high_scores.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/bots/get_inline_bot_results.py` & `PyroFork-2.2.5/pyrogram/methods/bots/get_inline_bot_results.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/bots/request_callback_answer.py` & `PyroFork-2.2.5/pyrogram/methods/bots/request_callback_answer.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/bots/send_game.py` & `PyroFork-2.2.5/pyrogram/methods/bots/send_game.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/bots/send_inline_bot_result.py` & `PyroFork-2.2.5/pyrogram/methods/bots/send_inline_bot_result.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/bots/set_bot_commands.py` & `PyroFork-2.2.5/pyrogram/methods/bots/set_bot_commands.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/bots/set_bot_default_privileges.py` & `PyroFork-2.2.5/pyrogram/methods/bots/set_bot_default_privileges.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/bots/set_chat_menu_button.py` & `PyroFork-2.2.5/pyrogram/methods/bots/set_chat_menu_button.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/bots/set_game_score.py` & `PyroFork-2.2.5/pyrogram/methods/bots/set_game_score.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/chats/__init__.py` & `PyroFork-2.2.5/pyrogram/methods/chats/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/chats/add_chat_members.py` & `PyroFork-2.2.5/pyrogram/methods/chats/add_chat_members.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/chats/archive_chats.py` & `PyroFork-2.2.5/pyrogram/methods/chats/archive_chats.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/chats/ban_chat_member.py` & `PyroFork-2.2.5/pyrogram/methods/chats/ban_chat_member.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/chats/close_forum_topic.py` & `PyroFork-2.2.5/pyrogram/methods/chats/close_forum_topic.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/chats/close_general_topic.py` & `PyroFork-2.2.5/pyrogram/methods/chats/close_general_topic.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/chats/create_channel.py` & `PyroFork-2.2.5/pyrogram/methods/chats/create_channel.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/chats/create_forum_topic.py` & `PyroFork-2.2.5/pyrogram/methods/chats/create_forum_topic.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/chats/create_group.py` & `PyroFork-2.2.5/pyrogram/methods/chats/create_group.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/chats/create_supergroup.py` & `PyroFork-2.2.5/pyrogram/methods/chats/create_supergroup.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/chats/delete_channel.py` & `PyroFork-2.2.5/pyrogram/methods/chats/delete_channel.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/chats/delete_chat_photo.py` & `PyroFork-2.2.5/pyrogram/methods/chats/delete_chat_photo.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/chats/delete_forum_topic.py` & `PyroFork-2.2.5/pyrogram/methods/chats/delete_forum_topic.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/chats/delete_supergroup.py` & `PyroFork-2.2.5/pyrogram/methods/chats/delete_supergroup.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/chats/delete_user_history.py` & `PyroFork-2.2.5/pyrogram/methods/chats/delete_user_history.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/chats/edit_forum_topic.py` & `PyroFork-2.2.5/pyrogram/methods/chats/edit_forum_topic.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/chats/edit_general_topic.py` & `PyroFork-2.2.5/pyrogram/methods/chats/edit_general_topic.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/chats/get_chat.py` & `PyroFork-2.2.5/pyrogram/methods/chats/get_chat.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/chats/get_chat_event_log.py` & `PyroFork-2.2.5/pyrogram/methods/chats/get_chat_event_log.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/chats/get_chat_member.py` & `PyroFork-2.2.5/pyrogram/methods/chats/get_chat_member.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/chats/get_chat_members.py` & `PyroFork-2.2.5/pyrogram/methods/chats/get_chat_members.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/chats/get_chat_members_count.py` & `PyroFork-2.2.5/pyrogram/methods/chats/get_chat_members_count.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/chats/get_chat_online_count.py` & `PyroFork-2.2.5/pyrogram/methods/chats/get_chat_online_count.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/chats/get_dialogs.py` & `PyroFork-2.2.5/pyrogram/methods/chats/get_dialogs.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/chats/get_dialogs_count.py` & `PyroFork-2.2.5/pyrogram/methods/chats/get_dialogs_count.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/chats/get_forum_topics.py` & `PyroFork-2.2.5/pyrogram/methods/chats/get_forum_topics.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/chats/get_forum_topics_by_id.py` & `PyroFork-2.2.5/pyrogram/methods/chats/get_forum_topics_by_id.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/chats/get_nearby_chats.py` & `PyroFork-2.2.5/pyrogram/methods/chats/get_nearby_chats.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/chats/get_send_as_chats.py` & `PyroFork-2.2.5/pyrogram/methods/chats/get_send_as_chats.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/chats/hide_general_topic.py` & `PyroFork-2.2.5/pyrogram/methods/chats/hide_general_topic.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/chats/join_chat.py` & `PyroFork-2.2.5/pyrogram/methods/chats/join_chat.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/chats/leave_chat.py` & `PyroFork-2.2.5/pyrogram/methods/chats/leave_chat.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/chats/mark_chat_unread.py` & `PyroFork-2.2.5/pyrogram/methods/chats/mark_chat_unread.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/chats/pin_chat_message.py` & `PyroFork-2.2.5/pyrogram/methods/chats/pin_chat_message.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/chats/promote_chat_member.py` & `PyroFork-2.2.5/pyrogram/methods/chats/promote_chat_member.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/chats/reopen_forum_topic.py` & `PyroFork-2.2.5/pyrogram/methods/chats/reopen_forum_topic.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/chats/reopen_general_topic.py` & `PyroFork-2.2.5/pyrogram/methods/chats/reopen_general_topic.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/chats/restrict_chat_member.py` & `PyroFork-2.2.5/pyrogram/methods/chats/restrict_chat_member.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/chats/set_administrator_title.py` & `PyroFork-2.2.5/pyrogram/methods/chats/set_administrator_title.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/chats/set_chat_description.py` & `PyroFork-2.2.5/pyrogram/methods/chats/set_chat_description.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/chats/set_chat_permissions.py` & `PyroFork-2.2.5/pyrogram/methods/chats/set_chat_permissions.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/chats/set_chat_photo.py` & `PyroFork-2.2.5/pyrogram/methods/chats/set_chat_photo.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/chats/set_chat_protected_content.py` & `PyroFork-2.2.5/pyrogram/methods/chats/set_chat_protected_content.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/chats/set_chat_title.py` & `PyroFork-2.2.5/pyrogram/methods/chats/set_chat_title.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/chats/set_chat_username.py` & `PyroFork-2.2.5/pyrogram/methods/chats/set_chat_username.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/chats/set_send_as_chat.py` & `PyroFork-2.2.5/pyrogram/methods/chats/set_send_as_chat.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/chats/set_slow_mode.py` & `PyroFork-2.2.5/pyrogram/methods/chats/set_slow_mode.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/chats/unarchive_chats.py` & `PyroFork-2.2.5/pyrogram/methods/chats/unarchive_chats.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/chats/unban_chat_member.py` & `PyroFork-2.2.5/pyrogram/methods/chats/unban_chat_member.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/chats/unhide_general_topic.py` & `PyroFork-2.2.5/pyrogram/methods/chats/unhide_general_topic.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/chats/unpin_all_chat_messages.py` & `PyroFork-2.2.5/pyrogram/methods/chats/unpin_all_chat_messages.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/chats/unpin_chat_message.py` & `PyroFork-2.2.5/pyrogram/methods/chats/unpin_chat_message.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/contacts/__init__.py` & `PyroFork-2.2.5/pyrogram/methods/contacts/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/contacts/add_contact.py` & `PyroFork-2.2.5/pyrogram/methods/contacts/add_contact.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/contacts/delete_contacts.py` & `PyroFork-2.2.5/pyrogram/methods/contacts/delete_contacts.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/contacts/get_contacts.py` & `PyroFork-2.2.5/pyrogram/methods/contacts/get_contacts.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/contacts/get_contacts_count.py` & `PyroFork-2.2.5/pyrogram/methods/contacts/get_contacts_count.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/contacts/import_contacts.py` & `PyroFork-2.2.5/pyrogram/methods/contacts/import_contacts.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/decorators/__init__.py` & `PyroFork-2.2.5/pyrogram/methods/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/decorators/on_callback_query.py` & `PyroFork-2.2.5/pyrogram/methods/decorators/on_callback_query.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/decorators/on_chat_join_request.py` & `PyroFork-2.2.5/pyrogram/methods/decorators/on_chat_join_request.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/decorators/on_chat_member_updated.py` & `PyroFork-2.2.5/pyrogram/methods/decorators/on_chat_member_updated.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/decorators/on_chosen_inline_result.py` & `PyroFork-2.2.5/pyrogram/methods/decorators/on_chosen_inline_result.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/decorators/on_deleted_messages.py` & `PyroFork-2.2.5/pyrogram/methods/decorators/on_deleted_messages.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/decorators/on_disconnect.py` & `PyroFork-2.2.5/pyrogram/methods/decorators/on_disconnect.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/decorators/on_edited_message.py` & `PyroFork-2.2.5/pyrogram/methods/decorators/on_edited_message.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/decorators/on_inline_query.py` & `PyroFork-2.2.5/pyrogram/methods/decorators/on_inline_query.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/decorators/on_message.py` & `PyroFork-2.2.5/pyrogram/methods/decorators/on_message.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/decorators/on_poll.py` & `PyroFork-2.2.5/pyrogram/methods/decorators/on_poll.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/decorators/on_raw_update.py` & `PyroFork-2.2.5/pyrogram/methods/decorators/on_raw_update.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/decorators/on_user_status.py` & `PyroFork-2.2.5/pyrogram/methods/decorators/on_user_status.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/invite_links/__init__.py` & `PyroFork-2.2.5/pyrogram/methods/invite_links/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/invite_links/approve_all_chat_join_requests.py` & `PyroFork-2.2.5/pyrogram/methods/invite_links/approve_all_chat_join_requests.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/invite_links/approve_chat_join_request.py` & `PyroFork-2.2.5/pyrogram/methods/invite_links/approve_chat_join_request.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/invite_links/create_chat_invite_link.py` & `PyroFork-2.2.5/pyrogram/methods/invite_links/create_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/invite_links/decline_all_chat_join_requests.py` & `PyroFork-2.2.5/pyrogram/methods/invite_links/decline_all_chat_join_requests.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/invite_links/decline_chat_join_request.py` & `PyroFork-2.2.5/pyrogram/methods/invite_links/decline_chat_join_request.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/invite_links/delete_chat_admin_invite_links.py` & `PyroFork-2.2.5/pyrogram/methods/invite_links/delete_chat_admin_invite_links.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/invite_links/delete_chat_invite_link.py` & `PyroFork-2.2.5/pyrogram/methods/invite_links/delete_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/invite_links/edit_chat_invite_link.py` & `PyroFork-2.2.5/pyrogram/methods/invite_links/edit_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/invite_links/export_chat_invite_link.py` & `PyroFork-2.2.5/pyrogram/methods/invite_links/export_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/invite_links/get_chat_admin_invite_links.py` & `PyroFork-2.2.5/pyrogram/methods/invite_links/get_chat_admin_invite_links.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/invite_links/get_chat_admin_invite_links_count.py` & `PyroFork-2.2.5/pyrogram/methods/invite_links/get_chat_admin_invite_links_count.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/invite_links/get_chat_admins_with_invite_links.py` & `PyroFork-2.2.5/pyrogram/methods/invite_links/get_chat_admins_with_invite_links.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/invite_links/get_chat_invite_link.py` & `PyroFork-2.2.5/pyrogram/methods/invite_links/get_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/invite_links/get_chat_invite_link_joiners.py` & `PyroFork-2.2.5/pyrogram/methods/invite_links/get_chat_invite_link_joiners.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/invite_links/get_chat_invite_link_joiners_count.py` & `PyroFork-2.2.5/pyrogram/methods/invite_links/get_chat_invite_link_joiners_count.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/invite_links/get_chat_join_requests.py` & `PyroFork-2.2.5/pyrogram/methods/invite_links/get_chat_join_requests.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/invite_links/revoke_chat_invite_link.py` & `PyroFork-2.2.5/pyrogram/methods/invite_links/revoke_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/messages/__init__.py` & `PyroFork-2.2.5/pyrogram/methods/messages/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/messages/copy_media_group.py` & `PyroFork-2.2.5/pyrogram/methods/messages/copy_media_group.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/messages/copy_message.py` & `PyroFork-2.2.5/pyrogram/methods/messages/copy_message.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/messages/delete_messages.py` & `PyroFork-2.2.5/pyrogram/methods/messages/delete_messages.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/messages/download_media.py` & `PyroFork-2.2.5/pyrogram/methods/messages/download_media.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/messages/edit_inline_caption.py` & `PyroFork-2.2.5/pyrogram/methods/messages/edit_inline_caption.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/messages/edit_inline_media.py` & `PyroFork-2.2.5/pyrogram/methods/messages/edit_inline_media.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/messages/edit_inline_reply_markup.py` & `PyroFork-2.2.5/pyrogram/methods/messages/edit_inline_reply_markup.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/messages/edit_inline_text.py` & `PyroFork-2.2.5/pyrogram/methods/messages/edit_inline_text.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/messages/edit_message_caption.py` & `PyroFork-2.2.5/pyrogram/methods/messages/edit_message_caption.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/messages/edit_message_media.py` & `PyroFork-2.2.5/pyrogram/methods/messages/edit_message_media.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/messages/edit_message_reply_markup.py` & `PyroFork-2.2.5/pyrogram/methods/messages/edit_message_reply_markup.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/messages/edit_message_text.py` & `PyroFork-2.2.5/pyrogram/methods/messages/edit_message_text.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/messages/forward_messages.py` & `PyroFork-2.2.5/pyrogram/methods/messages/forward_messages.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/messages/get_chat_history.py` & `PyroFork-2.2.5/pyrogram/methods/messages/get_chat_history.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/messages/get_chat_history_count.py` & `PyroFork-2.2.5/pyrogram/methods/messages/get_chat_history_count.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/messages/get_custom_emoji_stickers.py` & `PyroFork-2.2.5/pyrogram/methods/messages/get_custom_emoji_stickers.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/messages/get_discussion_message.py` & `PyroFork-2.2.5/pyrogram/methods/messages/get_discussion_message.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/messages/get_discussion_replies.py` & `PyroFork-2.2.5/pyrogram/methods/messages/get_discussion_replies.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/messages/get_discussion_replies_count.py` & `PyroFork-2.2.5/pyrogram/methods/messages/get_discussion_replies_count.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/messages/get_media_group.py` & `PyroFork-2.2.5/pyrogram/methods/messages/get_media_group.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/messages/get_messages.py` & `PyroFork-2.2.5/pyrogram/methods/messages/get_messages.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/messages/inline_session.py` & `PyroFork-2.2.5/pyrogram/methods/messages/inline_session.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/messages/read_chat_history.py` & `PyroFork-2.2.5/pyrogram/methods/messages/read_chat_history.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/messages/retract_vote.py` & `PyroFork-2.2.5/pyrogram/methods/messages/retract_vote.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/messages/search_global.py` & `PyroFork-2.2.5/pyrogram/methods/messages/search_global.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/messages/search_global_count.py` & `PyroFork-2.2.5/pyrogram/methods/messages/search_global_count.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/messages/search_messages.py` & `PyroFork-2.2.5/pyrogram/methods/messages/search_messages.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/messages/search_messages_count.py` & `PyroFork-2.2.5/pyrogram/methods/messages/search_messages_count.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/messages/send_animation.py` & `PyroFork-2.2.5/pyrogram/methods/messages/send_animation.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/messages/send_audio.py` & `PyroFork-2.2.5/pyrogram/methods/messages/send_audio.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/messages/send_cached_media.py` & `PyroFork-2.2.5/pyrogram/methods/messages/send_cached_media.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/messages/send_chat_action.py` & `PyroFork-2.2.5/pyrogram/methods/messages/send_chat_action.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/messages/send_contact.py` & `PyroFork-2.2.5/pyrogram/methods/messages/send_contact.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/messages/send_dice.py` & `PyroFork-2.2.5/pyrogram/methods/messages/send_dice.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/messages/send_document.py` & `PyroFork-2.2.5/pyrogram/methods/messages/send_document.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/messages/send_location.py` & `PyroFork-2.2.5/pyrogram/methods/messages/send_location.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/messages/send_media_group.py` & `PyroFork-2.2.5/pyrogram/methods/messages/send_media_group.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/messages/send_message.py` & `PyroFork-2.2.5/pyrogram/methods/messages/send_message.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/messages/send_photo.py` & `PyroFork-2.2.5/pyrogram/methods/messages/send_photo.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/messages/send_poll.py` & `PyroFork-2.2.5/pyrogram/methods/messages/send_poll.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/messages/send_reaction.py` & `PyroFork-2.2.5/pyrogram/methods/messages/send_reaction.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/messages/send_sticker.py` & `PyroFork-2.2.5/pyrogram/methods/messages/send_sticker.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/messages/send_venue.py` & `PyroFork-2.2.5/pyrogram/methods/messages/send_venue.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/messages/send_video.py` & `PyroFork-2.2.5/pyrogram/methods/messages/send_video.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/messages/send_video_note.py` & `PyroFork-2.2.5/pyrogram/methods/messages/send_video_note.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/messages/send_voice.py` & `PyroFork-2.2.5/pyrogram/methods/messages/send_voice.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/messages/stop_poll.py` & `PyroFork-2.2.5/pyrogram/methods/messages/stop_poll.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/messages/stream_media.py` & `PyroFork-2.2.5/pyrogram/methods/messages/stream_media.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/messages/vote_poll.py` & `PyroFork-2.2.5/pyrogram/methods/messages/vote_poll.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/password/__init__.py` & `PyroFork-2.2.5/pyrogram/methods/password/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/password/change_cloud_password.py` & `PyroFork-2.2.5/pyrogram/methods/password/change_cloud_password.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/password/enable_cloud_password.py` & `PyroFork-2.2.5/pyrogram/methods/password/enable_cloud_password.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/password/remove_cloud_password.py` & `PyroFork-2.2.5/pyrogram/methods/password/remove_cloud_password.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/stickers/__init__.py` & `PyroFork-2.2.5/pyrogram/methods/stickers/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/stickers/add_sticker_to_set.py` & `PyroFork-2.2.5/pyrogram/methods/stickers/add_sticker_to_set.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/stickers/create_sticker_set.py` & `PyroFork-2.2.5/pyrogram/methods/stickers/create_sticker_set.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/stickers/get_sticker_set.py` & `PyroFork-2.2.5/pyrogram/methods/stickers/get_sticker_set.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/users/__init__.py` & `PyroFork-2.2.5/pyrogram/methods/users/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/users/block_user.py` & `PyroFork-2.2.5/pyrogram/methods/users/block_user.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/users/delete_profile_photos.py` & `PyroFork-2.2.5/pyrogram/methods/users/delete_profile_photos.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/users/get_chat_photos.py` & `PyroFork-2.2.5/pyrogram/methods/users/get_chat_photos.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/users/get_chat_photos_count.py` & `PyroFork-2.2.5/pyrogram/methods/users/get_chat_photos_count.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/users/get_common_chats.py` & `PyroFork-2.2.5/pyrogram/methods/users/get_common_chats.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/users/get_default_emoji_statuses.py` & `PyroFork-2.2.5/pyrogram/methods/users/get_default_emoji_statuses.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/users/get_me.py` & `PyroFork-2.2.5/pyrogram/methods/users/get_me.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/users/get_users.py` & `PyroFork-2.2.5/pyrogram/methods/users/get_users.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/users/set_emoji_status.py` & `PyroFork-2.2.5/pyrogram/methods/users/set_emoji_status.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/users/set_profile_photo.py` & `PyroFork-2.2.5/pyrogram/methods/users/set_profile_photo.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/users/set_username.py` & `PyroFork-2.2.5/pyrogram/methods/users/set_username.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/users/unblock_user.py` & `PyroFork-2.2.5/pyrogram/methods/users/unblock_user.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/users/update_profile.py` & `PyroFork-2.2.5/pyrogram/methods/users/update_profile.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/utilities/__init__.py` & `PyroFork-2.2.5/pyrogram/methods/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/utilities/add_handler.py` & `PyroFork-2.2.5/pyrogram/methods/utilities/add_handler.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/utilities/compose.py` & `PyroFork-2.2.5/pyrogram/methods/utilities/compose.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/utilities/export_session_string.py` & `PyroFork-2.2.5/pyrogram/methods/utilities/export_session_string.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/utilities/idle.py` & `PyroFork-2.2.5/pyrogram/methods/utilities/idle.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/utilities/remove_handler.py` & `PyroFork-2.2.5/pyrogram/methods/utilities/remove_handler.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/utilities/restart.py` & `PyroFork-2.2.5/pyrogram/methods/utilities/restart.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/utilities/run.py` & `PyroFork-2.2.5/pyrogram/methods/utilities/run.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/utilities/run_sync.py` & `PyroFork-2.2.5/pyrogram/methods/utilities/run_sync.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/utilities/start.py` & `PyroFork-2.2.5/pyrogram/methods/utilities/start.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/utilities/stop.py` & `PyroFork-2.2.5/pyrogram/methods/utilities/stop.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/methods/utilities/stop_transmission.py` & `PyroFork-2.2.5/pyrogram/methods/utilities/stop_transmission.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/mime_types.py` & `PyroFork-2.2.5/pyrogram/mime_types.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/parser/__init__.py` & `PyroFork-2.2.5/pyrogram/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/parser/html.py` & `PyroFork-2.2.5/pyrogram/parser/html.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/parser/markdown.py` & `PyroFork-2.2.5/pyrogram/parser/markdown.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/parser/parser.py` & `PyroFork-2.2.5/pyrogram/parser/parser.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/parser/utils.py` & `PyroFork-2.2.5/pyrogram/parser/utils.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/raw/__init__.py` & `PyroFork-2.2.5/pyrogram/raw/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/raw/core/__init__.py` & `PyroFork-2.2.5/pyrogram/raw/core/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/raw/core/future_salt.py` & `PyroFork-2.2.5/pyrogram/raw/core/future_salt.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/raw/core/future_salts.py` & `PyroFork-2.2.5/pyrogram/raw/core/future_salts.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/raw/core/gzip_packed.py` & `PyroFork-2.2.5/pyrogram/raw/core/gzip_packed.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/raw/core/list.py` & `PyroFork-2.2.5/pyrogram/raw/core/list.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/raw/core/message.py` & `PyroFork-2.2.5/pyrogram/raw/core/message.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/raw/core/msg_container.py` & `PyroFork-2.2.5/pyrogram/raw/core/msg_container.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/raw/core/primitives/__init__.py` & `PyroFork-2.2.5/pyrogram/raw/core/primitives/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/raw/core/primitives/bool.py` & `PyroFork-2.2.5/pyrogram/raw/core/primitives/bool.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/raw/core/primitives/bytes.py` & `PyroFork-2.2.5/pyrogram/raw/core/primitives/bytes.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/raw/core/primitives/double.py` & `PyroFork-2.2.5/pyrogram/raw/core/primitives/double.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/raw/core/primitives/int.py` & `PyroFork-2.2.5/pyrogram/raw/core/primitives/int.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/raw/core/primitives/string.py` & `PyroFork-2.2.5/pyrogram/raw/core/primitives/string.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/raw/core/primitives/vector.py` & `PyroFork-2.2.5/pyrogram/raw/core/primitives/vector.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/raw/core/tl_object.py` & `PyroFork-2.2.5/pyrogram/raw/core/tl_object.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/session/__init__.py` & `PyroFork-2.2.5/pyrogram/session/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/session/auth.py` & `PyroFork-2.2.5/pyrogram/session/auth.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/session/internals/__init__.py` & `PyroFork-2.2.5/pyrogram/session/internals/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/session/internals/data_center.py` & `PyroFork-2.2.5/pyrogram/session/internals/data_center.py`

 * *Files 4% similar despite different names*

```diff
@@ -76,8 +76,8 @@
                     ip = cls.PROD_IPV6[dc_id]
             else:
                 if media:
                     ip = cls.PROD_MEDIA.get(dc_id, cls.PROD[dc_id])
                 else:
                     ip = cls.PROD[dc_id]
 
-            return ip, 443
+            return ip, 5222
```

### Comparing `PyroFork-2.2.4/pyrogram/session/internals/msg_factory.py` & `PyroFork-2.2.5/pyrogram/session/internals/msg_factory.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/session/internals/msg_id.py` & `PyroFork-2.2.5/pyrogram/session/internals/msg_id.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/session/internals/seq_no.py` & `PyroFork-2.2.5/pyrogram/session/internals/seq_no.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/session/session.py` & `PyroFork-2.2.5/pyrogram/session/session.py`

 * *Files 4% similar despite different names*

```diff
@@ -282,15 +282,15 @@
 
                 break
 
             self.loop.create_task(self.handle_packet(packet))
 
         log.info("NetworkTask stopped")
 
-    async def send(self, data: TLObject, wait_response: bool = True, timeout: float = WAIT_TIMEOUT):
+    async def send(self, data: TLObject, wait_response: bool = True, timeout: float = WAIT_TIMEOUT, retry: int = 0):
         message = self.msg_factory(data)
         msg_id = message.msg_id
 
         if wait_response:
             self.results[msg_id] = Result()
 
         # Call log.debug twice because calling it once by appending "data" to the previous string (i.e. f"Kind: {data}")
@@ -326,21 +326,32 @@
                 raise TimeoutError
             elif isinstance(result, raw.types.RpcError):
                 if isinstance(data, (raw.functions.InvokeWithoutUpdates, raw.functions.InvokeWithTakeout)):
                     data = data.query
 
                 RPCError.raise_it(result, type(data))
             elif isinstance(result, raw.types.BadMsgNotification):
-                raise BadMsgNotification(result.error_code)
+                if retry > 1:
+                    raise BadMsgNotification(result.error_code)
+
+                self._handle_bad_notification()
+                await self.send(data, wait_response, timeout, retry + 1)
             elif isinstance(result, raw.types.BadServerSalt):
                 self.salt = result.new_server_salt
                 return await self.send(data, wait_response, timeout)
             else:
                 return result
 
+    def _handle_bad_notification(self):
+        new_msg_id = MsgId()
+        if self.stored_msg_ids[len(self.stored_msg_ids)-1] >= new_msg_id:
+            new_msg_id = self.stored_msg_ids[len(self.stored_msg_ids)-1] + 4
+            log.debug("Changing msg_id old=%s new=%s", self.stored_msg_ids[len(self.stored_msg_ids)-1], new_msg_id)
+        self.stored_msg_ids[len(self.stored_msg_ids)-1] = new_msg_id
+
     async def invoke(
         self,
         query: TLObject,
         retries: int = MAX_RETRIES,
         timeout: float = WAIT_TIMEOUT,
         sleep_threshold: float = SLEEP_THRESHOLD
     ):
```

### Comparing `PyroFork-2.2.4/pyrogram/storage/__init__.py` & `PyroFork-2.2.5/pyrogram/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/storage/dummy_client.py` & `PyroFork-2.2.5/pyrogram/storage/dummy_client.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/storage/file_storage.py` & `PyroFork-2.2.5/pyrogram/storage/file_storage.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/storage/memory_storage.py` & `PyroFork-2.2.5/pyrogram/storage/memory_storage.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/storage/mongo_storage.py` & `PyroFork-2.2.5/pyrogram/storage/mongo_storage.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/storage/sqlite/sqlite.py` & `PyroFork-2.2.5/pyrogram/storage/sqlite/sqlite.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/storage/sqlite_storage.py` & `PyroFork-2.2.5/pyrogram/storage/sqlite_storage.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/storage/storage.py` & `PyroFork-2.2.5/pyrogram/storage/storage.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/sync.py` & `PyroFork-2.2.5/pyrogram/sync.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/types/__init__.py` & `PyroFork-2.2.5/pyrogram/types/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/types/authorization/__init__.py` & `PyroFork-2.2.5/pyrogram/types/authorization/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/types/authorization/sent_code.py` & `PyroFork-2.2.5/pyrogram/types/authorization/sent_code.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/types/authorization/terms_of_service.py` & `PyroFork-2.2.5/pyrogram/types/authorization/terms_of_service.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/types/bots_and_keyboards/__init__.py` & `PyroFork-2.2.5/pyrogram/types/bots_and_keyboards/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/types/bots_and_keyboards/bot_command.py` & `PyroFork-2.2.5/pyrogram/types/bots_and_keyboards/bot_command.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/types/bots_and_keyboards/bot_command_scope.py` & `PyroFork-2.2.5/pyrogram/types/bots_and_keyboards/bot_command_scope.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/types/bots_and_keyboards/bot_command_scope_all_chat_administrators.py` & `PyroFork-2.2.5/pyrogram/types/bots_and_keyboards/bot_command_scope_all_chat_administrators.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/types/bots_and_keyboards/bot_command_scope_all_group_chats.py` & `PyroFork-2.2.5/pyrogram/types/bots_and_keyboards/bot_command_scope_all_group_chats.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/types/bots_and_keyboards/bot_command_scope_all_private_chats.py` & `PyroFork-2.2.5/pyrogram/types/bots_and_keyboards/bot_command_scope_all_private_chats.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/types/bots_and_keyboards/bot_command_scope_chat.py` & `PyroFork-2.2.5/pyrogram/types/bots_and_keyboards/bot_command_scope_chat.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_administrators.py` & `PyroFork-2.2.5/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_administrators.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_member.py` & `PyroFork-2.2.5/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_member.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/types/bots_and_keyboards/bot_command_scope_default.py` & `PyroFork-2.2.5/pyrogram/types/bots_and_keyboards/bot_command_scope_default.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/types/bots_and_keyboards/callback_game.py` & `PyroFork-2.2.5/pyrogram/types/bots_and_keyboards/callback_game.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/types/bots_and_keyboards/callback_query.py` & `PyroFork-2.2.5/pyrogram/types/bots_and_keyboards/callback_query.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/types/bots_and_keyboards/force_reply.py` & `PyroFork-2.2.5/pyrogram/types/bots_and_keyboards/force_reply.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/types/bots_and_keyboards/game_high_score.py` & `PyroFork-2.2.5/pyrogram/types/bots_and_keyboards/game_high_score.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/types/bots_and_keyboards/inline_keyboard_button.py` & `PyroFork-2.2.5/pyrogram/types/bots_and_keyboards/inline_keyboard_button.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/types/bots_and_keyboards/inline_keyboard_markup.py` & `PyroFork-2.2.5/pyrogram/types/bots_and_keyboards/inline_keyboard_markup.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/types/bots_and_keyboards/keyboard_button.py` & `PyroFork-2.2.5/pyrogram/types/bots_and_keyboards/keyboard_button.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/types/bots_and_keyboards/login_url.py` & `PyroFork-2.2.5/pyrogram/types/bots_and_keyboards/login_url.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/types/bots_and_keyboards/menu_button.py` & `PyroFork-2.2.5/pyrogram/types/bots_and_keyboards/menu_button.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/types/bots_and_keyboards/menu_button_commands.py` & `PyroFork-2.2.5/pyrogram/types/bots_and_keyboards/menu_button_commands.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/types/bots_and_keyboards/menu_button_default.py` & `PyroFork-2.2.5/pyrogram/types/bots_and_keyboards/menu_button_default.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/types/bots_and_keyboards/menu_button_web_app.py` & `PyroFork-2.2.5/pyrogram/types/bots_and_keyboards/menu_button_web_app.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/types/bots_and_keyboards/reply_keyboard_markup.py` & `PyroFork-2.2.5/pyrogram/types/bots_and_keyboards/reply_keyboard_markup.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/types/bots_and_keyboards/reply_keyboard_remove.py` & `PyroFork-2.2.5/pyrogram/types/bots_and_keyboards/reply_keyboard_remove.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/types/bots_and_keyboards/sent_web_app_message.py` & `PyroFork-2.2.5/pyrogram/types/bots_and_keyboards/sent_web_app_message.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/types/bots_and_keyboards/web_app_info.py` & `PyroFork-2.2.5/pyrogram/types/bots_and_keyboards/web_app_info.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/types/inline_mode/__init__.py` & `PyroFork-2.2.5/pyrogram/types/inline_mode/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/types/inline_mode/chosen_inline_result.py` & `PyroFork-2.2.5/pyrogram/types/inline_mode/chosen_inline_result.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/types/inline_mode/inline_query.py` & `PyroFork-2.2.5/pyrogram/types/inline_mode/inline_query.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/types/inline_mode/inline_query_result.py` & `PyroFork-2.2.5/pyrogram/types/inline_mode/inline_query_result.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/types/inline_mode/inline_query_result_animation.py` & `PyroFork-2.2.5/pyrogram/types/inline_mode/inline_query_result_animation.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/types/inline_mode/inline_query_result_article.py` & `PyroFork-2.2.5/pyrogram/types/inline_mode/inline_query_result_article.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/types/inline_mode/inline_query_result_audio.py` & `PyroFork-2.2.5/pyrogram/types/inline_mode/inline_query_result_audio.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/types/inline_mode/inline_query_result_cached_animation.py` & `PyroFork-2.2.5/pyrogram/types/inline_mode/inline_query_result_cached_animation.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/types/inline_mode/inline_query_result_cached_audio.py` & `PyroFork-2.2.5/pyrogram/types/inline_mode/inline_query_result_cached_audio.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/types/inline_mode/inline_query_result_cached_document.py` & `PyroFork-2.2.5/pyrogram/types/inline_mode/inline_query_result_cached_document.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/types/inline_mode/inline_query_result_cached_photo.py` & `PyroFork-2.2.5/pyrogram/types/inline_mode/inline_query_result_cached_photo.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/types/inline_mode/inline_query_result_cached_sticker.py` & `PyroFork-2.2.5/pyrogram/types/inline_mode/inline_query_result_cached_sticker.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/types/inline_mode/inline_query_result_cached_video.py` & `PyroFork-2.2.5/pyrogram/types/inline_mode/inline_query_result_cached_video.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/types/inline_mode/inline_query_result_cached_voice.py` & `PyroFork-2.2.5/pyrogram/types/inline_mode/inline_query_result_cached_voice.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/types/inline_mode/inline_query_result_contact.py` & `PyroFork-2.2.5/pyrogram/types/inline_mode/inline_query_result_contact.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/types/inline_mode/inline_query_result_document.py` & `PyroFork-2.2.5/pyrogram/types/inline_mode/inline_query_result_document.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/types/inline_mode/inline_query_result_location.py` & `PyroFork-2.2.5/pyrogram/types/inline_mode/inline_query_result_location.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/types/inline_mode/inline_query_result_photo.py` & `PyroFork-2.2.5/pyrogram/types/inline_mode/inline_query_result_photo.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/types/inline_mode/inline_query_result_venue.py` & `PyroFork-2.2.5/pyrogram/types/inline_mode/inline_query_result_venue.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/types/inline_mode/inline_query_result_video.py` & `PyroFork-2.2.5/pyrogram/types/inline_mode/inline_query_result_video.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/types/inline_mode/inline_query_result_voice.py` & `PyroFork-2.2.5/pyrogram/types/inline_mode/inline_query_result_voice.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/types/input_media/__init__.py` & `PyroFork-2.2.5/pyrogram/types/input_media/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/types/input_media/input_media.py` & `PyroFork-2.2.5/pyrogram/types/input_media/input_media.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/types/input_media/input_media_animation.py` & `PyroFork-2.2.5/pyrogram/types/input_media/input_media_animation.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/types/input_media/input_media_audio.py` & `PyroFork-2.2.5/pyrogram/types/input_media/input_media_audio.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/types/input_media/input_media_document.py` & `PyroFork-2.2.5/pyrogram/types/input_media/input_media_document.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/types/input_media/input_media_photo.py` & `PyroFork-2.2.5/pyrogram/types/input_media/input_media_photo.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/types/input_media/input_media_video.py` & `PyroFork-2.2.5/pyrogram/types/input_media/input_media_video.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/types/input_media/input_phone_contact.py` & `PyroFork-2.2.5/pyrogram/types/input_media/input_phone_contact.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/types/input_message_content/__init__.py` & `PyroFork-2.2.5/pyrogram/types/input_message_content/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/types/input_message_content/input_message_content.py` & `PyroFork-2.2.5/pyrogram/types/input_message_content/input_message_content.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/types/input_message_content/input_text_message_content.py` & `PyroFork-2.2.5/pyrogram/types/input_message_content/input_text_message_content.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/types/list.py` & `PyroFork-2.2.5/pyrogram/types/list.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/types/messages_and_media/__init__.py` & `PyroFork-2.2.5/pyrogram/types/messages_and_media/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/types/messages_and_media/animation.py` & `PyroFork-2.2.5/pyrogram/types/messages_and_media/animation.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/types/messages_and_media/audio.py` & `PyroFork-2.2.5/pyrogram/types/messages_and_media/audio.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/types/messages_and_media/contact.py` & `PyroFork-2.2.5/pyrogram/types/messages_and_media/contact.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/types/messages_and_media/dice.py` & `PyroFork-2.2.5/pyrogram/types/messages_and_media/dice.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/types/messages_and_media/document.py` & `PyroFork-2.2.5/pyrogram/types/messages_and_media/document.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/types/messages_and_media/game.py` & `PyroFork-2.2.5/pyrogram/types/messages_and_media/game.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/types/messages_and_media/location.py` & `PyroFork-2.2.5/pyrogram/types/messages_and_media/location.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/types/messages_and_media/message.py` & `PyroFork-2.2.5/pyrogram/types/messages_and_media/message.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/types/messages_and_media/message_entity.py` & `PyroFork-2.2.5/pyrogram/types/messages_and_media/message_entity.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/types/messages_and_media/message_reactions.py` & `PyroFork-2.2.5/pyrogram/types/messages_and_media/message_reactions.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/types/messages_and_media/photo.py` & `PyroFork-2.2.5/pyrogram/types/messages_and_media/photo.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/types/messages_and_media/poll.py` & `PyroFork-2.2.5/pyrogram/types/messages_and_media/poll.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/types/messages_and_media/poll_option.py` & `PyroFork-2.2.5/pyrogram/types/messages_and_media/poll_option.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/types/messages_and_media/reaction.py` & `PyroFork-2.2.5/pyrogram/types/messages_and_media/reaction.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/types/messages_and_media/sticker.py` & `PyroFork-2.2.5/pyrogram/types/messages_and_media/sticker.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/types/messages_and_media/stickerset.py` & `PyroFork-2.2.5/pyrogram/types/messages_and_media/stickerset.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/types/messages_and_media/stripped_thumbnail.py` & `PyroFork-2.2.5/pyrogram/types/messages_and_media/stripped_thumbnail.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/types/messages_and_media/thumbnail.py` & `PyroFork-2.2.5/pyrogram/types/messages_and_media/thumbnail.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/types/messages_and_media/venue.py` & `PyroFork-2.2.5/pyrogram/types/messages_and_media/venue.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/types/messages_and_media/video.py` & `PyroFork-2.2.5/pyrogram/types/messages_and_media/video.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/types/messages_and_media/video_note.py` & `PyroFork-2.2.5/pyrogram/types/messages_and_media/video_note.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/types/messages_and_media/voice.py` & `PyroFork-2.2.5/pyrogram/types/messages_and_media/voice.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/types/messages_and_media/web_app_data.py` & `PyroFork-2.2.5/pyrogram/types/messages_and_media/web_app_data.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/types/messages_and_media/web_page.py` & `PyroFork-2.2.5/pyrogram/types/messages_and_media/web_page.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/types/object.py` & `PyroFork-2.2.5/pyrogram/types/object.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/types/update.py` & `PyroFork-2.2.5/pyrogram/types/update.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/types/user_and_chats/__init__.py` & `PyroFork-2.2.5/pyrogram/types/user_and_chats/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/types/user_and_chats/chat.py` & `PyroFork-2.2.5/pyrogram/types/user_and_chats/chat.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/types/user_and_chats/chat_admin_with_invite_links.py` & `PyroFork-2.2.5/pyrogram/types/user_and_chats/chat_admin_with_invite_links.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/types/user_and_chats/chat_event.py` & `PyroFork-2.2.5/pyrogram/types/user_and_chats/chat_event.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/types/user_and_chats/chat_event_filter.py` & `PyroFork-2.2.5/pyrogram/types/user_and_chats/chat_event_filter.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/types/user_and_chats/chat_invite_link.py` & `PyroFork-2.2.5/pyrogram/types/user_and_chats/chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/types/user_and_chats/chat_join_request.py` & `PyroFork-2.2.5/pyrogram/types/user_and_chats/chat_join_request.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/types/user_and_chats/chat_joined_by_request.py` & `PyroFork-2.2.5/pyrogram/types/user_and_chats/chat_joined_by_request.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/types/user_and_chats/chat_joiner.py` & `PyroFork-2.2.5/pyrogram/types/user_and_chats/chat_joiner.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/types/user_and_chats/chat_member.py` & `PyroFork-2.2.5/pyrogram/types/user_and_chats/chat_member.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/types/user_and_chats/chat_member_updated.py` & `PyroFork-2.2.5/pyrogram/types/user_and_chats/chat_member_updated.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/types/user_and_chats/chat_permissions.py` & `PyroFork-2.2.5/pyrogram/types/user_and_chats/chat_permissions.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/types/user_and_chats/chat_photo.py` & `PyroFork-2.2.5/pyrogram/types/user_and_chats/chat_photo.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/types/user_and_chats/chat_preview.py` & `PyroFork-2.2.5/pyrogram/types/user_and_chats/chat_preview.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/types/user_and_chats/chat_privileges.py` & `PyroFork-2.2.5/pyrogram/types/user_and_chats/chat_privileges.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/types/user_and_chats/chat_reactions.py` & `PyroFork-2.2.5/pyrogram/types/user_and_chats/chat_reactions.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/types/user_and_chats/dialog.py` & `PyroFork-2.2.5/pyrogram/types/user_and_chats/dialog.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/types/user_and_chats/emoji_status.py` & `PyroFork-2.2.5/pyrogram/types/user_and_chats/emoji_status.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/types/user_and_chats/forum_topic.py` & `PyroFork-2.2.5/pyrogram/types/user_and_chats/forum_topic.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/types/user_and_chats/forum_topic_closed.py` & `PyroFork-2.2.5/pyrogram/types/user_and_chats/forum_topic_closed.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/types/user_and_chats/forum_topic_created.py` & `PyroFork-2.2.5/pyrogram/types/user_and_chats/forum_topic_created.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/types/user_and_chats/forum_topic_edited.py` & `PyroFork-2.2.5/pyrogram/types/user_and_chats/forum_topic_edited.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/types/user_and_chats/forum_topic_reopened.py` & `PyroFork-2.2.5/pyrogram/types/user_and_chats/forum_topic_reopened.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/types/user_and_chats/general_forum_topic_hidden.py` & `PyroFork-2.2.5/pyrogram/types/user_and_chats/general_forum_topic_hidden.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/types/user_and_chats/general_forum_topic_unhidden.py` & `PyroFork-2.2.5/pyrogram/types/user_and_chats/general_forum_topic_unhidden.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/types/user_and_chats/invite_link_importer.py` & `PyroFork-2.2.5/pyrogram/types/user_and_chats/invite_link_importer.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/types/user_and_chats/peer_channel.py` & `PyroFork-2.2.5/pyrogram/types/user_and_chats/peer_channel.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/types/user_and_chats/peer_user.py` & `PyroFork-2.2.5/pyrogram/types/user_and_chats/peer_user.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/types/user_and_chats/restriction.py` & `PyroFork-2.2.5/pyrogram/types/user_and_chats/restriction.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/types/user_and_chats/user.py` & `PyroFork-2.2.5/pyrogram/types/user_and_chats/user.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/types/user_and_chats/username.py` & `PyroFork-2.2.5/pyrogram/types/user_and_chats/username.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/types/user_and_chats/video_chat_ended.py` & `PyroFork-2.2.5/pyrogram/types/user_and_chats/video_chat_ended.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/types/user_and_chats/video_chat_members_invited.py` & `PyroFork-2.2.5/pyrogram/types/user_and_chats/video_chat_members_invited.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/types/user_and_chats/video_chat_scheduled.py` & `PyroFork-2.2.5/pyrogram/types/user_and_chats/video_chat_scheduled.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/types/user_and_chats/video_chat_started.py` & `PyroFork-2.2.5/pyrogram/types/user_and_chats/video_chat_started.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/pyrogram/utils.py` & `PyroFork-2.2.5/pyrogram/utils.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/setup.py` & `PyroFork-2.2.5/setup.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/tests/__init__.py` & `PyroFork-2.2.5/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/tests/filters/__init__.py` & `PyroFork-2.2.5/tests/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/tests/filters/test_command.py` & `PyroFork-2.2.5/tests/filters/test_command.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/tests/parser/__init__.py` & `PyroFork-2.2.5/tests/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/tests/parser/test_html.py` & `PyroFork-2.2.5/tests/parser/test_html.py`

 * *Files identical despite different names*

### Comparing `PyroFork-2.2.4/tests/test_file_id.py` & `PyroFork-2.2.5/tests/test_file_id.py`

 * *Files identical despite different names*

